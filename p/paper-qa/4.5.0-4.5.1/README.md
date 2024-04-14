# Comparing `tmp/paper-qa-4.5.0.tar.gz` & `tmp/paper_qa-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-4.5.0.tar", last modified: Sat Mar 30 05:55:58 2024, max compression
+gzip compressed data, was "paper_qa-4.5.1.tar", last modified: Sun Apr 14 16:44:54 2024, max compression
```

## Comparing `paper-qa-4.5.0.tar` & `paper_qa-4.5.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:55:58.778332 paper-qa-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-30 05:53:47.000000 paper-qa-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    30432 2024-03-30 05:55:58.778332 paper-qa-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-03-30 05:53:47.000000 paper-qa-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:55:58.778332 paper-qa-4.5.0/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30432 2024-03-30 05:55:58.000000 paper-qa-4.5.0/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-30 05:55:58.000000 paper-qa-4.5.0/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 05:55:58.000000 paper-qa-4.5.0/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-30 05:55:58.000000 paper-qa-4.5.0/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-30 05:55:58.000000 paper-qa-4.5.0/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:55:58.778332 paper-qa-4.5.0/paperqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:55:58.778332 paper-qa-4.5.0/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)    32260 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31980 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/llms.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-30 05:53:47.000000 paper-qa-4.5.0/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-03-30 05:53:47.000000 paper-qa-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 05:55:58.778332 paper-qa-4.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 05:55:58.778332 paper-qa-4.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    62773 2024-03-30 05:53:47.000000 paper-qa-4.5.0/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.149600 paper_qa-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 16:42:43.000000 paper_qa-4.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-14 16:44:54.149600 paper_qa-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16388 2024-04-14 16:42:43.000000 paper_qa-4.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-14 16:42:43.000000 paper_qa-4.5.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.145600 paper_qa-4.5.1/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 16:44:54.000000 paper_qa-4.5.1/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.145600 paper_qa-4.5.1/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.145600 paper_qa-4.5.1/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32138 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31980 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/llms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-14 16:42:43.000000 paper_qa-4.5.1/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-14 16:42:43.000000 paper_qa-4.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:44:54.149600 paper_qa-4.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:44:54.145600 paper_qa-4.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    62211 2024-04-14 16:42:43.000000 paper_qa-4.5.1/tests/test_paperqa.py
```

### Comparing `paper-qa-4.5.0/LICENSE` & `paper_qa-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-4.5.0/PKG-INFO` & `paper_qa-4.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 4.5.0
+Version: 4.5.1
 Summary: LLM Chain for answering questions from docs
 Author-email: Andrew White <white.d.andrew@gmail.com>
 Maintainer-email: James Braza <jamesbraza@gmail.com>, Andrew White <white.d.andrew@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -223,14 +223,32 @@
 Requires-Dist: PyCryptodome
 Requires-Dist: html2text
 Requires-Dist: numpy
 Requires-Dist: openai>=1
 Requires-Dist: pydantic>=2
 Requires-Dist: pypdf
 Requires-Dist: tiktoken>=0.4.0
+Provides-Extra: dev
+Requires-Dist: anthropic; extra == "dev"
+Requires-Dist: faiss-cpu; extra == "dev"
+Requires-Dist: langchain-community; extra == "dev"
+Requires-Dist: langchain-openai; extra == "dev"
+Requires-Dist: pymupdf; extra == "dev"
+Requires-Dist: python-dotenv; extra == "dev"
+Requires-Dist: pyzotero; extra == "dev"
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: sentence_transformers; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: types-setuptools; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-sugar; extra == "dev"
+Requires-Dist: pytest-timer; extra == "dev"
 
 # PaperQA
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
```

### Comparing `paper-qa-4.5.0/README.md` & `paper_qa-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-4.5.0/paper_qa.egg-info/PKG-INFO` & `paper_qa-4.5.1/paper_qa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 4.5.0
+Version: 4.5.1
 Summary: LLM Chain for answering questions from docs
 Author-email: Andrew White <white.d.andrew@gmail.com>
 Maintainer-email: James Braza <jamesbraza@gmail.com>, Andrew White <white.d.andrew@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -223,14 +223,32 @@
 Requires-Dist: PyCryptodome
 Requires-Dist: html2text
 Requires-Dist: numpy
 Requires-Dist: openai>=1
 Requires-Dist: pydantic>=2
 Requires-Dist: pypdf
 Requires-Dist: tiktoken>=0.4.0
+Provides-Extra: dev
+Requires-Dist: anthropic; extra == "dev"
+Requires-Dist: faiss-cpu; extra == "dev"
+Requires-Dist: langchain-community; extra == "dev"
+Requires-Dist: langchain-openai; extra == "dev"
+Requires-Dist: pymupdf; extra == "dev"
+Requires-Dist: python-dotenv; extra == "dev"
+Requires-Dist: pyzotero; extra == "dev"
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: sentence_transformers; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: types-setuptools; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-sugar; extra == "dev"
+Requires-Dist: pytest-timer; extra == "dev"
 
 # PaperQA
 
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/whitead/paper-qa)
 [![tests](https://github.com/whitead/paper-qa/actions/workflows/tests.yml/badge.svg)](https://github.com/whitead/paper-qa)
 [![PyPI version](https://badge.fury.io/py/paper-qa.svg)](https://badge.fury.io/py/paper-qa)
```

### Comparing `paper-qa-4.5.0/paperqa/__init__.py` & `paper_qa-4.5.1/paperqa/__init__.py`

 * *Files identical despite different names*

### Comparing `paper-qa-4.5.0/paperqa/contrib/zotero.py` & `paper_qa-4.5.1/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-4.5.0/paperqa/docs.py` & `paper_qa-4.5.1/paperqa/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     PromptCollection,
     Text,
 )
 from .utils import (
     gather_with_concurrency,
     get_loop,
     guess_is_4xx,
+    llm_read_json,
     maybe_is_html,
     maybe_is_pdf,
     maybe_is_text,
     md5sum,
     name_in_text,
     strip_citations,
 )
@@ -653,17 +654,15 @@
                 except Exception as e:
                     if guess_is_4xx(str(e)):
                         return None, llm_result
                     raise
                 success = True
                 if self.prompts.summary_json:
                     try:
-                        # fetch from markdown ```json if present
-                        context = context.split("```json")[-1].split("```")[0]
-                        result_data = json.loads(context)
+                        result_data = llm_read_json(context)
                     except json.decoder.JSONDecodeError:
                         # fallback to string
                         success = False
                     else:
                         success = isinstance(result_data, dict)
                     if success:
                         try:
```

### Comparing `paper-qa-4.5.0/paperqa/llms.py` & `paper_qa-4.5.1/paperqa/llms.py`

 * *Files identical despite different names*

### Comparing `paper-qa-4.5.0/paperqa/prompts.py` & `paper_qa-4.5.1/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-4.5.0/paperqa/readers.py` & `paper_qa-4.5.1/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-4.5.0/paperqa/types.py` & `paper_qa-4.5.1/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-4.5.0/paperqa/utils.py` & `paper_qa-4.5.1/paperqa/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
+import json
 import math
 import re
 import string
 from pathlib import Path
 from typing import Any, BinaryIO, Coroutine, Iterator, Union
 
 import pypdf
@@ -175,7 +176,18 @@
 
 def is_coroutine_callable(obj):
     if inspect.isfunction(obj):
         return inspect.iscoroutinefunction(obj)
     elif callable(obj):  # noqa: RET505
         return inspect.iscoroutinefunction(obj.__call__)
     return False
+
+
+def llm_read_json(text: str) -> dict:
+    """Read LLM output and extract JSON data from it."""
+    # fetch from markdown ```json if present
+    text = text.strip().split("```json")[-1].split("```")[0]
+    # split anything before the first {
+    text = "{" + text.split("{", 1)[-1]
+    # split anything after the last }
+    text = text.rsplit("}", 1)[0] + "}"
+    return json.loads(text)
```

### Comparing `paper-qa-4.5.0/pyproject.toml` & `paper_qa-4.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools >= 61.0"]
+# Pin to 62.6 for support from reading requirements from requirements.txt
+requires = ["setuptools >= 62.6.0"]
 
 [project]
 authors = [
     {email = "white.d.andrew@gmail.com", name = "Andrew White"},
 ]
 # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
 classifiers = [
@@ -24,25 +25,26 @@
     "numpy",
     "openai>=1",
     "pydantic>=2",
     "pypdf",
     "tiktoken>=0.4.0",
 ]
 description = "LLM Chain for answering questions from docs"
+dynamic = ["optional-dependencies"]
 keywords = ["question answering"]
 license = {file = "LICENSE"}
 maintainers = [
     {email = "jamesbraza@gmail.com", name = "James Braza"},
     {email = "white.d.andrew@gmail.com", name = "Andrew White"},
 ]
 name = "paper-qa"
 readme = "README.md"
 requires-python = ">=3.8"
 urls = {repository = "https://github.com/whitead/paper-qa"}
-version = "4.5.0"
+version = "4.5.1"
 
 [tool.codespell]
 check-filenames = true
 check-hidden = true
 # SEE: https://github.com/codespell-project/codespell/issues/1212#issuecomment-1744768533
 ignore-regex = ".{1024}|.*codespell-ignore.*"
 ignore-words-list = "aadd,ser"
@@ -179,14 +181,17 @@
 max-doc-length = 120  # Match line-length
 
 [tool.ruff.lint.pydocstyle]
 # Whether to use Google-style or NumPy-style conventions or the PEP257
 # defaults when analyzing docstring sections.
 convention = "google"
 
+[tool.setuptools.dynamic.optional-dependencies.dev]
+file = ["dev-requirements.txt"]
+
 [tool.setuptools.packages.find]
 include = ["paperqa*"]
 
 [tool.tomlsort]
 all = true
 in_place = true
 spaces_before_inline_comment = 2  # Match Python PEP 8
```

### Comparing `paper-qa-4.5.0/tests/test_paperqa.py` & `paper_qa-4.5.1/tests/test_paperqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import os
 import pickle
 import tempfile
 from io import BytesIO
 from pathlib import Path
-from unittest import IsolatedAsyncioTestCase
 
 import numpy as np
 import pytest
 import requests
 from openai import AsyncOpenAI
 
 from paperqa import (
@@ -35,14 +34,15 @@
     get_score,
     guess_model_type,
     is_openai_model,
 )
 from paperqa.readers import read_doc
 from paperqa.utils import (
     get_citenames,
+    llm_read_json,
     maybe_is_html,
     maybe_is_text,
     name_in_text,
     strings_similarity,
     strip_citations,
 )
 
@@ -405,109 +405,145 @@
         "colors had different refrangibility. \n"
         "Relevance Score: 9.5"
     )
 
     assert get_score(sample) == 9
 
 
-class TestChains(IsolatedAsyncioTestCase):
-    async def test_chain_completion(self):
-        client = AsyncOpenAI()
-        llm = OpenAILLMModel(config={"model": "babbage-002", "temperature": 0.2})
-        call = llm.make_chain(
-            client,
-            "The {animal} says",
-            skip_system=True,
-        )
-        outputs = []
-
-        def accum(x):
-            outputs.append(x)
-
-        completion = await call({"animal": "duck"}, callbacks=[accum])  # type: ignore[call-arg]
-        assert completion.seconds_to_first_token > 0
-        assert completion.prompt_count > 0
-        assert completion.completion_count > 0
-        assert str(completion) == "".join(outputs)
-
-        completion = await call({"animal": "duck"})  # type: ignore[call-arg]
-        assert completion.seconds_to_first_token == 0
-        assert completion.seconds_to_last_token > 0
-
-    async def test_chain_chat(self):
-        client = AsyncOpenAI()
-        llm = OpenAILLMModel(
-            config={"temperature": 0, "model": "gpt-3.5-turbo", "max_tokens": 56}
-        )
-        call = llm.make_chain(
-            client,
-            "The {animal} says",
-            skip_system=True,
-        )
-        outputs = []
-
-        def accum(x):
-            outputs.append(x)
-
-        completion = await call({"animal": "duck"}, callbacks=[accum])  # type: ignore[call-arg]
-        assert completion.seconds_to_first_token > 0
-        assert completion.prompt_count > 0
-        assert completion.completion_count > 0
-        assert str(completion) == "".join(outputs)
-
-        completion = await call({"animal": "duck"})  # type: ignore[call-arg]
-        assert completion.seconds_to_first_token == 0
-        assert completion.seconds_to_last_token > 0
-
-        # check with mixed callbacks
-        async def ac(x):  # noqa: ARG001
-            pass
-
-        completion = await call({"animal": "duck"}, callbacks=[accum, ac])  # type: ignore[call-arg]
-
-    async def test_anthropic_chain(self):
-        try:
-            from anthropic import AsyncAnthropic
-        except ImportError:
-            return
-
-        client = AsyncAnthropic()
-        llm = AnthropicLLMModel()
-        call = llm.make_chain(
-            client,
-            "The {animal} says",
-            skip_system=True,
-        )
-
-        def accum(x):
-            outputs.append(x)
-
-        outputs: list[str] = []
-        completion = await call({"animal": "duck"}, callbacks=[accum])  # type: ignore[call-arg]
-        assert completion.seconds_to_first_token > 0
-        assert completion.prompt_count > 0
-        assert completion.completion_count > 0
-        assert str(completion) == "".join(outputs)
-        assert type(completion.text) is str  # noqa: E721
-
-        completion = await call({"animal": "duck"})  # type: ignore[call-arg]
-        assert completion.seconds_to_first_token == 0
-        assert completion.seconds_to_last_token > 0
-        assert type(completion.text) is str  # noqa: E721
-
-        docs = Docs(llm="claude-3-sonnet-20240229", client=client)
-        await docs.aadd_url(
-            "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
-            citation="WikiMedia Foundation, 2023, Accessed now",
-            dockey="test",
-        )
-        answer = await docs.aget_evidence(
-            Answer(question="What is the national flag of Canada?")
-        )
-        await docs.aquery("What is the national flag of Canada?", answer=answer)
+@pytest.mark.parametrize(
+    "example",
+    [
+        """Sure here is the json you asked for!
+
+    {
+    "example": "json"
+    }
+
+    Did you like it?""",
+        '{"example": "json"}',
+        """
+```json
+{
+    "example": "json"
+}
+```
+
+I have written the json you asked for.""",
+        """
+
+{
+    "example": "json"
+}
+
+""",
+    ],
+)
+def test_llm_read_json(example: str):
+    assert llm_read_json(example) == {"example": "json"}
+
+
+@pytest.mark.asyncio()
+async def test_chain_completion():
+    client = AsyncOpenAI()
+    llm = OpenAILLMModel(config={"model": "babbage-002", "temperature": 0.2})
+    call = llm.make_chain(
+        client,
+        "The {animal} says",
+        skip_system=True,
+    )
+    outputs = []
+
+    def accum(x):
+        outputs.append(x)
+
+    completion = await call({"animal": "duck"}, callbacks=[accum])  # type: ignore[call-arg]
+    assert completion.seconds_to_first_token > 0
+    assert completion.prompt_count > 0
+    assert completion.completion_count > 0
+    assert str(completion) == "".join(outputs)
+
+    completion = await call({"animal": "duck"})  # type: ignore[call-arg]
+    assert completion.seconds_to_first_token == 0
+    assert completion.seconds_to_last_token > 0
+
+
+@pytest.mark.asyncio()
+async def test_chain_chat():
+    client = AsyncOpenAI()
+    llm = OpenAILLMModel(
+        config={"temperature": 0, "model": "gpt-3.5-turbo", "max_tokens": 56}
+    )
+    call = llm.make_chain(
+        client,
+        "The {animal} says",
+        skip_system=True,
+    )
+    outputs = []
+
+    def accum(x):
+        outputs.append(x)
+
+    completion = await call({"animal": "duck"}, callbacks=[accum])  # type: ignore[call-arg]
+    assert completion.seconds_to_first_token > 0
+    assert completion.prompt_count > 0
+    assert completion.completion_count > 0
+    assert str(completion) == "".join(outputs)
+
+    completion = await call({"animal": "duck"})  # type: ignore[call-arg]
+    assert completion.seconds_to_first_token == 0
+    assert completion.seconds_to_last_token > 0
+
+    # check with mixed callbacks
+    async def ac(x):  # noqa: ARG001
+        pass
+
+    completion = await call({"animal": "duck"}, callbacks=[accum, ac])  # type: ignore[call-arg]
+
+
+@pytest.mark.asyncio()
+async def test_anthropic_chain():
+    try:
+        from anthropic import AsyncAnthropic
+    except ImportError:
+        return
+
+    client = AsyncAnthropic()
+    llm = AnthropicLLMModel()
+    call = llm.make_chain(
+        client,
+        "The {animal} says",
+        skip_system=True,
+    )
+
+    def accum(x):
+        outputs.append(x)
+
+    outputs: list[str] = []
+    completion = await call({"animal": "duck"}, callbacks=[accum])  # type: ignore[call-arg]
+    assert completion.seconds_to_first_token > 0
+    assert completion.prompt_count > 0
+    assert completion.completion_count > 0
+    assert str(completion) == "".join(outputs)
+    assert isinstance(completion.text, str)
+
+    completion = await call({"animal": "duck"})  # type: ignore[call-arg]
+    assert completion.seconds_to_first_token == 0
+    assert completion.seconds_to_last_token > 0
+    assert isinstance(completion.text, str)
+
+    docs = Docs(llm="claude-3-sonnet-20240229", client=client)
+    await docs.aadd_url(
+        "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    answer = await docs.aget_evidence(
+        Answer(question="What is the national flag of Canada?")
+    )
+    await docs.aquery("What is the national flag of Canada?", answer=answer)
 
 
 def test_docs():
     docs = Docs(llm="babbage-002")
     docs.add_url(
         "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
         citation="WikiMedia Foundation, 2023, Accessed now",
@@ -766,15 +802,15 @@
             SparseEmbeddingModel(),
         ]
     )
     docs = Docs(
         docs_index=NumpyVectorStore(embedding_model=model),
         texts_index=NumpyVectorStore(embedding_model=model),
     )
-    assert type(docs._embedding_client) is AsyncOpenAI
+    assert isinstance(docs._embedding_client, AsyncOpenAI)
     assert docs.embedding.startswith("hybrid")  # type: ignore[union-attr]
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
     assert any(docs.docs["test"].embedding)  # type: ignore[arg-type]
@@ -782,15 +818,15 @@
     # check the embeddings are the same size
     assert np.shape(docs.texts[0].embedding) == np.shape(docs.texts[1].embedding)
 
     # now try via alias
     docs = Docs(
         embedding="hybrid-text-embedding-3-small",
     )
-    assert type(docs._embedding_client) is AsyncOpenAI
+    assert isinstance(docs._embedding_client, AsyncOpenAI)
     assert docs.embedding.startswith("hybrid")  # type: ignore[union-attr]
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
     assert any(docs.docs["test"].embedding)  # type: ignore[arg-type]
@@ -863,25 +899,25 @@
     assert "Echo" in evidence.context
 
 
 def test_langchain_llm():
     from langchain_openai import ChatOpenAI, OpenAI
 
     docs = Docs(llm="langchain", client=ChatOpenAI(model="gpt-3.5-turbo"))
-    assert type(docs.llm_model) == LangchainLLMModel
-    assert type(docs.summary_llm_model) == LangchainLLMModel
+    assert isinstance(docs.llm_model, LangchainLLMModel)
+    assert isinstance(docs.summary_llm_model, LangchainLLMModel)
     assert docs.llm == "gpt-3.5-turbo"
     assert docs.summary_llm == "gpt-3.5-turbo"
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
     assert docs._client is not None
-    assert type(docs.llm_model) == LangchainLLMModel
+    assert isinstance(docs.llm_model, LangchainLLMModel)
     assert docs.summary_llm_model == docs.llm_model
 
     docs.get_evidence(
         Answer(question="What is Frederick Bates's greatest accomplishment?"),
         get_callbacks=lambda x: [lambda y: print(y, end="")],  # noqa: ARG005
     )
 
@@ -944,134 +980,122 @@
     docs.add_url(
         "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
 
 
-class TestVectorStore(IsolatedAsyncioTestCase):
-    async def test_langchain_vector_store(self):
-        from langchain_community.vectorstores.faiss import FAISS
-        from langchain_openai import OpenAIEmbeddings
-
-        some_texts = [
-            Text(
-                embedding=OpenAIEmbeddings().embed_query("test"),
-                text="this is a test",
-                name="test",
-                doc=Doc(docname="test", citation="test", dockey="test"),
-            )
-        ]
+@pytest.mark.asyncio()
+async def test_langchain_vector_store():
+    from langchain_community.vectorstores.faiss import FAISS
+    from langchain_openai import OpenAIEmbeddings
 
-        # checks on builder
-        try:
-            index = LangchainVectorStore()
-            index.add_texts_and_embeddings(some_texts)
-            raise "Failed to check for builder"  # type: ignore[misc]  # noqa: B016
-        except ValueError:
-            pass
-
-        try:
-            index = LangchainVectorStore(store_builder=lambda x: None)  # noqa: ARG005
-            raise "Failed to count arguments"  # type: ignore[misc]  # noqa: B016
-        except ValueError:
-            pass
-
-        try:
-            index = LangchainVectorStore(store_builder="foo")
-            raise "Failed to check if builder is callable"  # type: ignore[misc]  # noqa: B016
-        except ValueError:
-            pass
-
-        # now with real builder
-        index = LangchainVectorStore(
-            store_builder=lambda x, y: FAISS.from_embeddings(x, OpenAIEmbeddings(), y)
+    some_texts = [
+        Text(
+            embedding=OpenAIEmbeddings().embed_query("test"),
+            text="this is a test",
+            name="test",
+            doc=Doc(docname="test", citation="test", dockey="test"),
         )
-        assert index._store is None
-        index.add_texts_and_embeddings(some_texts)
-        assert index._store is not None
-        # check search returns Text obj
-        data, score = await index.similarity_search(None, "test", k=1)  # type: ignore[unreachable]
-        print(data)
-        assert type(data[0]) == Text
-
-        # now try with convenience
-        index = LangchainVectorStore(cls=FAISS, embedding_model=OpenAIEmbeddings())
-        assert index._store is None
+    ]
+
+    index = LangchainVectorStore()
+    with pytest.raises(ValueError, match="You must set store_builder"):
         index.add_texts_and_embeddings(some_texts)
-        assert index._store is not None
 
-        docs = Docs(
-            texts_index=LangchainVectorStore(
-                cls=FAISS, embedding_model=OpenAIEmbeddings()
-            )
-        )
-        assert docs._embedding_client is not None  # from docs_index default
+    with pytest.raises(ValueError, match="store_builder must take two arguments"):
+        index = LangchainVectorStore(store_builder=lambda x: None)  # noqa: ARG005
 
-        await docs.aadd_url(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
-            citation="WikiMedia Foundation, 2023, Accessed now",
-            dockey="test",
-        )
-        # should be embedded
+    with pytest.raises(ValueError, match="store_builder must be callable"):
+        index = LangchainVectorStore(store_builder="foo")
 
-        # now try with JIT
-        docs = Docs(texts_index=index, jit_texts_index=True)
-        await docs.aadd_url(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
-            citation="WikiMedia Foundation, 2023, Accessed now",
-            dockey="test",
-        )
-        # should get cleared and rebuilt here
-        ev = await docs.aget_evidence(
-            answer=Answer(question="What is Frederick Bates's greatest accomplishment?")
-        )
-        assert len(ev.context) > 0
-        # now with dockkey filter
-        await docs.aget_evidence(
-            answer=Answer(
-                question="What is Frederick Bates's greatest accomplishment?",
-                dockey_filter=["test"],
-            )
+    # now with real builder
+    index = LangchainVectorStore(
+        store_builder=lambda x, y: FAISS.from_embeddings(x, OpenAIEmbeddings(), y)
+    )
+    assert index._store is None
+    index.add_texts_and_embeddings(some_texts)
+    assert index._store is not None
+    # check search returns Text obj
+    data, score = await index.similarity_search(None, "test", k=1)  # type: ignore[unreachable]
+    print(data)
+    assert isinstance(data[0], Text)
+
+    # now try with convenience
+    index = LangchainVectorStore(cls=FAISS, embedding_model=OpenAIEmbeddings())
+    assert index._store is None
+    index.add_texts_and_embeddings(some_texts)
+    assert index._store is not None
+
+    docs = Docs(
+        texts_index=LangchainVectorStore(cls=FAISS, embedding_model=OpenAIEmbeddings())
+    )
+    assert docs._embedding_client is not None  # from docs_index default
+
+    await docs.aadd_url(
+        "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    # should be embedded
+
+    # now try with JIT
+    docs = Docs(texts_index=index, jit_texts_index=True)
+    await docs.aadd_url(
+        "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    # should get cleared and rebuilt here
+    ev = await docs.aget_evidence(
+        answer=Answer(question="What is Frederick Bates's greatest accomplishment?")
+    )
+    assert len(ev.context) > 0
+    # now with dockkey filter
+    await docs.aget_evidence(
+        answer=Answer(
+            question="What is Frederick Bates's greatest accomplishment?",
+            dockey_filter=["test"],
         )
+    )
 
-        # make sure we can pickle it
-        docs_pickle = pickle.dumps(docs)
-        pickle.loads(docs_pickle)  # noqa: S301
+    # make sure we can pickle it
+    docs_pickle = pickle.dumps(docs)
+    pickle.loads(docs_pickle)  # noqa: S301
 
-        # will not work at this point - have to reset index
+    # will not work at this point - have to reset index
 
 
-class Test(IsolatedAsyncioTestCase):
-    async def test_aquery(self):
-        docs = Docs()
-        await docs.aadd_url(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
-            citation="WikiMedia Foundation, 2023, Accessed now",
-            dockey="test",
-        )
-        await docs.aquery("What is Frederick Bates's greatest accomplishment?")
+@pytest.mark.asyncio()
+async def test_aquery():
+    docs = Docs()
+    await docs.aadd_url(
+        "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    await docs.aquery("What is Frederick Bates's greatest accomplishment?")
 
 
-class TestDocMatch(IsolatedAsyncioTestCase):
-    async def test_adoc_match(self):
-        docs = Docs()
-        await docs.aadd_url(
-            "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
-            citation="WikiMedia Foundation, 2023, Accessed now",
-            dockey="test",
-        )
-        sources = await docs.adoc_match(
-            "What is Frederick Bates's greatest accomplishment?"
-        )
-        assert len(sources) > 0
-        sources = await docs.adoc_match(
-            "What is Frederick Bates's greatest accomplishment?"
-        )
-        assert len(sources) > 0
+@pytest.mark.asyncio()
+async def test_adoc_match():
+    docs = Docs()
+    await docs.aadd_url(
+        "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+        citation="WikiMedia Foundation, 2023, Accessed now",
+        dockey="test",
+    )
+    sources = await docs.adoc_match(
+        "What is Frederick Bates's greatest accomplishment?"
+    )
+    assert len(sources) > 0
+    sources = await docs.adoc_match(
+        "What is Frederick Bates's greatest accomplishment?"
+    )
+    assert len(sources) > 0
 
 
 def test_docs_pickle() -> None:
     # 1. Fill out docs
     with tempfile.NamedTemporaryFile(mode="r+", encoding="utf-8", suffix=".html") as f:
         # get front page of wikipedia
         r = requests.get(  # noqa: S113
@@ -1636,25 +1660,25 @@
 def test_embedding_name_consistency():
     docs = Docs()
     assert docs.embedding == "text-embedding-ada-002"
     assert docs.texts_index.embedding_model.name == "text-embedding-ada-002"
     docs = Docs(embedding="langchain")
     assert docs.embedding == "langchain"
     assert docs.texts_index.embedding_model.name == "langchain"
-    assert type(docs.texts_index.embedding_model) == LangchainEmbeddingModel
+    assert isinstance(docs.texts_index.embedding_model, LangchainEmbeddingModel)
     docs = Docs(embedding="foo")
     assert docs.embedding == "foo"
-    assert type(docs.texts_index.embedding_model) == OpenAIEmbeddingModel
+    assert isinstance(docs.texts_index.embedding_model, OpenAIEmbeddingModel)
     docs = Docs(
         texts_index=NumpyVectorStore(embedding_model=OpenAIEmbeddingModel(name="test"))
     )
     assert docs.embedding == "test"
 
     docs = Docs(embedding="hybrid-text-embedding-ada-002")
-    assert type(docs.docs_index.embedding_model) is HybridEmbeddingModel
+    assert isinstance(docs.docs_index.embedding_model, HybridEmbeddingModel)
     assert docs.docs_index.embedding_model.models[0].name == "text-embedding-ada-002"
     assert docs.docs_index.embedding_model.models[1].name == "sparse"
 
 
 def test_external_texts_index():
     docs = Docs(jit_texts_index=True)
     docs.add_url(
```

