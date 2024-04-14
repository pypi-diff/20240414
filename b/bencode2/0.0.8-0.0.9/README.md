# Comparing `tmp/bencode2-0.0.8-cp39-cp39-win_amd64.whl.zip` & `tmp/bencode2-0.0.9-cp36-cp36m-musllinux_1_1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,21 @@
-Zip file size: 247586 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      592 b- defN 24-Apr-14 14:19 bencode2/__init__.py
--rw-rw-rw-  2.0 fat   470738 b- defN 24-Apr-14 14:21 bencode2/_decoder.c
--rw-rw-rw-  2.0 fat    75776 b- defN 24-Apr-14 14:22 bencode2/_decoder.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2711 b- defN 24-Apr-14 14:19 bencode2/_decoder.pyx
--rw-rw-rw-  2.0 fat   375816 b- defN 24-Apr-14 14:22 bencode2/_encoder.c
--rw-rw-rw-  2.0 fat    54784 b- defN 24-Apr-14 14:22 bencode2/_encoder.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2993 b- defN 24-Apr-14 14:19 bencode2/_encoder.pyx
--rw-rw-rw-  2.0 fat   190932 b- defN 24-Apr-14 14:21 bencode2/_exceptions.c
--rw-rw-rw-  2.0 fat    24064 b- defN 24-Apr-14 14:22 bencode2/_exceptions.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      176 b- defN 24-Apr-14 14:19 bencode2/_exceptions.pyx
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-14 14:19 bencode2/py.typed
--rw-rw-rw-  2.0 fat     1106 b- defN 24-Apr-14 14:22 bencode2-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      665 b- defN 24-Apr-14 14:22 bencode2-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-14 14:22 bencode2-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-14 14:22 bencode2-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1295 b- defN 24-Apr-14 14:22 bencode2-0.0.8.dist-info/RECORD
-16 files, 1201757 bytes uncompressed, 245472 bytes compressed:  79.6%
+Zip file size: 552139 bytes, number of entries: 19
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-14 14:32 bencode2.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-14 14:32 bencode2-0.0.9.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-14 14:32 bencode2/
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-14 14:32 bencode2-0.0.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      674 b- defN 24-Apr-14 14:32 bencode2-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 24-Apr-14 14:32 bencode2-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1353 b- defN 24-Apr-14 14:32 bencode2-0.0.9.dist-info/RECORD
+-rw-r--r--  2.0 unx     1085 b- defN 24-Apr-14 14:32 bencode2-0.0.9.dist-info/LICENSE
+-rwxr-xr-x  2.0 unx   106208 b- defN 24-Apr-14 14:32 bencode2/_exceptions.cpython-36m-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   433240 b- defN 24-Apr-14 14:32 bencode2/_encoder.cpython-36m-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   641536 b- defN 24-Apr-14 14:32 bencode2/_decoder.cpython-36m-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      568 b- defN 24-Apr-14 14:32 bencode2/__init__.py
+-rw-r--r--  2.0 unx   487607 b- defN 24-Apr-14 14:32 bencode2/_decoder.c
+-rw-r--r--  2.0 unx   375778 b- defN 24-Apr-14 14:32 bencode2/_encoder.c
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-14 14:32 bencode2/py.typed
+-rw-r--r--  2.0 unx     2890 b- defN 24-Apr-14 14:32 bencode2/_encoder.pyx
+-rw-r--r--  2.0 unx   190928 b- defN 24-Apr-14 14:32 bencode2/_exceptions.c
+-rw-r--r--  2.0 unx      168 b- defN 24-Apr-14 14:32 bencode2/_exceptions.pyx
+-rw-r--r--  2.0 unx     2934 b- defN 24-Apr-14 14:32 bencode2/_decoder.pyx
+19 files, 2245090 bytes uncompressed, 549623 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,49 +1,58 @@
-Filename: bencode2/__init__.py
+Filename: bencode2.libs/
 Comment: 
 
-Filename: bencode2/_decoder.c
+Filename: bencode2-0.0.9.dist-info/
 Comment: 
 
-Filename: bencode2/_decoder.cp39-win_amd64.pyd
+Filename: bencode2/
 Comment: 
 
-Filename: bencode2/_decoder.pyx
+Filename: bencode2-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bencode2/_encoder.c
+Filename: bencode2-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: bencode2/_encoder.cp39-win_amd64.pyd
+Filename: bencode2-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: bencode2/_encoder.pyx
+Filename: bencode2-0.0.9.dist-info/RECORD
 Comment: 
 
-Filename: bencode2/_exceptions.c
+Filename: bencode2-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: bencode2/_exceptions.cp39-win_amd64.pyd
+Filename: bencode2/_exceptions.cpython-36m-x86_64-linux-gnu.so
 Comment: 
 
-Filename: bencode2/_exceptions.pyx
+Filename: bencode2/_encoder.cpython-36m-x86_64-linux-gnu.so
 Comment: 
 
-Filename: bencode2/py.typed
+Filename: bencode2/_decoder.cpython-36m-x86_64-linux-gnu.so
+Comment: 
+
+Filename: bencode2/__init__.py
 Comment: 
 
-Filename: bencode2-0.0.8.dist-info/LICENSE
+Filename: bencode2/_decoder.c
 Comment: 
 
-Filename: bencode2-0.0.8.dist-info/METADATA
+Filename: bencode2/_encoder.c
 Comment: 
 
-Filename: bencode2-0.0.8.dist-info/WHEEL
+Filename: bencode2/py.typed
 Comment: 
 
-Filename: bencode2-0.0.8.dist-info/top_level.txt
+Filename: bencode2/_encoder.pyx
 Comment: 
 
-Filename: bencode2-0.0.8.dist-info/RECORD
+Filename: bencode2/_exceptions.c
+Comment: 
+
+Filename: bencode2/_exceptions.pyx
+Comment: 
+
+Filename: bencode2/_decoder.pyx
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## bencode2/__init__.py

 * *Ordering differences only*

```diff
@@ -1,24 +1,24 @@
-# cython: language_level=3
-
-from typing import Any
-
-from ._decoder import Decoder as _Decoder
-from ._encoder import encode as _encode
-from ._exceptions import BencodeDecodeError, BencodeEncodeError
-
-__all__ = (
-    "BencodeDecodeError",
-    "BencodeEncodeError",
-    "bencode",
-    "bdecode",
-)
-
-
-def bencode(value: Any) -> bytes:
-    """Encode value into the bencode format."""
-    return _encode(value)
-
-
-def bdecode(value: bytes, *, str_key: bool = False) -> Any:
-    """Decode bencode formatted bytes to python value."""
-    return _Decoder(str_key).decode(value)
+# cython: language_level=3
+
+from typing import Any
+
+from ._decoder import Decoder as _Decoder
+from ._encoder import encode as _encode
+from ._exceptions import BencodeDecodeError, BencodeEncodeError
+
+__all__ = (
+    "BencodeDecodeError",
+    "BencodeEncodeError",
+    "bencode",
+    "bdecode",
+)
+
+
+def bencode(value: Any) -> bytes:
+    """Encode value into the bencode format."""
+    return _encode(value)
+
+
+def bdecode(value: bytes, *, str_key: bool = False) -> Any:
+    """Decode bencode formatted bytes to python value."""
+    return _Decoder(str_key).decode(value)
```

## bencode2/_decoder.c

```diff
@@ -1,15 +1,15 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "bencode2._decoder",
         "sources": [
-            "bencode2\\_decoder.pyx"
+            "bencode2/_decoder.pyx"
         ]
     },
     "module_name": "bencode2._decoder"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1475,15 +1475,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "bencode2\\\\_decoder.pyx",
+  "bencode2/_decoder.pyx",
   "<stringsource>",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
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
-static const char __pyx_k_bencode2__decoder_pyx[] = "bencode2\\_decoder.pyx";
+static const char __pyx_k_bencode2__decoder_pyx[] = "bencode2/_decoder.pyx";
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
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 43, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_1, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_t_1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 43, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(__pyx_t_4)) {
+    __pyx_t_1 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_12 = PyObject_RichCompare(__pyx_t_10, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_12); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
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
+        PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_13};
+        __pyx_t_12 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+        if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 49, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_Raise(__pyx_t_7, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __PYX_ERR(0, 44, __pyx_L1_error)
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
+      PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_10};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
+      __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     }
-    __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __PYX_ERR(0, 48, __pyx_L1_error)
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

## bencode2/_decoder.pyx

```diff
@@ -1,86 +1,94 @@
-# cython: language_level=3
-
-from typing import Any
-
-from ._exceptions import BencodeDecodeError
-
-cdef class Decoder:
-    str_key: bool
-
-    def __init__(self, str_key: bool):
-        self.str_key = str_key
-
-    def decode(self, value: bytes)-> Any:
-        try:
-            data, length = self.__decode(value, 0)
-        except (IndexError, KeyError, TypeError, ValueError) as e:
-            raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e
-
-        if length != len(value):
-            raise BencodeDecodeError("invalid bencode value (data after valid prefix)")
-
-        return data
-
-    cdef tuple[Any, int] __decode(self, x: bytes, index: int):
-        if x[index] == c'l':
-            return self.__decode_list(x, index)
-        if x[index] == c'i':
-            return self.__decode_int(x, index)
-        if x[index] == c'd':
-            return self.__decode_dict(x, index)
-        if c'0' < x[index] <= c'9':
-            return self.__decode_str(x, index)
-
-        raise BencodeDecodeError(
-            f"unexpected token {x[index:index + 1]} at index {index}")
-
-    cdef tuple[object, int] __decode_int(self, x: bytes, index: int):
-        index += 1
-        new_f = x.index(b"e", index)
-        n = int(x[index:new_f])
-
-        if x[index] == c'-':
-            if x[index + 1] == c"0":
-                raise BencodeDecodeError(
-                    f'-0 is not allowed in bencoding. index: {index}'
-                )
-        elif x[index] == c'0' and new_f != index + 1:
-            raise BencodeDecodeError(
-                f'integer with leading zero is not allowed. index: {index}'
-            )
-        return n, new_f + 1
-
-    cdef tuple[list, int] __decode_list(self, x: bytes, index: int):
-        r, index = [], index + 1
-
-        while x[index] != c'e':
-            v, index = self.__decode(x, index)
-            r.append(v)
-
-        return r, index + 1
-
-    cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
-        if x[index] == c'0':
-            raise BencodeDecodeError(
-                f'malformed str/bytes length with leading 0. index {index}'
-            )
-
-        colon = x.index(b":", index)
-        n = int(x[index:colon])
-
-        colon += 1
-        s = x[colon: colon + n]
-
-        return s, colon + n
-
-    cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):
-        index += 1
-
-        r = {}
-        while x[index] != c'e':
-            k, index = self.__decode_str(x, index)
-            if self.str_key:
-                k = k.decode(encoding='utf-8', errors='strict')
-            r[k], index = self.__decode(x, index)
-
-        return r, index + 1
+# cython: language_level=3
+
+from typing import Any
+
+from ._exceptions import BencodeDecodeError
+
+cdef class Decoder:
+    str_key: bool
+
+    def __init__(self, str_key: bool):
+        self.str_key = str_key
+
+    def decode(self, value: bytes)-> Any:
+        try:
+            data, length = self.__decode(value, 0)
+        except (IndexError, KeyError, TypeError, ValueError) as e:
+            raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e
+
+        if length != len(value):
+            raise BencodeDecodeError("invalid bencode value (data after valid prefix)")
+
+        return data
+
+    cdef tuple[Any, int] __decode(self, x: bytes, index: int):
+        if x[index] == c'l':
+            return self.__decode_list(x, index)
+        if x[index] == c'i':
+            return self.__decode_int(x, index)
+        if x[index] == c'd':
+            return self.__decode_dict(x, index)
+        if c'0' < x[index] <= c'9':
+            return self.__decode_str(x, index)
+
+        raise BencodeDecodeError(
+            f"unexpected token {x[index:index + 1]} at index {index}")
+
+    cdef tuple[object, int] __decode_int(self, x: bytes, index: int):
+        index += 1
+        new_f = x.index(b"e", index)
+        try:
+            n = int(x[index:new_f], 10)
+        except ValueError:
+            raise BencodeDecodeError(
+                f'malformed int {x[index:new_f]}. index {index}'
+            )
+
+        if x[index] == c'-':
+            if x[index + 1] == c"0":
+                raise BencodeDecodeError(
+                    f'-0 is not allowed in bencoding. index: {index}'
+                )
+        elif x[index] == c'0' and new_f != index + 1:
+            raise BencodeDecodeError(
+                f'integer with leading zero is not allowed. index: {index}'
+            )
+        return n, new_f + 1
+
+    cdef tuple[list, int] __decode_list(self, x: bytes, index: int):
+        r, index = [], index + 1
+
+        while x[index] != c'e':
+            v, index = self.__decode(x, index)
+            r.append(v)
+
+        return r, index + 1
+
+    cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
+        if x[index] == c'0':
+            raise BencodeDecodeError(
+                f'malformed str/bytes length with leading 0. index {index}'
+            )
+
+        colon = x.index(b":", index)
+        try:
+            n = int(x[index:colon])
+        except ValueError:
+            raise BencodeDecodeError(f'malformed str/bytes length {x[index:colon]}, index {index}')
+
+        colon += 1
+        s = x[colon: colon + n]
+
+        return s, colon + n
+
+    cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):
+        index += 1
+
+        r = {}
+        while x[index] != c'e':
+            k, index = self.__decode_str(x, index)
+            if self.str_key:
+                k = k.decode(encoding='utf-8', errors='strict')
+            r[k], index = self.__decode(x, index)
+
+        return r, index + 1
```

## bencode2/_encoder.c

```diff
@@ -2,15 +2,15 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "bencode2._encoder",
         "sources": [
-            "build\\lib.win-amd64-cpython-38\\bencode2\\_encoder.pyx"
+            "bencode2/_encoder.pyx"
         ]
     },
     "module_name": "bencode2._encoder"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1483,15 +1483,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "bencode2\\\\_encoder.pyx",
+  "bencode2/_encoder.pyx",
   "type.pxd",
   "bool.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
@@ -2334,15 +2334,15 @@
 static const char __pyx_k_not_supported[] = "' not supported";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_bencode2__encoder[] = "bencode2._encoder";
 static const char __pyx_k_BencodeEncodeError[] = "BencodeEncodeError";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_find_duplicated_keys[] = "find duplicated keys ";
-static const char __pyx_k_bencode2__encoder_pyx[] = "bencode2\\_encoder.pyx";
+static const char __pyx_k_bencode2__encoder_pyx[] = "bencode2/_encoder.pyx";
 static const char __pyx_k_encode_dict_locals_lambda[] = "__encode_dict.<locals>.<lambda>";
 static const char __pyx_k_expected_binary_or_text_found_s[] = "expected binary or text (found %s)";
 static const char __pyx_k_empty_bytes_is_not_allowed_in_be[] = "empty bytes is not allowed in bencoding";
 static const char __pyx_k_empty_string_is_not_allowed_in_b[] = "empty string is not allowed in bencoding";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8bencode2_8_encoder_encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_kv); /* proto */
```

## bencode2/_encoder.pyx

 * *Ordering differences only*

```diff
@@ -1,103 +1,103 @@
-# cython: language_level=3
-
-from collections.abc import Mapping
-from typing import Any
-
-from cpython.bytes cimport PyBytes_Check
-from cpython.int cimport PyInt_Check
-from cpython.list cimport PyList_Check, PyList_Append
-from cpython.tuple cimport PyTuple_Check
-from cpython.bool cimport PyBool_Check
-from cpython.dict cimport PyDict_Check
-from cpython.string cimport PyString_Check
-
-from ._exceptions import BencodeEncodeError
-
-cpdef bytes encode(value: Any):
-    r: list[bytes] = []  # makes more sense for something with lots of appends
-
-    __encode(value, r)
-
-    # Join parts
-    return b"".join(r)
-
-cdef __encode(value, r: list[bytes]):
-    if PyDict_Check(value):
-        __encode_dict(value, r)
-    elif PyString_Check(value):
-        __encode_str(value, r)
-    elif PyList_Check(value):
-        __encode_list(value, r)
-    elif PyTuple_Check(value):
-        __encode_list(value, r)
-    elif PyBytes_Check(value):
-        __encode_bytes(value, r)
-    elif PyBool_Check(value):
-        __encode_bool(value, r)
-    elif PyInt_Check(value):
-        __encode_int(value, r)
-    else:
-        raise BencodeEncodeError(f"type '{type(value)}' not supported")
-
-cdef __encode_int(x: int, r: list[bytes]):
-    r.extend((b"i", str(x).encode("utf-8"), b"e"))
-
-cdef __encode_bool(x: bool, r: list[bytes]):
-    if x:
-        __encode_int(1, r)
-    else:
-        __encode_int(0, r)
-
-cdef __encode_bytes(x: bytes, r: list[bytes]):
-    if not x:
-        raise BencodeEncodeError('empty bytes is not allowed in bencoding')
-    PyList_Append(r, str(len(x)).encode("utf-8"))
-    PyList_Append(r, b":")
-    PyList_Append(r, x)
-
-cdef __encode_str(x: str, r: list[bytes]):
-    if not x:
-        raise BencodeEncodeError('empty string is not allowed in bencoding')
-    __encode_bytes(x.encode("UTF-8"), r)
-
-cdef __encode_list(x: list | tuple, r: list[bytes]):
-    PyList_Append(r, b"l")
-
-    for i in x:
-        __encode(i, r)
-
-    PyList_Append(r, b"e")
-
-cdef __encode_dict(x: Mapping, r: list[bytes]):
-    PyList_Append(r, b"d")
-
-    # force all keys to bytes, because str and bytes are incomparable
-    i_list: list[tuple[bytes, Any]] = [(to_binary(k), v) for k, v in x.items()]
-    i_list.sort(key=lambda kv: kv[0])
-    __check_duplicated_keys(i_list)
-
-    for k, v in i_list:
-        __encode(k, r)
-        __encode(v, r)
-
-    PyList_Append(r, b"e")
-
-cdef __check_duplicated_keys(s: list[tuple[bytes, Any]]):
-    if len(s) == 0:
-        return
-    last_key: bytes = s[0][0]
-    for current, _ in s[1:]:
-        if last_key == current:
-            raise BencodeEncodeError(
-                f'find duplicated keys {last_key} and {current.decode()}'
-            )
-        last_key = current
-
-cdef to_binary(s: str | bytes):
-    if PyBytes_Check(s):
-        return s
-
-    if PyString_Check(s):
-        return s.encode("utf-8", "strict")
-
-    raise TypeError("expected binary or text (found %s)" % type(s))
+# cython: language_level=3
+
+from collections.abc import Mapping
+from typing import Any
+
+from cpython.bytes cimport PyBytes_Check
+from cpython.int cimport PyInt_Check
+from cpython.list cimport PyList_Check, PyList_Append
+from cpython.tuple cimport PyTuple_Check
+from cpython.bool cimport PyBool_Check
+from cpython.dict cimport PyDict_Check
+from cpython.string cimport PyString_Check
+
+from ._exceptions import BencodeEncodeError
+
+cpdef bytes encode(value: Any):
+    r: list[bytes] = []  # makes more sense for something with lots of appends
+
+    __encode(value, r)
+
+    # Join parts
+    return b"".join(r)
+
+cdef __encode(value, r: list[bytes]):
+    if PyDict_Check(value):
+        __encode_dict(value, r)
+    elif PyString_Check(value):
+        __encode_str(value, r)
+    elif PyList_Check(value):
+        __encode_list(value, r)
+    elif PyTuple_Check(value):
+        __encode_list(value, r)
+    elif PyBytes_Check(value):
+        __encode_bytes(value, r)
+    elif PyBool_Check(value):
+        __encode_bool(value, r)
+    elif PyInt_Check(value):
+        __encode_int(value, r)
+    else:
+        raise BencodeEncodeError(f"type '{type(value)}' not supported")
+
+cdef __encode_int(x: int, r: list[bytes]):
+    r.extend((b"i", str(x).encode("utf-8"), b"e"))
+
+cdef __encode_bool(x: bool, r: list[bytes]):
+    if x:
+        __encode_int(1, r)
+    else:
+        __encode_int(0, r)
+
+cdef __encode_bytes(x: bytes, r: list[bytes]):
+    if not x:
+        raise BencodeEncodeError('empty bytes is not allowed in bencoding')
+    PyList_Append(r, str(len(x)).encode("utf-8"))
+    PyList_Append(r, b":")
+    PyList_Append(r, x)
+
+cdef __encode_str(x: str, r: list[bytes]):
+    if not x:
+        raise BencodeEncodeError('empty string is not allowed in bencoding')
+    __encode_bytes(x.encode("UTF-8"), r)
+
+cdef __encode_list(x: list | tuple, r: list[bytes]):
+    PyList_Append(r, b"l")
+
+    for i in x:
+        __encode(i, r)
+
+    PyList_Append(r, b"e")
+
+cdef __encode_dict(x: Mapping, r: list[bytes]):
+    PyList_Append(r, b"d")
+
+    # force all keys to bytes, because str and bytes are incomparable
+    i_list: list[tuple[bytes, Any]] = [(to_binary(k), v) for k, v in x.items()]
+    i_list.sort(key=lambda kv: kv[0])
+    __check_duplicated_keys(i_list)
+
+    for k, v in i_list:
+        __encode(k, r)
+        __encode(v, r)
+
+    PyList_Append(r, b"e")
+
+cdef __check_duplicated_keys(s: list[tuple[bytes, Any]]):
+    if len(s) == 0:
+        return
+    last_key: bytes = s[0][0]
+    for current, _ in s[1:]:
+        if last_key == current:
+            raise BencodeEncodeError(
+                f'find duplicated keys {last_key} and {current.decode()}'
+            )
+        last_key = current
+
+cdef to_binary(s: str | bytes):
+    if PyBytes_Check(s):
+        return s
+
+    if PyString_Check(s):
+        return s.encode("utf-8", "strict")
+
+    raise TypeError("expected binary or text (found %s)" % type(s))
```

## bencode2/_exceptions.c

```diff
@@ -1,15 +1,15 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "bencode2._exceptions",
         "sources": [
-            "bencode2\\_exceptions.pyx"
+            "bencode2/_exceptions.pyx"
         ]
     },
     "module_name": "bencode2._exceptions"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1475,15 +1475,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "bencode2\\\\_exceptions.pyx",
+  "bencode2/_exceptions.pyx",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
```

## bencode2/_exceptions.pyx

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-# cython: language_level=3
-
-class BencodeDecodeError(Exception):
-    """Bencode decode error."""
-
-
-class BencodeEncodeError(Exception):
-    """Bencode encode error."""
+# cython: language_level=3
+
+class BencodeDecodeError(Exception):
+    """Bencode decode error."""
+
+
+class BencodeEncodeError(Exception):
+    """Bencode encode error."""
```

## Comparing `bencode2-0.0.8.dist-info/LICENSE` & `bencode2-0.0.9.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 trim21 <trim21.me@gmail.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 trim21 <trim21.me@gmail.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

