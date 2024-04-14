# Comparing `tmp/deepchecks-llm-client-0.9.1.tar.gz` & `tmp/deepchecks-llm-client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchecks-llm-client-0.9.1.tar", last modified: Sun Jan 21 10:21:08 2024, max compression
+gzip compressed data, was "deepchecks-llm-client-0.9.2.tar", last modified: Mon Jan 22 13:34:29 2024, max compression
```

## Comparing `deepchecks-llm-client-0.9.1.tar` & `deepchecks-llm-client-0.9.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:08.835920 deepchecks-llm-client-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-21 10:21:08.835920 deepchecks-llm-client-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:08.831920 deepchecks-llm-client-0.9.1/deepchecks_llm_client/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16178 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:08.831920 deepchecks-llm-client-0.9.1/deepchecks_llm_client/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/examples/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/openai_instrumentor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:08.831920 deepchecks-llm-client-0.9.1/deepchecks_llm_client/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:08.831920 deepchecks-llm-client-0.9.1/deepchecks_llm_client/sdk/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/sdk/langchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:08.835920 deepchecks-llm-client-0.9.1/deepchecks_llm_client/sdk/langchain/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/sdk/langchain/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/sdk/langchain/callbacks/deepchecks_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 10:21:08.831920 deepchecks-llm-client-0.9.1/deepchecks_llm_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-21 10:21:08.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-21 10:21:08.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 10:21:08.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-21 10:21:08.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-21 10:21:08.000000 deepchecks-llm-client-0.9.1/deepchecks_llm_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 10:21:08.835920 deepchecks-llm-client-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-21 10:21:04.000000 deepchecks-llm-client-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/deepchecks_llm_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16178 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/deepchecks_llm_client/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/examples/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/openai_instrumentor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/deepchecks_llm_client/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/deepchecks_llm_client/sdk/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/sdk/langchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/deepchecks_llm_client/sdk/langchain/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/sdk/langchain/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/sdk/langchain/callbacks/deepchecks_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/deepchecks_llm_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-22 13:34:29.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-01-22 13:34:29.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 13:34:29.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-22 13:34:29.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-22 13:34:29.000000 deepchecks-llm-client-0.9.2/deepchecks_llm_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 13:34:29.298528 deepchecks-llm-client-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-22 13:34:23.000000 deepchecks-llm-client-0.9.2/setup.py
```

### Comparing `deepchecks-llm-client-0.9.1/deepchecks_llm_client/api.py` & `deepchecks-llm-client-0.9.2/deepchecks_llm_client/api.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.9.1/deepchecks_llm_client/client.py` & `deepchecks-llm-client-0.9.2/deepchecks_llm_client/client.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.9.1/deepchecks_llm_client/data_types.py` & `deepchecks-llm-client-0.9.2/deepchecks_llm_client/data_types.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.9.1/deepchecks_llm_client/examples/usage.py` & `deepchecks-llm-client-0.9.2/deepchecks_llm_client/examples/usage.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.9.1/deepchecks_llm_client/openai_instrumentor.py` & `deepchecks-llm-client-0.9.2/deepchecks_llm_client/openai_instrumentor.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.9.1/deepchecks_llm_client/sdk/langchain/callbacks/deepchecks_callback_handler.py` & `deepchecks-llm-client-0.9.2/deepchecks_llm_client/sdk/langchain/callbacks/deepchecks_callback_handler.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.9.1/deepchecks_llm_client/utils.py` & `deepchecks-llm-client-0.9.2/deepchecks_llm_client/utils.py`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.9.1/deepchecks_llm_client.egg-info/SOURCES.txt` & `deepchecks-llm-client-0.9.2/deepchecks_llm_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchecks-llm-client-0.9.1/pyproject.toml` & `deepchecks-llm-client-0.9.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 [project]
 description = "The SDK client for communicating with Deepchecks LLM service"
 name = 'deepchecks-llm-client'
 dynamic = ['version', 'dependencies']
 requires-python = ">=3.8"
 authors = [{ name = "deepchecks", email = "info@deepchecks.com" }]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
 
 [project.optional-dependencies]
 langchin = [
     "langchain>=0.0.313,<0.1",
 ]
 
 [tool.setuptools.packages.find]
```

