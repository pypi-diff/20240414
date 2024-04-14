# Comparing `tmp/phospho-0.3.8.tar.gz` & `tmp/phospho-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phospho-0.3.8.tar", max compression
+gzip compressed data, was "phospho-0.3.9.tar", max compression
```

## Comparing `phospho-0.3.8.tar` & `phospho-0.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11340 2024-03-13 01:38:38.506967 phospho-0.3.8/LICENCE
--rw-r--r--   0        0        0     2049 2024-03-13 01:38:38.506967 phospho-0.3.8/README.md
--rw-r--r--   0        0        0    35075 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/__init__.py
--rw-r--r--   0        0        0       79 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/_version.py
--rw-r--r--   0        0        0     6885 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/client.py
--rw-r--r--   0        0        0      234 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/collection.py
--rw-r--r--   0        0        0      248 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/config.py
--rw-r--r--   0        0        0     3207 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/consumer.py
--rw-r--r--   0        0        0    11831 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/extractor.py
--rw-r--r--   0        0        0     3825 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/integrations.py
--rw-r--r--   0        0        0      176 2024-03-13 01:38:38.506967 phospho-0.3.8/phospho/lab/__init__.py
--rw-r--r--   0        0        0    19419 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/lab/job_library.py
--rw-r--r--   0        0        0    15227 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/lab/lab.py
--rw-r--r--   0        0        0     1469 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/lab/language_models.py
--rw-r--r--   0        0        0     5144 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/lab/models.py
--rw-r--r--   0        0        0     3487 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/lab/utils.py
--rw-r--r--   0        0        0     2183 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/log_queue.py
--rw-r--r--   0        0        0     2719 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/models.py
--rw-r--r--   0        0        0        0 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/py.typed
--rw-r--r--   0        0        0     3346 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/sessions.py
--rw-r--r--   0        0        0     3169 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/steps.py
--rw-r--r--   0        0        0     3819 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/tasks.py
--rw-r--r--   0        0        0    21528 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/testing.py
--rw-r--r--   0        0        0     4261 2024-03-13 01:38:38.510967 phospho-0.3.8/phospho/utils.py
--rw-r--r--   0        0        0     1302 2024-03-13 01:38:38.510967 phospho-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 phospho-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11340 2024-03-14 03:36:19.894061 phospho-0.3.9/LICENCE
+-rw-r--r--   0        0        0     2049 2024-03-14 03:36:19.894061 phospho-0.3.9/README.md
+-rw-r--r--   0        0        0    35075 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/__init__.py
+-rw-r--r--   0        0        0       79 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/_version.py
+-rw-r--r--   0        0        0     6885 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/client.py
+-rw-r--r--   0        0        0      234 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/collection.py
+-rw-r--r--   0        0        0      408 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/config.py
+-rw-r--r--   0        0        0     3207 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/consumer.py
+-rw-r--r--   0        0        0    11831 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/extractor.py
+-rw-r--r--   0        0        0     3825 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/integrations.py
+-rw-r--r--   0        0        0      176 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/lab/__init__.py
+-rw-r--r--   0        0        0    19896 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/lab/job_library.py
+-rw-r--r--   0        0        0    15227 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/lab/lab.py
+-rw-r--r--   0        0        0     1809 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/lab/language_models.py
+-rw-r--r--   0        0        0     5144 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/lab/models.py
+-rw-r--r--   0        0        0     3487 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/lab/utils.py
+-rw-r--r--   0        0        0     2183 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/log_queue.py
+-rw-r--r--   0        0        0     2719 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/models.py
+-rw-r--r--   0        0        0        0 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/py.typed
+-rw-r--r--   0        0        0     3346 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/sessions.py
+-rw-r--r--   0        0        0     3169 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/steps.py
+-rw-r--r--   0        0        0     3819 2024-03-14 03:36:19.894061 phospho-0.3.9/phospho/tasks.py
+-rw-r--r--   0        0        0    21528 2024-03-14 03:36:19.898061 phospho-0.3.9/phospho/testing.py
+-rw-r--r--   0        0        0     4261 2024-03-14 03:36:19.898061 phospho-0.3.9/phospho/utils.py
+-rw-r--r--   0        0        0     1305 2024-03-14 03:36:19.898061 phospho-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 phospho-0.3.9/PKG-INFO
```

### Comparing `phospho-0.3.8/LICENCE` & `phospho-0.3.9/LICENCE`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/README.md` & `phospho-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/__init__.py` & `phospho-0.3.9/phospho/__init__.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/client.py` & `phospho-0.3.9/phospho/client.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/consumer.py` & `phospho-0.3.9/phospho/consumer.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/extractor.py` & `phospho-0.3.9/phospho/extractor.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/integrations.py` & `phospho-0.3.9/phospho/integrations.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/lab/job_library.py` & `phospho-0.3.9/phospho/lab/job_library.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 """
 Collection of jobs for the laboratory.
 Each job is a function that takes a message and a set of parameters and returns a result.
 The result is a JobResult object.
 """
 
+import os
 import logging
 import random
 import time
 from typing import List, Literal, Optional, cast
 
+import phospho.config as config
+
+try:
+    from openai import AsyncOpenAI, OpenAI
+except ImportError:
+    pass
+
 from phospho import config
 
 from .language_models import get_async_client, get_provider_and_model, get_sync_client
 from .models import JobResult, Message, ResultType
 
 logger = logging.getLogger(__name__)
 
@@ -22,27 +30,28 @@
     prompt: str,
     format_kwargs: Optional[dict] = None,
     model: str = "openai:gpt-3.5-turbo",
 ) -> JobResult:
     """
     Runs a prompt on a message and returns a boolean result.
     """
-    provider, model = get_provider_and_model(model)
+    # Check if some Env variables override the default model and LLM provider
+    provider, model_name = get_provider_and_model(model)
     openai_client = get_sync_client(provider)
 
     if format_kwargs is None:
         format_kwargs = {}
 
     formated_prompt = prompt.format(
         message_content=message.content,
         message_context=message.previous_messages_transcript(with_role=True),
         **format_kwargs,
     )
     response = openai_client.chat.completions.create(
-        model=model,
+        model=model_name,
         messages=[
             {"role": "system", "content": "You are a helpful assistant."},
             {
                 "role": "user",
                 "content": formated_prompt,
             },
         ],
@@ -70,29 +79,29 @@
     output_literal: List[str],
     format_kwargs: Optional[dict] = None,
     model: str = "openai:gpt-3.5-turbo",
 ) -> JobResult:
     """
     Runs a prompt on a message and returns a str from the list ouput_literal.
     """
-    provider, model = get_provider_and_model(model)
+    provider, model_name = get_provider_and_model(model)
     openai_client = get_sync_client(provider)
 
     if format_kwargs is None:
         format_kwargs = {}
 
     formated_prompt = prompt.format(
         message_content=message.transcript(with_role=True),
         message_context=message.transcript(
             only_previous_messages=True, with_previous_messages=True, with_role=True
         ),
         **format_kwargs,
     )
     response = openai_client.chat.completions.create(
-        model=model,
+        model=model_name,
         messages=[
             {"role": "system", "content": "You are a helpful assistant."},
             {
                 "role": "user",
                 "content": formated_prompt,
             },
         ],
@@ -136,14 +145,15 @@
     event_description: str,
     model: str = "openai:gpt-3.5-turbo",
 ) -> JobResult:
     """
     Detects if an event is present in a message.
     """
 
+    # Check if some Env variables override the default model and LLM provider
     provider, model_name = get_provider_and_model(model)
     async_openai_client = get_async_client(provider)
 
     # Build the prompt
     if len(message.previous_messages) > 0:
         prompt = f"""
 You are classifying an interaction between an end user and an assistant. The assistant is a chatbot that can perform tasks for the end user and answer his questions. 
@@ -262,14 +272,15 @@
     Message.metadata = {
         "successful_examples": [{input, output, flag}],
         "unsuccessful_examples": [{input, output, flag}],
     }
     """
     from phospho.utils import fits_in_context_window
 
+    # Check if some Env variables override the default model and LLM provider
     provider, model_name = get_provider_and_model(model)
     async_openai_client = get_async_client(provider)
 
     successful_examples = message.metadata.get("successful_examples", [])
     unsuccessful_examples = message.metadata.get("unsuccessful_examples", [])
 
     assert isinstance(successful_examples, list), "successful_examples is not a list"
@@ -292,23 +303,25 @@
 
     # Additional metadata
     api_call_time: Optional[float] = None
     llm_call: Optional[dict] = None
 
     async def zero_shot_evaluation(
         prompt: str,
-        model_name: str = "gpt-4-1106-preview",
+        model_name: str = os.getenv("MODEL_ID", "gpt-4-1106-preview"),
     ) -> Optional[Literal["success", "failure"]]:
         """
         Call the LLM API to get a zero shot classification of a task
         as a success or a failure.
         """
         nonlocal api_call_time
         nonlocal llm_call
 
+        logger.debug(f"Running zero shot evaluation with model {model_name}")
+
         start_time = time.time()
         response = await async_openai_client.chat.completions.create(
             model=model_name,
             messages=[
                 {"role": "system", "content": "You are a helpful assistant."},
                 {"role": "user", "content": prompt},
             ],
```

### Comparing `phospho-0.3.8/phospho/lab/lab.py` & `phospho-0.3.9/phospho/lab/lab.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/lab/language_models.py` & `phospho-0.3.9/phospho/lab/language_models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 from typing import Tuple
 
+import phospho.config as config
+
 try:
     from openai import AsyncOpenAI, OpenAI
 except ImportError:
     pass
 
 
 def get_provider_and_model(model: str) -> Tuple[str, str]:
@@ -14,14 +16,20 @@
 
     Args:
         model (str): The model string in the format "provider:model"
 
     Returns:
         tuple: A tuple with the provider and model
     """
+    # If the OVERRIDE_WITH_OLLAMA_MODEL environment variable is set, use the Ollama model
+    # in all cases. This is used in the preview mode or for tests.
+    if config.OVERRIDE_WITH_OLLAMA_MODEL is not None:
+        ollama_model = config.OVERRIDE_WITH_OLLAMA_MODEL
+        return "ollama", ollama_model
+
     split_result = model.split(":")
     if len(split_result) == 1:
         return "openai", split_result[0]
     return split_result[0], split_result[1]
 
 
 def get_async_client(provider: str) -> AsyncOpenAI:
```

### Comparing `phospho-0.3.8/phospho/lab/models.py` & `phospho-0.3.9/phospho/lab/models.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/lab/utils.py` & `phospho-0.3.9/phospho/lab/utils.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/log_queue.py` & `phospho-0.3.9/phospho/log_queue.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/models.py` & `phospho-0.3.9/phospho/models.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/sessions.py` & `phospho-0.3.9/phospho/sessions.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/steps.py` & `phospho-0.3.9/phospho/steps.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/tasks.py` & `phospho-0.3.9/phospho/tasks.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/testing.py` & `phospho-0.3.9/phospho/testing.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/phospho/utils.py` & `phospho-0.3.9/phospho/utils.py`

 * *Files identical despite different names*

### Comparing `phospho-0.3.8/pyproject.toml` & `phospho-0.3.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phospho"
-version = "0.3.8"
+version = "0.3.9"
 description = "Text Analytics for LLM apps"
 authors = ["Pierre-Louis Biojout <contact@phospho.app>"]
 readme = "README.md"
 homepage = "https://github.com/phospho-app/phospho"
 documentation = "https://docs.phospho.ai"
 keywords = ['LLM', 'Agents', 'gen ai', 'phospho', 'analytics', 'nlp']
 
@@ -40,11 +40,11 @@
 sphinx-copybutton = "^0.5.2"
 myst-parser = "^2.0.0"
 sphinx-autodoc2 = "^0.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-exclude = ["tests/", ".github/", ".pytest_cache/", "docs/", "local/"]
+# exclude = ["tests/", ".github/", ".pytest_cache/", "docs/", "local/"]
 
 [tool.poetry.extras]
 lab = ["openai", "tiktoken", "cohere", "pandas"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `phospho-0.3.8/PKG-INFO` & `phospho-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phospho
-Version: 0.3.8
+Version: 0.3.9
 Summary: Text Analytics for LLM apps
 Home-page: https://github.com/phospho-app/phospho
 Keywords: LLM,Agents,gen ai,phospho,analytics,nlp
 Author: Pierre-Louis Biojout
 Author-email: contact@phospho.app
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

