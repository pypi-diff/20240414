# Comparing `tmp/medimage_pkg-0.9.2.tar.gz` & `tmp/medimage_pkg-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medimage_pkg-0.9.2.tar", max compression
+gzip compressed data, was "medimage_pkg-0.9.3.tar", max compression
```

## Comparing `medimage_pkg-0.9.2.tar` & `medimage_pkg-0.9.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    35149 2024-04-06 22:02:39.205950 medimage_pkg-0.9.2/LICENSE.md
--rw-r--r--   0        0        0    76226 2024-04-06 22:02:39.205950 medimage_pkg-0.9.2/MEDimage/MEDscan.py
--rw-r--r--   0        0        0      565 2024-04-07 17:23:29.310526 medimage_pkg-0.9.2/MEDimage/__init__.py
--rw-r--r--   0        0        0    31152 2024-04-06 22:02:39.205950 medimage_pkg-0.9.2/MEDimage/biomarkers/BatchExtractor.py
--rw-r--r--   0        0        0    33266 2024-04-06 22:02:39.205950 medimage_pkg-0.9.2/MEDimage/biomarkers/BatchExtractorTexturalFilters.py
--rw-r--r--   0        0        0      417 2024-04-06 22:02:39.205950 medimage_pkg-0.9.2/MEDimage/biomarkers/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-06 22:02:39.205950 medimage_pkg-0.9.2/MEDimage/biomarkers/diagnostics.py
--rwxr-xr-x   0        0        0     4979 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/get_oriented_bound_box.py
--rwxr-xr-x   0        0        0    68346 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/glcm.py
--rwxr-xr-x   0        0        0    19443 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/gldzm.py
--rwxr-xr-x   0        0        0    55673 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/glrlm.py
--rwxr-xr-x   0        0        0    18564 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/glszm.py
--rwxr-xr-x   0        0        0    19481 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/int_vol_hist.py
--rwxr-xr-x   0        0        0    22494 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/intensity_histogram.py
--rwxr-xr-x   0        0        0     3488 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/local_intensity.py
--rwxr-xr-x   0        0        0    69854 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/morph.py
--rwxr-xr-x   0        0        0    28146 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/ngldm.py
--rwxr-xr-x   0        0        0    16450 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/ngtdm.py
--rwxr-xr-x   0        0        0    14996 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/stats.py
--rw-r--r--   0        0        0    12357 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/biomarkers/utils.py
--rw-r--r--   0        0        0    11452 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/filters/TexturalFilter.py
--rw-r--r--   0        0        0      198 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/filters/__init__.py
--rw-r--r--   0        0        0     5876 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/filters/apply_filter.py
--rw-r--r--   0        0        0     8879 2024-04-06 22:02:39.209950 medimage_pkg-0.9.2/MEDimage/filters/gabor.py
--rw-r--r--   0        0        0    11336 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/filters/laws.py
--rw-r--r--   0        0        0     5873 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/filters/log.py
--rw-r--r--   0        0        0     4479 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/filters/mean.py
--rw-r--r--   0        0        0    55254 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/filters/textural_filters_kernels.py
--rw-r--r--   0        0        0     4046 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/filters/utils.py
--rw-r--r--   0        0        0     8899 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/filters/wavelet.py
--rw-r--r--   0        0        0     8983 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/DataCleaner.py
--rw-r--r--   0        0        0    22038 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/DesignExperiment.py
--rw-r--r--   0        0        0    29070 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/FSR.py
--rw-r--r--   0        0        0     4611 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/Normalization.py
--rw-r--r--   0        0        0    32824 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/RadiomicsLearner.py
--rw-r--r--   0        0        0   101281 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/Results.py
--rw-r--r--   0        0        0    27090 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/Stats.py
--rw-r--r--   0        0        0      317 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/__init__.py
--rw-r--r--   0        0        0     3955 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/cleaning_utils.py
--rw-r--r--   0        0        0    40944 2024-04-06 22:02:39.213950 medimage_pkg-0.9.2/MEDimage/learning/ml_utils.py
--rw-r--r--   0        0        0      164 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/processing/__init__.py
--rw-r--r--   0        0        0     4273 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/processing/compute_suv_map.py
--rw-r--r--   0        0        0     5354 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/processing/discretisation.py
--rw-r--r--   0        0        0    13092 2024-04-07 17:16:00.850458 medimage_pkg-0.9.2/MEDimage/processing/interpolation.py
--rw-r--r--   0        0        0     1897 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/processing/resegmentation.py
--rw-r--r--   0        0        0    37451 2024-04-07 17:15:47.690455 medimage_pkg-0.9.2/MEDimage/processing/segmentation.py
--rw-r--r--   0        0        0      782 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/__init__.py
--rw-r--r--   0        0        0     1537 2024-04-07 16:32:39.073438 medimage_pkg-0.9.2/MEDimage/utils/batch_patients.py
--rw-r--r--   0        0        0     5317 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/create_radiomics_table.py
--rw-r--r--   0        0        0     1375 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/data_frame_export.py
--rw-r--r--   0        0        0      398 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/find_process_names.py
--rw-r--r--   0        0        0     1169 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/get_file_paths.py
--rw-r--r--   0        0        0      649 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/get_full_rad_names.py
--rw-r--r--   0        0        0      532 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/get_institutions_from_ids.py
--rw-r--r--   0        0        0      518 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/get_patient_id_from_scan_name.py
--rw-r--r--   0        0        0      674 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/get_patient_names.py
--rw-r--r--   0        0        0      682 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/get_radiomic_names.py
--rw-r--r--   0        0        0      583 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/get_scan_name_from_rad_name.py
--rw-r--r--   0        0        0     1215 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/image_reader_SITK.py
--rw-r--r--   0        0        0      677 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/image_volume_obj.py
--rw-r--r--   0        0        0    15426 2024-04-06 22:02:39.217949 medimage_pkg-0.9.2/MEDimage/utils/imref.py
--rw-r--r--   0        0        0     2779 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/initialize_features_names.py
--rw-r--r--   0        0        0     5667 2024-04-07 17:02:46.701938 medimage_pkg-0.9.2/MEDimage/utils/inpolygon.py
--rw-r--r--   0        0        0     1371 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/interp3.py
--rw-r--r--   0        0        0     2242 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/json_utils.py
--rw-r--r--   0        0        0      928 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/mode.py
--rw-r--r--   0        0        0     2119 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/parse_contour_string.py
--rw-r--r--   0        0        0      801 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/save_MEDscan.py
--rw-r--r--   0        0        0      877 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/strfind.py
--rw-r--r--   0        0        0     6162 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/textureTools.py
--rw-r--r--   0        0        0     2253 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/texture_features_names.py
--rw-r--r--   0        0        0     1537 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/utils/write_radiomics_csv.py
--rw-r--r--   0        0        0    84047 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/wrangling/DataManager.py
--rw-r--r--   0        0        0    24511 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/wrangling/ProcessDICOM.py
--rw-r--r--   0        0        0       71 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/MEDimage/wrangling/__init__.py
--rw-r--r--   0        0        0     9777 2024-04-06 22:02:39.221950 medimage_pkg-0.9.2/README.md
--rw-r--r--   0        0        0     1365 2024-04-07 17:23:09.142525 medimage_pkg-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    11504 1970-01-01 00:00:00.000000 medimage_pkg-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-06 22:02:39.205950 medimage_pkg-0.9.3/LICENSE.md
+-rw-r--r--   0        0        0    76226 2024-04-06 22:02:39.205950 medimage_pkg-0.9.3/MEDimage/MEDscan.py
+-rw-r--r--   0        0        0      565 2024-04-13 22:59:43.270211 medimage_pkg-0.9.3/MEDimage/__init__.py
+-rw-r--r--   0        0        0    31152 2024-04-06 22:02:39.205950 medimage_pkg-0.9.3/MEDimage/biomarkers/BatchExtractor.py
+-rw-r--r--   0        0        0    33266 2024-04-06 22:02:39.205950 medimage_pkg-0.9.3/MEDimage/biomarkers/BatchExtractorTexturalFilters.py
+-rw-r--r--   0        0        0      417 2024-04-06 22:02:39.205950 medimage_pkg-0.9.3/MEDimage/biomarkers/__init__.py
+-rw-r--r--   0        0        0     4199 2024-04-06 22:02:39.205950 medimage_pkg-0.9.3/MEDimage/biomarkers/diagnostics.py
+-rwxr-xr-x   0        0        0     4979 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/get_oriented_bound_box.py
+-rwxr-xr-x   0        0        0    68346 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/glcm.py
+-rwxr-xr-x   0        0        0    19443 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/gldzm.py
+-rwxr-xr-x   0        0        0    55673 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/glrlm.py
+-rwxr-xr-x   0        0        0    18564 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/glszm.py
+-rwxr-xr-x   0        0        0    19481 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/int_vol_hist.py
+-rwxr-xr-x   0        0        0    22494 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/intensity_histogram.py
+-rwxr-xr-x   0        0        0     3488 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/local_intensity.py
+-rwxr-xr-x   0        0        0    69854 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/morph.py
+-rwxr-xr-x   0        0        0    28146 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/ngldm.py
+-rwxr-xr-x   0        0        0    16450 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/ngtdm.py
+-rwxr-xr-x   0        0        0    14996 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/stats.py
+-rw-r--r--   0        0        0    12357 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/biomarkers/utils.py
+-rw-r--r--   0        0        0    11452 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/filters/TexturalFilter.py
+-rw-r--r--   0        0        0      198 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/filters/__init__.py
+-rw-r--r--   0        0        0     5876 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/filters/apply_filter.py
+-rw-r--r--   0        0        0     8879 2024-04-06 22:02:39.209950 medimage_pkg-0.9.3/MEDimage/filters/gabor.py
+-rw-r--r--   0        0        0    11336 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/filters/laws.py
+-rw-r--r--   0        0        0     5873 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/filters/log.py
+-rw-r--r--   0        0        0     4479 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/filters/mean.py
+-rw-r--r--   0        0        0    55254 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/filters/textural_filters_kernels.py
+-rw-r--r--   0        0        0     4046 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/filters/utils.py
+-rw-r--r--   0        0        0     8899 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/filters/wavelet.py
+-rw-r--r--   0        0        0     8983 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/DataCleaner.py
+-rw-r--r--   0        0        0    22038 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/DesignExperiment.py
+-rw-r--r--   0        0        0    29070 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/FSR.py
+-rw-r--r--   0        0        0     4611 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/Normalization.py
+-rw-r--r--   0        0        0    32824 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/RadiomicsLearner.py
+-rw-r--r--   0        0        0   101281 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/Results.py
+-rw-r--r--   0        0        0    27090 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/Stats.py
+-rw-r--r--   0        0        0      317 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/__init__.py
+-rw-r--r--   0        0        0     3955 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/cleaning_utils.py
+-rw-r--r--   0        0        0    40944 2024-04-06 22:02:39.213950 medimage_pkg-0.9.3/MEDimage/learning/ml_utils.py
+-rw-r--r--   0        0        0      164 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/processing/__init__.py
+-rw-r--r--   0        0        0     4273 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/processing/compute_suv_map.py
+-rw-r--r--   0        0        0     5354 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/processing/discretisation.py
+-rw-r--r--   0        0        0    13092 2024-04-07 17:16:00.850458 medimage_pkg-0.9.3/MEDimage/processing/interpolation.py
+-rw-r--r--   0        0        0     1897 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/processing/resegmentation.py
+-rw-r--r--   0        0        0    37451 2024-04-07 17:15:47.690455 medimage_pkg-0.9.3/MEDimage/processing/segmentation.py
+-rw-r--r--   0        0        0      782 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-07 16:32:39.073438 medimage_pkg-0.9.3/MEDimage/utils/batch_patients.py
+-rw-r--r--   0        0        0     5317 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/create_radiomics_table.py
+-rw-r--r--   0        0        0     1375 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/data_frame_export.py
+-rw-r--r--   0        0        0      398 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/find_process_names.py
+-rw-r--r--   0        0        0     1169 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/get_file_paths.py
+-rw-r--r--   0        0        0      649 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/get_full_rad_names.py
+-rw-r--r--   0        0        0      532 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/get_institutions_from_ids.py
+-rw-r--r--   0        0        0      518 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/get_patient_id_from_scan_name.py
+-rw-r--r--   0        0        0      674 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/get_patient_names.py
+-rw-r--r--   0        0        0      682 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/get_radiomic_names.py
+-rw-r--r--   0        0        0      583 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/get_scan_name_from_rad_name.py
+-rw-r--r--   0        0        0     1215 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/image_reader_SITK.py
+-rw-r--r--   0        0        0      677 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/image_volume_obj.py
+-rw-r--r--   0        0        0    15426 2024-04-06 22:02:39.217949 medimage_pkg-0.9.3/MEDimage/utils/imref.py
+-rw-r--r--   0        0        0     2779 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/initialize_features_names.py
+-rw-r--r--   0        0        0     5667 2024-04-07 17:02:46.701938 medimage_pkg-0.9.3/MEDimage/utils/inpolygon.py
+-rw-r--r--   0        0        0     1371 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/interp3.py
+-rw-r--r--   0        0        0     2242 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/json_utils.py
+-rw-r--r--   0        0        0      928 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/mode.py
+-rw-r--r--   0        0        0     2119 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/parse_contour_string.py
+-rw-r--r--   0        0        0      801 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/save_MEDscan.py
+-rw-r--r--   0        0        0      877 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/strfind.py
+-rw-r--r--   0        0        0     6162 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/textureTools.py
+-rw-r--r--   0        0        0     2253 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/texture_features_names.py
+-rw-r--r--   0        0        0     1537 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/utils/write_radiomics_csv.py
+-rw-r--r--   0        0        0    84492 2024-04-13 22:47:50.078020 medimage_pkg-0.9.3/MEDimage/wrangling/DataManager.py
+-rw-r--r--   0        0        0    24511 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/wrangling/ProcessDICOM.py
+-rw-r--r--   0        0        0       71 2024-04-06 22:02:39.221950 medimage_pkg-0.9.3/MEDimage/wrangling/__init__.py
+-rw-r--r--   0        0        0     9632 2024-04-07 19:47:46.976864 medimage_pkg-0.9.3/README.md
+-rw-r--r--   0        0        0     1401 2024-04-14 00:30:32.647459 medimage_pkg-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 medimage_pkg-0.9.3/PKG-INFO
```

### Comparing `medimage_pkg-0.9.2/LICENSE.md` & `medimage_pkg-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/MEDscan.py` & `medimage_pkg-0.9.3/MEDimage/MEDscan.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/__init__.py` & `medimage_pkg-0.9.3/MEDimage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 
 stream_handler = logging.StreamHandler()
 stream_handler.setLevel(logging.WARNING)
 logging.getLogger(__name__).addHandler(stream_handler)
 
 __author__ = "MEDomicsLab consortium"
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 __copyright__ = "Copyright (C) MEDomicsLab consortium"
 __license__ = "GNU General Public License 3.0"
 __maintainer__ = "MAHDI AIT LHAJ LOUTFI"
 __email__ = "medomics.info@gmail.com"
```

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/BatchExtractor.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/BatchExtractor.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/BatchExtractorTexturalFilters.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/BatchExtractorTexturalFilters.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/diagnostics.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/diagnostics.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/get_oriented_bound_box.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/get_oriented_bound_box.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/glcm.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/glcm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/gldzm.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/gldzm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/glrlm.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/glrlm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/glszm.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/glszm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/int_vol_hist.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/int_vol_hist.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/intensity_histogram.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/intensity_histogram.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/local_intensity.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/local_intensity.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/morph.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/morph.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/ngldm.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/ngldm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/ngtdm.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/ngtdm.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/stats.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/stats.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/biomarkers/utils.py` & `medimage_pkg-0.9.3/MEDimage/biomarkers/utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/TexturalFilter.py` & `medimage_pkg-0.9.3/MEDimage/filters/TexturalFilter.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/apply_filter.py` & `medimage_pkg-0.9.3/MEDimage/filters/apply_filter.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/gabor.py` & `medimage_pkg-0.9.3/MEDimage/filters/gabor.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/laws.py` & `medimage_pkg-0.9.3/MEDimage/filters/laws.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/log.py` & `medimage_pkg-0.9.3/MEDimage/filters/log.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/mean.py` & `medimage_pkg-0.9.3/MEDimage/filters/mean.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/textural_filters_kernels.py` & `medimage_pkg-0.9.3/MEDimage/filters/textural_filters_kernels.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/utils.py` & `medimage_pkg-0.9.3/MEDimage/filters/utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/filters/wavelet.py` & `medimage_pkg-0.9.3/MEDimage/filters/wavelet.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/DataCleaner.py` & `medimage_pkg-0.9.3/MEDimage/learning/DataCleaner.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/DesignExperiment.py` & `medimage_pkg-0.9.3/MEDimage/learning/DesignExperiment.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/FSR.py` & `medimage_pkg-0.9.3/MEDimage/learning/FSR.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/Normalization.py` & `medimage_pkg-0.9.3/MEDimage/learning/Normalization.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/RadiomicsLearner.py` & `medimage_pkg-0.9.3/MEDimage/learning/RadiomicsLearner.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/Results.py` & `medimage_pkg-0.9.3/MEDimage/learning/Results.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/Stats.py` & `medimage_pkg-0.9.3/MEDimage/learning/Stats.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/cleaning_utils.py` & `medimage_pkg-0.9.3/MEDimage/learning/cleaning_utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/learning/ml_utils.py` & `medimage_pkg-0.9.3/MEDimage/learning/ml_utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/processing/compute_suv_map.py` & `medimage_pkg-0.9.3/MEDimage/processing/compute_suv_map.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/processing/discretisation.py` & `medimage_pkg-0.9.3/MEDimage/processing/discretisation.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/processing/interpolation.py` & `medimage_pkg-0.9.3/MEDimage/processing/interpolation.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/processing/resegmentation.py` & `medimage_pkg-0.9.3/MEDimage/processing/resegmentation.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/processing/segmentation.py` & `medimage_pkg-0.9.3/MEDimage/processing/segmentation.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/__init__.py` & `medimage_pkg-0.9.3/MEDimage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/batch_patients.py` & `medimage_pkg-0.9.3/MEDimage/utils/batch_patients.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/create_radiomics_table.py` & `medimage_pkg-0.9.3/MEDimage/utils/create_radiomics_table.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/data_frame_export.py` & `medimage_pkg-0.9.3/MEDimage/utils/data_frame_export.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/get_file_paths.py` & `medimage_pkg-0.9.3/MEDimage/utils/get_file_paths.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/get_full_rad_names.py` & `medimage_pkg-0.9.3/MEDimage/utils/get_full_rad_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/get_institutions_from_ids.py` & `medimage_pkg-0.9.3/MEDimage/utils/get_institutions_from_ids.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/get_patient_id_from_scan_name.py` & `medimage_pkg-0.9.3/MEDimage/utils/get_patient_id_from_scan_name.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/get_patient_names.py` & `medimage_pkg-0.9.3/MEDimage/utils/get_patient_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/get_radiomic_names.py` & `medimage_pkg-0.9.3/MEDimage/utils/get_radiomic_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/get_scan_name_from_rad_name.py` & `medimage_pkg-0.9.3/MEDimage/utils/get_scan_name_from_rad_name.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/image_reader_SITK.py` & `medimage_pkg-0.9.3/MEDimage/utils/image_reader_SITK.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/image_volume_obj.py` & `medimage_pkg-0.9.3/MEDimage/utils/image_volume_obj.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/imref.py` & `medimage_pkg-0.9.3/MEDimage/utils/imref.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/initialize_features_names.py` & `medimage_pkg-0.9.3/MEDimage/utils/initialize_features_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/inpolygon.py` & `medimage_pkg-0.9.3/MEDimage/utils/inpolygon.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/interp3.py` & `medimage_pkg-0.9.3/MEDimage/utils/interp3.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/json_utils.py` & `medimage_pkg-0.9.3/MEDimage/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/mode.py` & `medimage_pkg-0.9.3/MEDimage/utils/mode.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/parse_contour_string.py` & `medimage_pkg-0.9.3/MEDimage/utils/parse_contour_string.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/save_MEDscan.py` & `medimage_pkg-0.9.3/MEDimage/utils/save_MEDscan.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/strfind.py` & `medimage_pkg-0.9.3/MEDimage/utils/strfind.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/textureTools.py` & `medimage_pkg-0.9.3/MEDimage/utils/textureTools.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/texture_features_names.py` & `medimage_pkg-0.9.3/MEDimage/utils/texture_features_names.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/utils/write_radiomics_csv.py` & `medimage_pkg-0.9.3/MEDimage/utils/write_radiomics_csv.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/MEDimage/wrangling/DataManager.py` & `medimage_pkg-0.9.3/MEDimage/wrangling/DataManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             self, 
             path_to_dicoms: List = [],
             path_to_niftis: List = [],
             path_csv: Union[Path, str] = None,
             path_save: Union[Path, str] = None,
             path_save_checks: Union[Path, str] = None,
             path_pre_checks_settings: Union[Path, str] = None,
-            save: bool = False,
+            save: bool = True,
             n_batch: int = 2
     ) -> None:
         """Constructor of the class DataManager.
 
         Args:
             path_to_dicoms (Union[Path, str], optional): Full path to the starting directory
                 where the DICOM data is located.
@@ -140,15 +140,14 @@
         )
         self.path_to_objects = []
         self.summary = {}
         self.csv_data = None
         self.__studies = []
         self.__institutions = []
         self.__scans = []
-        self.__warned = False
 
     def __find_uid_cell_index(self, uid: Union[str, List[str]], cell: List[str]) -> List: 
         """Finds the cell with the same `uid`. If not is present in `cell`, creates a new position
         in the `cell` for the new `uid`.
 
         Args:
             uid (Union[str, List[str]]):  Unique identifier of the Series to find.
@@ -547,17 +546,26 @@
 
         Args:
             None.
 
         Returns:
             List[MEDscan]: List of MEDscan instances.
         """
+
+        # Reading all NIfTI files
         self.__read_all_niftis()
+
+        # Create the MEDscan instances
         print('--> Reading all NIfTI objects (imaging volumes & masks) to create MEDscan classes')
+        list_instances = []
         for file in tqdm(self.__nifti.stack_path_images):
+            # Assert the list of instances does not exceed the a size of 10
+            if len(list_instances) >= 10:
+                print('The number of MEDscan instances exceeds 10, please consider saving the instances')
+                break
             # INITIALIZE MEDscan INSTANCE AND UPDATE ATTRIBUTES
             medscan = MEDscan()
             medscan.patientID = os.path.basename(file).split("_")[0]
             medscan.type = os.path.basename(file).split(".")[-3]
             medscan.series_description = file.name[file.name.find('__') + 2: file.name.find('(')]
             medscan.format = "nifti"
             medscan.data.set_orientation(orientation="Axial")
@@ -573,14 +581,16 @@
             
             # Get ROI
             medscan = self.__associate_roi_to_image(file, medscan, nib.load(file))
 
             # SAVE MEDscan INSTANCE
             if self.save and self.paths._path_save:
                 save_MEDscan(medscan, self.paths._path_save)
+            else:
+                list_instances.append(medscan)
             
             # Update the path to the created instances
             name_save = self.__get_MEDscan_name_save(medscan)
 
             # Clear memory
             del medscan
 
@@ -607,14 +617,17 @@
                     self.summary[name_save.split('-')[0]][name_save.split('-')[1]][scan_type].append(name_save)
             else:
                 if self.save:
                     logging.warning(f"The patient ID of the following file: {name_save} does not respect the MEDimage "\
                         "naming convention 'study-institution-id' (Ex: Glioma-TCGA-001)")
         print('DONE')
 
+        if list_instances:
+            return list_instances
+
     def update_from_csv(self, path_csv: Union[str, Path] = None) -> None:
         """Updates the class from a given CSV and summarizes the processed scans again according to it.
 
         Args:
             path_csv(optional, Union[str, Path]): Path to a csv file, if not given, will check
                 for csv info in the class attributes.
```

### Comparing `medimage_pkg-0.9.2/MEDimage/wrangling/ProcessDICOM.py` & `medimage_pkg-0.9.3/MEDimage/wrangling/ProcessDICOM.py`

 * *Files identical despite different names*

### Comparing `medimage_pkg-0.9.2/README.md` & `medimage_pkg-0.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/MahdiAll99/MEDimage/dev/docs/figures/MEDimageLogo.png" style="width:150px;"/>
+<img src="https://raw.githubusercontent.com/MEDomics-UdeS/MEDimage/dev/docs/figures/MEDimageLogo.png" style="width:150px;"/>
 
 [![PyPI - Python Version](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 [![TestPyPI - version](https://img.shields.io/badge/pypi-v0.2.0-blue)](https://test.pypi.org/project/medimage-pkg/0.2.0/)
-[![Continuous Integration](https://github.com/MahdiAll99/MEDimage/actions/workflows/python-app.yml/badge.svg)](https://github.com/MahdiAll99/MEDimage/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/MahdiAll99/MEDimage/actions/workflows/python-publish.yml/badge.svg)](https://github.com/MahdiAll99/MEDimage/actions/workflows/python-publish.yml)
+[![Continuous Integration](https://github.com/MEDomics-UdeS/MEDimage/actions/workflows/python-app.yml/badge.svg)](https://github.com/MEDomics-UdeS/MEDimage/actions/workflows/python-app.yml)
 [![Documentation Status](https://readthedocs.org/projects/medimage/badge/?version=latest)](https://medimage.readthedocs.io/en/latest/?badge=latest)
 [![License: GPL-3](https://img.shields.io/badge/license-GPLv3-blue)](LICENSE)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/tutorial/DataManager-Tutorial.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/tutorial/DataManager-Tutorial.ipynb)
 
 </div>
 
 ## Table of Contents
   * [1. Introduction](#1-introduction)
   * [2. Installation](#2-installation)
   * [3. Generating the documentation locally](#3-generating-the-documentation-locally)
@@ -24,26 +23,26 @@
   * [7. Acknowledgement](#7-acknowledgement)
   * [8. Authors](#8-authors)
   * [9. Statement](#9-statement)
 
 ## 1. Introduction
 MEDimage is an open-source Python package that can be used for processing multi-modal medical images (MRI, CT or PET) and for extracting their radiomic features. This package is meant to facilitate the processing of medical images and the subsequent computation of all types of radiomic features while maintaining the reproducibility of analyses. This package has been standardized with the [IBSI](https://theibsi.github.io/) norms.
 
-![MEDimage overview](https://raw.githubusercontent.com/MahdiAll99/MEDimage/main/docs/figures/pakcage-overview.png)
+![MEDimage overview](https://raw.githubusercontent.com/MEDomics-UdeS/MEDimage/main/docs/figures/pakcage-overview.png)
 
 
 ## 2. Installation
 
 ### Python installation
-The MEDimage package requires *Python 3.8* or more. If you don't have it installed on your machine, follow the instructions [here](https://github.com/MahdiAll99/MEDimage/blob/main/python.md) to install it.
+The MEDimage package requires *Python 3.8* or more. If you don't have it installed on your machine, follow the instructions [here](https://github.com/MEDomics-UdeS/MEDimage/blob/main/python.md) to install it.
 
 ### Package installation
 You can easily install the ``MEDimage`` package from PyPI using:
 ```
-pip install MEDimage
+pip install medimage-pkg
 ```
 
 For more installation options (Conda, Poetry...) check out the [installation documentation](https://medimage.readthedocs.io/en/latest/Installation.html).
 
 ## 3. Generating the documentation locally
 The [documentation](https://medimage.readthedocs.io/en/latest/) of the MEDimage package was created using Sphinx. However, you can generate and host it locally by compiling the documentation source code using :
 
@@ -96,30 +95,30 @@
                 roi_type='GrossTumorVolume',
                 roi_type_label='GTV',
             )
 ```
 
 ## 5. Tutorials
 
-We have created many [tutorial notebooks](https://github.com/MahdiAll99/MEDimage/tree/main/notebooks) to assist you in learning how to use the different parts of the package. More details can be found in the [documentation](https://medimage.readthedocs.io/en/latest/tutorials.html).
+We have created many [tutorial notebooks](https://github.com/MEDomics-UdeS/MEDimage/tree/main/notebooks) to assist you in learning how to use the different parts of the package. More details can be found in the [documentation](https://medimage.readthedocs.io/en/latest/tutorials.html).
 
 ## 6. IBSI Standardization
 The image biomarker standardization initiative ([IBSI](https://theibsi.github.io)) is an independent international collaboration that aims to standardize the extraction of image biomarkers from acquired imaging. The IBSI therefore seeks to provide image biomarker nomenclature and definitions, benchmark datasets, and benchmark values to verify image processing and image biomarker calculations, as well as reporting guidelines, for high-throughput image analysis. We participate in this collaboration with our package to make sure it respects international nomenclatures and definitions. The participation was separated into two chapters:
 
   - ### IBSI Chapter 1
-      [The IBSI chapter 1](https://theibsi.github.io/ibsi1/) is dedicated to the standardization of commonly used radiomic features. It was initiated in September 2016 and reached completion in March 2020. We have created two [jupyter notebooks](https://github.com/MahdiAll99/MEDimage/tree/main/notebooks/ibsi) for each phase of the chapter and made them available for the users to run the IBSI tests for themselves. The tests can also be explored in interactive Colab notebooks that are directly accessible here:
+      [The IBSI chapter 1](https://theibsi.github.io/ibsi1/) is dedicated to the standardization of commonly used radiomic features. It was initiated in September 2016 and reached completion in March 2020. We have created two [jupyter notebooks](https://github.com/MEDomics-UdeS/MEDimage/tree/main/notebooks/ibsi) for each phase of the chapter and made them available for the users to run the IBSI tests for themselves. The tests can also be explored in interactive Colab notebooks that are directly accessible here:
       
-      - **Phase 1**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/ibsi/ibsi1p1.ipynb)
-      - **Phase 2**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/ibsi/ibsi1p2.ipynb)
+      - **Phase 1**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/ibsi/ibsi1p1.ipynb)
+      - **Phase 2**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/ibsi/ibsi1p2.ipynb)
 
   - ### IBSI Chapter 2 (In progress)
-      [The IBSI chapter 2](https://theibsi.github.io/ibsi2/) was launched in June 2020 and is still in progress. It is dedicated to the standardization of commonly used imaging filters in radiomic studies. We have created two [jupyter notebooks](https://github.com/MahdiAll99/MEDimage/tree/main/notebooks/ibsi) for each phase of the chapter and made them available for the users to run the IBSI tests for themselves and validate image filtering and image biomarker calculations from filter response maps. The tests can also be explored in interactive Colab notebooks that are directly accessible here: 
+      [The IBSI chapter 2](https://theibsi.github.io/ibsi2/) was launched in June 2020 and is still in progress. It is dedicated to the standardization of commonly used imaging filters in radiomic studies. We have created two [jupyter notebooks](https://github.com/MEDomics-UdeS/MEDimage/tree/main/notebooks/ibsi) for each phase of the chapter and made them available for the users to run the IBSI tests for themselves and validate image filtering and image biomarker calculations from filter response maps. The tests can also be explored in interactive Colab notebooks that are directly accessible here: 
       
-      - **Phase 1**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/ibsi/ibsi2p1.ipynb)
-      - **Phase 2**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/ibsi/ibsi2p2.ipynb)
+      - **Phase 1**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/ibsi/ibsi2p1.ipynb)
+      - **Phase 2**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/ibsi/ibsi2p2.ipynb)
 
       Our team at *UdeS* (a.k.a. Université de Sherbrooke) has already submitted the benchmarked values to the [IBSI uploading website](https://ibsi.radiomics.hevs.ch/).
 
 ---
 **Miscellaneous**
 
 You can avoid the next steps (Jupyter installation and environment setup) if you installed the package using Conda or Poetry according to the documentation.
@@ -173,8 +172,8 @@
 5. If you dare build your business solely from this code, you risk open-sourcing the whole code base.
 6. If you modify it, you have to indicate changes made to the code.
 7. Any modifications of this code base MUST be distributed with the same license, GPLv3.
 8. This software is provided without warranty.
 9. The software author or license can not be held liable for any damages inflicted by the software.
 ```
 
-More information on about the [LICENSE can be found here](https://github.com/MahdiAll99/MEDimage/blob/main/LICENSE.md)
+More information on about the [LICENSE can be found here](https://github.com/MEDomics-UdeS/MEDimage/blob/main/LICENSE.md)
```

### Comparing `medimage_pkg-0.9.2/pyproject.toml` & `medimage_pkg-0.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medimage-pkg"
-version = "0.9.2"
+version = "0.9.3"
 description = "MEDimage is a Python package for processing and extracting features from medical images"
 authors = ["MEDomics Consortium <medomics.info@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/medomics/MEDomicsLab-develop"
 repository = "https://github.com/medomics/MEDomicsLab-develop"
 keywords = ["python", "ibsi", "medical-imaging", 
@@ -28,15 +28,15 @@
 numpyencoder = "*"
 pandas = "<2.0.0"
 Pillow = "*"
 protobuf = "*"
 pycaret = "*"
 pydicom = "<2.0.0"
 PyWavelets = "*"
-ray = "*"
+ray = { version = "*", extras = ["default"] }
 scikit_image = "*"
 scipy = "*"
 setuptools = "*"
 SimpleITK = "*"
 scikit_learn = "*"
 seaborn = "*"
 Sphinx = "*"
```

### Comparing `medimage_pkg-0.9.2/PKG-INFO` & `medimage_pkg-0.9.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medimage-pkg
-Version: 0.9.2
+Version: 0.9.3
 Summary: MEDimage is a Python package for processing and extracting features from medical images
 Home-page: https://github.com/medomics/MEDomicsLab-develop
 License: GPL-3.0
 Keywords: python,ibsi,medical-imaging,cancer-imaging-research,radiomics,medical-image-analysis,features-extraction,radiomics-extraction,radiomics-features,radiomics-analysis
 Author: MEDomics Consortium
 Author-email: medomics.info@gmail.com
 Requires-Python: >=3.8.0,<=3.10
@@ -28,15 +28,15 @@
 Requires-Dist: nilearn
 Requires-Dist: numpy
 Requires-Dist: numpyencoder
 Requires-Dist: pandas (<2.0.0)
 Requires-Dist: protobuf
 Requires-Dist: pycaret
 Requires-Dist: pydicom (<2.0.0)
-Requires-Dist: ray
+Requires-Dist: ray[default]
 Requires-Dist: scikit_image
 Requires-Dist: scikit_learn
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: setuptools
 Requires-Dist: sphinx-carousel (==1.2.0)
 Requires-Dist: sphinx-jsonschema (==1.19.1)
@@ -46,23 +46,22 @@
 Requires-Dist: wget
 Requires-Dist: xgboost
 Project-URL: Repository, https://github.com/medomics/MEDomicsLab-develop
 Description-Content-Type: text/markdown
 
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/MahdiAll99/MEDimage/dev/docs/figures/MEDimageLogo.png" style="width:150px;"/>
+<img src="https://raw.githubusercontent.com/MEDomics-UdeS/MEDimage/dev/docs/figures/MEDimageLogo.png" style="width:150px;"/>
 
 [![PyPI - Python Version](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 [![TestPyPI - version](https://img.shields.io/badge/pypi-v0.2.0-blue)](https://test.pypi.org/project/medimage-pkg/0.2.0/)
-[![Continuous Integration](https://github.com/MahdiAll99/MEDimage/actions/workflows/python-app.yml/badge.svg)](https://github.com/MahdiAll99/MEDimage/actions/workflows/python-app.yml)
-[![Upload Python Package](https://github.com/MahdiAll99/MEDimage/actions/workflows/python-publish.yml/badge.svg)](https://github.com/MahdiAll99/MEDimage/actions/workflows/python-publish.yml)
+[![Continuous Integration](https://github.com/MEDomics-UdeS/MEDimage/actions/workflows/python-app.yml/badge.svg)](https://github.com/MEDomics-UdeS/MEDimage/actions/workflows/python-app.yml)
 [![Documentation Status](https://readthedocs.org/projects/medimage/badge/?version=latest)](https://medimage.readthedocs.io/en/latest/?badge=latest)
 [![License: GPL-3](https://img.shields.io/badge/license-GPLv3-blue)](LICENSE)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/tutorial/DataManager-Tutorial.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/tutorial/DataManager-Tutorial.ipynb)
 
 </div>
 
 ## Table of Contents
   * [1. Introduction](#1-introduction)
   * [2. Installation](#2-installation)
   * [3. Generating the documentation locally](#3-generating-the-documentation-locally)
@@ -74,26 +73,26 @@
   * [7. Acknowledgement](#7-acknowledgement)
   * [8. Authors](#8-authors)
   * [9. Statement](#9-statement)
 
 ## 1. Introduction
 MEDimage is an open-source Python package that can be used for processing multi-modal medical images (MRI, CT or PET) and for extracting their radiomic features. This package is meant to facilitate the processing of medical images and the subsequent computation of all types of radiomic features while maintaining the reproducibility of analyses. This package has been standardized with the [IBSI](https://theibsi.github.io/) norms.
 
-![MEDimage overview](https://raw.githubusercontent.com/MahdiAll99/MEDimage/main/docs/figures/pakcage-overview.png)
+![MEDimage overview](https://raw.githubusercontent.com/MEDomics-UdeS/MEDimage/main/docs/figures/pakcage-overview.png)
 
 
 ## 2. Installation
 
 ### Python installation
-The MEDimage package requires *Python 3.8* or more. If you don't have it installed on your machine, follow the instructions [here](https://github.com/MahdiAll99/MEDimage/blob/main/python.md) to install it.
+The MEDimage package requires *Python 3.8* or more. If you don't have it installed on your machine, follow the instructions [here](https://github.com/MEDomics-UdeS/MEDimage/blob/main/python.md) to install it.
 
 ### Package installation
 You can easily install the ``MEDimage`` package from PyPI using:
 ```
-pip install MEDimage
+pip install medimage-pkg
 ```
 
 For more installation options (Conda, Poetry...) check out the [installation documentation](https://medimage.readthedocs.io/en/latest/Installation.html).
 
 ## 3. Generating the documentation locally
 The [documentation](https://medimage.readthedocs.io/en/latest/) of the MEDimage package was created using Sphinx. However, you can generate and host it locally by compiling the documentation source code using :
 
@@ -146,30 +145,30 @@
                 roi_type='GrossTumorVolume',
                 roi_type_label='GTV',
             )
 ```
 
 ## 5. Tutorials
 
-We have created many [tutorial notebooks](https://github.com/MahdiAll99/MEDimage/tree/main/notebooks) to assist you in learning how to use the different parts of the package. More details can be found in the [documentation](https://medimage.readthedocs.io/en/latest/tutorials.html).
+We have created many [tutorial notebooks](https://github.com/MEDomics-UdeS/MEDimage/tree/main/notebooks) to assist you in learning how to use the different parts of the package. More details can be found in the [documentation](https://medimage.readthedocs.io/en/latest/tutorials.html).
 
 ## 6. IBSI Standardization
 The image biomarker standardization initiative ([IBSI](https://theibsi.github.io)) is an independent international collaboration that aims to standardize the extraction of image biomarkers from acquired imaging. The IBSI therefore seeks to provide image biomarker nomenclature and definitions, benchmark datasets, and benchmark values to verify image processing and image biomarker calculations, as well as reporting guidelines, for high-throughput image analysis. We participate in this collaboration with our package to make sure it respects international nomenclatures and definitions. The participation was separated into two chapters:
 
   - ### IBSI Chapter 1
-      [The IBSI chapter 1](https://theibsi.github.io/ibsi1/) is dedicated to the standardization of commonly used radiomic features. It was initiated in September 2016 and reached completion in March 2020. We have created two [jupyter notebooks](https://github.com/MahdiAll99/MEDimage/tree/main/notebooks/ibsi) for each phase of the chapter and made them available for the users to run the IBSI tests for themselves. The tests can also be explored in interactive Colab notebooks that are directly accessible here:
+      [The IBSI chapter 1](https://theibsi.github.io/ibsi1/) is dedicated to the standardization of commonly used radiomic features. It was initiated in September 2016 and reached completion in March 2020. We have created two [jupyter notebooks](https://github.com/MEDomics-UdeS/MEDimage/tree/main/notebooks/ibsi) for each phase of the chapter and made them available for the users to run the IBSI tests for themselves. The tests can also be explored in interactive Colab notebooks that are directly accessible here:
       
-      - **Phase 1**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/ibsi/ibsi1p1.ipynb)
-      - **Phase 2**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/ibsi/ibsi1p2.ipynb)
+      - **Phase 1**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/ibsi/ibsi1p1.ipynb)
+      - **Phase 2**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/ibsi/ibsi1p2.ipynb)
 
   - ### IBSI Chapter 2 (In progress)
-      [The IBSI chapter 2](https://theibsi.github.io/ibsi2/) was launched in June 2020 and is still in progress. It is dedicated to the standardization of commonly used imaging filters in radiomic studies. We have created two [jupyter notebooks](https://github.com/MahdiAll99/MEDimage/tree/main/notebooks/ibsi) for each phase of the chapter and made them available for the users to run the IBSI tests for themselves and validate image filtering and image biomarker calculations from filter response maps. The tests can also be explored in interactive Colab notebooks that are directly accessible here: 
+      [The IBSI chapter 2](https://theibsi.github.io/ibsi2/) was launched in June 2020 and is still in progress. It is dedicated to the standardization of commonly used imaging filters in radiomic studies. We have created two [jupyter notebooks](https://github.com/MEDomics-UdeS/MEDimage/tree/main/notebooks/ibsi) for each phase of the chapter and made them available for the users to run the IBSI tests for themselves and validate image filtering and image biomarker calculations from filter response maps. The tests can also be explored in interactive Colab notebooks that are directly accessible here: 
       
-      - **Phase 1**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/ibsi/ibsi2p1.ipynb)
-      - **Phase 2**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MahdiAll99/MEDimage/blob/main/notebooks/ibsi/ibsi2p2.ipynb)
+      - **Phase 1**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/ibsi/ibsi2p1.ipynb)
+      - **Phase 2**: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MEDomics-UdeS/MEDimage/blob/main/notebooks/ibsi/ibsi2p2.ipynb)
 
       Our team at *UdeS* (a.k.a. Université de Sherbrooke) has already submitted the benchmarked values to the [IBSI uploading website](https://ibsi.radiomics.hevs.ch/).
 
 ---
 **Miscellaneous**
 
 You can avoid the next steps (Jupyter installation and environment setup) if you installed the package using Conda or Poetry according to the documentation.
@@ -223,9 +222,9 @@
 5. If you dare build your business solely from this code, you risk open-sourcing the whole code base.
 6. If you modify it, you have to indicate changes made to the code.
 7. Any modifications of this code base MUST be distributed with the same license, GPLv3.
 8. This software is provided without warranty.
 9. The software author or license can not be held liable for any damages inflicted by the software.
 ```
 
-More information on about the [LICENSE can be found here](https://github.com/MahdiAll99/MEDimage/blob/main/LICENSE.md)
+More information on about the [LICENSE can be found here](https://github.com/MEDomics-UdeS/MEDimage/blob/main/LICENSE.md)
```

