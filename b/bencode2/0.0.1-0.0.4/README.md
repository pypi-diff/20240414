# Comparing `tmp/bencode2-0.0.1.tar.gz` & `tmp/bencode2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode2-0.0.1.tar", last modified: Sun Apr 14 05:01:23 2024, max compression
+gzip compressed data, was "bencode2-0.0.4.tar", last modified: Sun Apr 14 07:39:28 2024, max compression
```

## Comparing `bencode2-0.0.1.tar` & `bencode2-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 05:01:23.014225 bencode2-0.0.1/
--rw-rw-rw-   0        0        0      150 2024-04-14 01:34:18.000000 bencode2-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0       41 2024-04-14 01:34:18.000000 bencode2-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      331 2024-04-14 05:01:23.013225 bencode2-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 05:01:23.006218 bencode2-0.0.1/bencode2/
--rw-rw-rw-   0        0        0      811 2024-04-14 04:16:17.000000 bencode2-0.0.1/bencode2/__init__.py
--rw-rw-rw-   0        0        0   253955 2024-04-14 04:19:28.000000 bencode2-0.0.1/bencode2/_compat.c
--rw-rw-rw-   0        0        0      232 2024-04-14 03:00:52.000000 bencode2-0.0.1/bencode2/_compat.pyx
--rw-rw-rw-   0        0        0   425532 2024-04-14 04:35:45.000000 bencode2-0.0.1/bencode2/decoder.c
--rw-rw-rw-   0        0        0     2837 2024-04-14 04:29:10.000000 bencode2-0.0.1/bencode2/decoder.pyx
--rw-rw-rw-   0        0        0   350900 2024-04-14 04:43:34.000000 bencode2-0.0.1/bencode2/encoder.c
--rw-rw-rw-   0        0        0     2214 2024-04-14 04:35:34.000000 bencode2-0.0.1/bencode2/encoder.pyx
--rw-rw-rw-   0        0        0   190889 2024-04-14 04:20:11.000000 bencode2-0.0.1/bencode2/exceptions.c
--rw-rw-rw-   0        0        0      176 2024-04-14 03:01:14.000000 bencode2-0.0.1/bencode2/exceptions.pyx
--rw-rw-rw-   0        0        0        0 2024-04-14 02:16:18.000000 bencode2-0.0.1/bencode2/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-14 05:01:23.013225 bencode2-0.0.1/bencode2.egg-info/
--rw-rw-rw-   0        0        0      331 2024-04-14 05:01:22.000000 bencode2-0.0.1/bencode2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2024-04-14 05:01:22.000000 bencode2-0.0.1/bencode2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 05:01:22.000000 bencode2-0.0.1/bencode2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 05:01:22.000000 bencode2-0.0.1/bencode2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       60 2024-04-14 03:26:16.000000 bencode2-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 05:01:23.014225 bencode2-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2024-04-14 05:00:59.000000 bencode2-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 05:01:23.011223 bencode2-0.0.1/tests/
--rw-rw-rw-   0        0        0      267 2024-04-14 01:48:57.000000 bencode2-0.0.1/tests/test_decode.py
--rw-rw-rw-   0        0        0     2565 2024-04-14 04:23:09.000000 bencode2-0.0.1/tests/test_encode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:39:28.948108 bencode2-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-14 07:39:24.000000 bencode2-0.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 07:39:24.000000 bencode2-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-14 07:39:28.948108 bencode2-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:39:28.944108 bencode2-0.0.4/bencode2/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-14 07:39:24.000000 bencode2-0.0.4/bencode2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   260090 2024-04-14 07:39:28.000000 bencode2-0.0.4/bencode2/_compat.c
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-14 07:39:24.000000 bencode2-0.0.4/bencode2/_compat.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   425745 2024-04-14 07:39:28.000000 bencode2-0.0.4/bencode2/_decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-14 07:39:24.000000 bencode2-0.0.4/bencode2/_decoder.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   351081 2024-04-14 07:39:28.000000 bencode2-0.0.4/bencode2/_encoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-14 07:39:24.000000 bencode2-0.0.4/bencode2/_encoder.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   190928 2024-04-14 07:39:28.000000 bencode2-0.0.4/bencode2/_exceptions.c
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-14 07:39:24.000000 bencode2-0.0.4/bencode2/_exceptions.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 07:39:24.000000 bencode2-0.0.4/bencode2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:39:28.948108 bencode2-0.0.4/bencode2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-14 07:39:28.000000 bencode2-0.0.4/bencode2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 07:39:28.000000 bencode2-0.0.4/bencode2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:39:28.000000 bencode2-0.0.4/bencode2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 07:39:28.000000 bencode2-0.0.4/bencode2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 07:39:24.000000 bencode2-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 07:39:28.948108 bencode2-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-14 07:39:24.000000 bencode2-0.0.4/setup.py
```

### Comparing `bencode2-0.0.1/bencode2/__init__.py` & `bencode2-0.0.4/bencode2/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cython: language_level=3
 
 from typing import Any
 
-from .decoder import BencodeDecoder
-from .encoder import encode
-from .exceptions import BencodeDecodeError, BencodeEncodeError
+from ._decoder import BencodeDecoder
+from ._encoder import encode
+from ._exceptions import BencodeDecodeError, BencodeEncodeError
 
 __all__ = (
     "BencodeDecodeError",
     "BencodeEncodeError",
     "bencode",
     "bdecode",
 )
```

### Comparing `bencode2-0.0.1/bencode2/_compat.c` & `bencode2-0.0.4/bencode2/_compat.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
+        "depends": [],
         "name": "bencode2._compat",
         "sources": [
-            "bencode2\\_compat.pyx"
+            "bencode2/_compat.pyx"
         ]
     },
     "module_name": "bencode2._compat"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -1227,14 +1228,16 @@
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
 #define __PYX_HAVE__bencode2___compat
 #define __PYX_HAVE_API__bencode2___compat
 /* Early includes */
+#include <string.h>
+#include <stdio.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -1475,15 +1478,16 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "bencode2\\\\_compat.pyx",
+  "bencode2/_compat.pyx",
+  "type.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -1768,14 +1772,33 @@
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* TypeImport.proto */
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
+};
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
+#endif
+
 /* IncludeStructmemberH.proto */
 #include <structmember.h>
 
 /* FixUpExtensionType.proto */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
@@ -2023,14 +2046,30 @@
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 
+/* Module declarations from "libc.string" */
+
+/* Module declarations from "libc.stdio" */
+
+/* Module declarations from "__builtin__" */
+
+/* Module declarations from "cpython.type" */
+
+/* Module declarations from "cpython" */
+
+/* Module declarations from "cpython.object" */
+
+/* Module declarations from "cpython.bytes" */
+
+/* Module declarations from "cpython.string" */
+
 /* Module declarations from "bencode2._compat" */
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "bencode2._compat"
 extern int __pyx_module_is_main_bencode2___compat;
 int __pyx_module_is_main_bencode2___compat = 0;
 
@@ -2048,15 +2087,15 @@
 static const char __pyx_k_strict[] = "strict";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_to_binary[] = "to_binary";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_bencode2__compat[] = "bencode2._compat";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_bencode2__compat_pyx[] = "bencode2\\_compat.pyx";
+static const char __pyx_k_bencode2__compat_pyx[] = "bencode2/_compat.pyx";
 static const char __pyx_k_expected_binary_or_text_found_s[] = "expected binary or text (found %s)";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8bencode2_7_compat_to_binary(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_s); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
@@ -2081,14 +2120,31 @@
   PyTypeObject *__pyx_CoroutineAwaitType;
   #endif
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s__4;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_bencode2__compat;
   PyObject *__pyx_kp_s_bencode2__compat_pyx;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_encode;
@@ -2142,14 +2198,15 @@
   Py_CLEAR(clear_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s__4);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_bencode2__compat);
   Py_CLEAR(clear_module_state->__pyx_kp_s_bencode2__compat_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
@@ -2181,14 +2238,15 @@
   Py_VISIT(traverse_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s__4);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_bencode2__compat);
   Py_VISIT(traverse_module_state->__pyx_kp_s_bencode2__compat_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
@@ -2230,14 +2288,31 @@
 #define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
 #endif
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s__4 __pyx_mstate_global->__pyx_n_s__4
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_bencode2__compat __pyx_mstate_global->__pyx_n_s_bencode2__compat
 #define __pyx_kp_s_bencode2__compat_pyx __pyx_mstate_global->__pyx_kp_s_bencode2__compat_pyx
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
@@ -2251,19 +2326,19 @@
 #define __pyx_n_s_to_binary __pyx_mstate_global->__pyx_n_s_to_binary
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_codeobj__3 __pyx_mstate_global->__pyx_codeobj__3
 /* #### Code section: module_code ### */
 
-/* "bencode2/_compat.pyx":3
- * # cython: language_level=3
+/* "bencode2/_compat.pyx":6
+ * from cpython.string cimport PyString_Check
  * 
  * def to_binary(s):             # <<<<<<<<<<<<<<
- *     if isinstance(s, bytes):
+ *     if PyBytes_Check(s):
  *         return s
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8bencode2_7_compat_1to_binary(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
@@ -2312,31 +2387,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_s)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 6, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "to_binary") < 0)) __PYX_ERR(0, 3, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "to_binary") < 0)) __PYX_ERR(0, 6, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_s = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("to_binary", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 3, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("to_binary", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 6, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -2366,100 +2441,100 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("to_binary", 1);
 
-  /* "bencode2/_compat.pyx":4
+  /* "bencode2/_compat.pyx":7
  * 
  * def to_binary(s):
- *     if isinstance(s, bytes):             # <<<<<<<<<<<<<<
+ *     if PyBytes_Check(s):             # <<<<<<<<<<<<<<
  *         return s
  * 
  */
-  __pyx_t_1 = PyBytes_Check(__pyx_v_s); 
+  __pyx_t_1 = PyBytes_Check(__pyx_v_s);
   if (__pyx_t_1) {
 
-    /* "bencode2/_compat.pyx":5
+    /* "bencode2/_compat.pyx":8
  * def to_binary(s):
- *     if isinstance(s, bytes):
+ *     if PyBytes_Check(s):
  *         return s             # <<<<<<<<<<<<<<
  * 
- *     if isinstance(s, str):
+ *     if PyString_Check(s):
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_s);
     __pyx_r = __pyx_v_s;
     goto __pyx_L0;
 
-    /* "bencode2/_compat.pyx":4
+    /* "bencode2/_compat.pyx":7
  * 
  * def to_binary(s):
- *     if isinstance(s, bytes):             # <<<<<<<<<<<<<<
+ *     if PyBytes_Check(s):             # <<<<<<<<<<<<<<
  *         return s
  * 
  */
   }
 
-  /* "bencode2/_compat.pyx":7
+  /* "bencode2/_compat.pyx":10
  *         return s
  * 
- *     if isinstance(s, str):             # <<<<<<<<<<<<<<
+ *     if PyString_Check(s):             # <<<<<<<<<<<<<<
  *         return s.encode("utf-8", "strict")
  * 
  */
-  __pyx_t_1 = PyUnicode_Check(__pyx_v_s); 
+  __pyx_t_1 = PyString_Check(__pyx_v_s);
   if (__pyx_t_1) {
 
-    /* "bencode2/_compat.pyx":8
+    /* "bencode2/_compat.pyx":11
  * 
- *     if isinstance(s, str):
+ *     if PyString_Check(s):
  *         return s.encode("utf-8", "strict")             # <<<<<<<<<<<<<<
  * 
  *     raise TypeError("expected binary or text (found %s)" % type(s))
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 8, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 8, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "bencode2/_compat.pyx":7
+    /* "bencode2/_compat.pyx":10
  *         return s
  * 
- *     if isinstance(s, str):             # <<<<<<<<<<<<<<
+ *     if PyString_Check(s):             # <<<<<<<<<<<<<<
  *         return s.encode("utf-8", "strict")
  * 
  */
   }
 
-  /* "bencode2/_compat.pyx":10
+  /* "bencode2/_compat.pyx":13
  *         return s.encode("utf-8", "strict")
  * 
  *     raise TypeError("expected binary or text (found %s)" % type(s))             # <<<<<<<<<<<<<<
  */
-  __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_expected_binary_or_text_found_s, ((PyObject *)Py_TYPE(__pyx_v_s))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_expected_binary_or_text_found_s, ((PyObject *)Py_TYPE(__pyx_v_s))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_2, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __PYX_ERR(0, 10, __pyx_L1_error)
+  __PYX_ERR(0, 13, __pyx_L1_error)
 
-  /* "bencode2/_compat.pyx":3
- * # cython: language_level=3
+  /* "bencode2/_compat.pyx":6
+ * from cpython.string cimport PyString_Check
  * 
  * def to_binary(s):             # <<<<<<<<<<<<<<
- *     if isinstance(s, bytes):
+ *     if PyBytes_Check(s):
  *         return s
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -2505,47 +2580,47 @@
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 13, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "bencode2/_compat.pyx":8
+  /* "bencode2/_compat.pyx":11
  * 
- *     if isinstance(s, str):
+ *     if PyString_Check(s):
  *         return s.encode("utf-8", "strict")             # <<<<<<<<<<<<<<
  * 
  *     raise TypeError("expected binary or text (found %s)" % type(s))
  */
-  __pyx_tuple_ = PyTuple_Pack(2, __pyx_kp_u_utf_8, __pyx_n_u_strict); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 8, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(2, __pyx_kp_u_utf_8, __pyx_n_u_strict); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "bencode2/_compat.pyx":3
- * # cython: language_level=3
+  /* "bencode2/_compat.pyx":6
+ * from cpython.string cimport PyString_Check
  * 
  * def to_binary(s):             # <<<<<<<<<<<<<<
- *     if isinstance(s, bytes):
+ *     if PyBytes_Check(s):
  *         return s
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_s); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_s); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__compat_pyx, __pyx_n_s_to_binary, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__compat_pyx, __pyx_n_s_to_binary, 6, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -2601,18 +2676,38 @@
   /*--- Type init code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_import_code(void) {
   __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
+  __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
+  #elif CYTHON_COMPILING_IN_LIMITED_API
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
+  #else
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
+  #endif
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_RefNannyFinishContext();
+  return -1;
 }
 
 static int __Pyx_modinit_variable_import_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
   __Pyx_RefNannyFinishContext();
@@ -2893,38 +2988,38 @@
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   (void)__Pyx_modinit_type_init_code();
-  (void)__Pyx_modinit_type_import_code();
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "bencode2/_compat.pyx":3
- * # cython: language_level=3
+  /* "bencode2/_compat.pyx":6
+ * from cpython.string cimport PyString_Check
  * 
  * def to_binary(s):             # <<<<<<<<<<<<<<
- *     if isinstance(s, bytes):
+ *     if PyBytes_Check(s):
  *         return s
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7_compat_1to_binary, 0, __pyx_n_s_to_binary, NULL, __pyx_n_s_bencode2__compat, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7_compat_1to_binary, 0, __pyx_n_s_to_binary, NULL, __pyx_n_s_bencode2__compat, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_binary, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_binary, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "bencode2/_compat.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
- * def to_binary(s):
+ * from cpython.bytes cimport PyBytes_Check
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
@@ -3989,14 +4084,94 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
+/* TypeImport */
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
+{
+    PyObject *result = 0;
+    char warning[200];
+    Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *py_basicsize;
+    PyObject *py_itemsize;
+#endif
+    result = PyObject_GetAttrString(module, class_name);
+    if (!result)
+        goto bad;
+    if (!PyType_Check(result)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s.%.200s is not a type object",
+            module_name, class_name);
+        goto bad;
+    }
+#if !CYTHON_COMPILING_IN_LIMITED_API
+    basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
+#else
+    py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
+    if (!py_basicsize)
+        goto bad;
+    basicsize = PyLong_AsSsize_t(py_basicsize);
+    Py_DECREF(py_basicsize);
+    py_basicsize = 0;
+    if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
+#endif
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
+        PyErr_Format(PyExc_ValueError,
+            "%.200s.%.200s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd from PyObject",
+            module_name, class_name, size, basicsize+itemsize);
+        goto bad;
+    }
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
+            ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
+        PyErr_Format(PyExc_ValueError,
+            "%.200s.%.200s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd-%zd from PyObject",
+            module_name, class_name, size, basicsize, basicsize+itemsize);
+        goto bad;
+    }
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
+        PyOS_snprintf(warning, sizeof(warning),
+            "%s.%s size changed, may indicate binary incompatibility. "
+            "Expected %zd from C header, got %zd from PyObject",
+            module_name, class_name, size, basicsize);
+        if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
+    }
+    return (PyTypeObject *)result;
+bad:
+    Py_XDECREF(result);
+    return NULL;
+}
+#endif
+
 /* FixUpExtensionType */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
 #if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     CYTHON_UNUSED_VAR(spec);
     CYTHON_UNUSED_VAR(type);
 #else
```

### Comparing `bencode2-0.0.1/bencode2/decoder.c` & `bencode2-0.0.4/bencode2/_decoder.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "name": "bencode2.decoder",
+        "name": "bencode2._decoder",
         "sources": [
-            "bencode2\\decoder.pyx"
+            "bencode2/_decoder.pyx"
         ]
     },
-    "module_name": "bencode2.decoder"
+    "module_name": "bencode2._decoder"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
@@ -1224,16 +1224,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__bencode2__decoder
-#define __PYX_HAVE_API__bencode2__decoder
+#define __PYX_HAVE__bencode2___decoder
+#define __PYX_HAVE_API__bencode2___decoder
 /* Early includes */
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -1475,15 +1475,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "bencode2\\\\decoder.pyx",
+  "bencode2/_decoder.pyx",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -2201,22 +2201,22 @@
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 
-/* Module declarations from "bencode2.decoder" */
+/* Module declarations from "bencode2._decoder" */
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "bencode2.decoder"
-extern int __pyx_module_is_main_bencode2__decoder;
-int __pyx_module_is_main_bencode2__decoder = 0;
+#define __Pyx_MODULE_NAME "bencode2._decoder"
+extern int __pyx_module_is_main_bencode2___decoder;
+int __pyx_module_is_main_bencode2___decoder = 0;
 
-/* Implementation of "bencode2.decoder" */
+/* Implementation of "bencode2._decoder" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_IndexError;
 static PyObject *__pyx_builtin_KeyError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_ValueError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "-";
@@ -2273,44 +2273,44 @@
 static const char __pyx_k_set_name[] = "__set_name__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_to_binary[] = "to_binary";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_decode_int[] = "decode_int";
-static const char __pyx_k_exceptions[] = "exceptions";
+static const char __pyx_k_exceptions[] = "_exceptions";
 static const char __pyx_k_decode_dict[] = "decode_dict";
 static const char __pyx_k_decode_func[] = "decode_func";
 static const char __pyx_k_decode_list[] = "decode_list";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_decode_string[] = "decode_string";
 static const char __pyx_k_init_subclass[] = "__init_subclass__";
 static const char __pyx_k_BencodeDecoder[] = "BencodeDecoder";
 static const char __pyx_k_collections_abc[] = "collections.abc";
-static const char __pyx_k_bencode2_decoder[] = "bencode2.decoder";
+static const char __pyx_k_bencode2__decoder[] = "bencode2._decoder";
 static const char __pyx_k_BencodeDecodeError[] = "BencodeDecodeError";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_bencode2_decoder_pyx[] = "bencode2\\decoder.pyx";
 static const char __pyx_k_BencodeDecoder___init[] = "BencodeDecoder.__init__";
 static const char __pyx_k_BencodeDecoder_decode[] = "BencodeDecoder.decode";
+static const char __pyx_k_bencode2__decoder_pyx[] = "bencode2/_decoder.pyx";
 static const char __pyx_k_BencodeDecoder_decode_int[] = "BencodeDecoder.decode_int";
 static const char __pyx_k_BencodeDecoder_decode_dict[] = "BencodeDecoder.decode_dict";
 static const char __pyx_k_BencodeDecoder_decode_list[] = "BencodeDecoder.decode_list";
 static const char __pyx_k_not_a_valid_bencoded_string[] = "not a valid bencoded string";
 static const char __pyx_k_BencodeDecoder_decode_string[] = "BencodeDecoder.decode_string";
 static const char __pyx_k_invalid_bencoded_value_data_afte[] = "invalid bencoded value (data after valid prefix)";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_2decode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_4decode_int(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_6decode_string(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_8decode_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_10decode_dict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_2decode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_4decode_int(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_6decode_string(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_8decode_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_10decode_dict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
   PyObject *__pyx_empty_tuple;
@@ -2361,16 +2361,16 @@
   PyObject *__pyx_n_s_KeyError;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s__16;
   PyObject *__pyx_kp_b__2;
   PyObject *__pyx_kp_u__3;
   PyObject *__pyx_n_s_asyncio_coroutines;
-  PyObject *__pyx_n_s_bencode2_decoder;
-  PyObject *__pyx_kp_s_bencode2_decoder_pyx;
+  PyObject *__pyx_n_s_bencode2__decoder;
+  PyObject *__pyx_kp_s_bencode2__decoder_pyx;
   PyObject *__pyx_n_s_bytes;
   PyObject *__pyx_n_s_class_getitem;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_collections_abc;
   PyObject *__pyx_n_s_colon;
   PyObject *__pyx_n_s_compat;
   PyObject *__pyx_n_b_d;
@@ -2499,16 +2499,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_KeyError);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s__16);
   Py_CLEAR(clear_module_state->__pyx_kp_b__2);
   Py_CLEAR(clear_module_state->__pyx_kp_u__3);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
-  Py_CLEAR(clear_module_state->__pyx_n_s_bencode2_decoder);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_bencode2_decoder_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bencode2__decoder);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_bencode2__decoder_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_collections_abc);
   Py_CLEAR(clear_module_state->__pyx_n_s_colon);
   Py_CLEAR(clear_module_state->__pyx_n_s_compat);
   Py_CLEAR(clear_module_state->__pyx_n_b_d);
@@ -2615,16 +2615,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_KeyError);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s__16);
   Py_VISIT(traverse_module_state->__pyx_kp_b__2);
   Py_VISIT(traverse_module_state->__pyx_kp_u__3);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
-  Py_VISIT(traverse_module_state->__pyx_n_s_bencode2_decoder);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_bencode2_decoder_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bencode2__decoder);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_bencode2__decoder_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_collections_abc);
   Py_VISIT(traverse_module_state->__pyx_n_s_colon);
   Py_VISIT(traverse_module_state->__pyx_n_s_compat);
   Py_VISIT(traverse_module_state->__pyx_n_b_d);
@@ -2741,16 +2741,16 @@
 #define __pyx_n_s_KeyError __pyx_mstate_global->__pyx_n_s_KeyError
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s__16 __pyx_mstate_global->__pyx_n_s__16
 #define __pyx_kp_b__2 __pyx_mstate_global->__pyx_kp_b__2
 #define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
-#define __pyx_n_s_bencode2_decoder __pyx_mstate_global->__pyx_n_s_bencode2_decoder
-#define __pyx_kp_s_bencode2_decoder_pyx __pyx_mstate_global->__pyx_kp_s_bencode2_decoder_pyx
+#define __pyx_n_s_bencode2__decoder __pyx_mstate_global->__pyx_n_s_bencode2__decoder
+#define __pyx_kp_s_bencode2__decoder_pyx __pyx_mstate_global->__pyx_kp_s_bencode2__decoder_pyx
 #define __pyx_n_s_bytes __pyx_mstate_global->__pyx_n_s_bytes
 #define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_collections_abc __pyx_mstate_global->__pyx_n_s_collections_abc
 #define __pyx_n_s_colon __pyx_mstate_global->__pyx_n_s_colon
 #define __pyx_n_s_compat __pyx_mstate_global->__pyx_n_s_compat
 #define __pyx_n_b_d __pyx_mstate_global->__pyx_n_b_d
@@ -2810,32 +2810,32 @@
 #define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 #define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
 /* #### Code section: module_code ### */
 
-/* "bencode2/decoder.pyx":11
+/* "bencode2/_decoder.pyx":11
  * 
  * class BencodeDecoder:
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
  *             b"l": self.decode_list,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_1__init__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_1__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8bencode2_7decoder_14BencodeDecoder_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_7decoder_14BencodeDecoder_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_1__init__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_1__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -2897,250 +2897,250 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8bencode2_7decoder_14BencodeDecoder___init__(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder___init__(__pyx_self, __pyx_v_self);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "bencode2/decoder.pyx":13
+  /* "bencode2/_decoder.pyx":13
  *     def __init__(self):
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
  *             b"l": self.decode_list,             # <<<<<<<<<<<<<<
  *             b"i": self.decode_int,
  *             b"0": self.decode_string,
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_b_l, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":14
+  /* "bencode2/_decoder.pyx":14
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
  *             b"l": self.decode_list,
  *             b"i": self.decode_int,             # <<<<<<<<<<<<<<
  *             b"0": self.decode_string,
  *             b"1": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_int); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_b_i, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":15
+  /* "bencode2/_decoder.pyx":15
  *             b"l": self.decode_list,
  *             b"i": self.decode_int,
  *             b"0": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"1": self.decode_string,
  *             b"2": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_0, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":16
+  /* "bencode2/_decoder.pyx":16
  *             b"i": self.decode_int,
  *             b"0": self.decode_string,
  *             b"1": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"2": self.decode_string,
  *             b"3": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_1, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":17
+  /* "bencode2/_decoder.pyx":17
  *             b"0": self.decode_string,
  *             b"1": self.decode_string,
  *             b"2": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"3": self.decode_string,
  *             b"4": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_2, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":18
+  /* "bencode2/_decoder.pyx":18
  *             b"1": self.decode_string,
  *             b"2": self.decode_string,
  *             b"3": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"4": self.decode_string,
  *             b"5": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_3, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":19
+  /* "bencode2/_decoder.pyx":19
  *             b"2": self.decode_string,
  *             b"3": self.decode_string,
  *             b"4": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"5": self.decode_string,
  *             b"6": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_4, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":20
+  /* "bencode2/_decoder.pyx":20
  *             b"3": self.decode_string,
  *             b"4": self.decode_string,
  *             b"5": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"6": self.decode_string,
  *             b"7": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_5, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":21
+  /* "bencode2/_decoder.pyx":21
  *             b"4": self.decode_string,
  *             b"5": self.decode_string,
  *             b"6": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"7": self.decode_string,
  *             b"8": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_6, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":22
+  /* "bencode2/_decoder.pyx":22
  *             b"5": self.decode_string,
  *             b"6": self.decode_string,
  *             b"7": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"8": self.decode_string,
  *             b"9": self.decode_string,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_7, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":23
+  /* "bencode2/_decoder.pyx":23
  *             b"6": self.decode_string,
  *             b"7": self.decode_string,
  *             b"8": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"9": self.decode_string,
  *             b"d": self.decode_dict,
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_8, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":24
+  /* "bencode2/_decoder.pyx":24
  *             b"7": self.decode_string,
  *             b"8": self.decode_string,
  *             b"9": self.decode_string,             # <<<<<<<<<<<<<<
  *             b"d": self.decode_dict,
  *         }
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_9, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":25
+  /* "bencode2/_decoder.pyx":25
  *             b"8": self.decode_string,
  *             b"9": self.decode_string,
  *             b"d": self.decode_dict,             # <<<<<<<<<<<<<<
  *         }
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_1, __pyx_n_b_d, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":12
+  /* "bencode2/_decoder.pyx":12
  * class BencodeDecoder:
  *     def __init__(self):
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {             # <<<<<<<<<<<<<<
  *             b"l": self.decode_list,
  *             b"i": self.decode_int,
  */
   if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_decode_func, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bencode2/decoder.pyx":11
+  /* "bencode2/_decoder.pyx":11
  * 
  * class BencodeDecoder:
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
  *             b"l": self.decode_list,
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/decoder.pyx":28
+/* "bencode2/_decoder.pyx":28
  *         }
  * 
  *     def decode(self, value: bytes) -> Any:             # <<<<<<<<<<<<<<
  *         """
  *         Decode bencode formatted byte string ``value``.
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_3decode(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_3decode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8bencode2_7decoder_14BencodeDecoder_2decode, "\n        Decode bencode formatted byte string ``value``.\n\n        :param value: Bencode formatted string\n        :type value: bytes\n\n        :return: Decoded value\n        :rtype: object\n        ");
-static PyMethodDef __pyx_mdef_8bencode2_7decoder_14BencodeDecoder_3decode = {"decode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_7decoder_14BencodeDecoder_3decode, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_7decoder_14BencodeDecoder_2decode};
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_3decode(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_8bencode2_8_decoder_14BencodeDecoder_2decode, "\n        Decode bencode formatted byte string ``value``.\n\n        :param value: Bencode formatted string\n        :type value: bytes\n\n        :return: Decoded value\n        :rtype: object\n        ");
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_3decode = {"decode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_3decode, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_8_decoder_14BencodeDecoder_2decode};
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_3decode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -3217,20 +3217,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_value), (&PyBytes_Type), 0, "value", 1))) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_7decoder_14BencodeDecoder_2decode(__pyx_self, __pyx_v_self, __pyx_v_value);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_2decode(__pyx_self, __pyx_v_self, __pyx_v_value);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -3239,15 +3239,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_2decode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_2decode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_v_length = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -3263,15 +3263,15 @@
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode", 0);
   __Pyx_INCREF(__pyx_v_value);
 
-  /* "bencode2/decoder.pyx":38
+  /* "bencode2/_decoder.pyx":38
  *         :rtype: object
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             value = to_binary(value)
  *             data, length = self.decode_func[value[0:1]](value, 0)
  */
   {
@@ -3279,15 +3279,15 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "bencode2/decoder.pyx":39
+      /* "bencode2/_decoder.pyx":39
  *         """
  *         try:
  *             value = to_binary(value)             # <<<<<<<<<<<<<<
  *             data, length = self.decode_func[value[0:1]](value, 0)
  *         except (IndexError, KeyError, TypeError, ValueError):
  */
       __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_to_binary); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L3_error)
@@ -3314,15 +3314,15 @@
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
       if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_4))) __PYX_ERR(0, 39, __pyx_L3_error)
       __Pyx_DECREF_SET(__pyx_v_value, ((PyObject*)__pyx_t_4));
       __pyx_t_4 = 0;
 
-      /* "bencode2/decoder.pyx":40
+      /* "bencode2/_decoder.pyx":40
  *         try:
  *             value = to_binary(value)
  *             data, length = self.decode_func[value[0:1]](value, 0)             # <<<<<<<<<<<<<<
  *         except (IndexError, KeyError, TypeError, ValueError):
  *             raise BencodeDecodeError("not a valid bencoded string")
  */
       __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_func); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L3_error)
@@ -3406,15 +3406,15 @@
         __pyx_L10_unpacking_done:;
       }
       __pyx_v_data = __pyx_t_8;
       __pyx_t_8 = 0;
       __pyx_v_length = __pyx_t_6;
       __pyx_t_6 = 0;
 
-      /* "bencode2/decoder.pyx":38
+      /* "bencode2/_decoder.pyx":38
  *         :rtype: object
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             value = to_binary(value)
  *             data, length = self.decode_func[value[0:1]](value, 0)
  */
     }
@@ -3424,30 +3424,30 @@
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "bencode2/decoder.pyx":41
+    /* "bencode2/_decoder.pyx":41
  *             value = to_binary(value)
  *             data, length = self.decode_func[value[0:1]](value, 0)
  *         except (IndexError, KeyError, TypeError, ValueError):             # <<<<<<<<<<<<<<
  *             raise BencodeDecodeError("not a valid bencoded string")
  * 
  */
     __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
     if (__pyx_t_7) {
-      __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_8) < 0) __PYX_ERR(0, 41, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_8);
 
-      /* "bencode2/decoder.pyx":42
+      /* "bencode2/_decoder.pyx":42
  *             data, length = self.decode_func[value[0:1]](value, 0)
  *         except (IndexError, KeyError, TypeError, ValueError):
  *             raise BencodeDecodeError("not a valid bencoded string")             # <<<<<<<<<<<<<<
  * 
  *         if length != len(value):
  */
       __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 42, __pyx_L5_except_error)
@@ -3476,15 +3476,15 @@
       }
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(0, 42, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "bencode2/decoder.pyx":38
+    /* "bencode2/_decoder.pyx":38
  *         :rtype: object
  *         """
  *         try:             # <<<<<<<<<<<<<<
  *             value = to_binary(value)
  *             data, length = self.decode_func[value[0:1]](value, 0)
  */
     __pyx_L5_except_error:;
@@ -3492,15 +3492,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "bencode2/decoder.pyx":44
+  /* "bencode2/_decoder.pyx":44
  *             raise BencodeDecodeError("not a valid bencoded string")
  * 
  *         if length != len(value):             # <<<<<<<<<<<<<<
  *             raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")
  * 
  */
   if (unlikely(__pyx_v_value == Py_None)) {
@@ -3512,15 +3512,15 @@
   __Pyx_GOTREF(__pyx_t_8);
   __pyx_t_6 = PyObject_RichCompare(__pyx_v_length, __pyx_t_8, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_13 < 0))) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (unlikely(__pyx_t_13)) {
 
-    /* "bencode2/decoder.pyx":45
+    /* "bencode2/_decoder.pyx":45
  * 
  *         if length != len(value):
  *             raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")             # <<<<<<<<<<<<<<
  * 
  *         return data
  */
     __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 45, __pyx_L1_error)
@@ -3547,36 +3547,36 @@
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __PYX_ERR(0, 45, __pyx_L1_error)
 
-    /* "bencode2/decoder.pyx":44
+    /* "bencode2/_decoder.pyx":44
  *             raise BencodeDecodeError("not a valid bencoded string")
  * 
  *         if length != len(value):             # <<<<<<<<<<<<<<
  *             raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")
  * 
  */
   }
 
-  /* "bencode2/decoder.pyx":47
+  /* "bencode2/_decoder.pyx":47
  *             raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")
  * 
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def decode_int(self, x, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "bencode2/decoder.pyx":28
+  /* "bencode2/_decoder.pyx":28
  *         }
  * 
  *     def decode(self, value: bytes) -> Any:             # <<<<<<<<<<<<<<
  *         """
  *         Decode bencode formatted byte string ``value``.
  */
 
@@ -3584,43 +3584,43 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/decoder.pyx":49
+/* "bencode2/_decoder.pyx":49
  *         return data
  * 
  *     def decode_int(self, x, index: int):             # <<<<<<<<<<<<<<
  *         index += 1
  *         new_f = x.index(b"e", index)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_5decode_int(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_5decode_int(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8bencode2_7decoder_14BencodeDecoder_5decode_int = {"decode_int", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_7decoder_14BencodeDecoder_5decode_int, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_5decode_int(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_5decode_int = {"decode_int", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_5decode_int, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_5decode_int(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
@@ -3712,20 +3712,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_index), (&PyInt_Type), 0, "index", 1))) __PYX_ERR(0, 49, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_7decoder_14BencodeDecoder_4decode_int(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_4decode_int(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -3734,15 +3734,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_4decode_int(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_4decode_int(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
   PyObject *__pyx_v_new_f = NULL;
   PyObject *__pyx_v_n = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -3751,28 +3751,28 @@
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_int", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "bencode2/decoder.pyx":50
+  /* "bencode2/_decoder.pyx":50
  * 
  *     def decode_int(self, x, index: int):
  *         index += 1             # <<<<<<<<<<<<<<
  *         new_f = x.index(b"e", index)
  *         n = int(x[index:new_f])
  */
   __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "bencode2/decoder.pyx":51
+  /* "bencode2/_decoder.pyx":51
  *     def decode_int(self, x, index: int):
  *         index += 1
  *         new_f = x.index(b"e", index)             # <<<<<<<<<<<<<<
  *         n = int(x[index:new_f])
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
@@ -3798,30 +3798,30 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_new_f = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "bencode2/decoder.pyx":52
+  /* "bencode2/_decoder.pyx":52
  *         index += 1
  *         new_f = x.index(b"e", index)
  *         n = int(x[index:new_f])             # <<<<<<<<<<<<<<
  * 
  *         if x[index : index + 1] == b"-":
  */
   __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_v_new_f, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_n = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":54
+  /* "bencode2/_decoder.pyx":54
  *         n = int(x[index:new_f])
  * 
  *         if x[index : index + 1] == b"-":             # <<<<<<<<<<<<<<
  *             if x[index + 1 : index + 2] == b"0":
  *                 raise ValueError
  */
   __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
@@ -3829,15 +3829,15 @@
   __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_5 = (__Pyx_PyBytes_Equals(__pyx_t_1, __pyx_kp_b_, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_5) {
 
-    /* "bencode2/decoder.pyx":55
+    /* "bencode2/_decoder.pyx":55
  * 
  *         if x[index : index + 1] == b"-":
  *             if x[index + 1 : index + 2] == b"0":             # <<<<<<<<<<<<<<
  *                 raise ValueError
  *         elif x[index : index + 1] == b"0" and new_f != index + 1:
  */
     __pyx_t_1 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
@@ -3848,44 +3848,44 @@
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_5 = (__Pyx_PyBytes_Equals(__pyx_t_3, __pyx_kp_b_0, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 55, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(__pyx_t_5)) {
 
-      /* "bencode2/decoder.pyx":56
+      /* "bencode2/_decoder.pyx":56
  *         if x[index : index + 1] == b"-":
  *             if x[index + 1 : index + 2] == b"0":
  *                 raise ValueError             # <<<<<<<<<<<<<<
  *         elif x[index : index + 1] == b"0" and new_f != index + 1:
  *             raise ValueError
  */
       __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
       __PYX_ERR(0, 56, __pyx_L1_error)
 
-      /* "bencode2/decoder.pyx":55
+      /* "bencode2/_decoder.pyx":55
  * 
  *         if x[index : index + 1] == b"-":
  *             if x[index + 1 : index + 2] == b"0":             # <<<<<<<<<<<<<<
  *                 raise ValueError
  *         elif x[index : index + 1] == b"0" and new_f != index + 1:
  */
     }
 
-    /* "bencode2/decoder.pyx":54
+    /* "bencode2/_decoder.pyx":54
  *         n = int(x[index:new_f])
  * 
  *         if x[index : index + 1] == b"-":             # <<<<<<<<<<<<<<
  *             if x[index + 1 : index + 2] == b"0":
  *                 raise ValueError
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/decoder.pyx":57
+  /* "bencode2/_decoder.pyx":57
  *             if x[index + 1 : index + 2] == b"0":
  *                 raise ValueError
  *         elif x[index : index + 1] == b"0" and new_f != index + 1:             # <<<<<<<<<<<<<<
  *             raise ValueError
  * 
  */
   __pyx_t_3 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
@@ -3906,35 +3906,35 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = __pyx_t_6;
   __pyx_L5_bool_binop_done:;
   if (unlikely(__pyx_t_5)) {
 
-    /* "bencode2/decoder.pyx":58
+    /* "bencode2/_decoder.pyx":58
  *                 raise ValueError
  *         elif x[index : index + 1] == b"0" and new_f != index + 1:
  *             raise ValueError             # <<<<<<<<<<<<<<
  * 
  *         return n, new_f + 1
  */
     __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
     __PYX_ERR(0, 58, __pyx_L1_error)
 
-    /* "bencode2/decoder.pyx":57
+    /* "bencode2/_decoder.pyx":57
  *             if x[index + 1 : index + 2] == b"0":
  *                 raise ValueError
  *         elif x[index : index + 1] == b"0" and new_f != index + 1:             # <<<<<<<<<<<<<<
  *             raise ValueError
  * 
  */
   }
   __pyx_L3:;
 
-  /* "bencode2/decoder.pyx":60
+  /* "bencode2/_decoder.pyx":60
  *             raise ValueError
  * 
  *         return n, new_f + 1             # <<<<<<<<<<<<<<
  * 
  *     def decode_string(self, x, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -3948,57 +3948,57 @@
   __Pyx_GIVEREF(__pyx_t_3);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/decoder.pyx":49
+  /* "bencode2/_decoder.pyx":49
  *         return data
  * 
  *     def decode_int(self, x, index: int):             # <<<<<<<<<<<<<<
  *         index += 1
  *         new_f = x.index(b"e", index)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_new_f);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/decoder.pyx":62
+/* "bencode2/_decoder.pyx":62
  *         return n, new_f + 1
  * 
  *     def decode_string(self, x, index: int):             # <<<<<<<<<<<<<<
  *         """Decode torrent bencoded 'string' in x starting at f."""
  *         colon = x.index(b":", index)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_7decode_string(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_7decode_string(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8bencode2_7decoder_14BencodeDecoder_6decode_string, "Decode torrent bencoded 'string' in x starting at f.");
-static PyMethodDef __pyx_mdef_8bencode2_7decoder_14BencodeDecoder_7decode_string = {"decode_string", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_7decoder_14BencodeDecoder_7decode_string, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_7decoder_14BencodeDecoder_6decode_string};
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_7decode_string(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_8bencode2_8_decoder_14BencodeDecoder_6decode_string, "Decode torrent bencoded 'string' in x starting at f.");
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_7decode_string = {"decode_string", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_7decode_string, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_8_decoder_14BencodeDecoder_6decode_string};
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_7decode_string(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v_self = 0;
@@ -4090,20 +4090,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_index), (&PyInt_Type), 0, "index", 1))) __PYX_ERR(0, 62, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_7decoder_14BencodeDecoder_6decode_string(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_6decode_string(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -4112,15 +4112,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_6decode_string(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_6decode_string(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
   PyObject *__pyx_v_colon = NULL;
   PyObject *__pyx_v_n = NULL;
   PyObject *__pyx_v_s = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -4129,15 +4129,15 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_string", 1);
 
-  /* "bencode2/decoder.pyx":64
+  /* "bencode2/_decoder.pyx":64
  *     def decode_string(self, x, index: int):
  *         """Decode torrent bencoded 'string' in x starting at f."""
  *         colon = x.index(b":", index)             # <<<<<<<<<<<<<<
  *         n = int(x[index:colon])
  * 
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
@@ -4163,30 +4163,30 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_colon = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "bencode2/decoder.pyx":65
+  /* "bencode2/_decoder.pyx":65
  *         """Decode torrent bencoded 'string' in x starting at f."""
  *         colon = x.index(b":", index)
  *         n = int(x[index:colon])             # <<<<<<<<<<<<<<
  * 
  *         if x[index : index + 1] == b"0" and colon != index + 1:
  */
   __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_v_colon, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_n = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":67
+  /* "bencode2/_decoder.pyx":67
  *         n = int(x[index:colon])
  * 
  *         if x[index : index + 1] == b"0" and colon != index + 1:             # <<<<<<<<<<<<<<
  *             raise ValueError
  * 
  */
   __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
@@ -4207,61 +4207,61 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_5 = __pyx_t_6;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_5)) {
 
-    /* "bencode2/decoder.pyx":68
+    /* "bencode2/_decoder.pyx":68
  * 
  *         if x[index : index + 1] == b"0" and colon != index + 1:
  *             raise ValueError             # <<<<<<<<<<<<<<
  * 
  *         colon += 1
  */
     __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
     __PYX_ERR(0, 68, __pyx_L1_error)
 
-    /* "bencode2/decoder.pyx":67
+    /* "bencode2/_decoder.pyx":67
  *         n = int(x[index:colon])
  * 
  *         if x[index : index + 1] == b"0" and colon != index + 1:             # <<<<<<<<<<<<<<
  *             raise ValueError
  * 
  */
   }
 
-  /* "bencode2/decoder.pyx":70
+  /* "bencode2/_decoder.pyx":70
  *             raise ValueError
  * 
  *         colon += 1             # <<<<<<<<<<<<<<
  *         s = x[colon : colon + n]
  * 
  */
   __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_colon, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF_SET(__pyx_v_colon, __pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":71
+  /* "bencode2/_decoder.pyx":71
  * 
  *         colon += 1
  *         s = x[colon : colon + n]             # <<<<<<<<<<<<<<
  * 
  *         return bytes(s), colon + n
  */
   __pyx_t_2 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_colon, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_s = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "bencode2/decoder.pyx":73
+  /* "bencode2/_decoder.pyx":73
  *         s = x[colon : colon + n]
  * 
  *         return bytes(s), colon + n             # <<<<<<<<<<<<<<
  * 
  *     def decode_list(self, x, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -4277,56 +4277,56 @@
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/decoder.pyx":62
+  /* "bencode2/_decoder.pyx":62
  *         return n, new_f + 1
  * 
  *     def decode_string(self, x, index: int):             # <<<<<<<<<<<<<<
  *         """Decode torrent bencoded 'string' in x starting at f."""
  *         colon = x.index(b":", index)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_colon);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/decoder.pyx":75
+/* "bencode2/_decoder.pyx":75
  *         return bytes(s), colon + n
  * 
  *     def decode_list(self, x, index: int):             # <<<<<<<<<<<<<<
  *         r, index = [], index + 1
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_9decode_list(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_9decode_list(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8bencode2_7decoder_14BencodeDecoder_9decode_list = {"decode_list", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_7decoder_14BencodeDecoder_9decode_list, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_9decode_list(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_9decode_list = {"decode_list", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_9decode_list, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_9decode_list(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -4418,20 +4418,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_index), (&PyInt_Type), 0, "index", 1))) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_7decoder_14BencodeDecoder_8decode_list(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_8decode_list(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -4440,15 +4440,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_8decode_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_8decode_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
   PyObject *__pyx_v_r = NULL;
   PyObject *__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
@@ -4459,15 +4459,15 @@
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_list", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "bencode2/decoder.pyx":76
+  /* "bencode2/_decoder.pyx":76
  * 
  *     def decode_list(self, x, index: int):
  *         r, index = [], index + 1             # <<<<<<<<<<<<<<
  * 
  *         while x[index : index + 1] != b"e":
  */
   __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
@@ -4476,15 +4476,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 76, __pyx_L1_error)
   __pyx_v_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_2));
   __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":78
+  /* "bencode2/_decoder.pyx":78
  *         r, index = [], index + 1
  * 
  *         while x[index : index + 1] != b"e":             # <<<<<<<<<<<<<<
  *             v, index = self.decode_func[x[index : index + 1]](x, index)
  *             r.append(v)
  */
   while (1) {
@@ -4493,15 +4493,15 @@
     __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_3 = (__Pyx_PyBytes_Equals(__pyx_t_1, __pyx_n_b_e, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 78, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (!__pyx_t_3) break;
 
-    /* "bencode2/decoder.pyx":79
+    /* "bencode2/_decoder.pyx":79
  * 
  *         while x[index : index + 1] != b"e":
  *             v, index = self.decode_func[x[index : index + 1]](x, index)             # <<<<<<<<<<<<<<
  *             r.append(v)
  * 
  */
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_func); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
@@ -4585,25 +4585,25 @@
     }
     if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_5))) __PYX_ERR(0, 79, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "bencode2/decoder.pyx":80
+    /* "bencode2/_decoder.pyx":80
  *         while x[index : index + 1] != b"e":
  *             v, index = self.decode_func[x[index : index + 1]](x, index)
  *             r.append(v)             # <<<<<<<<<<<<<<
  * 
  *         return r, index + 1
  */
     __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_r, __pyx_v_v); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 80, __pyx_L1_error)
   }
 
-  /* "bencode2/decoder.pyx":82
+  /* "bencode2/_decoder.pyx":82
  *             r.append(v)
  * 
  *         return r, index + 1             # <<<<<<<<<<<<<<
  * 
  *     def decode_dict(self, x, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
@@ -4617,58 +4617,58 @@
   __Pyx_GIVEREF(__pyx_t_1);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/decoder.pyx":75
+  /* "bencode2/_decoder.pyx":75
  *         return bytes(s), colon + n
  * 
  *     def decode_list(self, x, index: int):             # <<<<<<<<<<<<<<
  *         r, index = [], index + 1
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_r);
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/decoder.pyx":84
+/* "bencode2/_decoder.pyx":84
  *         return r, index + 1
  * 
  *     def decode_dict(self, x, index: int):             # <<<<<<<<<<<<<<
  *         """Decode bencoded dictionary."""
  *         index += 1
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_11decode_dict(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_11decode_dict(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8bencode2_7decoder_14BencodeDecoder_10decode_dict, "Decode bencoded dictionary.");
-static PyMethodDef __pyx_mdef_8bencode2_7decoder_14BencodeDecoder_11decode_dict = {"decode_dict", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_7decoder_14BencodeDecoder_11decode_dict, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_7decoder_14BencodeDecoder_10decode_dict};
-static PyObject *__pyx_pw_8bencode2_7decoder_14BencodeDecoder_11decode_dict(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_8bencode2_8_decoder_14BencodeDecoder_10decode_dict, "Decode bencoded dictionary.");
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_11decode_dict = {"decode_dict", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_11decode_dict, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_8_decoder_14BencodeDecoder_10decode_dict};
+static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_11decode_dict(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -4760,20 +4760,20 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_index), (&PyInt_Type), 0, "index", 1))) __PYX_ERR(0, 84, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_7decoder_14BencodeDecoder_10decode_dict(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_10decode_dict(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -4782,15 +4782,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_7decoder_14BencodeDecoder_10decode_dict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_10decode_dict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
   PyObject *__pyx_v_r = NULL;
   PyObject *__pyx_v_k = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
@@ -4800,40 +4800,40 @@
   PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("decode_dict", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "bencode2/decoder.pyx":86
+  /* "bencode2/_decoder.pyx":86
  *     def decode_dict(self, x, index: int):
  *         """Decode bencoded dictionary."""
  *         index += 1             # <<<<<<<<<<<<<<
  * 
  *         r = {}
  */
   __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "bencode2/decoder.pyx":88
+  /* "bencode2/_decoder.pyx":88
  *         index += 1
  * 
  *         r = {}             # <<<<<<<<<<<<<<
  * 
  *         while x[index : index + 1] != b"e":
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bencode2/decoder.pyx":90
+  /* "bencode2/_decoder.pyx":90
  *         r = {}
  * 
  *         while x[index : index + 1] != b"e":             # <<<<<<<<<<<<<<
  *             k, index = self.decode_string(x, index)
  *             r[k], index = self.decode_func[x[index : index + 1]](x, index)
  */
   while (1) {
@@ -4842,15 +4842,15 @@
     __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_1, NULL, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_3 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_n_b_e, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (!__pyx_t_3) break;
 
-    /* "bencode2/decoder.pyx":91
+    /* "bencode2/_decoder.pyx":91
  * 
  *         while x[index : index + 1] != b"e":
  *             k, index = self.decode_string(x, index)             # <<<<<<<<<<<<<<
  *             r[k], index = self.decode_func[x[index : index + 1]](x, index)
  * 
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
@@ -4925,15 +4925,15 @@
     }
     if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_4))) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_1);
     __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_4));
     __pyx_t_4 = 0;
 
-    /* "bencode2/decoder.pyx":92
+    /* "bencode2/_decoder.pyx":92
  *         while x[index : index + 1] != b"e":
  *             k, index = self.decode_string(x, index)
  *             r[k], index = self.decode_func[x[index : index + 1]](x, index)             # <<<<<<<<<<<<<<
  * 
  *         return r, index + 1
  */
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_func); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
@@ -5018,15 +5018,15 @@
     if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_6))) __PYX_ERR(0, 92, __pyx_L1_error)
     if (unlikely((PyDict_SetItem(__pyx_v_r, __pyx_v_k, __pyx_t_1) < 0))) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_6));
     __pyx_t_6 = 0;
   }
 
-  /* "bencode2/decoder.pyx":94
+  /* "bencode2/_decoder.pyx":94
  *             r[k], index = self.decode_func[x[index : index + 1]](x, index)
  * 
  *         return r, index + 1             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -5038,29 +5038,29 @@
   __Pyx_GIVEREF(__pyx_t_2);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/decoder.pyx":84
+  /* "bencode2/_decoder.pyx":84
  *         return r, index + 1
  * 
  *     def decode_dict(self, x, index: int):             # <<<<<<<<<<<<<<
  *         """Decode bencoded dictionary."""
  *         index += 1
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("bencode2.decoder.BencodeDecoder.decode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_r);
   __Pyx_XDECREF(__pyx_v_k);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -5108,16 +5108,16 @@
     {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s__16, __pyx_k__16, sizeof(__pyx_k__16), 0, 0, 1, 1},
     {&__pyx_kp_b__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 0, 0},
     {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
-    {&__pyx_n_s_bencode2_decoder, __pyx_k_bencode2_decoder, sizeof(__pyx_k_bencode2_decoder), 0, 0, 1, 1},
-    {&__pyx_kp_s_bencode2_decoder_pyx, __pyx_k_bencode2_decoder_pyx, sizeof(__pyx_k_bencode2_decoder_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_bencode2__decoder, __pyx_k_bencode2__decoder, sizeof(__pyx_k_bencode2__decoder), 0, 0, 1, 1},
+    {&__pyx_kp_s_bencode2__decoder_pyx, __pyx_k_bencode2__decoder_pyx, sizeof(__pyx_k_bencode2__decoder_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
     {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_collections_abc, __pyx_k_collections_abc, sizeof(__pyx_k_collections_abc), 0, 0, 1, 1},
     {&__pyx_n_s_colon, __pyx_k_colon, sizeof(__pyx_k_colon), 0, 0, 1, 1},
     {&__pyx_n_s_compat, __pyx_k_compat, sizeof(__pyx_k_compat), 0, 0, 1, 1},
     {&__pyx_n_b_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 0, 0, 1},
@@ -5180,85 +5180,85 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "bencode2/decoder.pyx":11
+  /* "bencode2/_decoder.pyx":11
  * 
  * class BencodeDecoder:
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
  *             b"l": self.decode_list,
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2_decoder_pyx, __pyx_n_s_init, 11, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_init, 11, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 11, __pyx_L1_error)
 
-  /* "bencode2/decoder.pyx":28
+  /* "bencode2/_decoder.pyx":28
  *         }
  * 
  *     def decode(self, value: bytes) -> Any:             # <<<<<<<<<<<<<<
  *         """
  *         Decode bencode formatted byte string ``value``.
  */
   __pyx_tuple__6 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_value, __pyx_n_s_data, __pyx_n_s_length); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2_decoder_pyx, __pyx_n_s_decode, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 28, __pyx_L1_error)
 
-  /* "bencode2/decoder.pyx":49
+  /* "bencode2/_decoder.pyx":49
  *         return data
  * 
  *     def decode_int(self, x, index: int):             # <<<<<<<<<<<<<<
  *         index += 1
  *         new_f = x.index(b"e", index)
  */
   __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_index, __pyx_n_s_new_f, __pyx_n_s_n); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2_decoder_pyx, __pyx_n_s_decode_int, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode_int, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 49, __pyx_L1_error)
 
-  /* "bencode2/decoder.pyx":62
+  /* "bencode2/_decoder.pyx":62
  *         return n, new_f + 1
  * 
  *     def decode_string(self, x, index: int):             # <<<<<<<<<<<<<<
  *         """Decode torrent bencoded 'string' in x starting at f."""
  *         colon = x.index(b":", index)
  */
   __pyx_tuple__10 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_index, __pyx_n_s_colon, __pyx_n_s_n, __pyx_n_s_s); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2_decoder_pyx, __pyx_n_s_decode_string, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode_string, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 62, __pyx_L1_error)
 
-  /* "bencode2/decoder.pyx":75
+  /* "bencode2/_decoder.pyx":75
  *         return bytes(s), colon + n
  * 
  *     def decode_list(self, x, index: int):             # <<<<<<<<<<<<<<
  *         r, index = [], index + 1
  * 
  */
   __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_index, __pyx_n_s_r, __pyx_n_s_v); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2_decoder_pyx, __pyx_n_s_decode_list, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode_list, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 75, __pyx_L1_error)
 
-  /* "bencode2/decoder.pyx":84
+  /* "bencode2/_decoder.pyx":84
  *         return r, index + 1
  * 
  *     def decode_dict(self, x, index: int):             # <<<<<<<<<<<<<<
  *         """Decode bencoded dictionary."""
  *         index += 1
  */
   __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_index, __pyx_n_s_r, __pyx_n_s_k); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2_decoder_pyx, __pyx_n_s_decode_dict, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode_dict, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -5343,31 +5343,31 @@
   return 0;
 }
 
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_decoder(PyObject* module); /*proto*/
+static int __pyx_pymod_exec__decoder(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_decoder},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__decoder},
   {0, NULL}
 };
 #endif
 
 #ifdef __cplusplus
 namespace {
   struct PyModuleDef __pyx_moduledef =
   #else
   static struct PyModuleDef __pyx_moduledef =
   #endif
   {
       PyModuleDef_HEAD_INIT,
-      "decoder",
+      "_decoder",
       0, /* m_doc */
     #if CYTHON_PEP489_MULTI_PHASE_INIT
       0, /* m_size */
     #elif CYTHON_USE_MODULE_STATE
       sizeof(__pyx_mstate), /* m_size */
     #else
       -1, /* m_size */
@@ -5407,19 +5407,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initdecoder(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initdecoder(void)
+__Pyx_PyMODINIT_FUNC init_decoder(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC init_decoder(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_decoder(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_decoder(void)
+__Pyx_PyMODINIT_FUNC PyInit__decoder(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit__decoder(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -5492,15 +5492,15 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_decoder(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec__decoder(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   int stringtab_initialized = 0;
   #if CYTHON_USE_MODULE_STATE
   int pystate_addmodule_run = 0;
   #endif
@@ -5511,33 +5511,33 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'decoder' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module '_decoder' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("decoder", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("_decoder", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "decoder" pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "_decoder" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -5553,15 +5553,15 @@
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_decoder(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__decoder(void)", 0);
   if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5591,22 +5591,22 @@
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_bencode2__decoder) {
+  if (__pyx_module_is_main_bencode2___decoder) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "bencode2.decoder")) {
-      if (unlikely((PyDict_SetItemString(modules, "bencode2.decoder", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "bencode2._decoder")) {
+      if (unlikely((PyDict_SetItemString(modules, "bencode2._decoder", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5619,15 +5619,15 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "bencode2/decoder.pyx":3
+  /* "bencode2/_decoder.pyx":3
  * # cython: language_level=3
  * 
  * from collections.abc import Callable             # <<<<<<<<<<<<<<
  * from typing import Any
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
@@ -5640,15 +5640,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Callable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Callable, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/decoder.pyx":4
+  /* "bencode2/_decoder.pyx":4
  * 
  * from collections.abc import Callable
  * from typing import Any             # <<<<<<<<<<<<<<
  * 
  * from ._compat import to_binary
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
@@ -5661,19 +5661,19 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Any); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Any, __pyx_t_3) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":6
+  /* "bencode2/_decoder.pyx":6
  * from typing import Any
  * 
  * from ._compat import to_binary             # <<<<<<<<<<<<<<
- * from .exceptions import BencodeDecodeError
+ * from ._exceptions import BencodeDecodeError
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_to_binary);
   __Pyx_GIVEREF(__pyx_n_s_to_binary);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_to_binary)) __PYX_ERR(0, 6, __pyx_L1_error);
@@ -5682,18 +5682,18 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_to_binary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_binary, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/decoder.pyx":7
+  /* "bencode2/_decoder.pyx":7
  * 
  * from ._compat import to_binary
- * from .exceptions import BencodeDecodeError             # <<<<<<<<<<<<<<
+ * from ._exceptions import BencodeDecodeError             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_BencodeDecodeError);
   __Pyx_GIVEREF(__pyx_n_s_BencodeDecodeError);
@@ -5703,136 +5703,136 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeDecodeError, __pyx_t_3) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":10
+  /* "bencode2/_decoder.pyx":10
  * 
  * 
  * class BencodeDecoder:             # <<<<<<<<<<<<<<
  *     def __init__(self):
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_BencodeDecoder, __pyx_n_s_BencodeDecoder, (PyObject *) NULL, __pyx_n_s_bencode2_decoder, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_BencodeDecoder, __pyx_n_s_BencodeDecoder, (PyObject *) NULL, __pyx_n_s_bencode2__decoder, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "bencode2/decoder.pyx":11
+  /* "bencode2/_decoder.pyx":11
  * 
  * class BencodeDecoder:
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
  *             b"l": self.decode_list,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7decoder_14BencodeDecoder_1__init__, 0, __pyx_n_s_BencodeDecoder___init, NULL, __pyx_n_s_bencode2_decoder, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_1__init__, 0, __pyx_n_s_BencodeDecoder___init, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/decoder.pyx":28
+  /* "bencode2/_decoder.pyx":28
  *         }
  * 
  *     def decode(self, value: bytes) -> Any:             # <<<<<<<<<<<<<<
  *         """
  *         Decode bencode formatted byte string ``value``.
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_value, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_Any) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7decoder_14BencodeDecoder_3decode, 0, __pyx_n_s_BencodeDecoder_decode, NULL, __pyx_n_s_bencode2_decoder, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_3decode, 0, __pyx_n_s_BencodeDecoder_decode, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode, __pyx_t_4) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "bencode2/decoder.pyx":49
+  /* "bencode2/_decoder.pyx":49
  *         return data
  * 
  *     def decode_int(self, x, index: int):             # <<<<<<<<<<<<<<
  *         index += 1
  *         new_f = x.index(b"e", index)
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_index, __pyx_n_s_int) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7decoder_14BencodeDecoder_5decode_int, 0, __pyx_n_s_BencodeDecoder_decode_int, NULL, __pyx_n_s_bencode2_decoder, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_5decode_int, 0, __pyx_n_s_BencodeDecoder_decode_int, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode_int, __pyx_t_3) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/decoder.pyx":62
+  /* "bencode2/_decoder.pyx":62
  *         return n, new_f + 1
  * 
  *     def decode_string(self, x, index: int):             # <<<<<<<<<<<<<<
  *         """Decode torrent bencoded 'string' in x starting at f."""
  *         colon = x.index(b":", index)
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_n_s_int) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7decoder_14BencodeDecoder_7decode_string, 0, __pyx_n_s_BencodeDecoder_decode_string, NULL, __pyx_n_s_bencode2_decoder, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_7decode_string, 0, __pyx_n_s_BencodeDecoder_decode_string, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode_string, __pyx_t_4) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "bencode2/decoder.pyx":75
+  /* "bencode2/_decoder.pyx":75
  *         return bytes(s), colon + n
  * 
  *     def decode_list(self, x, index: int):             # <<<<<<<<<<<<<<
  *         r, index = [], index + 1
  * 
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_index, __pyx_n_s_int) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7decoder_14BencodeDecoder_9decode_list, 0, __pyx_n_s_BencodeDecoder_decode_list, NULL, __pyx_n_s_bencode2_decoder, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_9decode_list, 0, __pyx_n_s_BencodeDecoder_decode_list, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode_list, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/decoder.pyx":84
+  /* "bencode2/_decoder.pyx":84
  *         return r, index + 1
  * 
  *     def decode_dict(self, x, index: int):             # <<<<<<<<<<<<<<
  *         """Decode bencoded dictionary."""
  *         index += 1
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_n_s_int) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7decoder_14BencodeDecoder_11decode_dict, 0, __pyx_n_s_BencodeDecoder_decode_dict, NULL, __pyx_n_s_bencode2_decoder, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_11decode_dict, 0, __pyx_n_s_BencodeDecoder_decode_dict, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode_dict, __pyx_t_4) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "bencode2/decoder.pyx":10
+  /* "bencode2/_decoder.pyx":10
  * 
  * 
  * class BencodeDecoder:             # <<<<<<<<<<<<<<
  *     def __init__(self):
  *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
  */
   __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_BencodeDecoder, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeDecoder, __pyx_t_4) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/decoder.pyx":1
+  /* "bencode2/_decoder.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
  * from collections.abc import Callable
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -5843,29 +5843,29 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init bencode2.decoder", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init bencode2._decoder", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
     Py_DECREF(__pyx_m);
     if (pystate_addmodule_run) {
       PyObject *tp, *value, *tb;
       PyErr_Fetch(&tp, &value, &tb);
       PyState_RemoveModule(&__pyx_moduledef);
       PyErr_Restore(tp, value, tb);
     }
     #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init bencode2.decoder");
+    PyErr_SetString(PyExc_ImportError, "init bencode2._decoder");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `bencode2-0.0.1/bencode2/decoder.pyx` & `bencode2-0.0.4/bencode2/_decoder.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cython: language_level=3
 
 from collections.abc import Callable
 from typing import Any
 
 from ._compat import to_binary
-from .exceptions import BencodeDecodeError
+from ._exceptions import BencodeDecodeError
 
 
 class BencodeDecoder:
     def __init__(self):
         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
             b"l": self.decode_list,
             b"i": self.decode_int,
```

### Comparing `bencode2-0.0.1/bencode2/encoder.c` & `bencode2-0.0.4/bencode2/_encoder.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
-        "name": "bencode2.encoder",
+        "name": "bencode2._encoder",
         "sources": [
-            "bencode2\\encoder.pyx"
+            "bencode2/_encoder.pyx"
         ]
     },
-    "module_name": "bencode2.encoder"
+    "module_name": "bencode2._encoder"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
@@ -1230,16 +1230,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__bencode2__encoder
-#define __PYX_HAVE_API__bencode2__encoder
+#define __PYX_HAVE__bencode2___encoder
+#define __PYX_HAVE_API__bencode2___encoder
 /* Early includes */
 #include <string.h>
 #include <stdio.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
@@ -1483,15 +1483,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "bencode2\\\\encoder.pyx",
+  "bencode2/_encoder.pyx",
   "type.pxd",
   "bool.pxd",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
@@ -2267,30 +2267,30 @@
 
 /* Module declarations from "cpython.pyport" */
 
 /* Module declarations from "cpython.dict" */
 
 /* Module declarations from "cpython.string" */
 
-/* Module declarations from "bencode2.encoder" */
-static PyObject *__pyx_f_8bencode2_7encoder_encode(PyObject *, int __pyx_skip_dispatch); /*proto*/
-static PyObject *__pyx_f_8bencode2_7encoder___encode(PyObject *, PyObject *); /*proto*/
-static PyObject *__pyx_f_8bencode2_7encoder___encode_int(PyObject *, PyObject *); /*proto*/
-static PyObject *__pyx_f_8bencode2_7encoder___encode_bool(PyObject *, PyObject *); /*proto*/
-static PyObject *__pyx_f_8bencode2_7encoder___encode_bytes(PyObject *, PyObject *); /*proto*/
-static PyObject *__pyx_f_8bencode2_7encoder___encode_str(PyObject *, PyObject *); /*proto*/
-static PyObject *__pyx_f_8bencode2_7encoder___encode_list(PyObject *, PyObject *); /*proto*/
-static PyObject *__pyx_f_8bencode2_7encoder___encode_dict(PyObject *, PyObject *); /*proto*/
+/* Module declarations from "bencode2._encoder" */
+static PyObject *__pyx_f_8bencode2_8_encoder_encode(PyObject *, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder___encode(PyObject *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_int(PyObject *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_bool(PyObject *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_bytes(PyObject *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_str(PyObject *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_list(PyObject *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_dict(PyObject *, PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "bencode2.encoder"
-extern int __pyx_module_is_main_bencode2__encoder;
-int __pyx_module_is_main_bencode2__encoder = 0;
+#define __Pyx_MODULE_NAME "bencode2._encoder"
+extern int __pyx_module_is_main_bencode2___encoder;
+int __pyx_module_is_main_bencode2___encoder = 0;
 
-/* Implementation of "bencode2.encoder" */
+/* Implementation of "bencode2._encoder" */
 /* #### Code section: global_var ### */
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "";
 static const char __pyx_k_d[] = "d";
 static const char __pyx_k_e[] = "e";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_l[] = "l";
@@ -2311,26 +2311,26 @@
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_compat[] = "_compat";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_Mapping[] = "Mapping";
 static const char __pyx_k_to_binary[] = "to_binary";
-static const char __pyx_k_exceptions[] = "exceptions";
+static const char __pyx_k_exceptions[] = "_exceptions";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_not_supported[] = "' not supported";
 static const char __pyx_k_collections_abc[] = "collections.abc";
-static const char __pyx_k_bencode2_encoder[] = "bencode2.encoder";
+static const char __pyx_k_bencode2__encoder[] = "bencode2._encoder";
 static const char __pyx_k_BencodeEncodeError[] = "BencodeEncodeError";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_bencode2_encoder_pyx[] = "bencode2\\encoder.pyx";
+static const char __pyx_k_bencode2__encoder_pyx[] = "bencode2/_encoder.pyx";
 static const char __pyx_k_encode_dict_locals_lambda[] = "__encode_dict.<locals>.<lambda>";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_8bencode2_7encoder_encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_encoder_encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_kv); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -2393,16 +2393,16 @@
   PyObject *__pyx_n_s_Any;
   PyObject *__pyx_n_s_BencodeEncodeError;
   PyObject *__pyx_n_s_Mapping;
   PyObject *__pyx_kp_b__2;
   PyObject *__pyx_kp_u__3;
   PyObject *__pyx_n_s__6;
   PyObject *__pyx_n_s_asyncio_coroutines;
-  PyObject *__pyx_n_s_bencode2_encoder;
-  PyObject *__pyx_kp_s_bencode2_encoder_pyx;
+  PyObject *__pyx_n_s_bencode2__encoder;
+  PyObject *__pyx_kp_s_bencode2__encoder_pyx;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_collections_abc;
   PyObject *__pyx_n_s_compat;
   PyObject *__pyx_n_b_d;
   PyObject *__pyx_n_b_e;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_encode_dict_locals_lambda;
@@ -2477,16 +2477,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Any);
   Py_CLEAR(clear_module_state->__pyx_n_s_BencodeEncodeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Mapping);
   Py_CLEAR(clear_module_state->__pyx_kp_b__2);
   Py_CLEAR(clear_module_state->__pyx_kp_u__3);
   Py_CLEAR(clear_module_state->__pyx_n_s__6);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
-  Py_CLEAR(clear_module_state->__pyx_n_s_bencode2_encoder);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_bencode2_encoder_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bencode2__encoder);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_bencode2__encoder_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_collections_abc);
   Py_CLEAR(clear_module_state->__pyx_n_s_compat);
   Py_CLEAR(clear_module_state->__pyx_n_b_d);
   Py_CLEAR(clear_module_state->__pyx_n_b_e);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode_dict_locals_lambda);
@@ -2539,16 +2539,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Any);
   Py_VISIT(traverse_module_state->__pyx_n_s_BencodeEncodeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Mapping);
   Py_VISIT(traverse_module_state->__pyx_kp_b__2);
   Py_VISIT(traverse_module_state->__pyx_kp_u__3);
   Py_VISIT(traverse_module_state->__pyx_n_s__6);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
-  Py_VISIT(traverse_module_state->__pyx_n_s_bencode2_encoder);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_bencode2_encoder_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bencode2__encoder);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_bencode2__encoder_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_collections_abc);
   Py_VISIT(traverse_module_state->__pyx_n_s_compat);
   Py_VISIT(traverse_module_state->__pyx_n_b_d);
   Py_VISIT(traverse_module_state->__pyx_n_b_e);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode_dict_locals_lambda);
@@ -2641,16 +2641,16 @@
 #define __pyx_n_s_Any __pyx_mstate_global->__pyx_n_s_Any
 #define __pyx_n_s_BencodeEncodeError __pyx_mstate_global->__pyx_n_s_BencodeEncodeError
 #define __pyx_n_s_Mapping __pyx_mstate_global->__pyx_n_s_Mapping
 #define __pyx_kp_b__2 __pyx_mstate_global->__pyx_kp_b__2
 #define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
 #define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
-#define __pyx_n_s_bencode2_encoder __pyx_mstate_global->__pyx_n_s_bencode2_encoder
-#define __pyx_kp_s_bencode2_encoder_pyx __pyx_mstate_global->__pyx_kp_s_bencode2_encoder_pyx
+#define __pyx_n_s_bencode2__encoder __pyx_mstate_global->__pyx_n_s_bencode2__encoder
+#define __pyx_kp_s_bencode2__encoder_pyx __pyx_mstate_global->__pyx_kp_s_bencode2__encoder_pyx
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_collections_abc __pyx_mstate_global->__pyx_n_s_collections_abc
 #define __pyx_n_s_compat __pyx_mstate_global->__pyx_n_s_compat
 #define __pyx_n_b_d __pyx_mstate_global->__pyx_n_b_d
 #define __pyx_n_b_e __pyx_mstate_global->__pyx_n_b_e
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_encode_dict_locals_lambda __pyx_mstate_global->__pyx_n_s_encode_dict_locals_lambda
@@ -2675,107 +2675,107 @@
 #define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
 /* #### Code section: module_code ### */
 
-/* "bencode2/encoder.pyx":17
- * from .exceptions import BencodeEncodeError
+/* "bencode2/_encoder.pyx":17
+ * from ._exceptions import BencodeEncodeError
  * 
  * cpdef bytes encode(value: Any):             # <<<<<<<<<<<<<<
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  */
 
-static PyObject *__pyx_pw_8bencode2_7encoder_1encode(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_encoder_1encode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyObject *__pyx_f_8bencode2_7encoder_encode(PyObject *__pyx_v_value, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_f_8bencode2_8_encoder_encode(PyObject *__pyx_v_value, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_v_r = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode", 1);
 
-  /* "bencode2/encoder.pyx":18
+  /* "bencode2/_encoder.pyx":18
  * 
  * cpdef bytes encode(value: Any):
  *     r: list[bytes] = []  # makes more sense for something with lots of appends             # <<<<<<<<<<<<<<
  * 
  *     __encode(value, r)
  */
   __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bencode2/encoder.pyx":20
+  /* "bencode2/_encoder.pyx":20
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  *     __encode(value, r)             # <<<<<<<<<<<<<<
  * 
  *     # Join parts
  */
-  __pyx_t_1 = __pyx_f_8bencode2_7encoder___encode(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bencode2/encoder.pyx":23
+  /* "bencode2/_encoder.pyx":23
  * 
  *     # Join parts
  *     return b"".join(r)             # <<<<<<<<<<<<<<
  * 
  * cdef __encode(value, r: list[bytes]):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __Pyx_PyBytes_Join(__pyx_kp_b_, __pyx_v_r); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_1))) __PYX_ERR(0, 23, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/encoder.pyx":17
- * from .exceptions import BencodeEncodeError
+  /* "bencode2/_encoder.pyx":17
+ * from ._exceptions import BencodeEncodeError
  * 
  * cpdef bytes encode(value: Any):             # <<<<<<<<<<<<<<
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("bencode2.encoder.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_r);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_7encoder_1encode(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_encoder_1encode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8bencode2_7encoder_1encode = {"encode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_7encoder_1encode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8bencode2_7encoder_1encode(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8bencode2_8_encoder_1encode = {"encode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_encoder_1encode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_encoder_1encode(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_value = 0;
@@ -2837,66 +2837,66 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2.encoder.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8bencode2_7encoder_encode(__pyx_self, __pyx_v_value);
+  __pyx_r = __pyx_pf_8bencode2_8_encoder_encode(__pyx_self, __pyx_v_value);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_7encoder_encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_8bencode2_8_encoder_encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8bencode2_7encoder_encode(__pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8bencode2_8_encoder_encode(__pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("bencode2.encoder.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/encoder.pyx":25
+/* "bencode2/_encoder.pyx":25
  *     return b"".join(r)
  * 
  * cdef __encode(value, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)
  */
 
-static PyObject *__pyx_f_8bencode2_7encoder___encode(PyObject *__pyx_v_value, PyObject *__pyx_v_r) {
+static PyObject *__pyx_f_8bencode2_8_encoder___encode(PyObject *__pyx_v_value, PyObject *__pyx_v_r) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   Py_ssize_t __pyx_t_5;
@@ -2904,235 +2904,235 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode", 1);
 
-  /* "bencode2/encoder.pyx":26
+  /* "bencode2/_encoder.pyx":26
  * 
  * cdef __encode(value, r: list[bytes]):
  *     if PyDict_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):
  */
   __pyx_t_1 = PyDict_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/encoder.pyx":27
+    /* "bencode2/_encoder.pyx":27
  * cdef __encode(value, r: list[bytes]):
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)             # <<<<<<<<<<<<<<
  *     elif PyString_Check(value):
  *         __encode_str(value, r)
  */
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_dict(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_dict(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/encoder.pyx":26
+    /* "bencode2/_encoder.pyx":26
  * 
  * cdef __encode(value, r: list[bytes]):
  *     if PyDict_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/encoder.pyx":28
+  /* "bencode2/_encoder.pyx":28
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_str(value, r)
  *     elif PyList_Check(value):
  */
   __pyx_t_1 = PyString_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/encoder.pyx":29
+    /* "bencode2/_encoder.pyx":29
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):
  *         __encode_str(value, r)             # <<<<<<<<<<<<<<
  *     elif PyList_Check(value):
  *         __encode_list(value, r)
  */
     if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(0, 29, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_str(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_str(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/encoder.pyx":28
+    /* "bencode2/_encoder.pyx":28
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_str(value, r)
  *     elif PyList_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/encoder.pyx":30
+  /* "bencode2/_encoder.pyx":30
  *     elif PyString_Check(value):
  *         __encode_str(value, r)
  *     elif PyList_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):
  */
   __pyx_t_1 = PyList_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/encoder.pyx":31
+    /* "bencode2/_encoder.pyx":31
  *         __encode_str(value, r)
  *     elif PyList_Check(value):
  *         __encode_list(value, r)             # <<<<<<<<<<<<<<
  *     elif PyTuple_Check(value):
  *         __encode_list(value, r)
  */
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_list(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_list(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/encoder.pyx":30
+    /* "bencode2/_encoder.pyx":30
  *     elif PyString_Check(value):
  *         __encode_str(value, r)
  *     elif PyList_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/encoder.pyx":32
+  /* "bencode2/_encoder.pyx":32
  *     elif PyList_Check(value):
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/encoder.pyx":33
+    /* "bencode2/_encoder.pyx":33
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):
  *         __encode_list(value, r)             # <<<<<<<<<<<<<<
  *     elif PyBytes_Check(value):
  *         __encode_bytes(value, r)
  */
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_list(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_list(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/encoder.pyx":32
+    /* "bencode2/_encoder.pyx":32
  *     elif PyList_Check(value):
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/encoder.pyx":34
+  /* "bencode2/_encoder.pyx":34
  *     elif PyTuple_Check(value):
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/encoder.pyx":35
+    /* "bencode2/_encoder.pyx":35
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):
  *         __encode_bytes(value, r)             # <<<<<<<<<<<<<<
  *     elif PyBool_Check(value):
  *         __encode_bool(value, r)
  */
     if (!(likely(PyBytes_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_value))) __PYX_ERR(0, 35, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_bytes(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bytes(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/encoder.pyx":34
+    /* "bencode2/_encoder.pyx":34
  *     elif PyTuple_Check(value):
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/encoder.pyx":36
+  /* "bencode2/_encoder.pyx":36
  *     elif PyBytes_Check(value):
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):
  */
   __pyx_t_1 = PyBool_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/encoder.pyx":37
+    /* "bencode2/_encoder.pyx":37
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):
  *         __encode_bool(value, r)             # <<<<<<<<<<<<<<
  *     elif PyInt_Check(value):
  *         __encode_int(value, r)
  */
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_bool(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bool(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/encoder.pyx":36
+    /* "bencode2/_encoder.pyx":36
  *     elif PyBytes_Check(value):
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/encoder.pyx":38
+  /* "bencode2/_encoder.pyx":38
  *     elif PyBool_Check(value):
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_int(value, r)
  *     else:
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_value);
   if (likely(__pyx_t_1)) {
 
-    /* "bencode2/encoder.pyx":39
+    /* "bencode2/_encoder.pyx":39
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):
  *         __encode_int(value, r)             # <<<<<<<<<<<<<<
  *     else:
  *         raise BencodeEncodeError(f"type '{type(value)}' not supported")
  */
     if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_v_value))) __PYX_ERR(0, 39, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_int(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/encoder.pyx":38
+    /* "bencode2/_encoder.pyx":38
  *     elif PyBool_Check(value):
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_int(value, r)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/encoder.pyx":41
+  /* "bencode2/_encoder.pyx":41
  *         __encode_int(value, r)
  *     else:
  *         raise BencodeEncodeError(f"type '{type(value)}' not supported")             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_int(x: int, r: list[bytes]):
  */
   /*else*/ {
@@ -3185,15 +3185,15 @@
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(0, 41, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "bencode2/encoder.pyx":25
+  /* "bencode2/_encoder.pyx":25
  *     return b"".join(r)
  * 
  * cdef __encode(value, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)
  */
 
@@ -3201,46 +3201,46 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("bencode2.encoder.__encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/encoder.pyx":43
+/* "bencode2/_encoder.pyx":43
  *         raise BencodeEncodeError(f"type '{type(value)}' not supported")
  * 
  * cdef __encode_int(x: int, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))
  * 
  */
 
-static PyObject *__pyx_f_8bencode2_7encoder___encode_int(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_int(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_int", 1);
 
-  /* "bencode2/encoder.pyx":44
+  /* "bencode2/_encoder.pyx":44
  * 
  * cdef __encode_int(x: int, r: list[bytes]):
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):
  */
   __pyx_t_2 = __Pyx_PyObject_Str(__pyx_v_x); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
@@ -3272,145 +3272,145 @@
   }
   __pyx_t_5 = __Pyx_ListComp_Append(__pyx_v_r, __pyx_n_b_i); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
   __pyx_t_6 = __Pyx_ListComp_Append(__pyx_v_r, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
   __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_r, __pyx_n_b_e); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   (void)((__pyx_t_5 | (__pyx_t_6 | __pyx_t_7)));
 
-  /* "bencode2/encoder.pyx":43
+  /* "bencode2/_encoder.pyx":43
  *         raise BencodeEncodeError(f"type '{type(value)}' not supported")
  * 
  * cdef __encode_int(x: int, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("bencode2.encoder.__encode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/encoder.pyx":46
+/* "bencode2/_encoder.pyx":46
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     if x:
  *         __encode_int(1, r)
  */
 
-static PyObject *__pyx_f_8bencode2_7encoder___encode_bool(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_bool(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_bool", 1);
 
-  /* "bencode2/encoder.pyx":47
+  /* "bencode2/_encoder.pyx":47
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):
  *     if x:             # <<<<<<<<<<<<<<
  *         __encode_int(1, r)
  *     else:
  */
   __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_x); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 47, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "bencode2/encoder.pyx":48
+    /* "bencode2/_encoder.pyx":48
  * cdef __encode_bool(x: bool, r: list[bytes]):
  *     if x:
  *         __encode_int(1, r)             # <<<<<<<<<<<<<<
  *     else:
  *         __encode_int(0, r)
  */
     if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_1))) __PYX_ERR(0, 48, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_int(((PyObject*)__pyx_int_1), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_int_1), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/encoder.pyx":47
+    /* "bencode2/_encoder.pyx":47
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):
  *     if x:             # <<<<<<<<<<<<<<
  *         __encode_int(1, r)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/encoder.pyx":50
+  /* "bencode2/_encoder.pyx":50
  *         __encode_int(1, r)
  *     else:
  *         __encode_int(0, r)             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_bytes(x: bytes, r: list[bytes]):
  */
   /*else*/ {
     if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 50, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_int(((PyObject*)__pyx_int_0), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_int_0), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "bencode2/encoder.pyx":46
+  /* "bencode2/_encoder.pyx":46
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     if x:
  *         __encode_int(1, r)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("bencode2.encoder.__encode_bool", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode_bool", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/encoder.pyx":52
+/* "bencode2/_encoder.pyx":52
  *         __encode_int(0, r)
  * 
  * cdef __encode_bytes(x: bytes, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, str(len(x)).encode("utf-8"))
  *     PyList_Append(r, b":")
  */
 
-static PyObject *__pyx_f_8bencode2_7encoder___encode_bytes(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_bytes(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_bytes", 1);
 
-  /* "bencode2/encoder.pyx":53
+  /* "bencode2/_encoder.pyx":53
  * 
  * cdef __encode_bytes(x: bytes, r: list[bytes]):
  *     PyList_Append(r, str(len(x)).encode("utf-8"))             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b":")
  *     PyList_Append(r, x)
  */
   __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_x); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
@@ -3443,141 +3443,141 @@
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bencode2/encoder.pyx":54
+  /* "bencode2/_encoder.pyx":54
  * cdef __encode_bytes(x: bytes, r: list[bytes]):
  *     PyList_Append(r, str(len(x)).encode("utf-8"))
  *     PyList_Append(r, b":")             # <<<<<<<<<<<<<<
  *     PyList_Append(r, x)
  * 
  */
   __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_kp_b__2); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 54, __pyx_L1_error)
 
-  /* "bencode2/encoder.pyx":55
+  /* "bencode2/_encoder.pyx":55
  *     PyList_Append(r, str(len(x)).encode("utf-8"))
  *     PyList_Append(r, b":")
  *     PyList_Append(r, x)             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_str(x: str, r: list[bytes]):
  */
   __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_v_x); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 55, __pyx_L1_error)
 
-  /* "bencode2/encoder.pyx":52
+  /* "bencode2/_encoder.pyx":52
  *         __encode_int(0, r)
  * 
  * cdef __encode_bytes(x: bytes, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, str(len(x)).encode("utf-8"))
  *     PyList_Append(r, b":")
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("bencode2.encoder.__encode_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/encoder.pyx":57
+/* "bencode2/_encoder.pyx":57
  *     PyList_Append(r, x)
  * 
  * cdef __encode_str(x: str, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     __encode_bytes(x.encode("UTF-8"), r)
  * 
  */
 
-static PyObject *__pyx_f_8bencode2_7encoder___encode_str(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_str(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_str", 1);
 
-  /* "bencode2/encoder.pyx":58
+  /* "bencode2/_encoder.pyx":58
  * 
  * cdef __encode_str(x: str, r: list[bytes]):
  *     __encode_bytes(x.encode("UTF-8"), r)             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_list(x: list | tuple, r: list[bytes]):
  */
   __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_x); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_f_8bencode2_7encoder___encode_bytes(((PyObject*)__pyx_t_1), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bytes(((PyObject*)__pyx_t_1), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/encoder.pyx":57
+  /* "bencode2/_encoder.pyx":57
  *     PyList_Append(r, x)
  * 
  * cdef __encode_str(x: str, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     __encode_bytes(x.encode("UTF-8"), r)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("bencode2.encoder.__encode_str", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode_str", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/encoder.pyx":60
+/* "bencode2/_encoder.pyx":60
  *     __encode_bytes(x.encode("UTF-8"), r)
  * 
  * cdef __encode_list(x: list | tuple, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b"l")
  * 
  */
 
-static PyObject *__pyx_f_8bencode2_7encoder___encode_list(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_list(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
   PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_list", 1);
 
-  /* "bencode2/encoder.pyx":61
+  /* "bencode2/_encoder.pyx":61
  * 
  * cdef __encode_list(x: list | tuple, r: list[bytes]):
  *     PyList_Append(r, b"l")             # <<<<<<<<<<<<<<
  * 
  *     for i in x:
  */
   __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_l); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 61, __pyx_L1_error)
 
-  /* "bencode2/encoder.pyx":63
+  /* "bencode2/_encoder.pyx":63
  *     PyList_Append(r, b"l")
  * 
  *     for i in x:             # <<<<<<<<<<<<<<
  *         __encode(i, r)
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_x)) || PyTuple_CheckExact(__pyx_v_x)) {
@@ -3631,85 +3631,85 @@
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "bencode2/encoder.pyx":64
+    /* "bencode2/_encoder.pyx":64
  * 
  *     for i in x:
  *         __encode(i, r)             # <<<<<<<<<<<<<<
  * 
  *     PyList_Append(r, b"e")
  */
-    __pyx_t_5 = __pyx_f_8bencode2_7encoder___encode(__pyx_v_i, __pyx_v_r); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_i, __pyx_v_r); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "bencode2/encoder.pyx":63
+    /* "bencode2/_encoder.pyx":63
  *     PyList_Append(r, b"l")
  * 
  *     for i in x:             # <<<<<<<<<<<<<<
  *         __encode(i, r)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/encoder.pyx":66
+  /* "bencode2/_encoder.pyx":66
  *         __encode(i, r)
  * 
  *     PyList_Append(r, b"e")             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_dict(x: Mapping, r: list[bytes]):
  */
   __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_e); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 66, __pyx_L1_error)
 
-  /* "bencode2/encoder.pyx":60
+  /* "bencode2/_encoder.pyx":60
  *     __encode_bytes(x.encode("UTF-8"), r)
  * 
  * cdef __encode_list(x: list | tuple, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b"l")
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("bencode2.encoder.__encode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/encoder.pyx":73
+/* "bencode2/_encoder.pyx":73
  *     # force all keys to bytes, because str and bytes are incomparable
  *     i_list = [(to_binary(k), v) for k, v in x.items()]
  *     i_list.sort(key=lambda kv: kv[0])             # <<<<<<<<<<<<<<
  * 
  *     for k, v in i_list:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_7encoder_13__encode_dict_lambda(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_encoder_13__encode_dict_lambda(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8bencode2_7encoder_13__encode_dict_lambda = {"lambda", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_7encoder_13__encode_dict_lambda, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8bencode2_7encoder_13__encode_dict_lambda(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8bencode2_8_encoder_13__encode_dict_lambda = {"lambda", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_encoder_13__encode_dict_lambda, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_encoder_13__encode_dict_lambda(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_kv = 0;
@@ -3771,15 +3771,15 @@
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2.encoder.__encode_dict.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode_dict.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_lambda_funcdef_lambda(__pyx_self, __pyx_v_kv);
 
   /* function exit code */
   {
@@ -3806,31 +3806,31 @@
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("bencode2.encoder.__encode_dict.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode_dict.lambda", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/encoder.pyx":68
+/* "bencode2/_encoder.pyx":68
  *     PyList_Append(r, b"e")
  * 
  * cdef __encode_dict(x: Mapping, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b"d")
  * 
  */
 
-static PyObject *__pyx_f_8bencode2_7encoder___encode_dict(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
+static PyObject *__pyx_f_8bencode2_8_encoder___encode_dict(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
   PyObject *__pyx_v_i_list = NULL;
   PyObject *__pyx_v_k = NULL;
   PyObject *__pyx_v_v = NULL;
   PyObject *__pyx_7genexpr__pyx_v_k = NULL;
   PyObject *__pyx_7genexpr__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -3845,24 +3845,24 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *(*__pyx_t_10)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_dict", 1);
 
-  /* "bencode2/encoder.pyx":69
+  /* "bencode2/_encoder.pyx":69
  * 
  * cdef __encode_dict(x: Mapping, r: list[bytes]):
  *     PyList_Append(r, b"d")             # <<<<<<<<<<<<<<
  * 
  *     # force all keys to bytes, because str and bytes are incomparable
  */
   __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_d); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 69, __pyx_L1_error)
 
-  /* "bencode2/encoder.pyx":72
+  /* "bencode2/_encoder.pyx":72
  * 
  *     # force all keys to bytes, because str and bytes are incomparable
  *     i_list = [(to_binary(k), v) for k, v in x.items()]             # <<<<<<<<<<<<<<
  *     i_list.sort(key=lambda kv: kv[0])
  * 
  */
   { /* enter inner scope */
@@ -3932,36 +3932,36 @@
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_i_list = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "bencode2/encoder.pyx":73
+  /* "bencode2/_encoder.pyx":73
  *     # force all keys to bytes, because str and bytes are incomparable
  *     i_list = [(to_binary(k), v) for k, v in x.items()]
  *     i_list.sort(key=lambda kv: kv[0])             # <<<<<<<<<<<<<<
  * 
  *     for k, v in i_list:
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_i_list, __pyx_n_s_sort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7encoder_13__encode_dict_lambda, 0, __pyx_n_s_encode_dict_locals_lambda, NULL, __pyx_n_s_bencode2_encoder, __pyx_d, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_encoder_13__encode_dict_lambda, 0, __pyx_n_s_encode_dict_locals_lambda, NULL, __pyx_n_s_bencode2__encoder, __pyx_d, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "bencode2/encoder.pyx":75
+  /* "bencode2/_encoder.pyx":75
  *     i_list.sort(key=lambda kv: kv[0])
  * 
  *     for k, v in i_list:             # <<<<<<<<<<<<<<
  *         __encode(k, r)
  *         __encode(v, r)
  */
   __pyx_t_6 = __pyx_v_i_list; __Pyx_INCREF(__pyx_t_6);
@@ -4027,54 +4027,54 @@
       __pyx_L12_unpacking_done:;
     }
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_2);
     __pyx_t_2 = 0;
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "bencode2/encoder.pyx":76
+    /* "bencode2/_encoder.pyx":76
  * 
  *     for k, v in i_list:
  *         __encode(k, r)             # <<<<<<<<<<<<<<
  *         __encode(v, r)
  * 
  */
-    __pyx_t_3 = __pyx_f_8bencode2_7encoder___encode(__pyx_v_k, __pyx_v_r); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_k, __pyx_v_r); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 76, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "bencode2/encoder.pyx":77
+    /* "bencode2/_encoder.pyx":77
  *     for k, v in i_list:
  *         __encode(k, r)
  *         __encode(v, r)             # <<<<<<<<<<<<<<
  * 
  *     PyList_Append(r, b"e")
  */
-    __pyx_t_3 = __pyx_f_8bencode2_7encoder___encode(__pyx_v_v, __pyx_v_r); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_v, __pyx_v_r); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "bencode2/encoder.pyx":75
+    /* "bencode2/_encoder.pyx":75
  *     i_list.sort(key=lambda kv: kv[0])
  * 
  *     for k, v in i_list:             # <<<<<<<<<<<<<<
  *         __encode(k, r)
  *         __encode(v, r)
  */
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "bencode2/encoder.pyx":79
+  /* "bencode2/_encoder.pyx":79
  *         __encode(v, r)
  * 
  *     PyList_Append(r, b"e")             # <<<<<<<<<<<<<<
  */
   __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_e); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "bencode2/encoder.pyx":68
+  /* "bencode2/_encoder.pyx":68
  *     PyList_Append(r, b"e")
  * 
  * cdef __encode_dict(x: Mapping, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b"d")
  * 
  */
 
@@ -4083,15 +4083,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_9);
-  __Pyx_AddTraceback("bencode2.encoder.__encode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._encoder.__encode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_i_list);
   __Pyx_XDECREF(__pyx_v_k);
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v);
@@ -4120,16 +4120,16 @@
     {&__pyx_n_s_Any, __pyx_k_Any, sizeof(__pyx_k_Any), 0, 0, 1, 1},
     {&__pyx_n_s_BencodeEncodeError, __pyx_k_BencodeEncodeError, sizeof(__pyx_k_BencodeEncodeError), 0, 0, 1, 1},
     {&__pyx_n_s_Mapping, __pyx_k_Mapping, sizeof(__pyx_k_Mapping), 0, 0, 1, 1},
     {&__pyx_kp_b__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 0, 0},
     {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
     {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
-    {&__pyx_n_s_bencode2_encoder, __pyx_k_bencode2_encoder, sizeof(__pyx_k_bencode2_encoder), 0, 0, 1, 1},
-    {&__pyx_kp_s_bencode2_encoder_pyx, __pyx_k_bencode2_encoder_pyx, sizeof(__pyx_k_bencode2_encoder_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_bencode2__encoder, __pyx_k_bencode2__encoder, sizeof(__pyx_k_bencode2__encoder), 0, 0, 1, 1},
+    {&__pyx_kp_s_bencode2__encoder_pyx, __pyx_k_bencode2__encoder_pyx, sizeof(__pyx_k_bencode2__encoder_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_collections_abc, __pyx_k_collections_abc, sizeof(__pyx_k_collections_abc), 0, 0, 1, 1},
     {&__pyx_n_s_compat, __pyx_k_compat, sizeof(__pyx_k_compat), 0, 0, 1, 1},
     {&__pyx_n_b_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 0, 0, 1},
     {&__pyx_n_b_e, __pyx_k_e, sizeof(__pyx_k_e), 0, 0, 0, 1},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_encode_dict_locals_lambda, __pyx_k_encode_dict_locals_lambda, sizeof(__pyx_k_encode_dict_locals_lambda), 0, 0, 1, 1},
@@ -4162,25 +4162,25 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "bencode2/encoder.pyx":17
- * from .exceptions import BencodeEncodeError
+  /* "bencode2/_encoder.pyx":17
+ * from ._exceptions import BencodeEncodeError
  * 
  * cpdef bytes encode(value: Any):             # <<<<<<<<<<<<<<
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_value); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2_encoder_pyx, __pyx_n_s_encode, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__encoder_pyx, __pyx_n_s_encode, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -4288,31 +4288,31 @@
   return 0;
 }
 
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_encoder(PyObject* module); /*proto*/
+static int __pyx_pymod_exec__encoder(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_encoder},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__encoder},
   {0, NULL}
 };
 #endif
 
 #ifdef __cplusplus
 namespace {
   struct PyModuleDef __pyx_moduledef =
   #else
   static struct PyModuleDef __pyx_moduledef =
   #endif
   {
       PyModuleDef_HEAD_INIT,
-      "encoder",
+      "_encoder",
       0, /* m_doc */
     #if CYTHON_PEP489_MULTI_PHASE_INIT
       0, /* m_size */
     #elif CYTHON_USE_MODULE_STATE
       sizeof(__pyx_mstate), /* m_size */
     #else
       -1, /* m_size */
@@ -4352,19 +4352,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initencoder(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initencoder(void)
+__Pyx_PyMODINIT_FUNC init_encoder(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC init_encoder(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_encoder(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_encoder(void)
+__Pyx_PyMODINIT_FUNC PyInit__encoder(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit__encoder(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -4437,15 +4437,15 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_encoder(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec__encoder(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   int stringtab_initialized = 0;
   #if CYTHON_USE_MODULE_STATE
   int pystate_addmodule_run = 0;
   #endif
@@ -4455,33 +4455,33 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'encoder' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module '_encoder' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("encoder", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("_encoder", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "encoder" pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "_encoder" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -4497,15 +4497,15 @@
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_encoder(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__encoder(void)", 0);
   if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -4535,22 +4535,22 @@
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_bencode2__encoder) {
+  if (__pyx_module_is_main_bencode2___encoder) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "bencode2.encoder")) {
-      if (unlikely((PyDict_SetItemString(modules, "bencode2.encoder", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "bencode2._encoder")) {
+      if (unlikely((PyDict_SetItemString(modules, "bencode2._encoder", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -4563,15 +4563,15 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "bencode2/encoder.pyx":3
+  /* "bencode2/_encoder.pyx":3
  * # cython: language_level=3
  * 
  * from collections.abc import Mapping             # <<<<<<<<<<<<<<
  * from typing import Any, Mapping
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
@@ -4584,15 +4584,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Mapping, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/encoder.pyx":4
+  /* "bencode2/_encoder.pyx":4
  * 
  * from collections.abc import Mapping
  * from typing import Any, Mapping             # <<<<<<<<<<<<<<
  * 
  * from cpython.bytes cimport PyBytes_Check
  */
   __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
@@ -4612,19 +4612,19 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Mapping, __pyx_t_3) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/encoder.pyx":14
+  /* "bencode2/_encoder.pyx":14
  * from cpython.string cimport PyString_Check
  * 
  * from ._compat import to_binary             # <<<<<<<<<<<<<<
- * from .exceptions import BencodeEncodeError
+ * from ._exceptions import BencodeEncodeError
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_to_binary);
   __Pyx_GIVEREF(__pyx_n_s_to_binary);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_to_binary)) __PYX_ERR(0, 14, __pyx_L1_error);
@@ -4633,18 +4633,18 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_to_binary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_binary, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/encoder.pyx":15
+  /* "bencode2/_encoder.pyx":15
  * 
  * from ._compat import to_binary
- * from .exceptions import BencodeEncodeError             # <<<<<<<<<<<<<<
+ * from ._exceptions import BencodeEncodeError             # <<<<<<<<<<<<<<
  * 
  * cpdef bytes encode(value: Any):
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_BencodeEncodeError);
   __Pyx_GIVEREF(__pyx_n_s_BencodeEncodeError);
@@ -4654,32 +4654,32 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_BencodeEncodeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeEncodeError, __pyx_t_3) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/encoder.pyx":17
- * from .exceptions import BencodeEncodeError
+  /* "bencode2/_encoder.pyx":17
+ * from ._exceptions import BencodeEncodeError
  * 
  * cpdef bytes encode(value: Any):             # <<<<<<<<<<<<<<
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_value, __pyx_n_s_Any) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_7encoder_1encode, 0, __pyx_n_s_encode, NULL, __pyx_n_s_bencode2_encoder, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_encoder_1encode, 0, __pyx_n_s_encode, NULL, __pyx_n_s_bencode2__encoder, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/encoder.pyx":1
+  /* "bencode2/_encoder.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
  * from collections.abc import Mapping
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -4689,29 +4689,29 @@
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init bencode2.encoder", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init bencode2._encoder", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
     Py_DECREF(__pyx_m);
     if (pystate_addmodule_run) {
       PyObject *tp, *value, *tb;
       PyErr_Fetch(&tp, &value, &tb);
       PyState_RemoveModule(&__pyx_moduledef);
       PyErr_Restore(tp, value, tb);
     }
     #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init bencode2.encoder");
+    PyErr_SetString(PyExc_ImportError, "init bencode2._encoder");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `bencode2-0.0.1/bencode2/encoder.pyx` & `bencode2-0.0.4/bencode2/_encoder.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cpython.list cimport PyList_Check, PyList_Append
 from cpython.tuple cimport PyTuple_Check
 from cpython.bool cimport PyBool_Check
 from cpython.dict cimport PyDict_Check
 from cpython.string cimport PyString_Check
 
 from ._compat import to_binary
-from .exceptions import BencodeEncodeError
+from ._exceptions import BencodeEncodeError
 
 cpdef bytes encode(value: Any):
     r: list[bytes] = []  # makes more sense for something with lots of appends
 
     __encode(value, r)
 
     # Join parts
```

### Comparing `bencode2-0.0.1/bencode2/exceptions.c` & `bencode2-0.0.4/bencode2/_exceptions.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 /* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "name": "bencode2.exceptions",
+        "name": "bencode2._exceptions",
         "sources": [
-            "bencode2\\exceptions.pyx"
+            "bencode2/_exceptions.pyx"
         ]
     },
-    "module_name": "bencode2.exceptions"
+    "module_name": "bencode2._exceptions"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
@@ -1224,16 +1224,16 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__bencode2__exceptions
-#define __PYX_HAVE_API__bencode2__exceptions
+#define __PYX_HAVE__bencode2___exceptions
+#define __PYX_HAVE_API__bencode2___exceptions
 /* Early includes */
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -1475,15 +1475,15 @@
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "bencode2\\\\exceptions.pyx",
+  "bencode2/_exceptions.pyx",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
@@ -1815,22 +1815,22 @@
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 
-/* Module declarations from "bencode2.exceptions" */
+/* Module declarations from "bencode2._exceptions" */
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "bencode2.exceptions"
-extern int __pyx_module_is_main_bencode2__exceptions;
-int __pyx_module_is_main_bencode2__exceptions = 0;
+#define __Pyx_MODULE_NAME "bencode2._exceptions"
+extern int __pyx_module_is_main_bencode2___exceptions;
+int __pyx_module_is_main_bencode2___exceptions = 0;
 
-/* Implementation of "bencode2.exceptions" */
+/* Implementation of "bencode2._exceptions" */
 /* #### Code section: global_var ### */
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "?";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
@@ -1842,17 +1842,17 @@
 static const char __pyx_k_set_name[] = "__set_name__";
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_mro_entries[] = "__mro_entries__";
 static const char __pyx_k_init_subclass[] = "__init_subclass__";
 static const char __pyx_k_BencodeDecodeError[] = "BencodeDecodeError";
 static const char __pyx_k_BencodeEncodeError[] = "BencodeEncodeError";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_bencode2_exceptions[] = "bencode2.exceptions";
 static const char __pyx_k_Bencode_decode_error[] = "Bencode decode error.";
 static const char __pyx_k_Bencode_encode_error[] = "Bencode encode error.";
+static const char __pyx_k_bencode2__exceptions[] = "bencode2._exceptions";
 /* #### Code section: decls ### */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -1880,15 +1880,15 @@
   #if CYTHON_USE_MODULE_STATE
   #endif
   PyObject *__pyx_n_s_;
   PyObject *__pyx_n_s_BencodeDecodeError;
   PyObject *__pyx_n_s_BencodeEncodeError;
   PyObject *__pyx_kp_s_Bencode_decode_error;
   PyObject *__pyx_kp_s_Bencode_encode_error;
-  PyObject *__pyx_n_s_bencode2_exceptions;
+  PyObject *__pyx_n_s_bencode2__exceptions;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_doc;
   PyObject *__pyx_n_s_init_subclass;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_metaclass;
   PyObject *__pyx_n_s_module;
@@ -1942,15 +1942,15 @@
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
   Py_CLEAR(clear_module_state->__pyx_n_s_);
   Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecodeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_BencodeEncodeError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Bencode_decode_error);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Bencode_encode_error);
-  Py_CLEAR(clear_module_state->__pyx_n_s_bencode2_exceptions);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bencode2__exceptions);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
   Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_module);
@@ -1982,15 +1982,15 @@
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
   Py_VISIT(traverse_module_state->__pyx_n_s_);
   Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecodeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_BencodeEncodeError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Bencode_decode_error);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Bencode_encode_error);
-  Py_VISIT(traverse_module_state->__pyx_n_s_bencode2_exceptions);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bencode2__exceptions);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
   Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_module);
@@ -2032,15 +2032,15 @@
 #if CYTHON_USE_MODULE_STATE
 #endif
 #define __pyx_n_s_ __pyx_mstate_global->__pyx_n_s_
 #define __pyx_n_s_BencodeDecodeError __pyx_mstate_global->__pyx_n_s_BencodeDecodeError
 #define __pyx_n_s_BencodeEncodeError __pyx_mstate_global->__pyx_n_s_BencodeEncodeError
 #define __pyx_kp_s_Bencode_decode_error __pyx_mstate_global->__pyx_kp_s_Bencode_decode_error
 #define __pyx_kp_s_Bencode_encode_error __pyx_mstate_global->__pyx_kp_s_Bencode_encode_error
-#define __pyx_n_s_bencode2_exceptions __pyx_mstate_global->__pyx_n_s_bencode2_exceptions
+#define __pyx_n_s_bencode2__exceptions __pyx_mstate_global->__pyx_n_s_bencode2__exceptions
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
 #define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
 #define __pyx_n_s_module __pyx_mstate_global->__pyx_n_s_module
@@ -2070,15 +2070,15 @@
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_n_s_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 1, 1},
     {&__pyx_n_s_BencodeDecodeError, __pyx_k_BencodeDecodeError, sizeof(__pyx_k_BencodeDecodeError), 0, 0, 1, 1},
     {&__pyx_n_s_BencodeEncodeError, __pyx_k_BencodeEncodeError, sizeof(__pyx_k_BencodeEncodeError), 0, 0, 1, 1},
     {&__pyx_kp_s_Bencode_decode_error, __pyx_k_Bencode_decode_error, sizeof(__pyx_k_Bencode_decode_error), 0, 0, 1, 0},
     {&__pyx_kp_s_Bencode_encode_error, __pyx_k_Bencode_encode_error, sizeof(__pyx_k_Bencode_encode_error), 0, 0, 1, 0},
-    {&__pyx_n_s_bencode2_exceptions, __pyx_k_bencode2_exceptions, sizeof(__pyx_k_bencode2_exceptions), 0, 0, 1, 1},
+    {&__pyx_n_s_bencode2__exceptions, __pyx_k_bencode2__exceptions, sizeof(__pyx_k_bencode2__exceptions), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
     {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
     {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
@@ -2184,31 +2184,31 @@
   return 0;
 }
 
 
 #if PY_MAJOR_VERSION >= 3
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_exceptions(PyObject* module); /*proto*/
+static int __pyx_pymod_exec__exceptions(PyObject* module); /*proto*/
 static PyModuleDef_Slot __pyx_moduledef_slots[] = {
   {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_exceptions},
+  {Py_mod_exec, (void*)__pyx_pymod_exec__exceptions},
   {0, NULL}
 };
 #endif
 
 #ifdef __cplusplus
 namespace {
   struct PyModuleDef __pyx_moduledef =
   #else
   static struct PyModuleDef __pyx_moduledef =
   #endif
   {
       PyModuleDef_HEAD_INIT,
-      "exceptions",
+      "_exceptions",
       0, /* m_doc */
     #if CYTHON_PEP489_MULTI_PHASE_INIT
       0, /* m_size */
     #elif CYTHON_USE_MODULE_STATE
       sizeof(__pyx_mstate), /* m_size */
     #else
       -1, /* m_size */
@@ -2248,19 +2248,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initexceptions(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initexceptions(void)
+__Pyx_PyMODINIT_FUNC init_exceptions(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC init_exceptions(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_exceptions(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_exceptions(void)
+__Pyx_PyMODINIT_FUNC PyInit__exceptions(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit__exceptions(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -2333,15 +2333,15 @@
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_exceptions(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec__exceptions(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   int stringtab_initialized = 0;
   #if CYTHON_USE_MODULE_STATE
   int pystate_addmodule_run = 0;
   #endif
@@ -2353,33 +2353,33 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'exceptions' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module '_exceptions' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("exceptions", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("_exceptions", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "exceptions" pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "_exceptions" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -2395,15 +2395,15 @@
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_exceptions(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__exceptions(void)", 0);
   if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2433,22 +2433,22 @@
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_bencode2__exceptions) {
+  if (__pyx_module_is_main_bencode2___exceptions) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "bencode2.exceptions")) {
-      if (unlikely((PyDict_SetItemString(modules, "bencode2.exceptions", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "bencode2._exceptions")) {
+      if (unlikely((PyDict_SetItemString(modules, "bencode2._exceptions", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2461,15 +2461,15 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "bencode2/exceptions.pyx":3
+  /* "bencode2/_exceptions.pyx":3
  * # cython: language_level=3
  * 
  * class BencodeDecodeError(Exception):             # <<<<<<<<<<<<<<
  *     """Bencode decode error."""
  * 
  */
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
@@ -2477,58 +2477,58 @@
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])))) __PYX_ERR(0, 3, __pyx_L1_error);
   __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_BencodeDecodeError, __pyx_n_s_BencodeDecodeError, (PyObject *) NULL, __pyx_n_s_bencode2_exceptions, __pyx_kp_s_Bencode_decode_error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_BencodeDecodeError, __pyx_n_s_BencodeDecodeError, (PyObject *) NULL, __pyx_n_s_bencode2__exceptions, __pyx_kp_s_Bencode_decode_error); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (__pyx_t_3 != __pyx_t_2) {
     if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 3, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_BencodeDecodeError, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeDecodeError, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/exceptions.pyx":7
+  /* "bencode2/_exceptions.pyx":7
  * 
  * 
  * class BencodeEncodeError(Exception):             # <<<<<<<<<<<<<<
  *     """Bencode encode error."""
  */
   __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   __Pyx_GIVEREF((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0]));
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])))) __PYX_ERR(0, 7, __pyx_L1_error);
   __pyx_t_4 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_BencodeEncodeError, __pyx_n_s_BencodeEncodeError, (PyObject *) NULL, __pyx_n_s_bencode2_exceptions, __pyx_kp_s_Bencode_encode_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_4, __pyx_n_s_BencodeEncodeError, __pyx_n_s_BencodeEncodeError, (PyObject *) NULL, __pyx_n_s_bencode2__exceptions, __pyx_kp_s_Bencode_encode_error); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__pyx_t_4 != __pyx_t_3) {
     if (unlikely((PyDict_SetItemString(__pyx_t_2, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(0, 7, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_BencodeEncodeError, __pyx_t_4, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeEncodeError, __pyx_t_3) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "bencode2/exceptions.pyx":1
+  /* "bencode2/_exceptions.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
  * class BencodeDecodeError(Exception):
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_4) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2540,29 +2540,29 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init bencode2.exceptions", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init bencode2._exceptions", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
     Py_DECREF(__pyx_m);
     if (pystate_addmodule_run) {
       PyObject *tp, *value, *tb;
       PyErr_Fetch(&tp, &value, &tb);
       PyState_RemoveModule(&__pyx_moduledef);
       PyErr_Restore(tp, value, tb);
     }
     #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init bencode2.exceptions");
+    PyErr_SetString(PyExc_ImportError, "init bencode2._exceptions");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
```

### Comparing `bencode2-0.0.1/setup.py` & `bencode2-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup
 
 from Cython.Build import cythonize
 
 
 def get_readme():
     """Load README.rst for display on PyPI."""
-    with open('readme.md') as f:
+    with open('readme.md', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='bencode2',
-    version='0.0.1',
+    version='0.0.4',
     description='bencode serialize/deserialize library',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     author='trim21',
     author_email='trim21.me@gmail.com',
     url='https://github.com/trim21/py-bencode',
     package_dir={'bencode2': 'bencode2'},
     packages=['bencode2'],
+    package_data={'bencode2': ['py.typed']},
     include_package_data=True,
     ext_modules=cythonize(
         "bencode2/**/*.pyx",
         compiler_directives={"language_level": "3"},
     ),
 )
```

