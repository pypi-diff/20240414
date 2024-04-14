# Comparing `tmp/ABSQL-0.6.0.tar.gz` & `tmp/absql-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABSQL-0.6.0.tar", last modified: Mon Apr  8 23:05:50 2024, max compression
+gzip compressed data, was "absql-0.6.1.tar", last modified: Sun Apr 14 01:20:41 2024, max compression
```

## Comparing `ABSQL-0.6.0.tar` & `absql-0.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.149817 ABSQL-0.6.0/
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.148357 ABSQL-0.6.0/ABSQL.egg-info/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/SOURCES.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/dependency_links.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       74 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/requires.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/top_level.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 ABSQL-0.6.0/LICENSE
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-08 23:05:50.149073 ABSQL-0.6.0/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 ABSQL-0.6.0/README.md
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.138519 ABSQL-0.6.0/absql/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 ABSQL-0.6.0/absql/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.139696 ABSQL-0.6.0/absql/files/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      790 2024-04-06 14:26:22.000000 ABSQL-0.6.0/absql/files/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 ABSQL-0.6.0/absql/files/loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3297 2024-04-08 22:30:40.000000 ABSQL-0.6.0/absql/files/parsers.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.141226 ABSQL-0.6.0/absql/functions/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/functions/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 ABSQL-0.6.0/absql/functions/db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/functions/env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/functions/time.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.141503 ABSQL-0.6.0/absql/render/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3084 2024-04-08 13:55:50.000000 ABSQL-0.6.0/absql/render/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.141797 ABSQL-0.6.0/absql/text/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/text/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.142103 ABSQL-0.6.0/absql/utils/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/utils/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-08 23:05:50.149938 ABSQL-0.6.0/setup.cfg
--rw-r--r--   0 chriscardillo   (501) staff       (20)      846 2024-04-08 22:22:37.000000 ABSQL-0.6.0/setup.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.147827 ABSQL-0.6.0/tests/
--rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_copy.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_funcs_db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_funcs_env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_funcs_time.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      923 2024-04-08 22:22:07.000000 ABSQL-0.6.0/tests/test_parse_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 ABSQL-0.6.0/tests/test_partial_kwargs.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 ABSQL-0.6.0/tests/test_render.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3575 2024-02-09 23:11:51.000000 ABSQL-0.6.0/tests/test_render_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1393 2024-04-08 22:31:38.000000 ABSQL-0.6.0/tests/test_render_file_return_dict.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_render_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_set.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_utils.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.643957 absql-0.6.1/
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.642482 absql-0.6.1/ABSQL.egg-info/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       74 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/requires.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-14 01:20:41.000000 absql-0.6.1/ABSQL.egg-info/top_level.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 absql-0.6.1/LICENSE
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-14 01:20:41.643258 absql-0.6.1/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 absql-0.6.1/README.md
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.632637 absql-0.6.1/absql/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 absql-0.6.1/absql/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.633735 absql-0.6.1/absql/files/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      790 2024-04-06 14:26:22.000000 absql-0.6.1/absql/files/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 absql-0.6.1/absql/files/loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     4100 2024-04-14 01:16:37.000000 absql-0.6.1/absql/files/parsers.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.635191 absql-0.6.1/absql/functions/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 absql-0.6.1/absql/functions/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 absql-0.6.1/absql/functions/db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 absql-0.6.1/absql/functions/env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 absql-0.6.1/absql/functions/time.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.635456 absql-0.6.1/absql/render/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3084 2024-04-08 13:55:50.000000 absql-0.6.1/absql/render/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.635800 absql-0.6.1/absql/text/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 absql-0.6.1/absql/text/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.636086 absql-0.6.1/absql/utils/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 absql-0.6.1/absql/utils/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-14 01:20:41.644110 absql-0.6.1/setup.cfg
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      846 2024-04-14 01:16:33.000000 absql-0.6.1/setup.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-14 01:20:41.641816 absql-0.6.1/tests/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 absql-0.6.1/tests/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_copy.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_funcs_db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_funcs_env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_funcs_time.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      923 2024-04-08 22:22:07.000000 absql-0.6.1/tests/test_parse_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 absql-0.6.1/tests/test_partial_kwargs.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 absql-0.6.1/tests/test_render.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3865 2024-04-14 01:15:40.000000 absql-0.6.1/tests/test_render_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1393 2024-04-14 01:15:28.000000 absql-0.6.1/tests/test_render_file_return_dict.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_render_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_set.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 absql-0.6.1/tests/test_utils.py
```

### Comparing `ABSQL-0.6.0/ABSQL.egg-info/PKG-INFO` & `absql-0.6.1/ABSQL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.6.0
+Version: 0.6.1
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.6.0/ABSQL.egg-info/SOURCES.txt` & `absql-0.6.1/ABSQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/LICENSE` & `absql-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/PKG-INFO` & `absql-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.6.0
+Version: 0.6.1
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.6.0/README.md` & `absql-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/__init__.py` & `absql-0.6.1/absql/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/files/__init__.py` & `absql-0.6.1/absql/files/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/files/loader.py` & `absql-0.6.1/absql/files/loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/files/parsers.py` & `absql-0.6.1/absql/files/parsers.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             content = content.strip("\n")
         elif text.startswith("{"):
             tmp_header = "/*ABSQLQSBA*/ "
             text = tmp_header + text
             metadata = {}
             content = yaml.load(text, Loader=loader)
             content = content.replace(tmp_header, "")
-        elif text.startswith("/*") and file_path.endswith((".sql", "js")):
+        elif text.startswith("/*") and file_path.endswith(".sql"):
             # Retrieve the first matched set of text within a block comment
             # (i.e. /* ... */).
             metadata = (
                 re.compile(r"^\/\*([\S\s]*?)\*\/$", re.MULTILINE).match(text).group(1)
             )
             # Text after the first block-comment end is considered the content of the
             # SQL file. This will handle block comments within the contents as well.
@@ -65,20 +65,40 @@
     file_content["absql_body"] = raw_content["content"]
     return file_content
 
 
 def parse_js(file_path, loader=None):
     if loader is None:
         loader = generate_loader()
-    raw_content = frontmatter_load(file_path, loader=loader)
-    file_content = raw_content["metadata"]
-    file_content["absql_body"] = raw_content["content"]
+    with open(file_path, "r") as file:
+        text = "".join(file.readlines())
+        if text.startswith("/*"):
+            # Retrieve the first matched set of text within a block comment
+            # (i.e. /* ... */).
+            metadata = (
+                re.compile(r"^\/\*([\S\s]*?)\*\/$", re.MULTILINE).match(text).group(1)
+            )
+            # Text after the first block-comment end is considered the content of the
+            # SQL file. This will handle block comments within the contents as well.
+            _, _, content = text.partition("*/")
+            metadata = yaml.load(metadata, Loader=loader)
+            content = content.strip("\n")
+        else:
+            metadata = {}
+            content = text.strip("\n")
+    file_content = metadata
+    file_content["absql_body"] = content
     return file_content
 
 
 def parse_py(file_path, loader=None):
     if loader is None:
         loader = generate_loader()
     raw_content = jupytext.read(file_path)["cells"]
-    file_content = yaml.load(raw_content[0]["source"].replace("---", ""), Loader=loader)
-    file_content["absql_body"] = raw_content[1]["source"]
+    if raw_content[0]["source"].startswith("---"):
+        file_content = yaml.load(
+            raw_content[0]["source"].replace("---", ""), Loader=loader
+        )
+        file_content["absql_body"] = raw_content[1]["source"]
+    else:
+        file_content = {"absql_body": raw_content[0]["source"]}
     return file_content
```

### Comparing `ABSQL-0.6.0/absql/functions/__init__.py` & `absql-0.6.1/absql/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/functions/db.py` & `absql-0.6.1/absql/functions/db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/functions/env.py` & `absql-0.6.1/absql/functions/env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/render/__init__.py` & `absql-0.6.1/absql/render/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/text/__init__.py` & `absql-0.6.1/absql/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/absql/utils/__init__.py` & `absql-0.6.1/absql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/setup.py` & `absql-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ABSQL",
-    version="0.6.0",
+    version="0.6.1",
     author="Chris Cardillo",
     author_email="cfcardillo23@gmail.com",
     description="A rendering engine for templated SQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pipeline-tools/ABSQL",
     packages=setuptools.find_packages(),
```

### Comparing `ABSQL-0.6.0/tests/test_copy.py` & `absql-0.6.1/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_funcs_db.py` & `absql-0.6.1/tests/test_funcs_db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_funcs_env.py` & `absql-0.6.1/tests/test_funcs_env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_funcs_time.py` & `absql-0.6.1/tests/test_funcs_time.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_loader.py` & `absql-0.6.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_parse_file.py` & `absql-0.6.1/tests/test_parse_file.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_partial_kwargs.py` & `absql-0.6.1/tests/test_partial_kwargs.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_render.py` & `absql-0.6.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_render_file.py` & `absql-0.6.1/tests/test_render_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,7 +130,17 @@
     assert got == want
 
 
 def test_constructor_plus_function(constructor_plus_function_sql_path):
     got = r.render_file(constructor_plus_function_sql_path)
     want = "SELECT * FROM somewhere_else"
     assert got == want
+
+
+def test_render_file_js_no_front():
+    res = r.render_file("tests/files/simple_no_front.js")
+    assert res == """var my_dict = {"hello": "goodbye"}"""
+
+
+def test_render_file_py_no_front():
+    res = r.render_file("tests/files/simple_no_front.py")
+    assert res == """print("hello")"""
```

### Comparing `ABSQL-0.6.0/tests/test_render_file_return_dict.py` & `absql-0.6.1/tests/test_render_file_return_dict.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_render_text.py` & `absql-0.6.1/tests/test_render_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_text.py` & `absql-0.6.1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.6.0/tests/test_utils.py` & `absql-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

