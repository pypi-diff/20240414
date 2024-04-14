# Comparing `tmp/tool_use-0.0.9.tar.gz` & `tmp/tool_use-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_use-0.0.9.tar", last modified: Sun Mar 17 15:23:50 2024, max compression
+gzip compressed data, was "tool_use-0.1.0.tar", last modified: Sun Apr 14 06:26:36 2024, max compression
```

## Comparing `tool_use-0.0.9.tar` & `tool_use-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-03-17 15:23:50.691623 tool_use-0.0.9/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.0.9/MANIFEST.in
--rw-r--r--   0 kimjaemin   (501) staff       (20)       86 2024-03-17 15:23:50.691413 tool_use-0.0.9/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      237 2024-03-17 15:10:50.000000 tool_use-0.0.9/README.md
--rw-r--r--   0 kimjaemin   (501) staff       (20)      389 2024-03-17 15:23:28.000000 tool_use-0.0.9/pyproject.toml
--rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-03-17 15:23:50.691667 tool_use-0.0.9/setup.cfg
--rw-r--r--   0 kimjaemin   (501) staff       (20)      408 2024-03-17 15:21:21.000000 tool_use-0.0.9/setup.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-03-17 15:23:50.689509 tool_use-0.0.9/tests/
--rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.0.9/tests/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)      697 2024-03-17 15:07:20.000000 tool_use-0.0.9/tests/test_openai_tool_use.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-03-17 15:23:50.689641 tool_use-0.0.9/tool_use/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.0.9/tool_use/__init__.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-03-17 15:23:50.690852 tool_use-0.0.9/tool_use/tools/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.0.9/tool_use/tools/__init__.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)    19938 2024-03-17 15:08:27.000000 tool_use-0.0.9/tool_use/tools/openai_tool_use.py
--rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.0.9/tool_use/tools/utils.py
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-03-17 15:23:50.691006 tool_use-0.0.9/tool_use/yamls/
--rw-r--r--   0 kimjaemin   (501) staff       (20)     1452 2024-03-17 15:23:01.000000 tool_use-0.0.9/tool_use/yamls/openai_tool_use.yaml
-drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-03-17 15:23:50.691190 tool_use-0.0.9/tool_use.egg-info/
--rw-r--r--   0 kimjaemin   (501) staff       (20)       86 2024-03-17 15:23:50.000000 tool_use-0.0.9/tool_use.egg-info/PKG-INFO
--rw-r--r--   0 kimjaemin   (501) staff       (20)      398 2024-03-17 15:23:50.000000 tool_use-0.0.9/tool_use.egg-info/SOURCES.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-03-17 15:23:50.000000 tool_use-0.0.9/tool_use.egg-info/dependency_links.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)       74 2024-03-17 15:23:50.000000 tool_use-0.0.9/tool_use.egg-info/entry_points.txt
--rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-03-17 15:23:50.000000 tool_use-0.0.9/tool_use.egg-info/top_level.txt
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.122943 tool_use-0.1.0/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       30 2024-03-17 15:07:20.000000 tool_use-0.1.0/MANIFEST.in
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      106 2024-04-14 06:26:36.122681 tool_use-0.1.0/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      265 2024-04-14 06:25:21.000000 tool_use-0.1.0/README.md
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      532 2024-04-14 06:26:15.000000 tool_use-0.1.0/pyproject.toml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       38 2024-04-14 06:26:36.123015 tool_use-0.1.0/setup.cfg
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      527 2024-04-14 05:56:49.000000 tool_use-0.1.0/setup.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.119863 tool_use-0.1.0/tests/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        0 2024-02-06 11:51:51.000000 tool_use-0.1.0/tests/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     2812 2024-04-14 06:22:21.000000 tool_use-0.1.0/tests/test_anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1235 2024-04-08 11:36:45.000000 tool_use-0.1.0/tests/test_exception.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1016 2024-04-14 05:56:49.000000 tool_use-0.1.0/tests/test_openai_tool_use.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.120037 tool_use-0.1.0/tool_use/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.0/tool_use/__init__.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.121754 tool_use-0.1.0/tool_use/tools/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       81 2024-02-06 11:51:51.000000 tool_use-0.1.0/tool_use/tools/__init__.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    16672 2024-04-14 06:22:21.000000 tool_use-0.1.0/tool_use/tools/anthropic_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)    22455 2024-04-14 06:13:17.000000 tool_use-0.1.0/tool_use/tools/openai_tool_use.py
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      537 2024-03-17 15:07:20.000000 tool_use-0.1.0/tool_use/tools/utils.py
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.122131 tool_use-0.1.0/tool_use/yamls/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      918 2024-04-14 05:35:46.000000 tool_use-0.1.0/tool_use/yamls/anthropic_tool_use.yaml
+-rw-r--r--   0 kimjaemin   (501) staff       (20)     1512 2024-04-08 11:29:56.000000 tool_use-0.1.0/tool_use/yamls/openai_tool_use.yaml
+drwxr-xr-x   0 kimjaemin   (501) staff       (20)        0 2024-04-14 06:26:36.122377 tool_use-0.1.0/tool_use.egg-info/
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      106 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/PKG-INFO
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      531 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/SOURCES.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)        1 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/dependency_links.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)      135 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/entry_points.txt
+-rw-r--r--   0 kimjaemin   (501) staff       (20)       15 2024-04-14 06:26:36.000000 tool_use-0.1.0/tool_use.egg-info/top_level.txt
```

### Comparing `tool_use-0.0.9/tool_use/tools/openai_tool_use.py` & `tool_use-0.1.0/tool_use/tools/openai_tool_use.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,48 @@
+import asyncio
 import functools
 import inspect
 import json
 import re
-import sys
 import time
 from ast import literal_eval
 from enum import Enum
-from typing import List, Optional, TypedDict, cast
+from typing import List, Optional, cast
 
 from openai import (
     APIConnectionError,
     APIStatusError,
     APITimeoutError,
     OpenAIError,
     RateLimitError,
 )
+from openai.types.chat.chat_completion_named_tool_choice_param import (
+    ChatCompletionNamedToolChoiceParam,
+)
+from openai.types.chat.chat_completion_tool_param import ChatCompletionToolParam
 from promptflow import tool
 from promptflow.connections import AzureOpenAIConnection, OpenAIConnection
 from promptflow.contracts.types import PromptTemplate
 from promptflow.exceptions import SystemErrorException, UserErrorException
 from promptflow.tools.common import (
     generate_retry_interval,
     normalize_connection_config,
-    post_process_chat_api_response,
     process_function_call,
     render_jinja_template,
     to_bool,
     to_content_str_or_list,
     try_parse_name_and_content,
     validate_functions,
     validate_role,
 )
 from promptflow.tools.exception import (
     ChatAPIFunctionRoleInvalidFormat,
     ChatAPIInvalidFunctions,
     ExceedMaxRetryTimes,
+    FunctionCallNotSupportedInStreamMode,
     LLMError,
     WrappedOpenAIError,
 )
 
 try:
     from openai import AsyncAzureOpenAI as AzureOpenAIClient
     from openai import AsyncOpenAI as OpenAIClient
@@ -54,36 +58,46 @@
     GPT_35_TURBO_1106 = "gpt-3.5-turbo-1106"
     GPT_35_TURBO_0125 = "gpt-3.5-turbo-0125"
     GPT_35_TURBO_16K_0613 = "gpt-3.5-turbo-16k-0613"
     GPT_35_TURBO_INSTRUCT = "gpt-3.5-turbo-instruct"
     GPT_35_TURBO_INSTRUCT_0914 = "gpt-3.5-turbo-instruct-0914"
     GPT_4_0125_PREVIEW = "gpt-4-0125-preview"
     GPT_4_1106_PREVIEW = "gpt-4-1106-preview"
-    GPT_4_VISION_PREVIEW = "gpt-4-vision-preview"
+    GPT_4_1106_VISION_PREVIEW = "gpt-4-1106-vision-preview"
+    GPT_4_240409 = "gpt-4-turbo-2024-04-09"
     GPT_4_0613 = "gpt-4-0613"
 
 
-class ToolFunctionDict(TypedDict):
-    parameters: object
-    description: str
-    name: str
-
-
-class ToolDict(TypedDict):
-    type: str
-    function: ToolFunctionDict
-
-
-class ToolChoiceFunctionDict(TypedDict):
-    name: str
-
-
-class ToolChoiceDict(TypedDict):
-    type: str
-    function: ToolChoiceFunctionDict
+class CompletionNoneExceptionFlag:
+    def __init__(self) -> None:
+        self._flag = False
+
+    def set_flag_true(self) -> None:
+        self._flag = True
+
+    def get_flag(self) -> bool:
+        return self._flag
+
+
+class CompletionNoneException(Exception):
+    """Exception raised when openai completion object is None."""
+
+    def __init__(self) -> None:
+        super().__init__("openai completion object is None.")
+
+    def is_first_exception(self, flag: CompletionNoneExceptionFlag) -> bool:
+        """
+        If flag is false, set flag as true and return true.
+        If flag is true, return false.
+        """
+        if not flag.get_flag():
+            flag.set_flag_true()
+            return True
+        else:
+            return False
 
 
 def _try_parse_tool_message(role_prompt):
     # customer can add ## in front of name/content for markdown highlight.
     # and we still support name/content without ## prefix for backward compatibility.
     pattern = r"\n*#{0,2}\s*tool_call_id:\n+\s*(\S+)\s*\n*#{0,2}\s*content:\n?(.*)"
     match = re.search(pattern, role_prompt, re.DOTALL)
@@ -175,222 +189,260 @@
             role = chunk.strip().lower()
             validate_role(role, valid_roles=valid_roles)
             new_message = {"role": role}
             chat_list.append(new_message)
     return chat_list
 
 
-# TODO(2971352): revisit this tries=100 when there is any change to the 10min timeout logic
-def handle_openai_error(tries: int = 100):
+# TODO(2971352): revisit this tries=5 when there is any change to the 10min timeout logic
+def handle_openai_error(tries: int = 5):
     """
     A decorator function that used to handle OpenAI error.
     OpenAI Error falls into retriable vs non-retriable ones.
 
     For retriable error, the decorator use below parameters to control its retry activity with exponential backoff:
      `tries` : max times for the function invocation, type is int
      'delay': base delay seconds for exponential delay, type is float
     """
 
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
+            flag = CompletionNoneExceptionFlag()
             for i in range(tries + 1):
                 try:
                     return func(*args, **kwargs)
                 except (SystemErrorException, UserErrorException) as e:
                     # Throw inner wrapped exception directly
                     raise e
                 except (APIStatusError, APIConnectionError) as e:
                     #  Handle retriable exception, please refer to
                     #  https://platform.openai.com/docs/guides/error-codes/api-errors
-                    print(
-                        f"Exception occurs: {type(e).__name__}: {str(e)}",
-                        file=sys.stderr,
-                    )
+                    # print(
+                    #     f"Exception occurs: {type(e).__name__}: {str(e)}",
+                    #     file=sys.stderr,
+                    # )
                     if (
                         isinstance(e, APIConnectionError)
                         and not isinstance(e, APITimeoutError)
                         and "connection aborted" not in str(e).lower()
                     ):
                         raise WrappedOpenAIError(e)
                     # Retry InternalServerError(>=500), RateLimitError(429), UnprocessableEntityError(422)
                     if isinstance(e, APIStatusError):
                         status_code = e.response.status_code
-                        if status_code < 500 and status_code not in [429, 422]:
+                        if status_code < 500 and status_code not in [429]:
                             raise WrappedOpenAIError(e)
                     if (
                         isinstance(e, RateLimitError)
                         and getattr(e, "type", None) == "insufficient_quota"
                     ):
                         # Exit retry if this is quota insufficient error
-                        print(
-                            f"{type(e).__name__} with insufficient quota. Throw user error.",
-                            file=sys.stderr,
-                        )
+                        # print(
+                        #     f"{type(e).__name__} with insufficient quota. Throw user error.",
+                        #     file=sys.stderr,
+                        # )
                         raise WrappedOpenAIError(e)
                     if i == tries:
                         # Exit retry if max retry reached
-                        print(
-                            f"{type(e).__name__} reached max retry. Exit retry with user error.",
-                            file=sys.stderr,
-                        )
+                        # print(
+                        #     f"{type(e).__name__} reached max retry. Exit retry with user error.",
+                        #     file=sys.stderr,
+                        # )
                         raise ExceedMaxRetryTimes(e)
 
                     if hasattr(e, "response") and e.response is not None:
                         retry_after_in_header = e.response.headers.get(
                             "retry-after", None
                         )
                     else:
                         retry_after_in_header = None
 
                     if not retry_after_in_header:
                         retry_after_seconds = generate_retry_interval(i)
-                        msg = (
+                        (
                             f"{type(e).__name__} #{i}, but no Retry-After header, "
                             + f"Back off {retry_after_seconds} seconds for retry."
                         )
-                        print(msg, file=sys.stderr)
+                        # print(msg, file=sys.stderr)
                     else:
                         retry_after_seconds = float(retry_after_in_header)
-                        msg = (
+                        (
                             f"{type(e).__name__} #{i}, Retry-After={retry_after_in_header}, "
                             f"Back off {retry_after_seconds} seconds for retry."
                         )
-                        print(msg, file=sys.stderr)
+                        # print(msg, file=sys.stderr)
                     time.sleep(retry_after_seconds)
                 except OpenAIError as e:
                     # For other non-retriable errors from OpenAIError,
                     # For example, AuthenticationError, APIConnectionError, BadRequestError, NotFoundError
                     # Mark UserError for all the non-retriable OpenAIError
-                    print(
-                        f"Exception occurs: {type(e).__name__}: {str(e)}",
-                        file=sys.stderr,
-                    )
+                    # print(
+                    #     f"Exception occurs: {type(e).__name__}: {str(e)}",
+                    #     file=sys.stderr,
+                    # )
                     raise WrappedOpenAIError(e)
+                except CompletionNoneException as e:
+                    if e.is_first_exception(flag=flag):
+                        continue
+                    else:
+                        raise e
                 except Exception as e:
-                    print(
-                        f"Exception occurs: {type(e).__name__}: {str(e)}",
-                        file=sys.stderr,
-                    )
+                    # print(
+                    #     f"Exception occurs: {type(e).__name__}: {str(e)}",
+                    #     file=sys.stderr,
+                    # )
                     error_message = (
                         f"OpenAI API hits exception: {type(e).__name__}: {str(e)}"
                     )
                     raise LLMError(message=error_message)
 
         @functools.wraps(func)
         async def async_wrapper(*args, **kwargs):
+            flag = CompletionNoneExceptionFlag()
             for i in range(tries + 1):
                 try:
                     return await func(*args, **kwargs)
                 except (SystemErrorException, UserErrorException) as e:
                     # Throw inner wrapped exception directly
                     raise e
                 except (APIStatusError, APIConnectionError) as e:
                     #  Handle retriable exception, please refer to
                     #  https://platform.openai.com/docs/guides/error-codes/api-errors
-                    print(
-                        f"Exception occurs: {type(e).__name__}: {str(e)}",
-                        file=sys.stderr,
-                    )
+                    # print(
+                    #     f"Exception occurs: {type(e).__name__}: {str(e)}",
+                    #     file=sys.stderr,
+                    # )
                     if (
                         isinstance(e, APIConnectionError)
                         and not isinstance(e, APITimeoutError)
                         and "connection aborted" not in str(e).lower()
                     ):
                         raise WrappedOpenAIError(e)
-                    # Retry InternalServerError(>=500), RateLimitError(429), UnprocessableEntityError(422)
+                    # Retry InternalServerError(>=500), RateLimitError(429)
                     if isinstance(e, APIStatusError):
                         status_code = e.response.status_code
-                        if status_code < 500 and status_code not in [429, 422]:
+                        if status_code < 500 and status_code not in [429]:
                             raise WrappedOpenAIError(e)
                     if (
                         isinstance(e, RateLimitError)
                         and getattr(e, "type", None) == "insufficient_quota"
                     ):
                         # Exit retry if this is quota insufficient error
-                        print(
-                            f"{type(e).__name__} with insufficient quota. Throw user error.",
-                            file=sys.stderr,
-                        )
+                        # print(
+                        #     f"{type(e).__name__} with insufficient quota. Throw user error.",
+                        #     file=sys.stderr,
+                        # )
                         raise WrappedOpenAIError(e)
                     if i == tries:
                         # Exit retry if max retry reached
-                        print(
-                            f"{type(e).__name__} reached max retry. Exit retry with user error.",
-                            file=sys.stderr,
-                        )
+                        # print(
+                        #     f"{type(e).__name__} reached max retry. Exit retry with user error.",
+                        #     file=sys.stderr,
+                        # )
                         raise ExceedMaxRetryTimes(e)
 
                     if hasattr(e, "response") and e.response is not None:
                         retry_after_in_header = e.response.headers.get(
                             "retry-after", None
                         )
                     else:
                         retry_after_in_header = None
 
                     if not retry_after_in_header:
                         retry_after_seconds = generate_retry_interval(i)
-                        msg = (
+                        (
                             f"{type(e).__name__} #{i}, but no Retry-After header, "
                             + f"Back off {retry_after_seconds} seconds for retry."
                         )
-                        print(msg, file=sys.stderr)
+                        # print(msg, file=sys.stderr)
                     else:
                         retry_after_seconds = float(retry_after_in_header)
-                        msg = (
+                        (
                             f"{type(e).__name__} #{i}, Retry-After={retry_after_in_header}, "
                             f"Back off {retry_after_seconds} seconds for retry."
                         )
-                        print(msg, file=sys.stderr)
-                    time.sleep(retry_after_seconds)
+                        # print(msg, file=sys.stderr)
+                    await asyncio.sleep(retry_after_seconds)
                 except OpenAIError as e:
                     # For other non-retriable errors from OpenAIError,
                     # For example, AuthenticationError, APIConnectionError, BadRequestError, NotFoundError
                     # Mark UserError for all the non-retriable OpenAIError
-                    print(
-                        f"Exception occurs: {type(e).__name__}: {str(e)}",
-                        file=sys.stderr,
-                    )
+                    # print(
+                    #     f"Exception occurs: {type(e).__name__}: {str(e)}",
+                    #     file=sys.stderr,
+                    # )
                     raise WrappedOpenAIError(e)
+                except CompletionNoneException as e:
+                    if e.is_first_exception(flag=flag):
+                        continue
+                    else:
+                        raise e
                 except Exception as e:
-                    print(
-                        f"Exception occurs: {type(e).__name__}: {str(e)}",
-                        file=sys.stderr,
-                    )
+                    # print(
+                    #     f"Exception occurs: {type(e).__name__}: {str(e)}",
+                    #     file=sys.stderr,
+                    # )
                     error_message = (
                         f"OpenAI API hits exception: {type(e).__name__}: {str(e)}"
                     )
                     raise LLMError(message=error_message)
 
         return wrapper if not inspect.iscoroutinefunction(func) else async_wrapper
 
     return decorator
 
 
+def async_post_process_chat_api_response(completion, stream, functions):
+    if stream:
+        if functions is not None:
+            error_message = (
+                "Function calling has not been supported by stream mode yet."
+            )
+            raise FunctionCallNotSupportedInStreamMode(message=error_message)
+
+        async def generator():
+            async for chunk in completion:
+                if chunk.choices:
+                    yield chunk.choices[0].delta.content if hasattr(
+                        chunk.choices[0].delta, "content"
+                    ) and chunk.choices[0].delta.content is not None else ""
+
+        return generator()
+    else:
+        # When calling function, function_call response will be returned as a field in message, so we need return
+        # message directly. Otherwise, we only return content.
+        if functions is not None:
+            return completion.model_dump()["choices"][0]["message"]
+        else:
+            # chat api may return message with no content.
+            return getattr(completion.choices[0].message, "content", "")
+
+
 @tool
 @handle_openai_error()
 async def openai_tool_use(
     connection: OpenAIConnection | AzureOpenAIConnection,
     prompt: PromptTemplate,
     model: ModelEnum,
     temperature: float = 1,
     top_p: float = 1,
     n: int = 1,
-    stream: bool = False,
+    stream: Optional[bool] = False,
     stop: Optional[list] = None,  # type: ignore
     max_tokens: Optional[int] = None,  # type: ignore
     presence_penalty: float = 0,
     frequency_penalty: float = 0,
     logit_bias: dict = {},
     user: Optional[str] = "",
     function_call: Optional[object] = None,
     functions: Optional[list] = None,  # type: ignore
     response_format: object = dict(type="text"),
-    tools: Optional[list[ToolDict]] = None,  # type: ignore
-    tool_choice: Optional[str] = None,  # type: ignore
+    tools: Optional[list[ChatCompletionToolParam]] = None,  # type: ignore
+    tool_choice: Optional[ChatCompletionNamedToolChoiceParam | str] = None,  # type: ignore
     extra_headers: Optional[dict] = {},
     is_raw_output: Optional[bool] = False,
     **kwargs,
 ) -> [str, dict]:  # type: ignore
     chat_str = render_jinja_template(
         prompt, trim_blocks=True, keep_trailing_newline=True, **kwargs
     )
@@ -419,15 +471,15 @@
         validate_functions(functions)
         params["functions"] = functions
         params["function_call"] = process_function_call(function_call)
 
     if tools is not None:
         functions = []
         for tool_desc in tools:
-            tool_desc = cast(ToolDict, tool_desc)
+            tool_desc = cast(ChatCompletionToolParam, tool_desc)
             if "type" in tool_desc and "function" in tool_desc:
                 functions.append(tool_desc["function"])
             else:
                 raise ChatAPIInvalidFunctions(
                     message=f"tools parameter is invalid: {tools}"
                 )
         validate_functions(functions)
@@ -439,15 +491,17 @@
         else:
             try:
                 tool_choice_dict = json.loads(tool_choice)
             except Exception:
                 raise ChatAPIInvalidFunctions(
                     message=f"tool_choice parameter is invalid: {tool_choice}"
                 )
-            tool_choice_dict = cast(ToolChoiceDict, tool_choice_dict)
+            tool_choice_dict = cast(
+                ChatCompletionNamedToolChoiceParam, tool_choice_dict
+            )
             if "type" not in tool_choice_dict or "function" not in tool_choice_dict:
                 raise ChatAPIInvalidFunctions(
                     message=f"tool_choice parameter is invalid: {tool_choice_dict}"
                 )
             else:
                 if "name" not in tool_choice_dict["function"]:
                     raise ChatAPIInvalidFunctions(
@@ -461,12 +515,16 @@
         OpenAIClient(**_connection_dict)
         if isinstance(connection, OpenAIConnection)
         else AzureOpenAIClient(**_connection_dict)
     )
     completion = await _client.chat.completions.create(
         **params, extra_headers=extra_headers
     )
+
+    if completion is None:
+        raise CompletionNoneException()
+
     return (
-        post_process_chat_api_response(completion, stream, functions)
+        async_post_process_chat_api_response(completion, stream, functions)
         if not is_raw_output
         else completion
     )
```

### Comparing `tool_use-0.0.9/tool_use/tools/utils.py` & `tool_use-0.1.0/tool_use/tools/utils.py`

 * *Files identical despite different names*

### Comparing `tool_use-0.0.9/tool_use/yamls/openai_tool_use.yaml` & `tool_use-0.1.0/tool_use/yamls/openai_tool_use.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -73,9 +73,13 @@
       type:
         - object
       optional: true
     is_raw_output:
       type:
         - bool
       optional: true
+    stream:
+      type:
+        - bool
+      optional: true
   module: tool_use.tools.openai_tool_use
   function: openai_tool_use
```

