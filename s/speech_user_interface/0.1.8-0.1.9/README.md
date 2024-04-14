# Comparing `tmp/speech_user_interface-0.1.8.tar.gz` & `tmp/speech_user_interface-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_user_interface-0.1.8.tar", max compression
+gzip compressed data, was "speech_user_interface-0.1.9.tar", max compression
```

## Comparing `speech_user_interface-0.1.8.tar` & `speech_user_interface-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      910 2024-04-13 08:32:55.828114 speech_user_interface-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      683 2024-04-13 08:18:10.670985 speech_user_interface-0.1.8/README.md
--rw-r--r--   0        0        0     1744 2024-04-13 08:21:20.836731 speech_user_interface-0.1.8/speech_user_interface/__init__.py
--rw-r--r--   0        0        0      191 2024-04-13 05:15:04.952636 speech_user_interface-0.1.8/speech_user_interface/compare_strings.py
--rw-r--r--   0        0        0       49 2024-04-13 04:37:33.298012 speech_user_interface-0.1.8/speech_user_interface/CONSTANTS.py
--rw-r--r--   0        0        0      630 2024-04-13 05:12:32.571540 speech_user_interface-0.1.8/speech_user_interface/load_vosk_model.py
--rw-r--r--   0        0        0     1416 2024-04-13 05:50:57.320876 speech_user_interface-0.1.8/speech_user_interface/read_in_speech.py
--rw-r--r--   0        0        0      462 2024-04-13 05:25:09.140507 speech_user_interface-0.1.8/speech_user_interface/send_text_to_chatgpt.py
--rw-r--r--   0        0        0      490 2024-04-13 04:33:28.596917 speech_user_interface-0.1.8/speech_user_interface/speak_text.py
--rw-r--r--   0        0        0     1776 1970-01-01 00:00:00.000000 speech_user_interface-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      907 2024-04-13 08:36:01.722861 speech_user_interface-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      683 2024-04-13 08:18:10.670985 speech_user_interface-0.1.9/README.md
+-rw-r--r--   0        0        0     1744 2024-04-13 08:21:20.836731 speech_user_interface-0.1.9/speech_user_interface/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-13 05:15:04.952636 speech_user_interface-0.1.9/speech_user_interface/compare_strings.py
+-rw-r--r--   0        0        0       49 2024-04-13 04:37:33.298012 speech_user_interface-0.1.9/speech_user_interface/CONSTANTS.py
+-rw-r--r--   0        0        0      630 2024-04-13 05:12:32.571540 speech_user_interface-0.1.9/speech_user_interface/load_vosk_model.py
+-rw-r--r--   0        0        0     1416 2024-04-13 05:50:57.320876 speech_user_interface-0.1.9/speech_user_interface/read_in_speech.py
+-rw-r--r--   0        0        0      462 2024-04-13 05:25:09.140507 speech_user_interface-0.1.9/speech_user_interface/send_text_to_chatgpt.py
+-rw-r--r--   0        0        0      490 2024-04-13 04:33:28.596917 speech_user_interface-0.1.9/speech_user_interface/speak_text.py
+-rw-r--r--   0        0        0     1776 1970-01-01 00:00:00.000000 speech_user_interface-0.1.9/PKG-INFO
```

### Comparing `speech_user_interface-0.1.8/pyproject.toml` & `speech_user_interface-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "speech_user_interface"
-version = "0.1.8"
+version = "0.1.9"
 description = "A universal speech user interface for wrapping applications to provide them with a user interface that uses speech rather than text commands or traditional user interfaces"
 authors = ["David Piper <dbpiper@gmail.com>"]
 readme = "README.md"
-include = ["speech_user_interface/models/vosk-model-en-us-0.22"]
+include = ["models"]
 
 [tool.poetry.scripts]
 sui = "speech_user_interface:main"
 
-[tool.poetry.dependencies]
+
+[tool.poetry.dependencies] # Include specific files or directories
 python = "^3.11"
 pandas = "^2.1.4"
 numpy = "^1.26.3"
 pydash = "^7.0.7"
 einops = "^0.7.0"
 tenacity = "^8.2.3"
 tqdm = "^4.66.2"
```

### Comparing `speech_user_interface-0.1.8/README.md` & `speech_user_interface-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.8/speech_user_interface/__init__.py` & `speech_user_interface-0.1.9/speech_user_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.8/speech_user_interface/load_vosk_model.py` & `speech_user_interface-0.1.9/speech_user_interface/load_vosk_model.py`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.8/speech_user_interface/read_in_speech.py` & `speech_user_interface-0.1.9/speech_user_interface/read_in_speech.py`

 * *Files identical despite different names*

### Comparing `speech_user_interface-0.1.8/PKG-INFO` & `speech_user_interface-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speech_user_interface
-Version: 0.1.8
+Version: 0.1.9
 Summary: A universal speech user interface for wrapping applications to provide them with a user interface that uses speech rather than text commands or traditional user interfaces
 Author: David Piper
 Author-email: dbpiper@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

