# Comparing `tmp/instructor-1.0.3.tar.gz` & `tmp/instructor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.0.3.tar", max compression
+gzip compressed data, was "instructor-1.1.0.tar", max compression
```

## Comparing `instructor-1.0.3.tar` & `instructor-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-04-05 13:30:03.247179 instructor-1.0.3/LICENSE
--rw-r--r--   0        0        0     8979 2024-04-05 13:30:03.247179 instructor-1.0.3/README.md
--rw-r--r--   0        0        0     1185 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6494 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/cli/usage.py
--rw-r--r--   0        0        0     9586 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/client.py
--rw-r--r--   0        0        0     1712 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/client_anthropic.py
--rw-r--r--   0        0        0     1335 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/client_groq.py
--rw-r--r--   0        0        0     8968 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2642 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11016 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1733 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4381 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/exceptions.py
--rw-r--r--   0        0        0     7339 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/function_calls.py
--rw-r--r--   0        0        0      818 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/mode.py
--rw-r--r--   0        0        0     4820 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/patch.py
--rw-r--r--   0        0        0    12534 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/py.typed
--rw-r--r--   0        0        0     6171 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/retry.py
--rw-r--r--   0        0        0     4373 2024-04-05 13:30:03.311180 instructor-1.0.3/instructor/utils.py
--rw-r--r--   0        0        0     2154 2024-04-05 13:30:03.315180 instructor-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    10662 1970-01-01 00:00:00.000000 instructor-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-11 18:17:53.874332 instructor-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8979 2024-04-11 18:17:53.874332 instructor-1.1.0/README.md
+-rw-r--r--   0        0        0     1185 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3792 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/cli/files.py
+-rw-r--r--   0        0        0     5348 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8255 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6494 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/cli/usage.py
+-rw-r--r--   0        0        0     9586 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/client.py
+-rw-r--r--   0        0        0     2062 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     1335 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/client_groq.py
+-rw-r--r--   0        0        0     8968 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2985 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     7929 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2165 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2642 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    11016 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1733 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4381 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/exceptions.py
+-rw-r--r--   0        0        0     7339 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/function_calls.py
+-rw-r--r--   0        0        0      818 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/mode.py
+-rw-r--r--   0        0        0     4820 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/patch.py
+-rw-r--r--   0        0        0    12534 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/py.typed
+-rw-r--r--   0        0        0     7317 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/retry.py
+-rw-r--r--   0        0        0     4642 2024-04-11 18:17:53.942332 instructor-1.1.0/instructor/utils.py
+-rw-r--r--   0        0        0     2158 2024-04-11 18:17:53.946332 instructor-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10651 1970-01-01 00:00:00.000000 instructor-1.1.0/PKG-INFO
```

### Comparing `instructor-1.0.3/LICENSE` & `instructor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/README.md` & `instructor-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/__init__.py` & `instructor-1.1.0/instructor/__init__.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/_types/_alias.py` & `instructor-1.1.0/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/cli/cli.py` & `instructor-1.1.0/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/cli/files.py` & `instructor-1.1.0/instructor/cli/files.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/cli/hub.py` & `instructor-1.1.0/instructor/cli/hub.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/cli/jobs.py` & `instructor-1.1.0/instructor/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/cli/usage.py` & `instructor-1.1.0/instructor/cli/usage.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/client.py` & `instructor-1.1.0/instructor/client.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/client_anthropic.py` & `instructor-1.1.0/instructor/client_anthropic.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,51 +2,59 @@
 import instructor
 
 from typing import overload
 
 
 @overload
 def from_anthropic(
-    client: anthropic.Anthropic,
+    client: anthropic.Anthropic | anthropic.AnthropicBedrock,
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
     **kwargs,
 ) -> instructor.Instructor: ...
 
 
 @overload
 def from_anthropic(
-    client: anthropic.AsyncAnthropic,
+    client: anthropic.AsyncAnthropic | anthropic.AsyncAnthropicBedrock,
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
     **kwargs,
 ) -> instructor.Instructor: ...
 
 
 def from_anthropic(
-    client: anthropic.Anthropic | anthropic.AsyncAnthropic,
+    client: (
+        anthropic.Anthropic
+        | anthropic.AsyncAnthropic
+        | anthropic.AnthropicBedrock
+        | anthropic.AsyncAnthropicBedrock
+    ),
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
     **kwargs,
 ) -> instructor.Instructor | instructor.AsyncInstructor:
-    assert (
-        mode
-        in {
-            instructor.Mode.ANTHROPIC_JSON,
-            instructor.Mode.ANTHROPIC_TOOLS,
-        }
-    ), "Mode be one of {instructor.Mode.ANTHROPIC_JSON, instructor.Mode.ANTHROPIC_TOOLS}"
+    assert mode in {
+        instructor.Mode.ANTHROPIC_JSON,
+        instructor.Mode.ANTHROPIC_TOOLS,
+    }, "Mode be one of {instructor.Mode.ANTHROPIC_JSON, instructor.Mode.ANTHROPIC_TOOLS}"
 
     assert isinstance(
-        client, (anthropic.Anthropic, anthropic.AsyncAnthropic)
-    ), "Client must be an instance of anthropic.Anthropic or anthropic.AsyncAnthropic"
+        client,
+        (
+            anthropic.Anthropic,
+            anthropic.AsyncAnthropic,
+            anthropic.AnthropicBedrock,
+            anthropic.AsyncAnthropicBedrock,
+        ),
+    ), "Client must be an instance of {anthropic.Anthropic, anthropic.AsyncAnthropic, anthropic.AnthropicBedrock, anthropic.AsyncAnthropicBedrock}"
 
     if mode == instructor.Mode.ANTHROPIC_TOOLS:
         create = client.beta.tools.messages.create
     else:
         create = client.messages.create
 
-    if isinstance(client, anthropic.Anthropic):
+    if isinstance(client, (anthropic.Anthropic, anthropic.AnthropicBedrock)):
         return instructor.Instructor(
             client=client,
             create=instructor.patch(create=create, mode=mode),
             provider=instructor.Provider.ANTHROPIC,
             mode=mode,
             **kwargs,
         )
```

### Comparing `instructor-1.0.3/instructor/client_groq.py` & `instructor-1.1.0/instructor/client_groq.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/distil.py` & `instructor-1.1.0/instructor/distil.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/dsl/citation.py` & `instructor-1.1.0/instructor/dsl/citation.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/dsl/iterable.py` & `instructor-1.1.0/instructor/dsl/iterable.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/dsl/maybe.py` & `instructor-1.1.0/instructor/dsl/maybe.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/dsl/parallel.py` & `instructor-1.1.0/instructor/dsl/parallel.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/dsl/partial.py` & `instructor-1.1.0/instructor/dsl/partial.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/dsl/simple_type.py` & `instructor-1.1.0/instructor/dsl/simple_type.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/dsl/validators.py` & `instructor-1.1.0/instructor/dsl/validators.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/function_calls.py` & `instructor-1.1.0/instructor/function_calls.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/mode.py` & `instructor-1.1.0/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/patch.py` & `instructor-1.1.0/instructor/patch.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/process_response.py` & `instructor-1.1.0/instructor/process_response.py`

 * *Files identical despite different names*

### Comparing `instructor-1.0.3/instructor/retry.py` & `instructor-1.1.0/instructor/retry.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,18 +25,43 @@
 T_Retval = TypeVar("T_Retval")
 T_ParamSpec = ParamSpec("T_ParamSpec")
 T = TypeVar("T")
 
 
 def reask_messages(response: ChatCompletion, mode: Mode, exception: Exception):
     if mode == Mode.ANTHROPIC_TOOLS:
-        # TODO: we need to include the original response
+        # The original response
+        assistant_content = []
+        tool_use_id = None
+        for content in response.content:
+            assistant_content.append(content.model_dump())
+            # Assuming exception from single tool invocation
+            if (
+                content.type == "tool_use"
+                and isinstance(exception, ValidationError)
+                and content.name == exception.title
+            ):
+                tool_use_id = content.id
+
+        assert tool_use_id is not None, "Tool use ID not found in the response"
+        yield {
+            "role": "assistant",
+            "content": assistant_content,
+        }
         yield {
             "role": "user",
-            "content": f"Validation Errors found:\n{exception}\nReca ll the function correctly, fix the errors from\n{response.content}",
+            "content": [
+                {
+                    "type": "tool_result",
+                    "tool_use_id": tool_use_id,
+                    "content": f"Validation Error found:\n{exception}\nRecall the function correctly, fix the errors",
+                    "is_error": True,
+                }
+            ],
+
         }
         return
     if mode == Mode.ANTHROPIC_JSON:
         from anthropic.types import Message
 
         assert isinstance(response, Message)
         yield {
@@ -103,15 +128,18 @@
                         validation_context=validation_context,
                         strict=strict,
                         mode=mode,
                     )
                 except (ValidationError, JSONDecodeError) as e:
                     logger.debug(f"Error response: {response}")
                     kwargs["messages"].extend(reask_messages(response, mode, e))
-                    kwargs["messages"] = merge_consecutive_messages(kwargs["messages"])
+                    if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
+                        kwargs["messages"] = merge_consecutive_messages(
+                            kwargs["messages"]
+                        )
                     raise e
     except RetryError as e:
         logger.exception(f"Failed after retries: {e.last_attempt.exception}")
         raise e.last_attempt.exception from e
 
 
 async def retry_async(
@@ -153,11 +181,15 @@
                         validation_context=validation_context,
                         strict=strict,
                         mode=mode,
                     )  # type: ignore[all]
                 except (ValidationError, JSONDecodeError) as e:
                     logger.debug(f"Error response: {response}", e)
                     kwargs["messages"].extend(reask_messages(response, mode, e))
+                    if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
+                        kwargs["messages"] = merge_consecutive_messages(
+                            kwargs["messages"]
+                        )
                     raise e
     except RetryError as e:
         logger.exception(f"Failed after retries: {e.last_attempt.exception}")
         raise e.last_attempt.exception from e
```

### Comparing `instructor-1.0.3/instructor/utils.py` & `instructor-1.1.0/instructor/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -122,13 +122,22 @@
     return is_coroutine
 
 
 def merge_consecutive_messages(messages: list[dict]) -> list[dict]:
     # merge all consecutive user messages into a single message
     new_messages = []
     for message in messages:
+        new_content = message["content"]
+        if isinstance(new_content, str):
+            new_content = [{"type": "text", "text": new_content}]
+
         if len(new_messages) > 0 and message["role"] == new_messages[-1]["role"]:
-            new_messages[-1]["content"] += f"\n\n{message['content']}"
+            new_messages[-1]["content"].extend(new_content)
         else:
-            new_messages.append(message)
+            new_messages.append(
+                {
+                    "role": message["role"],
+                    "content": new_content,
+                }
+            )
 
     return new_messages
```

### Comparing `instructor-1.0.3/pyproject.toml` & `instructor-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "instructor"
-version = "1.0.3"
+version = "1.1.0"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^1.1.0"
-pydantic = "^2.7.0b01"
+pydantic = "2.7.0"
 docstring-parser = "^0.15"
-typer = "^0.9.0"
+typer = ">=0.9.0,<1.0.0"
 rich = "^13.7.0"
 aiohttp = "^3.9.1"
 tenacity = "^8.2.3"
 pydantic-core = "^2.18.0"
 
 # dependency versions for extras
 fastapi = { version = "^0.109.2", optional = true }
```

### Comparing `instructor-1.0.3/PKG-INFO` & `instructor-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.0.3
+Version: 1.1.0
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,22 +20,22 @@
 Requires-Dist: diskcache (>=5.6.3,<6.0.0) ; extra == "test-docs"
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0) ; extra == "test-docs"
 Requires-Dist: groq (>=0.4.2,<0.5.0) ; extra == "groq" or extra == "test-docs"
 Requires-Dist: litellm (>=1.0.0,<2.0.0) ; extra == "test-docs"
 Requires-Dist: openai (>=1.1.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "test-docs"
-Requires-Dist: pydantic (>=2.7.0b01,<3.0.0)
+Requires-Dist: pydantic (==2.7.0)
 Requires-Dist: pydantic-core (>=2.18.0,<3.0.0)
 Requires-Dist: pydantic_extra_types (>=2.6.0,<3.0.0) ; extra == "test-docs"
 Requires-Dist: redis (>=5.0.1,<6.0.0) ; extra == "test-docs"
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "test-docs"
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9.0,<1.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0) ; extra == "anthropic"
 Project-URL: Repository, https://github.com/jxnl/instructor
 Description-Content-Type: text/markdown
 
 # Instructor: Structured LLM Outputs
 
 Instructor is a Python library that makes it a breeze to work with structured outputs from large language models (LLMs). Built on top of Pydantic, it provides a simple, transparent, and user-friendly API to manage validation, retries, and streaming responses. Get ready to supercharge your LLM workflows!
```

