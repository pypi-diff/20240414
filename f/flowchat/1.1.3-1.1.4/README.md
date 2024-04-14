# Comparing `tmp/flowchat-1.1.3.tar.gz` & `tmp/flowchat-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchat-1.1.3.tar", last modified: Tue Mar 12 01:05:38 2024, max compression
+gzip compressed data, was "flowchat-1.1.4.tar", last modified: Sun Apr 14 20:18:45 2024, max compression
```

## Comparing `flowchat-1.1.3.tar` & `flowchat-1.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-03-12 01:05:38.045478 flowchat-1.1.3/
--rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.1.3/LICENSE
--rw-r--r--   0 flatypus   (501) staff       (20)     7690 2024-03-12 01:05:38.045253 flowchat-1.1.3/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)     6719 2024-03-05 00:02:43.000000 flowchat-1.1.3/README.md
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-03-12 01:05:38.042330 flowchat-1.1.3/flowchat/
--rw-r--r--   0 flatypus   (501) staff       (20)       60 2023-11-08 10:22:34.000000 flowchat-1.1.3/flowchat/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.1.3/flowchat/autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)    11806 2024-03-12 01:04:35.000000 flowchat-1.1.3/flowchat/chain.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-03-12 01:05:38.043352 flowchat-1.1.3/flowchat/private/
--rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.1.3/flowchat/private/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      309 2024-03-08 00:59:53.000000 flowchat-1.1.3/flowchat/private/_private_helpers.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-03-12 01:05:38.044974 flowchat-1.1.3/flowchat.egg-info/
--rw-r--r--   0 flatypus   (501) staff       (20)     7690 2024-03-12 01:05:38.000000 flowchat-1.1.3/flowchat.egg-info/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)      437 2024-03-12 01:05:38.000000 flowchat-1.1.3/flowchat.egg-info/SOURCES.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-03-12 01:05:38.000000 flowchat-1.1.3/flowchat.egg-info/dependency_links.txt
--rw-r--r--   0 flatypus   (501) staff       (20)       44 2024-03-12 01:05:38.000000 flowchat-1.1.3/flowchat.egg-info/requires.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-03-12 01:05:38.000000 flowchat-1.1.3/flowchat.egg-info/top_level.txt
--rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.1.3/pyproject.toml
--rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-03-12 01:05:38.045525 flowchat-1.1.3/setup.cfg
--rw-r--r--   0 flatypus   (501) staff       (20)     1389 2024-03-12 01:05:27.000000 flowchat-1.1.3/setup.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-03-12 01:05:38.044606 flowchat-1.1.3/tests/
--rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.1.3/tests/test_autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4106 2024-03-08 00:59:53.000000 flowchat-1.1.3/tests/test_chaining.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.1.3/tests/test_config.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4796 2024-03-08 00:59:53.000000 flowchat-1.1.3/tests/test_pull.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.1.3/tests/test_stream.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.257724 flowchat-1.1.4/
+-rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.1.4/LICENSE
+-rw-r--r--   0 flatypus   (501) staff       (20)     7676 2024-04-14 20:18:45.257537 flowchat-1.1.4/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.1.4/README.md
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.254590 flowchat-1.1.4/flowchat/
+-rw-r--r--   0 flatypus   (501) staff       (20)      185 2024-04-14 20:12:59.000000 flowchat-1.1.4/flowchat/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.1.4/flowchat/autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)    11790 2024-04-14 20:15:39.000000 flowchat-1.1.4/flowchat/chain.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.255480 flowchat-1.1.4/flowchat/private/
+-rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.1.4/flowchat/private/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      309 2024-03-08 00:59:53.000000 flowchat-1.1.4/flowchat/private/_private_helpers.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.257312 flowchat-1.1.4/flowchat.egg-info/
+-rw-r--r--   0 flatypus   (501) staff       (20)     7676 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)      437 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)       44 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/requires.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/top_level.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.1.4/pyproject.toml
+-rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-04-14 20:18:45.257765 flowchat-1.1.4/setup.cfg
+-rw-r--r--   0 flatypus   (501) staff       (20)     1389 2024-04-14 20:18:18.000000 flowchat-1.1.4/setup.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.256898 flowchat-1.1.4/tests/
+-rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.1.4/tests/test_autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4106 2024-03-08 00:59:53.000000 flowchat-1.1.4/tests/test_chaining.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.1.4/tests/test_config.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4796 2024-03-08 00:59:53.000000 flowchat-1.1.4/tests/test_pull.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.1.4/tests/test_stream.py
```

### Comparing `flowchat-1.1.3/LICENSE` & `flowchat-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.3/PKG-INFO` & `flowchat-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.1.3
+Version: 1.1.4
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
@@ -77,15 +77,15 @@
     .link(lambda city: f"Design a basic three-act point-form short story about {city}.")
     .link("How long should it be?", assistant=True)
     .link("Around 100 words.")  # (For example) you can make multiple links!
     .pull(max_tokens=512).log().unhook()
 
     .anchor("You are a novelist. Your job is to write a novel about a story that you have heard.")
     .link(lambda storyline: f"Briefly elaborate on the first act of the storyline: {storyline}")
-    .pull(max_tokens=256, model="gpt-4-1106-preview").log().unhook()
+    .pull(max_tokens=256, model="gpt-4-turbo").log().unhook()
 
     .link(lambda act: f"Summarize this act in around three words:\n{act}")
     .pull(model="gpt-4")
     .log_tokens()  # Log token usage of the whole chain
 )
 
 print(f"Result: {chain.last()}") # >> "Artist's Dream Ignites"
@@ -129,15 +129,15 @@
 
         if should_exit.lower() in ("yes", "y"):
             print("Exiting the CLI.")
             break
 
         # Feed the input to flowchat
         command_suggestion = (
-            Chain(model="gpt-4-1106-preview")
+            Chain(model="gpt-4-turbo")
             .anchor(os_system_context)
             .link(autodedent(
                 "The user wants to do this: ",
                 user_input,
                 "Suggest a command that can achieve this in one line without user input or interaction."
             )).pull().unhook()
```

### Comparing `flowchat-1.1.3/README.md` & `flowchat-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     .link(lambda city: f"Design a basic three-act point-form short story about {city}.")
     .link("How long should it be?", assistant=True)
     .link("Around 100 words.")  # (For example) you can make multiple links!
     .pull(max_tokens=512).log().unhook()
 
     .anchor("You are a novelist. Your job is to write a novel about a story that you have heard.")
     .link(lambda storyline: f"Briefly elaborate on the first act of the storyline: {storyline}")
-    .pull(max_tokens=256, model="gpt-4-1106-preview").log().unhook()
+    .pull(max_tokens=256, model="gpt-4-turbo").log().unhook()
 
     .link(lambda act: f"Summarize this act in around three words:\n{act}")
     .pull(model="gpt-4")
     .log_tokens()  # Log token usage of the whole chain
 )
 
 print(f"Result: {chain.last()}") # >> "Artist's Dream Ignites"
@@ -104,15 +104,15 @@
 
         if should_exit.lower() in ("yes", "y"):
             print("Exiting the CLI.")
             break
 
         # Feed the input to flowchat
         command_suggestion = (
-            Chain(model="gpt-4-1106-preview")
+            Chain(model="gpt-4-turbo")
             .anchor(os_system_context)
             .link(autodedent(
                 "The user wants to do this: ",
                 user_input,
                 "Suggest a command that can achieve this in one line without user input or interaction."
             )).pull().unhook()
```

### Comparing `flowchat-1.1.3/flowchat/autodedent.py` & `flowchat-1.1.4/flowchat/autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.3/flowchat/chain.py` & `flowchat-1.1.4/flowchat/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 from typing_extensions import Unpack, NotRequired
 from wrapt_timeout_decorator.wrapt_timeout_decorator import timeout
 import json
 import logging
 import openai
 import os
 
-logging.basicConfig(level=logging.WARNING,
-                    format='[%(asctime)s] %(levelname)s: %(message)s')
+logging.basicConfig(
+    level=logging.WARNING,
+    format='[%(asctime)s] %(levelname)s: %(message)s'
+)
+
 Message = TypedDict('Message', {'role': str, 'content': str | List[Any]})
 ResponseFormat = TypedDict(
     'ResponseFormat', {'type': Literal['text', 'json_object']})
 ImageFormat = TypedDict('ImageFormat', {
     'url': str | PILImage,
     'format_type': str,
     'detail': Literal['low', 'high']
@@ -244,15 +247,15 @@
         if len(self.user_prompt) == 0:
             raise ValueError(
                 "User prompt is empty. Please set a user prompt before pulling."
             )
 
         if json_schema is not None:
             params['response_format'] = {'type': 'json_object'}
-            params['model'] = 'gpt-4-1106-preview'
+            params['model'] = 'gpt-4-turbo'
             self.user_prompt[-1]['content'] += autodedent(
                 "You must respond in the following example JSON format. Remember to enclose the entire JSON object in curly braces:",
                 json.dumps(json_schema, indent=4)
             )
 
         response = self._ask(
             self.system, self.user_prompt,
```

### Comparing `flowchat-1.1.3/flowchat.egg-info/PKG-INFO` & `flowchat-1.1.4/flowchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.1.3
+Version: 1.1.4
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
@@ -77,15 +77,15 @@
     .link(lambda city: f"Design a basic three-act point-form short story about {city}.")
     .link("How long should it be?", assistant=True)
     .link("Around 100 words.")  # (For example) you can make multiple links!
     .pull(max_tokens=512).log().unhook()
 
     .anchor("You are a novelist. Your job is to write a novel about a story that you have heard.")
     .link(lambda storyline: f"Briefly elaborate on the first act of the storyline: {storyline}")
-    .pull(max_tokens=256, model="gpt-4-1106-preview").log().unhook()
+    .pull(max_tokens=256, model="gpt-4-turbo").log().unhook()
 
     .link(lambda act: f"Summarize this act in around three words:\n{act}")
     .pull(model="gpt-4")
     .log_tokens()  # Log token usage of the whole chain
 )
 
 print(f"Result: {chain.last()}") # >> "Artist's Dream Ignites"
@@ -129,15 +129,15 @@
 
         if should_exit.lower() in ("yes", "y"):
             print("Exiting the CLI.")
             break
 
         # Feed the input to flowchat
         command_suggestion = (
-            Chain(model="gpt-4-1106-preview")
+            Chain(model="gpt-4-turbo")
             .anchor(os_system_context)
             .link(autodedent(
                 "The user wants to do this: ",
                 user_input,
                 "Suggest a command that can achieve this in one line without user input or interaction."
             )).pull().unhook()
```

### Comparing `flowchat-1.1.3/setup.py` & `flowchat-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '1.1.3'
+VERSION = '1.1.4'
 DESCRIPTION = 'Streamlining the process of multi-prompting LLMs with chains'
 
 setup(
     name="flowchat",
     version=VERSION,
     author="Hinson Chan",
     author_email="<yhc3141@gmail.com>",
```

### Comparing `flowchat-1.1.3/tests/test_autodedent.py` & `flowchat-1.1.4/tests/test_autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.3/tests/test_chaining.py` & `flowchat-1.1.4/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.3/tests/test_config.py` & `flowchat-1.1.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.3/tests/test_pull.py` & `flowchat-1.1.4/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.3/tests/test_stream.py` & `flowchat-1.1.4/tests/test_stream.py`

 * *Files identical despite different names*

