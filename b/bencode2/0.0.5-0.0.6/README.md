# Comparing `tmp/bencode2-0.0.5.tar.gz` & `tmp/bencode2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode2-0.0.5.tar", last modified: Sun Apr 14 07:57:18 2024, max compression
+gzip compressed data, was "bencode2-0.0.6.tar", last modified: Sun Apr 14 10:11:20 2024, max compression
```

## Comparing `bencode2-0.0.5.tar` & `bencode2-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:57:18.558986 bencode2-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-14 07:57:14.000000 bencode2-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 07:57:14.000000 bencode2-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-14 07:57:18.558986 bencode2-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:57:18.558986 bencode2-0.0.5/bencode2/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-14 07:57:14.000000 bencode2-0.0.5/bencode2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   260090 2024-04-14 07:57:18.000000 bencode2-0.0.5/bencode2/_compat.c
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-14 07:57:14.000000 bencode2-0.0.5/bencode2/_compat.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   425745 2024-04-14 07:57:18.000000 bencode2-0.0.5/bencode2/_decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-14 07:57:14.000000 bencode2-0.0.5/bencode2/_decoder.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   351081 2024-04-14 07:57:18.000000 bencode2-0.0.5/bencode2/_encoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-14 07:57:14.000000 bencode2-0.0.5/bencode2/_encoder.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   190928 2024-04-14 07:57:18.000000 bencode2-0.0.5/bencode2/_exceptions.c
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-14 07:57:14.000000 bencode2-0.0.5/bencode2/_exceptions.pyx
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 07:57:14.000000 bencode2-0.0.5/bencode2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:57:18.558986 bencode2-0.0.5/bencode2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-14 07:57:18.000000 bencode2-0.0.5/bencode2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 07:57:18.000000 bencode2-0.0.5/bencode2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:57:18.000000 bencode2-0.0.5/bencode2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 07:57:18.000000 bencode2-0.0.5/bencode2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-14 07:57:14.000000 bencode2-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 07:57:18.558986 bencode2-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-14 07:57:14.000000 bencode2-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:11:20.075430 bencode2-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-14 10:11:14.000000 bencode2-0.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 10:11:14.000000 bencode2-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-14 10:11:20.075430 bencode2-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:11:20.075430 bencode2-0.0.6/bencode2/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-14 10:11:14.000000 bencode2-0.0.6/bencode2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   260090 2024-04-14 10:11:19.000000 bencode2-0.0.6/bencode2/_compat.c
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-14 10:11:14.000000 bencode2-0.0.6/bencode2/_compat.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   468793 2024-04-14 10:11:19.000000 bencode2-0.0.6/bencode2/_decoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-14 10:11:14.000000 bencode2-0.0.6/bencode2/_decoder.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   370647 2024-04-14 10:11:19.000000 bencode2-0.0.6/bencode2/_encoder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-14 10:11:14.000000 bencode2-0.0.6/bencode2/_encoder.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   190928 2024-04-14 10:11:19.000000 bencode2-0.0.6/bencode2/_exceptions.c
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-14 10:11:14.000000 bencode2-0.0.6/bencode2/_exceptions.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:11:14.000000 bencode2-0.0.6/bencode2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:11:20.075430 bencode2-0.0.6/bencode2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-14 10:11:20.000000 bencode2-0.0.6/bencode2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 10:11:20.000000 bencode2-0.0.6/bencode2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 10:11:20.000000 bencode2-0.0.6/bencode2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 10:11:20.000000 bencode2-0.0.6/bencode2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-14 10:11:14.000000 bencode2-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 10:11:20.075430 bencode2-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-14 10:11:14.000000 bencode2-0.0.6/setup.py
```

### Comparing `bencode2-0.0.5/bencode2/__init__.py` & `bencode2-0.0.6/bencode2/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,24 @@
 # cython: language_level=3
 
 from typing import Any
 
-from ._decoder import BencodeDecoder
-from ._encoder import encode
+from ._decoder import Decoder as _Decoder
+from ._encoder import encode as _encode
 from ._exceptions import BencodeDecodeError, BencodeEncodeError
 
 __all__ = (
     "BencodeDecodeError",
     "BencodeEncodeError",
     "bencode",
     "bdecode",
 )
 
 
 def bencode(value: Any) -> bytes:
-    """
-    Encode ``value`` into the bencode format.
+    """Encode value into the bencode format."""
+    return _encode(value)
 
-    :param value: Value
-    :type value: object
 
-    :return: Bencode formatted string
-    """
-    return encode(value)
-
-
-_decoder = BencodeDecoder()
-
-
-def bdecode(value: bytes) -> Any:
-    """
-    Decode bencode formatted byte string ``value``.
-
-    :param value: Bencode formatted string
-    :type value: bytes
-
-    :return: Decoded value
-    :rtype: object
-    """
-    return _decoder.decode(value)
+def bdecode(value: bytes, *, str_key: bool = False) -> Any:
+    """Decode bencode formatted bytes to python value."""
+    return _Decoder(str_key).decode(value)
```

### Comparing `bencode2-0.0.5/bencode2/_compat.c` & `bencode2-0.0.6/bencode2/_compat.c`

 * *Files identical despite different names*

### Comparing `bencode2-0.0.5/bencode2/_decoder.c` & `bencode2-0.0.6/bencode2/_decoder.c`

 * *Files 8% similar despite different names*

```diff
@@ -1476,26 +1476,66 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "bencode2/_decoder.pyx",
+  "<stringsource>",
 };
 /* #### Code section: utility_code_proto_before_types ### */
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
+struct __pyx_obj_8bencode2_8_decoder_Decoder;
+struct __pyx_ctuple_int__and_int;
+typedef struct __pyx_ctuple_int__and_int __pyx_ctuple_int__and_int;
+
+/* "bencode2/_decoder.pyx":36
+ *             f"unexpected token {x[index:index + 1]} at index {index}")
+ * 
+ *     cdef tuple[int, int] __decode_int(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         index += 1
+ *         new_f = x.index(b"e", index)
+ */
+struct __pyx_ctuple_int__and_int {
+  int f0;
+  int f1;
+};
+
+/* "bencode2/_decoder.pyx":6
+ * from ._exceptions import BencodeDecodeError
+ * 
+ * cdef class Decoder:             # <<<<<<<<<<<<<<
+ *     str_key: bool
+ * 
+ */
+struct __pyx_obj_8bencode2_8_decoder_Decoder {
+  PyObject_HEAD
+  struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *__pyx_vtab;
+  PyObject *str_key;
+};
+
+
+
+struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder {
+  PyObject *(*_Decoder__decode)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *);
+  __pyx_ctuple_int__and_int (*_Decoder__decode_int)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *);
+  PyObject *(*_Decoder__decode_list)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *);
+  PyObject *(*_Decoder__decode_str)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *);
+  PyObject *(*_Decoder__decode_dict)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *);
+};
+static struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *__pyx_vtabptr_8bencode2_8_decoder_Decoder;
 /* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
@@ -1711,29 +1751,56 @@
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
-/* PyObjectSetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
-#else
-#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
-#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
-#endif
-
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
+/* RaiseUnexpectedTypeError.proto */
+static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
+
+/* RaiseTooManyValuesToUnpack.proto */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
+
+/* RaiseNeedMoreValuesToUnpack.proto */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
+
+/* RaiseNoneIterError.proto */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1773,14 +1840,36 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
+/* PyObjectFormatSimple.proto */
+#if CYTHON_COMPILING_IN_PYPY
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#elif PY_MAJOR_VERSION < 3
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
+        PyObject_Format(s, f))
+#elif CYTHON_USE_TYPE_SLOTS
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_repr(s) :\
+        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_repr(s) :\
+        PyObject_Format(s, f))
+#else
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#endif
+
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
 #if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
 #endif
@@ -1824,16 +1913,24 @@
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectFastCall.proto */
 #define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
-/* RaiseUnexpectedTypeError.proto */
-static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
+/* SwapException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
+#endif
 
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
@@ -1859,59 +1956,35 @@
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
-
-/* RaiseNeedMoreValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
-
-/* IterFinish.proto */
-static CYTHON_INLINE int __Pyx_IterFinish(void);
-
-/* UnpackItemEndCheck.proto */
-static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
-
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
+/* JoinPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char);
 
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+/* UnpackUnboundCMethod.proto */
+typedef struct {
+    PyObject *type;
+    PyObject **method_name;
+    PyCFunction func;
+    PyObject *method;
+    int flag;
+} __Pyx_CachedCFunction;
+
+/* CallUnboundCMethod2.proto */
+static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
+static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
 #endif
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
-
-/* SliceObject.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(
-        PyObject* obj, Py_ssize_t cstart, Py_ssize_t cstop,
-        PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
-        int has_cstart, int has_cstop, int wraparound);
-
 /* PyIntBinop.proto */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check);
 #else
 #define __Pyx_PyInt_AddObjC(op1, op2, intval, inplace, zerodivision_check)\
     (inplace ? PyNumber_InPlaceAdd(op1, op2) : PyNumber_Add(op1, op2))
 #endif
@@ -1933,28 +2006,97 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* KeywordStringCheck.proto */
+static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
+
+/* GetAttr3.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
+
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
+/* GetAttr.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
+
+/* HasAttr.proto */
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+#define __Pyx_HasAttr(o, n)  PyObject_HasAttrWithError(o, n)
+#else
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+#endif
+
 /* IncludeStructmemberH.proto */
 #include <structmember.h>
 
 /* FixUpExtensionType.proto */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
+/* PyObjectCallNoArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
+
+/* ValidateBasesTuple.proto */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
+#endif
+
+/* PyType_Ready.proto */
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
+
+/* PyObject_GenericGetAttrNoDict.proto */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
+#endif
+
+/* PyObject_GenericGetAttr.proto */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
+#endif
+
+/* SetVTable.proto */
+static int __Pyx_SetVtable(PyTypeObject* typeptr , void* vtable);
+
+/* GetVTable.proto */
+static void* __Pyx_GetVtable(PyTypeObject *type);
+
+/* MergeVTables.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_MergeVtables(PyTypeObject *type);
+#endif
+
+/* SetupReduce.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_setup_reduce(PyObject* type_obj);
+#endif
+
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
@@ -2087,47 +2229,14 @@
 /* CythonFunction.proto */
 static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
-/* SetNameInClass.proto */
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
-#define __Pyx_SetNameInClass(ns, name, value)\
-    (likely(PyDict_CheckExact(ns)) ? _PyDict_SetItem_KnownHash(ns, name, value, ((PyASCIIObject *) name)->hash) : PyObject_SetItem(ns, name, value))
-#elif CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_SetNameInClass(ns, name, value)\
-    (likely(PyDict_CheckExact(ns)) ? PyDict_SetItem(ns, name, value) : PyObject_SetItem(ns, name, value))
-#else
-#define __Pyx_SetNameInClass(ns, name, value)  PyObject_SetItem(ns, name, value)
-#endif
-
-/* CalculateMetaclass.proto */
-static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
-
-/* PyObjectCall2Args.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
-
-/* PyObjectLookupSpecial.proto */
-#if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
-#define __Pyx_PyObject_LookupSpecialNoError(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 0)
-#define __Pyx_PyObject_LookupSpecial(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 1)
-static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error);
-#else
-#define __Pyx_PyObject_LookupSpecialNoError(o,n) __Pyx_PyObject_GetAttrStrNoError(o,n)
-#define __Pyx_PyObject_LookupSpecial(o,n) __Pyx_PyObject_GetAttrStr(o,n)
-#endif
-
-/* Py3ClassCreate.proto */
-static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
-                                           PyObject *mkw, PyObject *modname, PyObject *doc);
-static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
-                                      PyObject *mkw, int calculate_metaclass, int allow_py2_metaclass);
-
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -2148,41 +2257,50 @@
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 #endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
+/* GCCDiagnostics.proto */
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
+/* ToPyCTupleUtility.proto */
+static PyObject* __pyx_convert__to_py___pyx_ctuple_int__and_int(__pyx_ctuple_int__and_int);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
 #define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
 #else
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
-/* GCCDiagnostics.proto */
-#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
-/* CIntFromPy.proto */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
-
-/* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
-
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
@@ -2200,117 +2318,114 @@
 static unsigned long __Pyx_get_runtime_version(void);
 static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
+static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto*/
+static __pyx_ctuple_int__and_int __pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_int(CYTHON_UNUSED struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto*/
+static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_list(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto*/
+static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_str(CYTHON_UNUSED struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto*/
+static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_dict(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto*/
 
 /* Module declarations from "bencode2._decoder" */
+static PyObject *__pyx_f_8bencode2_8_decoder___pyx_unpickle_Decoder__set_state(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "bencode2._decoder"
 extern int __pyx_module_is_main_bencode2___decoder;
 int __pyx_module_is_main_bencode2___decoder = 0;
 
 /* Implementation of "bencode2._decoder" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_IndexError;
 static PyObject *__pyx_builtin_KeyError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_ValueError;
 /* #### Code section: string_decls ### */
-static const char __pyx_k_[] = "-";
+static const char __pyx_k_[] = ":";
 static const char __pyx_k_0[] = "0";
-static const char __pyx_k_1[] = "1";
-static const char __pyx_k_2[] = "2";
-static const char __pyx_k_3[] = "3";
-static const char __pyx_k_4[] = "4";
-static const char __pyx_k_5[] = "5";
-static const char __pyx_k_6[] = "6";
-static const char __pyx_k_7[] = "7";
-static const char __pyx_k_8[] = "8";
-static const char __pyx_k_9[] = "9";
-static const char __pyx_k_d[] = "d";
 static const char __pyx_k_e[] = "e";
-static const char __pyx_k_i[] = "i";
-static const char __pyx_k_k[] = "k";
-static const char __pyx_k_l[] = "l";
-static const char __pyx_k_n[] = "n";
-static const char __pyx_k_r[] = "r";
-static const char __pyx_k_s[] = "s";
-static const char __pyx_k_v[] = "v";
-static const char __pyx_k_x[] = "x";
-static const char __pyx_k__2[] = ":";
 static const char __pyx_k__3[] = ".";
+static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_Any[] = "Any";
-static const char __pyx_k__16[] = "?";
-static const char __pyx_k_doc[] = "__doc__";
-static const char __pyx_k_int[] = "int";
+static const char __pyx_k__12[] = "?";
+static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
-static const char __pyx_k_init[] = "__init__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_bytes[] = "bytes";
-static const char __pyx_k_colon[] = "colon";
 static const char __pyx_k_index[] = "index";
-static const char __pyx_k_new_f[] = "new_f";
-static const char __pyx_k_super[] = "super";
+static const char __pyx_k_state[] = "state";
+static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_value[] = "value";
-static const char __pyx_k_compat[] = "_compat";
 static const char __pyx_k_decode[] = "decode";
+static const char __pyx_k_dict_2[] = "_dict";
+static const char __pyx_k_enable[] = "enable";
+static const char __pyx_k_errors[] = "errors";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_length[] = "length";
-static const char __pyx_k_module[] = "__module__";
+static const char __pyx_k_pickle[] = "pickle";
+static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_return[] = "return";
+static const char __pyx_k_strict[] = "strict";
 static const char __pyx_k_typing[] = "typing";
-static const char __pyx_k_prepare[] = "__prepare__";
-static const char __pyx_k_Callable[] = "Callable";
+static const char __pyx_k_update[] = "update";
+static const char __pyx_k_Decoder[] = "Decoder";
+static const char __pyx_k_disable[] = "disable";
+static const char __pyx_k_str_key[] = "str_key";
 static const char __pyx_k_KeyError[] = "KeyError";
-static const char __pyx_k_qualname[] = "__qualname__";
-static const char __pyx_k_set_name[] = "__set_name__";
+static const char __pyx_k_at_index[] = " at index ";
+static const char __pyx_k_encoding[] = "encoding";
+static const char __pyx_k_getstate[] = "__getstate__";
+static const char __pyx_k_pyx_type[] = "__pyx_type";
+static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
-static const char __pyx_k_metaclass[] = "__metaclass__";
-static const char __pyx_k_to_binary[] = "to_binary";
+static const char __pyx_k_isenabled[] = "isenabled";
+static const char __pyx_k_pyx_state[] = "__pyx_state";
+static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
-static const char __pyx_k_decode_int[] = "decode_int";
 static const char __pyx_k_exceptions[] = "_exceptions";
-static const char __pyx_k_decode_dict[] = "decode_dict";
-static const char __pyx_k_decode_func[] = "decode_func";
-static const char __pyx_k_decode_list[] = "decode_list";
+static const char __pyx_k_pyx_result[] = "__pyx_result";
+static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
+static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
+static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
+static const char __pyx_k_stringsource[] = "<stringsource>";
+static const char __pyx_k_use_setstate[] = "use_setstate";
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
-static const char __pyx_k_decode_string[] = "decode_string";
-static const char __pyx_k_init_subclass[] = "__init_subclass__";
-static const char __pyx_k_BencodeDecoder[] = "BencodeDecoder";
-static const char __pyx_k_collections_abc[] = "collections.abc";
+static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_Decoder_decode[] = "Decoder.decode";
+static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
+static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_unexpected_token[] = "unexpected token ";
 static const char __pyx_k_bencode2__decoder[] = "bencode2._decoder";
 static const char __pyx_k_BencodeDecodeError[] = "BencodeDecodeError";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_BencodeDecoder___init[] = "BencodeDecoder.__init__";
-static const char __pyx_k_BencodeDecoder_decode[] = "BencodeDecoder.decode";
+static const char __pyx_k_pyx_unpickle_Decoder[] = "__pyx_unpickle_Decoder";
 static const char __pyx_k_bencode2__decoder_pyx[] = "bencode2/_decoder.pyx";
-static const char __pyx_k_BencodeDecoder_decode_int[] = "BencodeDecoder.decode_int";
-static const char __pyx_k_BencodeDecoder_decode_dict[] = "BencodeDecoder.decode_dict";
-static const char __pyx_k_BencodeDecoder_decode_list[] = "BencodeDecoder.decode_list";
-static const char __pyx_k_not_a_valid_bencoded_string[] = "not a valid bencoded string";
-static const char __pyx_k_BencodeDecoder_decode_string[] = "BencodeDecoder.decode_string";
-static const char __pyx_k_invalid_bencoded_value_data_afte[] = "invalid bencoded value (data after valid prefix)";
+static const char __pyx_k_Decoder___reduce_cython[] = "Decoder.__reduce_cython__";
+static const char __pyx_k_Decoder___setstate_cython[] = "Decoder.__setstate_cython__";
+static const char __pyx_k_not_a_valid_bencode_bytes[] = "not a valid bencode bytes: ";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))";
+static const char __pyx_k_invalid_bencode_value_data_after[] = "invalid bencode value (data after valid prefix)";
 /* #### Code section: decls ### */
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_2decode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_4decode_int(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_6decode_string(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_8decode_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_10decode_dict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index); /* proto */
+static int __pyx_pf_8bencode2_8_decoder_7Decoder___init__(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_str_key); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_7Decoder_2decode(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_7Decoder_4__reduce_cython__(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder_7Decoder_6__setstate_cython__(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8bencode2_8_decoder___pyx_unpickle_Decoder(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_8bencode2_8_decoder_Decoder(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static __Pyx_CachedCFunction __pyx_umethod_PyBytes_Type_index = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
   PyObject *__pyx_empty_tuple;
@@ -2331,111 +2446,104 @@
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineAwaitType;
   #endif
   #ifdef __Pyx_Coroutine_USED
   PyTypeObject *__pyx_CoroutineType;
   #endif
   #if CYTHON_USE_MODULE_STATE
+  PyObject *__pyx_type_8bencode2_8_decoder_Decoder;
   #endif
+  PyTypeObject *__pyx_ptype_8bencode2_8_decoder_Decoder;
   PyObject *__pyx_kp_b_;
   PyObject *__pyx_kp_b_0;
-  PyObject *__pyx_kp_b_1;
-  PyObject *__pyx_kp_b_2;
-  PyObject *__pyx_kp_b_3;
-  PyObject *__pyx_kp_b_4;
-  PyObject *__pyx_kp_b_5;
-  PyObject *__pyx_kp_b_6;
-  PyObject *__pyx_kp_b_7;
-  PyObject *__pyx_kp_b_8;
-  PyObject *__pyx_kp_b_9;
   PyObject *__pyx_n_s_Any;
   PyObject *__pyx_n_s_BencodeDecodeError;
-  PyObject *__pyx_n_s_BencodeDecoder;
-  PyObject *__pyx_n_s_BencodeDecoder___init;
-  PyObject *__pyx_n_s_BencodeDecoder_decode;
-  PyObject *__pyx_n_s_BencodeDecoder_decode_dict;
-  PyObject *__pyx_n_s_BencodeDecoder_decode_int;
-  PyObject *__pyx_n_s_BencodeDecoder_decode_list;
-  PyObject *__pyx_n_s_BencodeDecoder_decode_string;
-  PyObject *__pyx_n_s_Callable;
+  PyObject *__pyx_n_s_Decoder;
+  PyObject *__pyx_n_s_Decoder___reduce_cython;
+  PyObject *__pyx_n_s_Decoder___setstate_cython;
+  PyObject *__pyx_n_s_Decoder_decode;
+  PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_n_s_IndexError;
   PyObject *__pyx_n_s_KeyError;
+  PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_ValueError;
-  PyObject *__pyx_n_s__16;
-  PyObject *__pyx_kp_b__2;
+  PyObject *__pyx_n_s__12;
   PyObject *__pyx_kp_u__3;
   PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_kp_u_at_index;
   PyObject *__pyx_n_s_bencode2__decoder;
   PyObject *__pyx_kp_s_bencode2__decoder_pyx;
   PyObject *__pyx_n_s_bytes;
   PyObject *__pyx_n_s_class_getitem;
   PyObject *__pyx_n_s_cline_in_traceback;
-  PyObject *__pyx_n_s_collections_abc;
-  PyObject *__pyx_n_s_colon;
-  PyObject *__pyx_n_s_compat;
-  PyObject *__pyx_n_b_d;
   PyObject *__pyx_n_s_data;
   PyObject *__pyx_n_s_decode;
-  PyObject *__pyx_n_s_decode_dict;
-  PyObject *__pyx_n_s_decode_func;
-  PyObject *__pyx_n_s_decode_int;
-  PyObject *__pyx_n_s_decode_list;
-  PyObject *__pyx_n_s_decode_string;
   PyObject *__pyx_n_s_dict;
-  PyObject *__pyx_n_s_doc;
+  PyObject *__pyx_n_s_dict_2;
+  PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_n_b_e;
+  PyObject *__pyx_n_s_e;
+  PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_s_encoding;
+  PyObject *__pyx_n_s_errors;
   PyObject *__pyx_n_s_exceptions;
-  PyObject *__pyx_n_b_i;
+  PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_index;
-  PyObject *__pyx_n_s_init;
-  PyObject *__pyx_n_s_init_subclass;
-  PyObject *__pyx_n_s_int;
-  PyObject *__pyx_kp_u_invalid_bencoded_value_data_afte;
+  PyObject *__pyx_kp_u_invalid_bencode_value_data_after;
   PyObject *__pyx_n_s_is_coroutine;
-  PyObject *__pyx_n_s_k;
-  PyObject *__pyx_n_b_l;
+  PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_length;
   PyObject *__pyx_n_s_main;
-  PyObject *__pyx_n_s_metaclass;
-  PyObject *__pyx_n_s_module;
-  PyObject *__pyx_n_s_n;
   PyObject *__pyx_n_s_name;
-  PyObject *__pyx_n_s_new_f;
-  PyObject *__pyx_kp_u_not_a_valid_bencoded_string;
-  PyObject *__pyx_n_s_prepare;
-  PyObject *__pyx_n_s_qualname;
-  PyObject *__pyx_n_s_r;
+  PyObject *__pyx_n_s_new;
+  PyObject *__pyx_kp_u_not_a_valid_bencode_bytes;
+  PyObject *__pyx_n_s_pickle;
+  PyObject *__pyx_n_s_pyx_PickleError;
+  PyObject *__pyx_n_s_pyx_checksum;
+  PyObject *__pyx_n_s_pyx_result;
+  PyObject *__pyx_n_s_pyx_state;
+  PyObject *__pyx_n_s_pyx_type;
+  PyObject *__pyx_n_s_pyx_unpickle_Decoder;
+  PyObject *__pyx_n_s_pyx_vtable;
+  PyObject *__pyx_n_s_reduce;
+  PyObject *__pyx_n_s_reduce_cython;
+  PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_return;
-  PyObject *__pyx_n_s_s;
   PyObject *__pyx_n_s_self;
-  PyObject *__pyx_n_s_set_name;
-  PyObject *__pyx_n_s_super;
+  PyObject *__pyx_n_s_setstate;
+  PyObject *__pyx_n_s_setstate_cython;
+  PyObject *__pyx_n_s_state;
+  PyObject *__pyx_n_s_str_key;
+  PyObject *__pyx_n_u_strict;
+  PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
-  PyObject *__pyx_n_s_to_binary;
   PyObject *__pyx_n_s_typing;
-  PyObject *__pyx_n_s_v;
+  PyObject *__pyx_kp_u_unexpected_token;
+  PyObject *__pyx_n_s_update;
+  PyObject *__pyx_n_s_use_setstate;
+  PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_value;
-  PyObject *__pyx_n_s_x;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_2;
+  PyObject *__pyx_int_27736365;
+  PyObject *__pyx_int_148187747;
+  PyObject *__pyx_int_211139970;
+  PyObject *__pyx_tuple__2;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__10;
-  PyObject *__pyx_tuple__12;
-  PyObject *__pyx_tuple__14;
   PyObject *__pyx_codeobj__5;
   PyObject *__pyx_codeobj__7;
   PyObject *__pyx_codeobj__9;
   PyObject *__pyx_codeobj__11;
-  PyObject *__pyx_codeobj__13;
-  PyObject *__pyx_codeobj__15;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2470,110 +2578,103 @@
   Py_CLEAR(clear_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_8bencode2_8_decoder_Decoder);
+  Py_CLEAR(clear_module_state->__pyx_type_8bencode2_8_decoder_Decoder);
   Py_CLEAR(clear_module_state->__pyx_kp_b_);
   Py_CLEAR(clear_module_state->__pyx_kp_b_0);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_1);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_2);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_3);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_4);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_5);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_6);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_7);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_8);
-  Py_CLEAR(clear_module_state->__pyx_kp_b_9);
   Py_CLEAR(clear_module_state->__pyx_n_s_Any);
   Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecodeError);
-  Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecoder);
-  Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecoder___init);
-  Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecoder_decode);
-  Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecoder_decode_dict);
-  Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecoder_decode_int);
-  Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecoder_decode_list);
-  Py_CLEAR(clear_module_state->__pyx_n_s_BencodeDecoder_decode_string);
-  Py_CLEAR(clear_module_state->__pyx_n_s_Callable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Decoder);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Decoder___reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Decoder___setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Decoder_decode);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_n_s_IndexError);
   Py_CLEAR(clear_module_state->__pyx_n_s_KeyError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
-  Py_CLEAR(clear_module_state->__pyx_n_s__16);
-  Py_CLEAR(clear_module_state->__pyx_kp_b__2);
+  Py_CLEAR(clear_module_state->__pyx_n_s__12);
   Py_CLEAR(clear_module_state->__pyx_kp_u__3);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_at_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_bencode2__decoder);
   Py_CLEAR(clear_module_state->__pyx_kp_s_bencode2__decoder_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_bytes);
   Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
-  Py_CLEAR(clear_module_state->__pyx_n_s_collections_abc);
-  Py_CLEAR(clear_module_state->__pyx_n_s_colon);
-  Py_CLEAR(clear_module_state->__pyx_n_s_compat);
-  Py_CLEAR(clear_module_state->__pyx_n_b_d);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_decode);
-  Py_CLEAR(clear_module_state->__pyx_n_s_decode_dict);
-  Py_CLEAR(clear_module_state->__pyx_n_s_decode_func);
-  Py_CLEAR(clear_module_state->__pyx_n_s_decode_int);
-  Py_CLEAR(clear_module_state->__pyx_n_s_decode_list);
-  Py_CLEAR(clear_module_state->__pyx_n_s_decode_string);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
-  Py_CLEAR(clear_module_state->__pyx_n_s_doc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_n_b_e);
+  Py_CLEAR(clear_module_state->__pyx_n_s_e);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_encoding);
+  Py_CLEAR(clear_module_state->__pyx_n_s_errors);
   Py_CLEAR(clear_module_state->__pyx_n_s_exceptions);
-  Py_CLEAR(clear_module_state->__pyx_n_b_i);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_index);
-  Py_CLEAR(clear_module_state->__pyx_n_s_init);
-  Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
-  Py_CLEAR(clear_module_state->__pyx_n_s_int);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_invalid_bencoded_value_data_afte);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_invalid_bencode_value_data_after);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
-  Py_CLEAR(clear_module_state->__pyx_n_s_k);
-  Py_CLEAR(clear_module_state->__pyx_n_b_l);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_length);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
-  Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
-  Py_CLEAR(clear_module_state->__pyx_n_s_module);
-  Py_CLEAR(clear_module_state->__pyx_n_s_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
-  Py_CLEAR(clear_module_state->__pyx_n_s_new_f);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_not_a_valid_bencoded_string);
-  Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
-  Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
-  Py_CLEAR(clear_module_state->__pyx_n_s_r);
+  Py_CLEAR(clear_module_state->__pyx_n_s_new);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_not_a_valid_bencode_bytes);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_Decoder);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_return);
-  Py_CLEAR(clear_module_state->__pyx_n_s_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
-  Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
-  Py_CLEAR(clear_module_state->__pyx_n_s_super);
+  Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_state);
+  Py_CLEAR(clear_module_state->__pyx_n_s_str_key);
+  Py_CLEAR(clear_module_state->__pyx_n_u_strict);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
-  Py_CLEAR(clear_module_state->__pyx_n_s_to_binary);
   Py_CLEAR(clear_module_state->__pyx_n_s_typing);
-  Py_CLEAR(clear_module_state->__pyx_n_s_v);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_unexpected_token);
+  Py_CLEAR(clear_module_state->__pyx_n_s_update);
+  Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_value);
-  Py_CLEAR(clear_module_state->__pyx_n_s_x);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_2);
+  Py_CLEAR(clear_module_state->__pyx_int_27736365);
+  Py_CLEAR(clear_module_state->__pyx_int_148187747);
+  Py_CLEAR(clear_module_state->__pyx_int_211139970);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__10);
-  Py_CLEAR(clear_module_state->__pyx_tuple__12);
-  Py_CLEAR(clear_module_state->__pyx_tuple__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__5);
   Py_CLEAR(clear_module_state->__pyx_codeobj__7);
   Py_CLEAR(clear_module_state->__pyx_codeobj__9);
   Py_CLEAR(clear_module_state->__pyx_codeobj__11);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2586,110 +2687,103 @@
   Py_VISIT(traverse_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_8bencode2_8_decoder_Decoder);
+  Py_VISIT(traverse_module_state->__pyx_type_8bencode2_8_decoder_Decoder);
   Py_VISIT(traverse_module_state->__pyx_kp_b_);
   Py_VISIT(traverse_module_state->__pyx_kp_b_0);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_1);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_2);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_3);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_4);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_5);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_6);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_7);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_8);
-  Py_VISIT(traverse_module_state->__pyx_kp_b_9);
   Py_VISIT(traverse_module_state->__pyx_n_s_Any);
   Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecodeError);
-  Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecoder);
-  Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecoder___init);
-  Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecoder_decode);
-  Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecoder_decode_dict);
-  Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecoder_decode_int);
-  Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecoder_decode_list);
-  Py_VISIT(traverse_module_state->__pyx_n_s_BencodeDecoder_decode_string);
-  Py_VISIT(traverse_module_state->__pyx_n_s_Callable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Decoder);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Decoder___reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Decoder___setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Decoder_decode);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_n_s_IndexError);
   Py_VISIT(traverse_module_state->__pyx_n_s_KeyError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
-  Py_VISIT(traverse_module_state->__pyx_n_s__16);
-  Py_VISIT(traverse_module_state->__pyx_kp_b__2);
+  Py_VISIT(traverse_module_state->__pyx_n_s__12);
   Py_VISIT(traverse_module_state->__pyx_kp_u__3);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_at_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_bencode2__decoder);
   Py_VISIT(traverse_module_state->__pyx_kp_s_bencode2__decoder_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_bytes);
   Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
-  Py_VISIT(traverse_module_state->__pyx_n_s_collections_abc);
-  Py_VISIT(traverse_module_state->__pyx_n_s_colon);
-  Py_VISIT(traverse_module_state->__pyx_n_s_compat);
-  Py_VISIT(traverse_module_state->__pyx_n_b_d);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_decode);
-  Py_VISIT(traverse_module_state->__pyx_n_s_decode_dict);
-  Py_VISIT(traverse_module_state->__pyx_n_s_decode_func);
-  Py_VISIT(traverse_module_state->__pyx_n_s_decode_int);
-  Py_VISIT(traverse_module_state->__pyx_n_s_decode_list);
-  Py_VISIT(traverse_module_state->__pyx_n_s_decode_string);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
-  Py_VISIT(traverse_module_state->__pyx_n_s_doc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_n_b_e);
+  Py_VISIT(traverse_module_state->__pyx_n_s_e);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_encoding);
+  Py_VISIT(traverse_module_state->__pyx_n_s_errors);
   Py_VISIT(traverse_module_state->__pyx_n_s_exceptions);
-  Py_VISIT(traverse_module_state->__pyx_n_b_i);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_index);
-  Py_VISIT(traverse_module_state->__pyx_n_s_init);
-  Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
-  Py_VISIT(traverse_module_state->__pyx_n_s_int);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_invalid_bencoded_value_data_afte);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_invalid_bencode_value_data_after);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
-  Py_VISIT(traverse_module_state->__pyx_n_s_k);
-  Py_VISIT(traverse_module_state->__pyx_n_b_l);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_length);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
-  Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
-  Py_VISIT(traverse_module_state->__pyx_n_s_module);
-  Py_VISIT(traverse_module_state->__pyx_n_s_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
-  Py_VISIT(traverse_module_state->__pyx_n_s_new_f);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_not_a_valid_bencoded_string);
-  Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
-  Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
-  Py_VISIT(traverse_module_state->__pyx_n_s_r);
+  Py_VISIT(traverse_module_state->__pyx_n_s_new);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_not_a_valid_bencode_bytes);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_Decoder);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_return);
-  Py_VISIT(traverse_module_state->__pyx_n_s_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
-  Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
-  Py_VISIT(traverse_module_state->__pyx_n_s_super);
+  Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_state);
+  Py_VISIT(traverse_module_state->__pyx_n_s_str_key);
+  Py_VISIT(traverse_module_state->__pyx_n_u_strict);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
-  Py_VISIT(traverse_module_state->__pyx_n_s_to_binary);
   Py_VISIT(traverse_module_state->__pyx_n_s_typing);
-  Py_VISIT(traverse_module_state->__pyx_n_s_v);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_unexpected_token);
+  Py_VISIT(traverse_module_state->__pyx_n_s_update);
+  Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_value);
-  Py_VISIT(traverse_module_state->__pyx_n_s_x);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_2);
+  Py_VISIT(traverse_module_state->__pyx_int_27736365);
+  Py_VISIT(traverse_module_state->__pyx_int_148187747);
+  Py_VISIT(traverse_module_state->__pyx_int_211139970);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__10);
-  Py_VISIT(traverse_module_state->__pyx_tuple__12);
-  Py_VISIT(traverse_module_state->__pyx_tuple__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__5);
   Py_VISIT(traverse_module_state->__pyx_codeobj__7);
   Py_VISIT(traverse_module_state->__pyx_codeobj__9);
   Py_VISIT(traverse_module_state->__pyx_codeobj__11);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -2711,449 +2805,255 @@
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
 #endif
 #ifdef __Pyx_Coroutine_USED
 #define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
 #endif
 #if CYTHON_USE_MODULE_STATE
+#define __pyx_type_8bencode2_8_decoder_Decoder __pyx_mstate_global->__pyx_type_8bencode2_8_decoder_Decoder
 #endif
+#define __pyx_ptype_8bencode2_8_decoder_Decoder __pyx_mstate_global->__pyx_ptype_8bencode2_8_decoder_Decoder
 #define __pyx_kp_b_ __pyx_mstate_global->__pyx_kp_b_
 #define __pyx_kp_b_0 __pyx_mstate_global->__pyx_kp_b_0
-#define __pyx_kp_b_1 __pyx_mstate_global->__pyx_kp_b_1
-#define __pyx_kp_b_2 __pyx_mstate_global->__pyx_kp_b_2
-#define __pyx_kp_b_3 __pyx_mstate_global->__pyx_kp_b_3
-#define __pyx_kp_b_4 __pyx_mstate_global->__pyx_kp_b_4
-#define __pyx_kp_b_5 __pyx_mstate_global->__pyx_kp_b_5
-#define __pyx_kp_b_6 __pyx_mstate_global->__pyx_kp_b_6
-#define __pyx_kp_b_7 __pyx_mstate_global->__pyx_kp_b_7
-#define __pyx_kp_b_8 __pyx_mstate_global->__pyx_kp_b_8
-#define __pyx_kp_b_9 __pyx_mstate_global->__pyx_kp_b_9
 #define __pyx_n_s_Any __pyx_mstate_global->__pyx_n_s_Any
 #define __pyx_n_s_BencodeDecodeError __pyx_mstate_global->__pyx_n_s_BencodeDecodeError
-#define __pyx_n_s_BencodeDecoder __pyx_mstate_global->__pyx_n_s_BencodeDecoder
-#define __pyx_n_s_BencodeDecoder___init __pyx_mstate_global->__pyx_n_s_BencodeDecoder___init
-#define __pyx_n_s_BencodeDecoder_decode __pyx_mstate_global->__pyx_n_s_BencodeDecoder_decode
-#define __pyx_n_s_BencodeDecoder_decode_dict __pyx_mstate_global->__pyx_n_s_BencodeDecoder_decode_dict
-#define __pyx_n_s_BencodeDecoder_decode_int __pyx_mstate_global->__pyx_n_s_BencodeDecoder_decode_int
-#define __pyx_n_s_BencodeDecoder_decode_list __pyx_mstate_global->__pyx_n_s_BencodeDecoder_decode_list
-#define __pyx_n_s_BencodeDecoder_decode_string __pyx_mstate_global->__pyx_n_s_BencodeDecoder_decode_string
-#define __pyx_n_s_Callable __pyx_mstate_global->__pyx_n_s_Callable
+#define __pyx_n_s_Decoder __pyx_mstate_global->__pyx_n_s_Decoder
+#define __pyx_n_s_Decoder___reduce_cython __pyx_mstate_global->__pyx_n_s_Decoder___reduce_cython
+#define __pyx_n_s_Decoder___setstate_cython __pyx_mstate_global->__pyx_n_s_Decoder___setstate_cython
+#define __pyx_n_s_Decoder_decode __pyx_mstate_global->__pyx_n_s_Decoder_decode
+#define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_n_s_IndexError __pyx_mstate_global->__pyx_n_s_IndexError
 #define __pyx_n_s_KeyError __pyx_mstate_global->__pyx_n_s_KeyError
+#define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
-#define __pyx_n_s__16 __pyx_mstate_global->__pyx_n_s__16
-#define __pyx_kp_b__2 __pyx_mstate_global->__pyx_kp_b__2
+#define __pyx_n_s__12 __pyx_mstate_global->__pyx_n_s__12
 #define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_kp_u_at_index __pyx_mstate_global->__pyx_kp_u_at_index
 #define __pyx_n_s_bencode2__decoder __pyx_mstate_global->__pyx_n_s_bencode2__decoder
 #define __pyx_kp_s_bencode2__decoder_pyx __pyx_mstate_global->__pyx_kp_s_bencode2__decoder_pyx
 #define __pyx_n_s_bytes __pyx_mstate_global->__pyx_n_s_bytes
 #define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
-#define __pyx_n_s_collections_abc __pyx_mstate_global->__pyx_n_s_collections_abc
-#define __pyx_n_s_colon __pyx_mstate_global->__pyx_n_s_colon
-#define __pyx_n_s_compat __pyx_mstate_global->__pyx_n_s_compat
-#define __pyx_n_b_d __pyx_mstate_global->__pyx_n_b_d
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
 #define __pyx_n_s_decode __pyx_mstate_global->__pyx_n_s_decode
-#define __pyx_n_s_decode_dict __pyx_mstate_global->__pyx_n_s_decode_dict
-#define __pyx_n_s_decode_func __pyx_mstate_global->__pyx_n_s_decode_func
-#define __pyx_n_s_decode_int __pyx_mstate_global->__pyx_n_s_decode_int
-#define __pyx_n_s_decode_list __pyx_mstate_global->__pyx_n_s_decode_list
-#define __pyx_n_s_decode_string __pyx_mstate_global->__pyx_n_s_decode_string
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
-#define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
+#define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
+#define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_n_b_e __pyx_mstate_global->__pyx_n_b_e
+#define __pyx_n_s_e __pyx_mstate_global->__pyx_n_s_e
+#define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_s_encoding __pyx_mstate_global->__pyx_n_s_encoding
+#define __pyx_n_s_errors __pyx_mstate_global->__pyx_n_s_errors
 #define __pyx_n_s_exceptions __pyx_mstate_global->__pyx_n_s_exceptions
-#define __pyx_n_b_i __pyx_mstate_global->__pyx_n_b_i
+#define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
-#define __pyx_n_s_init __pyx_mstate_global->__pyx_n_s_init
-#define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
-#define __pyx_n_s_int __pyx_mstate_global->__pyx_n_s_int
-#define __pyx_kp_u_invalid_bencoded_value_data_afte __pyx_mstate_global->__pyx_kp_u_invalid_bencoded_value_data_afte
+#define __pyx_kp_u_invalid_bencode_value_data_after __pyx_mstate_global->__pyx_kp_u_invalid_bencode_value_data_after
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
-#define __pyx_n_s_k __pyx_mstate_global->__pyx_n_s_k
-#define __pyx_n_b_l __pyx_mstate_global->__pyx_n_b_l
+#define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_length __pyx_mstate_global->__pyx_n_s_length
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
-#define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
-#define __pyx_n_s_module __pyx_mstate_global->__pyx_n_s_module
-#define __pyx_n_s_n __pyx_mstate_global->__pyx_n_s_n
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
-#define __pyx_n_s_new_f __pyx_mstate_global->__pyx_n_s_new_f
-#define __pyx_kp_u_not_a_valid_bencoded_string __pyx_mstate_global->__pyx_kp_u_not_a_valid_bencoded_string
-#define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
-#define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
-#define __pyx_n_s_r __pyx_mstate_global->__pyx_n_s_r
+#define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
+#define __pyx_kp_u_not_a_valid_bencode_bytes __pyx_mstate_global->__pyx_kp_u_not_a_valid_bencode_bytes
+#define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
+#define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
+#define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
+#define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
+#define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
+#define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
+#define __pyx_n_s_pyx_unpickle_Decoder __pyx_mstate_global->__pyx_n_s_pyx_unpickle_Decoder
+#define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
+#define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
+#define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
+#define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_return __pyx_mstate_global->__pyx_n_s_return
-#define __pyx_n_s_s __pyx_mstate_global->__pyx_n_s_s
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
-#define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
-#define __pyx_n_s_super __pyx_mstate_global->__pyx_n_s_super
+#define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
+#define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
+#define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
+#define __pyx_n_s_str_key __pyx_mstate_global->__pyx_n_s_str_key
+#define __pyx_n_u_strict __pyx_mstate_global->__pyx_n_u_strict
+#define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
-#define __pyx_n_s_to_binary __pyx_mstate_global->__pyx_n_s_to_binary
 #define __pyx_n_s_typing __pyx_mstate_global->__pyx_n_s_typing
-#define __pyx_n_s_v __pyx_mstate_global->__pyx_n_s_v
+#define __pyx_kp_u_unexpected_token __pyx_mstate_global->__pyx_kp_u_unexpected_token
+#define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
+#define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
+#define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
-#define __pyx_n_s_x __pyx_mstate_global->__pyx_n_s_x
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_2 __pyx_mstate_global->__pyx_int_2
+#define __pyx_int_27736365 __pyx_mstate_global->__pyx_int_27736365
+#define __pyx_int_148187747 __pyx_mstate_global->__pyx_int_148187747
+#define __pyx_int_211139970 __pyx_mstate_global->__pyx_int_211139970
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
-#define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
-#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
 #define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
-#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
-#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
 /* #### Code section: module_code ### */
 
-/* "bencode2/_decoder.pyx":11
+/* "bencode2/_decoder.pyx":9
+ *     str_key: bool
+ * 
+ *     def __init__(self, str_key: bool):             # <<<<<<<<<<<<<<
+ *         self.str_key = str_key
  * 
- * class BencodeDecoder:
- *     def __init__(self):             # <<<<<<<<<<<<<<
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
- *             b"l": self.decode_list,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_1__init__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_1__init__(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_self = 0;
-  #if !CYTHON_METH_FASTCALL
+static int __pyx_pw_8bencode2_8_decoder_7Decoder_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_8bencode2_8_decoder_7Decoder_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_str_key = 0;
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
+  int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_str_key,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_str_key)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 11, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 11, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
-    __pyx_v_self = values[0];
+    __pyx_v_str_key = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 11, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 9, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
-  return NULL;
+  return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder___init__(__pyx_self, __pyx_v_self);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_7Decoder___init__(((struct __pyx_obj_8bencode2_8_decoder_Decoder *)__pyx_v_self), __pyx_v_str_key);
 
   /* function exit code */
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
+static int __pyx_pf_8bencode2_8_decoder_7Decoder___init__(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_str_key) {
+  int __pyx_r;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "bencode2/_decoder.pyx":13
- *     def __init__(self):
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
- *             b"l": self.decode_list,             # <<<<<<<<<<<<<<
- *             b"i": self.decode_int,
- *             b"0": self.decode_string,
- */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(13); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_list); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_b_l, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":14
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
- *             b"l": self.decode_list,
- *             b"i": self.decode_int,             # <<<<<<<<<<<<<<
- *             b"0": self.decode_string,
- *             b"1": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_int); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_b_i, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":15
- *             b"l": self.decode_list,
- *             b"i": self.decode_int,
- *             b"0": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"1": self.decode_string,
- *             b"2": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_0, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":16
- *             b"i": self.decode_int,
- *             b"0": self.decode_string,
- *             b"1": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"2": self.decode_string,
- *             b"3": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_1, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":17
- *             b"0": self.decode_string,
- *             b"1": self.decode_string,
- *             b"2": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"3": self.decode_string,
- *             b"4": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_2, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":18
- *             b"1": self.decode_string,
- *             b"2": self.decode_string,
- *             b"3": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"4": self.decode_string,
- *             b"5": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_3, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":19
- *             b"2": self.decode_string,
- *             b"3": self.decode_string,
- *             b"4": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"5": self.decode_string,
- *             b"6": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_4, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":20
- *             b"3": self.decode_string,
- *             b"4": self.decode_string,
- *             b"5": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"6": self.decode_string,
- *             b"7": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_5, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":21
- *             b"4": self.decode_string,
- *             b"5": self.decode_string,
- *             b"6": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"7": self.decode_string,
- *             b"8": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 21, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_6, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":22
- *             b"5": self.decode_string,
- *             b"6": self.decode_string,
- *             b"7": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"8": self.decode_string,
- *             b"9": self.decode_string,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_7, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":23
- *             b"6": self.decode_string,
- *             b"7": self.decode_string,
- *             b"8": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"9": self.decode_string,
- *             b"d": self.decode_dict,
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_8, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":24
- *             b"7": self.decode_string,
- *             b"8": self.decode_string,
- *             b"9": self.decode_string,             # <<<<<<<<<<<<<<
- *             b"d": self.decode_dict,
- *         }
- */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_kp_b_9, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":25
- *             b"8": self.decode_string,
- *             b"9": self.decode_string,
- *             b"d": self.decode_dict,             # <<<<<<<<<<<<<<
- *         }
+  /* "bencode2/_decoder.pyx":10
  * 
+ *     def __init__(self, str_key: bool):
+ *         self.str_key = str_key             # <<<<<<<<<<<<<<
+ * 
+ *     def decode(self, value: bytes)-> Any:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_dict); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_b_d, __pyx_t_2) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":12
- * class BencodeDecoder:
- *     def __init__(self):
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {             # <<<<<<<<<<<<<<
- *             b"l": self.decode_list,
- *             b"i": self.decode_int,
- */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_decode_func, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_INCREF(__pyx_v_str_key);
+  __Pyx_GIVEREF(__pyx_v_str_key);
+  __Pyx_GOTREF(__pyx_v_self->str_key);
+  __Pyx_DECREF(__pyx_v_self->str_key);
+  __pyx_v_self->str_key = __pyx_v_str_key;
 
-  /* "bencode2/_decoder.pyx":11
+  /* "bencode2/_decoder.pyx":9
+ *     str_key: bool
+ * 
+ *     def __init__(self, str_key: bool):             # <<<<<<<<<<<<<<
+ *         self.str_key = str_key
  * 
- * class BencodeDecoder:
- *     def __init__(self):             # <<<<<<<<<<<<<<
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
- *             b"l": self.decode_list,
  */
 
   /* function exit code */
-  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
+  __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_decoder.pyx":28
- *         }
+/* "bencode2/_decoder.pyx":12
+ *         self.str_key = str_key
  * 
- *     def decode(self, value: bytes) -> Any:             # <<<<<<<<<<<<<<
- *         """
- *         Decode bencode formatted byte string ``value``.
+ *     def decode(self, value: bytes)-> Any:             # <<<<<<<<<<<<<<
+ *         try:
+ *             data, length = self.__decode(value, 0)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_3decode(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_7Decoder_3decode(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8bencode2_8_decoder_14BencodeDecoder_2decode, "\n        Decode bencode formatted byte string ``value``.\n\n        :param value: Bencode formatted string\n        :type value: bytes\n\n        :return: Decoded value\n        :rtype: object\n        ");
-static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_3decode = {"decode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_3decode, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_8_decoder_14BencodeDecoder_2decode};
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_3decode(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_7Decoder_3decode = {"decode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_7Decoder_3decode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_decoder_7Decoder_3decode(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
-  PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_value = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[2] = {0,0};
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("decode (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
@@ -3161,76 +3061,62 @@
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_value,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_value,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 12, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("decode", 1, 2, 2, 1); __PYX_ERR(0, 28, __pyx_L3_error)
-        }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode") < 0)) __PYX_ERR(0, 28, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode") < 0)) __PYX_ERR(0, 12, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 2)) {
+    } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_self = values[0];
-    __pyx_v_value = ((PyObject*)values[1]);
+    __pyx_v_value = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 28, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("decode", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 12, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_value), (&PyBytes_Type), 0, "value", 1))) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_2decode(__pyx_self, __pyx_v_self, __pyx_v_value);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_value), (&PyBytes_Type), 0, "value", 1))) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_7Decoder_2decode(((struct __pyx_obj_8bencode2_8_decoder_Decoder *)__pyx_v_self), __pyx_v_value);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   {
@@ -3239,1466 +3125,1970 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_2decode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
+static PyObject *__pyx_pf_8bencode2_8_decoder_7Decoder_2decode(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_value) {
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_v_length = NULL;
+  PyObject *__pyx_v_e = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
-  PyObject *(*__pyx_t_9)(PyObject *);
+  PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
-  Py_ssize_t __pyx_t_12;
-  int __pyx_t_13;
+  int __pyx_t_12;
+  char const *__pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
+  PyObject *__pyx_t_15 = NULL;
+  PyObject *__pyx_t_16 = NULL;
+  PyObject *__pyx_t_17 = NULL;
+  PyObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  Py_ssize_t __pyx_t_20;
+  int __pyx_t_21;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("decode", 0);
-  __Pyx_INCREF(__pyx_v_value);
+  __Pyx_RefNannySetupContext("decode", 1);
 
-  /* "bencode2/_decoder.pyx":38
- *         :rtype: object
- *         """
+  /* "bencode2/_decoder.pyx":13
+ * 
+ *     def decode(self, value: bytes)-> Any:
  *         try:             # <<<<<<<<<<<<<<
- *             value = to_binary(value)
- *             data, length = self.decode_func[value[0:1]](value, 0)
+ *             data, length = self.__decode(value, 0)
+ *         except (IndexError, KeyError, TypeError, ValueError) as e:
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "bencode2/_decoder.pyx":39
- *         """
- *         try:
- *             value = to_binary(value)             # <<<<<<<<<<<<<<
- *             data, length = self.decode_func[value[0:1]](value, 0)
- *         except (IndexError, KeyError, TypeError, ValueError):
- */
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_to_binary); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = NULL;
-      __pyx_t_7 = 0;
-      #if CYTHON_UNPACK_METHODS
-      if (unlikely(PyMethod_Check(__pyx_t_5))) {
-        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
-        if (likely(__pyx_t_6)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-          __Pyx_INCREF(__pyx_t_6);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_5, function);
-          __pyx_t_7 = 1;
-        }
-      }
-      #endif
-      {
-        PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_v_value};
-        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      }
-      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_4))) __PYX_ERR(0, 39, __pyx_L3_error)
-      __Pyx_DECREF_SET(__pyx_v_value, ((PyObject*)__pyx_t_4));
-      __pyx_t_4 = 0;
-
-      /* "bencode2/_decoder.pyx":40
+      /* "bencode2/_decoder.pyx":14
+ *     def decode(self, value: bytes)-> Any:
  *         try:
- *             value = to_binary(value)
- *             data, length = self.decode_func[value[0:1]](value, 0)             # <<<<<<<<<<<<<<
- *         except (IndexError, KeyError, TypeError, ValueError):
- *             raise BencodeDecodeError("not a valid bencoded string")
- */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_func); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__pyx_v_value == Py_None)) {
-        PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 40, __pyx_L3_error)
-      }
-      __pyx_t_6 = PySequence_GetSlice(__pyx_v_value, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 40, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 40, __pyx_L3_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = NULL;
-      __pyx_t_7 = 0;
-      #if CYTHON_UNPACK_METHODS
-      if (unlikely(PyMethod_Check(__pyx_t_8))) {
-        __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_8);
-        if (likely(__pyx_t_6)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
-          __Pyx_INCREF(__pyx_t_6);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_8, function);
-          __pyx_t_7 = 1;
-        }
-      }
-      #endif
-      {
-        PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_v_value, __pyx_int_0};
-        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
-        __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      }
-      if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
+ *             data, length = self.__decode(value, 0)             # <<<<<<<<<<<<<<
+ *         except (IndexError, KeyError, TypeError, ValueError) as e:
+ *             raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e
+ */
+      if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 14, __pyx_L3_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode(__pyx_v_self, __pyx_v_value, ((PyObject*)__pyx_int_0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      if (likely(__pyx_t_4 != Py_None)) {
         PyObject* sequence = __pyx_t_4;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 40, __pyx_L3_error)
+          __PYX_ERR(0, 14, __pyx_L3_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        if (likely(PyTuple_CheckExact(sequence))) {
-          __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
-          __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
-        } else {
-          __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
-          __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
-        }
-        __Pyx_INCREF(__pyx_t_8);
+        __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
+        __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         #else
-        __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 40, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 40, __pyx_L3_error)
+        __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 14, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 14, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else {
-        Py_ssize_t index = -1;
-        __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L3_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        __pyx_t_9 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5);
-        index = 0; __pyx_t_8 = __pyx_t_9(__pyx_t_5); if (unlikely(!__pyx_t_8)) goto __pyx_L9_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_8);
-        index = 1; __pyx_t_6 = __pyx_t_9(__pyx_t_5); if (unlikely(!__pyx_t_6)) goto __pyx_L9_unpacking_failed;
-        __Pyx_GOTREF(__pyx_t_6);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_5), 2) < 0) __PYX_ERR(0, 40, __pyx_L3_error)
-        __pyx_t_9 = NULL;
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        goto __pyx_L10_unpacking_done;
-        __pyx_L9_unpacking_failed:;
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __pyx_t_9 = NULL;
-        if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 40, __pyx_L3_error)
-        __pyx_L10_unpacking_done:;
+        __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 14, __pyx_L3_error)
       }
-      __pyx_v_data = __pyx_t_8;
-      __pyx_t_8 = 0;
+      __pyx_v_data = __pyx_t_5;
+      __pyx_t_5 = 0;
       __pyx_v_length = __pyx_t_6;
       __pyx_t_6 = 0;
 
-      /* "bencode2/_decoder.pyx":38
- *         :rtype: object
- *         """
+      /* "bencode2/_decoder.pyx":13
+ * 
+ *     def decode(self, value: bytes)-> Any:
  *         try:             # <<<<<<<<<<<<<<
- *             value = to_binary(value)
- *             data, length = self.decode_func[value[0:1]](value, 0)
+ *             data, length = self.__decode(value, 0)
+ *         except (IndexError, KeyError, TypeError, ValueError) as e:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "bencode2/_decoder.pyx":41
- *             value = to_binary(value)
- *             data, length = self.decode_func[value[0:1]](value, 0)
- *         except (IndexError, KeyError, TypeError, ValueError):             # <<<<<<<<<<<<<<
- *             raise BencodeDecodeError("not a valid bencoded string")
+    /* "bencode2/_decoder.pyx":15
+ *         try:
+ *             data, length = self.__decode(value, 0)
+ *         except (IndexError, KeyError, TypeError, ValueError) as e:             # <<<<<<<<<<<<<<
+ *             raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e
  * 
  */
     __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_IndexError) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError) || __Pyx_PyErr_ExceptionMatches(__pyx_builtin_ValueError);
     if (__pyx_t_7) {
-      __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_8) < 0) __PYX_ERR(0, 41, __pyx_L5_except_error)
+      __Pyx_AddTraceback("bencode2._decoder.Decoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_5) < 0) __PYX_ERR(0, 15, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_6);
-      __Pyx_XGOTREF(__pyx_t_8);
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_6);
+      __pyx_v_e = __pyx_t_6;
+      /*try:*/ {
 
-      /* "bencode2/_decoder.pyx":42
- *             data, length = self.decode_func[value[0:1]](value, 0)
- *         except (IndexError, KeyError, TypeError, ValueError):
- *             raise BencodeDecodeError("not a valid bencoded string")             # <<<<<<<<<<<<<<
+        /* "bencode2/_decoder.pyx":16
+ *             data, length = self.__decode(value, 0)
+ *         except (IndexError, KeyError, TypeError, ValueError) as e:
+ *             raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e             # <<<<<<<<<<<<<<
  * 
  *         if length != len(value):
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 42, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_11 = NULL;
-      __pyx_t_7 = 0;
-      #if CYTHON_UNPACK_METHODS
-      if (unlikely(PyMethod_Check(__pyx_t_10))) {
-        __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
-        if (likely(__pyx_t_11)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
-          __Pyx_INCREF(__pyx_t_11);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_10, function);
-          __pyx_t_7 = 1;
+        __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 16, __pyx_L14_error)
+        __Pyx_GOTREF(__pyx_t_9);
+        __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_v_e, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 16, __pyx_L14_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_not_a_valid_bencode_bytes, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 16, __pyx_L14_error)
+        __Pyx_GOTREF(__pyx_t_11);
+        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __pyx_t_10 = NULL;
+        __pyx_t_7 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_9))) {
+          __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+          if (likely(__pyx_t_10)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+            __Pyx_INCREF(__pyx_t_10);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_9, function);
+            __pyx_t_7 = 1;
+          }
         }
+        #endif
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_11};
+          __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 16, __pyx_L14_error)
+          __Pyx_GOTREF(__pyx_t_8);
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+        }
+        __Pyx_Raise(__pyx_t_8, 0, 0, __pyx_v_e);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __PYX_ERR(0, 16, __pyx_L14_error)
       }
-      #endif
-      {
-        PyObject *__pyx_callargs[2] = {__pyx_t_11, __pyx_kp_u_not_a_valid_bencoded_string};
-        __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-        __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L5_except_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+
+      /* "bencode2/_decoder.pyx":15
+ *         try:
+ *             data, length = self.__decode(value, 0)
+ *         except (IndexError, KeyError, TypeError, ValueError) as e:             # <<<<<<<<<<<<<<
+ *             raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e
+ * 
+ */
+      /*finally:*/ {
+        __pyx_L14_error:;
+        /*exception exit:*/{
+          __Pyx_PyThreadState_declare
+          __Pyx_PyThreadState_assign
+          __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
+          __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+          __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+          if (PY_MAJOR_VERSION >= 3) __Pyx_ExceptionSwap(&__pyx_t_17, &__pyx_t_18, &__pyx_t_19);
+          if ((PY_MAJOR_VERSION < 3) || unlikely(__Pyx_GetException(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16) < 0)) __Pyx_ErrFetch(&__pyx_t_14, &__pyx_t_15, &__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_14);
+          __Pyx_XGOTREF(__pyx_t_15);
+          __Pyx_XGOTREF(__pyx_t_16);
+          __Pyx_XGOTREF(__pyx_t_17);
+          __Pyx_XGOTREF(__pyx_t_18);
+          __Pyx_XGOTREF(__pyx_t_19);
+          __pyx_t_7 = __pyx_lineno; __pyx_t_12 = __pyx_clineno; __pyx_t_13 = __pyx_filename;
+          {
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
+          }
+          if (PY_MAJOR_VERSION >= 3) {
+            __Pyx_XGIVEREF(__pyx_t_17);
+            __Pyx_XGIVEREF(__pyx_t_18);
+            __Pyx_XGIVEREF(__pyx_t_19);
+            __Pyx_ExceptionReset(__pyx_t_17, __pyx_t_18, __pyx_t_19);
+          }
+          __Pyx_XGIVEREF(__pyx_t_14);
+          __Pyx_XGIVEREF(__pyx_t_15);
+          __Pyx_XGIVEREF(__pyx_t_16);
+          __Pyx_ErrRestore(__pyx_t_14, __pyx_t_15, __pyx_t_16);
+          __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0; __pyx_t_18 = 0; __pyx_t_19 = 0;
+          __pyx_lineno = __pyx_t_7; __pyx_clineno = __pyx_t_12; __pyx_filename = __pyx_t_13;
+          goto __pyx_L5_except_error;
+        }
       }
-      __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 42, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "bencode2/_decoder.pyx":38
- *         :rtype: object
- *         """
+    /* "bencode2/_decoder.pyx":13
+ * 
+ *     def decode(self, value: bytes)-> Any:
  *         try:             # <<<<<<<<<<<<<<
- *             value = to_binary(value)
- *             data, length = self.decode_func[value[0:1]](value, 0)
+ *             data, length = self.__decode(value, 0)
+ *         except (IndexError, KeyError, TypeError, ValueError) as e:
  */
     __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "bencode2/_decoder.pyx":44
- *             raise BencodeDecodeError("not a valid bencoded string")
+  /* "bencode2/_decoder.pyx":18
+ *             raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e
  * 
  *         if length != len(value):             # <<<<<<<<<<<<<<
- *             raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")
+ *             raise BencodeDecodeError("invalid bencode value (data after valid prefix)")
  * 
  */
-  if (unlikely(__pyx_v_value == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 44, __pyx_L1_error)
-  }
-  __pyx_t_12 = __Pyx_PyBytes_GET_SIZE(__pyx_v_value); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
-  __pyx_t_8 = PyInt_FromSsize_t(__pyx_t_12); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_6 = PyObject_RichCompare(__pyx_v_length, __pyx_t_8, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 44, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __pyx_t_13 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_13 < 0))) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_20 = __Pyx_PyBytes_GET_SIZE(__pyx_v_value); if (unlikely(__pyx_t_20 == ((Py_ssize_t)-1))) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_5 = PyInt_FromSsize_t(__pyx_t_20); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = PyObject_RichCompare(__pyx_v_length, __pyx_t_5, Py_NE); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_21 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_21 < 0))) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(__pyx_t_13)) {
+  if (unlikely(__pyx_t_21)) {
 
-    /* "bencode2/_decoder.pyx":45
+    /* "bencode2/_decoder.pyx":19
  * 
  *         if length != len(value):
- *             raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")             # <<<<<<<<<<<<<<
+ *             raise BencodeDecodeError("invalid bencode value (data after valid prefix)")             # <<<<<<<<<<<<<<
  * 
  *         return data
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 45, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_4 = NULL;
-    __pyx_t_7 = 0;
+    __pyx_t_12 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_8))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
+    if (unlikely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_8, function);
-        __pyx_t_7 = 1;
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_12 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_u_invalid_bencoded_value_data_afte};
-      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+      PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_u_invalid_bencode_value_data_after};
+      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_12, 1+__pyx_t_12);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 45, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 19, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 45, __pyx_L1_error)
+    __PYX_ERR(0, 19, __pyx_L1_error)
 
-    /* "bencode2/_decoder.pyx":44
- *             raise BencodeDecodeError("not a valid bencoded string")
+    /* "bencode2/_decoder.pyx":18
+ *             raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e
  * 
  *         if length != len(value):             # <<<<<<<<<<<<<<
- *             raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")
+ *             raise BencodeDecodeError("invalid bencode value (data after valid prefix)")
  * 
  */
   }
 
-  /* "bencode2/_decoder.pyx":47
- *             raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")
+  /* "bencode2/_decoder.pyx":21
+ *             raise BencodeDecodeError("invalid bencode value (data after valid prefix)")
  * 
  *         return data             # <<<<<<<<<<<<<<
  * 
- *     def decode_int(self, x, index: int):
+ *     cdef tuple[Any, int] __decode(self, x: bytes, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "bencode2/_decoder.pyx":28
- *         }
+  /* "bencode2/_decoder.pyx":12
+ *         self.str_key = str_key
  * 
- *     def decode(self, value: bytes) -> Any:             # <<<<<<<<<<<<<<
- *         """
- *         Decode bencode formatted byte string ``value``.
+ *     def decode(self, value: bytes)-> Any:             # <<<<<<<<<<<<<<
+ *         try:
+ *             data, length = self.__decode(value, 0)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder.decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_length);
-  __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_decoder.pyx":49
+/* "bencode2/_decoder.pyx":23
  *         return data
  * 
- *     def decode_int(self, x, index: int):             # <<<<<<<<<<<<<<
- *         index += 1
- *         new_f = x.index(b"e", index)
+ *     cdef tuple[Any, int] __decode(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         if x[index] == c'l':
+ *             return self.__decode_list(x, index)
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_5decode_int(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_5decode_int = {"decode_int", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_5decode_int, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_5decode_int(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  CYTHON_UNUSED PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_x = 0;
-  PyObject *__pyx_v_index = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[3] = {0,0,0};
+static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  __pyx_ctuple_int__and_int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  Py_ssize_t __pyx_t_7;
+  Py_UCS4 __pyx_t_8;
+  PyObject *__pyx_t_9 = NULL;
+  Py_ssize_t __pyx_t_10;
+  Py_ssize_t __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  PyObject *__pyx_t_13 = NULL;
+  int __pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("decode_int (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_x,&__pyx_n_s_index,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("decode_int", 1, 3, 3, 1); __PYX_ERR(0, 49, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("decode_int", 1, 3, 3, 2); __PYX_ERR(0, 49, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_int") < 0)) __PYX_ERR(0, 49, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 3)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+  __Pyx_RefNannySetupContext("_Decoder__decode", 1);
+
+  /* "bencode2/_decoder.pyx":24
+ * 
+ *     cdef tuple[Any, int] __decode(self, x: bytes, index: int):
+ *         if x[index] == c'l':             # <<<<<<<<<<<<<<
+ *             return self.__decode_list(x, index)
+ *         if x[index] == c'i':
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyInt_From_char('l'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__pyx_t_4) {
+
+    /* "bencode2/_decoder.pyx":25
+ *     cdef tuple[Any, int] __decode(self, x: bytes, index: int):
+ *         if x[index] == c'l':
+ *             return self.__decode_list(x, index)             # <<<<<<<<<<<<<<
+ *         if x[index] == c'i':
+ *             return self.__decode_int(x, index)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_3 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode_list(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_r = ((PyObject*)__pyx_t_3);
+    __pyx_t_3 = 0;
+    goto __pyx_L0;
+
+    /* "bencode2/_decoder.pyx":24
+ * 
+ *     cdef tuple[Any, int] __decode(self, x: bytes, index: int):
+ *         if x[index] == c'l':             # <<<<<<<<<<<<<<
+ *             return self.__decode_list(x, index)
+ *         if x[index] == c'i':
+ */
+  }
+
+  /* "bencode2/_decoder.pyx":26
+ *         if x[index] == c'l':
+ *             return self.__decode_list(x, index)
+ *         if x[index] == c'i':             # <<<<<<<<<<<<<<
+ *             return self.__decode_int(x, index)
+ *         if x[index] == c'd':
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyInt_From_char('i'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_4) {
+
+    /* "bencode2/_decoder.pyx":27
+ *             return self.__decode_list(x, index)
+ *         if x[index] == c'i':
+ *             return self.__decode_int(x, index)             # <<<<<<<<<<<<<<
+ *         if x[index] == c'd':
+ *             return self.__decode_dict(x, index)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_5 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode_int(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert__to_py___pyx_ctuple_int__and_int(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    if (!(likely(PyTuple_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_1))) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_r = ((PyObject*)__pyx_t_1);
+    __pyx_t_1 = 0;
+    goto __pyx_L0;
+
+    /* "bencode2/_decoder.pyx":26
+ *         if x[index] == c'l':
+ *             return self.__decode_list(x, index)
+ *         if x[index] == c'i':             # <<<<<<<<<<<<<<
+ *             return self.__decode_int(x, index)
+ *         if x[index] == c'd':
+ */
+  }
+
+  /* "bencode2/_decoder.pyx":28
+ *         if x[index] == c'i':
+ *             return self.__decode_int(x, index)
+ *         if x[index] == c'd':             # <<<<<<<<<<<<<<
+ *             return self.__decode_dict(x, index)
+ *         if c'0' <= x[index] <= c'9':
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyInt_From_char('d'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 28, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (__pyx_t_4) {
+
+    /* "bencode2/_decoder.pyx":29
+ *             return self.__decode_int(x, index)
+ *         if x[index] == c'd':
+ *             return self.__decode_dict(x, index)             # <<<<<<<<<<<<<<
+ *         if c'0' <= x[index] <= c'9':
+ *             return self.__decode_str(x, index)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_3 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode_dict(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_r = ((PyObject*)__pyx_t_3);
+    __pyx_t_3 = 0;
+    goto __pyx_L0;
+
+    /* "bencode2/_decoder.pyx":28
+ *         if x[index] == c'i':
+ *             return self.__decode_int(x, index)
+ *         if x[index] == c'd':             # <<<<<<<<<<<<<<
+ *             return self.__decode_dict(x, index)
+ *         if c'0' <= x[index] <= c'9':
+ */
+  }
+
+  /* "bencode2/_decoder.pyx":30
+ *         if x[index] == c'd':
+ *             return self.__decode_dict(x, index)
+ *         if c'0' <= x[index] <= c'9':             # <<<<<<<<<<<<<<
+ *             return self.__decode_str(x, index)
+ * 
+ */
+  __pyx_t_3 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_3, __pyx_t_2, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
+    __Pyx_DECREF(__pyx_t_1);
+    __pyx_t_6 = __Pyx_PyInt_From_char('9'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 30, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_t_6, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_4) {
+
+    /* "bencode2/_decoder.pyx":31
+ *             return self.__decode_dict(x, index)
+ *         if c'0' <= x[index] <= c'9':
+ *             return self.__decode_str(x, index)             # <<<<<<<<<<<<<<
+ * 
+ *         raise BencodeDecodeError(
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_1 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode_str(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 31, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_r = ((PyObject*)__pyx_t_1);
+    __pyx_t_1 = 0;
+    goto __pyx_L0;
+
+    /* "bencode2/_decoder.pyx":30
+ *         if x[index] == c'd':
+ *             return self.__decode_dict(x, index)
+ *         if c'0' <= x[index] <= c'9':             # <<<<<<<<<<<<<<
+ *             return self.__decode_str(x, index)
+ * 
+ */
+  }
+
+  /* "bencode2/_decoder.pyx":33
+ *             return self.__decode_str(x, index)
+ * 
+ *         raise BencodeDecodeError(             # <<<<<<<<<<<<<<
+ *             f"unexpected token {x[index:index + 1]} at index {index}")
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+
+  /* "bencode2/_decoder.pyx":34
+ * 
+ *         raise BencodeDecodeError(
+ *             f"unexpected token {x[index:index + 1]} at index {index}")             # <<<<<<<<<<<<<<
+ * 
+ *     cdef tuple[int, int] __decode_int(self, x: bytes, index: int):
+ */
+  __pyx_t_3 = PyTuple_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_7 = 0;
+  __pyx_t_8 = 127;
+  __Pyx_INCREF(__pyx_kp_u_unexpected_token);
+  __pyx_t_7 += 17;
+  __Pyx_GIVEREF(__pyx_kp_u_unexpected_token);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_kp_u_unexpected_token);
+  __Pyx_INCREF(__pyx_v_index);
+  __pyx_t_9 = __pyx_v_index;
+  __pyx_t_4 = (__pyx_t_9 == ((PyObject*)Py_None));
+  if (__pyx_t_4) {
+    __pyx_t_10 = 0;
+  } else {
+    __pyx_t_11 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_11 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_10 = __pyx_t_11;
+  }
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+  __pyx_t_6 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_4 = (__pyx_t_6 == Py_None);
+  if (__pyx_t_4) {
+    __pyx_t_11 = PY_SSIZE_T_MAX;
+  } else {
+    __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_11 = __pyx_t_12;
+  }
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = PySequence_GetSlice(__pyx_v_x, __pyx_t_10, __pyx_t_11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_t_6, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_8 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) > __pyx_t_8) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) : __pyx_t_8;
+  __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_13);
+  __Pyx_GIVEREF(__pyx_t_13);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_13);
+  __pyx_t_13 = 0;
+  __Pyx_INCREF(__pyx_kp_u_at_index);
+  __pyx_t_7 += 10;
+  __Pyx_GIVEREF(__pyx_kp_u_at_index);
+  PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_kp_u_at_index);
+  __pyx_t_13 = __Pyx_PyObject_FormatSimple(__pyx_v_index, __pyx_empty_unicode); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __pyx_t_8 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) > __pyx_t_8) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_13) : __pyx_t_8;
+  __pyx_t_7 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_13);
+  __Pyx_GIVEREF(__pyx_t_13);
+  PyTuple_SET_ITEM(__pyx_t_3, 3, __pyx_t_13);
+  __pyx_t_13 = 0;
+  __pyx_t_13 = __Pyx_PyUnicode_Join(__pyx_t_3, 4, __pyx_t_7, __pyx_t_8); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_13);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = NULL;
+  __pyx_t_14 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_14 = 1;
     }
-    __pyx_v_self = values[0];
-    __pyx_v_x = values[1];
-    __pyx_v_index = ((PyObject*)values[2]);
   }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode_int", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 49, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
+  #endif
   {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_13};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_14, 1+__pyx_t_14);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_index), (&PyInt_Type), 0, "index", 1))) __PYX_ERR(0, 49, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_4decode_int(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
+  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __PYX_ERR(0, 33, __pyx_L1_error)
+
+  /* "bencode2/_decoder.pyx":23
+ *         return data
+ * 
+ *     cdef tuple[Any, int] __decode(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         if x[index] == c'l':
+ *             return self.__decode_list(x, index)
+ */
 
   /* function exit code */
-  goto __pyx_L0;
   __pyx_L1_error:;
-  __pyx_r = NULL;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_13);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
+  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_4decode_int(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+/* "bencode2/_decoder.pyx":36
+ *             f"unexpected token {x[index:index + 1]} at index {index}")
+ * 
+ *     cdef tuple[int, int] __decode_int(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         index += 1
+ *         new_f = x.index(b"e", index)
+ */
+
+static __pyx_ctuple_int__and_int __pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_int(CYTHON_UNUSED struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
   PyObject *__pyx_v_new_f = NULL;
   PyObject *__pyx_v_n = NULL;
-  PyObject *__pyx_r = NULL;
+  __pyx_ctuple_int__and_int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
+  Py_ssize_t __pyx_t_5;
+  Py_ssize_t __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
+  int __pyx_t_10;
+  int __pyx_t_11;
+  __pyx_ctuple_int__and_int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("decode_int", 0);
+  __Pyx_RefNannySetupContext("_Decoder__decode_int", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "bencode2/_decoder.pyx":50
+  /* "bencode2/_decoder.pyx":37
  * 
- *     def decode_int(self, x, index: int):
+ *     cdef tuple[int, int] __decode_int(self, x: bytes, index: int):
  *         index += 1             # <<<<<<<<<<<<<<
  *         new_f = x.index(b"e", index)
  *         n = int(x[index:new_f])
  */
-  __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 50, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
   __pyx_t_1 = 0;
 
-  /* "bencode2/_decoder.pyx":51
- *     def decode_int(self, x, index: int):
+  /* "bencode2/_decoder.pyx":38
+ *     cdef tuple[int, int] __decode_int(self, x: bytes, index: int):
  *         index += 1
  *         new_f = x.index(b"e", index)             # <<<<<<<<<<<<<<
  *         n = int(x[index:new_f])
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  __pyx_t_4 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_4 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_n_b_e, __pyx_v_index};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  }
+  __pyx_t_1 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_index, __pyx_v_x, __pyx_n_b_e, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_new_f = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "bencode2/_decoder.pyx":52
+  /* "bencode2/_decoder.pyx":39
  *         index += 1
  *         new_f = x.index(b"e", index)
  *         n = int(x[index:new_f])             # <<<<<<<<<<<<<<
  * 
- *         if x[index : index + 1] == b"-":
+ *         if x[index] == c'-':
  */
-  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_v_new_f, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_v_index);
+  __pyx_t_2 = __pyx_v_index;
+  __pyx_t_4 = (__pyx_t_2 == ((PyObject*)Py_None));
+  if (__pyx_t_4) {
+    __pyx_t_3 = 0;
+  } else {
+    __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_3 = __pyx_t_5;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_INCREF(__pyx_v_new_f);
+  __pyx_t_1 = __pyx_v_new_f;
+  __pyx_t_4 = (__pyx_t_1 == Py_None);
+  if (__pyx_t_4) {
+    __pyx_t_5 = PY_SSIZE_T_MAX;
+  } else {
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 39, __pyx_L1_error)
+    __pyx_t_5 = __pyx_t_6;
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PySequence_GetSlice(__pyx_v_x, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_7 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_n = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_v_n = __pyx_t_7;
+  __pyx_t_7 = 0;
 
-  /* "bencode2/_decoder.pyx":54
+  /* "bencode2/_decoder.pyx":41
  *         n = int(x[index:new_f])
  * 
- *         if x[index : index + 1] == b"-":             # <<<<<<<<<<<<<<
- *             if x[index + 1 : index + 2] == b"0":
+ *         if x[index] == c'-':             # <<<<<<<<<<<<<<
+ *             if x[index + 1: index + 2] == b"0":
  *                 raise ValueError
  */
-  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_1 = __Pyx_PyInt_From_char('-'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = (__Pyx_PyBytes_Equals(__pyx_t_1, __pyx_kp_b_, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__pyx_t_5) {
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 41, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (__pyx_t_4) {
 
-    /* "bencode2/_decoder.pyx":55
+    /* "bencode2/_decoder.pyx":42
  * 
- *         if x[index : index + 1] == b"-":
- *             if x[index + 1 : index + 2] == b"0":             # <<<<<<<<<<<<<<
+ *         if x[index] == c'-':
+ *             if x[index + 1: index + 2] == b"0":             # <<<<<<<<<<<<<<
  *                 raise ValueError
- *         elif x[index : index + 1] == b"0" and new_f != index + 1:
+ *         elif x[index] == c'0' and new_f != index + 1:
  */
-    __pyx_t_1 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_t_1, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_5 = (__Pyx_PyBytes_Equals(__pyx_t_3, __pyx_kp_b_0, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 55, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(__pyx_t_5)) {
-
-      /* "bencode2/_decoder.pyx":56
- *         if x[index : index + 1] == b"-":
- *             if x[index + 1 : index + 2] == b"0":
+    __pyx_t_8 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_4 = (__pyx_t_8 == Py_None);
+    if (__pyx_t_4) {
+      __pyx_t_5 = 0;
+    } else {
+      __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_t_8); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L1_error)
+      __pyx_t_5 = __pyx_t_3;
+    }
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_8 = PyNumber_Add(__pyx_v_index, __pyx_int_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_4 = (__pyx_t_8 == Py_None);
+    if (__pyx_t_4) {
+      __pyx_t_3 = PY_SSIZE_T_MAX;
+    } else {
+      __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_8); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 42, __pyx_L1_error)
+      __pyx_t_3 = __pyx_t_6;
+    }
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_8 = PySequence_GetSlice(__pyx_v_x, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_4 = (__Pyx_PyBytes_Equals(__pyx_t_8, __pyx_kp_b_0, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 42, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(__pyx_t_4)) {
+
+      /* "bencode2/_decoder.pyx":43
+ *         if x[index] == c'-':
+ *             if x[index + 1: index + 2] == b"0":
  *                 raise ValueError             # <<<<<<<<<<<<<<
- *         elif x[index : index + 1] == b"0" and new_f != index + 1:
+ *         elif x[index] == c'0' and new_f != index + 1:
  *             raise ValueError
  */
       __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
-      __PYX_ERR(0, 56, __pyx_L1_error)
+      __PYX_ERR(0, 43, __pyx_L1_error)
 
-      /* "bencode2/_decoder.pyx":55
+      /* "bencode2/_decoder.pyx":42
  * 
- *         if x[index : index + 1] == b"-":
- *             if x[index + 1 : index + 2] == b"0":             # <<<<<<<<<<<<<<
+ *         if x[index] == c'-':
+ *             if x[index + 1: index + 2] == b"0":             # <<<<<<<<<<<<<<
  *                 raise ValueError
- *         elif x[index : index + 1] == b"0" and new_f != index + 1:
+ *         elif x[index] == c'0' and new_f != index + 1:
  */
     }
 
-    /* "bencode2/_decoder.pyx":54
+    /* "bencode2/_decoder.pyx":41
  *         n = int(x[index:new_f])
  * 
- *         if x[index : index + 1] == b"-":             # <<<<<<<<<<<<<<
- *             if x[index + 1 : index + 2] == b"0":
+ *         if x[index] == c'-':             # <<<<<<<<<<<<<<
+ *             if x[index + 1: index + 2] == b"0":
  *                 raise ValueError
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_decoder.pyx":57
- *             if x[index + 1 : index + 2] == b"0":
+  /* "bencode2/_decoder.pyx":44
+ *             if x[index + 1: index + 2] == b"0":
  *                 raise ValueError
- *         elif x[index : index + 1] == b"0" and new_f != index + 1:             # <<<<<<<<<<<<<<
+ *         elif x[index] == c'0' and new_f != index + 1:             # <<<<<<<<<<<<<<
  *             raise ValueError
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_3, NULL, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_kp_b_0, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__pyx_t_6) {
+  __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_1 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_7 = PyObject_RichCompare(__pyx_t_8, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (__pyx_t_9) {
   } else {
-    __pyx_t_5 = __pyx_t_6;
+    __pyx_t_4 = __pyx_t_9;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_v_new_f, __pyx_t_2, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 57, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __pyx_t_6;
+  __pyx_t_7 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_new_f, __pyx_t_7, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_4 = __pyx_t_9;
   __pyx_L5_bool_binop_done:;
-  if (unlikely(__pyx_t_5)) {
+  if (unlikely(__pyx_t_4)) {
 
-    /* "bencode2/_decoder.pyx":58
+    /* "bencode2/_decoder.pyx":45
  *                 raise ValueError
- *         elif x[index : index + 1] == b"0" and new_f != index + 1:
+ *         elif x[index] == c'0' and new_f != index + 1:
  *             raise ValueError             # <<<<<<<<<<<<<<
  * 
  *         return n, new_f + 1
  */
     __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
-    __PYX_ERR(0, 58, __pyx_L1_error)
+    __PYX_ERR(0, 45, __pyx_L1_error)
 
-    /* "bencode2/_decoder.pyx":57
- *             if x[index + 1 : index + 2] == b"0":
+    /* "bencode2/_decoder.pyx":44
+ *             if x[index + 1: index + 2] == b"0":
  *                 raise ValueError
- *         elif x[index : index + 1] == b"0" and new_f != index + 1:             # <<<<<<<<<<<<<<
+ *         elif x[index] == c'0' and new_f != index + 1:             # <<<<<<<<<<<<<<
  *             raise ValueError
  * 
  */
   }
   __pyx_L3:;
 
-  /* "bencode2/_decoder.pyx":60
+  /* "bencode2/_decoder.pyx":47
  *             raise ValueError
  * 
  *         return n, new_f + 1             # <<<<<<<<<<<<<<
  * 
- *     def decode_string(self, x, index: int):
+ *     cdef tuple[list, int] __decode_list(self, x: bytes, index: int):
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_v_new_f, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_v_n);
-  __Pyx_GIVEREF(__pyx_v_n);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_n)) __PYX_ERR(0, 60, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3)) __PYX_ERR(0, 60, __pyx_L1_error);
-  __pyx_t_3 = 0;
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_10 = __Pyx_PyInt_As_int(__pyx_v_n); if (unlikely((__pyx_t_10 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_new_f, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_12.f0 = __pyx_t_10;
+  __pyx_t_12.f1 = __pyx_t_11;
+  __pyx_r = __pyx_t_12;
   goto __pyx_L0;
 
-  /* "bencode2/_decoder.pyx":49
- *         return data
+  /* "bencode2/_decoder.pyx":36
+ *             f"unexpected token {x[index:index + 1]} at index {index}")
  * 
- *     def decode_int(self, x, index: int):             # <<<<<<<<<<<<<<
+ *     cdef tuple[int, int] __decode_int(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         index += 1
  *         new_f = x.index(b"e", index)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_new_f);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XDECREF(__pyx_v_index);
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_decoder.pyx":62
+/* "bencode2/_decoder.pyx":49
  *         return n, new_f + 1
  * 
- *     def decode_string(self, x, index: int):             # <<<<<<<<<<<<<<
- *         """Decode torrent bencoded 'string' in x starting at f."""
- *         colon = x.index(b":", index)
+ *     cdef tuple[list, int] __decode_list(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         r, index = [], index + 1
+ * 
  */
 
-/* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_7decode_string(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8bencode2_8_decoder_14BencodeDecoder_6decode_string, "Decode torrent bencoded 'string' in x starting at f.");
-static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_7decode_string = {"decode_string", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_7decode_string, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_8_decoder_14BencodeDecoder_6decode_string};
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_7decode_string(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  CYTHON_UNUSED PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_x = 0;
-  PyObject *__pyx_v_index = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[3] = {0,0,0};
+static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_list(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+  PyObject *__pyx_v_r = NULL;
+  PyObject *__pyx_v_v = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("decode_string (wrapper)", 0);
-  #if !CYTHON_METH_FASTCALL
-  #if CYTHON_ASSUME_SAFE_MACROS
-  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #else
-  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
-  #endif
-  #endif
-  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_x,&__pyx_n_s_index,0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("decode_string", 1, 3, 3, 1); __PYX_ERR(0, 62, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("decode_string", 1, 3, 3, 2); __PYX_ERR(0, 62, __pyx_L3_error)
-        }
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_string") < 0)) __PYX_ERR(0, 62, __pyx_L3_error)
+  __Pyx_RefNannySetupContext("_Decoder__decode_list", 0);
+  __Pyx_INCREF(__pyx_v_index);
+
+  /* "bencode2/_decoder.pyx":50
+ * 
+ *     cdef tuple[list, int] __decode_list(self, x: bytes, index: int):
+ *         r, index = [], index + 1             # <<<<<<<<<<<<<<
+ * 
+ *         while x[index] != c'e':
+ */
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_v_r = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+  __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_2));
+  __pyx_t_2 = 0;
+
+  /* "bencode2/_decoder.pyx":52
+ *         r, index = [], index + 1
+ * 
+ *         while x[index] != c'e':             # <<<<<<<<<<<<<<
+ *             v, index = self.__decode(x, index)
+ *             r.append(v)
+ */
+  while (1) {
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_char('e'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 52, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!__pyx_t_4) break;
+
+    /* "bencode2/_decoder.pyx":53
+ * 
+ *         while x[index] != c'e':
+ *             v, index = self.__decode(x, index)             # <<<<<<<<<<<<<<
+ *             r.append(v)
+ * 
+ */
+    __pyx_t_3 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    if (likely(__pyx_t_3 != Py_None)) {
+      PyObject* sequence = __pyx_t_3;
+      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+      if (unlikely(size != 2)) {
+        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+        __PYX_ERR(0, 53, __pyx_L1_error)
       }
-    } else if (unlikely(__pyx_nargs != 3)) {
-      goto __pyx_L5_argtuple_error;
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
+      __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_2);
+      #else
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      #endif
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-    }
-    __pyx_v_self = values[0];
-    __pyx_v_x = values[1];
-    __pyx_v_index = ((PyObject*)values[2]);
-  }
-  goto __pyx_L6_skip;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode_string", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 62, __pyx_L3_error)
-  __pyx_L6_skip:;
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 53, __pyx_L1_error)
     }
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_1);
+    __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_2));
+    __pyx_t_2 = 0;
+
+    /* "bencode2/_decoder.pyx":54
+ *         while x[index] != c'e':
+ *             v, index = self.__decode(x, index)
+ *             r.append(v)             # <<<<<<<<<<<<<<
+ * 
+ *         return r, index + 1
+ */
+    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_r, __pyx_v_v); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 54, __pyx_L1_error)
   }
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_index), (&PyInt_Type), 0, "index", 1))) __PYX_ERR(0, 62, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_6decode_string(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
 
-  /* function exit code */
+  /* "bencode2/_decoder.pyx":56
+ *             r.append(v)
+ * 
+ *         return r, index + 1             # <<<<<<<<<<<<<<
+ * 
+ *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_3 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_v_r);
+  __Pyx_GIVEREF(__pyx_v_r);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_r)) __PYX_ERR(0, 56, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3)) __PYX_ERR(0, 56, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_r = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
   goto __pyx_L0;
+
+  /* "bencode2/_decoder.pyx":49
+ *         return n, new_f + 1
+ * 
+ *     cdef tuple[list, int] __decode_list(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         r, index = [], index + 1
+ * 
+ */
+
+  /* function exit code */
   __pyx_L1_error:;
-  __pyx_r = NULL;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
-  {
-    Py_ssize_t __pyx_temp;
-    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
-      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
-    }
-  }
+  __Pyx_XDECREF(__pyx_v_r);
+  __Pyx_XDECREF(__pyx_v_v);
+  __Pyx_XDECREF(__pyx_v_index);
+  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_6decode_string(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+/* "bencode2/_decoder.pyx":58
+ *         return r, index + 1
+ * 
+ *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         colon = x.index(b":", index)
+ *         n = int(x[index:colon])
+ */
+
+static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_str(CYTHON_UNUSED struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
   PyObject *__pyx_v_colon = NULL;
   PyObject *__pyx_v_n = NULL;
   PyObject *__pyx_v_s = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
-  int __pyx_t_5;
-  int __pyx_t_6;
+  Py_ssize_t __pyx_t_5;
+  Py_ssize_t __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("decode_string", 1);
+  __Pyx_RefNannySetupContext("_Decoder__decode_str", 1);
 
-  /* "bencode2/_decoder.pyx":64
- *     def decode_string(self, x, index: int):
- *         """Decode torrent bencoded 'string' in x starting at f."""
+  /* "bencode2/_decoder.pyx":59
+ * 
+ *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
  *         colon = x.index(b":", index)             # <<<<<<<<<<<<<<
  *         n = int(x[index:colon])
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_x, __pyx_n_s_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = NULL;
-  __pyx_t_4 = 0;
-  #if CYTHON_UNPACK_METHODS
-  if (likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_3)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_3);
-      __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_4 = 1;
-    }
-  }
-  #endif
-  {
-    PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_kp_b__2, __pyx_v_index};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  }
+  __pyx_t_1 = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyBytes_Type_index, __pyx_v_x, __pyx_kp_b_, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_colon = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "bencode2/_decoder.pyx":65
- *         """Decode torrent bencoded 'string' in x starting at f."""
+  /* "bencode2/_decoder.pyx":60
+ *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):
  *         colon = x.index(b":", index)
  *         n = int(x[index:colon])             # <<<<<<<<<<<<<<
  * 
- *         if x[index : index + 1] == b"0" and colon != index + 1:
+ *         if x[index] == c'0' and colon != index + 1:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_v_colon, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_v_index);
+  __pyx_t_2 = __pyx_v_index;
+  __pyx_t_4 = (__pyx_t_2 == ((PyObject*)Py_None));
+  if (__pyx_t_4) {
+    __pyx_t_3 = 0;
+  } else {
+    __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L1_error)
+    __pyx_t_3 = __pyx_t_5;
+  }
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_INCREF(__pyx_v_colon);
+  __pyx_t_1 = __pyx_v_colon;
+  __pyx_t_4 = (__pyx_t_1 == Py_None);
+  if (__pyx_t_4) {
+    __pyx_t_5 = PY_SSIZE_T_MAX;
+  } else {
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L1_error)
+    __pyx_t_5 = __pyx_t_6;
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PySequence_GetSlice(__pyx_v_x, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_7 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 60, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_n = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_v_n = __pyx_t_7;
+  __pyx_t_7 = 0;
 
-  /* "bencode2/_decoder.pyx":67
+  /* "bencode2/_decoder.pyx":62
  *         n = int(x[index:colon])
  * 
- *         if x[index : index + 1] == b"0" and colon != index + 1:             # <<<<<<<<<<<<<<
+ *         if x[index] == c'0' and colon != index + 1:             # <<<<<<<<<<<<<<
  *             raise ValueError
  * 
  */
-  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_1 = __Pyx_PyInt_From_char('0'); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = (__Pyx_PyBytes_Equals(__pyx_t_1, __pyx_kp_b_0, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__pyx_t_6) {
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (__pyx_t_9) {
   } else {
-    __pyx_t_5 = __pyx_t_6;
+    __pyx_t_4 = __pyx_t_9;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_1 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_colon, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_8 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_colon, __pyx_t_8, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 67, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __pyx_t_6;
+  __pyx_t_4 = __pyx_t_9;
   __pyx_L4_bool_binop_done:;
-  if (unlikely(__pyx_t_5)) {
+  if (unlikely(__pyx_t_4)) {
 
-    /* "bencode2/_decoder.pyx":68
+    /* "bencode2/_decoder.pyx":63
  * 
- *         if x[index : index + 1] == b"0" and colon != index + 1:
+ *         if x[index] == c'0' and colon != index + 1:
  *             raise ValueError             # <<<<<<<<<<<<<<
  * 
  *         colon += 1
  */
     __Pyx_Raise(__pyx_builtin_ValueError, 0, 0, 0);
-    __PYX_ERR(0, 68, __pyx_L1_error)
+    __PYX_ERR(0, 63, __pyx_L1_error)
 
-    /* "bencode2/_decoder.pyx":67
+    /* "bencode2/_decoder.pyx":62
  *         n = int(x[index:colon])
  * 
- *         if x[index : index + 1] == b"0" and colon != index + 1:             # <<<<<<<<<<<<<<
+ *         if x[index] == c'0' and colon != index + 1:             # <<<<<<<<<<<<<<
  *             raise ValueError
  * 
  */
   }
 
-  /* "bencode2/_decoder.pyx":70
+  /* "bencode2/_decoder.pyx":65
  *             raise ValueError
  * 
  *         colon += 1             # <<<<<<<<<<<<<<
- *         s = x[colon : colon + n]
+ *         s = x[colon: colon + n]
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_v_colon, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF_SET(__pyx_v_colon, __pyx_t_2);
-  __pyx_t_2 = 0;
+  __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_colon, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF_SET(__pyx_v_colon, __pyx_t_1);
+  __pyx_t_1 = 0;
 
-  /* "bencode2/_decoder.pyx":71
+  /* "bencode2/_decoder.pyx":66
  * 
  *         colon += 1
- *         s = x[colon : colon + n]             # <<<<<<<<<<<<<<
+ *         s = x[colon: colon + n]             # <<<<<<<<<<<<<<
  * 
- *         return bytes(s), colon + n
+ *         return s, colon + n
  */
-  __pyx_t_2 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_colon, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_v_colon);
+  __pyx_t_1 = __pyx_v_colon;
+  __pyx_t_4 = (__pyx_t_1 == Py_None);
+  if (__pyx_t_4) {
+    __pyx_t_5 = 0;
+  } else {
+    __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_5 = __pyx_t_3;
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v_s = __pyx_t_1;
+  __pyx_t_4 = (__pyx_t_1 == Py_None);
+  if (__pyx_t_4) {
+    __pyx_t_3 = PY_SSIZE_T_MAX;
+  } else {
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_t_1); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
+    __pyx_t_3 = __pyx_t_6;
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PySequence_GetSlice(__pyx_v_x, __pyx_t_5, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_s = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bencode2/_decoder.pyx":73
- *         s = x[colon : colon + n]
+  /* "bencode2/_decoder.pyx":68
+ *         s = x[colon: colon + n]
  * 
- *         return bytes(s), colon + n             # <<<<<<<<<<<<<<
+ *         return s, colon + n             # <<<<<<<<<<<<<<
  * 
- *     def decode_list(self, x, index: int):
+ *     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_s); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_colon, __pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_INCREF(__pyx_v_s);
+  __Pyx_GIVEREF(__pyx_v_s);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_s)) __PYX_ERR(0, 68, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_r = ((PyObject*)__pyx_t_8);
+  __pyx_t_8 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/_decoder.pyx":62
- *         return n, new_f + 1
+  /* "bencode2/_decoder.pyx":58
+ *         return r, index + 1
  * 
- *     def decode_string(self, x, index: int):             # <<<<<<<<<<<<<<
- *         """Decode torrent bencoded 'string' in x starting at f."""
+ *     cdef tuple[bytes, int] __decode_str(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
  *         colon = x.index(b":", index)
+ *         n = int(x[index:colon])
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode_str", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_colon);
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_decoder.pyx":75
- *         return bytes(s), colon + n
+/* "bencode2/_decoder.pyx":70
+ *         return s, colon + n
  * 
- *     def decode_list(self, x, index: int):             # <<<<<<<<<<<<<<
- *         r, index = [], index + 1
+ *     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         index += 1
+ * 
+ */
+
+static PyObject *__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_dict(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
+  PyObject *__pyx_v_r = NULL;
+  PyObject *__pyx_v_k = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("_Decoder__decode_dict", 0);
+  __Pyx_INCREF(__pyx_v_index);
+
+  /* "bencode2/_decoder.pyx":71
+ * 
+ *     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):
+ *         index += 1             # <<<<<<<<<<<<<<
  * 
+ *         r = {}
+ */
+  __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 71, __pyx_L1_error)
+  __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
+  __pyx_t_1 = 0;
+
+  /* "bencode2/_decoder.pyx":73
+ *         index += 1
+ * 
+ *         r = {}             # <<<<<<<<<<<<<<
+ *         while x[index] != c'e':
+ *             k, index = self.__decode_str(x, index)
+ */
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_r = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "bencode2/_decoder.pyx":74
+ * 
+ *         r = {}
+ *         while x[index] != c'e':             # <<<<<<<<<<<<<<
+ *             k, index = self.__decode_str(x, index)
+ *             if self.str_key:
+ */
+  while (1) {
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = __Pyx_PyInt_From_char('e'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!__pyx_t_4) break;
+
+    /* "bencode2/_decoder.pyx":75
+ *         r = {}
+ *         while x[index] != c'e':
+ *             k, index = self.__decode_str(x, index)             # <<<<<<<<<<<<<<
+ *             if self.str_key:
+ *                 k = k.decode(encoding='utf-8', errors='strict')
+ */
+    __pyx_t_3 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode_str(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    if (likely(__pyx_t_3 != Py_None)) {
+      PyObject* sequence = __pyx_t_3;
+      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+      if (unlikely(size != 2)) {
+        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+        __PYX_ERR(0, 75, __pyx_L1_error)
+      }
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
+      __pyx_t_1 = PyTuple_GET_ITEM(sequence, 1); 
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_1);
+      #else
+      __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 75, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      #endif
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    } else {
+      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 75, __pyx_L1_error)
+    }
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 75, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_2);
+    __pyx_t_2 = 0;
+    __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
+    __pyx_t_1 = 0;
+
+    /* "bencode2/_decoder.pyx":76
+ *         while x[index] != c'e':
+ *             k, index = self.__decode_str(x, index)
+ *             if self.str_key:             # <<<<<<<<<<<<<<
+ *                 k = k.decode(encoding='utf-8', errors='strict')
+ *             r[k], index = self.__decode(x, index)
+ */
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_self->str_key); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 76, __pyx_L1_error)
+    if (__pyx_t_4) {
+
+      /* "bencode2/_decoder.pyx":77
+ *             k, index = self.__decode_str(x, index)
+ *             if self.str_key:
+ *                 k = k.decode(encoding='utf-8', errors='strict')             # <<<<<<<<<<<<<<
+ *             r[k], index = self.__decode(x, index)
+ * 
+ */
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_encoding, __pyx_kp_u_utf_8) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_errors, __pyx_n_u_strict) < 0) __PYX_ERR(0, 77, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF_SET(__pyx_v_k, __pyx_t_2);
+      __pyx_t_2 = 0;
+
+      /* "bencode2/_decoder.pyx":76
+ *         while x[index] != c'e':
+ *             k, index = self.__decode_str(x, index)
+ *             if self.str_key:             # <<<<<<<<<<<<<<
+ *                 k = k.decode(encoding='utf-8', errors='strict')
+ *             r[k], index = self.__decode(x, index)
+ */
+    }
+
+    /* "bencode2/_decoder.pyx":78
+ *             if self.str_key:
+ *                 k = k.decode(encoding='utf-8', errors='strict')
+ *             r[k], index = self.__decode(x, index)             # <<<<<<<<<<<<<<
+ * 
+ *         return r, index + 1
+ */
+    __pyx_t_2 = ((struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder *)__pyx_v_self->__pyx_vtab)->_Decoder__decode(__pyx_v_self, __pyx_v_x, __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    if (likely(__pyx_t_2 != Py_None)) {
+      PyObject* sequence = __pyx_t_2;
+      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+      if (unlikely(size != 2)) {
+        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+        __PYX_ERR(0, 78, __pyx_L1_error)
+      }
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
+      __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
+      __Pyx_INCREF(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_3);
+      #else
+      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 78, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      #endif
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    } else {
+      __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(0, 78, __pyx_L1_error)
+    }
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_3))) __PYX_ERR(0, 78, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_r, __pyx_v_k, __pyx_t_1) < 0))) __PYX_ERR(0, 78, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_3));
+    __pyx_t_3 = 0;
+  }
+
+  /* "bencode2/_decoder.pyx":80
+ *             r[k], index = self.__decode(x, index)
+ * 
+ *         return r, index + 1             # <<<<<<<<<<<<<<
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF(__pyx_v_r);
+  __Pyx_GIVEREF(__pyx_v_r);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_r)) __PYX_ERR(0, 80, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error);
+  __pyx_t_2 = 0;
+  __pyx_r = ((PyObject*)__pyx_t_3);
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "bencode2/_decoder.pyx":70
+ *         return s, colon + n
+ * 
+ *     cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):             # <<<<<<<<<<<<<<
+ *         index += 1
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder._Decoder__decode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_r);
+  __Pyx_XDECREF(__pyx_v_k);
+  __Pyx_XDECREF(__pyx_v_index);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_9decode_list(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_7Decoder_5__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_9decode_list = {"decode_list", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_9decode_list, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_9decode_list(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_7Decoder_5__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_7Decoder_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_decoder_7Decoder_5__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
-  PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_x = 0;
-  PyObject *__pyx_v_index = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  PyObject* values[3] = {0,0,0};
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_7Decoder_4__reduce_cython__(((struct __pyx_obj_8bencode2_8_decoder_Decoder *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8bencode2_8_decoder_7Decoder_4__reduce_cython__(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self) {
+  PyObject *__pyx_v_state = 0;
+  PyObject *__pyx_v__dict = 0;
+  int __pyx_v_use_setstate;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
+
+  /* "(tree fragment)":5
+ *     cdef object _dict
+ *     cdef bint use_setstate
+ *     state = (self.str_key,)             # <<<<<<<<<<<<<<
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ */
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_v_self->str_key);
+  __Pyx_GIVEREF(__pyx_v_self->str_key);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_self->str_key)) __PYX_ERR(1, 5, __pyx_L1_error);
+  __pyx_v_state = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":6
+ *     cdef bint use_setstate
+ *     state = (self.str_key,)
+ *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
+ *     if _dict is not None:
+ *         state += (_dict,)
+ */
+  __pyx_t_1 = __Pyx_GetAttr3(((PyObject *)__pyx_v_self), __pyx_n_s_dict, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v__dict = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":7
+ *     state = (self.str_key,)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+  __pyx_t_2 = (__pyx_v__dict != Py_None);
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":8
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:
+ *         state += (_dict,)             # <<<<<<<<<<<<<<
+ *         use_setstate = True
+ *     else:
+ */
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_v__dict);
+    __Pyx_GIVEREF(__pyx_v__dict);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict)) __PYX_ERR(1, 8, __pyx_L1_error);
+    __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 8, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_3));
+    __pyx_t_3 = 0;
+
+    /* "(tree fragment)":9
+ *     if _dict is not None:
+ *         state += (_dict,)
+ *         use_setstate = True             # <<<<<<<<<<<<<<
+ *     else:
+ *         use_setstate = self.str_key is not None
+ */
+    __pyx_v_use_setstate = 1;
+
+    /* "(tree fragment)":7
+ *     state = (self.str_key,)
+ *     _dict = getattr(self, '__dict__', None)
+ *     if _dict is not None:             # <<<<<<<<<<<<<<
+ *         state += (_dict,)
+ *         use_setstate = True
+ */
+    goto __pyx_L3;
+  }
+
+  /* "(tree fragment)":11
+ *         use_setstate = True
+ *     else:
+ *         use_setstate = self.str_key is not None             # <<<<<<<<<<<<<<
+ *     if use_setstate:
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, None), state
+ */
+  /*else*/ {
+    __pyx_t_2 = (__pyx_v_self->str_key != Py_None);
+    __pyx_v_use_setstate = __pyx_t_2;
+  }
+  __pyx_L3:;
+
+  /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self.str_key is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, None), state
+ *     else:
+ */
+  if (__pyx_v_use_setstate) {
+
+    /* "(tree fragment)":13
+ *         use_setstate = self.str_key is not None
+ *     if use_setstate:
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, None), state             # <<<<<<<<<<<<<<
+ *     else:
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, state)
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pyx_unpickle_Decoder); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))))) __PYX_ERR(1, 13, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_int_27736365);
+    __Pyx_GIVEREF(__pyx_int_27736365);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_27736365)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __Pyx_INCREF(Py_None);
+    __Pyx_GIVEREF(Py_None);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_state)) __PYX_ERR(1, 13, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_4;
+    __pyx_t_4 = 0;
+    goto __pyx_L0;
+
+    /* "(tree fragment)":12
+ *     else:
+ *         use_setstate = self.str_key is not None
+ *     if use_setstate:             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, None), state
+ *     else:
+ */
+  }
+
+  /* "(tree fragment)":15
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, None), state
+ *     else:
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, state)             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_Decoder__set_state(self, __pyx_state)
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_Decoder); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))))) __PYX_ERR(1, 15, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_int_27736365);
+    __Pyx_GIVEREF(__pyx_int_27736365);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_27736365)) __PYX_ERR(1, 15, __pyx_L1_error);
+    __Pyx_INCREF(__pyx_v_state);
+    __Pyx_GIVEREF(__pyx_v_state);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state)) __PYX_ERR(1, 15, __pyx_L1_error);
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error);
+    __pyx_t_4 = 0;
+    __pyx_t_1 = 0;
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
+    goto __pyx_L0;
+  }
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_state);
+  __Pyx_XDECREF(__pyx_v__dict);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_Decoder__set_state(self, __pyx_state)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8bencode2_8_decoder_7Decoder_7__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_7Decoder_7__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_7Decoder_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_decoder_7Decoder_7__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v___pyx_state = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("decode_list (wrapper)", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_x,&__pyx_n_s_index,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
-        CYTHON_FALLTHROUGH;
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-        CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 16, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
-        CYTHON_FALLTHROUGH;
-        case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("decode_list", 1, 3, 3, 1); __PYX_ERR(0, 75, __pyx_L3_error)
-        }
-        CYTHON_FALLTHROUGH;
-        case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) {
-          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
-          kw_args--;
-        }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L3_error)
-        else {
-          __Pyx_RaiseArgtupleInvalid("decode_list", 1, 3, 3, 2); __PYX_ERR(0, 75, __pyx_L3_error)
-        }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_list") < 0)) __PYX_ERR(0, 75, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 16, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 3)) {
+    } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_self = values[0];
-    __pyx_v_x = values[1];
-    __pyx_v_index = ((PyObject*)values[2]);
+    __pyx_v___pyx_state = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode_list", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 75, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_index), (&PyInt_Type), 0, "index", 1))) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_8decode_list(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder_7Decoder_6__setstate_cython__(((struct __pyx_obj_8bencode2_8_decoder_Decoder *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_8decode_list(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
-  PyObject *__pyx_v_r = NULL;
-  PyObject *__pyx_v_v = NULL;
+static PyObject *__pyx_pf_8bencode2_8_decoder_7Decoder_6__setstate_cython__(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  int __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
-  PyObject *(*__pyx_t_7)(PyObject *);
-  int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("decode_list", 0);
-  __Pyx_INCREF(__pyx_v_index);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
-  /* "bencode2/_decoder.pyx":76
- * 
- *     def decode_list(self, x, index: int):
- *         r, index = [], index + 1             # <<<<<<<<<<<<<<
- * 
- *         while x[index : index + 1] != b"e":
+  /* "(tree fragment)":17
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, state)
+ * def __setstate_cython__(self, __pyx_state):
+ *     __pyx_unpickle_Decoder__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8bencode2_8_decoder___pyx_unpickle_Decoder__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 76, __pyx_L1_error)
-  __pyx_v_r = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
-  __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_2));
-  __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":78
- *         r, index = [], index + 1
- * 
- *         while x[index : index + 1] != b"e":             # <<<<<<<<<<<<<<
- *             v, index = self.decode_func[x[index : index + 1]](x, index)
- *             r.append(v)
- */
-  while (1) {
-    __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_2, NULL, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = (__Pyx_PyBytes_Equals(__pyx_t_1, __pyx_n_b_e, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 78, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!__pyx_t_3) break;
-
-    /* "bencode2/_decoder.pyx":79
- * 
- *         while x[index : index + 1] != b"e":
- *             v, index = self.decode_func[x[index : index + 1]](x, index)             # <<<<<<<<<<<<<<
- *             r.append(v)
- * 
- */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_func); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_4, NULL, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = NULL;
-    __pyx_t_6 = 0;
-    #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_4))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
-        __Pyx_INCREF(__pyx_t_5);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_4, function);
-        __pyx_t_6 = 1;
-      }
-    }
-    #endif
-    {
-      PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_v_x, __pyx_v_index};
-      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    }
-    if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
-      PyObject* sequence = __pyx_t_1;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 79, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      if (likely(PyTuple_CheckExact(sequence))) {
-        __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
-      } else {
-        __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
-      }
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_5);
-      #else
-      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 79, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 79, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      #endif
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    } else {
-      Py_ssize_t index = -1;
-      __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2);
-      index = 0; __pyx_t_4 = __pyx_t_7(__pyx_t_2); if (unlikely(!__pyx_t_4)) goto __pyx_L5_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_4);
-      index = 1; __pyx_t_5 = __pyx_t_7(__pyx_t_2); if (unlikely(!__pyx_t_5)) goto __pyx_L5_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_2), 2) < 0) __PYX_ERR(0, 79, __pyx_L1_error)
-      __pyx_t_7 = NULL;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      goto __pyx_L6_unpacking_done;
-      __pyx_L5_unpacking_failed:;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_7 = NULL;
-      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 79, __pyx_L1_error)
-      __pyx_L6_unpacking_done:;
-    }
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_5))) __PYX_ERR(0, 79, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_4);
-    __pyx_t_4 = 0;
-    __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_5));
-    __pyx_t_5 = 0;
-
-    /* "bencode2/_decoder.pyx":80
- *         while x[index : index + 1] != b"e":
- *             v, index = self.decode_func[x[index : index + 1]](x, index)
- *             r.append(v)             # <<<<<<<<<<<<<<
- * 
- *         return r, index + 1
- */
-    __pyx_t_8 = __Pyx_PyList_Append(__pyx_v_r, __pyx_v_v); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 80, __pyx_L1_error)
-  }
-
-  /* "bencode2/_decoder.pyx":82
- *             r.append(v)
- * 
- *         return r, index + 1             # <<<<<<<<<<<<<<
- * 
- *     def decode_dict(self, x, index: int):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 82, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_INCREF(__pyx_v_r);
-  __Pyx_GIVEREF(__pyx_v_r);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_r)) __PYX_ERR(0, 82, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error);
-  __pyx_t_1 = 0;
-  __pyx_r = __pyx_t_5;
-  __pyx_t_5 = 0;
-  goto __pyx_L0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bencode2/_decoder.pyx":75
- *         return bytes(s), colon + n
- * 
- *     def decode_list(self, x, index: int):             # <<<<<<<<<<<<<<
- *         r, index = [], index + 1
- * 
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_Decoder__set_state(self, __pyx_state)
  */
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_list", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.Decoder.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_r);
-  __Pyx_XDECREF(__pyx_v_v);
-  __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_decoder.pyx":84
- *         return r, index + 1
- * 
- *     def decode_dict(self, x, index: int):             # <<<<<<<<<<<<<<
- *         """Decode bencoded dictionary."""
- *         index += 1
+/* "(tree fragment)":1
+ * def __pyx_unpickle_Decoder(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_11decode_dict(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_8bencode2_8_decoder_1__pyx_unpickle_Decoder(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_8bencode2_8_decoder_14BencodeDecoder_10decode_dict, "Decode bencoded dictionary.");
-static PyMethodDef __pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_11decode_dict = {"decode_dict", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_11decode_dict, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_8bencode2_8_decoder_14BencodeDecoder_10decode_dict};
-static PyObject *__pyx_pw_8bencode2_8_decoder_14BencodeDecoder_11decode_dict(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_8bencode2_8_decoder_1__pyx_unpickle_Decoder = {"__pyx_unpickle_Decoder", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_1__pyx_unpickle_Decoder, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_8bencode2_8_decoder_1__pyx_unpickle_Decoder(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
-  PyObject *__pyx_v_self = 0;
-  PyObject *__pyx_v_x = 0;
-  PyObject *__pyx_v_index = 0;
+  PyObject *__pyx_v___pyx_type = 0;
+  long __pyx_v___pyx_checksum;
+  PyObject *__pyx_v___pyx_state = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[3] = {0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("decode_dict (wrapper)", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Decoder (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_x,&__pyx_n_s_index,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -4706,370 +5096,562 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_type)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_checksum)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("decode_dict", 1, 3, 3, 1); __PYX_ERR(0, 84, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Decoder", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) {
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("decode_dict", 1, 3, 3, 2); __PYX_ERR(0, 84, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Decoder", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "decode_dict") < 0)) __PYX_ERR(0, 84, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__pyx_unpickle_Decoder") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_self = values[0];
-    __pyx_v_x = values[1];
-    __pyx_v_index = ((PyObject*)values[2]);
+    __pyx_v___pyx_type = values[0];
+    __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+    __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("decode_dict", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 84, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Decoder", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("bencode2._decoder.__pyx_unpickle_Decoder", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_index), (&PyInt_Type), 0, "index", 1))) __PYX_ERR(0, 84, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8bencode2_8_decoder_14BencodeDecoder_10decode_dict(__pyx_self, __pyx_v_self, __pyx_v_x, __pyx_v_index);
+  __pyx_r = __pyx_pf_8bencode2_8_decoder___pyx_unpickle_Decoder(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __pyx_r = NULL;
-  __pyx_L0:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8bencode2_8_decoder_14BencodeDecoder_10decode_dict(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_x, PyObject *__pyx_v_index) {
-  PyObject *__pyx_v_r = NULL;
-  PyObject *__pyx_v_k = NULL;
+static PyObject *__pyx_pf_8bencode2_8_decoder___pyx_unpickle_Decoder(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_v___pyx_PickleError = 0;
+  PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  int __pyx_t_3;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("decode_dict", 0);
-  __Pyx_INCREF(__pyx_v_index);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Decoder", 1);
 
-  /* "bencode2/_decoder.pyx":86
- *     def decode_dict(self, x, index: int):
- *         """Decode bencoded dictionary."""
- *         index += 1             # <<<<<<<<<<<<<<
- * 
- *         r = {}
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x1a7392d, 0x8d52a63, 0xc95bd82):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))" % __pyx_checksum
  */
-  __pyx_t_1 = PyNumber_InPlaceAdd(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 86, __pyx_L1_error)
-  __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_1));
-  __pyx_t_1 = 0;
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__2, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_2) {
 
-  /* "bencode2/_decoder.pyx":88
- *         index += 1
- * 
- *         r = {}             # <<<<<<<<<<<<<<
- * 
- *         while x[index : index + 1] != b"e":
+    /* "(tree fragment)":5
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x1a7392d, 0x8d52a63, 0xc95bd82):
+ *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))" % __pyx_checksum
+ *     __pyx_result = Decoder.__new__(__pyx_type)
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_r = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_n_s_PickleError);
+    __Pyx_GIVEREF(__pyx_n_s_PickleError);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError)) __PYX_ERR(1, 5, __pyx_L1_error);
+    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/_decoder.pyx":90
- *         r = {}
- * 
- *         while x[index : index + 1] != b"e":             # <<<<<<<<<<<<<<
- *             k, index = self.decode_string(x, index)
- *             r[k], index = self.decode_func[x[index : index + 1]](x, index)
+    /* "(tree fragment)":6
+ *     if __pyx_checksum not in (0x1a7392d, 0x8d52a63, 0xc95bd82):
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))" % __pyx_checksum             # <<<<<<<<<<<<<<
+ *     __pyx_result = Decoder.__new__(__pyx_type)
+ *     if __pyx_state is not None:
  */
-  while (1) {
-    __pyx_t_1 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_1, NULL, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_Raise(__pyx_v___pyx_PickleError, __pyx_t_1, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_n_b_e, Py_NE)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 90, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (!__pyx_t_3) break;
+    __PYX_ERR(1, 6, __pyx_L1_error)
 
-    /* "bencode2/_decoder.pyx":91
- * 
- *         while x[index : index + 1] != b"e":
- *             k, index = self.decode_string(x, index)             # <<<<<<<<<<<<<<
- *             r[k], index = self.decode_func[x[index : index + 1]](x, index)
- * 
+    /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x1a7392d, 0x8d52a63, 0xc95bd82):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))" % __pyx_checksum
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = NULL;
-    __pyx_t_5 = 0;
-    #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_4);
-        __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_5 = 1;
-      }
-    }
-    #endif
-    {
-      PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_v_x, __pyx_v_index};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    }
-    if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
-      PyObject* sequence = __pyx_t_2;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 91, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      if (likely(PyTuple_CheckExact(sequence))) {
-        __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-      } else {
-        __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
-      }
-      __Pyx_INCREF(__pyx_t_1);
+  }
+
+  /* "(tree fragment)":7
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))" % __pyx_checksum
+ *     __pyx_result = Decoder.__new__(__pyx_type)             # <<<<<<<<<<<<<<
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_Decoder__set_state(<Decoder> __pyx_result, __pyx_state)
+ */
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_8bencode2_8_decoder_Decoder), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = NULL;
+  __pyx_t_5 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
-      #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      #endif
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    } else {
-      Py_ssize_t index = -1;
-      __pyx_t_6 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 91, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6);
-      index = 0; __pyx_t_1 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_1)) goto __pyx_L5_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_1);
-      index = 1; __pyx_t_4 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_4)) goto __pyx_L5_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_4);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
-      __pyx_t_7 = NULL;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      goto __pyx_L6_unpacking_done;
-      __pyx_L5_unpacking_failed:;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_7 = NULL;
-      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 91, __pyx_L1_error)
-      __pyx_L6_unpacking_done:;
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_5 = 1;
     }
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_4))) __PYX_ERR(0, 91, __pyx_L1_error)
-    __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_1);
-    __pyx_t_1 = 0;
-    __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_4));
-    __pyx_t_4 = 0;
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v___pyx_type};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __pyx_v___pyx_result = __pyx_t_1;
+  __pyx_t_1 = 0;
 
-    /* "bencode2/_decoder.pyx":92
- *         while x[index : index + 1] != b"e":
- *             k, index = self.decode_string(x, index)
- *             r[k], index = self.decode_func[x[index : index + 1]](x, index)             # <<<<<<<<<<<<<<
- * 
- *         return r, index + 1
+  /* "(tree fragment)":8
+ *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))" % __pyx_checksum
+ *     __pyx_result = Decoder.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_Decoder__set_state(<Decoder> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  __pyx_t_2 = (__pyx_v___pyx_state != Py_None);
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":9
+ *     __pyx_result = Decoder.__new__(__pyx_type)
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_Decoder__set_state(<Decoder> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Decoder__set_state(Decoder __pyx_result, tuple __pyx_state):
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_decode_func); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_1 = __pyx_f_8bencode2_8_decoder___pyx_unpickle_Decoder__set_state(((struct __pyx_obj_8bencode2_8_decoder_Decoder *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_PyObject_GetSlice(__pyx_v_x, 0, 0, &__pyx_v_index, &__pyx_t_1, NULL, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = NULL;
-    __pyx_t_5 = 0;
+
+    /* "(tree fragment)":8
+ *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))" % __pyx_checksum
+ *     __pyx_result = Decoder.__new__(__pyx_type)
+ *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
+ *         __pyx_unpickle_Decoder__set_state(<Decoder> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ */
+  }
+
+  /* "(tree fragment)":10
+ *     if __pyx_state is not None:
+ *         __pyx_unpickle_Decoder__set_state(<Decoder> __pyx_result, __pyx_state)
+ *     return __pyx_result             # <<<<<<<<<<<<<<
+ * cdef __pyx_unpickle_Decoder__set_state(Decoder __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_key = __pyx_state[0]
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v___pyx_result);
+  __pyx_r = __pyx_v___pyx_result;
+  goto __pyx_L0;
+
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_Decoder(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("bencode2._decoder.__pyx_unpickle_Decoder", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v___pyx_PickleError);
+  __Pyx_XDECREF(__pyx_v___pyx_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":11
+ *         __pyx_unpickle_Decoder__set_state(<Decoder> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Decoder__set_state(Decoder __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.str_key = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ */
+
+static PyObject *__pyx_f_8bencode2_8_decoder___pyx_unpickle_Decoder__set_state(struct __pyx_obj_8bencode2_8_decoder_Decoder *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Decoder__set_state", 1);
+
+  /* "(tree fragment)":12
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Decoder__set_state(Decoder __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_key = __pyx_state[0]             # <<<<<<<<<<<<<<
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 12, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v___pyx_result->str_key);
+  __Pyx_DECREF(__pyx_v___pyx_result->str_key);
+  __pyx_v___pyx_result->str_key = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "(tree fragment)":13
+ * cdef __pyx_unpickle_Decoder__set_state(Decoder __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_key = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[1])
+ */
+  if (unlikely(__pyx_v___pyx_state == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(1, 13, __pyx_L1_error)
+  }
+  __pyx_t_3 = __Pyx_PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_4 = (__pyx_t_3 > 1);
+  if (__pyx_t_4) {
+  } else {
+    __pyx_t_2 = __pyx_t_4;
+    goto __pyx_L4_bool_binop_done;
+  }
+  __pyx_t_4 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_2 = __pyx_t_4;
+  __pyx_L4_bool_binop_done:;
+  if (__pyx_t_2) {
+
+    /* "(tree fragment)":14
+ *     __pyx_result.str_key = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
+ *         __pyx_result.__dict__.update(__pyx_state[1])             # <<<<<<<<<<<<<<
+ */
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_update); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(__pyx_v___pyx_state == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+      __PYX_ERR(1, 14, __pyx_L1_error)
+    }
+    __pyx_t_5 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_7 = NULL;
+    __pyx_t_8 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_6);
+    if (likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
-        __pyx_t_5 = 1;
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __pyx_t_8 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_v_x, __pyx_v_index};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    }
-    if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
-      PyObject* sequence = __pyx_t_2;
-      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-      if (unlikely(size != 2)) {
-        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
-        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 92, __pyx_L1_error)
-      }
-      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-      if (likely(PyTuple_CheckExact(sequence))) {
-        __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
-      } else {
-        __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
-      }
-      __Pyx_INCREF(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_6);
-      #else
-      __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 92, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      #endif
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    } else {
-      Py_ssize_t index = -1;
-      __pyx_t_4 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4);
-      index = 0; __pyx_t_1 = __pyx_t_7(__pyx_t_4); if (unlikely(!__pyx_t_1)) goto __pyx_L7_unpacking_failed;
+      PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      index = 1; __pyx_t_6 = __pyx_t_7(__pyx_t_4); if (unlikely(!__pyx_t_6)) goto __pyx_L7_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_6);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_4), 2) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
-      __pyx_t_7 = NULL;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      goto __pyx_L8_unpacking_done;
-      __pyx_L7_unpacking_failed:;
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_7 = NULL;
-      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 92, __pyx_L1_error)
-      __pyx_L8_unpacking_done:;
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_6))) __PYX_ERR(0, 92, __pyx_L1_error)
-    if (unlikely((PyDict_SetItem(__pyx_v_r, __pyx_v_k, __pyx_t_1) < 0))) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF_SET(__pyx_v_index, ((PyObject*)__pyx_t_6));
-    __pyx_t_6 = 0;
-  }
 
-  /* "bencode2/_decoder.pyx":94
- *             r[k], index = self.decode_func[x[index : index + 1]](x, index)
- * 
- *         return r, index + 1             # <<<<<<<<<<<<<<
+    /* "(tree fragment)":13
+ * cdef __pyx_unpickle_Decoder__set_state(Decoder __pyx_result, tuple __pyx_state):
+ *     __pyx_result.str_key = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
+ *         __pyx_result.__dict__.update(__pyx_state[1])
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyNumber_Add(__pyx_v_index, __pyx_int_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_INCREF(__pyx_v_r);
-  __Pyx_GIVEREF(__pyx_v_r);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_r)) __PYX_ERR(0, 94, __pyx_L1_error);
-  __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error);
-  __pyx_t_2 = 0;
-  __pyx_r = __pyx_t_6;
-  __pyx_t_6 = 0;
-  goto __pyx_L0;
+  }
 
-  /* "bencode2/_decoder.pyx":84
- *         return r, index + 1
- * 
- *     def decode_dict(self, x, index: int):             # <<<<<<<<<<<<<<
- *         """Decode bencoded dictionary."""
- *         index += 1
+  /* "(tree fragment)":11
+ *         __pyx_unpickle_Decoder__set_state(<Decoder> __pyx_result, __pyx_state)
+ *     return __pyx_result
+ * cdef __pyx_unpickle_Decoder__set_state(Decoder __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_result.str_key = __pyx_state[0]
+ *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  */
 
   /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("bencode2._decoder.BencodeDecoder.decode_dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("bencode2._decoder.__pyx_unpickle_Decoder__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_r);
-  __Pyx_XDECREF(__pyx_v_k);
-  __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+static struct __pyx_vtabstruct_8bencode2_8_decoder_Decoder __pyx_vtable_8bencode2_8_decoder_Decoder;
+
+static PyObject *__pyx_tp_new_8bencode2_8_decoder_Decoder(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_8bencode2_8_decoder_Decoder *p;
+  PyObject *o;
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
+    o = (*t->tp_alloc)(t, 0);
+  } else {
+    o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
+  }
+  if (unlikely(!o)) return 0;
+  #endif
+  p = ((struct __pyx_obj_8bencode2_8_decoder_Decoder *)o);
+  p->__pyx_vtab = __pyx_vtabptr_8bencode2_8_decoder_Decoder;
+  p->str_key = Py_None; Py_INCREF(Py_None);
+  return o;
+}
+
+static void __pyx_tp_dealloc_8bencode2_8_decoder_Decoder(PyObject *o) {
+  struct __pyx_obj_8bencode2_8_decoder_Decoder *p = (struct __pyx_obj_8bencode2_8_decoder_Decoder *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_8bencode2_8_decoder_Decoder) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
+  PyObject_GC_UnTrack(o);
+  Py_CLEAR(p->str_key);
+  #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+  (*Py_TYPE(o)->tp_free)(o);
+  #else
+  {
+    freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+    if (tp_free) tp_free(o);
+  }
+  #endif
+}
+
+static int __pyx_tp_traverse_8bencode2_8_decoder_Decoder(PyObject *o, visitproc v, void *a) {
+  int e;
+  struct __pyx_obj_8bencode2_8_decoder_Decoder *p = (struct __pyx_obj_8bencode2_8_decoder_Decoder *)o;
+  if (p->str_key) {
+    e = (*v)(p->str_key, a); if (e) return e;
+  }
+  return 0;
+}
+
+static int __pyx_tp_clear_8bencode2_8_decoder_Decoder(PyObject *o) {
+  PyObject* tmp;
+  struct __pyx_obj_8bencode2_8_decoder_Decoder *p = (struct __pyx_obj_8bencode2_8_decoder_Decoder *)o;
+  tmp = ((PyObject*)p->str_key);
+  p->str_key = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  return 0;
+}
+
+static PyMethodDef __pyx_methods_8bencode2_8_decoder_Decoder[] = {
+  {"decode", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_7Decoder_3decode, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_7Decoder_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_8bencode2_8_decoder_7Decoder_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {0, 0, 0, 0}
+};
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_8bencode2_8_decoder_Decoder_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_8bencode2_8_decoder_Decoder},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_8bencode2_8_decoder_Decoder},
+  {Py_tp_clear, (void *)__pyx_tp_clear_8bencode2_8_decoder_Decoder},
+  {Py_tp_methods, (void *)__pyx_methods_8bencode2_8_decoder_Decoder},
+  {Py_tp_init, (void *)__pyx_pw_8bencode2_8_decoder_7Decoder_1__init__},
+  {Py_tp_new, (void *)__pyx_tp_new_8bencode2_8_decoder_Decoder},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_8bencode2_8_decoder_Decoder_spec = {
+  "bencode2._decoder.Decoder",
+  sizeof(struct __pyx_obj_8bencode2_8_decoder_Decoder),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC,
+  __pyx_type_8bencode2_8_decoder_Decoder_slots,
+};
+#else
+
+static PyTypeObject __pyx_type_8bencode2_8_decoder_Decoder = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "bencode2._decoder.""Decoder", /*tp_name*/
+  sizeof(struct __pyx_obj_8bencode2_8_decoder_Decoder), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_8bencode2_8_decoder_Decoder, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
+  0, /*tp_doc*/
+  __pyx_tp_traverse_8bencode2_8_decoder_Decoder, /*tp_traverse*/
+  __pyx_tp_clear_8bencode2_8_decoder_Decoder, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  __pyx_methods_8bencode2_8_decoder_Decoder, /*tp_methods*/
+  0, /*tp_members*/
+  0, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
+  0, /*tp_dictoffset*/
+  #endif
+  __pyx_pw_8bencode2_8_decoder_7Decoder_1__init__, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_8bencode2_8_decoder_Decoder, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
+  0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+#endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
@@ -5081,197 +5663,175 @@
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_kp_b_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 0, 0},
     {&__pyx_kp_b_0, __pyx_k_0, sizeof(__pyx_k_0), 0, 0, 0, 0},
-    {&__pyx_kp_b_1, __pyx_k_1, sizeof(__pyx_k_1), 0, 0, 0, 0},
-    {&__pyx_kp_b_2, __pyx_k_2, sizeof(__pyx_k_2), 0, 0, 0, 0},
-    {&__pyx_kp_b_3, __pyx_k_3, sizeof(__pyx_k_3), 0, 0, 0, 0},
-    {&__pyx_kp_b_4, __pyx_k_4, sizeof(__pyx_k_4), 0, 0, 0, 0},
-    {&__pyx_kp_b_5, __pyx_k_5, sizeof(__pyx_k_5), 0, 0, 0, 0},
-    {&__pyx_kp_b_6, __pyx_k_6, sizeof(__pyx_k_6), 0, 0, 0, 0},
-    {&__pyx_kp_b_7, __pyx_k_7, sizeof(__pyx_k_7), 0, 0, 0, 0},
-    {&__pyx_kp_b_8, __pyx_k_8, sizeof(__pyx_k_8), 0, 0, 0, 0},
-    {&__pyx_kp_b_9, __pyx_k_9, sizeof(__pyx_k_9), 0, 0, 0, 0},
     {&__pyx_n_s_Any, __pyx_k_Any, sizeof(__pyx_k_Any), 0, 0, 1, 1},
     {&__pyx_n_s_BencodeDecodeError, __pyx_k_BencodeDecodeError, sizeof(__pyx_k_BencodeDecodeError), 0, 0, 1, 1},
-    {&__pyx_n_s_BencodeDecoder, __pyx_k_BencodeDecoder, sizeof(__pyx_k_BencodeDecoder), 0, 0, 1, 1},
-    {&__pyx_n_s_BencodeDecoder___init, __pyx_k_BencodeDecoder___init, sizeof(__pyx_k_BencodeDecoder___init), 0, 0, 1, 1},
-    {&__pyx_n_s_BencodeDecoder_decode, __pyx_k_BencodeDecoder_decode, sizeof(__pyx_k_BencodeDecoder_decode), 0, 0, 1, 1},
-    {&__pyx_n_s_BencodeDecoder_decode_dict, __pyx_k_BencodeDecoder_decode_dict, sizeof(__pyx_k_BencodeDecoder_decode_dict), 0, 0, 1, 1},
-    {&__pyx_n_s_BencodeDecoder_decode_int, __pyx_k_BencodeDecoder_decode_int, sizeof(__pyx_k_BencodeDecoder_decode_int), 0, 0, 1, 1},
-    {&__pyx_n_s_BencodeDecoder_decode_list, __pyx_k_BencodeDecoder_decode_list, sizeof(__pyx_k_BencodeDecoder_decode_list), 0, 0, 1, 1},
-    {&__pyx_n_s_BencodeDecoder_decode_string, __pyx_k_BencodeDecoder_decode_string, sizeof(__pyx_k_BencodeDecoder_decode_string), 0, 0, 1, 1},
-    {&__pyx_n_s_Callable, __pyx_k_Callable, sizeof(__pyx_k_Callable), 0, 0, 1, 1},
+    {&__pyx_n_s_Decoder, __pyx_k_Decoder, sizeof(__pyx_k_Decoder), 0, 0, 1, 1},
+    {&__pyx_n_s_Decoder___reduce_cython, __pyx_k_Decoder___reduce_cython, sizeof(__pyx_k_Decoder___reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Decoder___setstate_cython, __pyx_k_Decoder___setstate_cython, sizeof(__pyx_k_Decoder___setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Decoder_decode, __pyx_k_Decoder_decode, sizeof(__pyx_k_Decoder_decode), 0, 0, 1, 1},
+    {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
     {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
+    {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
-    {&__pyx_n_s__16, __pyx_k__16, sizeof(__pyx_k__16), 0, 0, 1, 1},
-    {&__pyx_kp_b__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 0, 0},
+    {&__pyx_n_s__12, __pyx_k__12, sizeof(__pyx_k__12), 0, 0, 1, 1},
     {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_kp_u_at_index, __pyx_k_at_index, sizeof(__pyx_k_at_index), 0, 1, 0, 0},
     {&__pyx_n_s_bencode2__decoder, __pyx_k_bencode2__decoder, sizeof(__pyx_k_bencode2__decoder), 0, 0, 1, 1},
     {&__pyx_kp_s_bencode2__decoder_pyx, __pyx_k_bencode2__decoder_pyx, sizeof(__pyx_k_bencode2__decoder_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_bytes, __pyx_k_bytes, sizeof(__pyx_k_bytes), 0, 0, 1, 1},
     {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-    {&__pyx_n_s_collections_abc, __pyx_k_collections_abc, sizeof(__pyx_k_collections_abc), 0, 0, 1, 1},
-    {&__pyx_n_s_colon, __pyx_k_colon, sizeof(__pyx_k_colon), 0, 0, 1, 1},
-    {&__pyx_n_s_compat, __pyx_k_compat, sizeof(__pyx_k_compat), 0, 0, 1, 1},
-    {&__pyx_n_b_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 0, 0, 1},
     {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
     {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
-    {&__pyx_n_s_decode_dict, __pyx_k_decode_dict, sizeof(__pyx_k_decode_dict), 0, 0, 1, 1},
-    {&__pyx_n_s_decode_func, __pyx_k_decode_func, sizeof(__pyx_k_decode_func), 0, 0, 1, 1},
-    {&__pyx_n_s_decode_int, __pyx_k_decode_int, sizeof(__pyx_k_decode_int), 0, 0, 1, 1},
-    {&__pyx_n_s_decode_list, __pyx_k_decode_list, sizeof(__pyx_k_decode_list), 0, 0, 1, 1},
-    {&__pyx_n_s_decode_string, __pyx_k_decode_string, sizeof(__pyx_k_decode_string), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-    {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
+    {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
+    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
     {&__pyx_n_b_e, __pyx_k_e, sizeof(__pyx_k_e), 0, 0, 0, 1},
+    {&__pyx_n_s_e, __pyx_k_e, sizeof(__pyx_k_e), 0, 0, 1, 1},
+    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_s_encoding, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 0, 1, 1},
+    {&__pyx_n_s_errors, __pyx_k_errors, sizeof(__pyx_k_errors), 0, 0, 1, 1},
     {&__pyx_n_s_exceptions, __pyx_k_exceptions, sizeof(__pyx_k_exceptions), 0, 0, 1, 1},
-    {&__pyx_n_b_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 0, 1},
+    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
-    {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
-    {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
-    {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
-    {&__pyx_kp_u_invalid_bencoded_value_data_afte, __pyx_k_invalid_bencoded_value_data_afte, sizeof(__pyx_k_invalid_bencoded_value_data_afte), 0, 1, 0, 0},
+    {&__pyx_kp_u_invalid_bencode_value_data_after, __pyx_k_invalid_bencode_value_data_after, sizeof(__pyx_k_invalid_bencode_value_data_after), 0, 1, 0, 0},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
-    {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
-    {&__pyx_n_b_l, __pyx_k_l, sizeof(__pyx_k_l), 0, 0, 0, 1},
+    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_length, __pyx_k_length, sizeof(__pyx_k_length), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-    {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
-    {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
-    {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-    {&__pyx_n_s_new_f, __pyx_k_new_f, sizeof(__pyx_k_new_f), 0, 0, 1, 1},
-    {&__pyx_kp_u_not_a_valid_bencoded_string, __pyx_k_not_a_valid_bencoded_string, sizeof(__pyx_k_not_a_valid_bencoded_string), 0, 1, 0, 0},
-    {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
-    {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
-    {&__pyx_n_s_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 0, 1, 1},
+    {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
+    {&__pyx_kp_u_not_a_valid_bencode_bytes, __pyx_k_not_a_valid_bencode_bytes, sizeof(__pyx_k_not_a_valid_bencode_bytes), 0, 1, 0, 0},
+    {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_unpickle_Decoder, __pyx_k_pyx_unpickle_Decoder, sizeof(__pyx_k_pyx_unpickle_Decoder), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
-    {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
-    {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
-    {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
+    {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
+    {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
+    {&__pyx_n_s_str_key, __pyx_k_str_key, sizeof(__pyx_k_str_key), 0, 0, 1, 1},
+    {&__pyx_n_u_strict, __pyx_k_strict, sizeof(__pyx_k_strict), 0, 1, 0, 1},
+    {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-    {&__pyx_n_s_to_binary, __pyx_k_to_binary, sizeof(__pyx_k_to_binary), 0, 0, 1, 1},
     {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
-    {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
+    {&__pyx_kp_u_unexpected_token, __pyx_k_unexpected_token, sizeof(__pyx_k_unexpected_token), 0, 1, 0, 0},
+    {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
+    {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
+    {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
-    {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 41, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 15, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "bencode2/_decoder.pyx":11
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0x1a7392d, 0x8d52a63, 0xc95bd82):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x1a7392d, 0x8d52a63, 0xc95bd82) = (str_key))" % __pyx_checksum
+ */
+  __pyx_tuple__2 = PyTuple_Pack(3, __pyx_int_27736365, __pyx_int_148187747, __pyx_int_211139970); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  /* "bencode2/_decoder.pyx":12
+ *         self.str_key = str_key
  * 
- * class BencodeDecoder:
- *     def __init__(self):             # <<<<<<<<<<<<<<
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
- *             b"l": self.decode_list,
+ *     def decode(self, value: bytes)-> Any:             # <<<<<<<<<<<<<<
+ *         try:
+ *             data, length = self.__decode(value, 0)
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_value, __pyx_n_s_data, __pyx_n_s_length, __pyx_n_s_e); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_init, 11, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode, 12, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 12, __pyx_L1_error)
 
-  /* "bencode2/_decoder.pyx":28
- *         }
- * 
- *     def decode(self, value: bytes) -> Any:             # <<<<<<<<<<<<<<
- *         """
- *         Decode bencode formatted byte string ``value``.
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
  */
-  __pyx_tuple__6 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_value, __pyx_n_s_data, __pyx_n_s_length); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode, 28, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 1, __pyx_L1_error)
 
-  /* "bencode2/_decoder.pyx":49
- *         return data
- * 
- *     def decode_int(self, x, index: int):             # <<<<<<<<<<<<<<
- *         index += 1
- *         new_f = x.index(b"e", index)
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_Decoder__set_state(self, __pyx_state)
  */
-  __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_index, __pyx_n_s_new_f, __pyx_n_s_n); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode_int, 49, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 16, __pyx_L1_error)
 
-  /* "bencode2/_decoder.pyx":62
- *         return n, new_f + 1
- * 
- *     def decode_string(self, x, index: int):             # <<<<<<<<<<<<<<
- *         """Decode torrent bencoded 'string' in x starting at f."""
- *         colon = x.index(b":", index)
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_Decoder(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
  */
-  __pyx_tuple__10 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_index, __pyx_n_s_colon, __pyx_n_s_n, __pyx_n_s_s); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode_string, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 62, __pyx_L1_error)
-
-  /* "bencode2/_decoder.pyx":75
- *         return bytes(s), colon + n
- * 
- *     def decode_list(self, x, index: int):             # <<<<<<<<<<<<<<
- *         r, index = [], index + 1
- * 
- */
-  __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_index, __pyx_n_s_r, __pyx_n_s_v); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode_list, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 75, __pyx_L1_error)
-
-  /* "bencode2/_decoder.pyx":84
- *         return r, index + 1
- * 
- *     def decode_dict(self, x, index: int):             # <<<<<<<<<<<<<<
- *         """Decode bencoded dictionary."""
- *         index += 1
- */
-  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_x, __pyx_n_s_index, __pyx_n_s_r, __pyx_n_s_k); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 84, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__decoder_pyx, __pyx_n_s_decode_dict, 84, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Decoder, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  __pyx_umethod_PyBytes_Type_index.type = (PyObject*)&PyBytes_Type;
+  __pyx_umethod_PyBytes_Type_index.method_name = &__pyx_n_s_index;
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_27736365 = PyInt_FromLong(27736365L); if (unlikely(!__pyx_int_27736365)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_148187747 = PyInt_FromLong(148187747L); if (unlikely(!__pyx_int_148187747)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_211139970 = PyInt_FromLong(211139970L); if (unlikely(!__pyx_int_211139970)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
@@ -5309,18 +5869,57 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
+  __pyx_vtabptr_8bencode2_8_decoder_Decoder = &__pyx_vtable_8bencode2_8_decoder_Decoder;
+  __pyx_vtable_8bencode2_8_decoder_Decoder._Decoder__decode = (PyObject *(*)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *))__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode;
+  __pyx_vtable_8bencode2_8_decoder_Decoder._Decoder__decode_int = (__pyx_ctuple_int__and_int (*)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *))__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_int;
+  __pyx_vtable_8bencode2_8_decoder_Decoder._Decoder__decode_list = (PyObject *(*)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *))__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_list;
+  __pyx_vtable_8bencode2_8_decoder_Decoder._Decoder__decode_str = (PyObject *(*)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *))__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_str;
+  __pyx_vtable_8bencode2_8_decoder_Decoder._Decoder__decode_dict = (PyObject *(*)(struct __pyx_obj_8bencode2_8_decoder_Decoder *, PyObject *, PyObject *))__pyx_f_8bencode2_8_decoder_7Decoder__Decoder__decode_dict;
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_8bencode2_8_decoder_Decoder = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8bencode2_8_decoder_Decoder_spec, NULL); if (unlikely(!__pyx_ptype_8bencode2_8_decoder_Decoder)) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8bencode2_8_decoder_Decoder_spec, __pyx_ptype_8bencode2_8_decoder_Decoder) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  #else
+  __pyx_ptype_8bencode2_8_decoder_Decoder = &__pyx_type_8bencode2_8_decoder_Decoder;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_8bencode2_8_decoder_Decoder) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_8bencode2_8_decoder_Decoder->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8bencode2_8_decoder_Decoder->tp_dictoffset && __pyx_ptype_8bencode2_8_decoder_Decoder->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_8bencode2_8_decoder_Decoder->tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  #endif
+  if (__Pyx_SetVtable(__pyx_ptype_8bencode2_8_decoder_Decoder, __pyx_vtabptr_8bencode2_8_decoder_Decoder) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_MergeVtables(__pyx_ptype_8bencode2_8_decoder_Decoder) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Decoder, (PyObject *) __pyx_ptype_8bencode2_8_decoder_Decoder) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8bencode2_8_decoder_Decoder) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  #endif
   __Pyx_RefNannyFinishContext();
   return 0;
+  __pyx_L1_error:;
+  __Pyx_RefNannyFinishContext();
+  return -1;
 }
 
 static int __Pyx_modinit_type_import_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __Pyx_RefNannyFinishContext();
@@ -5503,15 +6102,14 @@
   int stringtab_initialized = 0;
   #if CYTHON_USE_MODULE_STATE
   int pystate_addmodule_run = 0;
   #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -5610,245 +6208,132 @@
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  (void)__Pyx_modinit_type_init_code();
+  if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "bencode2/_decoder.pyx":3
+  /* "bencode2/_decoder.pyx":2
  * # cython: language_level=3
- * 
- * from collections.abc import Callable             # <<<<<<<<<<<<<<
- * from typing import Any
- * 
- */
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_Callable);
-  __Pyx_GIVEREF(__pyx_n_s_Callable);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Callable)) __PYX_ERR(0, 3, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_collections_abc, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Callable); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Callable, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-  /* "bencode2/_decoder.pyx":4
- * 
- * from collections.abc import Callable
  * from typing import Any             # <<<<<<<<<<<<<<
  * 
- * from ._compat import to_binary
- */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_INCREF(__pyx_n_s_Any);
-  __Pyx_GIVEREF(__pyx_n_s_Any);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_Any)) __PYX_ERR(0, 4, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Any); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Any, __pyx_t_3) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_decoder.pyx":6
- * from typing import Any
- * 
- * from ._compat import to_binary             # <<<<<<<<<<<<<<
  * from ._exceptions import BencodeDecodeError
- * 
  */
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_to_binary);
-  __Pyx_GIVEREF(__pyx_n_s_to_binary);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_to_binary)) __PYX_ERR(0, 6, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_compat, __pyx_t_2, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_Any);
+  __Pyx_GIVEREF(__pyx_n_s_Any);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Any)) __PYX_ERR(0, 2, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_to_binary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Any); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_binary, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Any, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/_decoder.pyx":7
+  /* "bencode2/_decoder.pyx":4
+ * from typing import Any
  * 
- * from ._compat import to_binary
  * from ._exceptions import BencodeDecodeError             # <<<<<<<<<<<<<<
  * 
- * 
+ * cdef class Decoder:
  */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_BencodeDecodeError);
   __Pyx_GIVEREF(__pyx_n_s_BencodeDecodeError);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_BencodeDecodeError)) __PYX_ERR(0, 7, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_exceptions, __pyx_t_3, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_BencodeDecodeError)) __PYX_ERR(0, 4, __pyx_L1_error);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_exceptions, __pyx_t_3, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_BencodeDecodeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeDecodeError, __pyx_t_3) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeDecodeError, __pyx_t_3) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/_decoder.pyx":10
- * 
+  /* "bencode2/_decoder.pyx":12
+ *         self.str_key = str_key
  * 
- * class BencodeDecoder:             # <<<<<<<<<<<<<<
- *     def __init__(self):
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
+ *     def decode(self, value: bytes)-> Any:             # <<<<<<<<<<<<<<
+ *         try:
+ *             data, length = self.__decode(value, 0)
  */
-  __pyx_t_2 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_BencodeDecoder, __pyx_n_s_BencodeDecoder, (PyObject *) NULL, __pyx_n_s_bencode2__decoder, (PyObject *) NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-
-  /* "bencode2/_decoder.pyx":11
- * 
- * class BencodeDecoder:
- *     def __init__(self):             # <<<<<<<<<<<<<<
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
- *             b"l": self.decode_list,
- */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_1__init__, 0, __pyx_n_s_BencodeDecoder___init, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_init, __pyx_t_3) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-  /* "bencode2/_decoder.pyx":28
- *         }
- * 
- *     def decode(self, value: bytes) -> Any:             # <<<<<<<<<<<<<<
- *         """
- *         Decode bencode formatted byte string ``value``.
- */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_value, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_Any) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_3decode, 0, __pyx_n_s_BencodeDecoder_decode, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode, __pyx_t_4) < 0) __PYX_ERR(0, 28, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-
-  /* "bencode2/_decoder.pyx":49
- *         return data
- * 
- *     def decode_int(self, x, index: int):             # <<<<<<<<<<<<<<
- *         index += 1
- *         new_f = x.index(b"e", index)
- */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 49, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_index, __pyx_n_s_int) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_5decode_int, 0, __pyx_n_s_BencodeDecoder_decode_int, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_value, __pyx_n_s_bytes) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_Any) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_7Decoder_3decode, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Decoder_decode, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode_int, __pyx_t_3) < 0) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8bencode2_8_decoder_Decoder, __pyx_n_s_decode, __pyx_t_3) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  PyType_Modified(__pyx_ptype_8bencode2_8_decoder_Decoder);
 
-  /* "bencode2/_decoder.pyx":62
- *         return n, new_f + 1
- * 
- *     def decode_string(self, x, index: int):             # <<<<<<<<<<<<<<
- *         """Decode torrent bencoded 'string' in x starting at f."""
- *         colon = x.index(b":", index)
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     cdef tuple state
+ *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_7Decoder_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Decoder___reduce_cython, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_n_s_int) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_7decode_string, 0, __pyx_n_s_BencodeDecoder_decode_string, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8bencode2_8_decoder_Decoder, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode_string, __pyx_t_4) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  PyType_Modified(__pyx_ptype_8bencode2_8_decoder_Decoder);
 
-  /* "bencode2/_decoder.pyx":75
- *         return bytes(s), colon + n
- * 
- *     def decode_list(self, x, index: int):             # <<<<<<<<<<<<<<
- *         r, index = [], index + 1
- * 
+  /* "(tree fragment)":16
+ *     else:
+ *         return __pyx_unpickle_Decoder, (type(self), 0x1a7392d, state)
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     __pyx_unpickle_Decoder__set_state(self, __pyx_state)
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 75, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_index, __pyx_n_s_int) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_9decode_list, 0, __pyx_n_s_BencodeDecoder_decode_list, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_7Decoder_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Decoder___setstate_cython, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode_list, __pyx_t_3) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8bencode2_8_decoder_Decoder, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  PyType_Modified(__pyx_ptype_8bencode2_8_decoder_Decoder);
 
-  /* "bencode2/_decoder.pyx":84
- *         return r, index + 1
- * 
- *     def decode_dict(self, x, index: int):             # <<<<<<<<<<<<<<
- *         """Decode bencoded dictionary."""
- *         index += 1
+  /* "(tree fragment)":1
+ * def __pyx_unpickle_Decoder(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_1__pyx_unpickle_Decoder, 0, __pyx_n_s_pyx_unpickle_Decoder, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_index, __pyx_n_s_int) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_decoder_14BencodeDecoder_11decode_dict, 0, __pyx_n_s_BencodeDecoder_decode_dict, NULL, __pyx_n_s_bencode2__decoder, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Decoder, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_2, __pyx_n_s_decode_dict, __pyx_t_4) < 0) __PYX_ERR(0, 84, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-
-  /* "bencode2/_decoder.pyx":10
- * 
- * 
- * class BencodeDecoder:             # <<<<<<<<<<<<<<
- *     def __init__(self):
- *         self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
- */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_BencodeDecoder, __pyx_empty_tuple, __pyx_t_2, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeDecoder, __pyx_t_4) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "bencode2/_decoder.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
+ * from typing import Any
  * 
- * from collections.abc import Callable
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init bencode2._decoder", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #else
@@ -6484,28 +6969,14 @@
     }
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
-/* PyObjectSetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_setattro))
-        return tp->tp_setattro(obj, attr_name, value);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_setattr))
-        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
-#endif
-    return PyObject_SetAttr(obj, attr_name, value);
-}
-#endif
-
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     __Pyx_TypeName type_name;
     __Pyx_TypeName obj_type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
@@ -6525,14 +6996,220 @@
         "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
         ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
     __Pyx_DECREF_TypeName(type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
+/* RaiseUnexpectedTypeError */
+static int
+__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
+{
+    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
+                 expected, obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
+/* RaiseTooManyValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
+    PyErr_Format(PyExc_ValueError,
+                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
+}
+
+/* RaiseNeedMoreValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
+    PyErr_Format(PyExc_ValueError,
+                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
+                 index, (index == 1) ? "" : "s");
+}
+
+/* RaiseNoneIterError */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+}
+
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -6845,391 +7522,14 @@
     #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
     return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
     #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
     #endif
 }
 
-/* RaiseUnexpectedTypeError */
-static int
-__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
-{
-    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
-                 expected, obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return 0;
-}
-
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (unlikely(!j)) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
-        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
-        if (mm && mm->mp_subscript) {
-            PyObject *r, *key = PyInt_FromSsize_t(i);
-            if (unlikely(!key)) return NULL;
-            r = mm->mp_subscript(o, key);
-            Py_DECREF(key);
-            return r;
-        }
-        if (likely(sm && sm->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
-                Py_ssize_t l = sm->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return sm->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || !PyMapping_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
-/* PyObjectCallOneArg */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *args[2] = {NULL, arg};
-    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
-/* ObjectGetItem */
-#if CYTHON_USE_TYPE_SLOTS
-static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
-    PyObject *runerr = NULL;
-    Py_ssize_t key_value;
-    key_value = __Pyx_PyIndex_AsSsize_t(index);
-    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
-        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
-    }
-    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
-        __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
-        PyErr_Clear();
-        PyErr_Format(PyExc_IndexError,
-            "cannot fit '" __Pyx_FMT_TYPENAME "' into an index-sized integer", index_type_name);
-        __Pyx_DECREF_TypeName(index_type_name);
-    }
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
-    __Pyx_TypeName obj_type_name;
-    if (likely(PyType_Check(obj))) {
-        PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
-        if (!meth) {
-            PyErr_Clear();
-        } else {
-            PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
-            Py_DECREF(meth);
-            return result;
-        }
-    }
-    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError,
-        "'" __Pyx_FMT_TYPENAME "' object is not subscriptable", obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return NULL;
-}
-static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key) {
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyMappingMethods *mm = tp->tp_as_mapping;
-    PySequenceMethods *sm = tp->tp_as_sequence;
-    if (likely(mm && mm->mp_subscript)) {
-        return mm->mp_subscript(obj, key);
-    }
-    if (likely(sm && sm->sq_item)) {
-        return __Pyx_PyObject_GetIndex(obj, key);
-    }
-    return __Pyx_PyObject_GetItem_Slow(obj, key);
-}
-#endif
-
-/* RaiseTooManyValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* IterFinish */
-static CYTHON_INLINE int __Pyx_IterFinish(void) {
-    PyObject* exc_type;
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    exc_type = __Pyx_PyErr_CurrentExceptionType();
-    if (unlikely(exc_type)) {
-        if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
-            return -1;
-        __Pyx_PyErr_Clear();
-        return 0;
-    }
-    return 0;
-}
-
-/* UnpackItemEndCheck */
-static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
-    if (unlikely(retval)) {
-        Py_DECREF(retval);
-        __Pyx_RaiseTooManyValuesError(expected);
-        return -1;
-    }
-    return __Pyx_IterFinish();
-}
-
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    PyObject *exc_value = exc_info->exc_value;
-    if (exc_value == NULL || exc_value == Py_None) {
-        *value = NULL;
-        *type = NULL;
-        *tb = NULL;
-    } else {
-        *value = exc_value;
-        Py_INCREF(*value);
-        *type = (PyObject*) Py_TYPE(exc_value);
-        Py_INCREF(*type);
-        *tb = PyException_GetTraceback(exc_value);
-    }
-  #elif CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-  #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-  #endif
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    PyObject *tmp_value = exc_info->exc_value;
-    exc_info->exc_value = value;
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-  #else
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-  #endif
-}
-#endif
-
-/* GetException */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
-#endif
-{
-    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-  #if PY_VERSION_HEX >= 0x030C00A6
-    local_value = tstate->current_exception;
-    tstate->current_exception = 0;
-    if (likely(local_value)) {
-        local_type = (PyObject*) Py_TYPE(local_value);
-        Py_INCREF(local_type);
-        local_tb = PyException_GetTraceback(local_value);
-    }
-  #else
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-  #endif
-#else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
-#endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
-    if (unlikely(tstate->current_exception))
-#elif CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
-#else
-    if (unlikely(PyErr_Occurred()))
-#endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
-    }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
-    {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-      #if PY_VERSION_HEX >= 0x030B00a4
-        tmp_value = exc_info->exc_value;
-        exc_info->exc_value = local_value;
-        tmp_type = NULL;
-        tmp_tb = NULL;
-        Py_XDECREF(local_type);
-        Py_XDECREF(local_tb);
-      #else
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
-      #endif
-    }
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
-#endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
-}
-
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
     __Pyx_PyThreadState_declare
     CYTHON_UNUSED_VAR(cause);
     Py_XINCREF(type);
     if (!value || value == Py_None)
@@ -7383,116 +7683,404 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* SliceObject */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetSlice(PyObject* obj,
-        Py_ssize_t cstart, Py_ssize_t cstop,
-        PyObject** _py_start, PyObject** _py_stop, PyObject** _py_slice,
-        int has_cstart, int has_cstop, int wraparound) {
-    __Pyx_TypeName obj_type_name;
-#if CYTHON_USE_TYPE_SLOTS
-    PyMappingMethods* mp;
-#if PY_MAJOR_VERSION < 3
-    PySequenceMethods* ms = Py_TYPE(obj)->tp_as_sequence;
-    if (likely(ms && ms->sq_slice)) {
-        if (!has_cstart) {
-            if (_py_start && (*_py_start != Py_None)) {
-                cstart = __Pyx_PyIndex_AsSsize_t(*_py_start);
-                if ((cstart == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
-            } else
-                cstart = 0;
+/* SwapException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_value = exc_info->exc_value;
+    exc_info->exc_value = *value;
+    if (tmp_value == NULL || tmp_value == Py_None) {
+        Py_XDECREF(tmp_value);
+        tmp_value = NULL;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+    } else {
+        tmp_type = (PyObject*) Py_TYPE(tmp_value);
+        Py_INCREF(tmp_type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        tmp_tb = ((PyBaseExceptionObject*) tmp_value)->traceback;
+        Py_XINCREF(tmp_tb);
+        #else
+        tmp_tb = PyException_GetTraceback(tmp_value);
+        #endif
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = *type;
+    exc_info->exc_value = *value;
+    exc_info->exc_traceback = *tb;
+  #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = *type;
+    tstate->exc_value = *value;
+    tstate->exc_traceback = *tb;
+  #endif
+    *type = tmp_type;
+    *value = tmp_value;
+    *tb = tmp_tb;
+}
+#else
+static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    PyErr_GetExcInfo(&tmp_type, &tmp_value, &tmp_tb);
+    PyErr_SetExcInfo(*type, *value, *tb);
+    *type = tmp_type;
+    *value = tmp_value;
+    *tb = tmp_tb;
+}
+#endif
+
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (unlikely(!j)) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
         }
-        if (!has_cstop) {
-            if (_py_stop && (*_py_stop != Py_None)) {
-                cstop = __Pyx_PyIndex_AsSsize_t(*_py_stop);
-                if ((cstop == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
-            } else
-                cstop = PY_SSIZE_T_MAX;
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
         }
-        if (wraparound && unlikely((cstart < 0) | (cstop < 0)) && likely(ms->sq_length)) {
-            Py_ssize_t l = ms->sq_length(obj);
-            if (likely(l >= 0)) {
-                if (cstop < 0) {
-                    cstop += l;
-                    if (cstop < 0) cstop = 0;
-                }
-                if (cstart < 0) {
-                    cstart += l;
-                    if (cstart < 0) cstart = 0;
+    } else {
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_subscript) {
+            PyObject *r, *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return NULL;
+            r = mm->mp_subscript(o, key);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
                 }
-            } else {
-                if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                    goto bad;
-                PyErr_Clear();
             }
+            return sm->sq_item(o, i);
         }
-        return ms->sq_slice(obj, cstart, cstop);
     }
 #else
-    CYTHON_UNUSED_VAR(wraparound);
+    if (is_list || !PyMapping_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
 #endif
-    mp = Py_TYPE(obj)->tp_as_mapping;
-    if (likely(mp && mp->mp_subscript))
-#else
-    CYTHON_UNUSED_VAR(wraparound);
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
+/* PyObjectCallOneArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* ObjectGetItem */
+#if CYTHON_USE_TYPE_SLOTS
+static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
+    PyObject *runerr = NULL;
+    Py_ssize_t key_value;
+    key_value = __Pyx_PyIndex_AsSsize_t(index);
+    if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
+        return __Pyx_GetItemInt_Fast(obj, key_value, 0, 1, 1);
+    }
+    if (PyErr_GivenExceptionMatches(runerr, PyExc_OverflowError)) {
+        __Pyx_TypeName index_type_name = __Pyx_PyType_GetName(Py_TYPE(index));
+        PyErr_Clear();
+        PyErr_Format(PyExc_IndexError,
+            "cannot fit '" __Pyx_FMT_TYPENAME "' into an index-sized integer", index_type_name);
+        __Pyx_DECREF_TypeName(index_type_name);
+    }
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
+    __Pyx_TypeName obj_type_name;
+    if (likely(PyType_Check(obj))) {
+        PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
+        if (!meth) {
+            PyErr_Clear();
+        } else {
+            PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
+            Py_DECREF(meth);
+            return result;
+        }
+    }
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+        "'" __Pyx_FMT_TYPENAME "' object is not subscriptable", obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return NULL;
+}
+static PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key) {
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyMappingMethods *mm = tp->tp_as_mapping;
+    PySequenceMethods *sm = tp->tp_as_sequence;
+    if (likely(mm && mm->mp_subscript)) {
+        return mm->mp_subscript(obj, key);
+    }
+    if (likely(sm && sm->sq_item)) {
+        return __Pyx_PyObject_GetIndex(obj, key);
+    }
+    return __Pyx_PyObject_GetItem_Slow(obj, key);
+}
 #endif
-    {
-        PyObject* result;
-        PyObject *py_slice, *py_start, *py_stop;
-        if (_py_slice) {
-            py_slice = *_py_slice;
+
+/* JoinPyUnicode */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char) {
+#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    PyObject *result_uval;
+    int result_ukind, kind_shift;
+    Py_ssize_t i, char_pos;
+    void *result_udata;
+    CYTHON_MAYBE_UNUSED_VAR(max_char);
+#if CYTHON_PEP393_ENABLED
+    result_uval = PyUnicode_New(result_ulength, max_char);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
+    kind_shift = (result_ukind == PyUnicode_4BYTE_KIND) ? 2 : result_ukind - 1;
+    result_udata = PyUnicode_DATA(result_uval);
+#else
+    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = sizeof(Py_UNICODE);
+    kind_shift = (result_ukind == 4) ? 2 : result_ukind - 1;
+    result_udata = PyUnicode_AS_UNICODE(result_uval);
+#endif
+    assert(kind_shift == 2 || kind_shift == 1 || kind_shift == 0);
+    char_pos = 0;
+    for (i=0; i < value_count; i++) {
+        int ukind;
+        Py_ssize_t ulength;
+        void *udata;
+        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
+        if (unlikely(__Pyx_PyUnicode_READY(uval)))
+            goto bad;
+        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
+        if (unlikely(!ulength))
+            continue;
+        if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
+            goto overflow;
+        ukind = __Pyx_PyUnicode_KIND(uval);
+        udata = __Pyx_PyUnicode_DATA(uval);
+        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
+            memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
-            PyObject* owned_start = NULL;
-            PyObject* owned_stop = NULL;
-            if (_py_start) {
-                py_start = *_py_start;
-            } else {
-                if (has_cstart) {
-                    owned_start = py_start = PyInt_FromSsize_t(cstart);
-                    if (unlikely(!py_start)) goto bad;
-                } else
-                    py_start = Py_None;
-            }
-            if (_py_stop) {
-                py_stop = *_py_stop;
-            } else {
-                if (has_cstop) {
-                    owned_stop = py_stop = PyInt_FromSsize_t(cstop);
-                    if (unlikely(!py_stop)) {
-                        Py_XDECREF(owned_start);
-                        goto bad;
-                    }
-                } else
-                    py_stop = Py_None;
+            #if PY_VERSION_HEX >= 0x030d0000
+            if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
+            #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
+            #else
+            Py_ssize_t j;
+            for (j=0; j < ulength; j++) {
+                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
+                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
             }
-            py_slice = PySlice_New(py_start, py_stop, Py_None);
-            Py_XDECREF(owned_start);
-            Py_XDECREF(owned_stop);
-            if (unlikely(!py_slice)) goto bad;
+            #endif
         }
-#if CYTHON_USE_TYPE_SLOTS
-        result = mp->mp_subscript(obj, py_slice);
+        char_pos += ulength;
+    }
+    return result_uval;
+overflow:
+    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
+bad:
+    Py_DECREF(result_uval);
+    return NULL;
 #else
-        result = PyObject_GetItem(obj, py_slice);
+    CYTHON_UNUSED_VAR(max_char);
+    CYTHON_UNUSED_VAR(result_ulength);
+    CYTHON_UNUSED_VAR(value_count);
+    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
 #endif
-        if (!_py_slice) {
-            Py_DECREF(py_slice);
+}
+
+/* UnpackUnboundCMethod */
+static PyObject *__Pyx_SelflessCall(PyObject *method, PyObject *args, PyObject *kwargs) {
+    PyObject *result;
+    PyObject *selfless_args = PyTuple_GetSlice(args, 1, PyTuple_Size(args));
+    if (unlikely(!selfless_args)) return NULL;
+    result = PyObject_Call(method, selfless_args, kwargs);
+    Py_DECREF(selfless_args);
+    return result;
+}
+static PyMethodDef __Pyx_UnboundCMethod_Def = {
+     "CythonUnboundCMethod",
+     __PYX_REINTERPRET_FUNCION(PyCFunction, __Pyx_SelflessCall),
+     METH_VARARGS | METH_KEYWORDS,
+     NULL
+};
+static int __Pyx_TryUnpackUnboundCMethod(__Pyx_CachedCFunction* target) {
+    PyObject *method;
+    method = __Pyx_PyObject_GetAttrStr(target->type, *target->method_name);
+    if (unlikely(!method))
+        return -1;
+    target->method = method;
+#if CYTHON_COMPILING_IN_CPYTHON
+    #if PY_MAJOR_VERSION >= 3
+    if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
+    #else
+    if (likely(!__Pyx_CyOrPyCFunction_Check(method)))
+    #endif
+    {
+        PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
+        target->func = descr->d_method->ml_meth;
+        target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
+    } else
+#endif
+#if CYTHON_COMPILING_IN_PYPY
+#else
+    if (PyCFunction_Check(method))
+#endif
+    {
+        PyObject *self;
+        int self_found;
+#if CYTHON_COMPILING_IN_LIMITED_API || CYTHON_COMPILING_IN_PYPY
+        self = PyObject_GetAttrString(method, "__self__");
+        if (!self) {
+            PyErr_Clear();
+        }
+#else
+        self = PyCFunction_GET_SELF(method);
+#endif
+        self_found = (self && self != Py_None);
+#if CYTHON_COMPILING_IN_LIMITED_API || CYTHON_COMPILING_IN_PYPY
+        Py_XDECREF(self);
+#endif
+        if (self_found) {
+            PyObject *unbound_method = PyCFunction_New(&__Pyx_UnboundCMethod_Def, method);
+            if (unlikely(!unbound_method)) return -1;
+            Py_DECREF(method);
+            target->method = unbound_method;
         }
-        return result;
     }
-    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError,
-        "'" __Pyx_FMT_TYPENAME "' object is unsliceable", obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
+/* CallUnboundCMethod2 */
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
+static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2) {
+    if (likely(cfunc->func)) {
+        PyObject *args[2] = {arg1, arg2};
+        if (cfunc->flag == METH_FASTCALL) {
+            #if PY_VERSION_HEX >= 0x030700A0
+            return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, args, 2);
+            #else
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, 2, NULL);
+            #endif
+        }
+        #if PY_VERSION_HEX >= 0x030700A0
+        if (cfunc->flag == (METH_FASTCALL | METH_KEYWORDS))
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, 2, NULL);
+        #endif
+    }
+    return __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2);
+}
+#endif
+static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2){
+    PyObject *args, *result = NULL;
+    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
+        args = PyTuple_New(2);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(arg1);
+        PyTuple_SET_ITEM(args, 0, arg1);
+        Py_INCREF(arg2);
+        PyTuple_SET_ITEM(args, 1, arg2);
+        if (cfunc->flag & METH_KEYWORDS)
+            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
+        else
+            result = (*cfunc->func)(self, args);
+    } else {
+        args = PyTuple_New(3);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(self);
+        PyTuple_SET_ITEM(args, 0, self);
+        Py_INCREF(arg1);
+        PyTuple_SET_ITEM(args, 1, arg1);
+        Py_INCREF(arg2);
+        PyTuple_SET_ITEM(args, 2, arg2);
+        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+    }
+#else
+    args = PyTuple_Pack(3, self, arg1, arg2);
+    if (unlikely(!args)) goto bad;
+    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+#endif
 bad:
-    return NULL;
+    Py_XDECREF(args);
+    return result;
 }
 
 /* PyIntBinop */
 #if !CYTHON_COMPILING_IN_PYPY
 static PyObject* __Pyx_PyInt_AddObjC(PyObject *op1, PyObject *op2, long intval, int inplace, int zerodivision_check) {
     CYTHON_MAYBE_UNUSED_VAR(intval);
     CYTHON_MAYBE_UNUSED_VAR(inplace);
@@ -7620,14 +8208,120 @@
             PyFPE_END_PROTECT(result)
             return PyFloat_FromDouble(result);
     }
     return (inplace ? PyNumber_InPlaceAdd : PyNumber_Add)(op1, op2);
 }
 #endif
 
+/* KeywordStringCheck */
+static int __Pyx_CheckKeywordStrings(
+    PyObject *kw,
+    const char* function_name,
+    int kw_allowed)
+{
+    PyObject* key = 0;
+    Py_ssize_t pos = 0;
+#if CYTHON_COMPILING_IN_PYPY
+    if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
+        goto invalid_keyword;
+    return 1;
+#else
+    if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
+        Py_ssize_t kwsize;
+#if CYTHON_ASSUME_SAFE_MACROS
+        kwsize = PyTuple_GET_SIZE(kw);
+#else
+        kwsize = PyTuple_Size(kw);
+        if (kwsize < 0) return 0;
+#endif
+        if (unlikely(kwsize == 0))
+            return 1;
+        if (!kw_allowed) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            key = PyTuple_GET_ITEM(kw, 0);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
+            goto invalid_keyword;
+        }
+#if PY_VERSION_HEX < 0x03090000
+        for (pos = 0; pos < kwsize; pos++) {
+#if CYTHON_ASSUME_SAFE_MACROS
+            key = PyTuple_GET_ITEM(kw, pos);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+        }
+#endif
+        return 1;
+    }
+    while (PyDict_Next(kw, &pos, &key, 0)) {
+        #if PY_MAJOR_VERSION < 3
+        if (unlikely(!PyString_Check(key)))
+        #endif
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+    }
+    if (!kw_allowed && unlikely(key))
+        goto invalid_keyword;
+    return 1;
+invalid_keyword_type:
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() keywords must be strings", function_name);
+    return 0;
+#endif
+invalid_keyword:
+    #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() got an unexpected keyword argument '%.200s'",
+        function_name, PyString_AsString(key));
+    #else
+    PyErr_Format(PyExc_TypeError,
+        "%s() got an unexpected keyword argument '%U'",
+        function_name, key);
+    #endif
+    return 0;
+}
+
+/* GetAttr3 */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
+static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        return NULL;
+    __Pyx_PyErr_Clear();
+    Py_INCREF(d);
+    return d;
+}
+#endif
+static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
+    PyObject *r;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    int res = PyObject_GetOptionalAttr(o, n, &r);
+    return (res != 0) ? r : __Pyx_NewRef(d);
+#else
+  #if CYTHON_USE_TYPE_SLOTS
+    if (likely(PyString_Check(n))) {
+        r = __Pyx_PyObject_GetAttrStrNoError(o, n);
+        if (unlikely(!r) && likely(!PyErr_Occurred())) {
+            r = __Pyx_NewRef(d);
+        }
+        return r;
+    }
+  #endif
+    r = PyObject_GetAttr(o, n);
+    return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
+#endif
+}
+
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
     PyObject *module = 0;
     PyObject *empty_dict = 0;
     PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
@@ -7721,14 +8415,47 @@
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
+#if PY_MAJOR_VERSION >= 3
+    if (likely(PyUnicode_Check(n)))
+#else
+    if (likely(PyString_Check(n)))
+#endif
+        return __Pyx_PyObject_GetAttrStr(o, n);
+#endif
+    return PyObject_GetAttr(o, n);
+}
+
+/* HasAttr */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
+static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
+    PyObject *r;
+    if (unlikely(!__Pyx_PyBaseString_Check(n))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "hasattr(): attribute name must be string");
+        return -1;
+    }
+    r = __Pyx_GetAttr(o, n);
+    if (!r) {
+        PyErr_Clear();
+        return 0;
+    } else {
+        Py_DECREF(r);
+        return 1;
+    }
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
@@ -7794,14 +8521,558 @@
             PyType_Modified(type);
     }
 #endif
     return 0;
 }
 #endif
 
+/* PyObjectCallNoArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectGetMethod */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
+#else
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
+#endif
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
+    }
+#endif
+    *method = attr;
+    return 0;
+}
+
+/* PyObjectCallMethod0 */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
+}
+
+/* ValidateBasesTuple */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
+    Py_ssize_t i, n;
+#if CYTHON_ASSUME_SAFE_MACROS
+    n = PyTuple_GET_SIZE(bases);
+#else
+    n = PyTuple_Size(bases);
+    if (n < 0) return -1;
+#endif
+    for (i = 1; i < n; i++)
+    {
+#if CYTHON_AVOID_BORROWED_REFS
+        PyObject *b0 = PySequence_GetItem(bases, i);
+        if (!b0) return -1;
+#elif CYTHON_ASSUME_SAFE_MACROS
+        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+#else
+        PyObject *b0 = PyTuple_GetItem(bases, i);
+        if (!b0) return -1;
+#endif
+        PyTypeObject *b;
+#if PY_MAJOR_VERSION < 3
+        if (PyClass_Check(b0))
+        {
+            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
+                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+#endif
+        b = (PyTypeObject*) b0;
+        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
+            __Pyx_DECREF_TypeName(b_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+        if (dictoffset == 0)
+        {
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+                Py_DECREF(b0);
+#endif
+                return -1;
+            }
+        }
+#if CYTHON_AVOID_BORROWED_REFS
+        Py_DECREF(b0);
+#endif
+    }
+    return 0;
+}
+#endif
+
+/* PyType_Ready */
+static int __Pyx_PyType_Ready(PyTypeObject *t) {
+#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
+    (void)__Pyx_PyObject_CallMethod0;
+#if CYTHON_USE_TYPE_SPECS
+    (void)__Pyx_validate_bases_tuple;
+#endif
+    return PyType_Ready(t);
+#else
+    int r;
+    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
+    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
+        return -1;
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+    {
+        int gc_was_enabled;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        gc_was_enabled = PyGC_Disable();
+        (void)__Pyx_PyObject_CallMethod0;
+    #else
+        PyObject *ret, *py_status;
+        PyObject *gc = NULL;
+        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
+        gc = PyImport_GetModule(__pyx_kp_u_gc);
+        #endif
+        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
+        if (unlikely(!gc)) return -1;
+        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
+        if (unlikely(!py_status)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
+        Py_DECREF(py_status);
+        if (gc_was_enabled > 0) {
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
+            if (unlikely(!ret)) {
+                Py_DECREF(gc);
+                return -1;
+            }
+            Py_DECREF(ret);
+        } else if (unlikely(gc_was_enabled == -1)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+    #endif
+        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
+#else
+        (void)__Pyx_PyObject_CallMethod0;
+#endif
+    r = PyType_Ready(t);
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        if (gc_was_enabled)
+            PyGC_Enable();
+    #else
+        if (gc_was_enabled) {
+            PyObject *tp, *v, *tb;
+            PyErr_Fetch(&tp, &v, &tb);
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
+            if (likely(ret || r == -1)) {
+                Py_XDECREF(ret);
+                PyErr_Restore(tp, v, tb);
+            } else {
+                Py_XDECREF(tp);
+                Py_XDECREF(v);
+                Py_XDECREF(tb);
+                r = -1;
+            }
+        }
+        Py_DECREF(gc);
+    #endif
+    }
+#endif
+    return r;
+#endif
+}
+
+/* PyObject_GenericGetAttrNoDict */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, attr_name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(attr_name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
+    PyObject *descr;
+    PyTypeObject *tp = Py_TYPE(obj);
+    if (unlikely(!PyString_Check(attr_name))) {
+        return PyObject_GenericGetAttr(obj, attr_name);
+    }
+    assert(!tp->tp_dictoffset);
+    descr = _PyType_Lookup(tp, attr_name);
+    if (unlikely(!descr)) {
+        return __Pyx_RaiseGenericGetAttributeError(tp, attr_name);
+    }
+    Py_INCREF(descr);
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_HAVE_CLASS)))
+    #endif
+    {
+        descrgetfunc f = Py_TYPE(descr)->tp_descr_get;
+        if (unlikely(f)) {
+            PyObject *res = f(descr, obj, (PyObject *)tp);
+            Py_DECREF(descr);
+            return res;
+        }
+    }
+    return descr;
+}
+#endif
+
+/* PyObject_GenericGetAttr */
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
+static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name) {
+    if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
+        return PyObject_GenericGetAttr(obj, attr_name);
+    }
+    return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
+}
+#endif
+
+/* SetVTable */
+static int __Pyx_SetVtable(PyTypeObject *type, void *vtable) {
+    PyObject *ob = PyCapsule_New(vtable, 0, 0);
+    if (unlikely(!ob))
+        goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(PyObject_SetAttr((PyObject *) type, __pyx_n_s_pyx_vtable, ob) < 0))
+#else
+    if (unlikely(PyDict_SetItem(type->tp_dict, __pyx_n_s_pyx_vtable, ob) < 0))
+#endif
+        goto bad;
+    Py_DECREF(ob);
+    return 0;
+bad:
+    Py_XDECREF(ob);
+    return -1;
+}
+
+/* GetVTable */
+static void* __Pyx_GetVtable(PyTypeObject *type) {
+    void* ptr;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *ob = PyObject_GetAttr((PyObject *)type, __pyx_n_s_pyx_vtable);
+#else
+    PyObject *ob = PyObject_GetItem(type->tp_dict, __pyx_n_s_pyx_vtable);
+#endif
+    if (!ob)
+        goto bad;
+    ptr = PyCapsule_GetPointer(ob, 0);
+    if (!ptr && !PyErr_Occurred())
+        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
+    Py_DECREF(ob);
+    return ptr;
+bad:
+    Py_XDECREF(ob);
+    return NULL;
+}
+
+/* MergeVTables */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_MergeVtables(PyTypeObject *type) {
+    int i;
+    void** base_vtables;
+    __Pyx_TypeName tp_base_name;
+    __Pyx_TypeName base_name;
+    void* unknown = (void*)-1;
+    PyObject* bases = type->tp_bases;
+    int base_depth = 0;
+    {
+        PyTypeObject* base = type->tp_base;
+        while (base) {
+            base_depth += 1;
+            base = base->tp_base;
+        }
+    }
+    base_vtables = (void**) malloc(sizeof(void*) * (size_t)(base_depth + 1));
+    base_vtables[0] = unknown;
+    for (i = 1; i < PyTuple_GET_SIZE(bases); i++) {
+        void* base_vtable = __Pyx_GetVtable(((PyTypeObject*)PyTuple_GET_ITEM(bases, i)));
+        if (base_vtable != NULL) {
+            int j;
+            PyTypeObject* base = type->tp_base;
+            for (j = 0; j < base_depth; j++) {
+                if (base_vtables[j] == unknown) {
+                    base_vtables[j] = __Pyx_GetVtable(base);
+                    base_vtables[j + 1] = unknown;
+                }
+                if (base_vtables[j] == base_vtable) {
+                    break;
+                } else if (base_vtables[j] == NULL) {
+                    goto bad;
+                }
+                base = base->tp_base;
+            }
+        }
+    }
+    PyErr_Clear();
+    free(base_vtables);
+    return 0;
+bad:
+    tp_base_name = __Pyx_PyType_GetName(type->tp_base);
+    base_name = __Pyx_PyType_GetName((PyTypeObject*)PyTuple_GET_ITEM(bases, i));
+    PyErr_Format(PyExc_TypeError,
+        "multiple bases have vtable conflict: '" __Pyx_FMT_TYPENAME "' and '" __Pyx_FMT_TYPENAME "'", tp_base_name, base_name);
+    __Pyx_DECREF_TypeName(tp_base_name);
+    __Pyx_DECREF_TypeName(base_name);
+    free(base_vtables);
+    return -1;
+}
+#endif
+
+/* SetupReduce */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
+  int ret;
+  PyObject *name_attr;
+  name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name);
+  if (likely(name_attr)) {
+      ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
+  } else {
+      ret = -1;
+  }
+  if (unlikely(ret < 0)) {
+      PyErr_Clear();
+      ret = 0;
+  }
+  Py_XDECREF(name_attr);
+  return ret;
+}
+static int __Pyx_setup_reduce(PyObject* type_obj) {
+    int ret = 0;
+    PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
+    PyObject *object_reduce_ex = NULL;
+    PyObject *reduce = NULL;
+    PyObject *reduce_ex = NULL;
+    PyObject *reduce_cython = NULL;
+    PyObject *setstate = NULL;
+    PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
+#if CYTHON_USE_PYTYPE_LOOKUP
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+#else
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
+#if CYTHON_USE_PYTYPE_LOOKUP
+    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+#else
+    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
+#endif
+    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
+    if (reduce_ex == object_reduce_ex) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+#else
+        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+#endif
+        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
+        if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
+            reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
+            if (likely(reduce_cython)) {
+                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+            } else if (reduce == object_reduce || PyErr_Occurred()) {
+                goto __PYX_BAD;
+            }
+            setstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate);
+            if (!setstate) PyErr_Clear();
+            if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
+                setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
+                if (likely(setstate_cython)) {
+                    ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                    ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
+                } else if (!setstate || PyErr_Occurred()) {
+                    goto __PYX_BAD;
+                }
+            }
+            PyType_Modified((PyTypeObject*)type_obj);
+        }
+    }
+    goto __PYX_GOOD;
+__PYX_BAD:
+    if (!PyErr_Occurred()) {
+        __Pyx_TypeName type_obj_name =
+            __Pyx_PyType_GetName((PyTypeObject*)type_obj);
+        PyErr_Format(PyExc_RuntimeError,
+            "Unable to initialize pickling for " __Pyx_FMT_TYPENAME, type_obj_name);
+        __Pyx_DECREF_TypeName(type_obj_name);
+    }
+    ret = -1;
+__PYX_GOOD:
+#if !CYTHON_USE_PYTYPE_LOOKUP
+    Py_XDECREF(object_reduce);
+    Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
+#endif
+    Py_XDECREF(reduce);
+    Py_XDECREF(reduce_ex);
+    Py_XDECREF(reduce_cython);
+    Py_XDECREF(setstate);
+    Py_XDECREF(setstate_cython);
+    return ret;
+}
+#endif
+
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
     return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
@@ -8971,301 +10242,14 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
-/* CalculateMetaclass */
-static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
-    Py_ssize_t i, nbases;
-#if CYTHON_ASSUME_SAFE_MACROS
-    nbases = PyTuple_GET_SIZE(bases);
-#else
-    nbases = PyTuple_Size(bases);
-    if (nbases < 0) return NULL;
-#endif
-    for (i=0; i < nbases; i++) {
-        PyTypeObject *tmptype;
-#if CYTHON_ASSUME_SAFE_MACROS
-        PyObject *tmp = PyTuple_GET_ITEM(bases, i);
-#else
-        PyObject *tmp = PyTuple_GetItem(bases, i);
-        if (!tmp) return NULL;
-#endif
-        tmptype = Py_TYPE(tmp);
-#if PY_MAJOR_VERSION < 3
-        if (tmptype == &PyClass_Type)
-            continue;
-#endif
-        if (!metaclass) {
-            metaclass = tmptype;
-            continue;
-        }
-        if (PyType_IsSubtype(metaclass, tmptype))
-            continue;
-        if (PyType_IsSubtype(tmptype, metaclass)) {
-            metaclass = tmptype;
-            continue;
-        }
-        PyErr_SetString(PyExc_TypeError,
-                        "metaclass conflict: "
-                        "the metaclass of a derived class "
-                        "must be a (non-strict) subclass "
-                        "of the metaclasses of all its bases");
-        return NULL;
-    }
-    if (!metaclass) {
-#if PY_MAJOR_VERSION < 3
-        metaclass = &PyClass_Type;
-#else
-        metaclass = &PyType_Type;
-#endif
-    }
-    Py_INCREF((PyObject*) metaclass);
-    return (PyObject*) metaclass;
-}
-
-/* PyObjectCall2Args */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args[3] = {NULL, arg1, arg2};
-    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
-/* PyObjectLookupSpecial */
-#if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error) {
-    PyObject *res;
-    PyTypeObject *tp = Py_TYPE(obj);
-#if PY_MAJOR_VERSION < 3
-    if (unlikely(PyInstance_Check(obj)))
-        return with_error ? __Pyx_PyObject_GetAttrStr(obj, attr_name) : __Pyx_PyObject_GetAttrStrNoError(obj, attr_name);
-#endif
-    res = _PyType_Lookup(tp, attr_name);
-    if (likely(res)) {
-        descrgetfunc f = Py_TYPE(res)->tp_descr_get;
-        if (!f) {
-            Py_INCREF(res);
-        } else {
-            res = f(res, obj, (PyObject *)tp);
-        }
-    } else if (with_error) {
-        PyErr_SetObject(PyExc_AttributeError, attr_name);
-    }
-    return res;
-}
-#endif
-
-/* Py3ClassCreate */
-static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
-                                           PyObject *qualname, PyObject *mkw, PyObject *modname, PyObject *doc) {
-    PyObject *ns;
-    if (metaclass) {
-        PyObject *prep = __Pyx_PyObject_GetAttrStrNoError(metaclass, __pyx_n_s_prepare);
-        if (prep) {
-            PyObject *pargs[3] = {NULL, name, bases};
-            ns = __Pyx_PyObject_FastCallDict(prep, pargs+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET, mkw);
-            Py_DECREF(prep);
-        } else {
-            if (unlikely(PyErr_Occurred()))
-                return NULL;
-            ns = PyDict_New();
-        }
-    } else {
-        ns = PyDict_New();
-    }
-    if (unlikely(!ns))
-        return NULL;
-    if (unlikely(PyObject_SetItem(ns, __pyx_n_s_module, modname) < 0)) goto bad;
-#if PY_VERSION_HEX >= 0x03030000
-    if (unlikely(PyObject_SetItem(ns, __pyx_n_s_qualname, qualname) < 0)) goto bad;
-#else
-    CYTHON_MAYBE_UNUSED_VAR(qualname);
-#endif
-    if (unlikely(doc && PyObject_SetItem(ns, __pyx_n_s_doc, doc) < 0)) goto bad;
-    return ns;
-bad:
-    Py_DECREF(ns);
-    return NULL;
-}
-#if PY_VERSION_HEX < 0x030600A4 && CYTHON_PEP487_INIT_SUBCLASS
-static int __Pyx_SetNamesPEP487(PyObject *type_obj) {
-    PyTypeObject *type = (PyTypeObject*) type_obj;
-    PyObject *names_to_set, *key, *value, *set_name, *tmp;
-    Py_ssize_t i = 0;
-#if CYTHON_USE_TYPE_SLOTS
-    names_to_set = PyDict_Copy(type->tp_dict);
-#else
-    {
-        PyObject *d = PyObject_GetAttr(type_obj, __pyx_n_s_dict);
-        names_to_set = NULL;
-        if (likely(d)) {
-            PyObject *names_to_set = PyDict_New();
-            int ret = likely(names_to_set) ? PyDict_Update(names_to_set, d) : -1;
-            Py_DECREF(d);
-            if (unlikely(ret < 0))
-                Py_CLEAR(names_to_set);
-        }
-    }
-#endif
-    if (unlikely(names_to_set == NULL))
-        goto bad;
-    while (PyDict_Next(names_to_set, &i, &key, &value)) {
-        set_name = __Pyx_PyObject_LookupSpecialNoError(value, __pyx_n_s_set_name);
-        if (unlikely(set_name != NULL)) {
-            tmp = __Pyx_PyObject_Call2Args(set_name, type_obj, key);
-            Py_DECREF(set_name);
-            if (unlikely(tmp == NULL)) {
-                __Pyx_TypeName value_type_name =
-                    __Pyx_PyType_GetName(Py_TYPE(value));
-                __Pyx_TypeName type_name = __Pyx_PyType_GetName(type);
-                PyErr_Format(PyExc_RuntimeError,
-#if PY_MAJOR_VERSION >= 3
-                    "Error calling __set_name__ on '" __Pyx_FMT_TYPENAME "' instance %R " "in '" __Pyx_FMT_TYPENAME "'",
-                    value_type_name, key, type_name);
-#else
-                    "Error calling __set_name__ on '" __Pyx_FMT_TYPENAME "' instance %.100s in '" __Pyx_FMT_TYPENAME "'",
-                    value_type_name,
-                    PyString_Check(key) ? PyString_AS_STRING(key) : "?",
-                    type_name);
-#endif
-                goto bad;
-            } else {
-                Py_DECREF(tmp);
-            }
-        }
-        else if (unlikely(PyErr_Occurred())) {
-            goto bad;
-        }
-    }
-    Py_DECREF(names_to_set);
-    return 0;
-bad:
-    Py_XDECREF(names_to_set);
-    return -1;
-}
-static PyObject *__Pyx_InitSubclassPEP487(PyObject *type_obj, PyObject *mkw) {
-#if CYTHON_USE_TYPE_SLOTS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    PyTypeObject *type = (PyTypeObject*) type_obj;
-    PyObject *mro = type->tp_mro;
-    Py_ssize_t i, nbases;
-    if (unlikely(!mro)) goto done;
-    (void) &__Pyx_GetBuiltinName;
-    Py_INCREF(mro);
-    nbases = PyTuple_GET_SIZE(mro);
-    assert(PyTuple_GET_ITEM(mro, 0) == type_obj);
-    for (i = 1; i < nbases-1; i++) {
-        PyObject *base, *dict, *meth;
-        base = PyTuple_GET_ITEM(mro, i);
-        dict = ((PyTypeObject *)base)->tp_dict;
-        meth = __Pyx_PyDict_GetItemStrWithError(dict, __pyx_n_s_init_subclass);
-        if (unlikely(meth)) {
-            descrgetfunc f = Py_TYPE(meth)->tp_descr_get;
-            PyObject *res;
-            Py_INCREF(meth);
-            if (likely(f)) {
-                res = f(meth, NULL, type_obj);
-                Py_DECREF(meth);
-                if (unlikely(!res)) goto bad;
-                meth = res;
-            }
-            res = __Pyx_PyObject_FastCallDict(meth, NULL, 0, mkw);
-            Py_DECREF(meth);
-            if (unlikely(!res)) goto bad;
-            Py_DECREF(res);
-            goto done;
-        } else if (unlikely(PyErr_Occurred())) {
-            goto bad;
-        }
-    }
-done:
-    Py_XDECREF(mro);
-    return type_obj;
-bad:
-    Py_XDECREF(mro);
-    Py_DECREF(type_obj);
-    return NULL;
-#else
-    PyObject *super_type, *super, *func, *res;
-#if CYTHON_COMPILING_IN_PYPY && !defined(PySuper_Type)
-    super_type = __Pyx_GetBuiltinName(__pyx_n_s_super);
-#else
-    super_type = (PyObject*) &PySuper_Type;
-    (void) &__Pyx_GetBuiltinName;
-#endif
-    super = likely(super_type) ? __Pyx_PyObject_Call2Args(super_type, type_obj, type_obj) : NULL;
-#if CYTHON_COMPILING_IN_PYPY && !defined(PySuper_Type)
-    Py_XDECREF(super_type);
-#endif
-    if (unlikely(!super)) {
-        Py_CLEAR(type_obj);
-        goto done;
-    }
-    func = __Pyx_PyObject_GetAttrStrNoError(super, __pyx_n_s_init_subclass);
-    Py_DECREF(super);
-    if (likely(!func)) {
-        if (unlikely(PyErr_Occurred()))
-            Py_CLEAR(type_obj);
-        goto done;
-    }
-    res = __Pyx_PyObject_FastCallDict(func, NULL, 0, mkw);
-    Py_DECREF(func);
-    if (unlikely(!res))
-        Py_CLEAR(type_obj);
-    Py_XDECREF(res);
-done:
-    return type_obj;
-#endif
-}
-#endif
-static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases,
-                                      PyObject *dict, PyObject *mkw,
-                                      int calculate_metaclass, int allow_py2_metaclass) {
-    PyObject *result;
-    PyObject *owned_metaclass = NULL;
-    PyObject *margs[4] = {NULL, name, bases, dict};
-    if (allow_py2_metaclass) {
-        owned_metaclass = PyObject_GetItem(dict, __pyx_n_s_metaclass);
-        if (owned_metaclass) {
-            metaclass = owned_metaclass;
-        } else if (likely(PyErr_ExceptionMatches(PyExc_KeyError))) {
-            PyErr_Clear();
-        } else {
-            return NULL;
-        }
-    }
-    if (calculate_metaclass && (!metaclass || PyType_Check(metaclass))) {
-        metaclass = __Pyx_CalculateMetaclass((PyTypeObject*) metaclass, bases);
-        Py_XDECREF(owned_metaclass);
-        if (unlikely(!metaclass))
-            return NULL;
-        owned_metaclass = metaclass;
-    }
-    result = __Pyx_PyObject_FastCallDict(metaclass, margs+1, 3 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET,
-#if PY_VERSION_HEX < 0x030600A4
-        (metaclass == (PyObject*)&PyType_Type) ? NULL : mkw
-#else
-        mkw
-#endif
-    );
-    Py_XDECREF(owned_metaclass);
-#if PY_VERSION_HEX < 0x030600A4 && CYTHON_PEP487_INIT_SUBCLASS
-    if (likely(result) && likely(PyType_Check(result))) {
-        if (unlikely(__Pyx_SetNamesPEP487(result) < 0)) {
-            Py_CLEAR(result);
-        } else {
-            result = __Pyx_InitSubclassPEP487(result, mkw);
-        }
-    }
-#else
-    (void) &__Pyx_GetBuiltinName;
-#endif
-    return result;
-}
-
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -9575,94 +10559,14 @@
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 #endif
 
-/* FormatTypeName */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static __Pyx_TypeName
-__Pyx_PyType_GetName(PyTypeObject* tp)
-{
-    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
-                                               __pyx_n_s_name);
-    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
-        PyErr_Clear();
-        Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__16);
-    }
-    return name;
-}
-#endif
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
-}
-
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -9677,14 +10581,32 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+/* ToPyCTupleUtility */
+static PyObject* __pyx_convert__to_py___pyx_ctuple_int__and_int(__pyx_ctuple_int__and_int value) {
+    PyObject* item = NULL;
+    PyObject* result = PyTuple_New(2);
+    if (!result) goto bad;
+        item = __Pyx_PyInt_From_int(value.f0);
+        if (!item) goto bad;
+        PyTuple_SET_ITEM(result, 0, item);
+        item = __Pyx_PyInt_From_int(value.f1);
+        if (!item) goto bad;
+        PyTuple_SET_ITEM(result, 1, item);
+    return result;
+bad:
+    Py_XDECREF(item);
+    Py_XDECREF(result);
+    return NULL;
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -9950,14 +10872,142 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const char neg_one = (char) -1, const_zero = (char) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(char) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(char) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(char) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(char),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(char));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
@@ -10223,14 +11273,94 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
+}
+
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__12);
+    }
+    return name;
+}
+#endif
+
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
```

### Comparing `bencode2-0.0.5/bencode2/_decoder.pyx` & `bencode2-0.0.6/bencode2/_decoder.pyx`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,80 @@
 # cython: language_level=3
-
-from collections.abc import Callable
 from typing import Any
 
-from ._compat import to_binary
 from ._exceptions import BencodeDecodeError
 
+cdef class Decoder:
+    str_key: bool
+
+    def __init__(self, str_key: bool):
+        self.str_key = str_key
 
-class BencodeDecoder:
-    def __init__(self):
-        self.decode_func: dict[bytes, Callable[[Any, int], tuple[list, int]]] = {
-            b"l": self.decode_list,
-            b"i": self.decode_int,
-            b"0": self.decode_string,
-            b"1": self.decode_string,
-            b"2": self.decode_string,
-            b"3": self.decode_string,
-            b"4": self.decode_string,
-            b"5": self.decode_string,
-            b"6": self.decode_string,
-            b"7": self.decode_string,
-            b"8": self.decode_string,
-            b"9": self.decode_string,
-            b"d": self.decode_dict,
-        }
-
-    def decode(self, value: bytes) -> Any:
-        """
-        Decode bencode formatted byte string ``value``.
-
-        :param value: Bencode formatted string
-        :type value: bytes
-
-        :return: Decoded value
-        :rtype: object
-        """
+    def decode(self, value: bytes)-> Any:
         try:
-            value = to_binary(value)
-            data, length = self.decode_func[value[0:1]](value, 0)
-        except (IndexError, KeyError, TypeError, ValueError):
-            raise BencodeDecodeError("not a valid bencoded string")
+            data, length = self.__decode(value, 0)
+        except (IndexError, KeyError, TypeError, ValueError) as e:
+            raise BencodeDecodeError(f"not a valid bencode bytes: {e}") from e
 
         if length != len(value):
-            raise BencodeDecodeError("invalid bencoded value (data after valid prefix)")
+            raise BencodeDecodeError("invalid bencode value (data after valid prefix)")
 
         return data
 
-    def decode_int(self, x, index: int):
+    cdef tuple[Any, int] __decode(self, x: bytes, index: int):
+        if x[index] == c'l':
+            return self.__decode_list(x, index)
+        if x[index] == c'i':
+            return self.__decode_int(x, index)
+        if x[index] == c'd':
+            return self.__decode_dict(x, index)
+        if c'0' <= x[index] <= c'9':
+            return self.__decode_str(x, index)
+
+        raise BencodeDecodeError(
+            f"unexpected token {x[index:index + 1]} at index {index}")
+
+    cdef tuple[int, int] __decode_int(self, x: bytes, index: int):
         index += 1
         new_f = x.index(b"e", index)
         n = int(x[index:new_f])
 
-        if x[index : index + 1] == b"-":
-            if x[index + 1 : index + 2] == b"0":
+        if x[index] == c'-':
+            if x[index + 1: index + 2] == b"0":
                 raise ValueError
-        elif x[index : index + 1] == b"0" and new_f != index + 1:
+        elif x[index] == c'0' and new_f != index + 1:
             raise ValueError
 
         return n, new_f + 1
 
-    def decode_string(self, x, index: int):
-        """Decode torrent bencoded 'string' in x starting at f."""
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
         colon = x.index(b":", index)
         n = int(x[index:colon])
 
-        if x[index : index + 1] == b"0" and colon != index + 1:
+        if x[index] == c'0' and colon != index + 1:
             raise ValueError
 
         colon += 1
-        s = x[colon : colon + n]
-
-        return bytes(s), colon + n
-
-    def decode_list(self, x, index: int):
-        r, index = [], index + 1
+        s = x[colon: colon + n]
 
-        while x[index : index + 1] != b"e":
-            v, index = self.decode_func[x[index : index + 1]](x, index)
-            r.append(v)
-
-        return r, index + 1
+        return s, colon + n
 
-    def decode_dict(self, x, index: int):
-        """Decode bencoded dictionary."""
+    cdef tuple[dict, int] __decode_dict(self, x: bytes, index: int):
         index += 1
 
         r = {}
-
-        while x[index : index + 1] != b"e":
-            k, index = self.decode_string(x, index)
-            r[k], index = self.decode_func[x[index : index + 1]](x, index)
+        while x[index] != c'e':
+            k, index = self.__decode_str(x, index)
+            if self.str_key:
+                k = k.decode(encoding='utf-8', errors='strict')
+            r[k], index = self.__decode(x, index)
 
         return r, index + 1
```

### Comparing `bencode2-0.0.5/bencode2/_encoder.c` & `bencode2-0.0.6/bencode2/_encoder.c`

 * *Files 2% similar despite different names*

```diff
@@ -1580,14 +1580,78 @@
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
+/* PyObjectGetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
+#endif
+
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
+/* GetBuiltinName.proto */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name);
+
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
 #if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
 #endif
@@ -1637,21 +1701,14 @@
 
 /* PyObjectCall2Args.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* PyObjectGetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
-#endif
-
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
 /* PyObjectCallMethod1.proto */
 static PyObject* __Pyx_PyObject_CallMethod1(PyObject* obj, PyObject* method_name, PyObject* arg);
 
 /* StringJoin.proto */
@@ -1740,71 +1797,14 @@
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
-
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#if PY_VERSION_HEX >= 0x030C00A6
-#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
-#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
-#else
-#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
-#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
-#endif
-#else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
-#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
-#endif
-
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
-
-/* GetBuiltinName.proto */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name);
-
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -2131,14 +2131,23 @@
 /* CythonFunction.proto */
 static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
+/* SliceTupleAndList.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_GetSlice(PyObject* src, Py_ssize_t start, Py_ssize_t stop);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_GetSlice(PyObject* src, Py_ssize_t start, Py_ssize_t stop);
+#else
+#define __Pyx_PyList_GetSlice(seq, start, stop)   PySequence_GetSlice(seq, start, stop)
+#define __Pyx_PyTuple_GetSlice(seq, start, stop)  PySequence_GetSlice(seq, start, stop)
+#endif
+
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
 #define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
@@ -2276,59 +2285,66 @@
 static PyObject *__pyx_f_8bencode2_8_encoder___encode(PyObject *, PyObject *); /*proto*/
 static PyObject *__pyx_f_8bencode2_8_encoder___encode_int(PyObject *, PyObject *); /*proto*/
 static PyObject *__pyx_f_8bencode2_8_encoder___encode_bool(PyObject *, PyObject *); /*proto*/
 static PyObject *__pyx_f_8bencode2_8_encoder___encode_bytes(PyObject *, PyObject *); /*proto*/
 static PyObject *__pyx_f_8bencode2_8_encoder___encode_str(PyObject *, PyObject *); /*proto*/
 static PyObject *__pyx_f_8bencode2_8_encoder___encode_list(PyObject *, PyObject *); /*proto*/
 static PyObject *__pyx_f_8bencode2_8_encoder___encode_dict(PyObject *, PyObject *); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder___check_duplicated_keys(PyObject *); /*proto*/
+static PyObject *__pyx_f_8bencode2_8_encoder_to_binary(PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "bencode2._encoder"
 extern int __pyx_module_is_main_bencode2___encoder;
 int __pyx_module_is_main_bencode2___encoder = 0;
 
 /* Implementation of "bencode2._encoder" */
 /* #### Code section: global_var ### */
+static PyObject *__pyx_builtin_TypeError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = "";
 static const char __pyx_k_d[] = "d";
 static const char __pyx_k_e[] = "e";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_l[] = "l";
 static const char __pyx_k__2[] = ":";
-static const char __pyx_k__3[] = ".";
-static const char __pyx_k__6[] = "?";
+static const char __pyx_k__4[] = ".";
+static const char __pyx_k__7[] = "?";
 static const char __pyx_k_kv[] = "kv";
 static const char __pyx_k_Any[] = "Any";
+static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_sort[] = "sort";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_type[] = "type '";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_value[] = "value";
-static const char __pyx_k_compat[] = "_compat";
+static const char __pyx_k_decode[] = "decode";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_import[] = "__import__";
+static const char __pyx_k_strict[] = "strict";
 static const char __pyx_k_typing[] = "typing";
 static const char __pyx_k_Mapping[] = "Mapping";
-static const char __pyx_k_to_binary[] = "to_binary";
+static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_exceptions[] = "_exceptions";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_not_supported[] = "' not supported";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_bencode2__encoder[] = "bencode2._encoder";
 static const char __pyx_k_BencodeEncodeError[] = "BencodeEncodeError";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_find_duplicated_keys[] = "find duplicated keys ";
 static const char __pyx_k_bencode2__encoder_pyx[] = "bencode2/_encoder.pyx";
 static const char __pyx_k_encode_dict_locals_lambda[] = "__encode_dict.<locals>.<lambda>";
+static const char __pyx_k_expected_binary_or_text_found_s[] = "expected binary or text (found %s)";
 /* #### Code section: decls ### */
 static PyObject *__pyx_pf_8bencode2_8_encoder_encode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_lambda_funcdef_lambda(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_kv); /* proto */
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
@@ -2389,50 +2405,55 @@
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   PyObject *__pyx_kp_b_;
   PyObject *__pyx_n_s_Any;
   PyObject *__pyx_n_s_BencodeEncodeError;
   PyObject *__pyx_n_s_Mapping;
+  PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_kp_b__2;
-  PyObject *__pyx_kp_u__3;
-  PyObject *__pyx_n_s__6;
+  PyObject *__pyx_kp_u__4;
+  PyObject *__pyx_n_s__7;
+  PyObject *__pyx_kp_u_and;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_bencode2__encoder;
   PyObject *__pyx_kp_s_bencode2__encoder_pyx;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_collections_abc;
-  PyObject *__pyx_n_s_compat;
   PyObject *__pyx_n_b_d;
+  PyObject *__pyx_n_s_decode;
   PyObject *__pyx_n_b_e;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_encode_dict_locals_lambda;
   PyObject *__pyx_n_s_exceptions;
+  PyObject *__pyx_kp_u_expected_binary_or_text_found_s;
+  PyObject *__pyx_kp_u_find_duplicated_keys;
   PyObject *__pyx_n_b_i;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_n_s_items;
   PyObject *__pyx_n_s_join;
   PyObject *__pyx_n_s_key;
   PyObject *__pyx_n_s_kv;
   PyObject *__pyx_n_b_l;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_kp_u_not_supported;
   PyObject *__pyx_n_s_sort;
+  PyObject *__pyx_n_u_strict;
   PyObject *__pyx_n_s_test;
-  PyObject *__pyx_n_s_to_binary;
   PyObject *__pyx_kp_u_type;
   PyObject *__pyx_n_s_typing;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_value;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
-  PyObject *__pyx_tuple__4;
-  PyObject *__pyx_codeobj__5;
+  PyObject *__pyx_tuple__3;
+  PyObject *__pyx_tuple__5;
+  PyObject *__pyx_codeobj__6;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2473,50 +2494,55 @@
   #endif
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
   Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4bool_bool);
   Py_CLEAR(clear_module_state->__pyx_kp_b_);
   Py_CLEAR(clear_module_state->__pyx_n_s_Any);
   Py_CLEAR(clear_module_state->__pyx_n_s_BencodeEncodeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Mapping);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_kp_b__2);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__3);
-  Py_CLEAR(clear_module_state->__pyx_n_s__6);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__4);
+  Py_CLEAR(clear_module_state->__pyx_n_s__7);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_and);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_bencode2__encoder);
   Py_CLEAR(clear_module_state->__pyx_kp_s_bencode2__encoder_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_collections_abc);
-  Py_CLEAR(clear_module_state->__pyx_n_s_compat);
   Py_CLEAR(clear_module_state->__pyx_n_b_d);
+  Py_CLEAR(clear_module_state->__pyx_n_s_decode);
   Py_CLEAR(clear_module_state->__pyx_n_b_e);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode_dict_locals_lambda);
   Py_CLEAR(clear_module_state->__pyx_n_s_exceptions);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_expected_binary_or_text_found_s);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_find_duplicated_keys);
   Py_CLEAR(clear_module_state->__pyx_n_b_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_n_s_items);
   Py_CLEAR(clear_module_state->__pyx_n_s_join);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_kv);
   Py_CLEAR(clear_module_state->__pyx_n_b_l);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_kp_u_not_supported);
   Py_CLEAR(clear_module_state->__pyx_n_s_sort);
+  Py_CLEAR(clear_module_state->__pyx_n_u_strict);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
-  Py_CLEAR(clear_module_state->__pyx_n_s_to_binary);
   Py_CLEAR(clear_module_state->__pyx_kp_u_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_typing);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_value);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
-  Py_CLEAR(clear_module_state->__pyx_tuple__4);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__5);
+  Py_CLEAR(clear_module_state->__pyx_tuple__3);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2535,50 +2561,55 @@
   #endif
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
   Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4bool_bool);
   Py_VISIT(traverse_module_state->__pyx_kp_b_);
   Py_VISIT(traverse_module_state->__pyx_n_s_Any);
   Py_VISIT(traverse_module_state->__pyx_n_s_BencodeEncodeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Mapping);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_kp_b__2);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__3);
-  Py_VISIT(traverse_module_state->__pyx_n_s__6);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__4);
+  Py_VISIT(traverse_module_state->__pyx_n_s__7);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_and);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_bencode2__encoder);
   Py_VISIT(traverse_module_state->__pyx_kp_s_bencode2__encoder_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_collections_abc);
-  Py_VISIT(traverse_module_state->__pyx_n_s_compat);
   Py_VISIT(traverse_module_state->__pyx_n_b_d);
+  Py_VISIT(traverse_module_state->__pyx_n_s_decode);
   Py_VISIT(traverse_module_state->__pyx_n_b_e);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode_dict_locals_lambda);
   Py_VISIT(traverse_module_state->__pyx_n_s_exceptions);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_expected_binary_or_text_found_s);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_find_duplicated_keys);
   Py_VISIT(traverse_module_state->__pyx_n_b_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_n_s_items);
   Py_VISIT(traverse_module_state->__pyx_n_s_join);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_kv);
   Py_VISIT(traverse_module_state->__pyx_n_b_l);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_kp_u_not_supported);
   Py_VISIT(traverse_module_state->__pyx_n_s_sort);
+  Py_VISIT(traverse_module_state->__pyx_n_u_strict);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
-  Py_VISIT(traverse_module_state->__pyx_n_s_to_binary);
   Py_VISIT(traverse_module_state->__pyx_kp_u_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_typing);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_value);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
-  Py_VISIT(traverse_module_state->__pyx_tuple__4);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__5);
+  Py_VISIT(traverse_module_state->__pyx_tuple__3);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -2637,53 +2668,58 @@
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #define __pyx_kp_b_ __pyx_mstate_global->__pyx_kp_b_
 #define __pyx_n_s_Any __pyx_mstate_global->__pyx_n_s_Any
 #define __pyx_n_s_BencodeEncodeError __pyx_mstate_global->__pyx_n_s_BencodeEncodeError
 #define __pyx_n_s_Mapping __pyx_mstate_global->__pyx_n_s_Mapping
+#define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_kp_b__2 __pyx_mstate_global->__pyx_kp_b__2
-#define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
-#define __pyx_n_s__6 __pyx_mstate_global->__pyx_n_s__6
+#define __pyx_kp_u__4 __pyx_mstate_global->__pyx_kp_u__4
+#define __pyx_n_s__7 __pyx_mstate_global->__pyx_n_s__7
+#define __pyx_kp_u_and __pyx_mstate_global->__pyx_kp_u_and
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_bencode2__encoder __pyx_mstate_global->__pyx_n_s_bencode2__encoder
 #define __pyx_kp_s_bencode2__encoder_pyx __pyx_mstate_global->__pyx_kp_s_bencode2__encoder_pyx
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_collections_abc __pyx_mstate_global->__pyx_n_s_collections_abc
-#define __pyx_n_s_compat __pyx_mstate_global->__pyx_n_s_compat
 #define __pyx_n_b_d __pyx_mstate_global->__pyx_n_b_d
+#define __pyx_n_s_decode __pyx_mstate_global->__pyx_n_s_decode
 #define __pyx_n_b_e __pyx_mstate_global->__pyx_n_b_e
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_encode_dict_locals_lambda __pyx_mstate_global->__pyx_n_s_encode_dict_locals_lambda
 #define __pyx_n_s_exceptions __pyx_mstate_global->__pyx_n_s_exceptions
+#define __pyx_kp_u_expected_binary_or_text_found_s __pyx_mstate_global->__pyx_kp_u_expected_binary_or_text_found_s
+#define __pyx_kp_u_find_duplicated_keys __pyx_mstate_global->__pyx_kp_u_find_duplicated_keys
 #define __pyx_n_b_i __pyx_mstate_global->__pyx_n_b_i
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_n_s_items __pyx_mstate_global->__pyx_n_s_items
 #define __pyx_n_s_join __pyx_mstate_global->__pyx_n_s_join
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
 #define __pyx_n_s_kv __pyx_mstate_global->__pyx_n_s_kv
 #define __pyx_n_b_l __pyx_mstate_global->__pyx_n_b_l
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_kp_u_not_supported __pyx_mstate_global->__pyx_kp_u_not_supported
 #define __pyx_n_s_sort __pyx_mstate_global->__pyx_n_s_sort
+#define __pyx_n_u_strict __pyx_mstate_global->__pyx_n_u_strict
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
-#define __pyx_n_s_to_binary __pyx_mstate_global->__pyx_n_s_to_binary
 #define __pyx_kp_u_type __pyx_mstate_global->__pyx_kp_u_type
 #define __pyx_n_s_typing __pyx_mstate_global->__pyx_n_s_typing
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
-#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
-#define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
+#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
+#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
 /* #### Code section: module_code ### */
 
-/* "bencode2/_encoder.pyx":17
+/* "bencode2/_encoder.pyx":16
  * from ._exceptions import BencodeEncodeError
  * 
  * cpdef bytes encode(value: Any):             # <<<<<<<<<<<<<<
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  */
 
@@ -2700,53 +2736,53 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode", 1);
 
-  /* "bencode2/_encoder.pyx":18
+  /* "bencode2/_encoder.pyx":17
  * 
  * cpdef bytes encode(value: Any):
  *     r: list[bytes] = []  # makes more sense for something with lots of appends             # <<<<<<<<<<<<<<
  * 
  *     __encode(value, r)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "bencode2/_encoder.pyx":20
+  /* "bencode2/_encoder.pyx":19
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  *     __encode(value, r)             # <<<<<<<<<<<<<<
  * 
  *     # Join parts
  */
-  __pyx_t_1 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bencode2/_encoder.pyx":23
+  /* "bencode2/_encoder.pyx":22
  * 
  *     # Join parts
  *     return b"".join(r)             # <<<<<<<<<<<<<<
  * 
  * cdef __encode(value, r: list[bytes]):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_Join(__pyx_kp_b_, __pyx_v_r); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_Join(__pyx_kp_b_, __pyx_v_r); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_1))) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_1))) __PYX_ERR(0, 22, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "bencode2/_encoder.pyx":17
+  /* "bencode2/_encoder.pyx":16
  * from ._exceptions import BencodeEncodeError
  * 
  * cpdef bytes encode(value: Any):             # <<<<<<<<<<<<<<
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  */
 
@@ -2811,31 +2847,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 17, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 16, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "encode") < 0)) __PYX_ERR(0, 17, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "encode") < 0)) __PYX_ERR(0, 16, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_value = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("encode", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 17, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("encode", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 16, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -2863,15 +2899,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8bencode2_8_encoder_encode(__pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8bencode2_8_encoder_encode(__pyx_v_value, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2880,15 +2916,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_encoder.pyx":25
+/* "bencode2/_encoder.pyx":24
  *     return b"".join(r)
  * 
  * cdef __encode(value, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)
  */
 
@@ -2904,264 +2940,264 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode", 1);
 
-  /* "bencode2/_encoder.pyx":26
+  /* "bencode2/_encoder.pyx":25
  * 
  * cdef __encode(value, r: list[bytes]):
  *     if PyDict_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):
  */
   __pyx_t_1 = PyDict_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/_encoder.pyx":27
+    /* "bencode2/_encoder.pyx":26
  * cdef __encode(value, r: list[bytes]):
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)             # <<<<<<<<<<<<<<
  *     elif PyString_Check(value):
  *         __encode_str(value, r)
  */
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_dict(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_dict(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/_encoder.pyx":26
+    /* "bencode2/_encoder.pyx":25
  * 
  * cdef __encode(value, r: list[bytes]):
  *     if PyDict_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_encoder.pyx":28
+  /* "bencode2/_encoder.pyx":27
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_str(value, r)
  *     elif PyList_Check(value):
  */
   __pyx_t_1 = PyString_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/_encoder.pyx":29
+    /* "bencode2/_encoder.pyx":28
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):
  *         __encode_str(value, r)             # <<<<<<<<<<<<<<
  *     elif PyList_Check(value):
  *         __encode_list(value, r)
  */
-    if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(0, 29, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_str(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(0, 28, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_str(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 28, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/_encoder.pyx":28
+    /* "bencode2/_encoder.pyx":27
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)
  *     elif PyString_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_str(value, r)
  *     elif PyList_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_encoder.pyx":30
+  /* "bencode2/_encoder.pyx":29
  *     elif PyString_Check(value):
  *         __encode_str(value, r)
  *     elif PyList_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):
  */
   __pyx_t_1 = PyList_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/_encoder.pyx":31
+    /* "bencode2/_encoder.pyx":30
  *         __encode_str(value, r)
  *     elif PyList_Check(value):
  *         __encode_list(value, r)             # <<<<<<<<<<<<<<
  *     elif PyTuple_Check(value):
  *         __encode_list(value, r)
  */
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_list(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_list(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/_encoder.pyx":30
+    /* "bencode2/_encoder.pyx":29
  *     elif PyString_Check(value):
  *         __encode_str(value, r)
  *     elif PyList_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_encoder.pyx":32
+  /* "bencode2/_encoder.pyx":31
  *     elif PyList_Check(value):
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/_encoder.pyx":33
+    /* "bencode2/_encoder.pyx":32
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):
  *         __encode_list(value, r)             # <<<<<<<<<<<<<<
  *     elif PyBytes_Check(value):
  *         __encode_bytes(value, r)
  */
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_list(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_list(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 32, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/_encoder.pyx":32
+    /* "bencode2/_encoder.pyx":31
  *     elif PyList_Check(value):
  *         __encode_list(value, r)
  *     elif PyTuple_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_encoder.pyx":34
+  /* "bencode2/_encoder.pyx":33
  *     elif PyTuple_Check(value):
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/_encoder.pyx":35
+    /* "bencode2/_encoder.pyx":34
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):
  *         __encode_bytes(value, r)             # <<<<<<<<<<<<<<
  *     elif PyBool_Check(value):
  *         __encode_bool(value, r)
  */
-    if (!(likely(PyBytes_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_value))) __PYX_ERR(0, 35, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bytes(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 35, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_value))) __PYX_ERR(0, 34, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bytes(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/_encoder.pyx":34
+    /* "bencode2/_encoder.pyx":33
  *     elif PyTuple_Check(value):
  *         __encode_list(value, r)
  *     elif PyBytes_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_encoder.pyx":36
+  /* "bencode2/_encoder.pyx":35
  *     elif PyBytes_Check(value):
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):
  */
   __pyx_t_1 = PyBool_Check(__pyx_v_value);
   if (__pyx_t_1) {
 
-    /* "bencode2/_encoder.pyx":37
+    /* "bencode2/_encoder.pyx":36
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):
  *         __encode_bool(value, r)             # <<<<<<<<<<<<<<
  *     elif PyInt_Check(value):
  *         __encode_int(value, r)
  */
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bool(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bool(__pyx_v_value, __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/_encoder.pyx":36
+    /* "bencode2/_encoder.pyx":35
  *     elif PyBytes_Check(value):
  *         __encode_bytes(value, r)
  *     elif PyBool_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_encoder.pyx":38
+  /* "bencode2/_encoder.pyx":37
  *     elif PyBool_Check(value):
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_int(value, r)
  *     else:
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_value);
   if (likely(__pyx_t_1)) {
 
-    /* "bencode2/_encoder.pyx":39
+    /* "bencode2/_encoder.pyx":38
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):
  *         __encode_int(value, r)             # <<<<<<<<<<<<<<
  *     else:
  *         raise BencodeEncodeError(f"type '{type(value)}' not supported")
  */
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_v_value))) __PYX_ERR(0, 39, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_v_value))) __PYX_ERR(0, 38, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_v_value), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 38, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/_encoder.pyx":38
+    /* "bencode2/_encoder.pyx":37
  *     elif PyBool_Check(value):
  *         __encode_bool(value, r)
  *     elif PyInt_Check(value):             # <<<<<<<<<<<<<<
  *         __encode_int(value, r)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_encoder.pyx":41
+  /* "bencode2/_encoder.pyx":40
  *         __encode_int(value, r)
  *     else:
  *         raise BencodeEncodeError(f"type '{type(value)}' not supported")             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_int(x: int, r: list[bytes]):
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BencodeEncodeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_BencodeEncodeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
     __Pyx_INCREF(__pyx_kp_u_type);
     __pyx_t_5 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_type);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_kp_u_type);
-    __pyx_t_7 = __Pyx_PyObject_FormatSimple(((PyObject *)Py_TYPE(__pyx_v_value)), __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(((PyObject *)Py_TYPE(__pyx_v_value)), __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_not_supported);
     __pyx_t_5 += 15;
     __Pyx_GIVEREF(__pyx_kp_u_not_supported);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_u_not_supported);
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 40, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_8 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -3175,25 +3211,25 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_7};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 41, __pyx_L1_error)
+    __PYX_ERR(0, 40, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "bencode2/_encoder.pyx":25
+  /* "bencode2/_encoder.pyx":24
  *     return b"".join(r)
  * 
  * cdef __encode(value, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     if PyDict_Check(value):
  *         __encode_dict(value, r)
  */
 
@@ -3209,15 +3245,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_encoder.pyx":43
+/* "bencode2/_encoder.pyx":42
  *         raise BencodeEncodeError(f"type '{type(value)}' not supported")
  * 
  * cdef __encode_int(x: int, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))
  * 
  */
 
@@ -3232,24 +3268,24 @@
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_int", 1);
 
-  /* "bencode2/_encoder.pyx":44
+  /* "bencode2/_encoder.pyx":43
  * 
  * cdef __encode_int(x: int, r: list[bytes]):
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):
  */
-  __pyx_t_2 = __Pyx_PyObject_Str(__pyx_v_x); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Str(__pyx_v_x); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -3262,25 +3298,25 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_kp_u_utf_8};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_5 = __Pyx_ListComp_Append(__pyx_v_r, __pyx_n_b_i); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_ListComp_Append(__pyx_v_r, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_r, __pyx_n_b_e); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_ListComp_Append(__pyx_v_r, __pyx_n_b_i); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_ListComp_Append(__pyx_v_r, __pyx_t_1); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_r, __pyx_n_b_e); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(0, 43, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   (void)((__pyx_t_5 | (__pyx_t_6 | __pyx_t_7)));
 
-  /* "bencode2/_encoder.pyx":43
+  /* "bencode2/_encoder.pyx":42
  *         raise BencodeEncodeError(f"type '{type(value)}' not supported")
  * 
  * cdef __encode_int(x: int, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))
  * 
  */
 
@@ -3295,15 +3331,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_encoder.pyx":46
+/* "bencode2/_encoder.pyx":45
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     if x:
  *         __encode_int(1, r)
  */
 
@@ -3313,62 +3349,62 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_bool", 1);
 
-  /* "bencode2/_encoder.pyx":47
+  /* "bencode2/_encoder.pyx":46
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):
  *     if x:             # <<<<<<<<<<<<<<
  *         __encode_int(1, r)
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_x); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_x); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 46, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "bencode2/_encoder.pyx":48
+    /* "bencode2/_encoder.pyx":47
  * cdef __encode_bool(x: bool, r: list[bytes]):
  *     if x:
  *         __encode_int(1, r)             # <<<<<<<<<<<<<<
  *     else:
  *         __encode_int(0, r)
  */
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_1))) __PYX_ERR(0, 48, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_int_1), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_1))) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_int_1), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 47, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "bencode2/_encoder.pyx":47
+    /* "bencode2/_encoder.pyx":46
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):
  *     if x:             # <<<<<<<<<<<<<<
  *         __encode_int(1, r)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "bencode2/_encoder.pyx":50
+  /* "bencode2/_encoder.pyx":49
  *         __encode_int(1, r)
  *     else:
  *         __encode_int(0, r)             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_bytes(x: bytes, r: list[bytes]):
  */
   /*else*/ {
-    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 50, __pyx_L1_error)
-    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_int_0), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+    if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_int_0)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_int_0))) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_int(((PyObject*)__pyx_int_0), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "bencode2/_encoder.pyx":46
+  /* "bencode2/_encoder.pyx":45
  *     r.extend((b"i", str(x).encode("utf-8"), b"e"))
  * 
  * cdef __encode_bool(x: bool, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     if x:
  *         __encode_int(1, r)
  */
 
@@ -3381,15 +3417,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_encoder.pyx":52
+/* "bencode2/_encoder.pyx":51
  *         __encode_int(0, r)
  * 
  * cdef __encode_bytes(x: bytes, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, str(len(x)).encode("utf-8"))
  *     PyList_Append(r, b":")
  */
 
@@ -3402,28 +3438,28 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_bytes", 1);
 
-  /* "bencode2/_encoder.pyx":53
+  /* "bencode2/_encoder.pyx":52
  * 
  * cdef __encode_bytes(x: bytes, r: list[bytes]):
  *     PyList_Append(r, str(len(x)).encode("utf-8"))             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b":")
  *     PyList_Append(r, x)
  */
-  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_x); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_GET_SIZE(__pyx_v_x); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Str(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -3436,40 +3472,40 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_u_utf_8};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "bencode2/_encoder.pyx":54
+  /* "bencode2/_encoder.pyx":53
  * cdef __encode_bytes(x: bytes, r: list[bytes]):
  *     PyList_Append(r, str(len(x)).encode("utf-8"))
  *     PyList_Append(r, b":")             # <<<<<<<<<<<<<<
  *     PyList_Append(r, x)
  * 
  */
-  __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_kp_b__2); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_kp_b__2); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
 
-  /* "bencode2/_encoder.pyx":55
+  /* "bencode2/_encoder.pyx":54
  *     PyList_Append(r, str(len(x)).encode("utf-8"))
  *     PyList_Append(r, b":")
  *     PyList_Append(r, x)             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_str(x: str, r: list[bytes]):
  */
-  __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_v_x); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_5 = PyList_Append(__pyx_v_r, __pyx_v_x); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 54, __pyx_L1_error)
 
-  /* "bencode2/_encoder.pyx":52
+  /* "bencode2/_encoder.pyx":51
  *         __encode_int(0, r)
  * 
  * cdef __encode_bytes(x: bytes, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, str(len(x)).encode("utf-8"))
  *     PyList_Append(r, b":")
  */
 
@@ -3484,15 +3520,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_encoder.pyx":57
+/* "bencode2/_encoder.pyx":56
  *     PyList_Append(r, x)
  * 
  * cdef __encode_str(x: str, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     __encode_bytes(x.encode("UTF-8"), r)
  * 
  */
 
@@ -3502,29 +3538,29 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_str", 1);
 
-  /* "bencode2/_encoder.pyx":58
+  /* "bencode2/_encoder.pyx":57
  * 
  * cdef __encode_str(x: str, r: list[bytes]):
  *     __encode_bytes(x.encode("UTF-8"), r)             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_list(x: list | tuple, r: list[bytes]):
  */
-  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_x); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsUTF8String(__pyx_v_x); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bytes(((PyObject*)__pyx_t_1), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_8bencode2_8_encoder___encode_bytes(((PyObject*)__pyx_t_1), __pyx_v_r); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/_encoder.pyx":57
+  /* "bencode2/_encoder.pyx":56
  *     PyList_Append(r, x)
  * 
  * cdef __encode_str(x: str, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     __encode_bytes(x.encode("UTF-8"), r)
  * 
  */
 
@@ -3538,15 +3574,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_encoder.pyx":60
+/* "bencode2/_encoder.pyx":59
  *     __encode_bytes(x.encode("UTF-8"), r)
  * 
  * cdef __encode_list(x: list | tuple, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b"l")
  * 
  */
 
@@ -3560,116 +3596,116 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_list", 1);
 
-  /* "bencode2/_encoder.pyx":61
+  /* "bencode2/_encoder.pyx":60
  * 
  * cdef __encode_list(x: list | tuple, r: list[bytes]):
  *     PyList_Append(r, b"l")             # <<<<<<<<<<<<<<
  * 
  *     for i in x:
  */
-  __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_l); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_l); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 60, __pyx_L1_error)
 
-  /* "bencode2/_encoder.pyx":63
+  /* "bencode2/_encoder.pyx":62
  *     PyList_Append(r, b"l")
  * 
  *     for i in x:             # <<<<<<<<<<<<<<
  *         __encode(i, r)
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_x)) || PyTuple_CheckExact(__pyx_v_x)) {
     __pyx_t_2 = __pyx_v_x; __Pyx_INCREF(__pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_x); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_x); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 62, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 63, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 62, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 63, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 62, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 63, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 62, __pyx_L1_error)
         #else
-        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 63, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 62, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 63, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 62, __pyx_L1_error)
         #else
-        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 63, __pyx_L1_error)
+          else __PYX_ERR(0, 62, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "bencode2/_encoder.pyx":64
+    /* "bencode2/_encoder.pyx":63
  * 
  *     for i in x:
  *         __encode(i, r)             # <<<<<<<<<<<<<<
  * 
  *     PyList_Append(r, b"e")
  */
-    __pyx_t_5 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_i, __pyx_v_r); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_i, __pyx_v_r); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "bencode2/_encoder.pyx":63
+    /* "bencode2/_encoder.pyx":62
  *     PyList_Append(r, b"l")
  * 
  *     for i in x:             # <<<<<<<<<<<<<<
  *         __encode(i, r)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "bencode2/_encoder.pyx":66
+  /* "bencode2/_encoder.pyx":65
  *         __encode(i, r)
  * 
  *     PyList_Append(r, b"e")             # <<<<<<<<<<<<<<
  * 
  * cdef __encode_dict(x: Mapping, r: list[bytes]):
  */
-  __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_e); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_e); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 65, __pyx_L1_error)
 
-  /* "bencode2/_encoder.pyx":60
+  /* "bencode2/_encoder.pyx":59
  *     __encode_bytes(x.encode("UTF-8"), r)
  * 
  * cdef __encode_list(x: list | tuple, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b"l")
  * 
  */
 
@@ -3684,20 +3720,20 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_encoder.pyx":73
+/* "bencode2/_encoder.pyx":72
  *     # force all keys to bytes, because str and bytes are incomparable
- *     i_list = [(to_binary(k), v) for k, v in x.items()]
+ *     i_list: list[tuple[bytes, Any]] = [(to_binary(k), v) for k, v in x.items()]
  *     i_list.sort(key=lambda kv: kv[0])             # <<<<<<<<<<<<<<
+ *     __check_duplicated_keys(i_list)
  * 
- *     for k, v in i_list:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8bencode2_8_encoder_13__encode_dict_lambda(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -3745,31 +3781,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kv)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 73, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 72, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_kv = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 73, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 72, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -3797,15 +3833,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_kv, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_kv, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3814,24 +3850,24 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "bencode2/_encoder.pyx":68
+/* "bencode2/_encoder.pyx":67
  *     PyList_Append(r, b"e")
  * 
  * cdef __encode_dict(x: Mapping, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b"d")
  * 
  */
 
 static PyObject *__pyx_f_8bencode2_8_encoder___encode_dict(PyObject *__pyx_v_x, PyObject *__pyx_v_r) {
-  PyObject *__pyx_v_i_list = NULL;
+  PyObject *__pyx_v_i_list = 0;
   PyObject *__pyx_v_k = NULL;
   PyObject *__pyx_v_v = NULL;
   PyObject *__pyx_7genexpr__pyx_v_k = NULL;
   PyObject *__pyx_7genexpr__pyx_v_v = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -3845,86 +3881,64 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *(*__pyx_t_10)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__encode_dict", 1);
 
-  /* "bencode2/_encoder.pyx":69
+  /* "bencode2/_encoder.pyx":68
  * 
  * cdef __encode_dict(x: Mapping, r: list[bytes]):
  *     PyList_Append(r, b"d")             # <<<<<<<<<<<<<<
  * 
  *     # force all keys to bytes, because str and bytes are incomparable
  */
-  __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_d); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_d); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 68, __pyx_L1_error)
 
-  /* "bencode2/_encoder.pyx":72
+  /* "bencode2/_encoder.pyx":71
  * 
  *     # force all keys to bytes, because str and bytes are incomparable
- *     i_list = [(to_binary(k), v) for k, v in x.items()]             # <<<<<<<<<<<<<<
+ *     i_list: list[tuple[bytes, Any]] = [(to_binary(k), v) for k, v in x.items()]             # <<<<<<<<<<<<<<
  *     i_list.sort(key=lambda kv: kv[0])
- * 
+ *     __check_duplicated_keys(i_list)
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L5_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = 0;
     if (unlikely(__pyx_v_x == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 72, __pyx_L5_error)
+      __PYX_ERR(0, 71, __pyx_L5_error)
     }
-    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_x, 0, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L5_error)
+    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_x, 0, __pyx_n_s_items, (&__pyx_t_5), (&__pyx_t_1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_6;
     __pyx_t_6 = 0;
     while (1) {
       __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_5, &__pyx_t_4, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_1);
       if (unlikely(__pyx_t_8 == 0)) break;
-      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 72, __pyx_L5_error)
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(0, 71, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_k, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_v, __pyx_t_7);
       __pyx_t_7 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_to_binary); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L5_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_9 = NULL;
-      __pyx_t_8 = 0;
-      #if CYTHON_UNPACK_METHODS
-      if (unlikely(PyMethod_Check(__pyx_t_6))) {
-        __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
-        if (likely(__pyx_t_9)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-          __Pyx_INCREF(__pyx_t_9);
-          __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_6, function);
-          __pyx_t_8 = 1;
-        }
-      }
-      #endif
-      {
-        PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_7genexpr__pyx_v_k};
-        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-        __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 72, __pyx_L5_error)
-        __Pyx_GOTREF(__pyx_t_7);
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      }
-      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L5_error)
+      __pyx_t_7 = __pyx_f_8bencode2_8_encoder_to_binary(__pyx_7genexpr__pyx_v_k); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 71, __pyx_L5_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 71, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_7);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7)) __PYX_ERR(0, 72, __pyx_L5_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_7)) __PYX_ERR(0, 71, __pyx_L5_error);
       __Pyx_INCREF(__pyx_7genexpr__pyx_v_v);
       __Pyx_GIVEREF(__pyx_7genexpr__pyx_v_v);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_7genexpr__pyx_v_v)) __PYX_ERR(0, 72, __pyx_L5_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_7genexpr__pyx_v_v)) __PYX_ERR(0, 71, __pyx_L5_error);
       __pyx_t_7 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 72, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 71, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k); __pyx_7genexpr__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
@@ -3932,37 +3946,48 @@
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_i_list = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "bencode2/_encoder.pyx":73
+  /* "bencode2/_encoder.pyx":72
  *     # force all keys to bytes, because str and bytes are incomparable
- *     i_list = [(to_binary(k), v) for k, v in x.items()]
+ *     i_list: list[tuple[bytes, Any]] = [(to_binary(k), v) for k, v in x.items()]
  *     i_list.sort(key=lambda kv: kv[0])             # <<<<<<<<<<<<<<
+ *     __check_duplicated_keys(i_list)
  * 
- *     for k, v in i_list:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_i_list, __pyx_n_s_sort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_i_list, __pyx_n_s_sort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_encoder_13__encode_dict_lambda, 0, __pyx_n_s_encode_dict_locals_lambda, NULL, __pyx_n_s_bencode2__encoder, __pyx_d, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_encoder_13__encode_dict_lambda, 0, __pyx_n_s_encode_dict_locals_lambda, NULL, __pyx_n_s_bencode2__encoder, __pyx_d, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_6) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "bencode2/_encoder.pyx":75
+  /* "bencode2/_encoder.pyx":73
+ *     i_list: list[tuple[bytes, Any]] = [(to_binary(k), v) for k, v in x.items()]
  *     i_list.sort(key=lambda kv: kv[0])
+ *     __check_duplicated_keys(i_list)             # <<<<<<<<<<<<<<
+ * 
+ *     for k, v in i_list:
+ */
+  __pyx_t_6 = __pyx_f_8bencode2_8_encoder___check_duplicated_keys(__pyx_v_i_list); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+  /* "bencode2/_encoder.pyx":75
+ *     __check_duplicated_keys(i_list)
  * 
  *     for k, v in i_list:             # <<<<<<<<<<<<<<
  *         __encode(k, r)
  *         __encode(v, r)
  */
   __pyx_t_6 = __pyx_v_i_list; __Pyx_INCREF(__pyx_t_6);
   __pyx_t_5 = 0;
@@ -4050,31 +4075,33 @@
  *     PyList_Append(r, b"e")
  */
     __pyx_t_3 = __pyx_f_8bencode2_8_encoder___encode(__pyx_v_v, __pyx_v_r); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "bencode2/_encoder.pyx":75
- *     i_list.sort(key=lambda kv: kv[0])
+ *     __check_duplicated_keys(i_list)
  * 
  *     for k, v in i_list:             # <<<<<<<<<<<<<<
  *         __encode(k, r)
  *         __encode(v, r)
  */
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
   /* "bencode2/_encoder.pyx":79
  *         __encode(v, r)
  * 
  *     PyList_Append(r, b"e")             # <<<<<<<<<<<<<<
+ * 
+ * cdef __check_duplicated_keys(s: list[tuple[bytes, Any]]):
  */
   __pyx_t_1 = PyList_Append(__pyx_v_r, __pyx_n_b_e); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 79, __pyx_L1_error)
 
-  /* "bencode2/_encoder.pyx":68
+  /* "bencode2/_encoder.pyx":67
  *     PyList_Append(r, b"e")
  * 
  * cdef __encode_dict(x: Mapping, r: list[bytes]):             # <<<<<<<<<<<<<<
  *     PyList_Append(r, b"d")
  * 
  */
 
@@ -4096,14 +4123,460 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "bencode2/_encoder.pyx":81
+ *     PyList_Append(r, b"e")
+ * 
+ * cdef __check_duplicated_keys(s: list[tuple[bytes, Any]]):             # <<<<<<<<<<<<<<
+ *     if len(s) == 0:
+ *         return
+ */
+
+static PyObject *__pyx_f_8bencode2_8_encoder___check_duplicated_keys(PyObject *__pyx_v_s) {
+  PyObject *__pyx_v_last_key = 0;
+  PyObject *__pyx_v_current = NULL;
+  CYTHON_UNUSED PyObject *__pyx_v__ = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  int __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *(*__pyx_t_8)(PyObject *);
+  Py_ssize_t __pyx_t_9;
+  Py_UCS4 __pyx_t_10;
+  PyObject *__pyx_t_11 = NULL;
+  PyObject *__pyx_t_12 = NULL;
+  int __pyx_t_13;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__check_duplicated_keys", 1);
+
+  /* "bencode2/_encoder.pyx":82
+ * 
+ * cdef __check_duplicated_keys(s: list[tuple[bytes, Any]]):
+ *     if len(s) == 0:             # <<<<<<<<<<<<<<
+ *         return
+ *     last_key: bytes = s[0][0]
+ */
+  __pyx_t_1 = __Pyx_PyList_GET_SIZE(__pyx_v_s); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_2 = (__pyx_t_1 == 0);
+  if (__pyx_t_2) {
+
+    /* "bencode2/_encoder.pyx":83
+ * cdef __check_duplicated_keys(s: list[tuple[bytes, Any]]):
+ *     if len(s) == 0:
+ *         return             # <<<<<<<<<<<<<<
+ *     last_key: bytes = s[0][0]
+ *     for current, _ in s[1:]:
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+    goto __pyx_L0;
+
+    /* "bencode2/_encoder.pyx":82
+ * 
+ * cdef __check_duplicated_keys(s: list[tuple[bytes, Any]]):
+ *     if len(s) == 0:             # <<<<<<<<<<<<<<
+ *         return
+ *     last_key: bytes = s[0][0]
+ */
+  }
+
+  /* "bencode2/_encoder.pyx":84
+ *     if len(s) == 0:
+ *         return
+ *     last_key: bytes = s[0][0]             # <<<<<<<<<<<<<<
+ *     for current, _ in s[1:]:
+ *         if last_key == current:
+ */
+  __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_s, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_4))) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_v_last_key = ((PyObject*)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "bencode2/_encoder.pyx":85
+ *         return
+ *     last_key: bytes = s[0][0]
+ *     for current, _ in s[1:]:             # <<<<<<<<<<<<<<
+ *         if last_key == current:
+ *             raise BencodeEncodeError(
+ */
+  __pyx_t_4 = __Pyx_PyList_GetSlice(__pyx_v_s, 1, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __pyx_t_4; __Pyx_INCREF(__pyx_t_3);
+  __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  for (;;) {
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 85, __pyx_L1_error)
+      #endif
+      if (__pyx_t_1 >= __pyx_temp) break;
+    }
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    __pyx_t_4 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 85, __pyx_L1_error)
+    #else
+    __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    #endif
+    if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
+      PyObject* sequence = __pyx_t_4;
+      Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
+      if (unlikely(size != 2)) {
+        if (size > 2) __Pyx_RaiseTooManyValuesError(2);
+        else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
+        __PYX_ERR(0, 85, __pyx_L1_error)
+      }
+      #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+      if (likely(PyTuple_CheckExact(sequence))) {
+        __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
+      } else {
+        __pyx_t_5 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
+      }
+      __Pyx_INCREF(__pyx_t_5);
+      __Pyx_INCREF(__pyx_t_6);
+      #else
+      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 85, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      #endif
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    } else {
+      Py_ssize_t index = -1;
+      __pyx_t_7 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 85, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_8 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_7);
+      index = 0; __pyx_t_5 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_5)) goto __pyx_L6_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_5);
+      index = 1; __pyx_t_6 = __pyx_t_8(__pyx_t_7); if (unlikely(!__pyx_t_6)) goto __pyx_L6_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_6);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_8(__pyx_t_7), 2) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+      __pyx_t_8 = NULL;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      goto __pyx_L7_unpacking_done;
+      __pyx_L6_unpacking_failed:;
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_8 = NULL;
+      if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
+      __PYX_ERR(0, 85, __pyx_L1_error)
+      __pyx_L7_unpacking_done:;
+    }
+    __Pyx_XDECREF_SET(__pyx_v_current, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __Pyx_XDECREF_SET(__pyx_v__, __pyx_t_6);
+    __pyx_t_6 = 0;
+
+    /* "bencode2/_encoder.pyx":86
+ *     last_key: bytes = s[0][0]
+ *     for current, _ in s[1:]:
+ *         if last_key == current:             # <<<<<<<<<<<<<<
+ *             raise BencodeEncodeError(
+ *                 f'find duplicated keys {last_key} and {current.decode()}'
+ */
+    __pyx_t_2 = (__Pyx_PyBytes_Equals(__pyx_v_last_key, __pyx_v_current, Py_EQ)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 86, __pyx_L1_error)
+    if (unlikely(__pyx_t_2)) {
+
+      /* "bencode2/_encoder.pyx":87
+ *     for current, _ in s[1:]:
+ *         if last_key == current:
+ *             raise BencodeEncodeError(             # <<<<<<<<<<<<<<
+ *                 f'find duplicated keys {last_key} and {current.decode()}'
+ *             )
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_BencodeEncodeError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 87, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+
+      /* "bencode2/_encoder.pyx":88
+ *         if last_key == current:
+ *             raise BencodeEncodeError(
+ *                 f'find duplicated keys {last_key} and {current.decode()}'             # <<<<<<<<<<<<<<
+ *             )
+ *         last_key = current
+ */
+      __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_9 = 0;
+      __pyx_t_10 = 127;
+      __Pyx_INCREF(__pyx_kp_u_find_duplicated_keys);
+      __pyx_t_9 += 21;
+      __Pyx_GIVEREF(__pyx_kp_u_find_duplicated_keys);
+      PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_kp_u_find_duplicated_keys);
+      __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_v_last_key, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_10;
+      __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
+      __Pyx_GIVEREF(__pyx_t_7);
+      PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7);
+      __pyx_t_7 = 0;
+      __Pyx_INCREF(__pyx_kp_u_and);
+      __pyx_t_9 += 5;
+      __Pyx_GIVEREF(__pyx_kp_u_and);
+      PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_u_and);
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_current, __pyx_n_s_decode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __pyx_t_12 = NULL;
+      __pyx_t_13 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_11))) {
+        __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
+        if (likely(__pyx_t_12)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
+          __Pyx_INCREF(__pyx_t_12);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_11, function);
+          __pyx_t_13 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_12, NULL};
+        __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_13, 0+__pyx_t_13);
+        __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 88, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_7);
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+      }
+      __pyx_t_11 = __Pyx_PyObject_FormatSimple(__pyx_t_7, __pyx_empty_unicode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __pyx_t_10 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_11) > __pyx_t_10) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_11) : __pyx_t_10;
+      __pyx_t_9 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_11);
+      __Pyx_GIVEREF(__pyx_t_11);
+      PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_11);
+      __pyx_t_11 = 0;
+      __pyx_t_11 = __Pyx_PyUnicode_Join(__pyx_t_5, 4, __pyx_t_9, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 88, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = NULL;
+      __pyx_t_13 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __pyx_t_13 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_11};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_13, 1+__pyx_t_13);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      }
+      __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __PYX_ERR(0, 87, __pyx_L1_error)
+
+      /* "bencode2/_encoder.pyx":86
+ *     last_key: bytes = s[0][0]
+ *     for current, _ in s[1:]:
+ *         if last_key == current:             # <<<<<<<<<<<<<<
+ *             raise BencodeEncodeError(
+ *                 f'find duplicated keys {last_key} and {current.decode()}'
+ */
+    }
+
+    /* "bencode2/_encoder.pyx":90
+ *                 f'find duplicated keys {last_key} and {current.decode()}'
+ *             )
+ *         last_key = current             # <<<<<<<<<<<<<<
+ * 
+ * cdef to_binary(s: str | bytes):
+ */
+    if (!(likely(PyBytes_CheckExact(__pyx_v_current))||((__pyx_v_current) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_current))) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_t_4 = __pyx_v_current;
+    __Pyx_INCREF(__pyx_t_4);
+    __Pyx_DECREF_SET(__pyx_v_last_key, ((PyObject*)__pyx_t_4));
+    __pyx_t_4 = 0;
+
+    /* "bencode2/_encoder.pyx":85
+ *         return
+ *     last_key: bytes = s[0][0]
+ *     for current, _ in s[1:]:             # <<<<<<<<<<<<<<
+ *         if last_key == current:
+ *             raise BencodeEncodeError(
+ */
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "bencode2/_encoder.pyx":81
+ *     PyList_Append(r, b"e")
+ * 
+ * cdef __check_duplicated_keys(s: list[tuple[bytes, Any]]):             # <<<<<<<<<<<<<<
+ *     if len(s) == 0:
+ *         return
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_AddTraceback("bencode2._encoder.__check_duplicated_keys", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_last_key);
+  __Pyx_XDECREF(__pyx_v_current);
+  __Pyx_XDECREF(__pyx_v__);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "bencode2/_encoder.pyx":92
+ *         last_key = current
+ * 
+ * cdef to_binary(s: str | bytes):             # <<<<<<<<<<<<<<
+ *     if PyBytes_Check(s):
+ *         return s
+ */
+
+static PyObject *__pyx_f_8bencode2_8_encoder_to_binary(PyObject *__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("to_binary", 1);
+
+  /* "bencode2/_encoder.pyx":93
+ * 
+ * cdef to_binary(s: str | bytes):
+ *     if PyBytes_Check(s):             # <<<<<<<<<<<<<<
+ *         return s
+ * 
+ */
+  __pyx_t_1 = PyBytes_Check(__pyx_v_s);
+  if (__pyx_t_1) {
+
+    /* "bencode2/_encoder.pyx":94
+ * cdef to_binary(s: str | bytes):
+ *     if PyBytes_Check(s):
+ *         return s             # <<<<<<<<<<<<<<
+ * 
+ *     if PyString_Check(s):
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_v_s);
+    __pyx_r = __pyx_v_s;
+    goto __pyx_L0;
+
+    /* "bencode2/_encoder.pyx":93
+ * 
+ * cdef to_binary(s: str | bytes):
+ *     if PyBytes_Check(s):             # <<<<<<<<<<<<<<
+ *         return s
+ * 
+ */
+  }
+
+  /* "bencode2/_encoder.pyx":96
+ *         return s
+ * 
+ *     if PyString_Check(s):             # <<<<<<<<<<<<<<
+ *         return s.encode("utf-8", "strict")
+ * 
+ */
+  __pyx_t_1 = PyString_Check(__pyx_v_s);
+  if (__pyx_t_1) {
+
+    /* "bencode2/_encoder.pyx":97
+ * 
+ *     if PyString_Check(s):
+ *         return s.encode("utf-8", "strict")             # <<<<<<<<<<<<<<
+ * 
+ *     raise TypeError("expected binary or text (found %s)" % type(s))
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_r = __pyx_t_3;
+    __pyx_t_3 = 0;
+    goto __pyx_L0;
+
+    /* "bencode2/_encoder.pyx":96
+ *         return s
+ * 
+ *     if PyString_Check(s):             # <<<<<<<<<<<<<<
+ *         return s.encode("utf-8", "strict")
+ * 
+ */
+  }
+
+  /* "bencode2/_encoder.pyx":99
+ *         return s.encode("utf-8", "strict")
+ * 
+ *     raise TypeError("expected binary or text (found %s)" % type(s))             # <<<<<<<<<<<<<<
+ */
+  __pyx_t_3 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_expected_binary_or_text_found_s, ((PyObject *)Py_TYPE(__pyx_v_s))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __PYX_ERR(0, 99, __pyx_L1_error)
+
+  /* "bencode2/_encoder.pyx":92
+ *         last_key = current
+ * 
+ * cdef to_binary(s: str | bytes):             # <<<<<<<<<<<<<<
+ *     if PyBytes_Check(s):
+ *         return s
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("bencode2._encoder.to_binary", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
@@ -4116,71 +4589,89 @@
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_kp_b_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 0, 0},
     {&__pyx_n_s_Any, __pyx_k_Any, sizeof(__pyx_k_Any), 0, 0, 1, 1},
     {&__pyx_n_s_BencodeEncodeError, __pyx_k_BencodeEncodeError, sizeof(__pyx_k_BencodeEncodeError), 0, 0, 1, 1},
     {&__pyx_n_s_Mapping, __pyx_k_Mapping, sizeof(__pyx_k_Mapping), 0, 0, 1, 1},
+    {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_kp_b__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 0, 0},
-    {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
-    {&__pyx_n_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 1},
+    {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
+    {&__pyx_n_s__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 0, 1, 1},
+    {&__pyx_kp_u_and, __pyx_k_and, sizeof(__pyx_k_and), 0, 1, 0, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_bencode2__encoder, __pyx_k_bencode2__encoder, sizeof(__pyx_k_bencode2__encoder), 0, 0, 1, 1},
     {&__pyx_kp_s_bencode2__encoder_pyx, __pyx_k_bencode2__encoder_pyx, sizeof(__pyx_k_bencode2__encoder_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_collections_abc, __pyx_k_collections_abc, sizeof(__pyx_k_collections_abc), 0, 0, 1, 1},
-    {&__pyx_n_s_compat, __pyx_k_compat, sizeof(__pyx_k_compat), 0, 0, 1, 1},
     {&__pyx_n_b_d, __pyx_k_d, sizeof(__pyx_k_d), 0, 0, 0, 1},
+    {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
     {&__pyx_n_b_e, __pyx_k_e, sizeof(__pyx_k_e), 0, 0, 0, 1},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_encode_dict_locals_lambda, __pyx_k_encode_dict_locals_lambda, sizeof(__pyx_k_encode_dict_locals_lambda), 0, 0, 1, 1},
     {&__pyx_n_s_exceptions, __pyx_k_exceptions, sizeof(__pyx_k_exceptions), 0, 0, 1, 1},
+    {&__pyx_kp_u_expected_binary_or_text_found_s, __pyx_k_expected_binary_or_text_found_s, sizeof(__pyx_k_expected_binary_or_text_found_s), 0, 1, 0, 0},
+    {&__pyx_kp_u_find_duplicated_keys, __pyx_k_find_duplicated_keys, sizeof(__pyx_k_find_duplicated_keys), 0, 1, 0, 0},
     {&__pyx_n_b_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 0, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
     {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
     {&__pyx_n_s_kv, __pyx_k_kv, sizeof(__pyx_k_kv), 0, 0, 1, 1},
     {&__pyx_n_b_l, __pyx_k_l, sizeof(__pyx_k_l), 0, 0, 0, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_kp_u_not_supported, __pyx_k_not_supported, sizeof(__pyx_k_not_supported), 0, 1, 0, 0},
     {&__pyx_n_s_sort, __pyx_k_sort, sizeof(__pyx_k_sort), 0, 0, 1, 1},
+    {&__pyx_n_u_strict, __pyx_k_strict, sizeof(__pyx_k_strict), 0, 1, 0, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-    {&__pyx_n_s_to_binary, __pyx_k_to_binary, sizeof(__pyx_k_to_binary), 0, 0, 1, 1},
     {&__pyx_kp_u_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 1, 0, 0},
     {&__pyx_n_s_typing, __pyx_k_typing, sizeof(__pyx_k_typing), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 99, __pyx_L1_error)
   return 0;
+  __pyx_L1_error:;
+  return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "bencode2/_encoder.pyx":17
+  /* "bencode2/_encoder.pyx":97
+ * 
+ *     if PyString_Check(s):
+ *         return s.encode("utf-8", "strict")             # <<<<<<<<<<<<<<
+ * 
+ *     raise TypeError("expected binary or text (found %s)" % type(s))
+ */
+  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_kp_u_utf_8, __pyx_n_u_strict); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+
+  /* "bencode2/_encoder.pyx":16
  * from ._exceptions import BencodeEncodeError
  * 
  * cpdef bytes encode(value: Any):             # <<<<<<<<<<<<<<
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_value); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__encoder_pyx, __pyx_n_s_encode, 17, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_value); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_bencode2__encoder_pyx, __pyx_n_s_encode, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -4615,79 +5106,58 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Mapping, __pyx_t_3) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "bencode2/_encoder.pyx":14
  * from cpython.string cimport PyString_Check
  * 
- * from ._compat import to_binary             # <<<<<<<<<<<<<<
- * from ._exceptions import BencodeEncodeError
+ * from ._exceptions import BencodeEncodeError             # <<<<<<<<<<<<<<
  * 
+ * cpdef bytes encode(value: Any):
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_INCREF(__pyx_n_s_to_binary);
-  __Pyx_GIVEREF(__pyx_n_s_to_binary);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_to_binary)) __PYX_ERR(0, 14, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_compat, __pyx_t_2, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_INCREF(__pyx_n_s_BencodeEncodeError);
+  __Pyx_GIVEREF(__pyx_n_s_BencodeEncodeError);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_BencodeEncodeError)) __PYX_ERR(0, 14, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_exceptions, __pyx_t_2, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_to_binary); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_BencodeEncodeError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_binary, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeEncodeError, __pyx_t_2) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "bencode2/_encoder.pyx":15
- * 
- * from ._compat import to_binary
- * from ._exceptions import BencodeEncodeError             # <<<<<<<<<<<<<<
- * 
- * cpdef bytes encode(value: Any):
- */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_INCREF(__pyx_n_s_BencodeEncodeError);
-  __Pyx_GIVEREF(__pyx_n_s_BencodeEncodeError);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_BencodeEncodeError)) __PYX_ERR(0, 15, __pyx_L1_error);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_exceptions, __pyx_t_3, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_BencodeEncodeError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_BencodeEncodeError, __pyx_t_3) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-
-  /* "bencode2/_encoder.pyx":17
+  /* "bencode2/_encoder.pyx":16
  * from ._exceptions import BencodeEncodeError
  * 
  * cpdef bytes encode(value: Any):             # <<<<<<<<<<<<<<
  *     r: list[bytes] = []  # makes more sense for something with lots of appends
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_value, __pyx_n_s_Any) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_encoder_1encode, 0, __pyx_n_s_encode, NULL, __pyx_n_s_bencode2__encoder, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_value, __pyx_n_s_Any) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8bencode2_8_encoder_1encode, 0, __pyx_n_s_encode, NULL, __pyx_n_s_bencode2__encoder, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_encode, __pyx_t_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "bencode2/_encoder.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
  * from collections.abc import Mapping
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -4750,14 +5220,173 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
+/* PyObjectGetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro))
+        return tp->tp_getattro(obj, attr_name);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_getattr))
+        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
+#endif
+    return PyObject_GetAttr(obj, attr_name);
+}
+#endif
+
+/* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+#endif
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+#endif
+}
+
+/* GetBuiltinName */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
+        PyErr_Format(PyExc_NameError,
+#if PY_MAJOR_VERSION >= 3
+            "name '%U' is not defined", name);
+#else
+            "name '%.200s' is not defined", PyString_AS_STRING(name));
+#endif
+    }
+    return result;
+}
+
 /* PyFunctionFastCall */
 #if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
@@ -5013,28 +5642,14 @@
 
 /* PyObjectCallOneArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *args[2] = {NULL, arg};
     return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
-/* PyObjectGetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro))
-        return tp->tp_getattro(obj, attr_name);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_getattr))
-        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
-#endif
-    return PyObject_GetAttr(obj, attr_name);
-}
-#endif
-
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     __Pyx_TypeName type_name;
     PyTypeObject *tp = Py_TYPE(obj);
     PyObject *descr;
@@ -5600,159 +6215,14 @@
     }
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    int result;
-    PyObject *exc_type;
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject *current_exception = tstate->current_exception;
-    if (unlikely(!current_exception)) return 0;
-    exc_type = (PyObject*) Py_TYPE(current_exception);
-    if (exc_type == err) return 1;
-#else
-    exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-#endif
-    #if CYTHON_AVOID_BORROWED_REFS
-    Py_INCREF(exc_type);
-    #endif
-    if (unlikely(PyTuple_Check(err))) {
-        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    } else {
-        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-    }
-    #if CYTHON_AVOID_BORROWED_REFS
-    Py_DECREF(exc_type);
-    #endif
-    return result;
-}
-#endif
-
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject *tmp_value;
-    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
-    if (value) {
-        #if CYTHON_COMPILING_IN_CPYTHON
-        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
-        #endif
-            PyException_SetTraceback(value, tb);
-    }
-    tmp_value = tstate->current_exception;
-    tstate->current_exception = value;
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-#else
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#endif
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject* exc_value;
-    exc_value = tstate->current_exception;
-    tstate->current_exception = 0;
-    *value = exc_value;
-    *type = NULL;
-    *tb = NULL;
-    if (exc_value) {
-        *type = (PyObject*) Py_TYPE(exc_value);
-        Py_INCREF(*type);
-        #if CYTHON_COMPILING_IN_CPYTHON
-        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
-        Py_XINCREF(*tb);
-        #else
-        *tb = PyException_GetTraceback(exc_value);
-        #endif
-    }
-#else
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#endif
-}
-#endif
-
-/* PyObjectGetAttrStrNoError */
-#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-#endif
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
-    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
-    return result;
-#else
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-#endif
-}
-
-/* GetBuiltinName */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
-    if (unlikely(!result) && !PyErr_Occurred()) {
-        PyErr_Format(PyExc_NameError,
-#if PY_MAJOR_VERSION >= 3
-            "name '%U' is not defined", name);
-#else
-            "name '%.200s' is not defined", PyString_AS_STRING(name));
-#endif
-    }
-    return result;
-}
-
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -7633,14 +8103,48 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
+/* SliceTupleAndList */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_crop_slice(Py_ssize_t* _start, Py_ssize_t* _stop, Py_ssize_t* _length) {
+    Py_ssize_t start = *_start, stop = *_stop, length = *_length;
+    if (start < 0) {
+        start += length;
+        if (start < 0)
+            start = 0;
+    }
+    if (stop < 0)
+        stop += length;
+    else if (stop > length)
+        stop = length;
+    *_length = stop - start;
+    *_start = start;
+    *_stop = stop;
+}
+static CYTHON_INLINE PyObject* __Pyx_PyList_GetSlice(
+            PyObject* src, Py_ssize_t start, Py_ssize_t stop) {
+    Py_ssize_t length = PyList_GET_SIZE(src);
+    __Pyx_crop_slice(&start, &stop, &length);
+    if (length <= 0) {
+        return PyList_New(0);
+    }
+    return __Pyx_PyList_FromArray(((PyListObject*)src)->ob_item + start, length);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_GetSlice(
+            PyObject* src, Py_ssize_t start, Py_ssize_t stop) {
+    Py_ssize_t length = PyTuple_GET_SIZE(src);
+    __Pyx_crop_slice(&start, &stop, &length);
+    return __Pyx_PyTuple_FromArray(((PyTupleObject*)src)->ob_item + start, length);
+}
+#endif
+
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType_3_0_10
 #define __PYX_HAVE_RT_ImportType_3_0_10
 static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
     size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
@@ -7784,15 +8288,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__3);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__4);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -8205,15 +8709,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__6);
+        name = __Pyx_NewRef(__pyx_n_s__7);
     }
     return name;
 }
 #endif
 
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
```

### Comparing `bencode2-0.0.5/bencode2/_encoder.pyx` & `bencode2-0.0.6/bencode2/_encoder.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from cpython.int cimport PyInt_Check
 from cpython.list cimport PyList_Check, PyList_Append
 from cpython.tuple cimport PyTuple_Check
 from cpython.bool cimport PyBool_Check
 from cpython.dict cimport PyDict_Check
 from cpython.string cimport PyString_Check
 
-from ._compat import to_binary
 from ._exceptions import BencodeEncodeError
 
 cpdef bytes encode(value: Any):
     r: list[bytes] = []  # makes more sense for something with lots of appends
 
     __encode(value, r)
 
@@ -65,15 +64,36 @@
 
     PyList_Append(r, b"e")
 
 cdef __encode_dict(x: Mapping, r: list[bytes]):
     PyList_Append(r, b"d")
 
     # force all keys to bytes, because str and bytes are incomparable
-    i_list = [(to_binary(k), v) for k, v in x.items()]
+    i_list: list[tuple[bytes, Any]] = [(to_binary(k), v) for k, v in x.items()]
     i_list.sort(key=lambda kv: kv[0])
+    __check_duplicated_keys(i_list)
 
     for k, v in i_list:
         __encode(k, r)
         __encode(v, r)
 
     PyList_Append(r, b"e")
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

### Comparing `bencode2-0.0.5/bencode2/_exceptions.c` & `bencode2-0.0.6/bencode2/_exceptions.c`

 * *Files identical despite different names*

### Comparing `bencode2-0.0.5/setup.py` & `bencode2-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 from Cython.Build import cythonize
 
 
 def get_readme():
     """Load README.rst for display on PyPI."""
-    with open('readme.md', 'r', encoding='utf-8') as f:
+    with open("readme.md", "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
-    name='bencode2',
-    version='0.0.5',
-    description='bencode serialize/deserialize library',
+    name="bencode2",
+    version="0.0.6",
+    description="bencode serialize/deserialize library",
     long_description=get_readme(),
-    long_description_content_type='text/markdown',
-    author='trim21',
-    author_email='trim21.me@gmail.com',
-    url='https://github.com/trim21/py-bencode',
-    package_dir={'bencode2': 'bencode2'},
-    packages=['bencode2'],
-    package_data={'bencode2': ['py.typed']},
+    long_description_content_type="text/markdown",
+    author="trim21",
+    author_email="trim21.me@gmail.com",
+    url="https://github.com/trim21/py-bencode",
+    package_dir={"bencode2": "bencode2"},
+    packages=["bencode2"],
+    package_data={"bencode2": ["py.typed"]},
     include_package_data=True,
     ext_modules=cythonize(
         "bencode2/**/*.pyx",
         compiler_directives={"language_level": "3"},
     ),
 )
```

