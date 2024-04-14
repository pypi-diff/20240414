# Comparing `tmp/llmt-0.0.3.tar.gz` & `tmp/llmt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmt-0.0.3.tar", last modified: Mon Apr  1 19:22:50 2024, max compression
+gzip compressed data, was "llmt-0.0.4.tar", last modified: Sun Apr 14 17:02:26 2024, max compression
```

## Comparing `llmt-0.0.3.tar` & `llmt-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:50.779800 llmt-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-01 19:22:46.000000 llmt-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-01 19:22:50.779800 llmt-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-01 19:22:46.000000 llmt-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:50.779800 llmt-0.0.3/llmt/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/assistants.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/json_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/openai_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/response.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-01 19:22:46.000000 llmt-0.0.3/llmt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:22:50.779800 llmt-0.0.3/llmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 19:22:50.000000 llmt-0.0.3/llmt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-01 19:22:46.000000 llmt-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 19:22:46.000000 llmt-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:22:50.779800 llmt-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:02:26.962675 llmt-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-14 17:02:22.000000 llmt-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-14 17:02:26.962675 llmt-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-14 17:02:22.000000 llmt-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:02:26.962675 llmt-0.0.4/llmt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/assistants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/json_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/openai_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/response.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-14 17:02:22.000000 llmt-0.0.4/llmt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:02:26.962675 llmt-0.0.4/llmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-14 17:02:26.000000 llmt-0.0.4/llmt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-14 17:02:22.000000 llmt-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-14 17:02:22.000000 llmt-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:02:26.962675 llmt-0.0.4/setup.cfg
```

### Comparing `llmt-0.0.3/LICENSE` & `llmt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llmt-0.0.3/PKG-INFO` & `llmt-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 Author-email: Artem Golub <artem@outermeasure.com>
 Project-URL: Homepage, https://github.com/omhq/llmt
 Project-URL: Bug Tracker, https://github.com/omhq/llmt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,18 @@
 Requires-Dist: pandas==2.2.1
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: SQLAlchemy==2.0.28
 Requires-Dist: pydantic==2.6.4
 
 # LLMT
 
+[![PyPI version](https://badge.fury.io/py/llmt.svg)](https://badge.fury.io/py/llmt)
+
+## Overview
+
 Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 
 Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
 
 ### Usage
 
 Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
```

### Comparing `llmt-0.0.3/README.md` & `llmt-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # LLMT
 
+[![PyPI version](https://badge.fury.io/py/llmt.svg)](https://badge.fury.io/py/llmt)
+
+## Overview
+
 Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 
 Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
 
 ### Usage
 
 Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
```

### Comparing `llmt-0.0.3/llmt/__init__.py` & `llmt-0.0.4/llmt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     OpenAIFunction,
     RawFunctionResult,
     WrapperConfig,
 )
 from .openai_types import FinalResponseMessage, FunctionCall, GenericMessage, Message
 from .parsers import ArgSchemaParser, defargparsers
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __all__ = [
     "LLMT",
     "OpenAIAssistant",
     "ChatManager",
     "FileManager",
     "prompt_create_chat",
     "prompt_init",
```

### Comparing `llmt-0.0.3/llmt/assistants.py` & `llmt-0.0.4/llmt/assistants.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         return self.client.chat.completions.create(
             messages=messages, model=self.model, tools=tools
         )
     
     def wrap_functions(self, functions):
         return [
             {"type": "function", "function": function} for function in functions
-        ]
+        ] if functions else None
 
     def generate_message(
         self, messages: List[ChatCompletionMessage], functions=None
     ) -> ChatCompletion:
         """Generate a response from the assistant.
 
         Args:
```

### Comparing `llmt-0.0.3/llmt/core.py` & `llmt-0.0.4/llmt/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def prompt_create_chat(self):
         return prompt_create_chat()
 
     def init_prompt(self):
         if not self.configs:
             raise ValueError("No configuration file provided.")
 
-        return prompt_init(self.configs["assistants"], self.get_chats())
+        return prompt_init(self.configs["assistants"], (["Create new chat file"] + self.get_chats()))
 
     def find_assistant(self, assistant_name):
         return next(
             (x for x in self.configs["assistants"] if x["name"] == assistant_name),
             None,
         )
```

### Comparing `llmt-0.0.3/llmt/exceptions.py` & `llmt-0.0.4/llmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `llmt-0.0.3/llmt/managers.py` & `llmt-0.0.4/llmt/managers.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,19 +71,33 @@
             with open(self.input_file, "w") as f:
                 f.write("")
 
         if not os.path.exists(self.output_file):
             with open(self.output_file, "w") as f:
                 f.write("")
 
+    def output_file_contents(self):
+        with open(self.output_file, "r") as f:
+            return f.read()
+
     def write_to_output(self, data):
         template = self.env.get_template(RESPONSE_TEMPLATE)
+        file_contents = self.output_file_contents()
+        date = time.strftime("%Y-%m-%d %I:%M%p")
+        data["date"] = date
+    
         with open(self.output_file, "w") as f:
             f.write(template.render(**data))
 
+            if file_contents:
+                f.write("\n\n")
+                f.write("---")
+                f.write("\n\n")
+                f.write(file_contents)
+
     def events_generator(self):
         yield from self.event_handler.events_generator()
         self.observer.join()
 
     def __del__(self):
         self.observer.stop()
```

### Comparing `llmt-0.0.3/llmt/openai_types.py` & `llmt-0.0.4/llmt/openai_types.py`

 * *Files identical despite different names*

### Comparing `llmt-0.0.3/llmt/prompts.py` & `llmt-0.0.4/llmt/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         inquirer.List(
             "assistant",
             message="Select an assistant to use",
             choices=[x["name"] for x in assistants],
         ),
         inquirer.List(
             "chat_name",
-            message="Select an existing chat",
+            message="Select a chat file",
             choices=chats,
         ),
     ]
 
     return inquirer.prompt(questions)
 
 
@@ -72,16 +72,19 @@
     )
 
 
 def run_until_response(messages, assistant, chat_manager, function_manager):
     function_calls = []
 
     while True:
+        function_schema = (
+            function_manager.functions_schema if function_manager else None
+        )
         chat_completion: ChatCompletion = assistant.generate_message(
-            messages, function_manager.functions_schema
+            messages, function_schema
         )
         chat_completion_choice: CompletionChoice = chat_completion.choices[0]
         chat_completion_message: ChatCompletionMessage = chat_completion_choice.message
         usage: CompletionUsage = chat_completion.usage
         response: str = chat_completion_message.content
 
         if chat_completion_choice.finish_reason == "tool_calls":
```

### Comparing `llmt-0.0.3/llmt/utils.py` & `llmt-0.0.4/llmt/utils.py`

 * *Files identical despite different names*

### Comparing `llmt-0.0.3/llmt.egg-info/PKG-INFO` & `llmt-0.0.4/llmt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 Author-email: Artem Golub <artem@outermeasure.com>
 Project-URL: Homepage, https://github.com/omhq/llmt
 Project-URL: Bug Tracker, https://github.com/omhq/llmt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,18 @@
 Requires-Dist: pandas==2.2.1
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: SQLAlchemy==2.0.28
 Requires-Dist: pydantic==2.6.4
 
 # LLMT
 
+[![PyPI version](https://badge.fury.io/py/llmt.svg)](https://badge.fury.io/py/llmt)
+
+## Overview
+
 Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces.
 
 Supports local function calling, chat history retention, and can run anywhere. Chat using a terminal, input/output files, or directly through LLMT API.
 
 ### Usage
 
 Use the package in directly in your python code (`pip install llmt`), or as a local workspace running a container to interact with ChatGPT.
```

### Comparing `llmt-0.0.3/pyproject.toml` & `llmt-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llmt"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Artem Golub", email="artem @ outermeasure.com"}
 ]
 description = "Convenient LLM chat wrapper for data pipelines, CI/CD, or personal workspaces."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

