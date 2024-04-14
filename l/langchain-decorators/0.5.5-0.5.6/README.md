# Comparing `tmp/langchain-decorators-0.5.5.tar.gz` & `tmp/langchain_decorators-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-decorators-0.5.5.tar", last modified: Tue Apr  2 11:00:30 2024, max compression
+gzip compressed data, was "langchain_decorators-0.5.6.tar", last modified: Sun Apr 14 18:33:31 2024, max compression
```

## Comparing `langchain-decorators-0.5.5.tar` & `langchain_decorators-0.5.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-02 11:00:30.452466 langchain-decorators-0.5.5/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.5.5/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22991 2024-04-02 11:00:30.452209 langchain-decorators-0.5.5/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22584 2023-11-15 22:10:25.000000 langchain-decorators-0.5.5/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.5.5/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-04-02 11:00:30.452508 langchain-decorators-0.5.5/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.5.5/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-02 11:00:30.444472 langchain-decorators-0.5.5/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-02 11:00:30.449942 langchain-decorators-0.5.5/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      432 2024-04-02 10:59:59.000000 langchain-decorators-0.5.5/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    37071 2024-02-14 08:32:56.000000 langchain-decorators-0.5.5/src/langchain_decorators/chains.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    20495 2023-12-18 09:15:59.000000 langchain-decorators-0.5.5/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    21044 2023-12-18 07:41:39.000000 langchain-decorators-0.5.5/src/langchain_decorators/function_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    24793 2024-04-02 10:37:57.000000 langchain-decorators-0.5.5/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    21900 2024-04-02 10:42:42.000000 langchain-decorators-0.5.5/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    19606 2024-02-12 07:38:17.000000 langchain-decorators-0.5.5/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4544 2023-09-13 06:19:53.000000 langchain-decorators-0.5.5/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4824 2024-01-05 14:48:06.000000 langchain-decorators-0.5.5/src/langchain_decorators/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1844 2023-06-18 11:01:20.000000 langchain-decorators-0.5.5/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-02 11:00:30.451899 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    22991 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2024-04-02 11:00:30.000000 langchain-decorators-0.5.5/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-14 18:33:31.356951 langchain_decorators-0.5.6/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain_decorators-0.5.6/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-04-14 18:33:31.356725 langchain_decorators-0.5.6/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    22976 2024-04-14 18:30:54.000000 langchain_decorators-0.5.6/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain_decorators-0.5.6/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2024-04-14 18:33:31.356991 langchain_decorators-0.5.6/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain_decorators-0.5.6/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-14 18:33:31.349706 langchain_decorators-0.5.6/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-14 18:33:31.354999 langchain_decorators-0.5.6/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      432 2024-04-14 18:33:00.000000 langchain_decorators-0.5.6/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    37071 2024-02-14 08:32:56.000000 langchain_decorators-0.5.6/src/langchain_decorators/chains.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    20495 2023-12-18 09:15:59.000000 langchain_decorators-0.5.6/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21281 2024-04-14 15:47:14.000000 langchain_decorators-0.5.6/src/langchain_decorators/function_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    24793 2024-04-02 10:37:57.000000 langchain_decorators-0.5.6/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    21900 2024-04-02 10:42:42.000000 langchain_decorators-0.5.6/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    19606 2024-02-12 07:38:17.000000 langchain_decorators-0.5.6/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4544 2023-09-13 06:19:53.000000 langchain_decorators-0.5.6/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4824 2024-01-05 14:48:06.000000 langchain_decorators-0.5.6/src/langchain_decorators/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1844 2023-06-18 11:01:20.000000 langchain_decorators-0.5.6/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2024-04-14 18:33:31.356422 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    23383 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      739 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2024-04-14 18:33:31.000000 langchain_decorators-0.5.6/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain-decorators-0.5.5/LICENSE` & `langchain_decorators-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/PKG-INFO` & `langchain_decorators-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.5.5
+Version: 0.5.6
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
@@ -228,14 +228,32 @@
 
 - by default the docstring format is automatically resolved, but setting the format of the docstring can speed things up a bit.
         -  `auto` (default): the format is automatically inferred from the docstring
         -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
         -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
         -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
 
+### Enum arguments
+
+The best way how to define enum is through type annotation using `Literal`:
+```python
+@llm_function
+def do_magic(spell:str, strength:Literal["light","medium","strong"]):
+    """
+    Do some kind of magic
+
+    Args:
+        spell (str): spall text
+        strength (str): the strength of the spell
+    """
+
+```
+
+---
+**Enum alternative to Literal**
 To annotate an *"enum"* like argument, you can use this "typescript" like format: `["value_a" | "value_b"]` ... if will be parsed out.
 This text will be a part of a description too... if you dont want it, you can use this notation as a type notation.
 Example:
 ```
 Args:
     message_type (["email" | "sms"]): type of a message  / channel how to send the message
         
@@ -247,21 +265,21 @@
 here is how to use it:
 
 ```python
 from langchain.agents import load_tools
 from langchian_decorators import llm_function, llm_prompt, GlobalSettings
 
 @llm_function
-def send_message(message:str, addressee:str=None, message_type:str="email"):
+def send_message(message:str, addressee:str=None, message_type:Literal["email", "whatsapp"]="email"):
     """ Use this if user asks to send some message
 
     Args:
         message (str): message text to send
-        addressee (str): email of the adressese... in format firstName.lastName@company.com
-        message_type (str, optional): enum: ["email"|"whatsapp"]
+        addressee (str): email of the addressee... in format firstName.lastName@company.com
+        message_type (str, optional): style of message by platform
     """
 
     if message_type=="email":
         send_email(addressee, message)
     elif message_type=="whatsapp":
         send_whatsapp(addressee, message)
         
@@ -270,18 +288,18 @@
 list_of_other_tools = load_tools(
     tool_names=[...], 
     llm=GlobalSettings.get_current_settings().default_llm)
 
 @llm_prompt
 def do_what_user_asks_for(user_input:str, functions:List[Union[Callable,BaseTool]]):
     """ 
-    ``` <prompt:system>
+    ```<prompt:system>
     Your role is to be a helpful asistant.
     ```
-    ``` <prompt:user>
+    ```<prompt:user>
     {user_input}
     ```
     """
 
 user_input="Yo, send an email to John Smith that I will be late for the meeting"
 result = do_what_user_asks_for(
         user_input=user_input,
```

### Comparing `langchain-decorators-0.5.5/README.md` & `langchain_decorators-0.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,32 @@
 
 - by default the docstring format is automatically resolved, but setting the format of the docstring can speed things up a bit.
         -  `auto` (default): the format is automatically inferred from the docstring
         -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
         -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
         -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
 
+### Enum arguments
+
+The best way how to define enum is through type annotation using `Literal`:
+```python
+@llm_function
+def do_magic(spell:str, strength:Literal["light","medium","strong"]):
+    """
+    Do some kind of magic
+
+    Args:
+        spell (str): spall text
+        strength (str): the strength of the spell
+    """
+
+```
+
+---
+**Enum alternative to Literal**
 To annotate an *"enum"* like argument, you can use this "typescript" like format: `["value_a" | "value_b"]` ... if will be parsed out.
 This text will be a part of a description too... if you dont want it, you can use this notation as a type notation.
 Example:
 ```
 Args:
     message_type (["email" | "sms"]): type of a message  / channel how to send the message
         
@@ -232,21 +250,21 @@
 here is how to use it:
 
 ```python
 from langchain.agents import load_tools
 from langchian_decorators import llm_function, llm_prompt, GlobalSettings
 
 @llm_function
-def send_message(message:str, addressee:str=None, message_type:str="email"):
+def send_message(message:str, addressee:str=None, message_type:Literal["email", "whatsapp"]="email"):
     """ Use this if user asks to send some message
 
     Args:
         message (str): message text to send
-        addressee (str): email of the adressese... in format firstName.lastName@company.com
-        message_type (str, optional): enum: ["email"|"whatsapp"]
+        addressee (str): email of the addressee... in format firstName.lastName@company.com
+        message_type (str, optional): style of message by platform
     """
 
     if message_type=="email":
         send_email(addressee, message)
     elif message_type=="whatsapp":
         send_whatsapp(addressee, message)
         
@@ -255,18 +273,18 @@
 list_of_other_tools = load_tools(
     tool_names=[...], 
     llm=GlobalSettings.get_current_settings().default_llm)
 
 @llm_prompt
 def do_what_user_asks_for(user_input:str, functions:List[Union[Callable,BaseTool]]):
     """ 
-    ``` <prompt:system>
+    ```<prompt:system>
     Your role is to be a helpful asistant.
     ```
-    ``` <prompt:user>
+    ```<prompt:user>
     {user_input}
     ```
     """
 
 user_input="Yo, send an email to John Smith that I will be late for the meeting"
 result = do_what_user_asks_for(
         user_input=user_input,
```

### Comparing `langchain-decorators-0.5.5/setup.py` & `langchain_decorators-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/chains.py` & `langchain_decorators-0.5.6/src/langchain_decorators/chains.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/common.py` & `langchain_decorators-0.5.6/src/langchain_decorators/common.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/function_decorator.py` & `langchain_decorators-0.5.6/src/langchain_decorators/function_decorator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,112 @@
-
-import re
 import inspect
+import re
 from enum import Enum
-from string import Formatter
 from functools import wraps
-from typing import Any, Callable, Dict, List, Set,  Union, Type, Tuple, get_args, get_origin
+from string import Formatter
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Set,
+    Tuple,
+    Type,
+    Union,
+    get_args,
+    get_origin,
+)
 
 import pydantic
-if pydantic.__version__ <"2.0.0":
+
+if pydantic.__version__ < "2.0.0":
     from pydantic import BaseModel
-    from pydantic.schema import  field_schema, get_flat_models_from_fields, get_model_name_map, add_field_type_to_schema
+    from pydantic.schema import (
+        add_field_type_to_schema,
+        field_schema,
+        get_flat_models_from_fields,
+        get_model_name_map,
+    )
 else:
     from pydantic.v1 import BaseModel
-    from pydantic.v1.schema import  field_schema, get_flat_models_from_fields, get_model_name_map, add_field_type_to_schema
-
-
+    from pydantic.v1.schema import (
+        field_schema,
+        get_flat_models_from_fields,
+        get_model_name_map,
+        add_field_type_to_schema,
+    )
+
+from .common import (
+    get_arguments_as_pydantic_fields,
+    get_function_docs,
+    get_function_full_name,
+)
 from .pydantic_helpers import sanitize_pydantic_schema
-from .common import  get_arguments_as_pydantic_fields, get_function_docs, get_function_full_name
+
 
 class DocstringsFormat(Enum):
     AUTO = "auto"
     GOOGLE = "google"
     SPHINX = "sphinx"
     NUMPY = "numpy"
 
+
 def get_function_schema(func, schema_template_args=None):
-    if callable(func) and hasattr(func,"get_function_schema"):
+    if callable(func) and hasattr(func, "get_function_schema"):
         return func.get_function_schema(func, schema_template_args)
     else:
-        raise ValueError(f"Invalid item value in functions. Unable to retrieve schema from function {f}")
+        raise ValueError(
+            f"Invalid item value in functions. Unable to retrieve schema from function {f}"
+        )
 
 
 def is_dynamic_llm_func(func):
-    if callable(func) and hasattr(func,"get_function_schema"):
-        return getattr(func,"is_dynamic",False)
+    if callable(func) and hasattr(func, "get_function_schema"):
+        return getattr(func, "is_dynamic", False)
+
 
-def get_dynamic_function_template_args(func:Callable)->Tuple[List[str],List[str]]:
-    """ 
-    returns tuple of (required_args:List[str], optional_args:List[str]) 
+def get_dynamic_function_template_args(func: Callable) -> Tuple[List[str], List[str]]:
+    """
+    returns tuple of (required_args:List[str], optional_args:List[str])
     """
     func_docs = get_function_docs(func)
     if not func_docs:
-        raise ValueError(f"LLM Function {get_function_full_name(func)} has no docstring")
-    
+        raise ValueError(
+            f"LLM Function {get_function_full_name(func)} has no docstring"
+        )
+
     return get_template_args(func_docs)
 
+
 class DotDict(dict):
-    def __init__(self, dictionary:dict):
+
+    def __init__(self, dictionary: dict):
         super().__init__(dictionary)
-    
+
     def __getattr__(self, name):
         if name in self:
 
             val = self.get(name)
             if isinstance(val, dict):
                 return DotDict(val)
             else:
                 return val
         else:
             return None
 
+
 def llm_function(
-        function_name:str=None,
-        validate_docstrings:bool=True,
-        docstring_format:str="auto",
-        arguments_schema:Union[Type[BaseModel], Type[List[Any]]]=None,
-        dynamic_schema:bool=False,
-        func_description:str=None,
-        **kwargs
-        ):
+    function_name: str = None,
+    validate_docstrings: bool = True,
+    docstring_format: str = "auto",
+    arguments_schema: Union[Type[BaseModel], Type[List[Any]]] = None,
+    dynamic_schema: bool = False,
+    func_description: str = None,
+    **kwargs,
+):
     """
     Decorator for functions that take a language model as first argument.
 
 
     Args:
         - function_name: the name of the function for LLM. If not provided, the name of the function will be used
 
@@ -100,15 +134,15 @@
         - docstring_format: the format of the docstring
             -  `auto` (default): the format is automatically inferred from the docstring
             -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
             -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
             -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
 
     Examples:
-    
+
         Google style docstrings:
         ```python
         @llm_function
         def function_with_google_docstrings(self, question:str)->bool:
             \"\"\"
             This is a function with google docstrings
             Args:  # but accepts also Parameters, Arguments
@@ -121,376 +155,419 @@
         def function_with_numpy_docstrings(self, question:str)->bool:
             \"\"\"
             This is a function with google docstrings
             Parameters # but accepts also Args, Arguments
             ----------
                 question :int
                     Question to ask
-                
+
             \"\"\"
         ```
 
         ```python
         @llm_function
         def function_with_sphinx_docstrings(self, question:str)->bool:
             \"\"\"
             This is a function with google docstrings
             :param question: Question to ask
-                
+
             \"\"\"
         ```
 
-    Note: 
+    Note:
         The fact whether the parameter is optional is inferred from the function signature. You can also document it, but it will be just part of the description. If typing annotations are used (i.e. Optional[str]), this will be stripped to native type.
-    
+
     """
-    
+
     if callable(function_name):
         # this is the case when the decorator is called without arguments
         # we initialize params with default values
         func = function_name
-        function_name=None
+        function_name = None
     else:
         func = None
 
-   
-    
     def decorator(func):
 
-        if dynamic_schema: 
+        if dynamic_schema:
+
             def get_function_schema(_func, schema_template_args):
-                return build_func_schema(_func, 
-                                                function_name = function_name, 
-                                                format=docstring_format, 
-                                                validate_docstrings=validate_docstrings,
-                                                arguments_schema=arguments_schema,
-                                                func_description=func_description,
-                                                schema_template_parameters=schema_template_args,
-                                            )
+                return build_func_schema(
+                    _func,
+                    function_name=function_name,
+                    format=docstring_format,
+                    validate_docstrings=validate_docstrings,
+                    arguments_schema=arguments_schema,
+                    func_description=func_description,
+                    schema_template_parameters=schema_template_args,
+                )
+
         else:
-            func_schema =  build_func_schema(func, 
-                                                function_name = function_name, 
-                                                format=docstring_format, 
-                                                validate_docstrings=validate_docstrings,
-                                                arguments_schema=arguments_schema,
-                                                func_description=func_description,
-                                                schema_template_parameters=None,
-                                            )
+            func_schema = build_func_schema(
+                func,
+                function_name=function_name,
+                format=docstring_format,
+                validate_docstrings=validate_docstrings,
+                arguments_schema=arguments_schema,
+                func_description=func_description,
+                schema_template_parameters=None,
+            )
+
             def get_function_schema(_func, schema_template_args=None):
                 return func_schema
-        
+
         is_async = inspect.iscoroutinefunction(func)
 
         if not is_async:
+
             @wraps(func)
             def func_wrapper(*args, **kwargs):
                 return func(*args, **kwargs)
-            
+
         else:
+
             @wraps(func)
             async def func_wrapper(*args, **kwargs):
                 return await func(*args, **kwargs)
-        
-        
-        
-       
 
-        func_wrapper.get_function_schema=get_function_schema
+        func_wrapper.get_function_schema = get_function_schema
         func_wrapper.is_dynamic = dynamic_schema
         func_wrapper.function_name = function_name or func.__name__
 
         return func_wrapper
-    
+
     if func:
         return decorator(func)
     else:
         return decorator
-    
+
 
 class LllFunctionWithModifiedSchema:
-    def __init__(self, func, modified_schema:dict):
+
+    def __init__(self, func, modified_schema: dict):
         self.func = func
         self._function_schema = modified_schema
 
-
     def __call__(self, *args, **kwargs):
         return self.func(*args, **kwargs)
 
     def get_function_schema(self):
         return self._function_schema
-        
+
 
 def build_func_schema(
-        func:Callable, 
-        function_name:str=None, 
-        format:Union[DocstringsFormat,str]="auto", 
-        validate_docstrings:bool=True,
-        arguments_schema:Union[Type[BaseModel], Type[List[Any]], None] = None,
-        func_description:str=None,
-        schema_template_parameters:Dict[str,Any]=None,
-        ):
-    
-    if isinstance(format,str):
+    func: Callable,
+    function_name: str = None,
+    format: Union[DocstringsFormat, str] = "auto",
+    validate_docstrings: bool = True,
+    arguments_schema: Union[Type[BaseModel], Type[List[Any]], None] = None,
+    func_description: str = None,
+    schema_template_parameters: Dict[str, Any] = None,
+):
+
+    if isinstance(format, str):
         format = DocstringsFormat(format)
 
     if not (func_description and arguments_schema):
-        func_docs = get_function_docs(func)  
+        func_docs = get_function_docs(func)
         if schema_template_parameters:
             func_docs = format_str_extra(func_docs, **schema_template_parameters)
     else:
         func_docs = None
 
-
     if function_name and not re.match(r"^[a-zA-Z_][a-zA-Z0-9_]*$", function_name):
-        raise ValueError(f"Invalid function name: {function_name} for {get_function_full_name(func)}. Only letters, numbers and underscores are allowed. The name must start with a letter or an underscore.")
-   
-    func_name =  function_name or func.__name__
+        raise ValueError(
+            f"Invalid function name: {function_name} for {get_function_full_name(func)}. Only letters, numbers and underscores are allowed. The name must start with a letter or an underscore."
+        )
+
+    func_name = function_name or func.__name__
     args_schema = None
-    
-    if arguments_schema and isinstance(arguments_schema,Type):
+
+    if arguments_schema and isinstance(arguments_schema, Type):
         args_schema = arguments_schema.schema()
         sanitize_pydantic_schema(args_schema)
-        args_schema={
-            "type":"object",
+        args_schema = {
+            "type": "object",
             "properties": args_schema["properties"],
-            "required":args_schema["required"]
+            "required": args_schema["required"],
         }
-    elif arguments_schema and isinstance(arguments_schema,dict):
+    elif arguments_schema and isinstance(arguments_schema, dict):
         if "properties" in arguments_schema:
-            sanitize_pydantic_schema(arguments_schema)  
-            #arguments schema is a OPENAPI schema
+            sanitize_pydantic_schema(arguments_schema)
+            # arguments schema is a OPENAPI schema
             args_schema = arguments_schema
-        elif any((v for v in arguments_schema.values() if isinstance(v,str))):
-            #arguments schema is a dict of types
+        elif any((v for v in arguments_schema.values() if isinstance(v, str))):
+            # arguments schema is a dict of types
             args_schema = {
-                "type":"object",
-                "properties":{k:{'title': k, 'description': v, 'type': 'string'} for k,v in arguments_schema.items()},
-                "required":[k for k,v in arguments_schema.items() if v is not None]
+                "type": "object",
+                "properties": {
+                    k: {"title": k, "description": v, "type": "string"}
+                    for k, v in arguments_schema.items()
+                },
+                "required": [k for k, v in arguments_schema.items() if v is not None],
             }
         else:
-            raise ValueError("Invalid arguments_schema... it must be a BaseModel type, a dict describing OPENAPI schema or a dict of of fields with descriptions as values")
+            raise ValueError(
+                "Invalid arguments_schema... it must be a BaseModel type, a dict describing OPENAPI schema or a dict of of fields with descriptions as values"
+            )
     else:
         arguments_fields = get_arguments_as_pydantic_fields(func)
-        
+
         if func_docs:
-            docstrings_param_description = find_and_parse_params_from_docstrings(func_docs,format=format)
+            docstrings_param_description = find_and_parse_params_from_docstrings(
+                func_docs, format=format
+            )
             if docstrings_param_description:
                 if validate_docstrings:
-                    documented_params=set(docstrings_param_description.keys()) 
-                    implemented_params= set(arguments_fields.keys())
-                    not_implemented = documented_params - implemented_params  # Set difference: keys in set1 but not in set2
-                    not_documented = implemented_params - documented_params  # Set difference: keys in set2 but not in set1
+                    documented_params = set(docstrings_param_description.keys())
+                    implemented_params = set(arguments_fields.keys())
+                    not_implemented = (
+                        documented_params - implemented_params
+                    )  # Set difference: keys in set1 but not in set2
+                    not_documented = (
+                        implemented_params - documented_params
+                    )  # Set difference: keys in set2 but not in set1
 
                     if not_implemented or not_documented:
                         errs = []
                         if not_implemented:
                             errs.append(f"Missing (not implemented): {not_implemented}")
                         if not_documented:
                             errs.append(f"Missing (not documented): {not_documented}")
-                        
-                        raise ValueError(f"Docstrings parameters do not match function {func.__module__}.{func.__name__} signature. "+ ",".join(errs))
-                
+
+                        raise ValueError(
+                            f"Docstrings parameters do not match function {func.__module__}.{func.__name__} signature. "
+                            + ",".join(errs)
+                        )
+
                 for arg_name, arg_model_field in arguments_fields.items():
                     arg_docs = docstrings_param_description.get(arg_name)
                     if arg_docs:
-                        
-                        arg_model_field.field_info.description =arg_docs["description"]
-                        enum = parse_enum_from_docstring_param(arg_docs["type"],arg_docs["description"])
+
+                        arg_model_field.field_info.description = arg_docs["description"]
+                        enum = parse_enum_from_docstring_param(
+                            arg_docs["type"], arg_docs["description"]
+                        )
                         if enum:
                             arg_model_field.field_info.extra["enum"] = enum
 
-        args_schema={
-            "type":"object",
-            "properties":{},
-            "required":[]
-        }
+        args_schema = {"type": "object", "properties": {}, "required": []}
 
         flat_models = get_flat_models_from_fields(arguments_fields.values(), set())
         model_name_map = get_model_name_map(flat_models)
         for arg_name, arg_model_field in arguments_fields.items():
-                
-            param_schema, ref_schema , nested_models_schema = field_schema(arg_model_field, model_name_map=model_name_map) 
+
+            param_schema, ref_schema, nested_models_schema = field_schema(
+                arg_model_field, model_name_map=model_name_map
+            )
             if "$ref" in param_schema:
-                ent_name = param_schema["$ref"].rsplit("/",1)[-1]
+                ent_name = param_schema["$ref"].rsplit("/", 1)[-1]
                 param_schema = ref_schema.get(ent_name)
-            elif "$ref" in param_schema.get("items",{}):
+            elif "$ref" in param_schema.get("items", {}):
                 param_schema["items"]["$ref"]
-                ent_name = param_schema["items"]["$ref"].rsplit("/",1)[-1]
+                ent_name = param_schema["items"]["$ref"].rsplit("/", 1)[-1]
                 param_schema["items"] = ref_schema.get(ent_name)
             if nested_models_schema:
                 raise NotImplementedError("Nested models are not supported yet")
-            
+
             args_schema["properties"][arg_name] = param_schema
             if arg_model_field.required:
                 args_schema["required"].append(arg_name)
 
-    
     def pop_prop_title(schema):
-        #title is autogenerated by pydantic and will just costs us tokens....
+        # title is autogenerated by pydantic and will just costs us tokens....
         if "title" in schema:
             del schema["title"]
         return schema
-    args_schema["properties"] = {prop:pop_prop_title(prop_schema) for prop, prop_schema in args_schema["properties"].items()}
-    
-    description = parse_function_description_from_docstrings(func_docs) if func_docs else func_description
-
-    result_schema = {
-        "name":func_name,
-        "parameters":args_schema
+
+    args_schema["properties"] = {
+        prop: pop_prop_title(prop_schema)
+        for prop, prop_schema in args_schema["properties"].items()
     }
+
+    description = (
+        parse_function_description_from_docstrings(func_docs)
+        if func_docs
+        else func_description
+    )
+
+    result_schema = {"name": func_name, "parameters": args_schema}
     if description:
-        result_schema["description"]=description
+        result_schema["description"] = description
     return result_schema
-            
 
 
-        
-def format_str_extra(template:str, **kwargs):
-    optional_blocks_regex = list(re.finditer(r"\{\?(?P<optional_partial>.+?)(?=\?\})\?\}", template, re.MULTILINE | re.DOTALL))
+def format_str_extra(template: str, **kwargs):
+    optional_blocks_regex = list(
+        re.finditer(
+            r"\{\?(?P<optional_partial>.+?)(?=\?\})\?\}",
+            template,
+            re.MULTILINE | re.DOTALL,
+        )
+    )
     for optional_block in optional_blocks_regex:
+        optional_partial = optional_block.group("optional_partial")
+        partial_input_variables = {
+            v for _, v, _, _ in Formatter().parse(optional_partial) if v is not None
+        }
+
+        if not partial_input_variables:
+            raise ValueError(
+                f"Optional partial {optional_partial} does not contain any optional variables. Didn't you forget to wrap your parameter in {{}}?"
+            )
+
+        if not all(kwargs.get(v) for v in partial_input_variables):
+            # all variables are provided, we can remove the optional block
+            template = template.replace(optional_block.group(0), "")
+        else:
             optional_partial = optional_block.group("optional_partial")
-            partial_input_variables = {v for _, v, _, _ in Formatter().parse(optional_partial) if v is not None}
-            
-            if not partial_input_variables:
-                raise ValueError(f"Optional partial {optional_partial} does not contain any optional variables. Didn't you forget to wrap your parameter in {{}}?")
-            
-            if not all(kwargs.get(v) for v in partial_input_variables):
-                # all variables are provided, we can remove the optional block
-                template = template.replace(optional_block.group(0), "")
-            else:
-                optional_partial = optional_block.group("optional_partial")
-                template = template.replace(optional_block.group(0),optional_partial )
+            template = template.replace(optional_block.group(0), optional_partial)
 
-    _format_args={k:v if not isinstance(v,dict) else DotDict(v) for k,v in kwargs.items() }
+    _format_args = {
+        k: v if not isinstance(v, dict) else DotDict(v) for k, v in kwargs.items()
+    }
     return Formatter().format(template, **_format_args)
-     
 
-def get_template_args(template:str)->Tuple[List[str],List[str]]:
-    """ returns tuple of (required_args:List[str], optional_args:List[str]) """
-    optional_args=set()
-    optional_blocks_regex = list(re.finditer(r"\{\?(?P<optional_partial>.+?)(?=\?\})\?\}", template, re.MULTILINE | re.DOTALL))
+
+def get_template_args(template: str) -> Tuple[List[str], List[str]]:
+    """returns tuple of (required_args:List[str], optional_args:List[str])"""
+    optional_args = set()
+    optional_blocks_regex = list(
+        re.finditer(
+            r"\{\?(?P<optional_partial>.+?)(?=\?\})\?\}",
+            template,
+            re.MULTILINE | re.DOTALL,
+        )
+    )
     for optional_block in optional_blocks_regex:
-            optional_partial = optional_block.group("optional_partial")
-            partial_input_variables = {v for _, v, _, _ in Formatter().parse(optional_partial) if v is not None}
-            optional_args.update(partial_input_variables)
-            if not partial_input_variables:
-                raise ValueError(f"Optional partial {optional_partial} does not contain any optional variables. Didn't you forget to wrap your parameter in {{}}?")
-            
-            
-            # replace optional block with underscore so it wont be parsed for required args
-            template = template.replace(optional_block.group(0), "_")
+        optional_partial = optional_block.group("optional_partial")
+        partial_input_variables = {
+            v for _, v, _, _ in Formatter().parse(optional_partial) if v is not None
+        }
+        optional_args.update(partial_input_variables)
+        if not partial_input_variables:
+            raise ValueError(
+                f"Optional partial {optional_partial} does not contain any optional variables. Didn't you forget to wrap your parameter in {{}}?"
+            )
+
+        # replace optional block with underscore so it wont be parsed for required args
+        template = template.replace(optional_block.group(0), "_")
 
-             
     required_args = {v for _, v, _, _ in Formatter().parse(template) if v is not None}
     return required_args, optional_args
 
 
-
-def parse_function_description_from_docstrings(docstring:str)->str:
+def parse_function_description_from_docstrings(docstring: str) -> str:
     # we will return first text until first empty line
-    
+
     lines = docstring.splitlines()
     description = []
     for line in lines:
         line = line.strip()
         if line:
             description.append(line)
         elif description:
             # if we have already some description, we stop at first empty line ... else continue
             break
     return "\n".join(description)
 
 
-
-
-
-    
-
-
-    
-
-def find_and_parse_params_from_docstrings(docstring:str,format:DocstringsFormat)->str:
+def find_and_parse_params_from_docstrings(
+    docstring: str, format: DocstringsFormat
+) -> str:
     """
     Find Args section in docstring.
     """
 
     args_section = None
     args_section_start = 0
     args_section_end = None
-    
+
     if format == DocstringsFormat.AUTO or format == DocstringsFormat.GOOGLE:
         # auto here means more more free format than google
-        args_section_start_regex_pattern = r"(^|\n)(Args|Arguments|Parameters)\s*:?\s*\n"
+        args_section_start_regex_pattern = (
+            r"(^|\n)(Args|Arguments|Parameters)\s*:?\s*\n"
+        )
         args_section_end_regex_pattern = r"(^|\n)([A-Z][a-z]+)\s*:?\s*\n"
-        if  format == DocstringsFormat.GOOGLE:
-            param_start_parser_regex=r"(^|\n)\s+(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)\s*(\((?P<type>[^\)]*)\))?\s*:\s*(?=\w+)"
+        if format == DocstringsFormat.GOOGLE:
+            param_start_parser_regex = r"(^|\n)\s+(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)\s*(\((?P<type>[^\)]*)\))?\s*:\s*(?=[^\n]+)"
         else:
-            param_start_parser_regex=r"(^|\n)\s+(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)\s*(\((?P<type>[^\)]*)\))?\s*(-|:)\s*(?=\w+)"
+            param_start_parser_regex = r"(^|\n)\s+(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)\s*(\((?P<type>[^\)]*)\))?\s*(-|:)\s*(?=[^\n]+)"
     elif format == DocstringsFormat.NUMPY:
-        args_section_start_regex_pattern = r"(^|\n)(Args|Arguments|Parameters)\s*\n\s*---+\s*\n"
+        args_section_start_regex_pattern = (
+            r"(^|\n)(Args|Arguments|Parameters)\s*\n\s*---+\s*\n"
+        )
         args_section_end_regex_pattern = r"(^|\n)([A-Z][a-z]+)\s*\n\s*---+\s*\n"
-        param_start_parser_regex=r"(^|\n)\s*(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)(\s*:\s*(?P<type>[^\)]*)\s*)?\n\s+(?=\w+)"
+        param_start_parser_regex = r"(^|\n)\s*(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)(\s*:\s*(?P<type>[^\)]*)\s*)?\n\s+(?=[^\n]+)"
     elif format == DocstringsFormat.SPHINX:
-        args_section_start_regex_pattern = None # we will look for :param everywhere
-        args_section_end_regex_pattern=r"(\n)\s*:[a-z]"
-        param_start_parser_regex=r"(^|\n)\s*:param\s+(?P<type>[^\)]*)\s+(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)\s*:\s*(?=\w+)"
+        args_section_start_regex_pattern = None  # we will look for :param everywhere
+        args_section_end_regex_pattern = r"(\n)\s*:[a-z]"
+        param_start_parser_regex = r"(^|\n)\s*:param\s+(?P<type>[^\)]*)\s+(?P<name>[a-zA-Z_][a-zA-Z0-9_]*)\s*:\s*(?=[^\n]+)"
 
     if args_section_start_regex_pattern:
         match = re.search(args_section_start_regex_pattern, docstring)
         if match:
             args_section_start = match.end()
             if args_section_end_regex_pattern:
-                match = re.search(args_section_end_regex_pattern, docstring[args_section_start:])
+                match = re.search(
+                    args_section_end_regex_pattern, docstring[args_section_start:]
+                )
                 if match:
                     args_section_end = match.start() + args_section_start
             if not args_section_end:
                 args_section_end = len(docstring)
             args_section = docstring[args_section_start:args_section_end]
         else:
-            args_section=None
+            args_section = None
     else:
-        args_section=docstring
-    
-    params={}
+        args_section = docstring
+
+    params = {}
     if args_section:
-        last_param=None
-        last_param_end=None
+        last_param = None
+        last_param_end = None
         for param_start_match in re.finditer(param_start_parser_regex, args_section):
             if last_param_end is not None:
-                last_param["description"]=args_section[last_param_end:param_start_match.start()].strip()
+                last_param["description"] = args_section[
+                    last_param_end : param_start_match.start()
+                ].strip()
 
             param_name = param_start_match.group("name")
             param_type = param_start_match.group("type")
-            last_param = {"type":param_type or "","description":None}
+            last_param = {"type": param_type or "", "description": None}
             last_param_end = param_start_match.end()
-            params[param_name]=last_param
+            params[param_name] = last_param
 
         if last_param_end is not None:
-            section_end=None
-            if args_section_start_regex_pattern is None and args_section_end_regex_pattern:
+            section_end = None
+            if (
+                args_section_start_regex_pattern is None
+                and args_section_end_regex_pattern
+            ):
                 # this is handling SPHINX, we didnt parse the start so we cant parse the end until all the params are consumed... now we can parse the end after the last param
-                section_end_match= re.search(args_section_end_regex_pattern, docstring[last_param_end:])    
+                section_end_match = re.search(
+                    args_section_end_regex_pattern, docstring[last_param_end:]
+                )
                 if section_end_match:
-                    section_end=last_param_end + section_end_match.start()
+                    section_end = last_param_end + section_end_match.start()
             if not section_end:
-                section_end=len(docstring)
-            last_param["description"]=args_section[last_param_end:section_end].strip()
-        
+                section_end = len(docstring)
+            last_param["description"] = args_section[last_param_end:section_end].strip()
 
-    if not params and  format == DocstringsFormat.AUTO:
-            # try other options            
+    if not params and format == DocstringsFormat.AUTO:
+        # try other options
         options = [DocstringsFormat.NUMPY, DocstringsFormat.SPHINX]
         for option in options:
-            result = find_and_parse_params_from_docstrings(docstring,option)
+            result = find_and_parse_params_from_docstrings(docstring, option)
             if result:
                 return result
     else:
         return params
-        
-            
-def parse_enum_from_docstring_param(type:str, description)->str:
-    enum_pattern=r"\[\s*(?P<value>[\"|'][\w|_|-| ]+[\"|']\s*(\||\]))+"
-    enum_part_match = re.search(enum_pattern, type +" / " +description)
+
+
+def parse_enum_from_docstring_param(type: str, description) -> str:
+    enum_pattern = r"\[\s*(?P<value>[\"|'][\w|_|-| ]+[\"|']\s*(\||\]))+"
+    enum_part_match = re.search(enum_pattern, type + " / " + description)
     if not enum_part_match:
         return None
-    enum_strings =enum_part_match.group(0).strip("[]").split("|")
+    enum_strings = enum_part_match.group(0).strip("[]").split("|")
     return [enum.strip(" \"'") for enum in enum_strings]
```

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/output_parsers.py` & `langchain_decorators-0.5.6/src/langchain_decorators/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/prompt_decorator.py` & `langchain_decorators-0.5.6/src/langchain_decorators/prompt_decorator.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/prompt_template.py` & `langchain_decorators-0.5.6/src/langchain_decorators/prompt_template.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/pydantic_helpers.py` & `langchain_decorators-0.5.6/src/langchain_decorators/pydantic_helpers.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/schema.py` & `langchain_decorators-0.5.6/src/langchain_decorators/schema.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators/streaming_context.py` & `langchain_decorators-0.5.6/src/langchain_decorators/streaming_context.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators.egg-info/PKG-INFO` & `langchain_decorators-0.5.6/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.5.5
+Version: 0.5.6
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
@@ -228,14 +228,32 @@
 
 - by default the docstring format is automatically resolved, but setting the format of the docstring can speed things up a bit.
         -  `auto` (default): the format is automatically inferred from the docstring
         -  `google`: the docstring is parsed as markdown (see [Google docstring format](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html))
         -  `numpy`: the docstring is parsed as markdown (see [Numpy docstring format](https://numpydoc.readthedocs.io/en/latest/format.html))
         -  `sphinx`: the docstring is parsed as sphinx format (see [Sphinx docstring format](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/docstrings.html))
 
+### Enum arguments
+
+The best way how to define enum is through type annotation using `Literal`:
+```python
+@llm_function
+def do_magic(spell:str, strength:Literal["light","medium","strong"]):
+    """
+    Do some kind of magic
+
+    Args:
+        spell (str): spall text
+        strength (str): the strength of the spell
+    """
+
+```
+
+---
+**Enum alternative to Literal**
 To annotate an *"enum"* like argument, you can use this "typescript" like format: `["value_a" | "value_b"]` ... if will be parsed out.
 This text will be a part of a description too... if you dont want it, you can use this notation as a type notation.
 Example:
 ```
 Args:
     message_type (["email" | "sms"]): type of a message  / channel how to send the message
         
@@ -247,21 +265,21 @@
 here is how to use it:
 
 ```python
 from langchain.agents import load_tools
 from langchian_decorators import llm_function, llm_prompt, GlobalSettings
 
 @llm_function
-def send_message(message:str, addressee:str=None, message_type:str="email"):
+def send_message(message:str, addressee:str=None, message_type:Literal["email", "whatsapp"]="email"):
     """ Use this if user asks to send some message
 
     Args:
         message (str): message text to send
-        addressee (str): email of the adressese... in format firstName.lastName@company.com
-        message_type (str, optional): enum: ["email"|"whatsapp"]
+        addressee (str): email of the addressee... in format firstName.lastName@company.com
+        message_type (str, optional): style of message by platform
     """
 
     if message_type=="email":
         send_email(addressee, message)
     elif message_type=="whatsapp":
         send_whatsapp(addressee, message)
         
@@ -270,18 +288,18 @@
 list_of_other_tools = load_tools(
     tool_names=[...], 
     llm=GlobalSettings.get_current_settings().default_llm)
 
 @llm_prompt
 def do_what_user_asks_for(user_input:str, functions:List[Union[Callable,BaseTool]]):
     """ 
-    ``` <prompt:system>
+    ```<prompt:system>
     Your role is to be a helpful asistant.
     ```
-    ``` <prompt:user>
+    ```<prompt:user>
     {user_input}
     ```
     """
 
 user_input="Yo, send an email to John Smith that I will be late for the meeting"
 result = do_what_user_asks_for(
         user_input=user_input,
```

### Comparing `langchain-decorators-0.5.5/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain_decorators-0.5.6/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

