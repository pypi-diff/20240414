# Comparing `tmp/bencode2-0.0.8.tar.gz` & `tmp/bencode2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode2-0.0.8.tar", last modified: Sun Apr 14 14:19:45 2024, max compression
+gzip compressed data, was "bencode2-0.0.9.tar", last modified: Sun Apr 14 14:26:11 2024, max compression
```

## Comparing `bencode2-0.0.8.tar` & `bencode2-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:19:45.766984 bencode2-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-14 14:19:38.000000 bencode2-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-14 14:19:38.000000 bencode2-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-14 14:19:45.766984 bencode2-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:19:45.766984 bencode2-0.0.8/bencode2/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 14:19:38.000000 bencode2-0.0.8/bencode2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   470733 2024-04-14 14:19:45.000000 bencode2-0.0.8/bencode2/_decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-14 14:19:38.000000 bencode2-0.0.8/bencode2/_decoder.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   375778 2024-04-14 14:19:45.000000 bencode2-0.0.8/bencode2/_encoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-14 14:19:38.000000 bencode2-0.0.8/bencode2/_encoder.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   190928 2024-04-14 14:19:45.000000 bencode2-0.0.8/bencode2/_exceptions.c
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-14 14:19:38.000000 bencode2-0.0.8/bencode2/_exceptions.pyx
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 14:19:38.000000 bencode2-0.0.8/bencode2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:19:45.766984 bencode2-0.0.8/bencode2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-14 14:19:45.000000 bencode2-0.0.8/bencode2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-14 14:19:45.000000 bencode2-0.0.8/bencode2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:19:45.000000 bencode2-0.0.8/bencode2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 14:19:45.000000 bencode2-0.0.8/bencode2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-14 14:19:38.000000 bencode2-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:19:45.766984 bencode2-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-14 14:19:38.000000 bencode2-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:19:45.766984 bencode2-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-14 14:19:38.000000 bencode2-0.0.8/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-14 14:19:38.000000 bencode2-0.0.8/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-14 14:19:38.000000 bencode2-0.0.8/tests/test_torrent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:11.301989 bencode2-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-14 14:26:06.000000 bencode2-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-14 14:26:06.000000 bencode2-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-14 14:26:11.301989 bencode2-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:11.297989 bencode2-0.0.9/bencode2/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   487607 2024-04-14 14:26:10.000000 bencode2-0.0.9/bencode2/_decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/_decoder.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   375778 2024-04-14 14:26:10.000000 bencode2-0.0.9/bencode2/_encoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/_encoder.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   190928 2024-04-14 14:26:10.000000 bencode2-0.0.9/bencode2/_exceptions.c
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/_exceptions.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:11.301989 bencode2-0.0.9/bencode2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-14 14:26:11.000000 bencode2-0.0.9/bencode2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-14 14:26:11.000000 bencode2-0.0.9/bencode2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:26:11.000000 bencode2-0.0.9/bencode2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 14:26:11.000000 bencode2-0.0.9/bencode2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-14 14:26:06.000000 bencode2-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:26:11.301989 bencode2-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-14 14:26:06.000000 bencode2-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:11.301989 bencode2-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-14 14:26:06.000000 bencode2-0.0.9/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-14 14:26:06.000000 bencode2-0.0.9/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-14 14:26:06.000000 bencode2-0.0.9/tests/test_torrent.py
```

### Comparing `bencode2-0.0.8/LICENSE` & `bencode2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bencode2-0.0.8/PKG-INFO` & `bencode2-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode2
-Version: 0.0.8
+Version: 0.0.9
 Summary: bencode serialize/deserialize library
 Home-page: https://github.com/trim21/py-bencode
 Author: trim21
 Author-email: trim21.me@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bencode2-0.0.8/bencode2/__init__.py` & `bencode2-0.0.9/bencode2/__init__.py`

 * *Files identical despite different names*

### Comparing `bencode2-0.0.8/bencode2/_decoder.c` & `bencode2-0.0.9/bencode2/_decoder.c`

 * *Files 6% similar despite different names*

```diff
@@ -2333,15 +2333,15 @@
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_bytes[] = "bytes";
-static const char __pyx_k_index[] = "index";
+static const char __pyx_k_index[] = ". index ";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_errors[] = "errors";
@@ -2351,14 +2351,16 @@
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_return[] = "return";
 static const char __pyx_k_strict[] = "strict";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_Decoder[] = "Decoder";
 static const char __pyx_k_disable[] = "disable";
+static const char __pyx_k_index_2[] = ", index ";
+static const char __pyx_k_index_3[] = "index";
 static const char __pyx_k_str_key[] = "str_key";
 static const char __pyx_k_KeyError[] = "KeyError";
 static const char __pyx_k_at_index[] = " at index ";
 static const char __pyx_k_encoding[] = "encoding";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
@@ -2373,28 +2375,30 @@
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_use_setstate[] = "use_setstate";
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
+static const char __pyx_k_malformed_int[] = "malformed int ";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_Decoder_decode[] = "Decoder.decode";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_unexpected_token[] = "unexpected token ";
 static const char __pyx_k_bencode2__decoder[] = "bencode2._decoder";
 static const char __pyx_k_BencodeDecodeError[] = "BencodeDecodeError";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_pyx_unpickle_Decoder[] = "__pyx_unpickle_Decoder";
 static const char __pyx_k_bencode2__decoder_pyx[] = "bencode2/_decoder.pyx";
 static const char __pyx_k_Decoder___reduce_cython[] = "Decoder.__reduce_cython__";
 static const char __pyx_k_Decoder___setstate_cython[] = "Decoder.__setstate_cython__";
 static const char __pyx_k_not_a_valid_bencode_bytes[] = "not a valid bencode bytes: ";
+static const char __pyx_k_malformed_str_bytes_length[] = "malformed str/bytes length ";
 static const char __pyx_k_0_is_not_allowed_in_bencoding_i[] = "-0 is not allowed in bencoding. index: ";
 static const char __pyx_k_malformed_str_bytes_length_with[] = "malformed str/bytes length with leading 0. index ";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))";
 static const char __pyx_k_integer_with_leading_zero_is_not[] = "integer with leading zero is not allowed. index: ";
 static const char __pyx_k_invalid_bencode_value_data_after[] = "invalid bencode value (data after valid prefix)";
 /* #### Code section: decls ### */
 static int __pyx_pf_8bencode2_8_decoder_7Decoder___init__(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_str_key); /* proto */
@@ -2468,21 +2472,25 @@
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_encoding;
   PyObject *__pyx_n_s_errors;
   PyObject *__pyx_n_s_exceptions;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_import;
-  PyObject *__pyx_n_s_index;
+  PyObject *__pyx_kp_u_index;
+  PyObject *__pyx_kp_u_index_2;
+  PyObject *__pyx_n_s_index_3;
   PyObject *__pyx_kp_u_integer_with_leading_zero_is_not;
   PyObject *__pyx_kp_u_invalid_bencode_value_data_after;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_length;
   PyObject *__pyx_n_s_main;
+  PyObject *__pyx_kp_u_malformed_int;
+  PyObject *__pyx_kp_u_malformed_str_bytes_length;
   PyObject *__pyx_kp_u_malformed_str_bytes_length_with;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_kp_u_not_a_valid_bencode_bytes;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
@@ -2507,14 +2515,15 @@
   PyObject *__pyx_kp_u_unexpected_token;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_value;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
+  PyObject *__pyx_int_10;
   PyObject *__pyx_int_27736365;
   PyObject *__pyx_int_148187747;
   PyObject *__pyx_int_211139970;
   PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__8;
@@ -2600,21 +2609,25 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_encoding);
   Py_CLEAR(clear_module_state->__pyx_n_s_errors);
   Py_CLEAR(clear_module_state->__pyx_n_s_exceptions);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
-  Py_CLEAR(clear_module_state->__pyx_n_s_index);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_index);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_index_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_index_3);
   Py_CLEAR(clear_module_state->__pyx_kp_u_integer_with_leading_zero_is_not);
   Py_CLEAR(clear_module_state->__pyx_kp_u_invalid_bencode_value_data_after);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_malformed_int);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_malformed_str_bytes_length);
   Py_CLEAR(clear_module_state->__pyx_kp_u_malformed_str_bytes_length_with);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_kp_u_not_a_valid_bencode_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
@@ -2639,14 +2652,15 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_unexpected_token);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_value);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
+  Py_CLEAR(clear_module_state->__pyx_int_10);
   Py_CLEAR(clear_module_state->__pyx_int_27736365);
   Py_CLEAR(clear_module_state->__pyx_int_148187747);
   Py_CLEAR(clear_module_state->__pyx_int_211139970);
   Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
@@ -2710,21 +2724,25 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_encoding);
   Py_VISIT(traverse_module_state->__pyx_n_s_errors);
   Py_VISIT(traverse_module_state->__pyx_n_s_exceptions);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
-  Py_VISIT(traverse_module_state->__pyx_n_s_index);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_index);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_index_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_index_3);
   Py_VISIT(traverse_module_state->__pyx_kp_u_integer_with_leading_zero_is_not);
   Py_VISIT(traverse_module_state->__pyx_kp_u_invalid_bencode_value_data_after);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_malformed_int);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_malformed_str_bytes_length);
   Py_VISIT(traverse_module_state->__pyx_kp_u_malformed_str_bytes_length_with);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_kp_u_not_a_valid_bencode_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
@@ -2749,14 +2767,15 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_unexpected_token);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_value);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
+  Py_VISIT(traverse_module_state->__pyx_int_10);
   Py_VISIT(traverse_module_state->__pyx_int_27736365);
   Py_VISIT(traverse_module_state->__pyx_int_148187747);
   Py_VISIT(traverse_module_state->__pyx_int_211139970);
   Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
@@ -2830,21 +2849,25 @@
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_encoding __pyx_mstate_global->__pyx_n_s_encoding
 #define __pyx_n_s_errors __pyx_mstate_global->__pyx_n_s_errors
 #define __pyx_n_s_exceptions __pyx_mstate_global->__pyx_n_s_exceptions
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
-#define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
+#define __pyx_kp_u_index __pyx_mstate_global->__pyx_kp_u_index
+#define __pyx_kp_u_index_2 __pyx_mstate_global->__pyx_kp_u_index_2
+#define __pyx_n_s_index_3 __pyx_mstate_global->__pyx_n_s_index_3
 #define __pyx_kp_u_integer_with_leading_zero_is_not __pyx_mstate_global->__pyx_kp_u_integer_with_leading_zero_is_not
 #define __pyx_kp_u_invalid_bencode_value_data_after __pyx_mstate_global->__pyx_kp_u_invalid_bencode_value_data_after
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_length __pyx_mstate_global->__pyx_n_s_length
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_kp_u_malformed_int __pyx_mstate_global->__pyx_kp_u_malformed_int
+#define __pyx_kp_u_malformed_str_bytes_length __pyx_mstate_global->__pyx_kp_u_malformed_str_bytes_length
 #define __pyx_kp_u_malformed_str_bytes_length_with __pyx_mstate_global->__pyx_kp_u_malformed_str_bytes_length_with
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_kp_u_not_a_valid_bencode_bytes __pyx_mstate_global->__pyx_kp_u_not_a_valid_bencode_bytes
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
@@ -2869,14 +2892,15 @@
 #define __pyx_kp_u_unexpected_token __pyx_mstate_global->__pyx_kp_u_unexpected_token
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
+#define __pyx_int_10 __pyx_mstate_global->__pyx_int_10
 #define __pyx_int_27736365 __pyx_mstate_global->__pyx_int_27736365
 #define __pyx_int_148187747 __pyx_mstate_global->__pyx_int_148187747
 #define __pyx_int_211139970 __pyx_mstate_global->__pyx_int_211139970
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
@@ -3772,335 +3796,518 @@
 static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_int(CYTHON_UNUSED struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
   PyObject *__pyx_v_new_f = NULL;
   PyObject *__pyx_v_n = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  Py_ssize_t __pyx_t_3;
-  int __pyx_t_4;
-  Py_ssize_t __pyx_t_5;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  PyObject *__pyx_t_9 = NULL;
-  int __pyx_t_10;
+  int __pyx_t_7;
+  Py_ssize_t __pyx_t_8;
+  Py_ssize_t __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
   int __pyx_t_11;
+  PyObject *__pyx_t_12 = NULL;
+  PyObject *__pyx_t_13 = NULL;
+  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_15 = NULL;
+  Py_UCS4 __pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
+  Py_ssize_t __pyx_t_18;
+  PyObject *__pyx_t_19 = NULL;
+  int __pyx_t_20;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_Decoder__decode_int", 0);
   __Pyx_INCREF(__pyx_v_index);
 
   /* "bencode2/_decoder.pyx":38
  * 
  *     cdef tuple[object, int] __decode_int(self, x: bytes, index: int):
  *         index += 1             # <<<<<<<<<<<<<<
  *         new_f = x.index(b"e", index)
- *         n = int(x[index:new_f])
+ *         try:
  */
   __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
   /* "bencode2/_decoder.pyx":39
  *     cdef tuple[object, int] __decode_int(self, x: bytes, index: int):
  *         index += 1
  *         new_f = x.index(b"e", index)             # <<<<<<<<<<<<<<
- *         n = int(x[index:new_f])
- * 
+ *         try:
+ *             n = int(x[index:new_f], 10)
  */
   __pyx_t_1 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_index, __pyx_v_x, __pyx_n_b_e, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_new_f = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "bencode2/_decoder.pyx":40
  *         index += 1
  *         new_f = x.index(b"e", index)
- *         n = int(x[index:new_f])             # <<<<<<<<<<<<<<
+ *         try:             # <<<<<<<<<<<<<<
+ *             n = int(x[index:new_f], 10)
+ *         except ValueError:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_4);
+    /*try:*/ {
+
+      /* "bencode2/_decoder.pyx":41
+ *         new_f = x.index(b"e", index)
+ *         try:
+ *             n = int(x[index:new_f], 10)             # <<<<<<<<<<<<<<
+ *         except ValueError:
+ *             raise BencodeDecodeError(
+ */
+      __Pyx_INCREF(__pyx_v_index);
+      __pyx_t_5 = __pyx_v_index;
+      __pyx_t_7 = (__pyx_t_5 == ((PyObject*)Py_None));
+      if (__pyx_t_7) {
+        __pyx_t_6 = 0;
+      } else {
+        __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
+        __pyx_t_6 = __pyx_t_8;
+      }
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_INCREF(__pyx_v_new_f);
+      __pyx_t_1 = __pyx_v_new_f;
+      __pyx_t_7 = (__pyx_t_1 == Py_None);
+      if (__pyx_t_7) {
+        __pyx_t_8 = PY_SSIZE_T_MAX;
+      } else {
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L3_error)
+        __pyx_t_8 = __pyx_t_9;
+      }
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = PySequence_GetSlice(__pyx_v_x, __pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 41, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_GIVEREF(__pyx_t_1);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_1)) __PYX_ERR(0, 41, __pyx_L3_error);
+      __Pyx_INCREF(__pyx_int_10);
+      __Pyx_GIVEREF(__pyx_int_10);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_int_10)) __PYX_ERR(0, 41, __pyx_L3_error);
+      __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyInt_Type)), __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_v_n = __pyx_t_1;
+      __pyx_t_1 = 0;
+
+      /* "bencode2/_decoder.pyx":40
+ *         index += 1
+ *         new_f = x.index(b"e", index)
+ *         try:             # <<<<<<<<<<<<<<
+ *             n = int(x[index:new_f], 10)
+ *         except ValueError:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    /* "bencode2/_decoder.pyx":42
+ *         try:
+ *             n = int(x[index:new_f], 10)
+ *         except ValueError:             # <<<<<<<<<<<<<<
+ *             raise BencodeDecodeError(
+ *                 f'malformed int {x[index:new_f]}. index {index}'
+ */
+    __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
+    if (__pyx_t_11) {
+      __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_10, &__pyx_t_12) < 0) __PYX_ERR(0, 42, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_10);
+      __Pyx_XGOTREF(__pyx_t_12);
+
+      /* "bencode2/_decoder.pyx":43
+ *             n = int(x[index:new_f], 10)
+ *         except ValueError:
+ *             raise BencodeDecodeError(             # <<<<<<<<<<<<<<
+ *                 f'malformed int {x[index:new_f]}. index {index}'
+ *             )
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 43, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_14);
+
+      /* "bencode2/_decoder.pyx":44
+ *         except ValueError:
+ *             raise BencodeDecodeError(
+ *                 f'malformed int {x[index:new_f]}. index {index}'             # <<<<<<<<<<<<<<
+ *             )
  * 
- *         if x[index] == c'-':
  */
-  __Pyx_INCREF(__pyx_v_index);
-  __pyx_t_2 = __pyx_v_index;
-  __pyx_t_4 = (__pyx_t_2 == ((PyObject*)Py_None));
-  if (__pyx_t_4) {
-    __pyx_t_3 = 0;
-  } else {
-    __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L1_error)
-    __pyx_t_3 = __pyx_t_5;
-  }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_INCREF(__pyx_v_new_f);
-  __pyx_t_1 = __pyx_v_new_f;
-  __pyx_t_4 = (__pyx_t_1 == Py_None);
-  if (__pyx_t_4) {
-    __pyx_t_5 = PY_SSIZE_T_MAX;
-  } else {
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L1_error)
-    __pyx_t_5 = __pyx_t_6;
+      __pyx_t_15 = PyTuple_New(4); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 44, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_15);
+      __pyx_t_8 = 0;
+      __pyx_t_16 = 127;
+      __Pyx_INCREF(__pyx_kp_u_malformed_int);
+      __pyx_t_8 += 14;
+      __Pyx_GIVEREF(__pyx_kp_u_malformed_int);
+      PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_kp_u_malformed_int);
+      __Pyx_INCREF(__pyx_v_index);
+      __pyx_t_5 = __pyx_v_index;
+      __pyx_t_7 = (__pyx_t_5 == ((PyObject*)Py_None));
+      if (__pyx_t_7) {
+        __pyx_t_6 = 0;
+      } else {
+        __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L5_except_error)
+        __pyx_t_6 = __pyx_t_9;
+      }
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_INCREF(__pyx_v_new_f);
+      __pyx_t_17 = __pyx_v_new_f;
+      __pyx_t_7 = (__pyx_t_17 == Py_None);
+      if (__pyx_t_7) {
+        __pyx_t_9 = PY_SSIZE_T_MAX;
+      } else {
+        __pyx_t_18 = __Pyx_PyIndex_AsSsize_t(__pyx_t_17); if (unlikely((__pyx_t_18 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L5_except_error)
+        __pyx_t_9 = __pyx_t_18;
+      }
+      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+      __pyx_t_17 = PySequence_GetSlice(__pyx_v_x, __pyx_t_6, __pyx_t_9); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 44, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_17);
+      __pyx_t_19 = __Pyx_PyObject_FormatSimple(__pyx_t_17, __pyx_empty_unicode); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 44, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+      __pyx_t_16 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) > __pyx_t_16) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) : __pyx_t_16;
+      __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_19);
+      __Pyx_GIVEREF(__pyx_t_19);
+      PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_19);
+      __pyx_t_19 = 0;
+      __Pyx_INCREF(__pyx_kp_u_index);
+      __pyx_t_8 += 8;
+      __Pyx_GIVEREF(__pyx_kp_u_index);
+      PyTuple_SET_ITEM(__pyx_t_15, 2, __pyx_kp_u_index);
+      __pyx_t_19 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 44, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __pyx_t_16 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) > __pyx_t_16) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) : __pyx_t_16;
+      __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_19);
+      __Pyx_GIVEREF(__pyx_t_19);
+      PyTuple_SET_ITEM(__pyx_t_15, 3, __pyx_t_19);
+      __pyx_t_19 = 0;
+      __pyx_t_19 = __Pyx_PyUnicode_Join(__pyx_t_15, 4, __pyx_t_8, __pyx_t_16); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 44, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+      __pyx_t_15 = NULL;
+      __pyx_t_11 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_14))) {
+        __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
+        if (likely(__pyx_t_15)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
+          __Pyx_INCREF(__pyx_t_15);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_14, function);
+          __pyx_t_11 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_15, __pyx_t_19};
+        __pyx_t_13 = __Pyx_PyObject_FastCall(__pyx_t_14, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+        if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 43, __pyx_L5_except_error)
+        __Pyx_GOTREF(__pyx_t_13);
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+      }
+      __Pyx_Raise(__pyx_t_13, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+      __PYX_ERR(0, 43, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "bencode2/_decoder.pyx":40
+ *         index += 1
+ *         new_f = x.index(b"e", index)
+ *         try:             # <<<<<<<<<<<<<<
+ *             n = int(x[index:new_f], 10)
+ *         except ValueError:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_XGIVEREF(__pyx_t_4);
+    __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
   }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PySequence_GetSlice(__pyx_v_x, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 40, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_n = __pyx_t_7;
-  __pyx_t_7 = 0;
 
-  /* "bencode2/_decoder.pyx":42
- *         n = int(x[index:new_f])
+  /* "bencode2/_decoder.pyx":47
+ *             )
  * 
  *         if x[index] == c'-':             # <<<<<<<<<<<<<<
  *             if x[index + 1] == c"0":
  *                 raise BencodeDecodeError(
  */
-  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_1 = __Pyx_PyInt_From_char('-'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_12 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_10 = __Pyx_PyInt_From_char('-'); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_12, __pyx_t_10, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 47, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 42, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (__pyx_t_4) {
+  if (__pyx_t_7) {
 
-    /* "bencode2/_decoder.pyx":43
+    /* "bencode2/_decoder.pyx":48
  * 
  *         if x[index] == c'-':
  *             if x[index + 1] == c"0":             # <<<<<<<<<<<<<<
  *                 raise BencodeDecodeError(
  *                     f'-0 is not allowed in bencoding. index: {index}'
  */
-    __pyx_t_8 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 43, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __pyx_t_1 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 43, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_1, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __pyx_t_12 = PyObject_RichCompare(__pyx_t_10, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_12); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 43, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(__pyx_t_4)) {
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_12); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 48, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    if (unlikely(__pyx_t_7)) {
 
-      /* "bencode2/_decoder.pyx":44
+      /* "bencode2/_decoder.pyx":49
  *         if x[index] == c'-':
  *             if x[index + 1] == c"0":
  *                 raise BencodeDecodeError(             # <<<<<<<<<<<<<<
  *                     f'-0 is not allowed in bencoding. index: {index}'
  *                 )
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 44, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
 
-      /* "bencode2/_decoder.pyx":45
+      /* "bencode2/_decoder.pyx":50
  *             if x[index + 1] == c"0":
  *                 raise BencodeDecodeError(
  *                     f'-0 is not allowed in bencoding. index: {index}'             # <<<<<<<<<<<<<<
  *                 )
  *         elif x[index] == c'0' and new_f != index + 1:
  */
-      __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_9 = __Pyx_PyUnicode_Concat(__pyx_kp_u_0_is_not_allowed_in_bencoding_i, __pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 45, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_9);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = NULL;
-      __pyx_t_10 = 0;
+      __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 50, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_10);
+      __pyx_t_13 = __Pyx_PyUnicode_Concat(__pyx_kp_u_0_is_not_allowed_in_bencoding_i, __pyx_t_10); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 50, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __pyx_t_10 = NULL;
+      __pyx_t_11 = 0;
       #if CYTHON_UNPACK_METHODS
-      if (unlikely(PyMethod_Check(__pyx_t_8))) {
-        __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_8);
-        if (likely(__pyx_t_1)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-          __Pyx_INCREF(__pyx_t_1);
+      if (unlikely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_10)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_10);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_8, function);
-          __pyx_t_10 = 1;
+          __Pyx_DECREF_SET(__pyx_t_1, function);
+          __pyx_t_11 = 1;
         }
       }
       #endif
       {
-        PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_9};
-        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
-        __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      }
-      __Pyx_Raise(__pyx_t_7, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __PYX_ERR(0, 44, __pyx_L1_error)
+        PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_13};
+        __pyx_t_12 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 49, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      }
+      __Pyx_Raise(__pyx_t_12, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __PYX_ERR(0, 49, __pyx_L1_error)
 
-      /* "bencode2/_decoder.pyx":43
+      /* "bencode2/_decoder.pyx":48
  * 
  *         if x[index] == c'-':
  *             if x[index + 1] == c"0":             # <<<<<<<<<<<<<<
  *                 raise BencodeDecodeError(
  *                     f'-0 is not allowed in bencoding. index: {index}'
  */
     }
 
-    /* "bencode2/_decoder.pyx":42
- *         n = int(x[index:new_f])
+    /* "bencode2/_decoder.pyx":47
+ *             )
  * 
  *         if x[index] == c'-':             # <<<<<<<<<<<<<<
  *             if x[index + 1] == c"0":
  *                 raise BencodeDecodeError(
  */
-    goto __pyx_L3;
+    goto __pyx_L11;
   }
 
-  /* "bencode2/_decoder.pyx":47
+  /* "bencode2/_decoder.pyx":52
  *                     f'-0 is not allowed in bencoding. index: {index}'
  *                 )
  *         elif x[index] == c'0' and new_f != index + 1:             # <<<<<<<<<<<<<<
  *             raise BencodeDecodeError(
  *                 f'integer with leading zero is not allowed. index: {index}'
  */
-  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = PyObject_RichCompare(__pyx_t_7, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_9); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  if (__pyx_t_11) {
+  __pyx_t_12 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_12);
+  __pyx_t_1 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_13 = PyObject_RichCompare(__pyx_t_12, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_20 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely((__pyx_t_20 < 0))) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  if (__pyx_t_20) {
   } else {
-    __pyx_t_4 = __pyx_t_11;
-    goto __pyx_L5_bool_binop_done;
+    __pyx_t_7 = __pyx_t_20;
+    goto __pyx_L13_bool_binop_done;
   }
-  __pyx_t_9 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_8 = PyObject_RichCompare(__pyx_v_new_f, __pyx_t_9, Py_NE); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-  __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_4 = __pyx_t_11;
-  __pyx_L5_bool_binop_done:;
-  if (unlikely(__pyx_t_4)) {
+  __pyx_t_13 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_new_f, __pyx_t_13, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+  __pyx_t_20 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_20 < 0))) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_7 = __pyx_t_20;
+  __pyx_L13_bool_binop_done:;
+  if (unlikely(__pyx_t_7)) {
 
-    /* "bencode2/_decoder.pyx":48
+    /* "bencode2/_decoder.pyx":53
  *                 )
  *         elif x[index] == c'0' and new_f != index + 1:
  *             raise BencodeDecodeError(             # <<<<<<<<<<<<<<
  *                 f'integer with leading zero is not allowed. index: {index}'
  *             )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 48, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_13);
 
-    /* "bencode2/_decoder.pyx":49
+    /* "bencode2/_decoder.pyx":54
  *         elif x[index] == c'0' and new_f != index + 1:
  *             raise BencodeDecodeError(
  *                 f'integer with leading zero is not allowed. index: {index}'             # <<<<<<<<<<<<<<
  *             )
  *         return n, new_f + 1
  */
-    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 49, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_kp_u_integer_with_leading_zero_is_not, __pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = NULL;
-    __pyx_t_10 = 0;
+    __pyx_t_12 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_integer_with_leading_zero_is_not, __pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_12 = NULL;
+    __pyx_t_11 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_9))) {
-      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_9);
-      if (likely(__pyx_t_7)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
-        __Pyx_INCREF(__pyx_t_7);
+    if (unlikely(PyMethod_Check(__pyx_t_13))) {
+      __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
+      if (likely(__pyx_t_12)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_13);
+        __Pyx_INCREF(__pyx_t_12);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_9, function);
-        __pyx_t_10 = 1;
+        __Pyx_DECREF_SET(__pyx_t_13, function);
+        __pyx_t_11 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_1};
-      __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
-      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 48, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    }
-    __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __PYX_ERR(0, 48, __pyx_L1_error)
+      PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_10};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
+      __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    }
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 53, __pyx_L1_error)
 
-    /* "bencode2/_decoder.pyx":47
+    /* "bencode2/_decoder.pyx":52
  *                     f'-0 is not allowed in bencoding. index: {index}'
  *                 )
  *         elif x[index] == c'0' and new_f != index + 1:             # <<<<<<<<<<<<<<
  *             raise BencodeDecodeError(
  *                 f'integer with leading zero is not allowed. index: {index}'
  */
   }
-  __pyx_L3:;
+  __pyx_L11:;
 
-  /* "bencode2/_decoder.pyx":51
+  /* "bencode2/_decoder.pyx":56
  *                 f'integer with leading zero is not allowed. index: {index}'
  *             )
  *         return n, new_f + 1             # <<<<<<<<<<<<<<
  * 
  *     cdef tuple[list, int] __decode_list(self, x: bytes, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = __Pyx_PyInt_AddObjC(__pyx_v_new_f, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = PyTuple_New(2); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_new_f, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_13 = PyTuple_New(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_v_n);
   __Pyx_GIVEREF(__pyx_v_n);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_v_n)) __PYX_ERR(0, 51, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_8);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_8)) __PYX_ERR(0, 51, __pyx_L1_error);
-  __pyx_t_8 = 0;
-  __pyx_r = ((PyObject*)__pyx_t_9);
-  __pyx_t_9 = 0;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_v_n)) __PYX_ERR(0, 56, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error);
+  __pyx_t_1 = 0;
+  __pyx_r = ((PyObject*)__pyx_t_13);
+  __pyx_t_13 = 0;
   goto __pyx_L0;
 
   /* "bencode2/_decoder.pyx":37
  *             f"unexpected token {x[index:index + 1]} at index {index}")
  * 
  *     cdef tuple[object, int] __decode_int(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         index += 1
  *         new_f = x.index(b"e", index)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_XDECREF(__pyx_t_14);
+  __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_17);
+  __Pyx_XDECREF(__pyx_t_19);
   __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_new_f);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_decoder.pyx":53
+/* "bencode2/_decoder.pyx":58
  *         return n, new_f + 1
  * 
  *     cdef tuple[list, int] __decode_list(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         r, index = [], index + 1
  * 
  */
 
@@ -4116,121 +4323,121 @@
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_Decoder__decode_list", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "bencode2/_decoder.pyx":54
+  /* "bencode2/_decoder.pyx":59
  * 
  *     cdef tuple[list, int] __decode_list(self, x: bytes, index: int):
  *         r, index = [], index + 1             # <<<<<<<<<<<<<<
  * 
  *         while x[index] != c'e':
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 59, __pyx_L1_error)
   __pyx_v_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_2));
   __pyx_t_2 = 0;
 
-  /* "bencode2/_decoder.pyx":56
+  /* "bencode2/_decoder.pyx":61
  *         r, index = [], index + 1
  * 
  *         while x[index] != c'e':             # <<<<<<<<<<<<<<
  *             v, index = self.__decode(x, index)
  *             r.append(v)
  */
   while (1) {
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyInt_From_char('e'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_char('e'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (!__pyx_t_4) break;
 
-    /* "bencode2/_decoder.pyx":57
+    /* "bencode2/_decoder.pyx":62
  * 
  *         while x[index] != c'e':
  *             v, index = self.__decode(x, index)             # <<<<<<<<<<<<<<
  *             r.append(v)
  * 
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (likely(__pyx_t_3 != Py_None)) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 57, __pyx_L1_error)
+        __PYX_ERR(0, 62, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_2);
       #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 57, __pyx_L1_error)
+      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 62, __pyx_L1_error)
     }
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 57, __pyx_L1_error)
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "bencode2/_decoder.pyx":58
+    /* "bencode2/_decoder.pyx":63
  *         while x[index] != c'e':
  *             v, index = self.__decode(x, index)
  *             r.append(v)             # <<<<<<<<<<<<<<
  * 
  *         return r, index + 1
  */
-    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_r, __pyx_v_v); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 58, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_r, __pyx_v_v); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 63, __pyx_L1_error)
   }
 
-  /* "bencode2/_decoder.pyx":60
+  /* "bencode2/_decoder.pyx":65
  *             r.append(v)
  * 
  *         return r, index + 1             # <<<<<<<<<<<<<<
  * 
  *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_r);
   __Pyx_GIVEREF(__pyx_v_r);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_r)) __PYX_ERR(0, 60, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_r)) __PYX_ERR(0, 65, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_r = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/_decoder.pyx":53
+  /* "bencode2/_decoder.pyx":58
  *         return n, new_f + 1
  * 
  *     cdef tuple[list, int] __decode_list(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         r, index = [], index + 1
  * 
  */
 
@@ -4246,15 +4453,15 @@
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_decoder.pyx":62
+/* "bencode2/_decoder.pyx":67
  *         return r, index + 1
  * 
  *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         if x[index] == c'0':
  *             raise BencodeDecodeError(
  */
 
@@ -4267,60 +4474,69 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
-  Py_ssize_t __pyx_t_8;
-  Py_ssize_t __pyx_t_9;
-  Py_ssize_t __pyx_t_10;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  Py_ssize_t __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  Py_ssize_t __pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_15 = NULL;
+  Py_UCS4 __pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
+  Py_ssize_t __pyx_t_18;
+  PyObject *__pyx_t_19 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_Decoder__decode_str", 1);
 
-  /* "bencode2/_decoder.pyx":63
+  /* "bencode2/_decoder.pyx":68
  * 
  *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
  *         if x[index] == c'0':             # <<<<<<<<<<<<<<
  *             raise BencodeDecodeError(
  *                 f'malformed str/bytes length with leading 0. index {index}'
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_t_4)) {
 
-    /* "bencode2/_decoder.pyx":64
+    /* "bencode2/_decoder.pyx":69
  *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
  *         if x[index] == c'0':
  *             raise BencodeDecodeError(             # <<<<<<<<<<<<<<
  *                 f'malformed str/bytes length with leading 0. index {index}'
  *             )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "bencode2/_decoder.pyx":65
+    /* "bencode2/_decoder.pyx":70
  *         if x[index] == c'0':
  *             raise BencodeDecodeError(
  *                 f'malformed str/bytes length with leading 0. index {index}'             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_malformed_str_bytes_length_with, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 65, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_malformed_str_bytes_length_with, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 70, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
@@ -4334,171 +4550,331 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_5};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 64, __pyx_L1_error)
+    __PYX_ERR(0, 69, __pyx_L1_error)
 
-    /* "bencode2/_decoder.pyx":63
+    /* "bencode2/_decoder.pyx":68
  * 
  *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
  *         if x[index] == c'0':             # <<<<<<<<<<<<<<
  *             raise BencodeDecodeError(
  *                 f'malformed str/bytes length with leading 0. index {index}'
  */
   }
 
-  /* "bencode2/_decoder.pyx":68
+  /* "bencode2/_decoder.pyx":73
  *             )
  * 
  *         colon = x.index(b":", index)             # <<<<<<<<<<<<<<
- *         n = int(x[index:colon])
- * 
+ *         try:
+ *             n = int(x[index:colon])
  */
-  __pyx_t_3 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_index, __pyx_v_x, __pyx_kp_b_, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_index, __pyx_v_x, __pyx_kp_b_, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_colon = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "bencode2/_decoder.pyx":69
+  /* "bencode2/_decoder.pyx":74
+ * 
+ *         colon = x.index(b":", index)
+ *         try:             # <<<<<<<<<<<<<<
+ *             n = int(x[index:colon])
+ *         except ValueError:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_7, &__pyx_t_8, &__pyx_t_9);
+    __Pyx_XGOTREF(__pyx_t_7);
+    __Pyx_XGOTREF(__pyx_t_8);
+    __Pyx_XGOTREF(__pyx_t_9);
+    /*try:*/ {
+
+      /* "bencode2/_decoder.pyx":75
+ *         colon = x.index(b":", index)
+ *         try:
+ *             n = int(x[index:colon])             # <<<<<<<<<<<<<<
+ *         except ValueError:
+ *             raise BencodeDecodeError(f'malformed str/bytes length {x[index:colon]}, index {index}')
+ */
+      __Pyx_INCREF(__pyx_v_index);
+      __pyx_t_10 = __pyx_v_index;
+      __pyx_t_4 = (__pyx_t_10 == ((PyObject*)Py_None));
+      if (__pyx_t_4) {
+        __pyx_t_11 = 0;
+      } else {
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_10); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L4_error)
+        __pyx_t_11 = __pyx_t_12;
+      }
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __Pyx_INCREF(__pyx_v_colon);
+      __pyx_t_3 = __pyx_v_colon;
+      __pyx_t_4 = (__pyx_t_3 == Py_None);
+      if (__pyx_t_4) {
+        __pyx_t_12 = PY_SSIZE_T_MAX;
+      } else {
+        __pyx_t_13 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_13 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L4_error)
+        __pyx_t_12 = __pyx_t_13;
+      }
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = PySequence_GetSlice(__pyx_v_x, __pyx_t_11, __pyx_t_12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L4_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L4_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_v_n = __pyx_t_2;
+      __pyx_t_2 = 0;
+
+      /* "bencode2/_decoder.pyx":74
  * 
  *         colon = x.index(b":", index)
- *         n = int(x[index:colon])             # <<<<<<<<<<<<<<
+ *         try:             # <<<<<<<<<<<<<<
+ *             n = int(x[index:colon])
+ *         except ValueError:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    goto __pyx_L9_try_end;
+    __pyx_L4_error:;
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    /* "bencode2/_decoder.pyx":76
+ *         try:
+ *             n = int(x[index:colon])
+ *         except ValueError:             # <<<<<<<<<<<<<<
+ *             raise BencodeDecodeError(f'malformed str/bytes length {x[index:colon]}, index {index}')
+ * 
+ */
+    __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
+    if (__pyx_t_6) {
+      __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode_str", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_2, &__pyx_t_3, &__pyx_t_5) < 0) __PYX_ERR(0, 76, __pyx_L6_except_error)
+      __Pyx_XGOTREF(__pyx_t_2);
+      __Pyx_XGOTREF(__pyx_t_3);
+      __Pyx_XGOTREF(__pyx_t_5);
+
+      /* "bencode2/_decoder.pyx":77
+ *             n = int(x[index:colon])
+ *         except ValueError:
+ *             raise BencodeDecodeError(f'malformed str/bytes length {x[index:colon]}, index {index}')             # <<<<<<<<<<<<<<
  * 
  *         colon += 1
  */
-  __Pyx_INCREF(__pyx_v_index);
-  __pyx_t_7 = __pyx_v_index;
-  __pyx_t_4 = (__pyx_t_7 == ((PyObject*)Py_None));
-  if (__pyx_t_4) {
-    __pyx_t_8 = 0;
-  } else {
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_7); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 69, __pyx_L1_error)
-    __pyx_t_8 = __pyx_t_9;
-  }
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __Pyx_INCREF(__pyx_v_colon);
-  __pyx_t_3 = __pyx_v_colon;
-  __pyx_t_4 = (__pyx_t_3 == Py_None);
-  if (__pyx_t_4) {
-    __pyx_t_9 = PY_SSIZE_T_MAX;
-  } else {
-    __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 69, __pyx_L1_error)
-    __pyx_t_9 = __pyx_t_10;
+      __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 77, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_14);
+      __pyx_t_15 = PyTuple_New(4); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 77, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_15);
+      __pyx_t_12 = 0;
+      __pyx_t_16 = 127;
+      __Pyx_INCREF(__pyx_kp_u_malformed_str_bytes_length);
+      __pyx_t_12 += 27;
+      __Pyx_GIVEREF(__pyx_kp_u_malformed_str_bytes_length);
+      PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_kp_u_malformed_str_bytes_length);
+      __Pyx_INCREF(__pyx_v_index);
+      __pyx_t_10 = __pyx_v_index;
+      __pyx_t_4 = (__pyx_t_10 == ((PyObject*)Py_None));
+      if (__pyx_t_4) {
+        __pyx_t_11 = 0;
+      } else {
+        __pyx_t_13 = __Pyx_PyIndex_AsSsize_t(__pyx_t_10); if (unlikely((__pyx_t_13 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L6_except_error)
+        __pyx_t_11 = __pyx_t_13;
+      }
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __Pyx_INCREF(__pyx_v_colon);
+      __pyx_t_17 = __pyx_v_colon;
+      __pyx_t_4 = (__pyx_t_17 == Py_None);
+      if (__pyx_t_4) {
+        __pyx_t_13 = PY_SSIZE_T_MAX;
+      } else {
+        __pyx_t_18 = __Pyx_PyIndex_AsSsize_t(__pyx_t_17); if (unlikely((__pyx_t_18 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L6_except_error)
+        __pyx_t_13 = __pyx_t_18;
+      }
+      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+      __pyx_t_17 = PySequence_GetSlice(__pyx_v_x, __pyx_t_11, __pyx_t_13); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 77, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_17);
+      __pyx_t_19 = __Pyx_PyObject_FormatSimple(__pyx_t_17, __pyx_empty_unicode); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 77, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+      __pyx_t_16 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) > __pyx_t_16) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) : __pyx_t_16;
+      __pyx_t_12 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_19);
+      __Pyx_GIVEREF(__pyx_t_19);
+      PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_19);
+      __pyx_t_19 = 0;
+      __Pyx_INCREF(__pyx_kp_u_index_2);
+      __pyx_t_12 += 8;
+      __Pyx_GIVEREF(__pyx_kp_u_index_2);
+      PyTuple_SET_ITEM(__pyx_t_15, 2, __pyx_kp_u_index_2);
+      __pyx_t_19 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 77, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __pyx_t_16 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) > __pyx_t_16) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_19) : __pyx_t_16;
+      __pyx_t_12 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_19);
+      __Pyx_GIVEREF(__pyx_t_19);
+      PyTuple_SET_ITEM(__pyx_t_15, 3, __pyx_t_19);
+      __pyx_t_19 = 0;
+      __pyx_t_19 = __Pyx_PyUnicode_Join(__pyx_t_15, 4, __pyx_t_12, __pyx_t_16); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 77, __pyx_L6_except_error)
+      __Pyx_GOTREF(__pyx_t_19);
+      __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
+      __pyx_t_15 = NULL;
+      __pyx_t_6 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_14))) {
+        __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_14);
+        if (likely(__pyx_t_15)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_14);
+          __Pyx_INCREF(__pyx_t_15);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_14, function);
+          __pyx_t_6 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_15, __pyx_t_19};
+        __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_14, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+        __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
+        __Pyx_DECREF(__pyx_t_19); __pyx_t_19 = 0;
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L6_except_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+      }
+      __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __PYX_ERR(0, 77, __pyx_L6_except_error)
+    }
+    goto __pyx_L6_except_error;
+
+    /* "bencode2/_decoder.pyx":74
+ * 
+ *         colon = x.index(b":", index)
+ *         try:             # <<<<<<<<<<<<<<
+ *             n = int(x[index:colon])
+ *         except ValueError:
+ */
+    __pyx_L6_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_7);
+    __Pyx_XGIVEREF(__pyx_t_8);
+    __Pyx_XGIVEREF(__pyx_t_9);
+    __Pyx_ExceptionReset(__pyx_t_7, __pyx_t_8, __pyx_t_9);
+    goto __pyx_L1_error;
+    __pyx_L9_try_end:;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PySequence_GetSlice(__pyx_v_x, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_v_n = __pyx_t_2;
-  __pyx_t_2 = 0;
 
-  /* "bencode2/_decoder.pyx":71
- *         n = int(x[index:colon])
+  /* "bencode2/_decoder.pyx":79
+ *             raise BencodeDecodeError(f'malformed str/bytes length {x[index:colon]}, index {index}')
  * 
  *         colon += 1             # <<<<<<<<<<<<<<
  *         s = x[colon: colon + n]
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_colon, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF_SET(__pyx_v_colon, __pyx_t_2);
-  __pyx_t_2 = 0;
+  __pyx_t_5 = __Pyx_PyInt_AddObjC(__pyx_v_colon, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF_SET(__pyx_v_colon, __pyx_t_5);
+  __pyx_t_5 = 0;
 
-  /* "bencode2/_decoder.pyx":72
+  /* "bencode2/_decoder.pyx":80
  * 
  *         colon += 1
  *         s = x[colon: colon + n]             # <<<<<<<<<<<<<<
  * 
  *         return s, colon + n
  */
   __Pyx_INCREF(__pyx_v_colon);
-  __pyx_t_2 = __pyx_v_colon;
-  __pyx_t_4 = (__pyx_t_2 == Py_None);
+  __pyx_t_5 = __pyx_v_colon;
+  __pyx_t_4 = (__pyx_t_5 == Py_None);
   if (__pyx_t_4) {
-    __pyx_t_9 = 0;
+    __pyx_t_12 = 0;
   } else {
-    __pyx_t_8 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_8 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L1_error)
-    __pyx_t_9 = __pyx_t_8;
+    __pyx_t_13 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_13 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_12 = __pyx_t_13;
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = (__pyx_t_2 == Py_None);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = (__pyx_t_5 == Py_None);
   if (__pyx_t_4) {
-    __pyx_t_8 = PY_SSIZE_T_MAX;
+    __pyx_t_13 = PY_SSIZE_T_MAX;
   } else {
-    __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L1_error)
-    __pyx_t_8 = __pyx_t_10;
+    __pyx_t_11 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_11 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_13 = __pyx_t_11;
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PySequence_GetSlice(__pyx_v_x, __pyx_t_9, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_v_s = ((PyObject*)__pyx_t_2);
-  __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = PySequence_GetSlice(__pyx_v_x, __pyx_t_12, __pyx_t_13); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_v_s = ((PyObject*)__pyx_t_5);
+  __pyx_t_5 = 0;
 
-  /* "bencode2/_decoder.pyx":74
+  /* "bencode2/_decoder.pyx":82
  *         s = x[colon: colon + n]
  * 
  *         return s, colon + n             # <<<<<<<<<<<<<<
  * 
  *     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+  __pyx_t_5 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_s);
   __Pyx_GIVEREF(__pyx_v_s);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_s)) __PYX_ERR(0, 74, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error);
-  __pyx_t_2 = 0;
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_s)) __PYX_ERR(0, 82, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_5)) __PYX_ERR(0, 82, __pyx_L1_error);
+  __pyx_t_5 = 0;
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/_decoder.pyx":62
+  /* "bencode2/_decoder.pyx":67
  *         return r, index + 1
  * 
  *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         if x[index] == c'0':
  *             raise BencodeDecodeError(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_14);
+  __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_17);
+  __Pyx_XDECREF(__pyx_t_19);
   __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode_str", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_colon);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_decoder.pyx":76
+/* "bencode2/_decoder.pyx":84
  *         return s, colon + n
  * 
  *     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         index += 1
  * 
  */
 
@@ -4513,195 +4889,195 @@
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_Decoder__decode_dict", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "bencode2/_decoder.pyx":77
+  /* "bencode2/_decoder.pyx":85
  * 
  *     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):
  *         index += 1             # <<<<<<<<<<<<<<
  * 
  *         r = {}
  */
-  __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 77, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "bencode2/_decoder.pyx":79
+  /* "bencode2/_decoder.pyx":87
  *         index += 1
  * 
  *         r = {}             # <<<<<<<<<<<<<<
  *         while x[index] != c'e':
  *             k, index = self.__decode_str(x, index)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bencode2/_decoder.pyx":80
+  /* "bencode2/_decoder.pyx":88
  * 
  *         r = {}
  *         while x[index] != c'e':             # <<<<<<<<<<<<<<
  *             k, index = self.__decode_str(x, index)
  *             if self.str_key:
  */
   while (1) {
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyInt_From_char('e'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_char('e'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (!__pyx_t_4) break;
 
-    /* "bencode2/_decoder.pyx":81
+    /* "bencode2/_decoder.pyx":89
  *         r = {}
  *         while x[index] != c'e':
  *             k, index = self.__decode_str(x, index)             # <<<<<<<<<<<<<<
  *             if self.str_key:
  *                 k = k.decode(encoding='utf-8', errors='strict')
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode_str(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode_str(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (likely(__pyx_t_3 != Py_None)) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 81, __pyx_L1_error)
+        __PYX_ERR(0, 89, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_1);
       #else
-      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+      __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 81, __pyx_L1_error)
+      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 89, __pyx_L1_error)
     }
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 81, __pyx_L1_error)
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "bencode2/_decoder.pyx":82
+    /* "bencode2/_decoder.pyx":90
  *         while x[index] != c'e':
  *             k, index = self.__decode_str(x, index)
  *             if self.str_key:             # <<<<<<<<<<<<<<
  *                 k = k.decode(encoding='utf-8', errors='strict')
  *             r[k], index = self.__decode(x, index)
  */
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_self->str_key); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 82, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_self->str_key); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 90, __pyx_L1_error)
     if (__pyx_t_4) {
 
-      /* "bencode2/_decoder.pyx":83
+      /* "bencode2/_decoder.pyx":91
  *             k, index = self.__decode_str(x, index)
  *             if self.str_key:
  *                 k = k.decode(encoding='utf-8', errors='strict')             # <<<<<<<<<<<<<<
  *             r[k], index = self.__decode(x, index)
  * 
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
-      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_errors, __pyx_n_u_strict) < 0) __PYX_ERR(0, 83, __pyx_L1_error)
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 83, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_errors, __pyx_n_u_strict) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF_SET(__pyx_v_k, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "bencode2/_decoder.pyx":82
+      /* "bencode2/_decoder.pyx":90
  *         while x[index] != c'e':
  *             k, index = self.__decode_str(x, index)
  *             if self.str_key:             # <<<<<<<<<<<<<<
  *                 k = k.decode(encoding='utf-8', errors='strict')
  *             r[k], index = self.__decode(x, index)
  */
     }
 
-    /* "bencode2/_decoder.pyx":84
+    /* "bencode2/_decoder.pyx":92
  *             if self.str_key:
  *                 k = k.decode(encoding='utf-8', errors='strict')
  *             r[k], index = self.__decode(x, index)             # <<<<<<<<<<<<<<
  * 
  *         return r, index + 1
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 84, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(__pyx_t_2 != Py_None)) {
       PyObject* sequence = __pyx_t_2;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 84, __pyx_L1_error)
+        __PYX_ERR(0, 92, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       #endif
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     } else {
-      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 84, __pyx_L1_error)
+      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 92, __pyx_L1_error)
     }
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 84, __pyx_L1_error)
-    if (unlikely((PyDict_SetItem(__pyx_v_r, __pyx_v_k, __pyx_t_1) < 0))) __PYX_ERR(0, 84, __pyx_L1_error)
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 92, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_r, __pyx_v_k, __pyx_t_1) < 0))) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
   }
 
-  /* "bencode2/_decoder.pyx":86
+  /* "bencode2/_decoder.pyx":94
  *             r[k], index = self.__decode(x, index)
  * 
  *         return r, index + 1             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_r);
   __Pyx_GIVEREF(__pyx_v_r);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_r)) __PYX_ERR(0, 86, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_r)) __PYX_ERR(0, 94, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/_decoder.pyx":76
+  /* "bencode2/_decoder.pyx":84
  *         return s, colon + n
  * 
  *     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         index += 1
  * 
  */
 
@@ -5781,21 +6157,25 @@
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_encoding, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 0, 1, 1},
     {&__pyx_n_s_errors, __pyx_k_errors, sizeof(__pyx_k_errors), 0, 0, 1, 1},
     {&__pyx_n_s_exceptions, __pyx_k_exceptions, sizeof(__pyx_k_exceptions), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-    {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
+    {&__pyx_kp_u_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 1, 0, 0},
+    {&__pyx_kp_u_index_2, __pyx_k_index_2, sizeof(__pyx_k_index_2), 0, 1, 0, 0},
+    {&__pyx_n_s_index_3, __pyx_k_index_3, sizeof(__pyx_k_index_3), 0, 0, 1, 1},
     {&__pyx_kp_u_integer_with_leading_zero_is_not, __pyx_k_integer_with_leading_zero_is_not, sizeof(__pyx_k_integer_with_leading_zero_is_not), 0, 1, 0, 0},
     {&__pyx_kp_u_invalid_bencode_value_data_after, __pyx_k_invalid_bencode_value_data_after, sizeof(__pyx_k_invalid_bencode_value_data_after), 0, 1, 0, 0},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_kp_u_malformed_int, __pyx_k_malformed_int, sizeof(__pyx_k_malformed_int), 0, 1, 0, 0},
+    {&__pyx_kp_u_malformed_str_bytes_length, __pyx_k_malformed_str_bytes_length, sizeof(__pyx_k_malformed_str_bytes_length), 0, 1, 0, 0},
     {&__pyx_kp_u_malformed_str_bytes_length_with, __pyx_k_malformed_str_bytes_length_with, sizeof(__pyx_k_malformed_str_bytes_length_with), 0, 1, 0, 0},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_kp_u_not_a_valid_bencode_bytes, __pyx_k_not_a_valid_bencode_bytes, sizeof(__pyx_k_not_a_valid_bencode_bytes), 0, 1, 0, 0},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
@@ -5901,18 +6281,19 @@
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   __pyx_umethod_PyBytes_Type_index.type = (PyObject*)&PyBytes_Type;
-  __pyx_umethod_PyBytes_Type_index.method_name = &__pyx_n_s_index;
+  __pyx_umethod_PyBytes_Type_index.method_name = &__pyx_n_s_index_3;
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_27736365 = PyInt_FromLong(27736365L); if (unlikely(!__pyx_int_27736365)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_148187747 = PyInt_FromLong(148187747L); if (unlikely(!__pyx_int_148187747)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_211139970 = PyInt_FromLong(211139970L); if (unlikely(!__pyx_int_211139970)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
```

### Comparing `bencode2-0.0.8/bencode2/_decoder.pyx` & `bencode2-0.0.9/bencode2/_decoder.pyx`

 * *Files 13% similar despite different names*

```diff
@@ -33,15 +33,20 @@
 
         raise BencodeDecodeError(
             f"unexpected token {x[index:index + 1]} at index {index}")
 
     cdef tuple[object, int] __decode_int(self, x: bytes, index: int):
         index += 1
         new_f = x.index(b"e", index)
-        n = int(x[index:new_f])
+        try:
+            n = int(x[index:new_f], 10)
+        except ValueError:
+            raise BencodeDecodeError(
+                f'malformed int {x[index:new_f]}. index {index}'
+            )
 
         if x[index] == c'-':
             if x[index + 1] == c"0":
                 raise BencodeDecodeError(
                     f'-0 is not allowed in bencoding. index: {index}'
                 )
         elif x[index] == c'0' and new_f != index + 1:
@@ -62,15 +67,18 @@
     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
         if x[index] == c'0':
             raise BencodeDecodeError(
                 f'malformed str/bytes length with leading 0. index {index}'
             )
 
         colon = x.index(b":", index)
-        n = int(x[index:colon])
+        try:
+            n = int(x[index:colon])
+        except ValueError:
+            raise BencodeDecodeError(f'malformed str/bytes length {x[index:colon]}, index {index}')
 
         colon += 1
         s = x[colon: colon + n]
 
         return s, colon + n
 
     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):
```

### Comparing `bencode2-0.0.8/bencode2/_encoder.c` & `bencode2-0.0.9/bencode2/_encoder.c`

 * *Files identical despite different names*

### Comparing `bencode2-0.0.8/bencode2/_encoder.pyx` & `bencode2-0.0.9/bencode2/_encoder.pyx`

 * *Files identical despite different names*

### Comparing `bencode2-0.0.8/bencode2/_exceptions.c` & `bencode2-0.0.9/bencode2/_exceptions.c`

 * *Files identical despite different names*

### Comparing `bencode2-0.0.8/bencode2.egg-info/PKG-INFO` & `bencode2-0.0.9/bencode2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencode2
-Version: 0.0.8
+Version: 0.0.9
 Summary: bencode serialize/deserialize library
 Home-page: https://github.com/trim21/py-bencode
 Author: trim21
 Author-email: trim21.me@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bencode2-0.0.8/setup.py` & `bencode2-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 extensions = [
     # Everything but primes.pyx is included here.
     Extension("*", ["**/*.pyx"], define_macros=define_macros)
 ]
 
 setup(
     name="bencode2",
-    version="0.0.8",
+    version="0.0.9",
     description="bencode serialize/deserialize library",
     long_description=get_readme(),
     long_description_content_type="text/markdown",
     author="trim21",
     author_email="trim21.me@gmail.com",
     url="https://github.com/trim21/py-bencode",
     package_dir={"bencode2": "bencode2"},
```

### Comparing `bencode2-0.0.8/tests/test_decode.py` & `bencode2-0.0.9/tests/test_decode.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,28 @@
     with pytest.raises(BencodeDecodeError):
         bdecode(b"i-0e")
 
     with pytest.raises(BencodeDecodeError):
         bdecode(b"i01e")
 
     with pytest.raises(BencodeDecodeError):
+        bdecode(b"iabce")
+
+    with pytest.raises(BencodeDecodeError):
         # empty str
         print(bdecode(b"d0:4:spam3:fooi42ee"))
 
     with pytest.raises(BencodeDecodeError):
         # empty str
         bdecode(b"0:")
 
+    with pytest.raises(BencodeDecodeError):
+        # empty str
+        bdecode(b"1a2:qwer")
+
 
 def test_decode1():
     assert bdecode(b"d1:ad2:id20:abcdefghij0123456789e1:q4:ping1:t2:aa1:y1:qe") == {
         b"a": {b"id": b"abcdefghij0123456789"},
         b"q": b"ping",
         b"t": b"aa",
         b"y": b"q",
```

### Comparing `bencode2-0.0.8/tests/test_encode.py` & `bencode2-0.0.9/tests/test_encode.py`

 * *Files identical despite different names*

