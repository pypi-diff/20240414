# Comparing `tmp/icodes-0.1.2.tar.gz` & `tmp/icodes-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icodes-0.1.2.tar", max compression
+gzip compressed data, was "icodes-0.1.3.tar", max compression
```

## Comparing `icodes-0.1.2.tar` & `icodes-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7048 2024-03-31 18:37:25.121754 icodes-0.1.2/LICENSE
--rw-r--r--   0        0        0     2883 2024-04-14 10:21:32.481639 icodes-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-06 19:55:00.301396 icodes-0.1.2/icds/__init__.py
--rw-r--r--   0        0        0     1935 2024-04-14 09:52:58.273822 icodes-0.1.2/icds/data.py
--rw-r--r--   0        0        0     1285 2024-04-14 09:43:58.775498 icodes-0.1.2/icds/git_helpers.py
--rw-r--r--   0        0        0     3124 2024-04-06 19:55:00.301396 icodes-0.1.2/icds/llm_interface.py
--rw-r--r--   0        0        0      797 2024-04-14 09:43:58.775498 icodes-0.1.2/icds/models.py
--rw-r--r--   0        0        0      241 2024-04-06 19:55:00.301396 icodes-0.1.2/icds/settings.py
--rw-r--r--   0        0        0     4520 2024-04-14 11:28:48.808145 icodes-0.1.2/icodes.py
--rw-r--r--   0        0        0     1145 2024-04-14 11:29:22.631732 icodes-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 icodes-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7048 2024-03-31 18:37:25.121754 icodes-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3198 2024-04-14 11:34:16.112163 icodes-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 19:55:00.301396 icodes-0.1.3/icds/__init__.py
+-rw-r--r--   0        0        0     1935 2024-04-14 09:52:58.273822 icodes-0.1.3/icds/data.py
+-rw-r--r--   0        0        0     1285 2024-04-14 09:43:58.775498 icodes-0.1.3/icds/git_helpers.py
+-rw-r--r--   0        0        0     3124 2024-04-06 19:55:00.301396 icodes-0.1.3/icds/llm_interface.py
+-rw-r--r--   0        0        0      797 2024-04-14 09:43:58.775498 icodes-0.1.3/icds/models.py
+-rw-r--r--   0        0        0      236 2024-04-14 11:31:26.942217 icodes-0.1.3/icds/settings.py
+-rw-r--r--   0        0        0     4520 2024-04-14 11:28:48.808145 icodes-0.1.3/icodes.py
+-rw-r--r--   0        0        0     1145 2024-04-14 11:34:40.779865 icodes-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4256 1970-01-01 00:00:00.000000 icodes-0.1.3/PKG-INFO
```

### Comparing `icodes-0.1.2/LICENSE` & `icodes-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `icodes-0.1.2/README.md` & `icodes-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 ## Installation
 
 iCODES requires Python 3.11 or higher. 
 
     pip install icodes
 
+Since the only supported LLM backend right now is OpenAI, you will need to export your OpenAI API key to the environment variable `OPENAI_API_KEY`. You can also set the `DEFAULT_MODEL` environment variable to the GPT model you wish to use (default value is "gpt-3.5-turbo" for a reasonable price / quality ratio.)
+
 ### Alternative installation 
 
 Or clone the repo:
 
     git clone https://github.com/a115/iCODES.git
 
 It is recommended to use Poetry for dependency management. To install the dependencies, run:
```

### Comparing `icodes-0.1.2/icds/data.py` & `icodes-0.1.3/icds/data.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.2/icds/git_helpers.py` & `icodes-0.1.3/icds/git_helpers.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.2/icds/llm_interface.py` & `icodes-0.1.3/icds/llm_interface.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.2/icds/models.py` & `icodes-0.1.3/icds/models.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.2/icodes.py` & `icodes-0.1.3/icodes.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.2/pyproject.toml` & `icodes-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "icodes"
-version = "0.1.2"
+version = "0.1.3"
 description = "LLM-powered Git archeology tool (a.k.a. Intelligent Commit Ontology Distiller and Enhanced Search)"
 authors = ["Jordan Dimov <jdimov@a115.co.uk>", "Bayo Ade <bayo.300@gmail.com>"]
 license = "CC0-1.0"
 readme = "README.md"
 packages = [
     { include = "icodes.py" },
     { include = "icds/**/*.py" },
```

### Comparing `icodes-0.1.2/PKG-INFO` & `icodes-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icodes
-Version: 0.1.2
+Version: 0.1.3
 Summary: LLM-powered Git archeology tool (a.k.a. Intelligent Commit Ontology Distiller and Enhanced Search)
 Home-page: https://github.com/a115/iCODES
 License: CC0-1.0
 Keywords: git,llm,archeology,commit,search
 Author: Jordan Dimov
 Author-email: jdimov@a115.co.uk
 Requires-Python: >=3.11,<4.0
@@ -40,14 +40,16 @@
 
 ## Installation
 
 iCODES requires Python 3.11 or higher. 
 
     pip install icodes
 
+Since the only supported LLM backend right now is OpenAI, you will need to export your OpenAI API key to the environment variable `OPENAI_API_KEY`. You can also set the `DEFAULT_MODEL` environment variable to the GPT model you wish to use (default value is "gpt-3.5-turbo" for a reasonable price / quality ratio.)
+
 ### Alternative installation 
 
 Or clone the repo:
 
     git clone https://github.com/a115/iCODES.git
 
 It is recommended to use Poetry for dependency management. To install the dependencies, run:
```

