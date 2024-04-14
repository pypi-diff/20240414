# Comparing `tmp/moneywiz-api-0.1.1.tar.gz` & `tmp/moneywiz_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneywiz-api-0.1.1.tar", last modified: Mon Mar 18 20:53:33 2024, max compression
+gzip compressed data, was "moneywiz_api-0.2.1.tar", last modified: Sun Apr 14 16:44:47 2024, max compression
```

## Comparing `moneywiz-api-0.1.1.tar` & `moneywiz_api-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:33.426297 moneywiz-api-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-18 20:53:33.426297 moneywiz-api-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 20:53:33.426297 moneywiz-api-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:33.422297 moneywiz-api-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:33.422297 moneywiz-api-0.1.1/src/moneywiz_api/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/database_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:33.422297 moneywiz-api-0.1.1/src/moneywiz_api/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/managers/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/managers/category_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/managers/investment_holding_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/managers/payee_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/managers/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/managers/tag_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/managers/transaction_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:33.426297 moneywiz-api-0.1.1/src/moneywiz_api/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/model/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/model/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/model/investment_holding.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/model/payee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/model/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/moneywiz_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/moneywiz_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:33.426297 moneywiz-api-0.1.1/src/moneywiz_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-18 20:53:33.000000 moneywiz-api-0.1.1/src/moneywiz_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-18 20:53:33.000000 moneywiz-api-0.1.1/src/moneywiz_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:53:33.000000 moneywiz-api-0.1.1/src/moneywiz_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 20:53:33.000000 moneywiz-api-0.1.1/src/moneywiz_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/src/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:53:33.426297 moneywiz-api-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-18 20:53:28.000000 moneywiz-api-0.1.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.434098 moneywiz_api-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.434098 moneywiz_api-0.2.1/src/moneywiz_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/database_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/src/moneywiz_api/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/category_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/investment_holding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/payee_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/tag_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/managers/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/src/moneywiz_api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/investment_holding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/payee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/moneywiz_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/moneywiz_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-14 16:44:47.000000 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-14 16:44:47.000000 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:44:47.000000 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 16:44:47.000000 moneywiz_api-0.2.1/src/moneywiz_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/src/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:47.438098 moneywiz_api-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-14 16:44:43.000000 moneywiz_api-0.2.1/tests/test_config.py
```

### Comparing `moneywiz-api-0.1.1/LICENSE` & `moneywiz_api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/PKG-INFO` & `moneywiz_api-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 0.1.1
+Version: 0.2.1
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 0.1.1 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 0.2.1 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
```

### Comparing `moneywiz-api-0.1.1/README.md` & `moneywiz_api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/pyproject.toml` & `moneywiz_api-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "moneywiz-api"
-version = "0.1.1"
+version = "0.2.1"
 authors = [
     { name="iLeoDo", email="iLeoDo@gmail.com" },
 ]
 description = "A Python api to access moneywiz sqlite database"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/database_accessor.py` & `moneywiz_api-0.2.1/src/moneywiz_api/database_accessor.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/managers/account_manager.py` & `moneywiz_api-0.2.1/src/moneywiz_api/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/managers/category_manager.py` & `moneywiz_api-0.2.1/src/moneywiz_api/managers/category_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/managers/investment_holding_manager.py` & `moneywiz_api-0.2.1/src/moneywiz_api/managers/investment_holding_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/managers/record_manager.py` & `moneywiz_api-0.2.1/src/moneywiz_api/managers/record_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/managers/transaction_manager.py` & `moneywiz_api-0.2.1/src/moneywiz_api/managers/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/model/__init__.py` & `moneywiz_api-0.2.1/src/moneywiz_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/model/account.py` & `moneywiz_api-0.2.1/src/moneywiz_api/model/account.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/model/category.py` & `moneywiz_api-0.2.1/src/moneywiz_api/model/category.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/model/investment_holding.py` & `moneywiz_api-0.2.1/src/moneywiz_api/model/investment_holding.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/model/record.py` & `moneywiz_api-0.2.1/src/moneywiz_api/model/record.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/model/transaction.py` & `moneywiz_api-0.2.1/src/moneywiz_api/model/transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -229,28 +229,46 @@
     ENT: 43
     """
 
     account: ID
     amount: float
     payee: Optional[ID]
 
+    # FX
+    original_currency: str
+    original_amount: float
+    original_exchange_rate: Optional[float]
+
     def __init__(self, row):
         super().__init__(row)
         self.account = row["ZACCOUNT2"]
         self.amount = row["ZAMOUNT1"]
         self.payee = row["ZPAYEE2"]
 
+        self.original_currency = row["ZORIGINALCURRENCY"]
+        self.original_amount = row["ZORIGINALAMOUNT"]
+        self.original_exchange_rate = row["ZORIGINALEXCHANGERATE"]
+
         # Validate
         self.validate()
 
     def validate(self):
         assert self.account is not None
         assert self.amount is not None
         assert self.amount > 0
 
+        assert self.original_currency is not None
+        assert self.original_amount is not None
+        assert self.original_amount > 0
+
+        if self.original_exchange_rate is not None:
+            assert self.amount == pytest.approx(
+                self.original_amount * self.original_exchange_rate, abs=0.001
+            )
+
 
 @dataclass
 class TransferBudgetTransaction(Transaction):
     """
     ENT: 44
     """
```

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api/moneywiz_api.py` & `moneywiz_api-0.2.1/src/moneywiz_api/moneywiz_api.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api.egg-info/PKG-INFO` & `moneywiz_api-0.2.1/src/moneywiz_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 0.1.1
+Version: 0.2.1
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 0.1.1 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 0.2.1 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
```

### Comparing `moneywiz-api-0.1.1/src/moneywiz_api.egg-info/SOURCES.txt` & `moneywiz_api-0.2.1/src/moneywiz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.1.1/src/shell.py` & `moneywiz_api-0.2.1/src/shell.py`

 * *Files identical despite different names*

