# Comparing `tmp/schwab-py-0.0.0a7.tar.gz` & `tmp/schwab-py-0.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-py-0.0.0a7.tar", last modified: Sun Apr 14 17:42:34 2024, max compression
+gzip compressed data, was "schwab-py-0.0.0a8.tar", last modified: Sun Apr 14 18:27:09 2024, max compression
```

## Comparing `schwab-py-0.0.0a7.tar` & `schwab-py-0.0.0a8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.278700 schwab-py-0.0.0a7/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a7/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 17:42:34.278627 schwab-py-0.0.0a7/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a7/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.276033 schwab-py-0.0.0a7/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a7/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    24395 2024-04-08 21:07:33.000000 schwab-py-0.0.0a7/schwab/auth.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.276592 schwab-py-0.0.0a7/schwab/client/
--rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a7/schwab/client/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a7/schwab/client/asynchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    25591 2024-04-14 17:39:18.000000 schwab-py-0.0.0a7/schwab/client/base.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-06 13:43:58.000000 schwab-py-0.0.0a7/schwab/client/synchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a7/schwab/debug.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.277221 schwab-py-0.0.0a7/schwab/orders/
--rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-04-06 23:27:37.000000 schwab-py-0.0.0a7/schwab/orders/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    11013 2024-04-14 17:35:12.000000 schwab-py-0.0.0a7/schwab/orders/common.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-04-14 17:35:34.000000 schwab-py-0.0.0a7/schwab/orders/equities.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    14184 2024-04-14 17:37:24.000000 schwab-py-0.0.0a7/schwab/orders/generic.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    17394 2024-04-14 17:35:49.000000 schwab-py-0.0.0a7/schwab/orders/options.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a7/schwab/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-14 17:41:58.000000 schwab-py-0.0.0a7/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.278144 schwab-py-0.0.0a7/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)      532 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-14 17:42:34.279022 schwab-py-0.0.0a7/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-06 13:16:58.000000 schwab-py-0.0.0a7/setup.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.277984 schwab-py-0.0.0a7/tests/
--rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a7/tests/test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.045671 schwab-py-0.0.0a8/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a8/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 18:27:09.045597 schwab-py-0.0.0a8/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a8/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.043051 schwab-py-0.0.0a8/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a8/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    24395 2024-04-08 21:07:33.000000 schwab-py-0.0.0a8/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.043558 schwab-py-0.0.0a8/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a8/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a8/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    27732 2024-04-14 18:26:28.000000 schwab-py-0.0.0a8/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-06 13:43:58.000000 schwab-py-0.0.0a8/schwab/client/synchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a8/schwab/debug.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.044223 schwab-py-0.0.0a8/schwab/orders/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-04-06 23:27:37.000000 schwab-py-0.0.0a8/schwab/orders/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    11013 2024-04-14 17:35:12.000000 schwab-py-0.0.0a8/schwab/orders/common.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-04-14 17:35:34.000000 schwab-py-0.0.0a8/schwab/orders/equities.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    14184 2024-04-14 17:37:24.000000 schwab-py-0.0.0a8/schwab/orders/generic.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17394 2024-04-14 17:35:49.000000 schwab-py-0.0.0a8/schwab/orders/options.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a8/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-14 18:26:39.000000 schwab-py-0.0.0a8/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.045114 schwab-py-0.0.0a8/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)      532 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-14 18:27:09.000000 schwab-py-0.0.0a8/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-14 18:27:09.045986 schwab-py-0.0.0a8/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-06 13:16:58.000000 schwab-py-0.0.0a8/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:27:09.044961 schwab-py-0.0.0a8/tests/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a8/tests/test.py
```

### Comparing `schwab-py-0.0.0a7/LICENSE` & `schwab-py-0.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/PKG-INFO` & `schwab-py-0.0.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
```

### Comparing `schwab-py-0.0.0a7/README.rst` & `schwab-py-0.0.0a8/README.rst`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/auth.py` & `schwab-py-0.0.0a8/schwab/auth.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/client/asynchronous.py` & `schwab-py-0.0.0a8/schwab/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/client/base.py` & `schwab-py-0.0.0a8/schwab/client/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -631,7 +631,64 @@
         if isinstance(order_spec, OrderBuilder):
             order_spec = order_spec.build()
 
         path = '/v1/trader/accounts/{}/previewOrder'.format(account_hash)
         return self._post_request(path, order_spec)
 
 
+    ##########################################################################
+    # Quotes
+
+    class GetQuote:
+        class Fields(Enum):
+            QUOTE = 'quote'
+            FUNDAMENTAL = 'fundamental'
+
+    def get_quote(self, symbol, *, fields=None):
+        '''
+        Get quote for a symbol. Note due to limitations in URL encoding, this
+        method is not recommended for instruments with symbols symbols
+        containing non-alphanumeric characters, for example as futures like
+        ``/ES``. To get quotes for those symbols, use :meth:`Client.get_quotes`.
+
+        :param symbol: Single symbol to fetch
+        :param fields: Fields to request. If unset, return all available data. 
+                       i.e. all fields. See :class:`GetQuote.Field` for options.
+        '''
+        fields = self.convert_enum_iterable(fields, self.GetQuote.Fields)
+        if fields:
+            params = {'fields': fields}
+        else:
+            params = {}
+
+        path = '/marketdata/v1/{}/quotes'.format(symbol)
+        return self._get_request(path, params)
+
+    def get_quotes(self, symbols, *, fields=None, indicative=None):
+        '''Get quote for a symbol. This method supports all symbols, including
+        those containing non-alphanumeric characters like ``/ES``.
+
+        :param symbols: Iterable of symbols to fetch.
+        :param fields: Fields to request. If unset, return all available data. 
+                       i.e. all fields. See :class:`GetQuote.Field` for options.
+        '''
+        if isinstance(symbols, str):
+            symbols = [symbols]
+
+        params = {
+            'symbols': ','.join(symbols)
+        }
+
+        fields = self.convert_enum_iterable(fields, self.GetQuote.Fields)
+        if fields:
+            params['fields'] = fields
+
+        if indicative is not None:
+            if type(indicative) is not bool:
+                raise ValueError(
+                        'value of \'indicative\' must be either True or False')
+            params['indicative'] = 'true' if indicative else 'false'
+
+        path = '/marketdata/v1/quotes'
+        return self._get_request(path, params)
+
+
```

### Comparing `schwab-py-0.0.0a7/schwab/client/synchronous.py` & `schwab-py-0.0.0a8/schwab/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/debug.py` & `schwab-py-0.0.0a8/schwab/debug.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/orders/__init__.py` & `schwab-py-0.0.0a8/schwab/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/orders/common.py` & `schwab-py-0.0.0a8/schwab/orders/common.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/orders/equities.py` & `schwab-py-0.0.0a8/schwab/orders/equities.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/orders/generic.py` & `schwab-py-0.0.0a8/schwab/orders/generic.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/orders/options.py` & `schwab-py-0.0.0a8/schwab/orders/options.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab/utils.py` & `schwab-py-0.0.0a8/schwab/utils.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/schwab_py.egg-info/PKG-INFO` & `schwab-py-0.0.0a8/schwab_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a7
+Version: 0.0.0a8
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
```

### Comparing `schwab-py-0.0.0a7/schwab_py.egg-info/SOURCES.txt` & `schwab-py-0.0.0a8/schwab_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/setup.cfg` & `schwab-py-0.0.0a8/setup.cfg`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a7/setup.py` & `schwab-py-0.0.0a8/setup.py`

 * *Files identical despite different names*

