# Comparing `tmp/static-frame-2.5.2.tar.gz` & `tmp/static-frame-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-2.5.2.tar", last modified: Tue Apr  9 14:10:57 2024, max compression
+gzip compressed data, was "static-frame-2.6.0.tar", last modified: Sun Apr 14 21:01:15 2024, max compression
```

## Comparing `static-frame-2.5.2.tar` & `static-frame-2.6.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.848351 static-frame-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-09 14:10:23.000000 static-frame-2.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 14:10:23.000000 static-frame-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-04-09 14:10:57.848351 static-frame-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23373 2024-04-09 14:10:23.000000 static-frame-2.5.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-09 14:10:23.000000 static-frame-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 14:10:23.000000 static-frame-2.5.2/requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 14:10:23.000000 static-frame-2.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 14:10:57.852351 static-frame-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-09 14:10:23.000000 static-frame-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.824351 static-frame-2.5.2/static_frame/
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.840351 static-frame-2.5.2/static_frame/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/archive_npy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22196 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/archive_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/axis_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    60237 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    53865 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25063 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    74108 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    35749 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display_html_datatables.py
--rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display_visidata.py
--rw-r--r--   0 runner    (1001) docker     (127)    30186 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/doc_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/fill_value_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)   389646 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/generic_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/hloc.py
--rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_correspondence.py
--rw-r--r--   0 runner    (1001) docker     (127)    21797 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)   108897 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_hierarchy_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    50743 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/interface_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    24238 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/loc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/memory_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    36391 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24378 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_fill_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    32552 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_re.py
--rw-r--r--   0 runner    (1001) docker     (127)    21953 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    34568 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_str.py
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/protocol_dfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/protocol_dfi_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    56284 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/quilt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)   130408 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/series.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_client_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7273 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/style_config.py
--rw-r--r--   0 runner    (1001) docker     (127)   182216 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/type_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    60093 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/type_clinic.py
--rw-r--r--   0 runner    (1001) docker     (127)   136685 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/www.py
--rw-r--r--   0 runner    (1001) docker     (127)    29258 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/yarn.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.840351 static-frame-2.5.2/static_frame/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.848351 static-frame-2.5.2/static_frame/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26053 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_archive_npy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_archive_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_axis_map.py
--rw-r--r--   0 runner    (1001) docker     (127)   139072 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    84900 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    37362 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_display_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_fill_value_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)   651135 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_he.py
--rw-r--r--   0 runner    (1001) docker     (127)    60937 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31762 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_via_fill_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_via_re.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_hloc.py
--rw-r--r--   0 runner    (1001) docker     (127)    66981 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_correspondence.py
--rw-r--r--   0 runner    (1001) docker     (127)    41680 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)   166603 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_loc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_memory_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    22679 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_protocol_dfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    75455 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_quilt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)   251061 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_series_he.py
--rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_style_config.py
--rw-r--r--   0 runner    (1001) docker     (127)   161671 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_type_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    69155 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_type_clinic.py
--rw-r--r--   0 runner    (1001) docker     (127)   119583 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_www.py
--rw-r--r--   0 runner    (1001) docker     (127)    48834 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_yarn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.828351 static-frame-2.5.2/static_frame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.174146 static-frame-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-14 21:00:37.000000 static-frame-2.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 21:00:37.000000 static-frame-2.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-04-14 21:01:15.174146 static-frame-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24088 2024-04-14 21:00:37.000000 static-frame-2.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-14 21:00:37.000000 static-frame-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 21:00:37.000000 static-frame-2.6.0/requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 21:00:37.000000 static-frame-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 21:01:15.174146 static-frame-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-14 21:00:37.000000 static-frame-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.150146 static-frame-2.6.0/static_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.162146 static-frame-2.6.0/static_frame/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/archive_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22196 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/archive_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/axis_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60237 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53545 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25063 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74176 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35749 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display_html_datatables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display_visidata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30186 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/doc_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/fill_value_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)   389646 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/generic_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/hloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21797 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109246 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17248 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_hierarchy_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50743 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/interface_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24238 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/loc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/memory_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36391 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24378 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_fill_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32552 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21953 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/protocol_dfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/protocol_dfi_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56284 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/quilt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130410 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_client_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7273 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/style_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182216 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/type_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60093 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/type_clinic.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136804 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/www.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39939 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/yarn.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.162146 static-frame-2.6.0/static_frame/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.174146 static-frame-2.6.0/static_frame/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26053 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_archive_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_archive_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_axis_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139072 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85364 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37362 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_display_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_fill_value_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)   651135 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60937 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31762 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_via_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_hloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66981 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41680 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166603 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_loc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_memory_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22703 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_protocol_dfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75455 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_quilt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)   251061 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_series_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_style_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   161671 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_type_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69155 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_type_clinic.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119583 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_www.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66889 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_yarn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.150146 static-frame-2.6.0/static_frame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-2.5.2/LICENSE.txt` & `static-frame-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/PKG-INFO` & `static-frame-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 2.5.2
+Version: 2.6.0
 Summary: Immutable and statically-typeable DataFrames with runtime type and data validation.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Keywords: staticframe pandas numpy immutable array
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -106,280 +106,282 @@
 ---------------------
 
 To get startred quickly, let's download the classic iris (flower) characteristics data set and build a simple naive Bayes classifier that can predict species from iris petal characteristics.
 
 While StaticFrame's API has over 7,500 endpoints, much will be familiar to users of Pandas or other DataFrame libraries. Rather than offering fewer interfaces with greater configurability, StaticFrame favors more numerous interfaces with more narrow parameters and functionality. This design leads to more maintainable code. (Read more about differences between Pandas and StaticFrame `here <https://static-frame.readthedocs.io/en/latest/articles/upgrade.html>`__.)
 
 
-We can download the data set from the UCI Machine Learning Repository and create a ``Frame``. StaticFrame exposes all constructors on the class: here, we will use the ``Frame.from_csv()`` constructor. To download a file from the internet and provide it to a constructor, we can use StaticFrame's ``WWW.from_file()`` interface.
+We can download the data set from the UCI Machine Learning Repository and create a ``Frame``. StaticFrame exposes all constructors on the class: here, we will use the ``Frame.from_csv()`` constructor. To download a file from the internet and provide it to a constructor, we can use StaticFrame's ``WWW.from_file()`` interface::
 
->>> import static_frame as sf
->>> data = sf.Frame.from_csv(sf.WWW.from_file('https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'), columns_depth=0)
+    >>> import static_frame as sf
+    >>> data = sf.Frame.from_csv(sf.WWW.from_file('https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'), columns_depth=0)
 
 
-Each record (or row) in this dataset describes observations of an iris flower, including its sepal and petal characteristics, as well as its species (of which there are three). To display just the first few rows, we can use the ``head()`` method. Notice that StaticFrame's default display makes it very clear what type of ``Frame``, ``Index``, and NumPy datatypes are present.
+Each record (or row) in this dataset describes observations of an iris flower, including its sepal and petal characteristics, as well as its species (of which there are three). To display just the first few rows, we can use the ``head()`` method. Notice that StaticFrame's default display makes it very clear what type of ``Frame``, ``Index``, and NumPy datatypes are present::
 
->>> data.head()
-<Frame>
-<Index> 0         1         2         3         4           <int64>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-1       4.9       3.0       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
+    >>> data.head()
+    <Frame>
+    <Index> 0         1         2         3         4           <int64>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    1       4.9       3.0       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
 
 As the columns are unlabelled, let's next add column labels. StaticFrame supports reindexing (conforming existing axis labels to new labels, potentially changing the size and ordering) and relabeling (simply applying new labels without regard to existing labels). As we can ignore the default column labels (auto-incremented integers), the ``relabel()`` method is used to provide new labels.
 
-Note that while ``relabel()`` creates a new ``Frame``, underlying NumPy data is not copied. As all NumPy data is immutable in StaticFrame, we can reuse it in our new container, making such operations very efficient. (Read more about no-copy operations `here <https://static-frame.readthedocs.io/en/latest/articles/no_copy.html>`__.)
+Note that while ``relabel()`` creates a new ``Frame``, underlying NumPy data is not copied. As all NumPy data is immutable in StaticFrame, we can reuse it in our new container, making such operations very efficient::
 
+    >>> data = data.relabel(columns=('sepal_l', 'sepal_w', 'petal_l', 'petal_w', 'species'))
+    >>> data.head()
+    <Frame>
+    <Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    1       4.9       3.0       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
->>> data = data.relabel(columns=('sepal_l', 'sepal_w', 'petal_l', 'petal_w', 'species'))
->>> data.head()
-<Frame>
-<Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-1       4.9       3.0       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
 
+(Read more about no-copy operations `here <https://static-frame.readthedocs.io/en/latest/articles/no_copy.html>`__.)
 
 For this example, eighty percent of the data will be used to train the classifier; the remaining twenty percent will be used to test the classifier. As all records are labelled with the known species, we can conclude by measuring the effectiveness of the classifier on the test data.
 
-To divide the data into two groups, we create a ``Series`` of contiguous integers and then extract a random selection of 80% of the values into a new ``Series``, here named ``sel_train``. This will be used to select our traning data. As the ``sample()`` method, given a count, randomly samples that many values, your results will be different unless use the same ``seed`` argument.
+To divide the data into two groups, we create a ``Series`` of contiguous integers and then extract a random selection of 80% of the values into a new ``Series``, here named ``sel_train``. This will be used to select our traning data. As the ``sample()`` method, given a count, randomly samples that many values, your results will be different unless use the same ``seed`` argument::
 
->>> sel = sf.Series(np.arange(len(data)))
->>> sel_train = sel.sample(round(len(data) * .8), seed=42)
->>> sel_train.head()
-<Series>
-<Index>
-0        0
-2        2
-3        3
-4        4
-5        5
-<int64>  <int64>
-
-We will create another ``Series`` to select the test data. The ``drop[]`` interface can be used to create a new ``Series`` that excludes the training selections, leaving just the testing selections. As with many interfaces in StaticFrame (such as ``astype`` and ``assign``), brackets can be used to do ``loc[]`` style selections.
-
->>> sel_test = sel.drop[sel_train]
->>> sel_test.head()
-<Series>
-<Index>
-1        1
-14       14
-20       20
-21       21
-37       37
-<int64>  <int64>
-
-
-To select a subset of the data for training, the ``sel_train`` ``Series`` can be passed to ``loc[]`` to select just those rows.
-
->>> data_train = data.loc[sel_train]
->>> data_train.head()
-<Frame>
-<Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-5       5.4       3.9       1.7       0.4       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
+    >>> sel = sf.Series(np.arange(len(data)))
+    >>> sel_train = sel.sample(round(len(data) * .8), seed=42)
+    >>> sel_train.head()
+    <Series>
+    <Index>
+    0        0
+    2        2
+    3        3
+    4        4
+    5        5
+    <int64>  <int64>
+
+
+We will create another ``Series`` to select the test data. The ``drop[]`` interface can be used to create a new ``Series`` that excludes the training selections, leaving just the testing selections. As with many interfaces in StaticFrame (such as ``astype`` and ``assign``), brackets can be used to do ``loc[]`` style selections::
+
+    >>> sel_test = sel.drop[sel_train]
+    >>> sel_test.head()
+    <Series>
+    <Index>
+    1        1
+    14       14
+    20       20
+    21       21
+    37       37
+    <int64>  <int64>
+
+
+To select a subset of the data for training, the ``sel_train`` ``Series`` can be passed to ``loc[]`` to select just those rows::
+
+    >>> data_train = data.loc[sel_train]
+    >>> data_train.head()
+    <Frame>
+    <Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    5       5.4       3.9       1.7       0.4       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
 
 With our data divided into two randomly-selected, non-overlapping groups, we can proceed to implement the naive Bayes classifier. We will compute the ``posterior`` of the test data by multiplying the ``prior`` and the ``likelihood``. With the ``posterior``, we can determine which species the classifier has calculated is most likely. (More on naive Bayes classifiers can be found `here <https://en.wikipedia.org/wiki/Naive_Bayes_classifier>`__.)
 
 The ``prior`` is calculated as the percentage of samples of each species in the training data. This is the "normalized" count per species. To get a ``Series`` of counts per species, we can select the species column, iterate over groups based on species name, and count the size of each group.
 
 In StaticFrame, this can be done by calling ``Series.iter_group_items()`` to get an iterator of pairs of group label, group (where the group is a ``Series``). This iterator (or any similar iterator) can be given to a ``Batch``, a chaining processor of ``Frame`` or ``Series``, to perform operations on each group. (For more on the ``Batch`` and other higher-order containers in StaticFrame, see `here <https://static-frame.readthedocs.io/en/latest/articles/uhoc.html>`__.)
 
-Once the ``Batch`` is created, selections, method calls, and operator expressions can be chained as if they were being called on a single container. Processing happens to every contained container, and a container is returned, only when a finalizer method, such as ``to_series()``, is called.
+Once the ``Batch`` is created, selections, method calls, and operator expressions can be chained as if they were being called on a single container. Processing happens to every contained container, and a container is returned, only when a finalizer method, such as ``to_series()``, is called::
 
->>> counts = sf.Batch(data_train['species'].iter_group_items()).count().to_series()
->>> counts
-<Series>
-<Index>
-Iris-setosa     43
-Iris-versicolor 39
-Iris-virginica  38
-<<U15>          <int64>
-
-
-As with NumPy, StaticFrame containers can be used in expressions with binary operators. The ``prior`` can be derived by dividing ``counts`` by the size of the training data. This returns a ``Series`` of the percentage of records per species.
-
->>> prior = counts / len(data_train)
->>> prior
-<Series>
-<Index>
-Iris-setosa     0.35833333333333334
-Iris-versicolor 0.325
-Iris-virginica  0.31666666666666665
-<<U15>          <float64>
+    >>> counts = sf.Batch(data_train['species'].iter_group_items()).count().to_series()
+    >>> counts
+    <Series>
+    <Index>
+    Iris-setosa     43
+    Iris-versicolor 39
+    Iris-virginica  38
+    <<U15>          <int64>
+
+
+As with NumPy, StaticFrame containers can be used in expressions with binary operators. The ``prior`` can be derived by dividing ``counts`` by the size of the training data. This returns a ``Series`` of the percentage of records per species::
+
+    >>> prior = counts / len(data_train)
+    >>> prior
+    <Series>
+    <Index>
+    Iris-setosa     0.35833333333333334
+    Iris-versicolor 0.325
+    Iris-virginica  0.31666666666666665
+    <<U15>          <float64>
 
 
 Having calculated the ``prior``, we can calculate ``likelihood`` next. To calculate ``likelihood``, we will call a probability distribution function (imported from SciPy) with the test data, once for each species, given the characteristics (mean and standard deviation) observed in the test data for that species.
 
-The ``Batch`` can again be used to calculate the mean and standard deviation, per species, from the training data. With the ``Frame`` of training data, we call ``iter_group_items()`` to group by species and, passing that iterator to ``Batch``, call ``mean()`` (assigned to ``mu``) or ``std()`` (assigned to ``sigma``). Note that ``iter_group_items()`` has an optional ``drop`` parameter to remove the column used for grouping from subsequent operations.
+The ``Batch`` can again be used to calculate the mean and standard deviation, per species, from the training data. With the ``Frame`` of training data, we call ``iter_group_items()`` to group by species and, passing that iterator to ``Batch``, call ``mean()`` (assigned to ``mu``) or ``std()`` (assigned to ``sigma``). Note that ``iter_group_items()`` has an optional ``drop`` parameter to remove the column used for grouping from subsequent operations::
 
 
->>> mu = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).mean().to_frame()
->>> mu
-<Frame>
-<Index>         sepal_l            sepal_w            <<U7>
-<Index>
-Iris-setosa     4.986046511627907  3.434883720930233
-Iris-versicolor 5.920512820512819  2.771794871794872
-Iris-virginica  6.6078947368421055 2.9763157894736842
-<<U15>          <float64>          <float64>
-
->>> sigma = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).std(ddof=1).to_frame()
->>> sigma
-<Frame>
-<Index>         sepal_l            sepal_w             <<U7>
-<Index>
-Iris-setosa     0.3419700595003668 0.3477024733400345
-Iris-versicolor 0.508444214804487  0.33082728674826684
-Iris-virginica  0.6055516042229233 0.3513942965328924
-<<U15>          <float64>          <float64>
-
-
-For a unified display of these characteristics, we can build a hierarchical index on each ``Frame`` with ``relabel_level_add()`` (adding the "mu" or "sigma" labels), then vertically concatenate the tables. As StaticFrame always requires unique labels in indices, adding an additional label is required before concatenation. The built-in ``round`` function can be used for more tidy display.
-
->>> stats = sf.Frame.from_concat((mu.relabel_level_add('mu'), sigma.relabel_level_add('sigma')))
->>> round(stats, 2)
-<Frame>
-<Index>                          sepal_l   sepal_w   <<U7>
-<IndexHierarchy>
-mu               Iris-setosa     4.99      3.43
-mu               Iris-versicolor 5.92      2.77
-mu               Iris-virginica  6.61      2.98
-sigma            Iris-setosa     0.34      0.35
-sigma            Iris-versicolor 0.51      0.33
-sigma            Iris-virginica  0.61      0.35
-<<U5>            <<U15>          <float64> <float64>
+    >>> mu = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).mean().to_frame()
+    >>> mu
+    <Frame>
+    <Index>         sepal_l            sepal_w            <<U7>
+    <Index>
+    Iris-setosa     4.986046511627907  3.434883720930233
+    Iris-versicolor 5.920512820512819  2.771794871794872
+    Iris-virginica  6.6078947368421055 2.9763157894736842
+    <<U15>          <float64>          <float64>
+
+    >>> sigma = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).std(ddof=1).to_frame()
+    >>> sigma
+    <Frame>
+    <Index>         sepal_l            sepal_w             <<U7>
+    <Index>
+    Iris-setosa     0.3419700595003668 0.3477024733400345
+    Iris-versicolor 0.508444214804487  0.33082728674826684
+    Iris-virginica  0.6055516042229233 0.3513942965328924
+    <<U15>          <float64>          <float64>
+
+
+For a unified display of these characteristics, we can build a hierarchical index on each ``Frame`` with ``relabel_level_add()`` (adding the "mu" or "sigma" labels), then vertically concatenate the tables. As StaticFrame always requires unique labels in indices, adding an additional label is required before concatenation. The built-in ``round`` function can be used for more tidy display::
+
+    >>> stats = sf.Frame.from_concat((mu.relabel_level_add('mu'), sigma.relabel_level_add('sigma')))
+    >>> round(stats, 2)
+    <Frame>
+    <Index>                          sepal_l   sepal_w   <<U7>
+    <IndexHierarchy>
+    mu               Iris-setosa     4.99      3.43
+    mu               Iris-versicolor 5.92      2.77
+    mu               Iris-virginica  6.61      2.98
+    sigma            Iris-setosa     0.34      0.35
+    sigma            Iris-versicolor 0.51      0.33
+    sigma            Iris-virginica  0.61      0.35
+    <<U5>            <<U15>          <float64> <float64>
 
 
 We can now move on to processing the test data with the characteristics derived from the training data. To do that, we will extract our previously selected test records with ``sel_test`` into a new ``Frame``, to which we can add our ``posterior`` predictions and final species classifications.
 
 It is common to process data in table by adding columns from left to right. StaticFrame permits this limited form of mutability with the grow-only ``FrameGO``. While underlying NumPy arrays are still always immutable, columns can be added to a ``FrameGO`` with bracket-style assignments. A ``FrameGO`` can be created from a ``Frame`` with the ``to_frame_go()`` method. As mentioned elsewhere, underlying immutable NumPy arrays are not copied: this is an efficient, no-copy operation.
 
-Passing two arguments to ``loc[]``, we can select rows with the values from ``sel_test``, and we can select columns with a list of labels for the sepal length and sepal width.
+Passing two arguments to ``loc[]``, we can select rows with the values from ``sel_test``, and we can select columns with a list of labels for the sepal length and sepal width::
 
->>> data_test = data.loc[sel_test.values, ['sepal_l', 'sepal_w']].to_frame_go()
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   <<U7>
-<Index>
-1         4.9       3.0
-14        5.8       4.0
-20        5.4       3.4
-21        5.1       3.7
-37        4.9       3.1
-<int64>   <float64> <float64>
+    >>> data_test = data.loc[sel_test.values, ['sepal_l', 'sepal_w']].to_frame_go()
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   <<U7>
+    <Index>
+    1         4.9       3.0
+    14        5.8       4.0
+    20        5.4       3.4
+    21        5.1       3.7
+    37        4.9       3.1
+    <int64>   <float64> <float64>
 
 
 StaticFrame interfaces make extensive use of iterators and generators. As used below, the ``Frame.from_fields()`` constructor will create a ``Frame`` from any iterable (or generator) of column arrays.
 
-The ``likelihood_of_species()`` function (defined below), for each index label in ``mu`` (which provides each unique iris species), calculates a probability density function for the test data, given the ``mu`` (mean) and ``sigma`` (standard deviation) for the species. An array of the sum of the log is yielded.
+The ``likelihood_of_species()`` function (defined below), for each index label in ``mu`` (which provides each unique iris species), calculates a probability density function for the test data, given the ``mu`` (mean) and ``sigma`` (standard deviation) for the species. An array of the sum of the log is yielded::
 
->>> from scipy.stats import norm
->>> def likelihood_of_species():
-...     for label in mu.index:
-...             pdf = norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])
-...             yield np.log(pdf).sum(axis=1)
+    >>> from scipy.stats import norm
+    >>> def likelihood_of_species():
+    ...     for label in mu.index:
+    ...             pdf = norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])
+    ...             yield np.log(pdf).sum(axis=1)
 
 
 While the generator function above is easy to read, it is hard to copy and paste. If you are following along, using the one-line generator expression, below, will be easier. The two are equivalent:
 
 >>> likelihood_of_species = (np.log(norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])).sum(axis=1) for label in mu.index)
 
 
-With this generator expression defined, we call the ``from_fields`` constructor to produce the ``likelihood`` table, providing column labels from ``mu.index`` and index labels from ``data_test.index``. For each test record row we now have a likelihood per species.
+With this generator expression defined, we call the ``from_fields`` constructor to produce the ``likelihood`` table, providing column labels from ``mu.index`` and index labels from ``data_test.index``. For each test record row we now have a likelihood per species::
 
->>> likelihood = sf.Frame.from_fields(likelihood_of_species, columns=mu.index, index=data_test.index)
->>> round(likelihood.head(), 2)
-<Frame>
-<Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
-<Index>
-1       -0.52       -2.31           -4.27
-14      -3.86       -6.97           -5.42
-20      -0.45       -2.38           -3.01
-21      -0.05       -5.29           -5.51
-37      -0.2        -2.56           -4.33
-<int64> <float64>   <float64>       <float64>
-
-
-We can calculate the ``posterior`` by multiplying ``likelihood`` by ``prior``. Whenever performing binary operations on ``Frame`` and ``Series``, indices will be aligned and, if necessary, reindexed before processing.
-
->>> posterior = likelihood * prior
->>> round(posterior.head(), 2)
-<Frame>
-<Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
-<Index>
-1       -0.19       -0.75           -1.35
-14      -1.38       -2.27           -1.72
-20      -0.16       -0.77           -0.95
-21      -0.02       -1.72           -1.75
-37      -0.07       -0.83           -1.37
-<int64> <float64>   <float64>       <float64>
-
-
-We can now add columns to our ``data_test`` ``FrameGO``. To determine our best prediction of species for each row of the test data, the column label (the species) of the maximum a posteriori estimate is selected with ``loc_max()``.
-
->>> data_test['predict'] = posterior.loc_max(axis=1)
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict     <<U7>
-<Index>
-1         4.9       3.0       Iris-setosa
-14        5.8       4.0       Iris-setosa
-20        5.4       3.4       Iris-setosa
-21        5.1       3.7       Iris-setosa
-37        4.9       3.1       Iris-setosa
-<int64>   <float64> <float64> <<U15>
-
-
-We can add two additional columns to evaluate the effectivess of the classifier. First, we can add an "observed" column by adding the original "species" column from the original ``data`` ``Frame``. In assigning a ``Series`` to a ``Frame``, only values found in the intersection of the indices will be added as a column.
-
->>> data_test['observed'] = data['species']
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict     observed    <<U8>
-<Index>
-1         4.9       3.0       Iris-setosa Iris-setosa
-14        5.8       4.0       Iris-setosa Iris-setosa
-20        5.4       3.4       Iris-setosa Iris-setosa
-21        5.1       3.7       Iris-setosa Iris-setosa
-37        4.9       3.1       Iris-setosa Iris-setosa
-<int64>   <float64> <float64> <<U15>      <<U15>
-
-
-Having populated a column of predicted and observed values, we can compare the two to get a Boolean column indicating when the classifier calculated a correct predicton.
-
->>> data_test['correct'] = data_test['predict'] == data_test['observed']
->>> data_test.tail()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict         observed       correct <<U8>
-<Index>
-129       7.2       3.0       Iris-virginica  Iris-virginica True
-130       7.4       2.8       Iris-virginica  Iris-virginica True
-140       6.7       3.1       Iris-virginica  Iris-virginica True
-144       6.7       3.3       Iris-virginica  Iris-virginica True
-149       5.9       3.0       Iris-versicolor Iris-virginica False
-<int64>   <float64> <float64> <<U15>          <<U15>         <bool>
+    >>> likelihood = sf.Frame.from_fields(likelihood_of_species, columns=mu.index, index=data_test.index)
+    >>> round(likelihood.head(), 2)
+    <Frame>
+    <Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
+    <Index>
+    1       -0.52       -2.31           -4.27
+    14      -3.86       -6.97           -5.42
+    20      -0.45       -2.38           -3.01
+    21      -0.05       -5.29           -5.51
+    37      -0.2        -2.56           -4.33
+    <int64> <float64>   <float64>       <float64>
+
+
+We can calculate the ``posterior`` by multiplying ``likelihood`` by ``prior``. Whenever performing binary operations on ``Frame`` and ``Series``, indices will be aligned and, if necessary, reindexed before processing::
+
+    >>> posterior = likelihood * prior
+    >>> round(posterior.head(), 2)
+    <Frame>
+    <Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
+    <Index>
+    1       -0.19       -0.75           -1.35
+    14      -1.38       -2.27           -1.72
+    20      -0.16       -0.77           -0.95
+    21      -0.02       -1.72           -1.75
+    37      -0.07       -0.83           -1.37
+    <int64> <float64>   <float64>       <float64>
+
+
+We can now add columns to our ``data_test`` ``FrameGO``. To determine our best prediction of species for each row of the test data, the column label (the species) of the maximum a posteriori estimate is selected with ``loc_max()``::
+
+    >>> data_test['predict'] = posterior.loc_max(axis=1)
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict     <<U7>
+    <Index>
+    1         4.9       3.0       Iris-setosa
+    14        5.8       4.0       Iris-setosa
+    20        5.4       3.4       Iris-setosa
+    21        5.1       3.7       Iris-setosa
+    37        4.9       3.1       Iris-setosa
+    <int64>   <float64> <float64> <<U15>
+
+
+We can add two additional columns to evaluate the effectivess of the classifier. First, we can add an "observed" column by adding the original "species" column from the original ``data`` ``Frame``. In assigning a ``Series`` to a ``Frame``, only values found in the intersection of the indices will be added as a column::
+
+    >>> data_test['observed'] = data['species']
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict     observed    <<U8>
+    <Index>
+    1         4.9       3.0       Iris-setosa Iris-setosa
+    14        5.8       4.0       Iris-setosa Iris-setosa
+    20        5.4       3.4       Iris-setosa Iris-setosa
+    21        5.1       3.7       Iris-setosa Iris-setosa
+    37        4.9       3.1       Iris-setosa Iris-setosa
+    <int64>   <float64> <float64> <<U15>      <<U15>
+
+
+Having populated a column of predicted and observed values, we can compare the two to get a Boolean column indicating when the classifier calculated a correct predicton::
+
+    >>> data_test['correct'] = data_test['predict'] == data_test['observed']
+    >>> data_test.tail()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict         observed       correct <<U8>
+    <Index>
+    129       7.2       3.0       Iris-virginica  Iris-virginica True
+    130       7.4       2.8       Iris-virginica  Iris-virginica True
+    140       6.7       3.1       Iris-virginica  Iris-virginica True
+    144       6.7       3.3       Iris-virginica  Iris-virginica True
+    149       5.9       3.0       Iris-versicolor Iris-virginica False
+    <int64>   <float64> <float64> <<U15>          <<U15>         <bool>
 
 
-To find the percentage of correct classifications among the test data, we can sum the ``correct`` Boolean column and divide that by the size of the test data.
+To find the percentage of correct classifications among the test data, we can sum the ``correct`` Boolean column and divide that by the size of the test data::
 
->>> data_test["correct"].sum() / len(data_test)
-0.7333333333333333
+    >>> data_test["correct"].sum() / len(data_test)
+    0.7333333333333333
 
 This simple naive Bayes classifier can predict iris species correctly about 73% of the time.
 
 For further introduction to StaticFrame, including links to articles, videos, and documentation, see `here <https://static-frame.readthedocs.io/en/latest/intro.html>`__.
```

### Comparing `static-frame-2.5.2/README.rst` & `static-frame-2.6.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -120,283 +120,285 @@
 ---------------------
 
 To get startred quickly, let's download the classic iris (flower) characteristics data set and build a simple naive Bayes classifier that can predict species from iris petal characteristics.
 
 While StaticFrame's API has over 7,500 endpoints, much will be familiar to users of Pandas or other DataFrame libraries. Rather than offering fewer interfaces with greater configurability, StaticFrame favors more numerous interfaces with more narrow parameters and functionality. This design leads to more maintainable code. (Read more about differences between Pandas and StaticFrame `here <https://static-frame.readthedocs.io/en/latest/articles/upgrade.html>`__.)
 
 
-We can download the data set from the UCI Machine Learning Repository and create a ``Frame``. StaticFrame exposes all constructors on the class: here, we will use the ``Frame.from_csv()`` constructor. To download a file from the internet and provide it to a constructor, we can use StaticFrame's ``WWW.from_file()`` interface.
+We can download the data set from the UCI Machine Learning Repository and create a ``Frame``. StaticFrame exposes all constructors on the class: here, we will use the ``Frame.from_csv()`` constructor. To download a file from the internet and provide it to a constructor, we can use StaticFrame's ``WWW.from_file()`` interface::
 
->>> import static_frame as sf
->>> data = sf.Frame.from_csv(sf.WWW.from_file('https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'), columns_depth=0)
+    >>> import static_frame as sf
+    >>> data = sf.Frame.from_csv(sf.WWW.from_file('https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'), columns_depth=0)
 
 
-Each record (or row) in this dataset describes observations of an iris flower, including its sepal and petal characteristics, as well as its species (of which there are three). To display just the first few rows, we can use the ``head()`` method. Notice that StaticFrame's default display makes it very clear what type of ``Frame``, ``Index``, and NumPy datatypes are present.
+Each record (or row) in this dataset describes observations of an iris flower, including its sepal and petal characteristics, as well as its species (of which there are three). To display just the first few rows, we can use the ``head()`` method. Notice that StaticFrame's default display makes it very clear what type of ``Frame``, ``Index``, and NumPy datatypes are present::
 
->>> data.head()
-<Frame>
-<Index> 0         1         2         3         4           <int64>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-1       4.9       3.0       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
+    >>> data.head()
+    <Frame>
+    <Index> 0         1         2         3         4           <int64>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    1       4.9       3.0       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
 
 As the columns are unlabelled, let's next add column labels. StaticFrame supports reindexing (conforming existing axis labels to new labels, potentially changing the size and ordering) and relabeling (simply applying new labels without regard to existing labels). As we can ignore the default column labels (auto-incremented integers), the ``relabel()`` method is used to provide new labels.
 
-Note that while ``relabel()`` creates a new ``Frame``, underlying NumPy data is not copied. As all NumPy data is immutable in StaticFrame, we can reuse it in our new container, making such operations very efficient. (Read more about no-copy operations `here <https://static-frame.readthedocs.io/en/latest/articles/no_copy.html>`__.)
+Note that while ``relabel()`` creates a new ``Frame``, underlying NumPy data is not copied. As all NumPy data is immutable in StaticFrame, we can reuse it in our new container, making such operations very efficient::
 
+    >>> data = data.relabel(columns=('sepal_l', 'sepal_w', 'petal_l', 'petal_w', 'species'))
+    >>> data.head()
+    <Frame>
+    <Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    1       4.9       3.0       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
->>> data = data.relabel(columns=('sepal_l', 'sepal_w', 'petal_l', 'petal_w', 'species'))
->>> data.head()
-<Frame>
-<Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-1       4.9       3.0       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
 
+(Read more about no-copy operations `here <https://static-frame.readthedocs.io/en/latest/articles/no_copy.html>`__.)
 
 For this example, eighty percent of the data will be used to train the classifier; the remaining twenty percent will be used to test the classifier. As all records are labelled with the known species, we can conclude by measuring the effectiveness of the classifier on the test data.
 
-To divide the data into two groups, we create a ``Series`` of contiguous integers and then extract a random selection of 80% of the values into a new ``Series``, here named ``sel_train``. This will be used to select our traning data. As the ``sample()`` method, given a count, randomly samples that many values, your results will be different unless use the same ``seed`` argument.
+To divide the data into two groups, we create a ``Series`` of contiguous integers and then extract a random selection of 80% of the values into a new ``Series``, here named ``sel_train``. This will be used to select our traning data. As the ``sample()`` method, given a count, randomly samples that many values, your results will be different unless use the same ``seed`` argument::
 
->>> sel = sf.Series(np.arange(len(data)))
->>> sel_train = sel.sample(round(len(data) * .8), seed=42)
->>> sel_train.head()
-<Series>
-<Index>
-0        0
-2        2
-3        3
-4        4
-5        5
-<int64>  <int64>
-
-We will create another ``Series`` to select the test data. The ``drop[]`` interface can be used to create a new ``Series`` that excludes the training selections, leaving just the testing selections. As with many interfaces in StaticFrame (such as ``astype`` and ``assign``), brackets can be used to do ``loc[]`` style selections.
-
->>> sel_test = sel.drop[sel_train]
->>> sel_test.head()
-<Series>
-<Index>
-1        1
-14       14
-20       20
-21       21
-37       37
-<int64>  <int64>
-
-
-To select a subset of the data for training, the ``sel_train`` ``Series`` can be passed to ``loc[]`` to select just those rows.
-
->>> data_train = data.loc[sel_train]
->>> data_train.head()
-<Frame>
-<Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-5       5.4       3.9       1.7       0.4       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
+    >>> sel = sf.Series(np.arange(len(data)))
+    >>> sel_train = sel.sample(round(len(data) * .8), seed=42)
+    >>> sel_train.head()
+    <Series>
+    <Index>
+    0        0
+    2        2
+    3        3
+    4        4
+    5        5
+    <int64>  <int64>
+
+
+We will create another ``Series`` to select the test data. The ``drop[]`` interface can be used to create a new ``Series`` that excludes the training selections, leaving just the testing selections. As with many interfaces in StaticFrame (such as ``astype`` and ``assign``), brackets can be used to do ``loc[]`` style selections::
+
+    >>> sel_test = sel.drop[sel_train]
+    >>> sel_test.head()
+    <Series>
+    <Index>
+    1        1
+    14       14
+    20       20
+    21       21
+    37       37
+    <int64>  <int64>
+
+
+To select a subset of the data for training, the ``sel_train`` ``Series`` can be passed to ``loc[]`` to select just those rows::
+
+    >>> data_train = data.loc[sel_train]
+    >>> data_train.head()
+    <Frame>
+    <Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    5       5.4       3.9       1.7       0.4       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
 
 With our data divided into two randomly-selected, non-overlapping groups, we can proceed to implement the naive Bayes classifier. We will compute the ``posterior`` of the test data by multiplying the ``prior`` and the ``likelihood``. With the ``posterior``, we can determine which species the classifier has calculated is most likely. (More on naive Bayes classifiers can be found `here <https://en.wikipedia.org/wiki/Naive_Bayes_classifier>`__.)
 
 The ``prior`` is calculated as the percentage of samples of each species in the training data. This is the "normalized" count per species. To get a ``Series`` of counts per species, we can select the species column, iterate over groups based on species name, and count the size of each group.
 
 In StaticFrame, this can be done by calling ``Series.iter_group_items()`` to get an iterator of pairs of group label, group (where the group is a ``Series``). This iterator (or any similar iterator) can be given to a ``Batch``, a chaining processor of ``Frame`` or ``Series``, to perform operations on each group. (For more on the ``Batch`` and other higher-order containers in StaticFrame, see `here <https://static-frame.readthedocs.io/en/latest/articles/uhoc.html>`__.)
 
-Once the ``Batch`` is created, selections, method calls, and operator expressions can be chained as if they were being called on a single container. Processing happens to every contained container, and a container is returned, only when a finalizer method, such as ``to_series()``, is called.
+Once the ``Batch`` is created, selections, method calls, and operator expressions can be chained as if they were being called on a single container. Processing happens to every contained container, and a container is returned, only when a finalizer method, such as ``to_series()``, is called::
 
->>> counts = sf.Batch(data_train['species'].iter_group_items()).count().to_series()
->>> counts
-<Series>
-<Index>
-Iris-setosa     43
-Iris-versicolor 39
-Iris-virginica  38
-<<U15>          <int64>
-
-
-As with NumPy, StaticFrame containers can be used in expressions with binary operators. The ``prior`` can be derived by dividing ``counts`` by the size of the training data. This returns a ``Series`` of the percentage of records per species.
-
->>> prior = counts / len(data_train)
->>> prior
-<Series>
-<Index>
-Iris-setosa     0.35833333333333334
-Iris-versicolor 0.325
-Iris-virginica  0.31666666666666665
-<<U15>          <float64>
+    >>> counts = sf.Batch(data_train['species'].iter_group_items()).count().to_series()
+    >>> counts
+    <Series>
+    <Index>
+    Iris-setosa     43
+    Iris-versicolor 39
+    Iris-virginica  38
+    <<U15>          <int64>
+
+
+As with NumPy, StaticFrame containers can be used in expressions with binary operators. The ``prior`` can be derived by dividing ``counts`` by the size of the training data. This returns a ``Series`` of the percentage of records per species::
+
+    >>> prior = counts / len(data_train)
+    >>> prior
+    <Series>
+    <Index>
+    Iris-setosa     0.35833333333333334
+    Iris-versicolor 0.325
+    Iris-virginica  0.31666666666666665
+    <<U15>          <float64>
 
 
 Having calculated the ``prior``, we can calculate ``likelihood`` next. To calculate ``likelihood``, we will call a probability distribution function (imported from SciPy) with the test data, once for each species, given the characteristics (mean and standard deviation) observed in the test data for that species.
 
-The ``Batch`` can again be used to calculate the mean and standard deviation, per species, from the training data. With the ``Frame`` of training data, we call ``iter_group_items()`` to group by species and, passing that iterator to ``Batch``, call ``mean()`` (assigned to ``mu``) or ``std()`` (assigned to ``sigma``). Note that ``iter_group_items()`` has an optional ``drop`` parameter to remove the column used for grouping from subsequent operations.
+The ``Batch`` can again be used to calculate the mean and standard deviation, per species, from the training data. With the ``Frame`` of training data, we call ``iter_group_items()`` to group by species and, passing that iterator to ``Batch``, call ``mean()`` (assigned to ``mu``) or ``std()`` (assigned to ``sigma``). Note that ``iter_group_items()`` has an optional ``drop`` parameter to remove the column used for grouping from subsequent operations::
 
 
->>> mu = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).mean().to_frame()
->>> mu
-<Frame>
-<Index>         sepal_l            sepal_w            <<U7>
-<Index>
-Iris-setosa     4.986046511627907  3.434883720930233
-Iris-versicolor 5.920512820512819  2.771794871794872
-Iris-virginica  6.6078947368421055 2.9763157894736842
-<<U15>          <float64>          <float64>
-
->>> sigma = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).std(ddof=1).to_frame()
->>> sigma
-<Frame>
-<Index>         sepal_l            sepal_w             <<U7>
-<Index>
-Iris-setosa     0.3419700595003668 0.3477024733400345
-Iris-versicolor 0.508444214804487  0.33082728674826684
-Iris-virginica  0.6055516042229233 0.3513942965328924
-<<U15>          <float64>          <float64>
-
-
-For a unified display of these characteristics, we can build a hierarchical index on each ``Frame`` with ``relabel_level_add()`` (adding the "mu" or "sigma" labels), then vertically concatenate the tables. As StaticFrame always requires unique labels in indices, adding an additional label is required before concatenation. The built-in ``round`` function can be used for more tidy display.
-
->>> stats = sf.Frame.from_concat((mu.relabel_level_add('mu'), sigma.relabel_level_add('sigma')))
->>> round(stats, 2)
-<Frame>
-<Index>                          sepal_l   sepal_w   <<U7>
-<IndexHierarchy>
-mu               Iris-setosa     4.99      3.43
-mu               Iris-versicolor 5.92      2.77
-mu               Iris-virginica  6.61      2.98
-sigma            Iris-setosa     0.34      0.35
-sigma            Iris-versicolor 0.51      0.33
-sigma            Iris-virginica  0.61      0.35
-<<U5>            <<U15>          <float64> <float64>
+    >>> mu = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).mean().to_frame()
+    >>> mu
+    <Frame>
+    <Index>         sepal_l            sepal_w            <<U7>
+    <Index>
+    Iris-setosa     4.986046511627907  3.434883720930233
+    Iris-versicolor 5.920512820512819  2.771794871794872
+    Iris-virginica  6.6078947368421055 2.9763157894736842
+    <<U15>          <float64>          <float64>
+
+    >>> sigma = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).std(ddof=1).to_frame()
+    >>> sigma
+    <Frame>
+    <Index>         sepal_l            sepal_w             <<U7>
+    <Index>
+    Iris-setosa     0.3419700595003668 0.3477024733400345
+    Iris-versicolor 0.508444214804487  0.33082728674826684
+    Iris-virginica  0.6055516042229233 0.3513942965328924
+    <<U15>          <float64>          <float64>
+
+
+For a unified display of these characteristics, we can build a hierarchical index on each ``Frame`` with ``relabel_level_add()`` (adding the "mu" or "sigma" labels), then vertically concatenate the tables. As StaticFrame always requires unique labels in indices, adding an additional label is required before concatenation. The built-in ``round`` function can be used for more tidy display::
+
+    >>> stats = sf.Frame.from_concat((mu.relabel_level_add('mu'), sigma.relabel_level_add('sigma')))
+    >>> round(stats, 2)
+    <Frame>
+    <Index>                          sepal_l   sepal_w   <<U7>
+    <IndexHierarchy>
+    mu               Iris-setosa     4.99      3.43
+    mu               Iris-versicolor 5.92      2.77
+    mu               Iris-virginica  6.61      2.98
+    sigma            Iris-setosa     0.34      0.35
+    sigma            Iris-versicolor 0.51      0.33
+    sigma            Iris-virginica  0.61      0.35
+    <<U5>            <<U15>          <float64> <float64>
 
 
 We can now move on to processing the test data with the characteristics derived from the training data. To do that, we will extract our previously selected test records with ``sel_test`` into a new ``Frame``, to which we can add our ``posterior`` predictions and final species classifications.
 
 It is common to process data in table by adding columns from left to right. StaticFrame permits this limited form of mutability with the grow-only ``FrameGO``. While underlying NumPy arrays are still always immutable, columns can be added to a ``FrameGO`` with bracket-style assignments. A ``FrameGO`` can be created from a ``Frame`` with the ``to_frame_go()`` method. As mentioned elsewhere, underlying immutable NumPy arrays are not copied: this is an efficient, no-copy operation.
 
-Passing two arguments to ``loc[]``, we can select rows with the values from ``sel_test``, and we can select columns with a list of labels for the sepal length and sepal width.
+Passing two arguments to ``loc[]``, we can select rows with the values from ``sel_test``, and we can select columns with a list of labels for the sepal length and sepal width::
 
->>> data_test = data.loc[sel_test.values, ['sepal_l', 'sepal_w']].to_frame_go()
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   <<U7>
-<Index>
-1         4.9       3.0
-14        5.8       4.0
-20        5.4       3.4
-21        5.1       3.7
-37        4.9       3.1
-<int64>   <float64> <float64>
+    >>> data_test = data.loc[sel_test.values, ['sepal_l', 'sepal_w']].to_frame_go()
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   <<U7>
+    <Index>
+    1         4.9       3.0
+    14        5.8       4.0
+    20        5.4       3.4
+    21        5.1       3.7
+    37        4.9       3.1
+    <int64>   <float64> <float64>
 
 
 StaticFrame interfaces make extensive use of iterators and generators. As used below, the ``Frame.from_fields()`` constructor will create a ``Frame`` from any iterable (or generator) of column arrays.
 
-The ``likelihood_of_species()`` function (defined below), for each index label in ``mu`` (which provides each unique iris species), calculates a probability density function for the test data, given the ``mu`` (mean) and ``sigma`` (standard deviation) for the species. An array of the sum of the log is yielded.
+The ``likelihood_of_species()`` function (defined below), for each index label in ``mu`` (which provides each unique iris species), calculates a probability density function for the test data, given the ``mu`` (mean) and ``sigma`` (standard deviation) for the species. An array of the sum of the log is yielded::
 
->>> from scipy.stats import norm
->>> def likelihood_of_species():
-...     for label in mu.index:
-...             pdf = norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])
-...             yield np.log(pdf).sum(axis=1)
+    >>> from scipy.stats import norm
+    >>> def likelihood_of_species():
+    ...     for label in mu.index:
+    ...             pdf = norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])
+    ...             yield np.log(pdf).sum(axis=1)
 
 
 While the generator function above is easy to read, it is hard to copy and paste. If you are following along, using the one-line generator expression, below, will be easier. The two are equivalent:
 
 >>> likelihood_of_species = (np.log(norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])).sum(axis=1) for label in mu.index)
 
 
-With this generator expression defined, we call the ``from_fields`` constructor to produce the ``likelihood`` table, providing column labels from ``mu.index`` and index labels from ``data_test.index``. For each test record row we now have a likelihood per species.
+With this generator expression defined, we call the ``from_fields`` constructor to produce the ``likelihood`` table, providing column labels from ``mu.index`` and index labels from ``data_test.index``. For each test record row we now have a likelihood per species::
 
->>> likelihood = sf.Frame.from_fields(likelihood_of_species, columns=mu.index, index=data_test.index)
->>> round(likelihood.head(), 2)
-<Frame>
-<Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
-<Index>
-1       -0.52       -2.31           -4.27
-14      -3.86       -6.97           -5.42
-20      -0.45       -2.38           -3.01
-21      -0.05       -5.29           -5.51
-37      -0.2        -2.56           -4.33
-<int64> <float64>   <float64>       <float64>
-
-
-We can calculate the ``posterior`` by multiplying ``likelihood`` by ``prior``. Whenever performing binary operations on ``Frame`` and ``Series``, indices will be aligned and, if necessary, reindexed before processing.
-
->>> posterior = likelihood * prior
->>> round(posterior.head(), 2)
-<Frame>
-<Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
-<Index>
-1       -0.19       -0.75           -1.35
-14      -1.38       -2.27           -1.72
-20      -0.16       -0.77           -0.95
-21      -0.02       -1.72           -1.75
-37      -0.07       -0.83           -1.37
-<int64> <float64>   <float64>       <float64>
-
-
-We can now add columns to our ``data_test`` ``FrameGO``. To determine our best prediction of species for each row of the test data, the column label (the species) of the maximum a posteriori estimate is selected with ``loc_max()``.
-
->>> data_test['predict'] = posterior.loc_max(axis=1)
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict     <<U7>
-<Index>
-1         4.9       3.0       Iris-setosa
-14        5.8       4.0       Iris-setosa
-20        5.4       3.4       Iris-setosa
-21        5.1       3.7       Iris-setosa
-37        4.9       3.1       Iris-setosa
-<int64>   <float64> <float64> <<U15>
-
-
-We can add two additional columns to evaluate the effectivess of the classifier. First, we can add an "observed" column by adding the original "species" column from the original ``data`` ``Frame``. In assigning a ``Series`` to a ``Frame``, only values found in the intersection of the indices will be added as a column.
-
->>> data_test['observed'] = data['species']
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict     observed    <<U8>
-<Index>
-1         4.9       3.0       Iris-setosa Iris-setosa
-14        5.8       4.0       Iris-setosa Iris-setosa
-20        5.4       3.4       Iris-setosa Iris-setosa
-21        5.1       3.7       Iris-setosa Iris-setosa
-37        4.9       3.1       Iris-setosa Iris-setosa
-<int64>   <float64> <float64> <<U15>      <<U15>
-
-
-Having populated a column of predicted and observed values, we can compare the two to get a Boolean column indicating when the classifier calculated a correct predicton.
-
->>> data_test['correct'] = data_test['predict'] == data_test['observed']
->>> data_test.tail()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict         observed       correct <<U8>
-<Index>
-129       7.2       3.0       Iris-virginica  Iris-virginica True
-130       7.4       2.8       Iris-virginica  Iris-virginica True
-140       6.7       3.1       Iris-virginica  Iris-virginica True
-144       6.7       3.3       Iris-virginica  Iris-virginica True
-149       5.9       3.0       Iris-versicolor Iris-virginica False
-<int64>   <float64> <float64> <<U15>          <<U15>         <bool>
+    >>> likelihood = sf.Frame.from_fields(likelihood_of_species, columns=mu.index, index=data_test.index)
+    >>> round(likelihood.head(), 2)
+    <Frame>
+    <Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
+    <Index>
+    1       -0.52       -2.31           -4.27
+    14      -3.86       -6.97           -5.42
+    20      -0.45       -2.38           -3.01
+    21      -0.05       -5.29           -5.51
+    37      -0.2        -2.56           -4.33
+    <int64> <float64>   <float64>       <float64>
+
+
+We can calculate the ``posterior`` by multiplying ``likelihood`` by ``prior``. Whenever performing binary operations on ``Frame`` and ``Series``, indices will be aligned and, if necessary, reindexed before processing::
+
+    >>> posterior = likelihood * prior
+    >>> round(posterior.head(), 2)
+    <Frame>
+    <Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
+    <Index>
+    1       -0.19       -0.75           -1.35
+    14      -1.38       -2.27           -1.72
+    20      -0.16       -0.77           -0.95
+    21      -0.02       -1.72           -1.75
+    37      -0.07       -0.83           -1.37
+    <int64> <float64>   <float64>       <float64>
+
+
+We can now add columns to our ``data_test`` ``FrameGO``. To determine our best prediction of species for each row of the test data, the column label (the species) of the maximum a posteriori estimate is selected with ``loc_max()``::
+
+    >>> data_test['predict'] = posterior.loc_max(axis=1)
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict     <<U7>
+    <Index>
+    1         4.9       3.0       Iris-setosa
+    14        5.8       4.0       Iris-setosa
+    20        5.4       3.4       Iris-setosa
+    21        5.1       3.7       Iris-setosa
+    37        4.9       3.1       Iris-setosa
+    <int64>   <float64> <float64> <<U15>
+
+
+We can add two additional columns to evaluate the effectivess of the classifier. First, we can add an "observed" column by adding the original "species" column from the original ``data`` ``Frame``. In assigning a ``Series`` to a ``Frame``, only values found in the intersection of the indices will be added as a column::
+
+    >>> data_test['observed'] = data['species']
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict     observed    <<U8>
+    <Index>
+    1         4.9       3.0       Iris-setosa Iris-setosa
+    14        5.8       4.0       Iris-setosa Iris-setosa
+    20        5.4       3.4       Iris-setosa Iris-setosa
+    21        5.1       3.7       Iris-setosa Iris-setosa
+    37        4.9       3.1       Iris-setosa Iris-setosa
+    <int64>   <float64> <float64> <<U15>      <<U15>
+
+
+Having populated a column of predicted and observed values, we can compare the two to get a Boolean column indicating when the classifier calculated a correct predicton::
+
+    >>> data_test['correct'] = data_test['predict'] == data_test['observed']
+    >>> data_test.tail()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict         observed       correct <<U8>
+    <Index>
+    129       7.2       3.0       Iris-virginica  Iris-virginica True
+    130       7.4       2.8       Iris-virginica  Iris-virginica True
+    140       6.7       3.1       Iris-virginica  Iris-virginica True
+    144       6.7       3.3       Iris-virginica  Iris-virginica True
+    149       5.9       3.0       Iris-versicolor Iris-virginica False
+    <int64>   <float64> <float64> <<U15>          <<U15>         <bool>
 
 
-To find the percentage of correct classifications among the test data, we can sum the ``correct`` Boolean column and divide that by the size of the test data.
+To find the percentage of correct classifications among the test data, we can sum the ``correct`` Boolean column and divide that by the size of the test data::
 
->>> data_test["correct"].sum() / len(data_test)
-0.7333333333333333
+    >>> data_test["correct"].sum() / len(data_test)
+    0.7333333333333333
 
 This simple naive Bayes classifier can predict iris species correctly about 73% of the time.
 
 For further introduction to StaticFrame, including links to articles, videos, and documentation, see `here <https://static-frame.readthedocs.io/en/latest/intro.html>`__.
```

### Comparing `static-frame-2.5.2/pyproject.toml` & `static-frame-2.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/setup.py` & `static-frame-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/__init__.py` & `static-frame-2.6.0/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,8 +131,8 @@
 from static_frame.core.util import TLocSelectorCompound as TLocSelectorCompound
 from static_frame.core.util import TPathSpecifierOrBinaryIO as TPathSpecifierOrBinaryIO
 from static_frame.core.util import TPathSpecifierOrTextIO as TPathSpecifierOrTextIO
 from static_frame.core.util import TSeriesInitializer as TSeriesInitializer
 from static_frame.core.www import WWW as WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '2.5.2'
+__version__ = '2.6.0'
```

### Comparing `static-frame-2.5.2/static_frame/__main__.py` & `static-frame-2.6.0/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/archive_npy.py` & `static-frame-2.6.0/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/archive_zip.py` & `static-frame-2.6.0/static_frame/core/archive_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/axis_map.py` & `static-frame-2.6.0/static_frame/core/axis_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import typing_extensions as tp
 from arraykit import array_deepcopy
 
 from static_frame.core.bus import Bus
 from static_frame.core.exception import AxisInvalid
 from static_frame.core.generic_aliases import TBusAny
 from static_frame.core.generic_aliases import TFrameAny
+from static_frame.core.generic_aliases import TIndexAny
+from static_frame.core.generic_aliases import TIndexIntDefault
 from static_frame.core.index import Index
 from static_frame.core.index_auto import IndexAutoConstructorFactory
 from static_frame.core.index_base import IndexBase
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.index_hierarchy import IndexHierarchyGO
 from static_frame.core.index_hierarchy import TTreeNode
 from static_frame.core.util import DTYPE_INT_DEFAULT
@@ -130,24 +132,24 @@
             index_constructors=IndexAutoConstructorFactory), opposite
 
 
 def buses_to_iloc_hierarchy(
         buses: tp.Iterable[TBusAny],
         deepcopy_from_bus: bool,
         init_exception_cls: tp.Type[Exception],
-        ) -> IndexHierarchy:
+        ) -> IndexHierarchy[TIndexIntDefault, TIndexAny]:
     '''
     Given an iterable of named :obj:`Bus` derive a obj:`IndexHierarchy` with iloc labels on the outer depth, loc labels on the inner depth.
     '''
     extractor = get_extractor(deepcopy_from_bus, is_array=False, memo_active=False)
 
     tree: TTreeNode = {}
     for label, bus in enumerate(buses):
         if not isinstance(bus, Bus):
-            raise init_exception_cls('Must provide an interable of Bus.')
+            raise init_exception_cls(f'Must provide an instance of a `Bus`, not {type(bus)}.')
         tree[label] = extractor(bus._index)
 
     ctor: tp.Callable[..., IndexBase] = partial(Index, dtype=DTYPE_INT_DEFAULT)
     return IndexHierarchy.from_tree(tree,
             index_constructors=[ctor, IndexAutoConstructorFactory], # type: ignore
             )
```

### Comparing `static-frame-2.5.2/static_frame/core/batch.py` & `static-frame-2.6.0/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/bus.py` & `static-frame-2.6.0/static_frame/core/bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from static_frame.core.util import TILocSelector
 from static_frame.core.util import TIndexCtorSpecifier
 from static_frame.core.util import TIndexCtorSpecifiers
 from static_frame.core.util import TIndexInitializer
 from static_frame.core.util import TLabel
 from static_frame.core.util import TLocSelector
 from static_frame.core.util import TName
+from static_frame.core.util import TNDArrayObject
 from static_frame.core.util import TPathSpecifier
 from static_frame.core.util import TSortKinds
 
 
 #-------------------------------------------------------------------------------
 class FrameDeferredMeta(type):
     def __repr__(cls) -> str:
@@ -550,24 +551,14 @@
         Returns a reverse iterator on the :obj:`Bus` index.
 
         Returns:
             :obj:`Index`
         '''
         return reversed(self._index)
 
-    # def __copy__(self) -> tp.Self:
-    #     '''
-    #     Return a new Bus, holding new references to Frames as well as a link to the a new Store instance.
-    #     '''
-    #     return self.__class__(series,
-    #             store=self._store.__copy__(),
-    #             config=self._config,
-    #             max_persiste=self._max_persist,
-    #             )
-
     #---------------------------------------------------------------------------
     # name interface
 
     @property
     @doc_inject()
     def name(self) -> TName:
         '''{}'''
@@ -636,15 +627,15 @@
                 yield_type=IterNodeType.ITEMS,
                 apply_type=IterNodeApplyType.SERIES_VALUES,
                 )
 
     #---------------------------------------------------------------------------
     # index manipulation
 
-    # NOTE: must return a new Bus with fully-realized Frames, as cannot gaurantee usage of a Store after labels have been changed.
+    # NOTE: must return a new Bus with fully-realized Frames, as cannot guarantee usage of a Store after labels have been changed.
 
     @doc_inject(selector='reindex', class_name='Bus')
     def reindex(self,
             index: TIndexInitializer,
             *,
             fill_value: tp.Any,
             own_index: bool = False,
@@ -995,15 +986,15 @@
             for i, label in enumerate(self._index.values):
                 self._update_values_mutable_iloc(key=i)
                 yield label, self._values_mutable[i]
 
     _items_store = items
 
     @property
-    def values(self) -> TNDArrayAny:
+    def values(self) -> TNDArrayObject:
         '''A 1D object array of all :obj:`Frame` contained in the :obj:`Bus`. The returned ``np.ndarray`` will have ``Frame``; this will never return an array with ``FrameDeferred``, but ``max_persist`` will be observed in reading from the Store.
         '''
         # NOTE: when self._values_mutable is fully loaded, it could become immutable and avoid a copy. However, with unpersist(), we might unload all Frame
 
         if self._loaded_all:
             post = self._values_mutable.copy()
             post.flags.writeable = False
@@ -1317,15 +1308,14 @@
             {count}
 
         Returns:
             :obj:`Bus`
         '''
         return self.iloc[-count:]
 
-
     #---------------------------------------------------------------------------
     # transformations resulting in the same dimensionality
 
     @doc_inject(selector='sort')
     def sort_index(self,
             *,
             ascending: TBoolOrBools = True,
@@ -1453,13 +1443,12 @@
                 (self._index._to_signature_bytes(
                         include_name=include_name,
                         include_class=include_class,
                         encoding=encoding),),
                 v))
 
 
-
 TBusAny = Bus[tp.Any]
```

### Comparing `static-frame-2.5.2/static_frame/core/container.py` & `static-frame-2.6.0/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/container_util.py` & `static-frame-2.6.0/static_frame/core/container_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 from static_frame.core.util import TIndexCtor
 from static_frame.core.util import TIndexCtorSpecifier
 from static_frame.core.util import TIndexCtorSpecifiers
 from static_frame.core.util import TIndexInitializer
 from static_frame.core.util import TLabel
 from static_frame.core.util import TLocSelector
 from static_frame.core.util import TName
+from static_frame.core.util import TNDArrayIntDefault
 from static_frame.core.util import TSortKinds
 from static_frame.core.util import TUFunc
 from static_frame.core.util import WarningsSilent
 from static_frame.core.util import concat_resolved
 from static_frame.core.util import is_dtype_specifier
 from static_frame.core.util import is_mapping
 from static_frame.core.util import iterable_to_array_1d
@@ -1723,15 +1724,15 @@
     return asc_is_element, values_for_lex
 
 def sort_index_for_order(
         index: 'IndexBase',
         ascending: TBoolOrBools,
         kind: TSortKinds,
         key: tp.Optional[tp.Callable[['IndexBase'], tp.Union[TNDArrayAny, 'IndexBase']]],
-        ) -> TNDArrayAny:
+        ) -> TNDArrayIntDefault:
     '''Return an integer array defing the new ordering.
     '''
     # cfs is container_for_sort
     if key:
         cfs = key(index)
         cfs_is_array = cfs.__class__ is np.ndarray
         if cfs_is_array:
@@ -1742,15 +1743,15 @@
             raise RuntimeError('key function returned a container of invalid length')
     else:
         cfs = index
         cfs_is_array = False
         cfs_depth = cfs.depth
 
     asc_is_element: bool
-    order: TNDArrayAny
+    order: TNDArrayIntDefault
     # argsort lets us do the sort once and reuse the results
     if cfs_depth > 1:
         if cfs_is_array:
             values_for_lex = [cfs[NULL_SLICE, i] for i in range(cfs.shape[1]-1, -1, -1)] # type: ignore
         else: # cfs is an IndexHierarchy
             values_for_lex = [cfs.values_at_depth(i) #type: ignore
                     for i in range(cfs.depth-1, -1, -1)] #type: ignore
```

### Comparing `static-frame-2.5.2/static_frame/core/display.py` & `static-frame-2.6.0/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/display_color.py` & `static-frame-2.6.0/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/display_config.py` & `static-frame-2.6.0/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/display_html_datatables.py` & `static-frame-2.6.0/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/display_visidata.py` & `static-frame-2.6.0/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/doc_str.py` & `static-frame-2.6.0/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/exception.py` & `static-frame-2.6.0/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/fill_value_auto.py` & `static-frame-2.6.0/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/frame.py` & `static-frame-2.6.0/static_frame/core/frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/generic_aliases.py` & `static-frame-2.6.0/static_frame/core/generic_aliases.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,25 @@
+import numpy as np
 import typing_extensions as tp
 
 from static_frame.core.bus import Bus
 from static_frame.core.frame import Frame
 from static_frame.core.frame import FrameGO
 from static_frame.core.frame import FrameHE
 from static_frame.core.index import Index
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.series import Series
 from static_frame.core.series import SeriesHE
 
 TIndexAny = Index[tp.Any]
+TIndexIntDefault = Index[np.int64]
 TIndexHierarchyAny = IndexHierarchy[tp.Unpack[tp.Tuple[tp.Any, ...]]]
 
 TSeriesAny = Series[tp.Any, tp.Any]
+TSeriesObject = Series[tp.Any, np.object_]
 TSeriesHEAny = SeriesHE[tp.Any, tp.Any]
 
 
 TFrameAny = Frame[tp.Any, tp.Any, tp.Unpack[tp.Tuple[tp.Any, ...]]]  #pragma: no cover
 TFrameGOAny = FrameGO[tp.Any, tp.Any] #pragma: no cover
 TFrameHEAny = FrameHE[tp.Any, tp.Any, tp.Unpack[tp.Tuple[tp.Any, ...]]]  #pragma: no cover
```

### Comparing `static-frame-2.5.2/static_frame/core/hloc.py` & `static-frame-2.6.0/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/index.py` & `static-frame-2.6.0/static_frame/core/index.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/index_auto.py` & `static-frame-2.6.0/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/index_base.py` & `static-frame-2.6.0/static_frame/core/index_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from static_frame.core.display import Display
 from static_frame.core.display import DisplayActive
 from static_frame.core.display_config import DisplayConfig
 from static_frame.core.display_config import DisplayFormats
 from static_frame.core.doc_str import doc_inject
 from static_frame.core.exception import ErrorInitIndex
 from static_frame.core.node_dt import InterfaceDatetime
+from static_frame.core.node_iter import IterNodeDepthLevel
 from static_frame.core.node_re import InterfaceRe
 from static_frame.core.node_str import InterfaceString
 from static_frame.core.style_config import STYLE_CONFIG_DEFAULT
 from static_frame.core.style_config import StyleConfig
 from static_frame.core.style_config import style_config_css_factory
 from static_frame.core.util import DTYPE_OBJECT
 from static_frame.core.util import OPERATORS
@@ -185,14 +186,18 @@
     def __iter__(self) -> tp.Iterator[TLabel]:
         raise NotImplementedError() #pragma: no cover
 
     def __contains__(self, value: TLabel) -> bool:
         raise NotImplementedError() #pragma: no cover
 
     @property
+    def iter_label(self) -> IterNodeDepthLevel[tp.Any]:
+        raise NotImplementedError() #pragma: no cover
+
+    @property
     def shape(self) -> tp.Tuple[int, ...]:
         raise NotImplementedError() #pragma: no cover
 
     @property
     def ndim(self) -> int:
         raise NotImplementedError() #pragma: no cover
```

### Comparing `static-frame-2.5.2/static_frame/core/index_correspondence.py` & `static-frame-2.6.0/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/index_datetime.py` & `static-frame-2.6.0/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/index_hierarchy.py` & `static-frame-2.6.0/static_frame/core/index_hierarchy.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 from static_frame.core.util import KEY_MULTIPLE_TYPES
 from static_frame.core.util import NAME_DEFAULT
 from static_frame.core.util import NULL_SLICE
 from static_frame.core.util import PositionsAllocator
 from static_frame.core.util import TBoolOrBools
 from static_frame.core.util import TDepthLevel
 from static_frame.core.util import TDepthLevelSpecifier
+from static_frame.core.util import TDepthLevelSpecifierMany
+from static_frame.core.util import TDepthLevelSpecifierOne
 from static_frame.core.util import TDtypesSpecifier
 from static_frame.core.util import TILocSelector
 from static_frame.core.util import TIndexCtor
 from static_frame.core.util import TIndexCtorSpecifier
 from static_frame.core.util import TIndexCtorSpecifiers
 from static_frame.core.util import TIndexInitializer
 from static_frame.core.util import TKeyTransform
@@ -1498,14 +1500,20 @@
 
         dl = depth_level_from_specifier(depth_level, self.depth)
 
         if isinstance(dl, INT_TYPES):
             return self._blocks._extract_array_column(dl)
         return self._blocks._extract_array(column_key=dl)
 
+    @tp.overload
+    def index_at_depth(self, depth_level: TDepthLevelSpecifierOne) -> Index[tp.Any]: ...
+
+    @tp.overload
+    def index_at_depth(self, depth_level: TDepthLevelSpecifierMany) -> tp.Tuple[Index[tp.Any], ...]: ...
+
     def index_at_depth(self,
             depth_level: TDepthLevelSpecifier = 0,
             ) -> tp.Union[Index[tp.Any], tp.Tuple[Index[tp.Any], ...]]:
         '''
         Return an index, or a tuple of indices for the ``depth_level`` specified.
 
         Args:
```

### Comparing `static-frame-2.5.2/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-2.6.0/static_frame/core/index_hierarchy_set_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,23 +149,20 @@
     '''Encode `ih` based on the union indices'''
     remapped_indexers: tp.List[TNDArrayAny] = []
 
     union_idx: Index[tp.Any]
     idx: Index[tp.Any]
     indexer: TNDArrayAny
     depth_level = list(range(depth))
-    for ( # type: ignore
-        union_idx,
-        idx,
-        indexer
-    ) in zip(
-        union_indices,
-        ih.index_at_depth(depth_level),
-        ih.indexer_at_depth(depth_level)
-    ):
+
+    for union_idx, idx, indexer in zip(
+            union_indices,
+            ih.index_at_depth(depth_level),
+            ih.indexer_at_depth(depth_level)
+            ):
         # 2. For each depth, for each index, remap the indexers to the shared base.
         indexer_remap_key = idx._index_iloc_map(union_idx)
         remapped_indexers.append(indexer_remap_key[indexer])
 
     return HierarchicalLocMap.encode(
             np.array(remapped_indexers, dtype=encoding_dtype).T,
             bit_offset_encoders,
```

### Comparing `static-frame-2.5.2/static_frame/core/interface.py` & `static-frame-2.6.0/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/interface_meta.py` & `static-frame-2.6.0/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/join.py` & `static-frame-2.6.0/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/loc_map.py` & `static-frame-2.6.0/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/memory_measure.py` & `static-frame-2.6.0/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/metadata.py` & `static-frame-2.6.0/static_frame/core/metadata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/node_dt.py` & `static-frame-2.6.0/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/node_fill_value.py` & `static-frame-2.6.0/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/node_hashlib.py` & `static-frame-2.6.0/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/node_iter.py` & `static-frame-2.6.0/static_frame/core/node_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/node_re.py` & `static-frame-2.6.0/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/node_selector.py` & `static-frame-2.6.0/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/node_str.py` & `static-frame-2.6.0/static_frame/core/node_str.py`

 * *Files identical despite different names*

```diff
@@ -246,15 +246,15 @@
 
     def endswith(self,
             suffix: tp.Union[str, tp.Iterable[str]],
             start: tp.Optional[int] = None,
             end: tp.Optional[int] = None
             ) -> TVContainer_co:
         '''
-        Returns a container with the number of non-overlapping occurrences of substring ``suffix`` (or an interable of suffixes) in the optional range ``start``, ``end``.
+        Returns a container with the number of non-overlapping occurrences of substring ``suffix`` (or an iterable of suffixes) in the optional range ``start``, ``end``.
         '''
 
         if isinstance(suffix, str):
             block_iter = self._process_blocks(self._blocks, npc.endswith, (suffix, start, end))
             return self._blocks_to_container(block_iter)
 
         def block_gen() -> tp.Iterator[TNDArrayAny]:
@@ -544,15 +544,15 @@
 
     def startswith(self,
             prefix: tp.Union[str, tp.Iterable[str]],
             start: tp.Optional[int] = None,
             end: tp.Optional[int] = None
             ) -> TVContainer_co:
         '''
-        Returns a container with the number of non-overlapping occurrences of substring `prefix` (or an interable of prefixes) in the optional range ``start``, ``end``.
+        Returns a container with the number of non-overlapping occurrences of substring `prefix` (or an iterable of prefixes) in the optional range ``start``, ``end``.
         '''
         if isinstance(prefix, str):
             block_iter = self._process_blocks(self._blocks, npc.startswith, (prefix, start, end))
             return self._blocks_to_container(block_iter)
 
         def block_gen() -> tp.Iterator[TNDArrayAny]:
             blocks_per_sub = (
@@ -683,15 +683,15 @@
 
     def endswith(self,
             suffix: tp.Union[str, tp.Iterable[str]],
             start: tp.Optional[int] = None,
             end: tp.Optional[int] = None
             ) -> 'Batch':
         '''
-        Returns a container with the number of non-overlapping occurrences of substring ``suffix`` (or an interable of suffixes) in the optional range ``start``, ``end``.
+        Returns a container with the number of non-overlapping occurrences of substring ``suffix`` (or an iterable of suffixes) in the optional range ``start``, ``end``.
         '''
         return self._batch_apply(lambda c: c.via_str.endswith(suffix, start, end))
 
     def find(self,
             sub: str,
             start: tp.Optional[int] = None,
             end: tp.Optional[int] = None
@@ -887,15 +887,15 @@
 
     def startswith(self,
             prefix: tp.Union[str, tp.Iterable[str]],
             start: tp.Optional[int] = None,
             end: tp.Optional[int] = None
             ) -> 'Batch':
         '''
-        Returns a container with the number of non-overlapping occurrences of substring `prefix` (or an interable of prefixes) in the optional range ``start``, ``end``.
+        Returns a container with the number of non-overlapping occurrences of substring `prefix` (or an iterable of prefixes) in the optional range ``start``, ``end``.
         '''
         return self._batch_apply(lambda c: c.via_str.startswith(prefix, start, end))
 
     def strip(self,
             chars: tp.Optional[str] = None,
             ) -> 'Batch':
         '''
```

### Comparing `static-frame-2.5.2/static_frame/core/node_transpose.py` & `static-frame-2.6.0/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/node_values.py` & `static-frame-2.6.0/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/pivot.py` & `static-frame-2.6.0/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/platform.py` & `static-frame-2.6.0/static_frame/core/platform.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 class Platform:
 
     @staticmethod
     def to_series() -> Series[Index[np.str_], tp.Any]:
         def items() -> tp.Iterator[tp.Tuple[str, tp.Any]]:
             yield 'platform', platform_mod.platform()
             yield 'sys.version', sys.version.replace('\n', '')
-
             yield 'static-frame', static_frame.__version__
 
             # NOTE: see requirements-extras.txt
             for package in (
                     'numpy',
                     'pandas',
                     'xlsxwriter',
@@ -40,16 +39,14 @@
                     mod = importlib.import_module(package)
                 except ModuleNotFoundError: #pragma: no cover
                     yield package, ModuleNotFoundError #pragma: no cover
                     continue #pragma: no cover
 
                 if hasattr(mod, '__version__'):
                     yield package, mod.__version__
-                elif hasattr(mod, 'version'): # msgpack
-                    yield package, mod.version
                 else:
                     yield package, None
 
         return Series.from_items(items(), name='platform')
 
     @classmethod
     def display(cls) -> Display:
```

### Comparing `static-frame-2.5.2/static_frame/core/protocol_dfi.py` & `static-frame-2.6.0/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/protocol_dfi_abc.py` & `static-frame-2.6.0/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/quilt.py` & `static-frame-2.6.0/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/rank.py` & `static-frame-2.6.0/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/series.py` & `static-frame-2.6.0/static_frame/core/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -2476,15 +2476,15 @@
                 own_index=own_index)
 
     def shift(self,
             shift: int,
             *,
             fill_value: tp.Any = np.nan,
             ) -> tp.Self:
-        '''Return a Series with values shifted forward on the index (with a positive shift) or backward on the index (with a negative shift).
+        '''Return a `Series` with values shifted forward on the index (with a positive shift) or backward on the index (with a negative shift).
 
         Args:
             shift: Positive or negative integer shift.
             fill_value: Value to be used to fill data missing after the shift.
 
         Returns:
             :obj:`Series`
```

### Comparing `static-frame-2.5.2/static_frame/core/store.py` & `static-frame-2.6.0/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/store_client_mixin.py` & `static-frame-2.6.0/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/store_config.py` & `static-frame-2.6.0/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/store_filter.py` & `static-frame-2.6.0/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/store_hdf5.py` & `static-frame-2.6.0/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/store_sqlite.py` & `static-frame-2.6.0/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/store_xlsx.py` & `static-frame-2.6.0/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/store_zip.py` & `static-frame-2.6.0/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/style_config.py` & `static-frame-2.6.0/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/type_blocks.py` & `static-frame-2.6.0/static_frame/core/type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/type_clinic.py` & `static-frame-2.6.0/static_frame/core/type_clinic.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/util.py` & `static-frame-2.6.0/static_frame/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     from static_frame.core.index_hierarchy import IndexHierarchy  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.series import Series  # pylint: disable=W0611 #pragma: no cover
     from static_frame.core.type_blocks import TypeBlocks  # pylint: disable=W0611 #pragma: no cover
 
 TNDArrayAny = np.ndarray[tp.Any, tp.Any]
 TNDArrayBool = np.ndarray[tp.Any, np.dtype[np.bool_]]
 TNDArrayObject = np.ndarray[tp.Any, np.dtype[np.object_]]
-
 TNDArrayIntDefault = np.ndarray[tp.Any, np.dtype[np.int64]]
 
 TDtypeAny = np.dtype[tp.Any]
 TDtypeObject = np.dtype[np.object_] #pragma: no cover
 TOptionalArrayList = tp.Optional[tp.List[TNDArrayAny]]
 
 # dtype.kind
@@ -418,15 +417,18 @@
 # support an iterable of specifiers, or mapping based on column names
 TDtypesSpecifier = tp.Optional[tp.Union[
         TDtypeSpecifier,
         tp.Iterable[TDtypeSpecifier],
         tp.Dict[TLabel, TDtypeSpecifier]
         ]]
 
-TDepthLevelSpecifier = tp.Union[int, tp.List[int], slice, TNDArrayAny, None]
+TDepthLevelSpecifierOne = int
+TDepthLevelSpecifierMany = tp.Union[tp.List[int], slice, TNDArrayIntDefault, None]
+TDepthLevelSpecifier = tp.Union[TDepthLevelSpecifierOne, TDepthLevelSpecifierMany]
+
 TDepthLevel = tp.Union[int, tp.List[int]]
 
 TCallableToIter = tp.Callable[[], tp.Iterable[tp.Any]]
 
 TIndexSpecifier = tp.Union[int, TLabel] # specify a position in an index
 TIndexInitializer = tp.Union[
         'IndexBase',
```

### Comparing `static-frame-2.5.2/static_frame/core/www.py` & `static-frame-2.6.0/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/core/yarn.py` & `static-frame-2.6.0/static_frame/core/yarn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,108 @@
 from __future__ import annotations
 
 from collections.abc import Set
+from functools import partial
 from itertools import chain
 
 import numpy as np
 import typing_extensions as tp
 
 from static_frame.core.axis_map import buses_to_iloc_hierarchy
 from static_frame.core.axis_map import buses_to_loc_hierarchy
-from static_frame.core.bus import Bus
+from static_frame.core.bus import FrameDeferred
 from static_frame.core.container import ContainerBase
 from static_frame.core.container_util import index_from_optional_constructor
 from static_frame.core.container_util import index_many_concat
 from static_frame.core.container_util import iter_component_signature_bytes
 from static_frame.core.container_util import rehierarch_from_index_hierarchy
+from static_frame.core.container_util import sort_index_for_order
 from static_frame.core.display import Display
 from static_frame.core.display import DisplayActive
 from static_frame.core.display import DisplayHeader
 from static_frame.core.display_config import DisplayConfig
 from static_frame.core.doc_str import doc_inject
 from static_frame.core.exception import ErrorInitYarn
 from static_frame.core.exception import RelabelInvalid
 from static_frame.core.frame import Frame
+from static_frame.core.generic_aliases import TBusAny
+from static_frame.core.generic_aliases import TFrameAny
+from static_frame.core.generic_aliases import TIndexAny
+from static_frame.core.generic_aliases import TIndexIntDefault
+from static_frame.core.generic_aliases import TSeriesAny
+from static_frame.core.generic_aliases import TSeriesObject
 from static_frame.core.index import Index
+from static_frame.core.index_auto import IndexAutoConstructorFactory
 from static_frame.core.index_auto import IndexAutoFactory
 from static_frame.core.index_auto import TIndexAutoFactory
 from static_frame.core.index_auto import TRelabelInput
 from static_frame.core.index_base import IndexBase
+from static_frame.core.index_correspondence import IndexCorrespondence
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.node_iter import IterNodeApplyType
 from static_frame.core.node_iter import IterNodeNoArg
 from static_frame.core.node_iter import IterNodeType
 from static_frame.core.node_selector import InterfaceSelectTrio
 from static_frame.core.node_selector import InterGetItemILocReduces
 from static_frame.core.node_selector import InterGetItemLocReduces
 from static_frame.core.series import Series
 from static_frame.core.store_client_mixin import StoreClientMixin
 from static_frame.core.style_config import StyleConfig
+from static_frame.core.util import BOOL_TYPES
+from static_frame.core.util import DEFAULT_SORT_KIND
+from static_frame.core.util import DTYPE_INT_DEFAULT
 from static_frame.core.util import DTYPE_OBJECT
+from static_frame.core.util import EMPTY_SLICE
+from static_frame.core.util import INT_TYPES
 from static_frame.core.util import NAME_DEFAULT
+from static_frame.core.util import PositionsAllocator
+from static_frame.core.util import TBoolOrBools
 from static_frame.core.util import TDtypeObject
 from static_frame.core.util import TILocSelector
+from static_frame.core.util import TILocSelectorMany
+from static_frame.core.util import TILocSelectorOne
 from static_frame.core.util import TIndexCtorSpecifier
 from static_frame.core.util import TIndexCtorSpecifiers
 from static_frame.core.util import TIndexInitializer
 from static_frame.core.util import TLabel
 from static_frame.core.util import TLocSelector
 from static_frame.core.util import TName
 from static_frame.core.util import TNDArrayAny
+from static_frame.core.util import TNDArrayIntDefault
 from static_frame.core.util import TNDArrayObject
+from static_frame.core.util import TSortKinds
+from static_frame.core.util import array_shift
 from static_frame.core.util import is_callable_or_mapping
 from static_frame.core.util import iterable_to_array_1d
 
-TSeriesObject = Series[tp.Any, np.object_]
-TFrameAny = Frame[tp.Any, tp.Any, tp.Unpack[tp.Tuple[tp.Any, ...]]]
-TBusAny = Bus[tp.Any]
-
 #-------------------------------------------------------------------------------
+TIHInternal = IndexHierarchy[TIndexIntDefault, TIndexAny]
+
 TVIndex = tp.TypeVar('TVIndex', bound=IndexBase, default=tp.Any)
 
 class Yarn(ContainerBase, StoreClientMixin, tp.Generic[TVIndex]):
     '''
     A :obj:`Series`-like container made of an ordered collection of :obj:`Bus`. :obj:`Yarn` can be indexed independently of the contained :obj:`Bus`, permitting independent labels per contained :obj:`Frame`.
     '''
 
     __slots__ = (
             '_values',
             '_hierarchy',
             '_index',
+            '_indexer',
             '_name',
             '_deepcopy_from_bus',
             )
 
     _values: TNDArrayObject
-    _hierarchy: IndexHierarchy
+    _hierarchy: TIHInternal
     _index: IndexBase
+    _indexer: TNDArrayIntDefault
     _name: TName
+    _deepcopy_from_bus: bool
 
     _NDIM: int = 1
 
     @classmethod
     def from_buses(cls,
             buses: tp.Iterable[TBusAny],
             *,
@@ -126,57 +149,83 @@
 
         Args:
             containers:
             index: Optionally provide new labels for the result of the concatenation.
             name:
             deepcopy_from_bus:
         '''
-        bus_components: tp.List[TBusAny] = []
+        values_components: tp.List[TNDArrayObject] = []
+        indexer_components: tp.List[TNDArrayIntDefault] = []
         index_components: tp.Optional[tp.List[IndexBase]] = None if index is not None else []
-        for element in containers:
-            if isinstance(element, Yarn):
-                bus_components.extend(element._values)
-                if index_components is not None:
-                    index_components.append(element.index)
-            else:
-                raise NotImplementedError(f'cannot instantiate from {type(element)}')
-
-        array = np.empty(len(bus_components), dtype=DTYPE_OBJECT)
-        for i, bus in enumerate(bus_components):
-            array[i] = bus
-        array.flags.writeable = False
+        labels = [] # for new hierarchy
+
+        bus_count = 0
+        hierarchy_count = 0
+
+        for y in containers:
+            if not isinstance(y, Yarn):
+                raise NotImplementedError(f'Cannot concatenate from {type(y)}')
+
+            b_pos: int
+            for b_pos, frame_label in y._hierarchy: # type: ignore[assignment]
+                labels.append((b_pos + bus_count, frame_label))
+
+            values_components.append(y._values)
+            indexer_components.append(y._indexer + hierarchy_count)
+
+            bus_count += len(y._values)
+            hierarchy_count += len(y._hierarchy)
+
+            if index_components is not None: # only accumulate if index not provided
+                index_components.append(y.index)
+
+        values = np.concatenate(values_components, dtype=DTYPE_OBJECT) # pylint: disable=E1123
+        indexer = np.concatenate(indexer_components, dtype=DTYPE_INT_DEFAULT) # pylint: disable=E1123
+
+        ctor: tp.Callable[..., IndexBase] = partial(Index, dtype=DTYPE_INT_DEFAULT)
+        ctors: TIndexCtorSpecifiers = [ctor, IndexAutoConstructorFactory] # type: ignore[list-item]
+        hierarchy: TIHInternal = IndexHierarchy.from_labels(labels,
+                index_constructors=ctors,
+                )
 
         if index_components is not None:
             index = index_many_concat(index_components, Index)
+            own_index = True
+        else: # provided index must be evaluated
+            own_index = False
 
-        # series: TSeriesObject = Series(array)
-        return cls(array,
-                deepcopy_from_bus=deepcopy_from_bus,
+        return cls(values,
                 index=index,
-                name=name,
+                deepcopy_from_bus=deepcopy_from_bus,
+                indexer=indexer,
+                hierarchy=hierarchy,
+                name=name if name is not NAME_DEFAULT else None,
+                own_index=own_index,
                 )
 
     #---------------------------------------------------------------------------
     def __init__(self,
             series: tp.Union[TSeriesObject, tp.Iterable[TBusAny]], # rename: values
             *,
             index: TIndexInitializer | TIndexAutoFactory | None = None,
             index_constructor: tp.Optional[TIndexCtorSpecifier] = None,
             deepcopy_from_bus: bool = False,
-            hierarchy: tp.Optional[IndexHierarchy] = None,
+            indexer: tp.Optional[TNDArrayIntDefault] = None,
+            hierarchy: tp.Optional[TIHInternal] = None,
             name: TName = None,
             own_index: bool = False,
             ) -> None:
         '''
         Args:
             series: An iterable (or :obj:`Series`) of :obj:`Bus`. The length of this container may not be the same as ``index``, if provided.
             index: Optionally provide an index for the :obj:`Frame` contained in all :obj:`Bus`.
             index_constructor:
             deepcopy_from_bus:
             hierarchy: Optionally provide a depth-two `IndexHierarchy` constructed from `Bus` integer positions on the outer level, and contained `Frame` labels on the inner level.
+            indexer: For each `Frame` referenced by the index, provide the location within the internal `IndexHierarchy`.
             name:
             own_index:
         '''
 
         if isinstance(series, Series):
             if series.dtype != DTYPE_OBJECT:
                 raise ErrorInitYarn(
@@ -196,39 +245,50 @@
                     self._values,
                     deepcopy_from_bus=self._deepcopy_from_bus,
                     init_exception_cls=ErrorInitYarn,
                     )
         else: # NOTE: we assume this hierarchy is well-formed
             self._hierarchy = hierarchy
 
+        self._index: IndexBase
         if own_index:
             self._index = index #type: ignore
         elif index is None or index is IndexAutoFactory:
             self._index = IndexAutoFactory.from_optional_constructor(
                     len(self._hierarchy),
                     default_constructor=Index,
                     explicit_constructor=index_constructor
                     )
         else: # an iterable of labels or an Index
             self._index = index_from_optional_constructor(index,
                     default_constructor=Index,
                     explicit_constructor=index_constructor
                     )
 
-        if len(self._index) != len(self._hierarchy): # pyright: ignore
+        if len(self._index) > len(self._hierarchy): # pyright: ignore
             raise ErrorInitYarn(f'Length of supplied index ({len(self._index)}) not of sufficient size ({len(self._hierarchy)}).') # pyright: ignore
 
+        self._indexer: TNDArrayIntDefault
+        if indexer is None:
+            self._indexer = PositionsAllocator.get(len(self._index)) # pyright: ignore
+        else:
+            self._indexer = indexer
+            if len(self._indexer) != len(self._index): # pyright: ignore
+                raise ErrorInitYarn(f'Length of supplied indexer ({len(self._indexer)}) not of sufficient size ({len(self._index)}).') # pyright: ignore
+
+
     #---------------------------------------------------------------------------
     # deferred loading of axis info
 
     def unpersist(self) -> None:
         '''For the :obj:`Bus` contained in this object, replace all loaded :obj:`Frame` with :obj:`FrameDeferred`.
         '''
         for b in self._values:
-            b.unpersist()
+            if b is not None:
+                b.unpersist()
 
     #---------------------------------------------------------------------------
     def __reversed__(self) -> tp.Iterator[TLabel]:
         '''
         Returns a reverse iterator on the :obj:`Yarn` index.
 
         Returns:
@@ -252,28 +312,30 @@
         Args:
             name
         '''
         # NOTE: do not need to call _update_index_labels; can continue to defer
         return self.__class__(self._values,
                 index=self._index,
                 hierarchy=self._hierarchy,
+                indexer=self._indexer,
                 name=name,
                 deepcopy_from_bus=self._deepcopy_from_bus,
+                own_index=True,
                 )
 
     #---------------------------------------------------------------------------
     # interfaces
 
     @property
     def loc(self) -> InterGetItemLocReduces[TYarnAny, np.object_]:
         return InterGetItemLocReduces(self._extract_loc) # type: ignore
 
     @property
     def iloc(self) -> InterGetItemILocReduces[TYarnAny, np.object_]:
-        return InterGetItemILocReduces(self._extract_iloc) # type: ignore
+        return InterGetItemILocReduces(self._extract_iloc)
 
     @property
     def drop(self) -> InterfaceSelectTrio[TYarnAny]:
         '''
         Interface for dropping elements from :obj:`Yarn`.
         '''
         return InterfaceSelectTrio( #type: ignore
@@ -305,14 +367,408 @@
                 container=self,
                 function_items=self._axis_element_items,
                 function_values=self._axis_element,
                 yield_type=IterNodeType.ITEMS,
                 apply_type=IterNodeApplyType.SERIES_VALUES,
                 )
 
+    #---------------------------------------------------------------------------
+    # extraction
+
+    @tp.overload
+    def _extract_iloc(self, key: TILocSelectorMany) -> tp.Self: ...
+
+    @tp.overload
+    def _extract_iloc(self, key: TILocSelectorOne) -> TFrameAny: ...
+
+    def _extract_iloc(self, key: TILocSelector) -> tp.Self | TFrameAny:
+        '''
+        Returns:
+            Yarn or, if an element is selected, a Frame
+        '''
+        indexer: tp.Union[TNDArrayIntDefault, int] = self._indexer[key]
+
+        sel_hierarchy = self._hierarchy._extract_iloc(indexer)
+
+        if isinstance(indexer, INT_TYPES):
+            # got a single element, return a Frame
+            b_pos, frame_label = sel_hierarchy # always two-item tuple
+            f: Frame = self._values[b_pos]._extract_loc(frame_label) # pyright: ignore
+            return f
+
+        # NOTE: identify Bus that are no longer needed, and remove them from the values such that they can be GCd if necessary; for now, we leave the hierarchy (and the position numbers) unchanged
+        bus_pos = self._hierarchy.index_at_depth(depth_level=0)
+        sel_bus_pos = sel_hierarchy.index_at_depth(depth_level=0)
+        if len(sel_bus_pos) < len(bus_pos):
+            values = self._values.copy() # becomes mutable
+            for pos in bus_pos.difference(sel_bus_pos):
+                values[pos] = None
+            values.flags.writeable = False
+        else:
+            values = self._values
+
+        return self.__class__(values,
+                index=self._index.iloc[key],
+                deepcopy_from_bus=self._deepcopy_from_bus,
+                hierarchy=self._hierarchy,
+                indexer=indexer,
+                name=self._name,
+                own_index=True,
+                )
+
+    def _extract_loc(self, key: TLocSelector) -> TYarnAny | TFrameAny:
+        # use the index active for this Yarn
+        key_iloc = self._index._loc_to_iloc(key)
+        return self._extract_iloc(key_iloc)
+
+    @doc_inject(selector='selector')
+    def __getitem__(self, key: TLocSelector) -> TYarnAny | TFrameAny:
+        '''Selector of values by label.
+
+        Args:
+            key: {key_loc}
+        '''
+        return self._extract_loc(key)
+
+    #---------------------------------------------------------------------------
+    # utilities for alternate extraction: drop
+
+    def _drop_iloc(self, key: TILocSelector) -> tp.Self:
+        invalid = np.full(len(self._index), True)
+        invalid[key] = False
+        return self._extract_iloc(invalid)
+
+    def _drop_loc(self, key: TLocSelector) -> tp.Self:
+        return self._drop_iloc(self._index._loc_to_iloc(key))
+
+    #---------------------------------------------------------------------------
+    # axis functions
+
+    def _axis_element_items(self,
+            ) -> tp.Iterator[tp.Tuple[TLabel, tp.Any]]:
+        '''Generator of index, value pairs, equivalent to Series.items(). Repeated to have a common signature as other axis functions.
+        '''
+        yield from self.items()
+
+    def _axis_element(self,
+            ) -> tp.Iterator[TFrameAny]:
+        for b_pos, frame_label in self._hierarchy._extract_iloc(self._indexer):
+            yield self._values[b_pos]._extract_loc(frame_label) # pyright: ignore
+
+    #---------------------------------------------------------------------------
+    # index manipulation
+
+    @doc_inject(selector='reindex', class_name='Bus')
+    def reindex(self,
+            index: TIndexInitializer,
+            *,
+            fill_value: tp.Any = None,
+            own_index: bool = False,
+            check_equals: bool = True
+            ) -> tp.Self:
+        '''
+        {doc}
+
+        Args:
+            index: {index_initializer}
+            columns: {index_initializer}
+            {fill_value}
+            {own_index}
+        '''
+        index_owned: IndexBase
+        if own_index:
+            index_owned = index # type: ignore
+        else:
+            index_owned = index_from_optional_constructor(index,
+                    default_constructor=Index)
+
+        if check_equals and self._index.equals(index_owned):
+            # if labels are equal (even if a different Index subclass), we can simply use the new Index
+            return self.__class__(self._values,
+                    index=index_owned,
+                    hierarchy=self._hierarchy,
+                    indexer=self._indexer,
+                    name=self._name,
+                    deepcopy_from_bus=self._deepcopy_from_bus,
+                    own_index=True,
+                    )
+
+        ic = IndexCorrespondence.from_correspondence(self._index, index_owned)
+        if not ic.size:
+            return self._extract_iloc(EMPTY_SLICE)
+
+        if ic.is_subset: # must have some common
+            indexer = self._indexer[ic.iloc_src]
+            indexer.flags.writeable = False
+
+            return self.__class__(self._values,
+                    index=index_owned,
+                    hierarchy=self._hierarchy,
+                    indexer=indexer,
+                    name=self._name,
+                    deepcopy_from_bus=self._deepcopy_from_bus,
+                    own_index=True,
+                    )
+
+        raise NotImplementedError('Reindex operations that are not strict subsets are not supported by `Yarn`')
+
+    @doc_inject(selector='relabel', class_name='Yarn')
+    def relabel(self,
+            index: tp.Optional[TRelabelInput]
+            ) -> tp.Self:
+        '''
+        {doc}
+
+        Args:
+            index: {relabel_input_index}
+        '''
+        #NOTE: we name the parameter index for alignment with the corresponding Frame method
+        own_index = False
+        if index is IndexAutoFactory:
+            index_init = None
+        elif index is None:
+            index_init = self._index
+        elif is_callable_or_mapping(index):
+            index_init = self._index.relabel(index)
+            own_index = True
+        elif isinstance(index, Set):
+            raise RelabelInvalid()
+        else:
+            index_init = index #type: ignore
+
+        return self.__class__(self._values, # no change to Buses
+                index=index_init, # pyright: ignore
+                deepcopy_from_bus=self._deepcopy_from_bus,
+                hierarchy=self._hierarchy, # no change
+                indexer=self._indexer,
+                own_index=own_index,
+                )
+
+    @doc_inject(selector='relabel_flat', class_name='Yarn')
+    def relabel_flat(self) -> tp.Self:
+        '''
+        {doc}
+        '''
+        if not isinstance(self._index, IndexHierarchy):
+            raise RuntimeError('cannot flatten an Index that is not an IndexHierarchy')
+
+        return self.__class__(self._values, # no change to Buses
+                index=self._index.flat(),
+                deepcopy_from_bus=self._deepcopy_from_bus,
+                hierarchy=self._hierarchy, # no change
+                indexer=self._indexer,
+                own_index=True,
+                )
+
+    @doc_inject(selector='relabel_level_add', class_name='Yarn')
+    def relabel_level_add(self,
+            level: TLabel
+            ) -> tp.Self:
+        '''
+        {doc}
+
+        Args:
+            level: {level}
+        '''
+        return self.__class__(self._values, # no change to Buses
+                index=self._index.level_add(level),
+                deepcopy_from_bus=self._deepcopy_from_bus,
+                hierarchy=self._hierarchy, # no change
+                indexer=self._indexer,
+                own_index=True,
+                )
+
+    @doc_inject(selector='relabel_level_drop', class_name='Yarn')
+    def relabel_level_drop(self,
+            count: int = 1
+            ) -> tp.Self:
+        '''
+        {doc}
+
+        Args:
+            count: {count}
+        '''
+        if not isinstance(self._index, IndexHierarchy):
+            raise RuntimeError('cannot drop level of an Index that is not an IndexHierarchy')
+
+        return self.__class__(self._values, # no change to Buses
+                index=self._index.level_drop(count),
+                deepcopy_from_bus=self._deepcopy_from_bus,
+                hierarchy=self._hierarchy, # no change
+                indexer=self._indexer,
+                own_index=True,
+                )
+
+    def rehierarch(self,
+            depth_map: tp.Sequence[int],
+            *,
+            index_constructors: TIndexCtorSpecifiers = None,
+            ) -> tp.Self:
+        '''
+        Return a new :obj:`Series` with new a hierarchy based on the supplied ``depth_map``.
+        '''
+        if self.index.depth == 1:
+            raise RuntimeError('cannot rehierarch when there is no hierarchy')
+
+        index, iloc_map = rehierarch_from_index_hierarchy(
+                labels=self._index, #type: ignore
+                depth_map=depth_map,
+                index_constructors=index_constructors,
+                name=self._index.name,
+                )
+
+        return self._extract_iloc(iloc_map).relabel(index)
+
+    #---------------------------------------------------------------------------
+
+    def items(self) -> tp.Iterator[tp.Tuple[TLabel, TFrameAny]]:
+        '''Iterator of pairs of :obj:`Yarn` label and contained :obj:`Frame`.
+        '''
+        labels = iter(self._index)
+        for b_pos, frame_label in self._hierarchy._extract_iloc(self._indexer):
+            # NOTE: missing optimization to read multiple Frame from Bus in one extraction
+            yield next(labels), self._values[b_pos]._extract_loc(frame_label) # pyright: ignore
+
+    _items_store = items
+
+    @property
+    def values(self) -> TNDArrayObject:
+        '''A 1D object array of all :obj:`Frame` contained in all contained :obj:`Bus`.
+        '''
+        array = np.empty(shape=len(self._index), dtype=DTYPE_OBJECT)
+
+        for i, (b_pos, frame_label) in enumerate(
+                self._hierarchy._extract_iloc(self._indexer)):
+            array[i] = self._values[b_pos]._extract_loc(frame_label) # pyright: ignore
+
+        array.flags.writeable = False
+        return array
+
+    #---------------------------------------------------------------------------
+
+    def __len__(self) -> int:
+        '''Length of values.
+        '''
+        return self._index.__len__()
+
+    @doc_inject()
+    def display(self,
+            config: tp.Optional[DisplayConfig] = None,
+            *,
+            style_config: tp.Optional[StyleConfig] = None,
+            ) -> Display:
+        '''{doc}
+
+        Args:
+            {config}
+        '''
+        # NOTE: the key change over serires is providing the Bus as the displayed class
+        config = config or DisplayActive.get()
+        display_cls = Display.from_values((),
+                header=DisplayHeader(self.__class__, self._name),
+                config=config)
+
+        array = np.empty(shape=len(self._index), dtype=DTYPE_OBJECT)
+
+        for i, (b_pos, frame_label) in enumerate(
+                self._hierarchy._extract_iloc(self._indexer)):
+            b = self._values[b_pos]
+            # NOTE: do not load FrameDeferred
+            array[i] = b._values_mutable[b.index.loc_to_iloc(frame_label)] # pyright: ignore
+
+        array.flags.writeable = False
+
+        # create temporary series just for display
+        series: TSeriesObject = Series(array, index=self._index, own_index=True)
+        return series._display(config,
+                display_cls=display_cls,
+                style_config=style_config,
+                )
+
+    #---------------------------------------------------------------------------
+    # extended discriptors; in general, these do not force loading Frame
+
+    @property
+    def mloc(self) -> TSeriesObject:
+        '''Returns a :obj:`Series` showing a tuple of memory locations within each loaded Frame.
+        '''
+        mlocs = [(b.mloc if b is not None else None) for b in self._values]
+        array = np.empty(shape=len(self._index), dtype=DTYPE_OBJECT)
+
+        for i, (b_pos, frame_label) in enumerate(
+                self._hierarchy._extract_iloc(self._indexer)):
+            array[i] = mlocs[b_pos]._extract_loc(frame_label)
+
+        array.flags.writeable = False
+        return Series(array, index=self._index, own_index=True, name='mloc')
+
+    @property
+    def dtypes(self) -> TFrameAny:
+        '''Returns a Frame of dtypes for all loaded Frames.
+        '''
+        deferred_dtypes = Series((None,))
+
+        def gen() -> tp.Iterator[TSeriesObject]:
+            for b_pos, frame_label in self._hierarchy._extract_iloc(self._indexer):
+                b = self._values[b_pos]
+                f = b._values_mutable[b.index.loc_to_iloc(frame_label)] # pyright: ignore
+                if f is FrameDeferred:
+                    yield deferred_dtypes
+                else:
+                    yield f.dtypes
+
+        return Frame.from_concat(gen(), index=self._index, fill_value=None)
+
+    @property
+    def shapes(self) -> TSeriesObject:
+        '''A :obj:`Series` describing the shape of each loaded :obj:`Frame`. Unloaded :obj:`Frame` will have a shape of None.
+
+        Returns:
+            :obj:`tp.Series`
+        '''
+        # collect shape Series
+        shapes = [(b.shapes if b is not None else None) for b in self._values]
+        array = np.empty(shape=len(self._index), dtype=DTYPE_OBJECT)
+
+        for i, (b_pos, frame_label) in enumerate(
+                self._hierarchy._extract_iloc(self._indexer)):
+            array[i] = shapes[b_pos][frame_label] # pyright: ignore
+
+        array.flags.writeable = False
+        return Series(array, index=self._index, own_index=True, name='shape')
+
+    @property
+    def nbytes(self) -> int:
+        '''Total bytes of data currently loaded in :obj:`Frame` contained in this :obj:`Yarn`.
+        '''
+        post = 0
+        for b_pos, frame_label in self._hierarchy._extract_iloc(self._indexer):
+            b = self._values[b_pos]
+            f = b._values_mutable[b.index.loc_to_iloc(frame_label)] # pyright: ignore
+            if f is not FrameDeferred:
+                post += f.nbytes
+
+        return post
+
+    @property
+    def status(self) -> TFrameAny:
+        '''
+        Return a :obj:`Frame` indicating loaded status, size, bytes, and shape of all loaded :obj:`Frame` in :obj:`Bus` contined in this :obj:`Yarn`.
+        '''
+        # collect status Frame
+        status = [(b.status if b is not None else None) for b in self._values]
+
+        def gen() -> tp.Iterator[TNDArrayObject]:
+            for b_pos, frame_label in self._hierarchy._extract_iloc(self._indexer):
+                f = status[b_pos]
+                yield f._extract_array(f.index.loc_to_iloc(frame_label))
+
+        return Frame.from_records(gen(),
+                index=self._index,
+                columns=('loaded', 'size', 'nbytes', 'shape'))
 
     #---------------------------------------------------------------------------
     # common attributes from the numpy array
 
     @property
     def dtype(self) -> TDtypeObject:
         '''
@@ -327,35 +783,35 @@
     def shape(self) -> tp.Tuple[int]:
         '''
         Return a tuple describing the shape of the realized NumPy array.
 
         Returns:
             :obj:`Tuple[int]`
         '''
-        return (self._hierarchy.shape[0],)
+        return (self._index.__len__(),)
 
     @property
     def ndim(self) -> int:
         '''
         Return the number of dimensions, which for a :obj:`Yarn` is always 1.
 
         Returns:
             :obj:`int`
         '''
         return self._NDIM
 
     @property
     def size(self) -> int:
         '''
-        Return the size of the underlying NumPy array.
+        Return the size.
 
         Returns:
             :obj:`int`
         '''
-        return self._hierarchy.shape[0]
+        return self._index.__len__()
 
     #---------------------------------------------------------------------------
 
     @property
     def index(self) -> IndexBase:
         '''
         The index instance assigned to this container.
@@ -404,36 +860,14 @@
         Returns:
             :obj:`Any`
         '''
         if key not in self._index:
             return default
         return self.__getitem__(key)
 
-    def items(self) -> tp.Iterator[tp.Tuple[TLabel, TFrameAny]]:
-        '''Iterator of pairs of :obj:`Yarn` label and contained :obj:`Frame`.
-        '''
-        labels = iter(self._index)
-        for bus in self._values:
-            # NOTE: cannot use Bus.items() as it may not have the same index representation as the Yarn; Bus._axis_element is optimized for handling max_persist > 1 loading
-            for f in bus._axis_element():
-                yield next(labels), f
-
-    _items_store = items
-
-    @property
-    def values(self) -> TNDArrayAny:
-        '''A 1D object array of all :obj:`Frame` contained in all contained :obj:`Bus`.
-        '''
-        # NOTE self._values is likely not the same size as self.values
-        array = np.empty(shape=len(self._index), dtype=DTYPE_OBJECT)
-        np.concatenate([b.values for b in self._values], out=array)
-        array.flags.writeable = False
-        return array
-
-
     #---------------------------------------------------------------------------
     @doc_inject()
     def equals(self,
             other: tp.Any,
             *,
             compare_name: bool = False,
             compare_dtype: bool = False,
@@ -512,329 +946,166 @@
             {count}
 
         Returns:
             :obj:`Yarn`
         '''
         return self.iloc[-count:]
 
-
     #---------------------------------------------------------------------------
-    # extraction
+    # transformations resulting in the same dimensionality
 
-    def _extract_iloc(self, key: TILocSelector) -> TYarnAny | TFrameAny:
-        '''
-        Returns:
-            Yarn or, if an element is selected, a Frame
+    @doc_inject(selector='sort')
+    def sort_index(self,
+            *,
+            ascending: TBoolOrBools = True,
+            kind: TSortKinds = DEFAULT_SORT_KIND,
+            key: tp.Optional[tp.Callable[[IndexBase], tp.Union[TNDArrayAny, IndexBase]]] = None,
+            ) -> tp.Self:
         '''
-        target_hierarchy = self._hierarchy._extract_iloc(key)
-        if isinstance(target_hierarchy, tuple):
-            # got a single element, return a Frame
-            b_pos, frame_label = target_hierarchy
-            return self._values[b_pos]._extract_loc(frame_label) # type: ignore
+        Return a new Yarn ordered by the sorted Index.
 
-        # get the outer-most index of the hierarchical index; we cannot use index_at_depth
-        target_bus_labels = target_hierarchy.unique(
-                depth_level=0,
-                order_by_occurrence=True)
-        ctor = next(iter(target_hierarchy._index_constructors))
-        target_bus_index = ctor(target_bus_labels)
-
-        # create a Boolean array equal to the entire realized length
-        valid = np.full(len(self._index), False)
-        valid[key] = True
-
-        buses = np.empty(len(target_bus_index), dtype=DTYPE_OBJECT)
-
-        pos = 0
-        for b_pos, width in self._hierarchy.label_widths_at_depth(0):
-            if b_pos not in target_bus_index:
-                pos += width
-                continue
-            # create Boolean selection within this Bus
-            extract_per_bus = valid[pos: pos + width]
-            pos += width
-            # given original bus position, look-up the bus position in returned array
-            idx = target_bus_index.loc_to_iloc(b_pos)
-            buses[idx] = self._values[b_pos]._extract_iloc(extract_per_bus) # type: ignore
-
-        buses.flags.writeable = False
+        Args:
+            *
+            {ascendings}
+            {kind}
+            {key}
 
-        return self.__class__(buses,
-                index=self._index.iloc[key],
-                deepcopy_from_bus=self._deepcopy_from_bus,
-                name=self._name,
-                own_index=True,
+        Returns:
+            :obj:`Yarn`
+        '''
+        order = sort_index_for_order(self._index,
+                kind=kind,
+                ascending=ascending,
+                key=key,
                 )
+        return self._extract_iloc(order)
 
-    def _extract_loc(self, key: TLocSelector) -> TYarnAny | TFrameAny:
-        # use the index active for this Yarn
-        key_iloc = self._index._loc_to_iloc(key)
-        return self._extract_iloc(key_iloc)
-
-
-    @doc_inject(selector='selector')
-    def __getitem__(self, key: TLocSelector) -> TYarnAny | TFrameAny:
-        '''Selector of values by label.
-
-        Args:
-            key: {key_loc}
+    @doc_inject(selector='sort')
+    def sort_values(self,
+            *,
+            ascending: bool = True,
+            kind: TSortKinds = DEFAULT_SORT_KIND,
+            key: tp.Callable[[TYarnAny], tp.Union[TNDArrayAny, TSeriesAny]],
+            ) -> tp.Self:
         '''
-        return self._extract_loc(key)
-
-    #---------------------------------------------------------------------------
-    # utilities for alternate extraction: drop
-
-    def _drop_iloc(self, key: TILocSelector) -> tp.Self:
-        invalid = np.full(len(self._index), True)
-        invalid[key] = False
-        return self._extract_iloc(invalid) # type: ignore
-
-    def _drop_loc(self, key: TLocSelector) -> tp.Self:
-        return self._drop_iloc(self._index._loc_to_iloc(key))
+        Return a new Yarn ordered by the sorted values. Note that as a Yarn contains Frames, a `key` argument must be provided to extract a sortable value, and this key function will process a :obj:`Series` of :obj:`Frame`.
 
-    #---------------------------------------------------------------------------
-    # axis functions
+        Args:
+            *
+            {ascending}
+            {kind}
+            {key}
 
-    def _axis_element_items(self,
-            ) -> tp.Iterator[tp.Tuple[TLabel, tp.Any]]:
-        '''Generator of index, value pairs, equivalent to Series.items(). Repeated to have a common signature as other axis functions.
+        Returns:
+            :obj:`Yarn`
         '''
-        yield from self.items()
+        cfs = key(self)
+        cfs_values: TNDArrayAny = cfs if cfs.__class__ is np.ndarray else cfs.values # type: ignore
+        asc_is_element = isinstance(ascending, BOOL_TYPES)
+        if not asc_is_element:
+            raise RuntimeError('Multiple ascending values not permitted.')
+
+        # argsort lets us do the sort once and reuse the results
+        order = np.argsort(cfs_values, kind=kind)
+        if not ascending:
+            order = order[::-1]
 
-    def _axis_element(self,
-            ) -> tp.Iterator[tp.Any]:
+        return self._extract_iloc(order)
 
-        for bus in self._values:
-            yield from bus._axis_element()
-
-    #---------------------------------------------------------------------------
-    def __len__(self) -> int:
-        '''Length of values.
-        '''
-        return self._index.__len__()
-
-    @doc_inject()
-    def display(self,
-            config: tp.Optional[DisplayConfig] = None,
+    def roll(self,
+            shift: int,
             *,
-            style_config: tp.Optional[StyleConfig] = None,
-            ) -> Display:
-        '''{doc}
+            include_index: bool = False,
+            ) -> tp.Self:
+        '''Return a Yarn with values rotated forward and wrapped around the index (with a positive shift) or backward and wrapped around the index (with a negative shift).
 
         Args:
-            {config}
+            shift: Positive or negative integer shift.
+            include_index: Determine if the Index is shifted with the underlying data.
+
+        Returns:
+            :obj:`Yarn`
         '''
-        # NOTE: the key change over serires is providing the Bus as the displayed class
-        config = config or DisplayActive.get()
-        display_cls = Display.from_values((),
-                header=DisplayHeader(self.__class__, self._name),
-                config=config)
+        if shift % len(self._indexer):
+            indexer = array_shift(
+                    array=self._indexer,
+                    shift=shift,
+                    axis=0,
+                    wrap=True)
+            indexer.flags.writeable = False
+        else:
+            indexer = self._indexer
 
-        # NOTE: do not load FrameDeferred, so concatenate contained Series's values directly
-        array = np.empty(shape=len(self._index), dtype=DTYPE_OBJECT)
-        np.concatenate(
-            [b._values_mutable for b in self._values],
-            out=array)
-        array.flags.writeable = False
+        if include_index:
+            index = self._index.roll(shift=shift)
+            own_index = True
+        else:
+            index = self._index
+            own_index = False
 
-        # create temporary series just for display
-        series: TSeriesObject = Series(array, index=self._index, own_index=True)
-        return series._display(config,
-                display_cls=display_cls,
-                style_config=style_config,
+        return self.__class__(self._values,
+                index=index,
+                own_index=own_index,
+                indexer=indexer,
+                hierarchy=self._hierarchy,
+                name=self._name,
+                deepcopy_from_bus=self._deepcopy_from_bus,
                 )
 
-    #---------------------------------------------------------------------------
-    # extended discriptors; in general, these do not force loading Frame
-
-    @property
-    def mloc(self) -> TSeriesObject:
-        '''Returns a :obj:`Series` showing a tuple of memory locations within each loaded Frame.
-        '''
-        return Series.from_concat((b.mloc for b in self._values),
-                index=self._index)
-
-    @property
-    def dtypes(self) -> TFrameAny:
-        '''Returns a Frame of dtypes for all loaded Frames.
-        '''
-        return Frame.from_concat(
-                frames=(f.dtypes for f in self._values),
-                fill_value=None,
-                ).relabel(index=self._index)
+    def shift(self,
+            shift: int,
+            *,
+            fill_value: tp.Any,
+            ) -> tp.Self:
+        '''Return a :obj:`Yarn` with values shifted forward on the index (with a positive shift) or backward on the index (with a negative shift).
 
-    @property
-    def shapes(self) -> TSeriesObject:
-        '''A :obj:`Series` describing the shape of each loaded :obj:`Frame`. Unloaded :obj:`Frame` will have a shape of None.
+        Args:
+            shift: Positive or negative integer shift.
+            fill_value: Value to be used to fill data missing after the shift.
 
         Returns:
-            :obj:`tp.Series`
-        '''
-        return Series.from_concat((b.shapes for b in self._values),
-                index=self._index)
-
-    @property
-    def nbytes(self) -> int:
-        '''Total bytes of data currently loaded in :obj:`Bus` contained in this :obj:`Yarn`.
-        '''
-        return sum(b.nbytes for b in self._values)
-
-    @property
-    def status(self) -> TFrameAny:
-        '''
-        Return a :obj:`Frame` indicating loaded status, size, bytes, and shape of all loaded :obj:`Frame` in :obj:`Bus` contined in this :obj:`Yarn`.
+            :obj:`Yarn`
         '''
-        f: TFrameAny = Frame.from_concat(
-                (b.status for b in self._values),
-                index=IndexAutoFactory)
-        return f.relabel(index=self._index)
-
+        raise NotImplementedError('A `Yarn` cannot be shifted as newly created missing values cannot be filled without replacing stored `Bus`.')
 
     #---------------------------------------------------------------------------
     # exporter
 
     def to_series(self) -> TSeriesObject: # can get generic Bus index
         '''Return a :obj:`Series` with the :obj:`Frame` contained in all contained :obj:`Bus`.
         '''
-        # NOTE: this should load all deferred Frame
-        return Series(self.values, index=self._index, own_index=True)
+        # NOTE: this will load all deferred Frame
+        return Series(self.values,
+                index=self._index,
+                own_index=True,
+                name=self._name,
+                )
 
     def _to_signature_bytes(self,
             include_name: bool = True,
             include_class: bool = True,
             encoding: str = 'utf-8',
             ) -> bytes:
 
+        # For a Yarn, the signature bytes need only contain the signature of the associated Frame and the index; all else are internal implementation mechanisms
+
         v = (f._to_signature_bytes(
                 include_name=include_name,
                 include_class=include_class,
                 encoding=encoding,
                 ) for f in self._axis_element())
 
         return b''.join(chain(
                 iter_component_signature_bytes(self,
                         include_name=include_name,
                         include_class=include_class,
                         encoding=encoding),
                 (self._index._to_signature_bytes(
                         include_name=include_name,
                         include_class=include_class,
-                        encoding=encoding),
-                self._hierarchy._to_signature_bytes(
-                        include_name=include_name,
-                        include_class=include_class,
                         encoding=encoding),),
                 v))
 
 
-
-
-    #---------------------------------------------------------------------------
-    # index manipulation
-
-    @doc_inject(selector='relabel', class_name='Yarn')
-    def relabel(self,
-            index: tp.Optional[TRelabelInput]
-            ) -> tp.Self:
-        '''
-        {doc}
-
-        Args:
-            index: {relabel_input_index}
-        '''
-        #NOTE: we name the parameter index for alignment with the corresponding Frame method
-        own_index = False
-        if index is IndexAutoFactory:
-            index_init = None
-        elif index is None:
-            index_init = self._index
-        elif is_callable_or_mapping(index):
-            index_init = self._index.relabel(index)
-            own_index = True
-        elif isinstance(index, Set):
-            raise RelabelInvalid()
-        else:
-            index_init = index #type: ignore
-
-        return self.__class__(self._values, # no change to Buses
-                index=index_init, # pyright: ignore
-                deepcopy_from_bus=self._deepcopy_from_bus,
-                hierarchy=self._hierarchy, # no change
-                own_index=own_index,
-                )
-
-    @doc_inject(selector='relabel_flat', class_name='Yarn')
-    def relabel_flat(self) -> tp.Self:
-        '''
-        {doc}
-        '''
-        if not isinstance(self._index, IndexHierarchy):
-            raise RuntimeError('cannot flatten an Index that is not an IndexHierarchy')
-
-        return self.__class__(self._values, # no change to Buses
-                index=self._index.flat(),
-                deepcopy_from_bus=self._deepcopy_from_bus,
-                hierarchy=self._hierarchy, # no change
-                own_index=True,
-                )
-
-    @doc_inject(selector='relabel_level_add', class_name='Yarn')
-    def relabel_level_add(self,
-            level: TLabel
-            ) -> tp.Self:
-        '''
-        {doc}
-
-        Args:
-            level: {level}
-        '''
-        return self.__class__(self._values, # no change to Buses
-                index=self._index.level_add(level),
-                deepcopy_from_bus=self._deepcopy_from_bus,
-                hierarchy=self._hierarchy, # no change
-                own_index=True,
-                )
-
-    @doc_inject(selector='relabel_level_drop', class_name='Yarn')
-    def relabel_level_drop(self,
-            count: int = 1
-            ) -> tp.Self:
-        '''
-        {doc}
-
-        Args:
-            count: {count}
-        '''
-        if not isinstance(self._index, IndexHierarchy):
-            raise RuntimeError('cannot drop level of an Index that is not an IndexHierarchy')
-
-        return self.__class__(self._values, # no change to Buses
-                index=self._index.level_drop(count),
-                deepcopy_from_bus=self._deepcopy_from_bus,
-                hierarchy=self._hierarchy, # no change
-                own_index=True,
-                )
-
-    def rehierarch(self,
-            depth_map: tp.Sequence[int],
-            *,
-            index_constructors: TIndexCtorSpecifiers = None,
-            ) -> tp.Self:
-        '''
-        Return a new :obj:`Series` with new a hierarchy based on the supplied ``depth_map``.
-        '''
-        if self.index.depth == 1:
-            raise RuntimeError('cannot rehierarch when there is no hierarchy')
-
-        index, iloc_map = rehierarch_from_index_hierarchy(
-                labels=self._index, #type: ignore
-                depth_map=depth_map,
-                index_constructors=index_constructors,
-                name=self._index.name,
-                )
-
-        return self._extract_iloc(iloc_map).relabel(index) # type: ignore
-
-
 TYarnAny = Yarn[tp.Any]
```

### Comparing `static-frame-2.5.2/static_frame/test/test_case.py` & `static-frame-2.6.0/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_archive_npy.py` & `static-frame-2.6.0/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_archive_zip.py` & `static-frame-2.6.0/static_frame/test/unit/test_archive_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_axis_map.py` & `static-frame-2.6.0/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_batch.py` & `static-frame-2.6.0/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_bus.py` & `static-frame-2.6.0/static_frame/test/unit/test_bus.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,14 +392,29 @@
 
             self.assertEqual(b2.keys().values.tolist(), ['f1', 'f2', 'f3', 'f4'])
             self.assertFalse(b2._loaded.any())
             # accessing values forces loading all
             self.assertEqual(b2.values[2].name, 'f3')
             self.assertTrue(b2._loaded_all)
 
+
+    def test_bus_iter_a(self) -> None:
+        f1 = Frame.from_dict(
+                dict(a=(1,2), b=(3,4)),
+                index=('x', 'y'),
+                name='f1')
+        f2 = Frame.from_dict(
+                dict(c=(1,2,3), b=(4,5,6)),
+                index=('x', 'y', 'z'),
+                name='f2')
+        b1 = Bus.from_frames((f1, f2))
+        biter = iter(b1)
+        self.assertEqual(next(biter), 'f1')
+        self.assertEqual(next(biter), 'f2')
+
     def test_bus_reversed_a(self) -> None:
         f1 = Frame.from_dict(
                 dict(a=(1,2), b=(3,4)),
                 index=('x', 'y'),
                 name='f1')
         f2 = Frame.from_dict(
                 dict(c=(1,2,3), b=(4,5,6)),
```

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_container.py` & `static-frame-2.6.0/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_container_util.py` & `static-frame-2.6.0/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_display.py` & `static-frame-2.6.0/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_display_color.py` & `static-frame-2.6.0/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_doc.py` & `static-frame-2.6.0/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-2.6.0/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_frame.py` & `static-frame-2.6.0/static_frame/test/unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_frame_he.py` & `static-frame-2.6.0/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_frame_iter.py` & `static-frame-2.6.0/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_frame_join.py` & `static-frame-2.6.0/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-2.6.0/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_frame_via_re.py` & `static-frame-2.6.0/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_hloc.py` & `static-frame-2.6.0/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_index.py` & `static-frame-2.6.0/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_index_auto.py` & `static-frame-2.6.0/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_index_base.py` & `static-frame-2.6.0/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_index_correspondence.py` & `static-frame-2.6.0/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_index_datetime.py` & `static-frame-2.6.0/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-2.6.0/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-2.6.0/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_interface.py` & `static-frame-2.6.0/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_loc_map.py` & `static-frame-2.6.0/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_memory_measure.py` & `static-frame-2.6.0/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-2.6.0/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files 1% similar despite different names*

```diff
@@ -572,14 +572,15 @@
 
         y = Yarn((b1, b2))
         seen: tp.Set[int] = set()
         self.assertEqual(memory_total(y), sum(memory_total(e, seen=seen) for e in (
             y._values,
             y._hierarchy,
             y._index,
+            y._indexer,
             y._deepcopy_from_bus,
         )) + getsizeof(y))
 
     #---------------------------------------------------------------------------
     # Quilt
 
     def test_getsizeof_total_quilt_simple_before_columns(self) -> None:
```

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_metadata.py` & `static-frame-2.6.0/static_frame/test/unit/test_metadata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_pivot.py` & `static-frame-2.6.0/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-2.6.0/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_quilt.py` & `static-frame-2.6.0/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_rank.py` & `static-frame-2.6.0/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_series.py` & `static-frame-2.6.0/static_frame/test/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_series_he.py` & `static-frame-2.6.0/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_store.py` & `static-frame-2.6.0/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_store_filter.py` & `static-frame-2.6.0/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_store_hdf5.py` & `static-frame-2.6.0/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_store_sqlite.py` & `static-frame-2.6.0/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_store_xlsx.py` & `static-frame-2.6.0/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_store_zip.py` & `static-frame-2.6.0/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_style_config.py` & `static-frame-2.6.0/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_type_blocks.py` & `static-frame-2.6.0/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_type_clinic.py` & `static-frame-2.6.0/static_frame/test/unit/test_type_clinic.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_util.py` & `static-frame-2.6.0/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_www.py` & `static-frame-2.6.0/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.2/static_frame/test/unit/test_yarn.py` & `static-frame-2.6.0/static_frame/test/unit/test_yarn.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from static_frame import HLoc
 from static_frame import ILoc
 from static_frame.core.bus import Bus
 from static_frame.core.display_config import DisplayConfig
 from static_frame.core.exception import ErrorInitYarn
 from static_frame.core.exception import RelabelInvalid
 from static_frame.core.frame import Frame
+from static_frame.core.index import Index
 from static_frame.core.index_auto import IndexAutoFactory
 from static_frame.core.index_datetime import IndexDate
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.series import Series
 from static_frame.core.yarn import Yarn
 from static_frame.test.test_case import TestCase
 from static_frame.test.test_case import temp_file
@@ -90,14 +91,23 @@
         b1 = Bus.from_frames((ff.parse("s(3,3)").rename("f1"),))
         b2 = Bus.from_frames((ff.parse("s(3,4)").rename("f2"),))
         b3 = Bus.from_frames((ff.parse("s(3,2)").rename("f3"),))
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False)
         self.assertEqual(y1.index.values.tolist(), ['f1', 'f2', 'f3'])
         self.assertEqual(y1['f3'].shape, (3, 2))
 
+    def test_yarn_init_f(self) -> None:
+        b1 = Bus.from_frames((ff.parse("s(3,3)").rename("f1"),))
+        b2 = Bus.from_frames((ff.parse("s(3,4)").rename("f2"),))
+
+        with self.assertRaises(ErrorInitYarn):
+            y1 = Yarn((b1, b2), indexer=np.array([2, 1, 4]))
+
+
+
 
     #---------------------------------------------------------------------------
 
     def test_yarn_from_buses_a(self) -> None:
 
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
@@ -160,15 +170,14 @@
         b1 = Bus.from_frames((f1, f2, f3))
         b2 = Bus.from_frames((f4, f5, f6))
 
         with temp_file('.zip') as fp1, temp_file('.zip') as fp2:
             b1.to_zip_pickle(fp1)
             b2.to_zip_pickle(fp2)
 
-
             bus_a = Bus.from_zip_pickle(fp1, max_persist=1).rename('a')
             bus_b = Bus.from_zip_pickle(fp2, max_persist=1).rename('b')
 
             y1 = Yarn.from_buses((bus_a, bus_b), retain_labels=False)
             self.assertEqual(y1.nbytes, 0)
             self.assertEqual(y1.status['loaded'].sum(), 0)
 
@@ -176,14 +185,15 @@
             self.assertEqual(y1['f6'].shape, (6, 4))
             self.assertEqual(y1.nbytes, 352)
             self.assertEqual(y1.status['loaded'].sum(), 2)
 
             self.assertEqual(y1.shapes.to_pairs(),
                     (('f1', None), ('f2', (4, 5)), ('f3', None), ('f4', None), ('f5', None), ('f6', (6, 4)))
                     )
+
             self.assertEqual(y1.mloc.isna().sum(), 4)
             self.assertEqual((y1.dtypes == float).sum().sum(), 9)
 
     #---------------------------------------------------------------------------
 
     def test_yarn_from_concat_a(self) -> None:
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
@@ -237,14 +247,127 @@
     def test_yarn_from_concat_c(self) -> None:
         f1 = ff.parse('s(4,2)').rename('f1')
         f2 = ff.parse('s(4,5)').rename('f2')
 
         with self.assertRaises(NotImplementedError):
             Yarn.from_concat((f1, f2))
 
+    def test_yarn_from_concat_d(self) -> None:
+        f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
+        f2 = ff.parse('s(4,4)|v(str)').rename('f2')
+        f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
+        b1 = Bus.from_frames((f1, f2, f3))
+
+        f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
+        f5 = ff.parse('s(4,4)|v(str)').rename('f5')
+        b2 = Bus.from_frames((f4, f5))
+
+        f6 = ff.parse('s(2,4)|v(int,float)').rename('f6')
+        f7 = ff.parse('s(4,2)|v(str)').rename('f7')
+        b3 = Bus.from_frames((f6, f7))
+
+
+        y1 = Yarn.from_buses((b1,), retain_labels=False)
+        y2 = Yarn.from_buses((b2, b3), retain_labels=False)
+
+        y3 = y1[['f2']]
+        y4 = y2[['f7']]
+
+        y5 = Yarn.from_concat((y3, y4))
+        self.assertEqual(y5.shape, (2,))
+        self.assertEqual(y5.index.values.tolist(), ['f2', 'f7'])
+        self.assertEqual(len(y5._values), 3) # all bus are retained
+        self.assertEqual(len(y5._hierarchy), 7) # concat of all found
+
+
+    def test_yarn_from_concat_e(self) -> None:
+        f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
+        f2 = ff.parse('s(4,4)|v(str)').rename('f2')
+        f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
+        b1 = Bus.from_frames((f1, f2, f3))
+
+        f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
+        f5 = ff.parse('s(4,4)|v(str)').rename('f5')
+        b2 = Bus.from_frames((f4, f5))
+
+        f6 = ff.parse('s(2,4)|v(int,float)').rename('f6')
+        f7 = ff.parse('s(4,2)|v(str)').rename('f7')
+        b3 = Bus.from_frames((f6, f7))
+
+        f8 = ff.parse('s(2,4)|v(int,float)').rename('f8')
+        f9 = ff.parse('s(4,2)|v(str)').rename('f9')
+        f10 = ff.parse('s(4,2)|v(str)').rename('f10')
+        b4 = Bus.from_frames((f8, f9, f10))
+
+        f11 = ff.parse('s(4,4)|v(int,float)').rename('f11')
+        f12 = ff.parse('s(4,4)|v(str)').rename('f12')
+        b5 = Bus.from_frames((f11, f12))
+
+        f13 = ff.parse('s(2,4)|v(int,float)').rename('f13')
+        f14 = ff.parse('s(4,2)|v(str)').rename('f14')
+        b6 = Bus.from_frames((f13, f14))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = Yarn.from_buses((b3, b4), retain_labels=False)
+        y3 = Yarn.from_buses((b5, b6), retain_labels=False)
+
+        yc1 = y1[['f2', 'f4', 'f1']]
+        yc2 = y2[['f7', 'f6']]
+        yc3 = y3[['f14', 'f12']]
+
+        yp = Yarn.from_concat((yc1, yc2, yc3))
+
+        self.assertEqual(yp.shape, (7,))
+        self.assertEqual(yp.index.values.tolist(), ['f2', 'f4', 'f1', 'f7', 'f6', 'f14', 'f12'])
+        self.assertEqual(len(yp._values), 6) # all bus are retained
+        self.assertEqual(len(yp._hierarchy), 14) # concat of all found
+
+
+    def test_yarn_from_concat_f(self) -> None:
+        f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
+        f2 = ff.parse('s(4,4)|v(str)').rename('f2')
+        f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
+        b1 = Bus.from_frames((f1, f2, f3))
+
+        f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
+        f5 = ff.parse('s(4,4)|v(str)').rename('f5')
+        b2 = Bus.from_frames((f4, f5))
+
+        f6 = ff.parse('s(2,4)|v(int,float)').rename('f6')
+        f7 = ff.parse('s(4,2)|v(str)').rename('f7')
+        b3 = Bus.from_frames((f6, f7))
+
+        f8 = ff.parse('s(2,4)|v(int,float)').rename('f8')
+        f9 = ff.parse('s(4,2)|v(str)').rename('f9')
+        f10 = ff.parse('s(4,2)|v(str)').rename('f10')
+        b4 = Bus.from_frames((f8, f9, f10))
+
+        f11 = ff.parse('s(4,4)|v(int,float)').rename('f11')
+        f12 = ff.parse('s(4,4)|v(str)').rename('f12')
+        b5 = Bus.from_frames((f11, f12))
+
+        f13 = ff.parse('s(2,4)|v(int,float)').rename('f13')
+        f14 = ff.parse('s(4,2)|v(str)').rename('f14')
+        b6 = Bus.from_frames((f13, f14))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = Yarn.from_buses((b3, b4), retain_labels=False)
+        y3 = Yarn.from_buses((b5, b6), retain_labels=False)
+
+        yc1 = y1['f3': 'f5']
+        yc2 = y2['f9':]
+        yc3 = y3[['f14', 'f11']]
+
+        yp = Yarn.from_concat((yc1, yc2, yc3))
+
+        self.assertEqual(yp.shape, (7,))
+        self.assertEqual(yp.index.values.tolist(), ['f3', 'f4', 'f5', 'f9', 'f10', 'f14', 'f11'])
+        self.assertEqual(len(yp._values), 6) # all bus are retained
+        self.assertEqual(len(yp._hierarchy), 14) # concat of all found
+
     #---------------------------------------------------------------------------
 
     def test_yarn_reversed_a(self) -> None:
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
         b1 = Bus.from_frames((f1, f2, f3), name='a')
@@ -371,35 +494,35 @@
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=True, name='foo')
         y2 = y1.loc[[('a', 'f3'), ('b', 'f5'), ('c', 'f6')]]
         self.assertEqual(y2.shapes.to_pairs(),
                 ((('a', 'f3'), (4, 4)), (('b', 'f5'), (4, 4)), (('c', 'f6'), (2, 4))))
 
     def test_yarn_loc_d(self) -> None:
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
-        f2 = ff.parse('s(4,4)|v(str)').rename('f2')
-        f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
+        f2 = ff.parse('s(4,3)|v(str)').rename('f2')
+        f3 = ff.parse('s(4,5)|v(bool)').rename('f3')
         b1 = Bus.from_frames((f1, f2, f3), name='a')
 
-        f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
-        f5 = ff.parse('s(4,4)|v(str)').rename('f5')
+        f4 = ff.parse('s(3,4)|v(int,float)').rename('f4')
+        f5 = ff.parse('s(3,2)|v(str)').rename('f5')
         b2 = Bus.from_frames((f4, f5), name='b')
 
         f6 = ff.parse('s(2,4)|v(int,float)').rename('f6')
-        f7 = ff.parse('s(4,2)|v(str)').rename('f7')
+        f7 = ff.parse('s(2,8)|v(str)').rename('f7')
         b3 = Bus.from_frames((f6, f7), name='c')
 
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False, name='foo')
         y2 = y1.loc[['f7', 'f3']]
         self.assertEqual(y2.shapes.to_pairs(),
-                (('f7', (4, 2)), ('f3', (4, 4)))
+                (('f7', (2, 8)), ('f3', (4, 5)))
                 )
 
-        y2 = y1.loc[['f1', 'f7', 'f3']]
-        self.assertEqual(y2.shapes.to_pairs(),
-                (('f1', (4, 4)), ('f7', (4, 4)), ('f3', (4, 2)))
+        y3 = y1.loc[['f1', 'f7', 'f3']]
+        self.assertEqual(y3.shapes.to_pairs(),
+                (('f1', (4, 4)), ('f7', (2, 8)), ('f3', (4, 5)))
                 )
 
     def test_yarn_loc_e(self) -> None:
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
         b1 = Bus.from_frames((f1, f2, f3), name='a')
@@ -438,14 +561,51 @@
         self.assertEqual(y2.shapes.to_pairs(),
                 ((('a', 'f3'), (4, 5)), (('c', 'f6'), (2, 4))))
 
         y3 = y1.loc[HLoc[['a', 'c']]]
         self.assertEqual(y3.shapes.to_pairs(),
                 ((('a', 'f1'), (4, 4)), (('a', 'f2'), (3, 4)), (('a', 'f3'), (4, 5)), (('c', 'f6'), (2, 4)), (('c', 'f7'), (4, 2))))
 
+    def test_yarn_loc_g(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+
+        y2 = y1[['f3', 'f1', 'f4']]
+        self.assertEqual(y2.index.values.tolist(), ['f3', 'f1', 'f4'])
+        self.assertEqual(y2.index.values.tolist(), [f.name for f in y2.values])
+
+        y3 = y2[['f1', 'f3', 'f4']]
+        self.assertEqual(y3.index.values.tolist(), ['f1', 'f3', 'f4'])
+        self.assertEqual(y3.index.values.tolist(), [f.name for f in y3.values])
+
+    def test_yarn_loc_h(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+
+        y2 = y1[['f1', 'f2']]
+        self.assertEqual(y2.index.values.tolist(), ['f1', 'f2'])
+        self.assertEqual([f.name for f in y2.values], ['f1', 'f2'])
+        self.assertIsNone(y2._values[1]) # removed Bus
+        # we keep an old hierarchy
+        self.assertTrue(y2._hierarchy.equals(y1._hierarchy))
+
     #---------------------------------------------------------------------------
 
     def test_yarn_iloc_a(self) -> None:
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
         b1 = Bus.from_frames((f1, f2, f3), name='a')
@@ -517,14 +677,34 @@
         f6 = ff.parse('s(2,4)|v(int,float)').rename('f6')
         f7 = ff.parse('s(4,2)|v(str)').rename('f7')
         b3 = Bus.from_frames((f6, f7), name='c')
 
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False, name='foo')
         self.assertTrue('f6' in y1)
 
+    def test_yarn_contains_b(self) -> None:
+        f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
+        f2 = ff.parse('s(4,4)|v(str)').rename('f2')
+        f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
+        b1 = Bus.from_frames((f1, f2, f3))
+
+        f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
+        f5 = ff.parse('s(4,4)|v(str)').rename('f5')
+        b2 = Bus.from_frames((f4, f5))
+
+        f6 = ff.parse('s(2,4)|v(int,float)').rename('f6')
+        f7 = ff.parse('s(4,2)|v(str)').rename('f7')
+        b3 = Bus.from_frames((f6, f7))
+
+        y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False, name='foo')
+        y2 = y1[['f6', 'f4']]
+        self.assertTrue('f6' in y2) # pylint: disable=E1135
+        self.assertTrue('f4' in y2) # pylint: disable=E1135
+        self.assertFalse('f3' in y2) # pylint: disable=E1135
+
     #---------------------------------------------------------------------------
 
     def test_yarn_get_a(self) -> None:
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
         b1 = Bus.from_frames((f1, f2, f3), name='a')
@@ -557,14 +737,37 @@
         f7 = ff.parse('s(4,2)|v(str)').rename('f7')
         b3 = Bus.from_frames((f6, f7), name='c')
 
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False, name='foo')
         self.assertEqual(y1.head(2).shape, (2,))
         self.assertEqual(tuple(y1.head(2).keys()), ('f1', 'f2'))
 
+    def test_yarn_head_b(self) -> None:
+        f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
+        f2 = ff.parse('s(4,3)|v(str)').rename('f2')
+        f3 = ff.parse('s(4,2)|v(bool)').rename('f3')
+        b1 = Bus.from_frames((f1, f2, f3))
+
+        f4 = ff.parse('s(3,4)|v(int,float)').rename('f4')
+        f5 = ff.parse('s(3,5)|v(str)').rename('f5')
+        b2 = Bus.from_frames((f4, f5))
+
+        f6 = ff.parse('s(2,4)|v(int,float)').rename('f6')
+        f7 = ff.parse('s(2,2)|v(str)').rename('f7')
+        b3 = Bus.from_frames((f6, f7))
+
+        y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False, name='foo')
+        y2 = y1[['f7', 'f1', 'f6']]
+        self.assertEqual(y2.index.values.tolist(), ['f7', 'f1', 'f6'])
+        self.assertEqual([f.name for f in y2.values], ['f7', 'f1', 'f6'])
+
+        y3 = y2.head(2)
+        self.assertEqual(y3.shape, (2,))
+        self.assertEqual(tuple(y3.keys()), ('f7', 'f1'))
+
     #---------------------------------------------------------------------------
 
     def test_yarn_tail_a(self) -> None:
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
         b1 = Bus.from_frames((f1, f2, f3), name='a')
@@ -662,28 +865,70 @@
 
         b1 = Bus.from_frames((f1, f2), name='a')
         b2 = Bus.from_frames((f3, f4), name='b')
 
         y1 = Yarn.from_buses((b1, b2), retain_labels=False)
         self.assertEqual(y1.mloc.shape, (4,))
 
+    def test_yarn_mloc_b(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = y1[['f4', 'f2']]
+        self.assertEqual(y2.mloc.shape, (2,))
+
+    def test_yarn_mloc_c(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = y1[['f3']]
+        self.assertEqual(y2.mloc.shape, (1,))
+
+
+
     #---------------------------------------------------------------------------
 
     def test_yarn_dtypes_a(self) -> None:
         f1 = ff.parse('s(4,2)').rename('f1')
         f2 = ff.parse('s(4,5)').rename('f2')
         f3 = ff.parse('s(2,2)').rename('f3')
         f4 = ff.parse('s(2,8)').rename('f4')
 
         b1 = Bus.from_frames((f1, f2), name='a')
         b2 = Bus.from_frames((f3, f4), name='b')
 
         y1 = Yarn.from_buses((b1, b2), retain_labels=False)
         self.assertEqual(y1.dtypes.shape, (4, 8))
 
+    def test_yarn_dtypes_b(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2), name='a')
+        b2 = Bus.from_frames((f3, f4), name='b')
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = y1[['f4', 'f1']]
+        self.assertEqual(y2.dtypes.shape, (2, 8))
+
+
     #---------------------------------------------------------------------------
 
     def test_yarn_shapes_a(self) -> None:
         f1 = ff.parse('s(4,2)').rename('f1')
         f2 = ff.parse('s(4,5)').rename('f2')
         f3 = ff.parse('s(2,2)').rename('f3')
         f4 = ff.parse('s(2,8)').rename('f4')
@@ -865,14 +1110,30 @@
         self.assertEqual(s1.to_pairs(),
                 (('f1', (4, 2)), ('f2', (4, 5)), ('f3', (2, 2)), ('f4', (2, 8)), ('f5', (4, 4)), ('f6', (6, 4))))
 
         self.assertEqual([f.name for f in y1.iter_element() if f.shape[0] > 2], #type: ignore
                 ['f1', 'f2', 'f5', 'f6'],
                 )
 
+    def test_yarn_iter_element_b(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+        f5 = ff.parse('s(4,4)').rename('f5')
+        f6 = ff.parse('s(6,4)').rename('f6')
+
+        b1 = Bus.from_frames((f1, f2, f3), name='b1')
+        b2 = Bus.from_frames((f4, f5, f6), name='b2')
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+
+        y2 = y1[['f5', 'f1', 'f4']]
+        post = list(y2.iter_element())
+        self.assertEqual(len(post), 3)
+
     #---------------------------------------------------------------------------
 
     def test_yarn_iter_element_items_a(self) -> None:
         f1 = ff.parse('s(4,2)').rename('f1')
         f2 = ff.parse('s(4,5)').rename('f2')
         f3 = ff.parse('s(2,2)').rename('f3')
         f4 = ff.parse('s(2,8)').rename('f4')
@@ -906,15 +1167,14 @@
         b1 = Bus.from_frames((f1, f2, f3), name='b1')
         b2 = Bus.from_frames((f4,), name='b2')
         b3 = Bus.from_frames((f5, f6), name='b3')
 
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False)
 
         y2 = y1.drop['f3':'f5'] #type: ignore
-        self.assertEqual(len(y2._values), 2) # 2 buses remain
         self.assertEqual([(f.name, f.shape) for f in y2.values],
                 [('f1', (4, 2)), ('f2', (4, 5)), ('f6', (6, 4))]
                 )
 
         y3 = y1.drop[y1.index.isin(('f1', 'f6'))]
         self.assertEqual([(f.name, f.shape) for f in y3.values],
                 [('f2', (4, 5)), ('f3', (2, 2)), ('f4', (2, 8)), ('f5', (4, 4))]
@@ -941,15 +1201,14 @@
         b1 = Bus.from_frames((f1, f2, f3), name='b1')
         b2 = Bus.from_frames((f4,), name='b2')
         b3 = Bus.from_frames((f5, f6), name='b3')
 
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False)
 
         y2 = y1.drop.iloc[2: 5]
-        self.assertEqual(len(y2._values), 2) # 2 buses remain
         self.assertEqual([(f.name, f.shape) for f in y2.values],
                 [('f1', (4, 2)), ('f2', (4, 5)), ('f6', (6, 4))]
                 )
 
         y3 = y1.drop.iloc[np.array([True, False, False, False, False, True])]
         self.assertEqual([(f.name, f.shape) for f in y3.values],
                 [('f2', (4, 5)), ('f3', (2, 2)), ('f4', (2, 8)), ('f5', (4, 4))]
@@ -1165,15 +1424,15 @@
 
         a1 = np.array((1, 2, 3), dtype=np.int64)
         a1.flags.writeable = False
         y1 = Yarn((b1, b2, b3), index=IndexHierarchy.from_product(('a', 'b'), a1))
 
         bytes1 = y1._to_signature_bytes(include_name=False)
         self.assertEqual(sha256(bytes1).hexdigest(),
-            '0a6978231ec671903449e39ae465747a68a0da8492e9b5b5fcf4dc98afb8143e')
+            '4f080dceb07b959487a84134447e0e838754ac45246975080b9fc8bc85829bc6')
 
     def test_yarn_to_signature_bytes_b(self) -> None:
         f1 = ff.parse('s(4,2)').rename('f1')
         f2 = ff.parse('s(4,5)').rename('f2')
         f3 = ff.parse('s(2,2)').rename('f3')
         f4 = ff.parse('s(2,8)').rename('f4')
         f5 = ff.parse('s(4,4)').rename('f5')
@@ -1210,29 +1469,254 @@
         bytes1 = y1._to_signature_bytes(include_name=False)
 
         y2 = Yarn((b1, b2, b4))
         bytes2 = y2._to_signature_bytes(include_name=False)
 
         self.assertNotEqual(sha256(bytes1).hexdigest(), sha256(bytes2).hexdigest())
 
+    def test_yarn_to_signature_bytes_d(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+
+        b1 = Bus.from_frames((f1, f2, f3))
+        y1 = Yarn.from_buses((b1,), retain_labels=False)
+
+        # if not comparing class, the bytes of a Yarn and Bus will be the same as only index and contained frame are read
+        bytes1 = b1._to_signature_bytes(include_name=False, include_class=False)
+        bytes2 = y1._to_signature_bytes(include_name=False, include_class=False)
+
+        self.assertEqual(sha256(bytes1).hexdigest(), sha256(bytes2).hexdigest())
+
     def test_yarn_via_hashlib_a(self) -> None:
         f1 = ff.parse('s(4,2)').rename('f1')
         f2 = ff.parse('s(4,5)').rename('f2')
         f3 = ff.parse('s(2,2)').rename('f3')
         f4 = ff.parse('s(2,8)').rename('f4')
         f5 = ff.parse('s(4,4)').rename('f5')
         f6 = ff.parse('s(6,4)').rename('f6')
 
         b1 = Bus.from_frames((f1, f2, f3))
         b2 = Bus.from_frames((f4,))
         b3 = Bus.from_frames((f5, f6))
 
         y1 = Yarn((b1, b2, b3))
         digest = y1.via_hashlib(include_name=False).sha256().hexdigest()
-        self.assertEqual(digest, '694e92cccad9bc2ae2f6bf9e0cb212bfd4b0677f79c155c89ece4dcaf7311324')
+        self.assertEqual(digest, 'c966f3bfa983b696da219838197f627135b3405dc2f50c0ab29c02ed74ac3bd1')
+
+    #---------------------------------------------------------------------------
+
+    def test_yarn_sort_index_a(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f4, f2))
+        b2 = Bus.from_frames((f1, f3))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+
+        self.assertEqual(y1.shapes.to_pairs(),
+            (('f4', (2, 8)), ('f2', (4, 5)), ('f1', (4, 2)), ('f3', (2, 2))))
+
+        y2 = y1.sort_index()
+        self.assertEqual(y2.shapes.to_pairs(),
+            (('f1', (4, 2)), ('f2', (4, 5)), ('f3', (2, 2)), ('f4', (2, 8))))
+
+    #---------------------------------------------------------------------------
+
+    def test_yarn_sort_values_a(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = y1.sort_values(key=lambda y: np.array([f.size for f in y.iter_element()]))
+
+        self.assertEqual(y2.index.values.tolist(), ['f3', 'f1', 'f4', 'f2'])
+        self.assertEqual([f.name for f in y2.iter_element()], ['f3', 'f1', 'f4', 'f2'])
+
+    def test_yarn_sort_values_b(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+
+        with self.assertRaises(RuntimeError):
+            _ = y1.sort_values(key=lambda y: np.array([f.size for f in y.iter_element()]), ascending=[True, False])
+
+        y2 = y1.sort_values(key=lambda y: np.array([f.size for f in y.iter_element()]), ascending=False)
+
+        self.assertEqual(y2.index.values.tolist(), ['f2', 'f4', 'f1', 'f3'])
+        self.assertEqual([f.name for f in y2.iter_element()], ['f2', 'f4', 'f1', 'f3'])
+
+    def test_yarn_sort_values_c(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+
+        y2 = y1[['f4', 'f3']]
+
+        y3 = y2.sort_values(key=lambda y: np.array([f.size for f in y.iter_element()]))
+
+        self.assertEqual(y3.index.values.tolist(), ['f3', 'f4'])
+        self.assertEqual([f.name for f in y3.iter_element()], ['f3', 'f4'])
+
+    #---------------------------------------------------------------------------
+
+    def test_yarn_roll_a(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = y1.roll(2)
 
+        self.assertEqual(
+                [(l, f.name) for l, f in y2.items()],
+                [('f1', 'f3'), ('f2', 'f4'), ('f3', 'f1'), ('f4', 'f2')],
+                )
+
+        y3 = y1.roll(4)
+        self.assertTrue(y3.equals(y1))
+
+    def test_yarn_roll_b(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = y1.roll(2, include_index=True)
+
+        self.assertEqual(
+                [(l, f.name) for l, f in y2.items()],
+                [('f3', 'f3'), ('f4', 'f4'), ('f1', 'f1'), ('f2', 'f2')],
+                )
+
+    def test_yarn_shift_a(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        with self.assertRaises(NotImplementedError):
+            _ = y1.shift(2, fill_value=None)
+
+    #---------------------------------------------------------------------------
+
+    def test_yarn_reindex_a(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = y1.reindex(['f3', 'f1', 'f2'])
+        self.assertEqual(y2.index.values.tolist(), ['f3', 'f1', 'f2'])
+        self.assertEqual([f.name for f in y2.iter_element()], ['f3', 'f1', 'f2'])
+
+    def test_yarn_reindex_b(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        with self.assertRaises(NotImplementedError):
+            _ = y1.reindex(['f3', 'f1', 'f2', 'f8'])
+
+    def test_yarn_reindex_c(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+        y2 = y1.reindex(['f3', 'f1', 'f2', 'f4'])
+        self.assertEqual(y2.index.values.tolist(), ['f3', 'f1', 'f2', 'f4'])
+        self.assertEqual([f.name for f in y2.iter_element()], ['f3', 'f1', 'f2', 'f4'])
+
+        y3 = y2[['f4', 'f3']]
+        y4 = y3.reindex(('f3',))
+
+        self.assertEqual(y4.index.values.tolist(), ['f3'])
+        self.assertEqual([f.name for f in y4.iter_element()], ['f3'])
+
+        # y4 still retains the original hierarchyh
+        self.assertIs(y1._hierarchy, y4._hierarchy)
+
+    def test_yarn_reindex_d(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
+
+        idx = Index(['f3', 'f1', 'f2'])
+        y2 = y1.reindex(idx, own_index=True)
+        self.assertTrue(y2.index is idx)
+
+        y3 = y2.reindex(y2.index, own_index=True)
+        self.assertTrue(y3.index is idx)
+
+
+    def test_yarn_reindex_e(self) -> None:
+        f1 = ff.parse('s(4,2)').rename('f1')
+        f2 = ff.parse('s(4,5)').rename('f2')
+        f3 = ff.parse('s(2,2)').rename('f3')
+        f4 = ff.parse('s(2,8)').rename('f4')
+
+        b1 = Bus.from_frames((f1, f2))
+        b2 = Bus.from_frames((f3, f4))
+
+        y1 = Yarn.from_buses((b1, b2), retain_labels=False)
 
+        y2 = y1.reindex(())
+        self.assertEqual(len(y2), 0)
+        self.assertEqual(y2._values.tolist(), [None, None])
+        self.assertEqual(len(y2._hierarchy), 4)
 
 
 if __name__ == '__main__':
     import unittest
     unittest.main()
```

### Comparing `static-frame-2.5.2/static_frame.egg-info/PKG-INFO` & `static-frame-2.6.0/static_frame.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 2.5.2
+Version: 2.6.0
 Summary: Immutable and statically-typeable DataFrames with runtime type and data validation.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Keywords: staticframe pandas numpy immutable array
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -106,280 +106,282 @@
 ---------------------
 
 To get startred quickly, let's download the classic iris (flower) characteristics data set and build a simple naive Bayes classifier that can predict species from iris petal characteristics.
 
 While StaticFrame's API has over 7,500 endpoints, much will be familiar to users of Pandas or other DataFrame libraries. Rather than offering fewer interfaces with greater configurability, StaticFrame favors more numerous interfaces with more narrow parameters and functionality. This design leads to more maintainable code. (Read more about differences between Pandas and StaticFrame `here <https://static-frame.readthedocs.io/en/latest/articles/upgrade.html>`__.)
 
 
-We can download the data set from the UCI Machine Learning Repository and create a ``Frame``. StaticFrame exposes all constructors on the class: here, we will use the ``Frame.from_csv()`` constructor. To download a file from the internet and provide it to a constructor, we can use StaticFrame's ``WWW.from_file()`` interface.
+We can download the data set from the UCI Machine Learning Repository and create a ``Frame``. StaticFrame exposes all constructors on the class: here, we will use the ``Frame.from_csv()`` constructor. To download a file from the internet and provide it to a constructor, we can use StaticFrame's ``WWW.from_file()`` interface::
 
->>> import static_frame as sf
->>> data = sf.Frame.from_csv(sf.WWW.from_file('https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'), columns_depth=0)
+    >>> import static_frame as sf
+    >>> data = sf.Frame.from_csv(sf.WWW.from_file('https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data'), columns_depth=0)
 
 
-Each record (or row) in this dataset describes observations of an iris flower, including its sepal and petal characteristics, as well as its species (of which there are three). To display just the first few rows, we can use the ``head()`` method. Notice that StaticFrame's default display makes it very clear what type of ``Frame``, ``Index``, and NumPy datatypes are present.
+Each record (or row) in this dataset describes observations of an iris flower, including its sepal and petal characteristics, as well as its species (of which there are three). To display just the first few rows, we can use the ``head()`` method. Notice that StaticFrame's default display makes it very clear what type of ``Frame``, ``Index``, and NumPy datatypes are present::
 
->>> data.head()
-<Frame>
-<Index> 0         1         2         3         4           <int64>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-1       4.9       3.0       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
+    >>> data.head()
+    <Frame>
+    <Index> 0         1         2         3         4           <int64>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    1       4.9       3.0       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
 
 As the columns are unlabelled, let's next add column labels. StaticFrame supports reindexing (conforming existing axis labels to new labels, potentially changing the size and ordering) and relabeling (simply applying new labels without regard to existing labels). As we can ignore the default column labels (auto-incremented integers), the ``relabel()`` method is used to provide new labels.
 
-Note that while ``relabel()`` creates a new ``Frame``, underlying NumPy data is not copied. As all NumPy data is immutable in StaticFrame, we can reuse it in our new container, making such operations very efficient. (Read more about no-copy operations `here <https://static-frame.readthedocs.io/en/latest/articles/no_copy.html>`__.)
+Note that while ``relabel()`` creates a new ``Frame``, underlying NumPy data is not copied. As all NumPy data is immutable in StaticFrame, we can reuse it in our new container, making such operations very efficient::
 
+    >>> data = data.relabel(columns=('sepal_l', 'sepal_w', 'petal_l', 'petal_w', 'species'))
+    >>> data.head()
+    <Frame>
+    <Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    1       4.9       3.0       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
->>> data = data.relabel(columns=('sepal_l', 'sepal_w', 'petal_l', 'petal_w', 'species'))
->>> data.head()
-<Frame>
-<Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-1       4.9       3.0       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
 
+(Read more about no-copy operations `here <https://static-frame.readthedocs.io/en/latest/articles/no_copy.html>`__.)
 
 For this example, eighty percent of the data will be used to train the classifier; the remaining twenty percent will be used to test the classifier. As all records are labelled with the known species, we can conclude by measuring the effectiveness of the classifier on the test data.
 
-To divide the data into two groups, we create a ``Series`` of contiguous integers and then extract a random selection of 80% of the values into a new ``Series``, here named ``sel_train``. This will be used to select our traning data. As the ``sample()`` method, given a count, randomly samples that many values, your results will be different unless use the same ``seed`` argument.
+To divide the data into two groups, we create a ``Series`` of contiguous integers and then extract a random selection of 80% of the values into a new ``Series``, here named ``sel_train``. This will be used to select our traning data. As the ``sample()`` method, given a count, randomly samples that many values, your results will be different unless use the same ``seed`` argument::
 
->>> sel = sf.Series(np.arange(len(data)))
->>> sel_train = sel.sample(round(len(data) * .8), seed=42)
->>> sel_train.head()
-<Series>
-<Index>
-0        0
-2        2
-3        3
-4        4
-5        5
-<int64>  <int64>
-
-We will create another ``Series`` to select the test data. The ``drop[]`` interface can be used to create a new ``Series`` that excludes the training selections, leaving just the testing selections. As with many interfaces in StaticFrame (such as ``astype`` and ``assign``), brackets can be used to do ``loc[]`` style selections.
-
->>> sel_test = sel.drop[sel_train]
->>> sel_test.head()
-<Series>
-<Index>
-1        1
-14       14
-20       20
-21       21
-37       37
-<int64>  <int64>
-
-
-To select a subset of the data for training, the ``sel_train`` ``Series`` can be passed to ``loc[]`` to select just those rows.
-
->>> data_train = data.loc[sel_train]
->>> data_train.head()
-<Frame>
-<Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
-<Index>
-0       5.1       3.5       1.4       0.2       Iris-setosa
-2       4.7       3.2       1.3       0.2       Iris-setosa
-3       4.6       3.1       1.5       0.2       Iris-setosa
-4       5.0       3.6       1.4       0.2       Iris-setosa
-5       5.4       3.9       1.7       0.4       Iris-setosa
-<int64> <float64> <float64> <float64> <float64> <<U15>
+    >>> sel = sf.Series(np.arange(len(data)))
+    >>> sel_train = sel.sample(round(len(data) * .8), seed=42)
+    >>> sel_train.head()
+    <Series>
+    <Index>
+    0        0
+    2        2
+    3        3
+    4        4
+    5        5
+    <int64>  <int64>
+
+
+We will create another ``Series`` to select the test data. The ``drop[]`` interface can be used to create a new ``Series`` that excludes the training selections, leaving just the testing selections. As with many interfaces in StaticFrame (such as ``astype`` and ``assign``), brackets can be used to do ``loc[]`` style selections::
+
+    >>> sel_test = sel.drop[sel_train]
+    >>> sel_test.head()
+    <Series>
+    <Index>
+    1        1
+    14       14
+    20       20
+    21       21
+    37       37
+    <int64>  <int64>
+
+
+To select a subset of the data for training, the ``sel_train`` ``Series`` can be passed to ``loc[]`` to select just those rows::
+
+    >>> data_train = data.loc[sel_train]
+    >>> data_train.head()
+    <Frame>
+    <Index> sepal_l   sepal_w   petal_l   petal_w   species     <<U7>
+    <Index>
+    0       5.1       3.5       1.4       0.2       Iris-setosa
+    2       4.7       3.2       1.3       0.2       Iris-setosa
+    3       4.6       3.1       1.5       0.2       Iris-setosa
+    4       5.0       3.6       1.4       0.2       Iris-setosa
+    5       5.4       3.9       1.7       0.4       Iris-setosa
+    <int64> <float64> <float64> <float64> <float64> <<U15>
 
 
 With our data divided into two randomly-selected, non-overlapping groups, we can proceed to implement the naive Bayes classifier. We will compute the ``posterior`` of the test data by multiplying the ``prior`` and the ``likelihood``. With the ``posterior``, we can determine which species the classifier has calculated is most likely. (More on naive Bayes classifiers can be found `here <https://en.wikipedia.org/wiki/Naive_Bayes_classifier>`__.)
 
 The ``prior`` is calculated as the percentage of samples of each species in the training data. This is the "normalized" count per species. To get a ``Series`` of counts per species, we can select the species column, iterate over groups based on species name, and count the size of each group.
 
 In StaticFrame, this can be done by calling ``Series.iter_group_items()`` to get an iterator of pairs of group label, group (where the group is a ``Series``). This iterator (or any similar iterator) can be given to a ``Batch``, a chaining processor of ``Frame`` or ``Series``, to perform operations on each group. (For more on the ``Batch`` and other higher-order containers in StaticFrame, see `here <https://static-frame.readthedocs.io/en/latest/articles/uhoc.html>`__.)
 
-Once the ``Batch`` is created, selections, method calls, and operator expressions can be chained as if they were being called on a single container. Processing happens to every contained container, and a container is returned, only when a finalizer method, such as ``to_series()``, is called.
+Once the ``Batch`` is created, selections, method calls, and operator expressions can be chained as if they were being called on a single container. Processing happens to every contained container, and a container is returned, only when a finalizer method, such as ``to_series()``, is called::
 
->>> counts = sf.Batch(data_train['species'].iter_group_items()).count().to_series()
->>> counts
-<Series>
-<Index>
-Iris-setosa     43
-Iris-versicolor 39
-Iris-virginica  38
-<<U15>          <int64>
-
-
-As with NumPy, StaticFrame containers can be used in expressions with binary operators. The ``prior`` can be derived by dividing ``counts`` by the size of the training data. This returns a ``Series`` of the percentage of records per species.
-
->>> prior = counts / len(data_train)
->>> prior
-<Series>
-<Index>
-Iris-setosa     0.35833333333333334
-Iris-versicolor 0.325
-Iris-virginica  0.31666666666666665
-<<U15>          <float64>
+    >>> counts = sf.Batch(data_train['species'].iter_group_items()).count().to_series()
+    >>> counts
+    <Series>
+    <Index>
+    Iris-setosa     43
+    Iris-versicolor 39
+    Iris-virginica  38
+    <<U15>          <int64>
+
+
+As with NumPy, StaticFrame containers can be used in expressions with binary operators. The ``prior`` can be derived by dividing ``counts`` by the size of the training data. This returns a ``Series`` of the percentage of records per species::
+
+    >>> prior = counts / len(data_train)
+    >>> prior
+    <Series>
+    <Index>
+    Iris-setosa     0.35833333333333334
+    Iris-versicolor 0.325
+    Iris-virginica  0.31666666666666665
+    <<U15>          <float64>
 
 
 Having calculated the ``prior``, we can calculate ``likelihood`` next. To calculate ``likelihood``, we will call a probability distribution function (imported from SciPy) with the test data, once for each species, given the characteristics (mean and standard deviation) observed in the test data for that species.
 
-The ``Batch`` can again be used to calculate the mean and standard deviation, per species, from the training data. With the ``Frame`` of training data, we call ``iter_group_items()`` to group by species and, passing that iterator to ``Batch``, call ``mean()`` (assigned to ``mu``) or ``std()`` (assigned to ``sigma``). Note that ``iter_group_items()`` has an optional ``drop`` parameter to remove the column used for grouping from subsequent operations.
+The ``Batch`` can again be used to calculate the mean and standard deviation, per species, from the training data. With the ``Frame`` of training data, we call ``iter_group_items()`` to group by species and, passing that iterator to ``Batch``, call ``mean()`` (assigned to ``mu``) or ``std()`` (assigned to ``sigma``). Note that ``iter_group_items()`` has an optional ``drop`` parameter to remove the column used for grouping from subsequent operations::
 
 
->>> mu = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).mean().to_frame()
->>> mu
-<Frame>
-<Index>         sepal_l            sepal_w            <<U7>
-<Index>
-Iris-setosa     4.986046511627907  3.434883720930233
-Iris-versicolor 5.920512820512819  2.771794871794872
-Iris-virginica  6.6078947368421055 2.9763157894736842
-<<U15>          <float64>          <float64>
-
->>> sigma = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).std(ddof=1).to_frame()
->>> sigma
-<Frame>
-<Index>         sepal_l            sepal_w             <<U7>
-<Index>
-Iris-setosa     0.3419700595003668 0.3477024733400345
-Iris-versicolor 0.508444214804487  0.33082728674826684
-Iris-virginica  0.6055516042229233 0.3513942965328924
-<<U15>          <float64>          <float64>
-
-
-For a unified display of these characteristics, we can build a hierarchical index on each ``Frame`` with ``relabel_level_add()`` (adding the "mu" or "sigma" labels), then vertically concatenate the tables. As StaticFrame always requires unique labels in indices, adding an additional label is required before concatenation. The built-in ``round`` function can be used for more tidy display.
-
->>> stats = sf.Frame.from_concat((mu.relabel_level_add('mu'), sigma.relabel_level_add('sigma')))
->>> round(stats, 2)
-<Frame>
-<Index>                          sepal_l   sepal_w   <<U7>
-<IndexHierarchy>
-mu               Iris-setosa     4.99      3.43
-mu               Iris-versicolor 5.92      2.77
-mu               Iris-virginica  6.61      2.98
-sigma            Iris-setosa     0.34      0.35
-sigma            Iris-versicolor 0.51      0.33
-sigma            Iris-virginica  0.61      0.35
-<<U5>            <<U15>          <float64> <float64>
+    >>> mu = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).mean().to_frame()
+    >>> mu
+    <Frame>
+    <Index>         sepal_l            sepal_w            <<U7>
+    <Index>
+    Iris-setosa     4.986046511627907  3.434883720930233
+    Iris-versicolor 5.920512820512819  2.771794871794872
+    Iris-virginica  6.6078947368421055 2.9763157894736842
+    <<U15>          <float64>          <float64>
+
+    >>> sigma = sf.Batch(data_train[['sepal_l', 'sepal_w', 'species']].iter_group_items('species', drop=True)).std(ddof=1).to_frame()
+    >>> sigma
+    <Frame>
+    <Index>         sepal_l            sepal_w             <<U7>
+    <Index>
+    Iris-setosa     0.3419700595003668 0.3477024733400345
+    Iris-versicolor 0.508444214804487  0.33082728674826684
+    Iris-virginica  0.6055516042229233 0.3513942965328924
+    <<U15>          <float64>          <float64>
+
+
+For a unified display of these characteristics, we can build a hierarchical index on each ``Frame`` with ``relabel_level_add()`` (adding the "mu" or "sigma" labels), then vertically concatenate the tables. As StaticFrame always requires unique labels in indices, adding an additional label is required before concatenation. The built-in ``round`` function can be used for more tidy display::
+
+    >>> stats = sf.Frame.from_concat((mu.relabel_level_add('mu'), sigma.relabel_level_add('sigma')))
+    >>> round(stats, 2)
+    <Frame>
+    <Index>                          sepal_l   sepal_w   <<U7>
+    <IndexHierarchy>
+    mu               Iris-setosa     4.99      3.43
+    mu               Iris-versicolor 5.92      2.77
+    mu               Iris-virginica  6.61      2.98
+    sigma            Iris-setosa     0.34      0.35
+    sigma            Iris-versicolor 0.51      0.33
+    sigma            Iris-virginica  0.61      0.35
+    <<U5>            <<U15>          <float64> <float64>
 
 
 We can now move on to processing the test data with the characteristics derived from the training data. To do that, we will extract our previously selected test records with ``sel_test`` into a new ``Frame``, to which we can add our ``posterior`` predictions and final species classifications.
 
 It is common to process data in table by adding columns from left to right. StaticFrame permits this limited form of mutability with the grow-only ``FrameGO``. While underlying NumPy arrays are still always immutable, columns can be added to a ``FrameGO`` with bracket-style assignments. A ``FrameGO`` can be created from a ``Frame`` with the ``to_frame_go()`` method. As mentioned elsewhere, underlying immutable NumPy arrays are not copied: this is an efficient, no-copy operation.
 
-Passing two arguments to ``loc[]``, we can select rows with the values from ``sel_test``, and we can select columns with a list of labels for the sepal length and sepal width.
+Passing two arguments to ``loc[]``, we can select rows with the values from ``sel_test``, and we can select columns with a list of labels for the sepal length and sepal width::
 
->>> data_test = data.loc[sel_test.values, ['sepal_l', 'sepal_w']].to_frame_go()
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   <<U7>
-<Index>
-1         4.9       3.0
-14        5.8       4.0
-20        5.4       3.4
-21        5.1       3.7
-37        4.9       3.1
-<int64>   <float64> <float64>
+    >>> data_test = data.loc[sel_test.values, ['sepal_l', 'sepal_w']].to_frame_go()
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   <<U7>
+    <Index>
+    1         4.9       3.0
+    14        5.8       4.0
+    20        5.4       3.4
+    21        5.1       3.7
+    37        4.9       3.1
+    <int64>   <float64> <float64>
 
 
 StaticFrame interfaces make extensive use of iterators and generators. As used below, the ``Frame.from_fields()`` constructor will create a ``Frame`` from any iterable (or generator) of column arrays.
 
-The ``likelihood_of_species()`` function (defined below), for each index label in ``mu`` (which provides each unique iris species), calculates a probability density function for the test data, given the ``mu`` (mean) and ``sigma`` (standard deviation) for the species. An array of the sum of the log is yielded.
+The ``likelihood_of_species()`` function (defined below), for each index label in ``mu`` (which provides each unique iris species), calculates a probability density function for the test data, given the ``mu`` (mean) and ``sigma`` (standard deviation) for the species. An array of the sum of the log is yielded::
 
->>> from scipy.stats import norm
->>> def likelihood_of_species():
-...     for label in mu.index:
-...             pdf = norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])
-...             yield np.log(pdf).sum(axis=1)
+    >>> from scipy.stats import norm
+    >>> def likelihood_of_species():
+    ...     for label in mu.index:
+    ...             pdf = norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])
+    ...             yield np.log(pdf).sum(axis=1)
 
 
 While the generator function above is easy to read, it is hard to copy and paste. If you are following along, using the one-line generator expression, below, will be easier. The two are equivalent:
 
 >>> likelihood_of_species = (np.log(norm.pdf(data_test.values, mu.loc[label], sigma.loc[label])).sum(axis=1) for label in mu.index)
 
 
-With this generator expression defined, we call the ``from_fields`` constructor to produce the ``likelihood`` table, providing column labels from ``mu.index`` and index labels from ``data_test.index``. For each test record row we now have a likelihood per species.
+With this generator expression defined, we call the ``from_fields`` constructor to produce the ``likelihood`` table, providing column labels from ``mu.index`` and index labels from ``data_test.index``. For each test record row we now have a likelihood per species::
 
->>> likelihood = sf.Frame.from_fields(likelihood_of_species, columns=mu.index, index=data_test.index)
->>> round(likelihood.head(), 2)
-<Frame>
-<Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
-<Index>
-1       -0.52       -2.31           -4.27
-14      -3.86       -6.97           -5.42
-20      -0.45       -2.38           -3.01
-21      -0.05       -5.29           -5.51
-37      -0.2        -2.56           -4.33
-<int64> <float64>   <float64>       <float64>
-
-
-We can calculate the ``posterior`` by multiplying ``likelihood`` by ``prior``. Whenever performing binary operations on ``Frame`` and ``Series``, indices will be aligned and, if necessary, reindexed before processing.
-
->>> posterior = likelihood * prior
->>> round(posterior.head(), 2)
-<Frame>
-<Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
-<Index>
-1       -0.19       -0.75           -1.35
-14      -1.38       -2.27           -1.72
-20      -0.16       -0.77           -0.95
-21      -0.02       -1.72           -1.75
-37      -0.07       -0.83           -1.37
-<int64> <float64>   <float64>       <float64>
-
-
-We can now add columns to our ``data_test`` ``FrameGO``. To determine our best prediction of species for each row of the test data, the column label (the species) of the maximum a posteriori estimate is selected with ``loc_max()``.
-
->>> data_test['predict'] = posterior.loc_max(axis=1)
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict     <<U7>
-<Index>
-1         4.9       3.0       Iris-setosa
-14        5.8       4.0       Iris-setosa
-20        5.4       3.4       Iris-setosa
-21        5.1       3.7       Iris-setosa
-37        4.9       3.1       Iris-setosa
-<int64>   <float64> <float64> <<U15>
-
-
-We can add two additional columns to evaluate the effectivess of the classifier. First, we can add an "observed" column by adding the original "species" column from the original ``data`` ``Frame``. In assigning a ``Series`` to a ``Frame``, only values found in the intersection of the indices will be added as a column.
-
->>> data_test['observed'] = data['species']
->>> data_test.head()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict     observed    <<U8>
-<Index>
-1         4.9       3.0       Iris-setosa Iris-setosa
-14        5.8       4.0       Iris-setosa Iris-setosa
-20        5.4       3.4       Iris-setosa Iris-setosa
-21        5.1       3.7       Iris-setosa Iris-setosa
-37        4.9       3.1       Iris-setosa Iris-setosa
-<int64>   <float64> <float64> <<U15>      <<U15>
-
-
-Having populated a column of predicted and observed values, we can compare the two to get a Boolean column indicating when the classifier calculated a correct predicton.
-
->>> data_test['correct'] = data_test['predict'] == data_test['observed']
->>> data_test.tail()
-<FrameGO>
-<IndexGO> sepal_l   sepal_w   predict         observed       correct <<U8>
-<Index>
-129       7.2       3.0       Iris-virginica  Iris-virginica True
-130       7.4       2.8       Iris-virginica  Iris-virginica True
-140       6.7       3.1       Iris-virginica  Iris-virginica True
-144       6.7       3.3       Iris-virginica  Iris-virginica True
-149       5.9       3.0       Iris-versicolor Iris-virginica False
-<int64>   <float64> <float64> <<U15>          <<U15>         <bool>
+    >>> likelihood = sf.Frame.from_fields(likelihood_of_species, columns=mu.index, index=data_test.index)
+    >>> round(likelihood.head(), 2)
+    <Frame>
+    <Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
+    <Index>
+    1       -0.52       -2.31           -4.27
+    14      -3.86       -6.97           -5.42
+    20      -0.45       -2.38           -3.01
+    21      -0.05       -5.29           -5.51
+    37      -0.2        -2.56           -4.33
+    <int64> <float64>   <float64>       <float64>
+
+
+We can calculate the ``posterior`` by multiplying ``likelihood`` by ``prior``. Whenever performing binary operations on ``Frame`` and ``Series``, indices will be aligned and, if necessary, reindexed before processing::
+
+    >>> posterior = likelihood * prior
+    >>> round(posterior.head(), 2)
+    <Frame>
+    <Index> Iris-setosa Iris-versicolor Iris-virginica <<U15>
+    <Index>
+    1       -0.19       -0.75           -1.35
+    14      -1.38       -2.27           -1.72
+    20      -0.16       -0.77           -0.95
+    21      -0.02       -1.72           -1.75
+    37      -0.07       -0.83           -1.37
+    <int64> <float64>   <float64>       <float64>
+
+
+We can now add columns to our ``data_test`` ``FrameGO``. To determine our best prediction of species for each row of the test data, the column label (the species) of the maximum a posteriori estimate is selected with ``loc_max()``::
+
+    >>> data_test['predict'] = posterior.loc_max(axis=1)
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict     <<U7>
+    <Index>
+    1         4.9       3.0       Iris-setosa
+    14        5.8       4.0       Iris-setosa
+    20        5.4       3.4       Iris-setosa
+    21        5.1       3.7       Iris-setosa
+    37        4.9       3.1       Iris-setosa
+    <int64>   <float64> <float64> <<U15>
+
+
+We can add two additional columns to evaluate the effectivess of the classifier. First, we can add an "observed" column by adding the original "species" column from the original ``data`` ``Frame``. In assigning a ``Series`` to a ``Frame``, only values found in the intersection of the indices will be added as a column::
+
+    >>> data_test['observed'] = data['species']
+    >>> data_test.head()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict     observed    <<U8>
+    <Index>
+    1         4.9       3.0       Iris-setosa Iris-setosa
+    14        5.8       4.0       Iris-setosa Iris-setosa
+    20        5.4       3.4       Iris-setosa Iris-setosa
+    21        5.1       3.7       Iris-setosa Iris-setosa
+    37        4.9       3.1       Iris-setosa Iris-setosa
+    <int64>   <float64> <float64> <<U15>      <<U15>
+
+
+Having populated a column of predicted and observed values, we can compare the two to get a Boolean column indicating when the classifier calculated a correct predicton::
+
+    >>> data_test['correct'] = data_test['predict'] == data_test['observed']
+    >>> data_test.tail()
+    <FrameGO>
+    <IndexGO> sepal_l   sepal_w   predict         observed       correct <<U8>
+    <Index>
+    129       7.2       3.0       Iris-virginica  Iris-virginica True
+    130       7.4       2.8       Iris-virginica  Iris-virginica True
+    140       6.7       3.1       Iris-virginica  Iris-virginica True
+    144       6.7       3.3       Iris-virginica  Iris-virginica True
+    149       5.9       3.0       Iris-versicolor Iris-virginica False
+    <int64>   <float64> <float64> <<U15>          <<U15>         <bool>
 
 
-To find the percentage of correct classifications among the test data, we can sum the ``correct`` Boolean column and divide that by the size of the test data.
+To find the percentage of correct classifications among the test data, we can sum the ``correct`` Boolean column and divide that by the size of the test data::
 
->>> data_test["correct"].sum() / len(data_test)
-0.7333333333333333
+    >>> data_test["correct"].sum() / len(data_test)
+    0.7333333333333333
 
 This simple naive Bayes classifier can predict iris species correctly about 73% of the time.
 
 For further introduction to StaticFrame, including links to articles, videos, and documentation, see `here <https://static-frame.readthedocs.io/en/latest/intro.html>`__.
```

### Comparing `static-frame-2.5.2/static_frame.egg-info/SOURCES.txt` & `static-frame-2.6.0/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

