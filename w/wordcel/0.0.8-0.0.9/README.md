# Comparing `tmp/wordcel-0.0.8.tar.gz` & `tmp/wordcel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordcel-0.0.8.tar", max compression
+gzip compressed data, was "wordcel-0.0.9.tar", max compression
```

## Comparing `wordcel-0.0.8.tar` & `wordcel-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2023-07-25 01:08:30.881980 wordcel-0.0.8/LICENSE
--rw-r--r--   0        0        0     2783 2023-07-25 21:14:13.262827 wordcel-0.0.8/README.md
--rw-r--r--   0        0        0      333 2023-08-09 00:59:58.577670 wordcel-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 00:46:00.681902 wordcel-0.0.8/wordcel/__init__.py
--rw-r--r--   0        0        0     2671 2023-08-09 01:03:09.703779 wordcel-0.0.8/wordcel/featurize.py
--rw-r--r--   0        0        0     1042 2023-07-25 00:48:13.299968 wordcel-0.0.8/wordcel/llm_providers.py
--rw-r--r--   0        0        0     3603 1970-01-01 00:00:00.000000 wordcel-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-25 01:08:30.881980 wordcel-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2783 2023-07-25 21:14:13.262827 wordcel-0.0.9/README.md
+-rw-r--r--   0        0        0      333 2023-08-09 01:14:11.501088 wordcel-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 00:46:00.681902 wordcel-0.0.9/wordcel/__init__.py
+-rw-r--r--   0        0        0     2768 2023-08-09 01:14:05.831186 wordcel-0.0.9/wordcel/featurize.py
+-rw-r--r--   0        0        0     1042 2023-07-25 00:48:13.299968 wordcel-0.0.9/wordcel/llm_providers.py
+-rw-r--r--   0        0        0     3603 1970-01-01 00:00:00.000000 wordcel-0.0.9/PKG-INFO
```

### Comparing `wordcel-0.0.8/LICENSE` & `wordcel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.8/README.md` & `wordcel-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.8/wordcel/featurize.py` & `wordcel-0.0.9/wordcel/featurize.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,16 +39,17 @@
 
     user_fn_name = user_function.__name__
 
     def process_text_with_caching(text, identifier):
         if cache_folder:
             # Check if result is already cached
             identifier = str(identifier).replace("/", "_")
+            result_field_normalized = result_field.replace("/", "_")  # For naming...
             cache_file = os.path.join(
-                cache_folder, f"{identifier}_{user_fn_name}_{result_field}.json"
+                cache_folder, f"{identifier}_{user_fn_name}_{result_field_normalized}.json"
             )
             if os.path.exists(cache_file):
                 with open(cache_file, "r") as f:
                     print(f"Found cached result: {cache_file}.")
                     return json.load(f)
 
         result = user_function(text)
```

### Comparing `wordcel-0.0.8/wordcel/llm_providers.py` & `wordcel-0.0.9/wordcel/llm_providers.py`

 * *Files identical despite different names*

### Comparing `wordcel-0.0.8/PKG-INFO` & `wordcel-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordcel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create text-based features from large language models
 Author: Andrew Han
 Author-email: handrew11@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

