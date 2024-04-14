# Comparing `tmp/databonsai-0.2.0.tar.gz` & `tmp/databonsai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databonsai-0.2.0.tar", last modified: Sun Apr  7 21:02:29 2024, max compression
+gzip compressed data, was "databonsai-0.3.0.tar", last modified: Sun Apr 14 21:12:52 2024, max compression
```

## Comparing `databonsai-0.2.0.tar` & `databonsai-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:02:29.861397 databonsai-0.2.0/
--rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     7912 2024-04-07 21:02:29.861397 databonsai-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7082 2024-04-07 21:01:18.000000 databonsai-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 21:02:29.840039 databonsai-0.2.0/databonsai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.2.0/databonsai/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:02:29.860024 databonsai-0.2.0/databonsai/categorize/
--rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.2.0/databonsai/categorize/__init__.py
--rw-rw-rw-   0        0        0     2614 2024-04-06 20:49:12.000000 databonsai-0.2.0/databonsai/categorize/base_categorizer.py
--rw-rw-rw-   0        0        0     1932 2024-04-06 20:53:51.000000 databonsai-0.2.0/databonsai/categorize/multi_categorizer.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:02:29.861397 databonsai-0.2.0/databonsai/llm_providers/
--rw-rw-rw-   0        0        0      471 2024-04-07 00:16:34.000000 databonsai-0.2.0/databonsai/llm_providers/__init__.py
--rw-rw-rw-   0        0        0     3927 2024-04-07 20:20:07.000000 databonsai-0.2.0/databonsai/llm_providers/anthropic_provider.py
--rw-rw-rw-   0        0        0     2047 2024-04-07 20:19:59.000000 databonsai-0.2.0/databonsai/llm_providers/llm_provider.py
--rw-rw-rw-   0        0        0     4048 2024-04-07 20:20:11.000000 databonsai-0.2.0/databonsai/llm_providers/openai_provider.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:02:29.861397 databonsai-0.2.0/databonsai/transform/
--rw-rw-rw-   0        0        0      104 2024-04-07 00:17:44.000000 databonsai-0.2.0/databonsai/transform/__init__.py
--rw-rw-rw-   0        0        0     1740 2024-04-06 20:56:39.000000 databonsai-0.2.0/databonsai/transform/base_transformer.py
--rw-rw-rw-   0        0        0     3187 2024-04-07 18:56:25.000000 databonsai-0.2.0/databonsai/transform/decompose_transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:02:29.861397 databonsai-0.2.0/databonsai/utils/
--rw-rw-rw-   0        0        0        0 2024-04-07 00:48:35.000000 databonsai-0.2.0/databonsai/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:02:29.861397 databonsai-0.2.0/databonsai.egg-info/
--rw-rw-rw-   0        0        0     7912 2024-04-07 21:02:29.000000 databonsai-0.2.0/databonsai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-07 21:02:29.000000 databonsai-0.2.0/databonsai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:02:29.000000 databonsai-0.2.0/databonsai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-07 21:02:29.000000 databonsai-0.2.0/databonsai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 21:02:29.000000 databonsai-0.2.0/databonsai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      561 2024-04-07 21:01:48.000000 databonsai-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 21:02:29.861397 databonsai-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1013 2024-04-07 21:02:04.000000 databonsai-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.664238 databonsai-0.3.0/
+-rw-rw-rw-   0        0        0     1093 2024-04-05 20:10:20.000000 databonsai-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     6270 2024-04-14 21:12:52.663235 databonsai-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5414 2024-04-14 19:45:20.000000 databonsai-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.638498 databonsai-0.3.0/databonsai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:11:02.000000 databonsai-0.3.0/databonsai/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.650999 databonsai-0.3.0/databonsai/categorize/
+-rw-rw-rw-   0        0        0       96 2024-04-07 00:17:28.000000 databonsai-0.3.0/databonsai/categorize/__init__.py
+-rw-rw-rw-   0        0        0     4919 2024-04-14 21:07:08.000000 databonsai-0.3.0/databonsai/categorize/base_categorizer.py
+-rw-rw-rw-   0        0        0     3961 2024-04-14 21:07:14.000000 databonsai-0.3.0/databonsai/categorize/multi_categorizer.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.655005 databonsai-0.3.0/databonsai/llm_providers/
+-rw-rw-rw-   0        0        0      471 2024-04-07 00:16:34.000000 databonsai-0.3.0/databonsai/llm_providers/__init__.py
+-rw-rw-rw-   0        0        0     3927 2024-04-07 20:20:07.000000 databonsai-0.3.0/databonsai/llm_providers/anthropic_provider.py
+-rw-rw-rw-   0        0        0     2047 2024-04-07 20:19:59.000000 databonsai-0.3.0/databonsai/llm_providers/llm_provider.py
+-rw-rw-rw-   0        0        0     5525 2024-04-14 20:33:50.000000 databonsai-0.3.0/databonsai/llm_providers/openai_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.657705 databonsai-0.3.0/databonsai/transform/
+-rw-rw-rw-   0        0        0      104 2024-04-07 00:17:44.000000 databonsai-0.3.0/databonsai/transform/__init__.py
+-rw-rw-rw-   0        0        0     3453 2024-04-14 20:41:57.000000 databonsai-0.3.0/databonsai/transform/base_transformer.py
+-rw-rw-rw-   0        0        0     3182 2024-04-14 21:02:23.000000 databonsai-0.3.0/databonsai/transform/decompose_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.659224 databonsai-0.3.0/databonsai/utils/
+-rw-rw-rw-   0        0        0       59 2024-04-13 21:14:08.000000 databonsai-0.3.0/databonsai/utils/__init__.py
+-rw-rw-rw-   0        0        0     5583 2024-04-14 20:38:55.000000 databonsai-0.3.0/databonsai/utils/apply.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.662236 databonsai-0.3.0/databonsai.egg-info/
+-rw-rw-rw-   0        0        0     6270 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-14 21:12:52.000000 databonsai-0.3.0/databonsai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      561 2024-04-14 21:12:37.000000 databonsai-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 21:12:52.664238 databonsai-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-04-14 21:12:38.000000 databonsai-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 21:12:52.661235 databonsai-0.3.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-14 19:59:02.000000 databonsai-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4855 2024-04-14 21:01:40.000000 databonsai-0.3.0/tests/test_categorization.py
```

### Comparing `databonsai-0.2.0/LICENSE` & `databonsai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databonsai-0.2.0/databonsai/llm_providers/anthropic_provider.py` & `databonsai-0.3.0/databonsai/llm_providers/anthropic_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.2.0/databonsai/llm_providers/llm_provider.py` & `databonsai-0.3.0/databonsai/llm_providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `databonsai-0.2.0/databonsai/transform/decompose_transformer.py` & `databonsai-0.3.0/databonsai/transform/decompose_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, List
-from pydantic import validator
+from pydantic import field_validator
 from databonsai.transform.base_transformer import BaseTransformer
 
 
 class DecomposeTransformer(BaseTransformer):
     """
     This class extends the BaseTransformer class and overrides the transform method to
     decompose the input data into a list of dictionaries based on a provided output schema.
@@ -15,15 +15,15 @@
         ValueError: If the output schema dictionary is empty, or if the transformed data
                     does not match the expected format or schema.
 
     """
 
     output_schema: Dict[str, str]
 
-    @validator("output_schema")
+    @field_validator("output_schema")
     def validate_schema(cls, v):
         """
         Validates the output schema.
 
         Args:
             v (Dict[str, str]): The output schema to be validated.
 
@@ -39,16 +39,15 @@
 
     def transform(self, input_data: str, max_tokens=1000) -> List[Dict[str, str]]:
         """
         Transforms the input data into a list of dictionaries using the specified LLM provider.
 
         Args:
             input_data (str): The text data to be transformed.
-            max_tokens (int, optional): The maximum number of tokens to generate in the response.
-                Defaults to 1000.
+            max_tokens (int, optional): The maximum number of tokens to generate in the response. Defaults to 1000.
 
         Returns:
             List[Dict[str, str]]: The transformed data as a list of dictionaries.
 
         Raises:
             ValueError: If the transformed data does not match the expected format or schema.
         """
```

### Comparing `databonsai-0.2.0/databonsai.egg-info/SOURCES.txt` & `databonsai-0.3.0/databonsai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,8 +14,11 @@
 databonsai/llm_providers/__init__.py
 databonsai/llm_providers/anthropic_provider.py
 databonsai/llm_providers/llm_provider.py
 databonsai/llm_providers/openai_provider.py
 databonsai/transform/__init__.py
 databonsai/transform/base_transformer.py
 databonsai/transform/decompose_transformer.py
-databonsai/utils/__init__.py
+databonsai/utils/__init__.py
+databonsai/utils/apply.py
+tests/__init__.py
+tests/test_categorization.py
```

### Comparing `databonsai-0.2.0/pyproject.toml` & `databonsai-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databonsai"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python package to clean and curate your data with LLMs"
 authors = ["Alvin Ryanputra <databonsai.ai@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"  
 
 openai = "^1.16.2"
```

### Comparing `databonsai-0.2.0/setup.py` & `databonsai-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name="databonsai",
-    version="0.2.0",
+    version="0.3.0",
     description="A package for cleaning and curating data with LLMs",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Alvin Ryanputra",
     author_email="databonsai.ai@gmail.com",
     url="https://github.com/databonsai/databonsai",
     packages=find_packages(),
     install_requires=[
         "openai",
         "anthropic",
         "tenacity",
         "python-dotenv",
         "pydantic",
+        "anthropic",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

