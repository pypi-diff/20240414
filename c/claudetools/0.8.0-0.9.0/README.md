# Comparing `tmp/claudetools-0.8.0.tar.gz` & `tmp/claudetools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudetools-0.8.0.tar", last modified: Fri Mar 29 12:08:16 2024, max compression
+gzip compressed data, was "claudetools-0.9.0.tar", last modified: Sun Apr 14 09:56:13 2024, max compression
```

## Comparing `claudetools-0.8.0.tar` & `claudetools-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:16.255427 claudetools-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-29 12:08:04.000000 claudetools-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-03-29 12:08:16.255427 claudetools-0.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:16.251427 claudetools-0.8.0/claudetools/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:16.251427 claudetools-0.8.0/claudetools/completion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/completion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/completion/async_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/completion/complete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:16.251427 claudetools-0.8.0/claudetools/extract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/extract/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/extract/single.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:16.251427 claudetools-0.8.0/claudetools/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/prompts/multi_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/prompts/single_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:16.255427 claudetools-0.8.0/claudetools/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8323 2024-03-29 12:08:04.000000 claudetools-0.8.0/claudetools/tools/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:16.251427 claudetools-0.8.0/claudetools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-03-29 12:08:16.000000 claudetools-0.8.0/claudetools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-29 12:08:16.000000 claudetools-0.8.0/claudetools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:08:16.000000 claudetools-0.8.0/claudetools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-29 12:08:16.000000 claudetools-0.8.0/claudetools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-29 12:08:16.000000 claudetools-0.8.0/claudetools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 12:08:16.255427 claudetools-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-29 12:08:04.000000 claudetools-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:16.255427 claudetools-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:08:04.000000 claudetools-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-29 12:08:04.000000 claudetools-0.8.0/tests/test_bedrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-29 12:08:04.000000 claudetools-0.8.0/tests/test_multiple_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-29 12:08:04.000000 claudetools-0.8.0/tests/test_single_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-29 12:08:04.000000 claudetools-0.8.0/tests/test_single_specific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:13.327939 claudetools-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 09:56:06.000000 claudetools-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-14 09:56:13.327939 claudetools-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:13.323939 claudetools-0.9.0/claudetools/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:13.323939 claudetools-0.9.0/claudetools/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/completion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/completion/async_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/completion/complete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:13.323939 claudetools-0.9.0/claudetools/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/extract/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/extract/single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:13.323939 claudetools-0.9.0/claudetools/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/prompts/multi_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/prompts/single_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:13.323939 claudetools-0.9.0/claudetools/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-04-14 09:56:06.000000 claudetools-0.9.0/claudetools/tools/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:13.323939 claudetools-0.9.0/claudetools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-14 09:56:13.000000 claudetools-0.9.0/claudetools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-14 09:56:13.000000 claudetools-0.9.0/claudetools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:56:13.000000 claudetools-0.9.0/claudetools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 09:56:13.000000 claudetools-0.9.0/claudetools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 09:56:13.000000 claudetools-0.9.0/claudetools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:56:13.327939 claudetools-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-14 09:56:06.000000 claudetools-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:13.327939 claudetools-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:06.000000 claudetools-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-14 09:56:06.000000 claudetools-0.9.0/tests/test_bedrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-14 09:56:06.000000 claudetools-0.9.0/tests/test_multiple_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-14 09:56:06.000000 claudetools-0.9.0/tests/test_single_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-14 09:56:06.000000 claudetools-0.9.0/tests/test_single_specific.py
```

### Comparing `claudetools-0.8.0/LICENSE` & `claudetools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/PKG-INFO` & `claudetools-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudetools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Claudetools is a Python library that enables function calling with the Claude 3 family of language models from Anthropic.
 Home-page: https://github.com/vatsalsaglani/claudetools
 Author: Vatsal J. Saglani
 Author-email: saglanivatsal@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `claudetools-0.8.0/claudetools/completion/async_complete.py` & `claudetools-0.9.0/claudetools/completion/async_complete.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/claudetools/completion/complete.py` & `claudetools-0.9.0/claudetools/completion/complete.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/claudetools/extract/multiple.py` & `claudetools-0.9.0/claudetools/extract/multiple.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/claudetools/extract/single.py` & `claudetools-0.9.0/claudetools/extract/single.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/claudetools/prompts/multi_functions.py` & `claudetools-0.9.0/claudetools/prompts/multi_functions.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/claudetools/prompts/single_function.py` & `claudetools-0.9.0/claudetools/prompts/single_function.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/claudetools/tools/tool.py` & `claudetools-0.9.0/claudetools/tools/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class ToolChoice(BaseModel):
     name: str
 
 
 class Message(BaseModel):
     role: Literal["user", "assistant"]
-    content: str
+    content: Union[str, List, List[Dict]]
 
 
 class Messages(BaseModel):
     messages: List[Message]
 
 
 class BaseTool(ABC):
```

### Comparing `claudetools-0.8.0/claudetools.egg-info/PKG-INFO` & `claudetools-0.9.0/claudetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudetools
-Version: 0.8.0
+Version: 0.9.0
 Summary: Claudetools is a Python library that enables function calling with the Claude 3 family of language models from Anthropic.
 Home-page: https://github.com/vatsalsaglani/claudetools
 Author: Vatsal J. Saglani
 Author-email: saglanivatsal@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `claudetools-0.8.0/claudetools.egg-info/SOURCES.txt` & `claudetools-0.9.0/claudetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/setup.py` & `claudetools-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="claudetools",
-    version="0.8.0",
+    version="0.9.0",
     author="Vatsal J. Saglani",
     author_email="saglanivatsal@gmail.com",
     description=
     "Claudetools is a Python library that enables function calling with the Claude 3 family of language models from Anthropic.",
     long_description=open("Readme.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/vatsalsaglani/claudetools",
```

### Comparing `claudetools-0.8.0/tests/test_bedrock.py` & `claudetools-0.9.0/tests/test_bedrock.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/tests/test_multiple_function.py` & `claudetools-0.9.0/tests/test_multiple_function.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/tests/test_single_function.py` & `claudetools-0.9.0/tests/test_single_function.py`

 * *Files identical despite different names*

### Comparing `claudetools-0.8.0/tests/test_single_specific.py` & `claudetools-0.9.0/tests/test_single_specific.py`

 * *Files identical despite different names*

