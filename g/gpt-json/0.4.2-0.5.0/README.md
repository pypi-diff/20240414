# Comparing `tmp/gpt_json-0.4.2.tar.gz` & `tmp/gpt_json-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_json-0.4.2.tar", max compression
+gzip compressed data, was "gpt_json-0.5.0.tar", max compression
```

## Comparing `gpt_json-0.4.2.tar` & `gpt_json-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1071 2024-03-20 15:03:58.409861 gpt_json-0.4.2/LICENSE
--rw-r--r--   0        0        0    11206 2024-03-20 15:03:58.409861 gpt_json-0.4.2/README.md
--rw-r--r--   0        0        0       93 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/enums.py
--rw-r--r--   0        0        0      837 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/exceptions.py
--rw-r--r--   0        0        0     4899 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/fn_calling.py
--rw-r--r--   0        0        0    24060 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/gpt.py
--rw-r--r--   0        0        0     2608 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/models.py
--rw-r--r--   0        0        0     1372 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/parsers.py
--rw-r--r--   0        0        0     1987 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/prompts.py
--rw-r--r--   0        0        0        0 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/py.typed
--rw-r--r--   0        0        0     4069 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/streaming.py
--rw-r--r--   0        0        0        0 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/conftest.py
--rw-r--r--   0        0        0     1051 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/shared.py
--rw-r--r--   0        0        0      381 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_api.py
--rw-r--r--   0        0        0      292 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_fixtures.py
--rw-r--r--   0        0        0     2377 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_fn_calling.py
--rw-r--r--   0        0        0    14081 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_gpt.py
--rw-r--r--   0        0        0     1386 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_models.py
--rw-r--r--   0        0        0     1517 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_parsers.py
--rw-r--r--   0        0        0     1502 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_prompts.py
--rw-r--r--   0        0        0     4747 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_streaming.py
--rw-r--r--   0        0        0     6186 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_transformations.py
--rw-r--r--   0        0        0     4319 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/test_truncation.py
--rw-r--r--   0        0        0     3177 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/utils/streaming_utils.py
--rw-r--r--   0        0        0     9903 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/tests/utils/test_streaming_utils.py
--rw-r--r--   0        0        0     5030 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/transformations.py
--rw-r--r--   0        0        0     3351 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/truncation.py
--rw-r--r--   0        0        0      404 2024-03-20 15:03:58.413861 gpt_json-0.4.2/gpt_json/types_oai.py
--rw-r--r--   0        0        0      668 2024-03-20 15:03:58.413861 gpt_json-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    11756 1970-01-01 00:00:00.000000 gpt_json-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-14 04:11:48.762114 gpt_json-0.5.0/LICENSE
+-rw-r--r--   0        0        0    11250 2024-04-14 04:11:48.762114 gpt_json-0.5.0/README.md
+-rw-r--r--   0        0        0       90 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/enums.py
+-rw-r--r--   0        0        0      837 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/exceptions.py
+-rw-r--r--   0        0        0     4899 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/fn_calling.py
+-rw-r--r--   0        0        0    28113 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/gpt.py
+-rw-r--r--   0        0        0     5551 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/models.py
+-rw-r--r--   0        0        0     1372 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/parsers.py
+-rw-r--r--   0        0        0     1987 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/prompts.py
+-rw-r--r--   0        0        0        0 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/py.typed
+-rw-r--r--   0        0        0     4069 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/streaming.py
+-rw-r--r--   0        0        0        0 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/conftest.py
+-rw-r--r--   0        0        0     1051 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/shared.py
+-rw-r--r--   0        0        0      381 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_api.py
+-rw-r--r--   0        0        0      292 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_fixtures.py
+-rw-r--r--   0        0        0     2377 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_fn_calling.py
+-rw-r--r--   0        0        0    14822 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_gpt.py
+-rw-r--r--   0        0        0     1040 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_models.py
+-rw-r--r--   0        0        0     1517 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_parsers.py
+-rw-r--r--   0        0        0     1502 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_prompts.py
+-rw-r--r--   0        0        0     4926 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_streaming.py
+-rw-r--r--   0        0        0     6186 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_transformations.py
+-rw-r--r--   0        0        0     4337 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/test_truncation.py
+-rw-r--r--   0        0        0     3177 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/utils/streaming_utils.py
+-rw-r--r--   0        0        0     9903 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/tests/utils/test_streaming_utils.py
+-rw-r--r--   0        0        0     5030 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/transformations.py
+-rw-r--r--   0        0        0     1806 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/truncation.py
+-rw-r--r--   0        0        0      404 2024-04-14 04:11:48.766114 gpt_json-0.5.0/gpt_json/types_oai.py
+-rw-r--r--   0        0        0      693 2024-04-14 04:11:48.766114 gpt_json-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11799 1970-01-01 00:00:00.000000 gpt_json-0.5.0/PKG-INFO
```

### Comparing `gpt_json-0.4.2/LICENSE` & `gpt_json-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/README.md` & `gpt_json-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,36 @@
+Metadata-Version: 2.1
+Name: gpt-json
+Version: 0.5.0
+Summary: Structured and typehinted GPT responses in Python.
+Author: Pierce Freeman
+Author-email: pierce@freeman.vc
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: backoff (>=2.2.1,<3.0.0)
+Requires-Dist: openai (>=1.16.2,<2.0.0)
+Requires-Dist: pydantic (>2.0.0,<3.0.0)
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
+Description-Content-Type: text/markdown
+
 # gpt-json
 
 `gpt-json` is a wrapper around GPT that allows for declarative definition of expected output format. Set up a schema, write a prompt, and get results back as beautiful typehinted objects.
 
-Specifically this library:
-- Utilizes Pydantic schema definitions for type casting and validations
-- Adds typehinting for both the API and the output schema
-- Allows GPT to respond with both single-objects and lists of objects
-- Includes some lightweight transformations of the output to remove superfluous context and fix broken json
-- Includes retry logic for the most common API failures
-- Formats the JSON schema as a flexible prompt that can be added into any message
-- Supports templating of prompts to allow for dynamic content
-- Validate typehinted function calls in the new GPT models, to better support agent creation
+This library introduces the following features:
+
+- 🏗️ Pydantic schema definitions for type casting and validations
+- 🧵 Templating of prompts to allow for dynamic content
+- 🔎 Supports Vision API, Function Calling, and standard chat prompts
+- 🚕 Lightweight transformations of the output to fix broken json
+- ♻️ Retry logic for the most common API failures
+- 📋 Predict single-objects and lists of objects
+- ✈️ Lightweight dependencies: only OpenAI, pydantic, and backoff
 
 ## Getting Started
 
 ```bash
 pip install gpt-json
 ```
 
@@ -193,27 +209,27 @@
 `InvalidFunctionResponse` - The function name is incorrect.
 `InvalidFunctionParameters` - The function name is correct, but doesn't match the input schema that was provided.
 
 ## Other Configurations
 
 The `GPTJSON` class supports other configuration parameters at initialization.
 
-| Parameter                   | Type                   | Description                                                                                                                                                                            |
-|-----------------------------|------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| model                       | GPTModelVersion \| str | (default: GPTModelVersion.GPT_4) - For convenience we provide the currently supported GPT model versions in the `GPTModelVersion` enum. You can also pass a string value if you want to use another more specific architecture.                                                                                                                                                       |
-| auto_trim                   | bool                   | (default: False) - If your input prompt is too long, perhaps because of dynamic injected content, will automatically truncate the text to create enough room for the model's response. |
-| auto_trim_response_overhead | int                    | (default: 0) - If you're using auto_trim, configures the max amount of tokens to allow in the model's response.                                                                        |
-| **kwargs | Any | Any other parameters you want to pass to the underlying `GPT` class, will just be a passthrough. |
+| Parameter                   | Type                   | Description                                                                                                                                                                                                                     |
+| --------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| model                       | GPTModelVersion \| str | (default: GPTModelVersion.GPT_4) - For convenience we provide the currently supported GPT model versions in the `GPTModelVersion` enum. You can also pass a string value if you want to use another more specific architecture. |
+| auto_trim                   | bool                   | (default: False) - If your input prompt is too long, perhaps because of dynamic injected content, will automatically truncate the text to create enough room for the model's response.                                          |
+| auto_trim_response_overhead | int                    | (default: 0) - If you're using auto_trim, configures the max amount of tokens to allow in the model's response.                                                                                                                 |
+| \*\*kwargs                  | Any                    | Any other parameters you want to pass to the underlying `GPT` class, will just be a passthrough.                                                                                                                                |
 
 ## Transformations
 
 GPT (especially GPT-4) is relatively good at formatting responses at JSON, but it's not perfect. Some of the more common issues are:
 
-- *Response truncation*: Since GPT is not internally aware of its response length limit, JSON payloads will sometimes exhaust the available token space. This results in a broken JSON payload where much of the data is valid but the JSON object is not closed, which is not valid syntax. There are many cases where this behavior is actually okay for production applications - for instance, if you list 100 generated strings, it's sometimes okay for you to take the 70 that actually rendered. In this case, `gpt-json` will attempt to fix the truncated payload by recreating the JSON object and closing it.
-- *Boolean variables*: GPT will sometimes confuse valid JSON boolean values with the boolean tokens that are used in other languages. The most common is generating `True` instead of `true`. `gpt-json` will attempt to fix these values.
+- _Response truncation_: Since GPT is not internally aware of its response length limit, JSON payloads will sometimes exhaust the available token space. This results in a broken JSON payload where much of the data is valid but the JSON object is not closed, which is not valid syntax. There are many cases where this behavior is actually okay for production applications - for instance, if you list 100 generated strings, it's sometimes okay for you to take the 70 that actually rendered. In this case, `gpt-json` will attempt to fix the truncated payload by recreating the JSON object and closing it.
+- _Boolean variables_: GPT will sometimes confuse valid JSON boolean values with the boolean tokens that are used in other languages. The most common is generating `True` instead of `true`. `gpt-json` will attempt to fix these values.
 
 When calling `gpt_json.run()`, we return a tuple of values:
 
 ```python
 payload = await gpt_json.run(...)
 
 print(transformations.fix_transforms)
@@ -221,15 +237,15 @@
 
 ```bash
 FixTransforms(fixed_truncation=True, fixed_bools=False)
 ```
 
 The first object is your generated Pydantic model. The second object is our correction storage object `FixTransforms`. This dataclass contains flags for each of the supported transformation cases that are sketched out above. This allows you to determine whether the response was explicitly parsed from the GPT JSON, or was passed through some middlelayers to get a correct output. From there you can accept or reject the response based on your own business logic.
 
-*Where you can help*: There are certainly more areas of common (and not-so-common failures). If you see these, please add a test case to the unit tests. If you can write a handler to help solve the general case, please do so. Otherwise flag it as a `pytest.xfail` and we'll add it to the backlog.
+_Where you can help_: There are certainly more areas of common (and not-so-common failures). If you see these, please add a test case to the unit tests. If you can write a handler to help solve the general case, please do so. Otherwise flag it as a `pytest.xfail` and we'll add it to the backlog.
 
 ## Testing
 
 We use poetry for package management. To run the bundled tests, clone the package from github.
 
 ```bash
 poetry install
@@ -249,7 +265,8 @@
 We use black and mypy for formatting. You can set up a pre-commit git hook to do this automatically via the `./lint.sh` helper file.
 
 If you perform a bulk reformatting to the codebase, you should add your most recent commit to the `.git-blame-ignore-revs` file and run:
 
 ```
 git config blame.ignoreRevsFile .git-blame-ignore-revs
 ```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gpt_json-0.4.2/gpt_json/exceptions.py` & `gpt_json-0.5.0/gpt_json/exceptions.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/fn_calling.py` & `gpt_json-0.5.0/gpt_json/fn_calling.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/gpt.py` & `gpt_json-0.5.0/gpt_json/gpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
+import warnings
 from asyncio import TimeoutError as AsyncTimeoutError
 from asyncio import wait_for
 from copy import copy
+from datetime import datetime
 from json import dumps as json_dumps
 from json import loads as json_loads
 from json.decoder import JSONDecodeError
 from typing import (
     Any,
     AsyncIterator,
     Callable,
@@ -14,50 +16,58 @@
     TypeVar,
     cast,
     get_args,
     get_origin,
 )
 
 import backoff
-import openai
-from openai.error import APIConnectionError, RateLimitError
-from openai.error import Timeout as OpenAITimeout
+from openai import AsyncOpenAI
+from openai._exceptions import APIConnectionError
+from openai._exceptions import APITimeoutError as OpenAITimeout
+from openai._exceptions import RateLimitError
+from openai.types.chat import ChatCompletionMessage
 from pydantic import BaseModel, Field, ValidationError
 from tiktoken import encoding_for_model
 
 from gpt_json.exceptions import InvalidFunctionParameters, InvalidFunctionResponse
 from gpt_json.fn_calling import (
     function_to_name,
     get_argument_for_function,
     parse_function,
 )
 from gpt_json.models import (
     FixTransforms,
     GPTMessage,
     GPTModelVersion,
+    ImageContent,
+    ModelVersionParams,
     ResponseType,
+    TextContent,
     TruncationOptions,
 )
 from gpt_json.parsers import find_json_response
 from gpt_json.prompts import generate_schema_prompt
 from gpt_json.streaming import (
     StreamingObject,
     parse_streamed_json,
     prepare_streaming_object,
 )
 from gpt_json.transformations import fix_bools, fix_truncated_json
-from gpt_json.truncation import num_tokens_from_messages, truncate_tokens
+from gpt_json.truncation import truncate_tokens
 from gpt_json.types_oai import ChatCompletionChunk
 
 logger = logging.getLogger("gptjson_logger")
 handler = logging.StreamHandler()
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 handler.setFormatter(formatter)
 logger.addHandler(handler)
 
+# https://github.com/openai/openai-python/issues/1306
+ChatCompletionMessage.model_rebuild()
+
 
 def handle_backoff(details):
     logger.warning(
         "Backing off {wait:0.1f} seconds after {tries} tries "
         "calling function {target} with args {args} and kwargs "
         "{kwargs}".format(**details)
     )
@@ -99,38 +109,42 @@
     """
 
     _cls_schema_model: Type[SchemaType] | None = None
     schema_model: Type[SchemaType] | None = None
 
     def __init__(
         self,
-        api_key: str | None = None,
+        api_key: str,
         model: GPTModelVersion | str = GPTModelVersion.GPT_4,
+        model_max_tokens: int | None = None,
         auto_trim: bool = False,
         auto_trim_response_overhead: int = 0,
         functions: list[Callable[[Any], Any]] | None = None,
         # For messages that are relatively deterministic
         temperature=0.2,
         timeout: int | None = None,
         openai_max_retries=3,
         **kwargs,
     ):
         """
         :param api_key: OpenAI API key, if `OPENAI_API_KEY` environment variable is not set
         :param model: GPTModelVersion or string model name
+        :param model_max_tokens: If a string is provided for the model name, users must specify the maximum tokens
+            that it supports. Allows for more flexibility in adding newer models that aren't yet specified
+            in the core library enum.
         :param auto_trim: If True, automatically trim messages to fit within the model's token limit
         :param auto_trim_response_overhead: If auto_trim is True, will leave at least `auto_trim_response_overhead` space
             for the output payload. For GPT, initial prompt + response <= allowed tokens.
         :param temperature: Temperature (or variation) of response payload; 0 is the most deterministic, 1 is the most random
         :param timeout: Timeout in seconds for each OpenAI API calls before timing out.
         :param openai_max_retries: Amount of times to retry failed API calls, caused by often transient load or rate limit issues
         :param kwargs: Additional arguments to pass to OpenAI's `openai.Completion.create` method
 
         """
-        self.model = model.value if isinstance(model, GPTModelVersion) else model
+        self.model = self.get_model_metadata(model, model_max_tokens)
         self.auto_trim = auto_trim
         self.temperature = temperature
         self.timeout = timeout
         self.openai_max_retries = openai_max_retries
         self.openai_arguments = kwargs
         self.schema_model = self._cls_schema_model
         self.functions = {
@@ -162,29 +176,24 @@
         elif issubclass(self.schema_model, BaseModel):
             self.extract_type = ResponseType.DICTIONARY
         else:
             raise ValueError(
                 "GPTJSON needs to be instantiated with a pydantic.BaseModel schema."
             )
 
-        if "gpt-4" in self.model:
-            self.max_tokens = (
-                8192 - auto_trim_response_overhead if self.auto_trim else 8192
-            )
-        elif "gpt-3.5" in self.model:
-            self.max_tokens = (
-                4096 - auto_trim_response_overhead if self.auto_trim else 4096
-            )
-        else:
-            raise ValueError(
-                "Unknown model to infer max tokens, see https://platform.openai.com/docs/models/gpt-4 for more information on token length."
-            )
+        self.max_tokens = (
+            self.model.max_length - auto_trim_response_overhead
+            if self.auto_trim
+            else self.model.max_length
+        )
 
         self.schema_prompt = generate_schema_prompt(self.schema_model)
-        self.api_key = api_key
+
+        # We use separate retry logic, versus the one that's baked into OpenAPI
+        self.client = AsyncOpenAI(api_key=api_key, max_retries=1)
 
     async def run(
         self,
         messages: list[GPTMessage],
         max_response_tokens: int | None = None,
         format_variables: dict[str, Any] | None = None,
         truncation_options: TruncationOptions | None = None,
@@ -218,15 +227,15 @@
         response = await backoff_request_submission(
             messages,
             max_response_tokens=max_response_tokens,
             allow_functions=allow_functions,
         )
 
         logger.debug("------- RAW RESPONSE ----------")
-        logger.debug(response["choices"])
+        logger.debug(response.choices)
         logger.debug("------- END RAW RESPONSE ----------")
 
         # If the response requests a function call, prefer this over the main response
         response_message = self.extract_response_message(response)
         if response_message is None:
             return RunResponse(
                 raw_response=None,
@@ -235,36 +244,36 @@
                 function_call=None,
                 function_arg=None,
             )
 
         function_call: Callable[[BaseModel], Any] | None = None
         function_parsed: BaseModel | None = None
 
-        if response_message.get("function_call"):
-            function_name = response_message["function_call"]["name"]
-            function_args_string = response_message["function_call"]["arguments"]
+        if response_message.function_call:
+            function_name = response_message.function_call.name
+            function_args_string = response_message.function_call.arguments
             if function_name not in self.functions:
                 raise InvalidFunctionResponse(function_name)
 
             function_call = self.functions[function_name]
             function_arg_model = get_argument_for_function(function_call)
 
             # Parameters are formatted as raw json strings
             try:
                 function_parsed = function_arg_model.model_validate_json(
                     function_args_string
                 )
             except (ValueError, ValidationError):
                 raise InvalidFunctionParameters(function_name, function_args_string)
 
-        raw_response = GPTMessage.model_validate(response_message)
+        raw_response = GPTMessage.model_validate(response_message.model_dump())
         raw_response.allow_templating = False
 
         extracted_json, fixed_payload = self.extract_json(
-            response_message, self.extract_type
+            raw_response, self.extract_type
         )
 
         # Cast to schema model
         if extracted_json is None:
             return RunResponse(
                 raw_response=raw_response,
                 response=None,
@@ -363,20 +372,20 @@
             if (
                 previous_partial is None
                 or previous_partial.partial_obj != partial_response.partial_obj
             ):
                 yield partial_response
                 previous_partial = partial_response
 
-    def extract_json(self, response_message, extract_type: ResponseType):
+    def extract_json(self, response_message: GPTMessage, extract_type: ResponseType):
         """
         Assumes one main block of results, either list of dictionary
         """
 
-        full_response = response_message["content"]
+        full_response = self.get_content_text(response_message.get_content_payloads())
         if not full_response:
             return None, None
 
         extracted_response = find_json_response(full_response, extract_type)
         if extracted_response is None:
             return None, None
 
@@ -395,21 +404,21 @@
         except JSONDecodeError as e:
             logger.debug(f"Extracted: {extracted_response}")
             logger.debug(f"Did parse: {fixed_response}")
             logger.error(f"JSON decode error, likely malformed json input: {e}")
             return None, fixed_payload
 
     def extract_response_message(self, completion_response):
-        choices = completion_response["choices"]
+        choices = completion_response.choices
 
         if not choices:
             logger.warning("No choices available, should report error...")
             return None
 
-        return choices[0]["message"]
+        return choices[0].message
 
     async def submit_request(
         self,
         messages: list[GPTMessage],
         max_response_tokens: int | None,
         allow_functions: bool,
         stream: bool = False,
@@ -431,36 +440,45 @@
 
         if allow_functions and self.functions:
             optional_parameters["functions"] = [
                 parse_function(fn) for fn in self.functions.values()
             ]
             optional_parameters["function_call"] = "auto"
 
-        execute_prediction = openai.ChatCompletion.acreate(
-            model=self.model,
+        execute_prediction = self.client.chat.completions.create(
+            model=self.model.api_name,
             messages=[self.message_to_dict(message) for message in messages],
             temperature=self.temperature,
-            api_key=self.api_key,
             stream=stream,
             **optional_parameters,
             **self.openai_arguments,
         )
 
+        # We can't combine streams (which return async generators) with timeouts, since our client
+        # functions expect us to return immediately
+        if self.timeout is not None and stream:
+            raise ValueError("Timeouts are not supported with streaming completions")
+
+        if stream:
+            return execute_prediction
+
         # The 'timeout' parameter supported by the OpenAI API is only used to cycle
         # the model while it's warming up
         # https://github.com/openai/openai-python/blob/fe3abd16b582ae784d8a73fd249bcdfebd5752c9/openai/api_resources/chat_completion.py#L41
         # We instead use a client-side timeout to prevent the API from hanging, which is more inline
         # with the expected behavior of our passed timeout.
         if self.timeout is None:
             return await execute_prediction
         else:
             try:
                 return await wait_for(execute_prediction, timeout=self.timeout)
             except AsyncTimeoutError:
-                raise OpenAITimeout
+                # We don't have access to the underlying httpx.Request, so we just return None in place
+                # of the request object
+                raise OpenAITimeout(None)  # type: ignore
 
     def fill_messages(
         self,
         messages: list[GPTMessage],
         format_variables: dict[str, Any] | None,
         truncation_options: TruncationOptions | None,
         max_response_tokens: int | None,
@@ -495,37 +513,39 @@
         # allowed amount of response tokens to keep the full prompt and response
         # within the model length bounds
         truncation_options.max_prompt_tokens = truncation_options.max_prompt_tokens or (
             self.max_tokens - (max_response_tokens or 0)
         )
 
         # fill the messages without the target variable to calculate the "space" we have left
+        enc = encoding_for_model("gpt-4")
         format_variables_no_target = format_variables.copy()
         format_variables_no_target[truncation_options.target_variable] = ""
-        target_variable_max_tokens = (
-            truncation_options.max_prompt_tokens
-            - num_tokens_from_messages(
-                [
-                    self.message_to_dict(
-                        self.fill_message_template(message, format_variables_no_target)
+        target_variable_max_tokens = truncation_options.max_prompt_tokens - sum(
+            [
+                len(
+                    enc.encode(
+                        self.get_content_text(new_message.get_content_payloads())
                     )
-                    for message in messages
-                ],
-                self.model,
-            )
+                )
+                for message in messages
+                for new_message in [
+                    self.fill_message_template(message, format_variables_no_target)
+                ]
+            ],
         )
 
-        if target_variable_max_tokens < 0:
+        if target_variable_max_tokens <= 0:
             raise ValueError(
-                f"Truncation options max_prompt_tokens {truncation_options.max_prompt_tokens} is too small to fit the messages."
+                f"Truncation options max_prompt_tokens {truncation_options.max_prompt_tokens} is too small to fit any part of the variable."
             )
 
         truncated_target_variable = truncate_tokens(
             text=format_variables[truncation_options.target_variable],
-            model=self.model,
+            model=self.model.api_name,
             mode=truncation_options.truncation_mode,
             max_tokens=target_variable_max_tokens,
             custom_truncate_next=truncation_options.custom_truncate_next,
         )
 
         return [
             self.fill_message_template(
@@ -547,71 +567,91 @@
                 [function_to_name(fn) for fn in self.functions.values()]
             ),
         }
 
         if message.content is None or not message.allow_templating:
             return message
 
+        new_message = copy(message)
+        new_message.content = []
+
         # Regular quotes should passthrough to the next stage, except for our special keys
-        content = message.content.replace("{", "{{").replace("}", "}}")
-        for key in auto_format.keys():
-            content = content.replace("{{" + key + "}}", "{" + key + "}")
-        content = content.format(**auto_format)
-
-        # We do this formatting in a separate pass so we can fill any template variables that might
-        # have been left in the pydantic field typehints
-        content = content.format(**format_variables)
+        for payload in message.get_content_payloads():
+            if not isinstance(payload, TextContent):
+                new_message.content.append(payload)
+                continue
+
+            content = payload.text.replace("{", "{{").replace("}", "}}")
+            for key in auto_format.keys():
+                content = content.replace("{{" + key + "}}", "{" + key + "}")
+
+            content = content.format(**auto_format)
+
+            # We do this formatting in a separate pass so we can fill any template variables that might
+            # have been left in the pydantic field typehints
+            content = content.format(**format_variables)
+
+            new_payload = copy(payload)
+            new_payload.text = content
+            new_message.content.append(new_payload)
 
-        new_message = copy(message)
-        new_message.content = content
         return new_message
 
     def message_to_dict(self, message: GPTMessage):
-        obj = json_loads(message.model_dump_json(exclude_unset=True))
+        obj = json_loads(message.model_dump_json(by_alias=True, exclude_none=True))
         obj.pop("allow_templating", None)
         return obj
 
-    def trim_messages(self, messages: list[GPTMessage], n: int):
+    def trim_messages(self, messages: list[GPTMessage], n: int) -> list[GPTMessage]:
         """
         Returns a list of messages with a total token count less than n tokens,
-        cropping the last message if needed.
+        cropping the last message if needed. Note - right now images are excluded
+        from the token count.
 
         Args:
             messages (list): List of strings to be checked.
             n (int): The maximum number of tokens allowed.
 
         Returns:
             list: A list of messages with a total token count less than n tokens.
         """
-        message_text = [message.content for message in messages if message.content]
+        message_text = [message.get_content_payloads() for message in messages]
 
         enc = encoding_for_model("gpt-4")
-        filtered_messages = []
+        filtered_messages: list[list[TextContent | ImageContent]] = []
         current_token_count = 0
         original_token_count = sum(
-            [len(enc.encode(message)) for message in message_text]
+            [
+                len(enc.encode(self.get_content_text(message)))
+                for message in message_text
+            ]
         )
 
         for message in message_text:
-            tokens = enc.encode(message)
+            tokens = enc.encode(self.get_content_text(message))
             message_token_count = len(tokens)
 
             if current_token_count + message_token_count < n:
                 filtered_messages.append(message)
                 current_token_count += message_token_count
             else:
                 remaining_tokens = n - current_token_count
                 if remaining_tokens > 0:
                     cropped_message = enc.decode(tokens[:remaining_tokens])
-                    filtered_messages.append(cropped_message)
+                    filtered_messages.append(
+                        [
+                            # Note that this will drop any images in the current message
+                            TextContent(text=cropped_message)
+                        ]
+                    )
                 current_token_count += remaining_tokens
                 break
 
         # Recreate the messages with our new text
-        new_messages = []
+        new_messages: list[GPTMessage] = []
         for i, content in enumerate(filtered_messages):
             new_message = copy(messages[i])
             new_message.content = content
             new_messages.append(new_message)
 
         # Log a copy of the message array if we have to crop it
         if current_token_count != original_token_count:
@@ -621,10 +661,63 @@
         else:
             logger.debug(
                 f"Skipping trim ({original_token_count}) ({current_token_count})"
             )
 
         return new_messages
 
+    def get_content_text(self, content: list[TextContent | ImageContent]):
+        return " ".join(
+            [payload.text for payload in content if isinstance(payload, TextContent)]
+        )
+
+    def get_model_metadata(
+        self,
+        model: GPTModelVersion | str,
+        model_max_tokens: int | None,
+    ):
+        if isinstance(model, GPTModelVersion):
+            # User should not specify the model_max_tokens if they are passing a GPTModelVersion, since
+            # their value will be overridden by our default config
+            if model_max_tokens is not None:
+                raise ValueError(
+                    "model_max_tokens should not be specified when passing a GPTModelVersion object."
+                )
+
+            # Determine if the deprecation date is specified, should re-raise a deprecation warning
+            if model.value.deprecated_date is not None:
+                deprecation_date = model.value.deprecated_date
+                if deprecation_date < datetime.now().date():
+                    raise ValueError(
+                        f"Model {model.value.api_name} is deprecated as of {deprecation_date}."
+                    )
+                warnings.warn(
+                    f"Model {model.value.api_name} is deprecated as of {deprecation_date}.",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+
+            # Specific deprecation warning related to our implementation. We want to encourage users
+            # to use a absolute model version instead of a continuously updating one.
+            if model in {GPTModelVersion.GPT_4, GPTModelVersion.GPT_3_5}:
+                warnings.warn(
+                    f"gpt-json will not support continuous model updates going forward.\n"
+                    "Switch to an absolute model revision like `GPTModelVersion.GPT_4_0613`.",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+
+            return model.value
+
+        if not model_max_tokens:
+            raise ValueError(
+                "You must specify a `model_max_tokens` if you are using a custom model"
+            )
+
+        return ModelVersionParams(
+            api_name=model,
+            max_length=model_max_tokens,
+        )
+
     def __class_getitem__(cls, item):
         cls._cls_schema_model = item
         return cls
```

### Comparing `gpt_json-0.4.2/gpt_json/parsers.py` & `gpt_json-0.5.0/gpt_json/parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/prompts.py` & `gpt_json-0.5.0/gpt_json/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/streaming.py` & `gpt_json-0.5.0/gpt_json/streaming.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/tests/shared.py` & `gpt_json-0.5.0/gpt_json/tests/shared.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/tests/test_fn_calling.py` & `gpt_json-0.5.0/gpt_json/tests/test_fn_calling.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/tests/test_gpt.py` & `gpt_json-0.5.0/gpt_json/tests/test_gpt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,71 @@
 import asyncio
 from json import dumps as json_dumps
 from time import time
+from typing import Any
 from unittest.mock import AsyncMock, patch
 
-import openai
 import pytest
-from openai.error import Timeout as OpenAITimeout
+from openai._exceptions import APITimeoutError as OpenAITimeout
 from pydantic import BaseModel, Field
+from pytest_httpx import HTTPXMock
 
-from gpt_json.fn_calling import parse_function
 from gpt_json.gpt import GPTJSON, ListResponse
-from gpt_json.models import FixTransforms, GPTMessage, GPTMessageRole, GPTModelVersion
+from gpt_json.models import (
+    FixTransforms,
+    GPTMessage,
+    GPTMessageRole,
+    GPTModelVersion,
+    TextContent,
+)
 from gpt_json.tests.shared import (
     GetCurrentWeatherRequest,
     MySchema,
     MySubSchema,
     UnitType,
     get_current_weather,
 )
 from gpt_json.transformations import JsonFixEnum
 
 
+def make_assistant_response(choices: list[Any]):
+    # https://platform.openai.com/docs/api-reference/chat/create
+    return {
+        "id": "chatcmpl-123",
+        "object": "chat.completion",
+        "created": 1677652288,
+        "model": "gpt-3.5-turbo-0125",
+        "system_fingerprint": "fp_3478aj6f3a",
+        "choices": choices,
+        "usage": {"prompt_tokens": 9, "completion_tokens": 12, "total_tokens": 21},
+    }
+
+
 def test_throws_error_if_no_model_specified():
     with pytest.raises(
         ValueError, match="needs to be instantiated with a schema model"
     ):
-        GPTJSON(None)
+        GPTJSON(api_key="TEST")
 
 
 @pytest.mark.parametrize(
     "role_type,expected",
     [
         (GPTMessageRole.SYSTEM, "system"),
         (GPTMessageRole.USER, "user"),
         (GPTMessageRole.ASSISTANT, "assistant"),
     ],
 )
 def test_cast_message_to_gpt_format(role_type: GPTMessageRole, expected: str):
-    parser = GPTJSON[MySchema](None)
+    parser = GPTJSON[MySchema](api_key="TEST")
     assert (
         parser.message_to_dict(
             GPTMessage(
                 role=role_type,
-                content="test",
+                content=[TextContent(text="test")],
             )
         )["role"]
         == expected
     )
 
 
 @pytest.mark.asyncio
@@ -134,138 +153,109 @@
             ),
             FixTransforms(
                 fixed_bools=True, fixed_truncation=JsonFixEnum.UNCLOSED_VALUE
             ),
         ),
     ],
 )
-async def test_acreate(
+async def test_create(
     schema_typehint,
+    httpx_mock: HTTPXMock,
     response_raw: str,
     parsed: BaseModel,
     expected_transformations: FixTransforms,
 ):
     model_version = GPTModelVersion.GPT_3_5
     messages = [
         GPTMessage(
             role=GPTMessageRole.USER,
-            content="Input prompt",
+            content=[TextContent(text="Input prompt")],
         )
     ]
 
+    # Define mock response
+    httpx_mock.add_response(
+        url="https://api.openai.com/v1/chat/completions",
+        json=make_assistant_response(
+            [
+                {
+                    "message": {
+                        "role": "assistant",
+                        "content": response_raw,
+                    },
+                    "index": 0,
+                    "finish_reason": "stop",
+                }
+            ]
+        ),
+    )
+
     model = GPTJSON[schema_typehint](
-        None,
+        api_key="TEST",
         model=model_version,
         temperature=0.0,
         timeout=60,
     )
 
-    # Define mock response
-    mock_response = {
-        "choices": [
-            {
-                "message": {
-                    "role": "assistant",
-                    "content": response_raw,
-                },
-                "index": 0,
-                "finish_reason": "stop",
-            }
-        ]
-    }
-
-    # Create the mock
-    with patch.object(openai.ChatCompletion, "acreate") as mock_acreate:
-        # Make the mock function asynchronous
-        mock_acreate.return_value = mock_response
-
-        # Call the function and pass the expected parameters
-        response = await model.run(messages=messages)
-
-        # Assert that the mock function was called with the expected parameters
-        mock_acreate.assert_called_with(
-            model=model_version.value,
-            messages=[
-                {
-                    "role": message.role.value,
-                    "content": message.content,
-                }
-                for message in messages
-            ],
-            temperature=0.0,
-            api_key=None,
-            stream=False,
-        )
+    # Call the function and pass the expected parameters
+    response = await model.run(messages=messages)
 
     assert response
     assert response.response
     assert response.response.model_dump() == parsed.model_dump()
     assert response.fix_transforms == expected_transformations
 
 
 @pytest.mark.asyncio
-async def test_acreate_with_function_calls():
+async def test_create_with_function_calls(
+    httpx_mock: HTTPXMock,
+):
     model_version = GPTModelVersion.GPT_3_5
     messages = [
         GPTMessage(
             role=GPTMessageRole.USER,
-            content="Input prompt",
+            content=[TextContent(text="Input prompt")],
         )
     ]
 
+    # Define mock response
+    httpx_mock.add_response(
+        url="https://api.openai.com/v1/chat/completions",
+        json=make_assistant_response(
+            [
+                {
+                    "message": {
+                        "role": "assistant",
+                        "content": "",
+                        "function_call": {
+                            "name": "get_current_weather",
+                            "arguments": json_dumps(
+                                {
+                                    "location": "Boston",
+                                    "unit": "fahrenheit",
+                                }
+                            ),
+                        },
+                    },
+                    "index": 0,
+                    "finish_reason": "stop",
+                }
+            ]
+        ),
+    )
+
     model = GPTJSON[MySchema](
-        None,
+        api_key="TEST",
         model=model_version,
         temperature=0.0,
         timeout=60,
         functions=[get_current_weather],
     )
 
-    mock_response = {
-        "choices": [
-            {
-                "message": {
-                    "role": "assistant",
-                    "content": "",
-                    "function_call": {
-                        "name": "get_current_weather",
-                        "arguments": json_dumps(
-                            {
-                                "location": "Boston",
-                                "unit": "fahrenheit",
-                            }
-                        ),
-                    },
-                },
-                "index": 0,
-                "finish_reason": "stop",
-            }
-        ]
-    }
-
-    with patch.object(openai.ChatCompletion, "acreate") as mock_acreate:
-        mock_acreate.return_value = mock_response
-
-        response = await model.run(messages=messages)
-
-        mock_acreate.assert_called_with(
-            model=model_version.value,
-            messages=[
-                {
-                    "role": message.role.value,
-                    "content": message.content,
-                }
-                for message in messages
-            ],
-            temperature=0.0,
-            api_key=None,
-            stream=False,
-            functions=[parse_function(get_current_weather)],
-            function_call="auto",
-        )
+    response = await model.run(messages=messages)
 
     assert response
     assert response.response is None
     assert response.function_call == get_current_weather
     assert response.function_arg == GetCurrentWeatherRequest(
         location="Boston", unit=UnitType.FAHRENHEIT
     )
@@ -295,15 +285,17 @@
                 GPTMessage(role=GPTMessageRole.SYSTEM, content="Hello"),
                 GPTMessage(role=GPTMessageRole.USER, content="World" * (8192 - 1)),
             ],
         ),
     ],
 )
 def test_trim_messages(input_messages, expected_output_messages):
-    gpt = GPTJSON[MySchema](None, auto_trim=True, auto_trim_response_overhead=0)
+    gpt = GPTJSON[MySchema](
+        api_key="TEST", auto_trim=True, auto_trim_response_overhead=0
+    )
 
     output_messages = gpt.trim_messages(input_messages, n=8192)
 
     assert len(output_messages) == len(expected_output_messages)
 
     for output_message, expected_output_message in zip(
         output_messages, expected_output_messages
@@ -315,117 +307,151 @@
 def test_two_gptjsons():
     class TestSchema1(BaseModel):
         field1: str
 
     class TestSchema2(BaseModel):
         field2: str
 
-    gptjson1 = GPTJSON[TestSchema1](None)
+    gptjson1 = GPTJSON[TestSchema1](api_key="TRUE")
 
     # Shouldn't allow instantion without a schema
     # We already expect a mypy error here, which is why we need a `type ignore`
     # butr we also want to make sure that the error is raised at runtime
     with pytest.raises(ValueError):
         gptjson2 = GPTJSON(None)  # type: ignore
 
-    gptjson2 = GPTJSON[TestSchema2](None)
+    gptjson2 = GPTJSON[TestSchema2](api_key="TRUE")
 
     assert gptjson1.schema_model == TestSchema1
     assert gptjson2.schema_model == TestSchema2
 
 
 def test_fill_message_schema_template():
     class TestTemplateSchema(BaseModel):
         template_field: str = Field(description="Max length {max_length}")
 
-    gpt = GPTJSON[TestTemplateSchema](None)
+    gpt = GPTJSON[TestTemplateSchema](api_key="TRUE")
     assert gpt.fill_message_template(
         GPTMessage(
             role=GPTMessageRole.USER,
-            content="Variable: {max_length}\nMy schema is here: {json_schema}",
+            content=[
+                TextContent(
+                    text="Variable: {max_length}\nMy schema is here: {json_schema}"
+                )
+            ],
         ),
         dict(
             max_length=100,
         ),
     ) == GPTMessage(
         role=GPTMessageRole.USER,
-        content='Variable: 100\nMy schema is here: {\n"template_field": str // Max length 100\n}',
+        content=[
+            TextContent(
+                text='Variable: 100\nMy schema is here: {\n"template_field": str // Max length 100\n}'
+            )
+        ],
     )
 
 
 def test_fill_message_functions_template():
     class TestTemplateSchema(BaseModel):
         template_field: str = Field(description="Max length {max_length}")
 
-    gpt = GPTJSON[TestTemplateSchema](None, functions=[get_current_weather])
+    gpt = GPTJSON[TestTemplateSchema](api_key="TRUE", functions=[get_current_weather])
     assert gpt.fill_message_template(
         GPTMessage(
             role=GPTMessageRole.USER,
-            content="Here are the functions available: {functions}",
+            content=[TextContent(text="Here are the functions available: {functions}")],
         ),
         format_variables=dict(),
     ) == GPTMessage(
         role=GPTMessageRole.USER,
-        content='Here are the functions available: ["get_current_weather"]',
+        content=[
+            TextContent(
+                text='Here are the functions available: ["get_current_weather"]'
+            )
+        ],
     )
 
 
 @pytest.mark.asyncio
-async def test_extracted_json_is_None():
-    gpt = GPTJSON[MySchema](None)
+async def test_extracted_json_is_none(httpx_mock: HTTPXMock):
+    gpt = GPTJSON[MySchema](api_key="TRUE")
+
+    httpx_mock.add_response(
+        url="https://api.openai.com/v1/chat/completions",
+        json=make_assistant_response(
+            [{"message": {"content": "some content", "role": "assistant"}}]
+        ),
+    )
 
     with patch.object(
-        gpt,
-        "submit_request",
-        return_value={
-            "choices": [{"message": {"content": "some content", "role": "assistant"}}]
-        },
-    ), patch.object(
         gpt, "extract_json", return_value=(None, FixTransforms(None, False))
     ):
         result = await gpt.run(
-            [GPTMessage(role=GPTMessageRole.SYSTEM, content="message content")]
+            [
+                GPTMessage(
+                    role=GPTMessageRole.SYSTEM,
+                    content=[TextContent(text="message content")],
+                )
+            ]
         )
         assert result.response is None
 
 
 @pytest.mark.asyncio
-async def test_no_valid_results_from_remote_request():
-    gpt = GPTJSON[MySchema](None)
+async def test_no_valid_results_from_remote_request(
+    httpx_mock: HTTPXMock,
+):
+    gpt = GPTJSON[MySchema](api_key="TRUE")
 
-    with patch.object(gpt, "submit_request", return_value={"choices": []}):
-        result = await gpt.run(
-            [GPTMessage(role=GPTMessageRole.SYSTEM, content="message content")]
-        )
-        assert result.response is None
+    httpx_mock.add_response(
+        url="https://api.openai.com/v1/chat/completions",
+        json=make_assistant_response([]),
+    )
+
+    result = await gpt.run(
+        [
+            GPTMessage(
+                role=GPTMessageRole.SYSTEM,
+                content=[TextContent(text="message content")],
+            )
+        ]
+    )
+    assert result.response is None
 
 
 @pytest.mark.asyncio
-async def test_unable_to_find_valid_json_payload():
-    gpt = GPTJSON[MySchema](None)
+async def test_unable_to_find_valid_json_payload(httpx_mock: HTTPXMock):
+    httpx_mock.add_response(
+        url="https://api.openai.com/v1/chat/completions",
+        json=make_assistant_response(
+            [{"message": {"content": "some content", "role": "assistant"}}]
+        ),
+    )
+    gpt = GPTJSON[MySchema](api_key="TRUE")
 
     with patch.object(
-        gpt,
-        "submit_request",
-        return_value={
-            "choices": [{"message": {"content": "some content", "role": "assistant"}}]
-        },
-    ), patch.object(
         gpt, "extract_json", return_value=(None, FixTransforms(None, False))
     ):
         result = await gpt.run(
-            [GPTMessage(role=GPTMessageRole.SYSTEM, content="message content")]
+            [
+                GPTMessage(
+                    role=GPTMessageRole.SYSTEM,
+                    content=[TextContent(text="message content")],
+                )
+            ]
         )
         assert result.response is None
 
 
 @pytest.mark.asyncio
 async def test_unknown_model_to_infer_max_tokens():
     with pytest.raises(ValueError):
-        GPTJSON[MySchema](model="UnknownModel", auto_trim=True)
+        GPTJSON[MySchema](api_key="TRUE", model="UnknownModel", auto_trim=True)
 
 
 @pytest.mark.asyncio
 async def test_timeout():
     class MockResponse:
         """
         We need to build an actual response class here because the internal openai
@@ -449,29 +475,36 @@
                         "index": 0,
                         "finish_reason": "stop",
                     }
                 ]
             }
             return json_dumps(mock_response).encode()
 
-    with patch("aiohttp.ClientSession.request", new_callable=AsyncMock) as mock_request:
+    with patch("gpt_json.gpt.AsyncOpenAI") as mock_client:
         # Mock a stalling request
         async def side_effect(*args, **kwargs):
             await asyncio.sleep(4)
             return MockResponse("TEST_RESPONSE")
 
-        mock_request.side_effect = side_effect
+        mock_client.return_value.chat.completions.create = AsyncMock(
+            side_effect=side_effect
+        )
 
         gpt = GPTJSON[MySchema](api_key="ABC", timeout=2)
 
         start_time = time()
 
         with pytest.raises(OpenAITimeout):
             await gpt.run(
-                [GPTMessage(role=GPTMessageRole.SYSTEM, content="message content")],
+                [
+                    GPTMessage(
+                        role=GPTMessageRole.SYSTEM,
+                        content=[TextContent(text="message content")],
+                    )
+                ],
             )
 
         end_time = time()
         duration = end_time - start_time
 
         # Assert duration is about 2 seconds
         pytest.approx(duration, 2, 0.2)
```

### Comparing `gpt_json-0.4.2/gpt_json/tests/test_parsers.py` & `gpt_json-0.5.0/gpt_json/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/tests/test_prompts.py` & `gpt_json-0.5.0/gpt_json/tests/test_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/tests/test_streaming.py` & `gpt_json-0.5.0/gpt_json/tests/test_streaming.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 from unittest.mock import patch
 
-import openai
 import pytest
 
 from gpt_json.gpt import GPTJSON
-from gpt_json.models import GPTMessage, GPTMessageRole, GPTModelVersion
+from gpt_json.models import GPTMessage, GPTMessageRole, GPTModelVersion, TextContent
 from gpt_json.streaming import StreamingObject
 from gpt_json.tests.utils.streaming_utils import tokenize
 from gpt_json.tests.utils.test_streaming_utils import (
     EXAMPLE_DICT,
     EXAMPLE_DICT_STREAM_DATA,
     EXAMPLE_MULTI_NESTED,
     EXAMPLE_MULTI_NESTED_STREAM_DATA,
@@ -82,38 +81,36 @@
     expected_stream_data,
     should_support,
 ):
     model_version = GPTModelVersion.GPT_3_5
     messages = [
         GPTMessage(
             role=GPTMessageRole.USER,
-            content="Input prompt",
+            content=[TextContent(text="Input prompt")],
         )
     ]
 
-    model = GPTJSON[schema_typehint](  # type: ignore
-        None,
-        model=model_version,
-        temperature=0.0,
-        timeout=60,
-    )
-
     # Define mock response
     mocked_oai_raw_responses = _mock_oai_streaming_chunks(full_object)
 
     async def async_list_to_generator(my_list):
         for item in my_list:
             yield item
 
     mock_response = async_list_to_generator(mocked_oai_raw_responses)
 
     # Create the mock
-    with patch.object(openai.ChatCompletion, "acreate") as mock_acreate:
-        # Make the mock function asynchronous
-        mock_acreate.return_value = mock_response
+    with patch("gpt_json.gpt.AsyncOpenAI") as mock_client:
+        mock_client.return_value.chat.completions.create.return_value = mock_response
+
+        model = GPTJSON[schema_typehint](  # type: ignore
+            api_key="TEST",
+            model=model_version,
+            temperature=0.0,
+        )
 
         if not should_support:
             with pytest.raises(NotImplementedError):
                 streaming_objects = [
                     obj async for obj in model.stream(messages=messages)
                 ]
             return True
@@ -133,20 +130,22 @@
                 value_change=expected_value_change,
             )
             assert stream_obj == expected_obj
 
             idx += 1
 
         # Assert that the mock function was called with the expected parameters, including streaming
-        mock_acreate.assert_called_with(
-            model=model_version.value,
+        mock_client.return_value.chat.completions.create.assert_called_with(
+            model=model_version.value.api_name,
             messages=[
                 {
                     "role": message.role.value,
-                    "content": message.content,
+                    "content": [
+                        content.model_dump(by_alias=True, exclude_none=True)
+                        for content in message.get_content_payloads()
+                    ],
                 }
                 for message in messages
             ],
             temperature=0.0,
             stream=True,
-            api_key=None,
         )
```

### Comparing `gpt_json-0.4.2/gpt_json/tests/test_transformations.py` & `gpt_json-0.5.0/gpt_json/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/tests/test_truncation.py` & `gpt_json-0.5.0/gpt_json/tests/test_truncation.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,159 +4,160 @@
 from pydantic import BaseModel
 
 from gpt_json.gpt import GPTJSON
 from gpt_json.models import (
     GPTMessage,
     GPTMessageRole,
     GPTModelVersion,
+    TextContent,
     TruncationOptions,
     VariableTruncationMode,
 )
-from gpt_json.truncation import num_tokens_from_messages, truncate_tokens
-
-
-@pytest.mark.parametrize("model", [model.value for model in GPTModelVersion])
-def test_num_tokens_implemented(model):
-    # no need to assert anything specific, just that its implemented for all models
-    # i.e. doesn't throw an error
-    num_tokens_from_messages([], model)
+from gpt_json.truncation import truncate_tokens
 
 
 def test_fill_messages_truncated():
     class TestSchema(BaseModel):
         summary: str
 
-    gpt = GPTJSON[TestSchema](None)
+    gpt = GPTJSON[TestSchema](api_key="TEST")
     assert gpt.fill_messages(
         [
-            GPTMessage(role=GPTMessageRole.SYSTEM, content="system"),
+            GPTMessage(
+                role=GPTMessageRole.SYSTEM, content=[TextContent(text="system")]
+            ),
             GPTMessage(
                 role=GPTMessageRole.USER,
-                content="some long text: {long_text}",
+                content=[TextContent(text="some long text: {long_text}")],
             ),
         ],
         dict(
             long_text="hello world goodbye world",
         ),
         truncation_options=TruncationOptions(
             target_variable="long_text",
-            max_prompt_tokens=20,
+            max_prompt_tokens=8,
             truncation_mode=VariableTruncationMode.BEGINNING,
         ),
         max_response_tokens=None,
     ) == [
-        GPTMessage(role=GPTMessageRole.SYSTEM, content="system"),
-        GPTMessage(role=GPTMessageRole.USER, content="some long text: hello world"),
+        GPTMessage(role=GPTMessageRole.SYSTEM, content=[TextContent(text="system")]),
+        GPTMessage(
+            role=GPTMessageRole.USER,
+            content=[TextContent(text="some long text: hello world")],
+        ),
     ]
 
 
 def test_fill_messages_truncated_failure_case():
     class TestSchema(BaseModel):
         summary: str
 
-    gpt = GPTJSON[TestSchema](None)
+    gpt = GPTJSON[TestSchema](api_key="TEST")
 
     # this should fail because the max_prompt_tokens is too small
     with pytest.raises(ValueError, match=".* max_prompt_tokens .* too small .*"):
         gpt.fill_messages(
             [
-                GPTMessage(role=GPTMessageRole.SYSTEM, content="system"),
+                GPTMessage(
+                    role=GPTMessageRole.SYSTEM, content=[TextContent(text="system")]
+                ),
                 GPTMessage(
                     role=GPTMessageRole.USER,
-                    content="{long_text}",
+                    content=[TextContent(text="{long_text}")],
                 ),
             ],
             dict(
                 long_text="hello world goodbye world",
             ),
             truncation_options=TruncationOptions(
                 target_variable="long_text",
-                max_prompt_tokens=2,
+                max_prompt_tokens=1,
                 truncation_mode=VariableTruncationMode.BEGINNING,
             ),
             max_response_tokens=None,
         )
 
 
 def test_token_truncation_end_mode():
     assert (
         truncate_tokens(
             "hello world goodbye world world",
-            GPTModelVersion.GPT_3_5.value,
+            GPTModelVersion.GPT_3_5.value.api_name,
             VariableTruncationMode.BEGINNING,
             2,
         )
         == "hello world"
     )
 
 
 def test_token_truncation_beginning_mode():
     assert (
         truncate_tokens(
             "hello world world goodbye world",
-            GPTModelVersion.GPT_3_5.value,
+            GPTModelVersion.GPT_3_5.value.api_name,
             VariableTruncationMode.TRAILING,
             2,
         )
         == " goodbye world"
     )
 
 
 def test_token_truncation_middle_mode():
     assert (
         truncate_tokens(
             "hello world goodbye world world",
-            GPTModelVersion.GPT_3_5.value,
+            GPTModelVersion.GPT_3_5.value.api_name,
             VariableTruncationMode.MIDDLE,
             1,
         )
         == " goodbye"
     )
 
     assert (
         truncate_tokens(
             "hello world goodbye world world",
-            GPTModelVersion.GPT_3_5.value,
+            GPTModelVersion.GPT_3_5.value.api_name,
             VariableTruncationMode.MIDDLE,
             2,
         )
         == " world goodbye"
     )
 
     assert (
         truncate_tokens(
             "hello world goodbye world world",
-            GPTModelVersion.GPT_3_5.value,
+            GPTModelVersion.GPT_3_5.value.api_name,
             VariableTruncationMode.MIDDLE,
             3,
         )
         == " world goodbye world"
     )
 
 
 def test_token_truncation_random_mode():
     random.seed(1)
     assert (
         truncate_tokens(
             "hello world goodbye world",
-            GPTModelVersion.GPT_3_5.value,
+            GPTModelVersion.GPT_3_5.value.api_name,
             VariableTruncationMode.RANDOM,
             2,
         )
         == "hello world"
     )
 
 
 def test_token_truncation_custom_mode():
     def _custom_truncate(text_prev):
         return " | ".join(text_prev.split(" | ")[:-1])
 
     assert (
         truncate_tokens(
             "hello | world | goodbye | world | world",
-            GPTModelVersion.GPT_3_5.value,
+            GPTModelVersion.GPT_3_5.value.api_name,
             VariableTruncationMode.CUSTOM,
             3,
             _custom_truncate,
         )
         == "hello | world"
     )
```

### Comparing `gpt_json-0.4.2/gpt_json/tests/utils/streaming_utils.py` & `gpt_json-0.5.0/gpt_json/tests/utils/streaming_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/tests/utils/test_streaming_utils.py` & `gpt_json-0.5.0/gpt_json/tests/utils/test_streaming_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/gpt_json/transformations.py` & `gpt_json-0.5.0/gpt_json/transformations.py`

 * *Files identical despite different names*

### Comparing `gpt_json-0.4.2/pyproject.toml` & `gpt_json-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "gpt-json"
-version = "0.4.2"
+version = "0.5.0"
 description = "Structured and typehinted GPT responses in Python."
 authors = ["Pierce Freeman <pierce@freeman.vc>"]
 readme = "README.md"
 packages = [{ include = "gpt_json" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 tiktoken = "^0.3.3"
-openai = "^0.27.6"
+openai = "^1.16.2"
 pydantic = ">2.0.0, <3.0.0"
 backoff = "^2.2.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 isort = "^5.12.0"
 pytest-asyncio = "^0.21.0"
 autoflake = "^2.1.1"
 black = "^23.3.0"
 mypy = "^1.3.0"
 types-setuptools = "^68.1.0.0"
+pytest-httpx = "^0.30.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 check_untyped_defs = true
```

### Comparing `gpt_json-0.4.2/PKG-INFO` & `gpt_json-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-Metadata-Version: 2.1
-Name: gpt-json
-Version: 0.4.2
-Summary: Structured and typehinted GPT responses in Python.
-Author: Pierce Freeman
-Author-email: pierce@freeman.vc
-Requires-Python: >=3.11,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: openai (>=0.27.6,<0.28.0)
-Requires-Dist: pydantic (>2.0.0,<3.0.0)
-Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
-Description-Content-Type: text/markdown
-
 # gpt-json
 
 `gpt-json` is a wrapper around GPT that allows for declarative definition of expected output format. Set up a schema, write a prompt, and get results back as beautiful typehinted objects.
 
-Specifically this library:
-- Utilizes Pydantic schema definitions for type casting and validations
-- Adds typehinting for both the API and the output schema
-- Allows GPT to respond with both single-objects and lists of objects
-- Includes some lightweight transformations of the output to remove superfluous context and fix broken json
-- Includes retry logic for the most common API failures
-- Formats the JSON schema as a flexible prompt that can be added into any message
-- Supports templating of prompts to allow for dynamic content
-- Validate typehinted function calls in the new GPT models, to better support agent creation
+This library introduces the following features:
+
+- 🏗️ Pydantic schema definitions for type casting and validations
+- 🧵 Templating of prompts to allow for dynamic content
+- 🔎 Supports Vision API, Function Calling, and standard chat prompts
+- 🚕 Lightweight transformations of the output to fix broken json
+- ♻️ Retry logic for the most common API failures
+- 📋 Predict single-objects and lists of objects
+- ✈️ Lightweight dependencies: only OpenAI, pydantic, and backoff
 
 ## Getting Started
 
 ```bash
 pip install gpt-json
 ```
 
@@ -209,27 +193,27 @@
 `InvalidFunctionResponse` - The function name is incorrect.
 `InvalidFunctionParameters` - The function name is correct, but doesn't match the input schema that was provided.
 
 ## Other Configurations
 
 The `GPTJSON` class supports other configuration parameters at initialization.
 
-| Parameter                   | Type                   | Description                                                                                                                                                                            |
-|-----------------------------|------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| model                       | GPTModelVersion \| str | (default: GPTModelVersion.GPT_4) - For convenience we provide the currently supported GPT model versions in the `GPTModelVersion` enum. You can also pass a string value if you want to use another more specific architecture.                                                                                                                                                       |
-| auto_trim                   | bool                   | (default: False) - If your input prompt is too long, perhaps because of dynamic injected content, will automatically truncate the text to create enough room for the model's response. |
-| auto_trim_response_overhead | int                    | (default: 0) - If you're using auto_trim, configures the max amount of tokens to allow in the model's response.                                                                        |
-| **kwargs | Any | Any other parameters you want to pass to the underlying `GPT` class, will just be a passthrough. |
+| Parameter                   | Type                   | Description                                                                                                                                                                                                                     |
+| --------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| model                       | GPTModelVersion \| str | (default: GPTModelVersion.GPT_4) - For convenience we provide the currently supported GPT model versions in the `GPTModelVersion` enum. You can also pass a string value if you want to use another more specific architecture. |
+| auto_trim                   | bool                   | (default: False) - If your input prompt is too long, perhaps because of dynamic injected content, will automatically truncate the text to create enough room for the model's response.                                          |
+| auto_trim_response_overhead | int                    | (default: 0) - If you're using auto_trim, configures the max amount of tokens to allow in the model's response.                                                                                                                 |
+| \*\*kwargs                  | Any                    | Any other parameters you want to pass to the underlying `GPT` class, will just be a passthrough.                                                                                                                                |
 
 ## Transformations
 
 GPT (especially GPT-4) is relatively good at formatting responses at JSON, but it's not perfect. Some of the more common issues are:
 
-- *Response truncation*: Since GPT is not internally aware of its response length limit, JSON payloads will sometimes exhaust the available token space. This results in a broken JSON payload where much of the data is valid but the JSON object is not closed, which is not valid syntax. There are many cases where this behavior is actually okay for production applications - for instance, if you list 100 generated strings, it's sometimes okay for you to take the 70 that actually rendered. In this case, `gpt-json` will attempt to fix the truncated payload by recreating the JSON object and closing it.
-- *Boolean variables*: GPT will sometimes confuse valid JSON boolean values with the boolean tokens that are used in other languages. The most common is generating `True` instead of `true`. `gpt-json` will attempt to fix these values.
+- _Response truncation_: Since GPT is not internally aware of its response length limit, JSON payloads will sometimes exhaust the available token space. This results in a broken JSON payload where much of the data is valid but the JSON object is not closed, which is not valid syntax. There are many cases where this behavior is actually okay for production applications - for instance, if you list 100 generated strings, it's sometimes okay for you to take the 70 that actually rendered. In this case, `gpt-json` will attempt to fix the truncated payload by recreating the JSON object and closing it.
+- _Boolean variables_: GPT will sometimes confuse valid JSON boolean values with the boolean tokens that are used in other languages. The most common is generating `True` instead of `true`. `gpt-json` will attempt to fix these values.
 
 When calling `gpt_json.run()`, we return a tuple of values:
 
 ```python
 payload = await gpt_json.run(...)
 
 print(transformations.fix_transforms)
@@ -237,15 +221,15 @@
 
 ```bash
 FixTransforms(fixed_truncation=True, fixed_bools=False)
 ```
 
 The first object is your generated Pydantic model. The second object is our correction storage object `FixTransforms`. This dataclass contains flags for each of the supported transformation cases that are sketched out above. This allows you to determine whether the response was explicitly parsed from the GPT JSON, or was passed through some middlelayers to get a correct output. From there you can accept or reject the response based on your own business logic.
 
-*Where you can help*: There are certainly more areas of common (and not-so-common failures). If you see these, please add a test case to the unit tests. If you can write a handler to help solve the general case, please do so. Otherwise flag it as a `pytest.xfail` and we'll add it to the backlog.
+_Where you can help_: There are certainly more areas of common (and not-so-common failures). If you see these, please add a test case to the unit tests. If you can write a handler to help solve the general case, please do so. Otherwise flag it as a `pytest.xfail` and we'll add it to the backlog.
 
 ## Testing
 
 We use poetry for package management. To run the bundled tests, clone the package from github.
 
 ```bash
 poetry install
@@ -265,8 +249,7 @@
 We use black and mypy for formatting. You can set up a pre-commit git hook to do this automatically via the `./lint.sh` helper file.
 
 If you perform a bulk reformatting to the codebase, you should add your most recent commit to the `.git-blame-ignore-revs` file and run:
 
 ```
 git config blame.ignoreRevsFile .git-blame-ignore-revs
 ```
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

