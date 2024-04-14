# Comparing `tmp/pysqream-blue-1.0.45.tar.gz` & `tmp/pysqream-blue-1.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqream-blue-1.0.45.tar", last modified: Wed Apr  3 10:56:21 2024, max compression
+gzip compressed data, was "pysqream-blue-1.0.46.tar", last modified: Sun Apr 14 14:46:33 2024, max compression
```

## Comparing `pysqream-blue-1.0.45.tar` & `pysqream-blue-1.0.46.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:56:21.809649 pysqream-blue-1.0.45/protos/
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/authentication_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/authentication_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/authentication_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/authentication_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/client_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/client_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/queryhandler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/protos/queryhandler_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/pysqream_blue/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/array_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/casting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    18064 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3237 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/pysqream_blue.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/pysqream_blue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/pysqream_blue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 10:56:21.000000 pysqream-blue-1.0.45/pysqream_blue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:56:21.813649 pysqream-blue-1.0.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-03 10:56:03.000000 pysqream-blue-1.0.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/authentication_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/authentication_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/authentication_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/authentication_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/client_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/client_info_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/queryhandler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/queryhandler_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/pysqream_blue/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/array_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18099 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3237 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/pysqream_blue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/pysqream_blue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/setup.py
```

### Comparing `pysqream-blue-1.0.45/LICENSE` & `pysqream-blue-1.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/PKG-INFO` & `pysqream-blue-1.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.45
+Version: 1.0.46
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 Keywords: database db-api sqream sqreamdbV2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.44
+* **Version:**  1.0.46
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.45/README.rst` & `pysqream-blue-1.0.46/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.44
+* **Version:**  1.0.46
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.45/protos/authentication_pb2.py` & `pysqream-blue-1.0.46/protos/authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/protos/authentication_pb2_grpc.py` & `pysqream-blue-1.0.46/protos/authentication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/protos/authentication_type_pb2.py` & `pysqream-blue-1.0.46/protos/authentication_type_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/protos/client_info_pb2.py` & `pysqream-blue-1.0.46/protos/client_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/protos/error_pb2.py` & `pysqream-blue-1.0.46/protos/error_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/protos/queryhandler_pb2.py` & `pysqream-blue-1.0.46/protos/queryhandler_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/protos/queryhandler_pb2_grpc.py` & `pysqream-blue-1.0.46/protos/queryhandler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/pysqream_blue/array_parser.py` & `pysqream-blue-1.0.46/pysqream_blue/array_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         lists also.
 
         [true, null, false]
     """
     data_fixed_size = struct.calcsize(type_to_letter[sub_type])
     array_size = _get_array_size(data_fixed_size, buffer_len)
 
-    data = buffer[array_size + _padding(array_size):buffer_len]
+    data = buffer[array_size + padding(array_size):buffer_len]
     nulls = buffer[0:array_size]
 
     transform = _get_trasform_func(sub_type, scale)
     return [
         transform(data[i * data_fixed_size:(i + 1) * data_fixed_size], nulls[i])
         for i in range(array_size)
     ]
@@ -67,18 +67,18 @@
 
 
 def _arr_lengths_to_pairs(text_lengths: List[int]):
     """Generator for parsing ARRAY TEXT columns' data"""
     start = 0
     for length in text_lengths:
         yield start, length
-        start = length + _padding(length)
+        start = length + padding(length)
 
 
-def _padding(number: int):
+def padding(number: int):
     return (8 - number % 8) % 8
 
 
 def _get_unfixed_size_array(data: memoryview, nulls: List[bool], dlen: List[int]):
     """Construct one single array from data with dlen right bounds"""
     arr = []
     # lengths_to_pairs is not appropriate due to differences
@@ -133,15 +133,15 @@
      Returns:
          A list with Strings. Array represented as python
          lists also.
 
          ["ABC", "ABCDEF", None]
      """
     num_of_elements = buffer[:8].cast('q')[0]  # Long
-    cur = 8 + num_of_elements + _padding(num_of_elements)
+    cur = 8 + num_of_elements + padding(num_of_elements)
     # data lengths
     d_len = buffer[cur:cur + num_of_elements * 4].cast('i')
     cur += (num_of_elements + num_of_elements % 2) * 4
     data = buffer[cur: buffer_len]
     nulls = buffer[8: 8 + num_of_elements]
     return _get_unfixed_size_array(data, nulls, d_len)
```

### Comparing `pysqream-blue-1.0.45/pysqream_blue/casting.py` & `pysqream-blue-1.0.46/pysqream_blue/casting.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/pysqream_blue/connection.py` & `pysqream-blue-1.0.46/pysqream_blue/connection.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/pysqream_blue/cursor.py` & `pysqream-blue-1.0.46/pysqream_blue/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
                     row.append(None)
                 elif col_meta.type == qh_messages.COLUMN_TYPE_ARRAY:
                     buffer_len = col_data[1][i] if col_meta.nullable else col_data[0][i]
                     data_buffer = col_data[-1]
                     array_object = array_parser.convert_buffer_to_array(
                         data_buffer[0:buffer_len], buffer_len, col_meta.sub_type, col_meta.scale)
                     row.append(array_object)
-                    col_data[-1] = col_data[-1][buffer_len:]
+                    col_data[-1] = col_data[-1][buffer_len + array_parser.padding(buffer_len):]
                 elif col_meta.tru_varchar:
                     size = col_data[1][i] if col_meta.nullable else col_data[0][i]
                     start_byte = add_and_return(size)
                     current_size = col_data[-1]
                     data = col_data[2] if col_meta.nullable else col_data[1]
                     row.append(data[current_size: current_size + size].decode('utf8'))
                     col_data[-1] += start_byte
```

### Comparing `pysqream-blue-1.0.45/pysqream_blue/globals.py` & `pysqream-blue-1.0.46/pysqream_blue/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import protos.queryhandler_pb2_grpc as qh_services
 import protos.authentication_pb2 as auth_messages
 import protos.authentication_pb2_grpc as auth_services
 import protos.client_info_pb2 as cl_messages
 import protos.client_info_pb2_grpc as cl_services
 import protos.authentication_type_pb2 as auth_type_messages
 
-__version__ = '1.0.45'
+__version__ = '1.0.46'
 
 dbapi_typecodes = {
     qh_messages.COLUMN_TYPE_LONG_INT:  'NUMBER',
     qh_messages.COLUMN_TYPE_ULONG_INT: 'NUMBER',
     qh_messages.COLUMN_TYPE_INT:       'NUMBER',
     qh_messages.COLUMN_TYPE_UINT:      'NUMBER',
     qh_messages.COLUMN_TYPE_VARCHAR:   'STRING',
```

### Comparing `pysqream-blue-1.0.45/pysqream_blue/logger.py` & `pysqream-blue-1.0.46/pysqream_blue/logger.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/pysqream_blue/pysqream_blue.py` & `pysqream-blue-1.0.46/pysqream_blue/pysqream_blue.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/pysqream_blue/utils.py` & `pysqream-blue-1.0.46/pysqream_blue/utils.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/pysqream_blue.egg-info/PKG-INFO` & `pysqream-blue-1.0.46/pysqream_blue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.45
+Version: 1.0.46
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 Keywords: database db-api sqream sqreamdbV2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.44
+* **Version:**  1.0.46
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
```

### Comparing `pysqream-blue-1.0.45/pysqream_blue.egg-info/SOURCES.txt` & `pysqream-blue-1.0.46/pysqream_blue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.45/setup.py` & `pysqream-blue-1.0.46/setup.py`

 * *Files identical despite different names*

