# Comparing `tmp/furchain-0.1.3.tar.gz` & `tmp/furchain-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furchain-0.1.3.tar", max compression
+gzip compressed data, was "furchain-0.1.4.tar", max compression
```

## Comparing `furchain-0.1.3.tar` & `furchain-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     3207 2024-04-13 05:23:28.617788 furchain-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/__init__.py
--rw-r--r--   0        0        0       59 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/conversion/__init__.py
--rw-r--r--   0        0        0      751 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/conversion/gpt_sovits_vc.py
--rw-r--r--   0        0        0     3282 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/conversion/rvc.py
--rw-r--r--   0        0        0     1047 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/conversion/sovits.py
--rw-r--r--   0        0        0     3943 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/schema.py
--rw-r--r--   0        0        0       34 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/speech/__init__.py
--rw-r--r--   0        0        0     3716 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/speech/gpt_sovits.py
--rw-r--r--   0        0        0       27 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/transcriptions/__init__.py
--rw-r--r--   0        0        0    10530 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/transcriptions/funasr.py
--rw-r--r--   0        0        0      230 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/__init__.py
--rw-r--r--   0        0        0     3141 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/audio_editor.py
--rw-r--r--   0        0        0     3872 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/audio_iterator.py
--rw-r--r--   0        0        0     3097 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/audio_separator.py
--rw-r--r--   0        0        0     2934 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/convert.py
--rw-r--r--   0        0        0      897 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/get_format.py
--rw-r--r--   0        0        0     3557 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/microphone.py
--rw-r--r--   0        0        0     2136 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/audio/utils/play.py
--rw-r--r--   0        0        0     2009 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/config.py
--rw-r--r--   0        0        0        0 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/image/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 05:23:28.617788 furchain-0.1.3/furchain/image/captions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/image/generation/__init__.py
--rw-r--r--   0        0        0      881 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/image/generation/stable_diffusion_webui.py
--rw-r--r--   0        0        0      127 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/image/schema.py
--rw-r--r--   0        0        0        0 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/interaction/__init__.py
--rw-r--r--   0        0        0     6710 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/interaction/actions.py
--rw-r--r--   0        0        0     1647 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/interaction/schema.py
--rw-r--r--   0        0        0     3171 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/interaction/tools.py
--rw-r--r--   0        0        0     2796 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/logger.py
--rw-r--r--   0        0        0      101 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/__init__.py
--rw-r--r--   0        0        0     2314 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/callbacks.py
--rw-r--r--   0        0        0    14081 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/chat_format.py
--rw-r--r--   0        0        0     7241 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/chat_message_history.py
--rw-r--r--   0        0        0     6789 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/chat_prompt_templates.py
--rw-r--r--   0        0        0      615 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/grammars.py
--rw-r--r--   0        0        0     4297 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/llama_cpp_client.py
--rw-r--r--   0        0        0     2779 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/output_parsers.py
--rw-r--r--   0        0        0    53992 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/text/schema.py
--rw-r--r--   0        0        0        0 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/utils/__init__.py
--rw-r--r--   0        0        0     3208 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/utils/broadcaster.py
--rw-r--r--   0        0        0     1998 2024-04-13 05:23:28.621788 furchain-0.1.3/furchain/utils/iterator.py
--rw-r--r--   0        0        0     1029 2024-04-13 05:23:28.621788 furchain-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 furchain-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3207 2024-04-14 09:13:42.783499 furchain-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 09:13:42.783499 furchain-0.1.4/furchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:13:42.783499 furchain-0.1.4/furchain/audio/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/conversion/__init__.py
+-rw-r--r--   0        0        0      751 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/conversion/gpt_sovits_vc.py
+-rw-r--r--   0        0        0     3282 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/conversion/rvc.py
+-rw-r--r--   0        0        0     1047 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/conversion/sovits.py
+-rw-r--r--   0        0        0     3943 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/schema.py
+-rw-r--r--   0        0        0       34 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/speech/__init__.py
+-rw-r--r--   0        0        0     3716 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/speech/gpt_sovits.py
+-rw-r--r--   0        0        0       27 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/transcriptions/__init__.py
+-rw-r--r--   0        0        0    10530 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/transcriptions/funasr.py
+-rw-r--r--   0        0        0      230 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/__init__.py
+-rw-r--r--   0        0        0     3141 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/audio_editor.py
+-rw-r--r--   0        0        0     3872 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/audio_iterator.py
+-rw-r--r--   0        0        0     3097 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/audio_separator.py
+-rw-r--r--   0        0        0     2491 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/convert.py
+-rw-r--r--   0        0        0      897 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/get_format.py
+-rw-r--r--   0        0        0     3557 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/microphone.py
+-rw-r--r--   0        0        0     2136 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/play.py
+-rw-r--r--   0        0        0     2009 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/config.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/captions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/generation/__init__.py
+-rw-r--r--   0        0        0      881 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/generation/stable_diffusion_webui.py
+-rw-r--r--   0        0        0      127 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/schema.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/interaction/__init__.py
+-rw-r--r--   0        0        0     6710 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/interaction/actions.py
+-rw-r--r--   0        0        0     1647 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/interaction/schema.py
+-rw-r--r--   0        0        0     3171 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/interaction/tools.py
+-rw-r--r--   0        0        0     2796 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/logger.py
+-rw-r--r--   0        0        0      101 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/__init__.py
+-rw-r--r--   0        0        0     2314 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/callbacks.py
+-rw-r--r--   0        0        0    14081 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/chat_format.py
+-rw-r--r--   0        0        0     7241 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/chat_message_history.py
+-rw-r--r--   0        0        0     6789 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/chat_prompt_templates.py
+-rw-r--r--   0        0        0      615 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/grammars.py
+-rw-r--r--   0        0        0     4297 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/llama_cpp_client.py
+-rw-r--r--   0        0        0     2779 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/output_parsers.py
+-rw-r--r--   0        0        0    53992 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/schema.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/utils/__init__.py
+-rw-r--r--   0        0        0     3208 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/utils/broadcaster.py
+-rw-r--r--   0        0        0     1998 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/utils/iterator.py
+-rw-r--r--   0        0        0     1029 2024-04-14 09:13:42.787500 furchain-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 furchain-0.1.4/PKG-INFO
```

### Comparing `furchain-0.1.3/README.md` & `furchain-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/conversion/gpt_sovits_vc.py` & `furchain-0.1.4/furchain/audio/conversion/gpt_sovits_vc.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/conversion/rvc.py` & `furchain-0.1.4/furchain/audio/conversion/rvc.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/conversion/sovits.py` & `furchain-0.1.4/furchain/audio/conversion/sovits.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/schema.py` & `furchain-0.1.4/furchain/audio/schema.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/speech/gpt_sovits.py` & `furchain-0.1.4/furchain/audio/speech/gpt_sovits.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/transcriptions/funasr.py` & `furchain-0.1.4/furchain/audio/transcriptions/funasr.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/utils/audio_editor.py` & `furchain-0.1.4/furchain/audio/utils/audio_editor.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/utils/audio_iterator.py` & `furchain-0.1.4/furchain/audio/utils/audio_iterator.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/utils/audio_separator.py` & `furchain-0.1.4/furchain/audio/utils/audio_separator.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/utils/convert.py` & `furchain-0.1.4/furchain/audio/utils/convert.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,28 @@
 import os
 import tempfile
 from typing import Literal
 
 import ffmpeg
 from pydub import AudioSegment
 
-from furchain.audio.utils.play import get_format_from_magic_bytes
-
 
 def convert_to_pcm(audio_bytes: bytes, sample_rate: int = 16000) -> bytes:
     """
     This function converts an audio file to PCM format.
 
     Args:
         audio_bytes (bytes): The audio file in bytes.
         sample_rate (int, optional): The sample rate for the audio file. Default is 16000.
 
     Returns:
         bytes: The audio file in PCM format.
     """
-    audio_format = get_format_from_magic_bytes(audio_bytes)
-
-    if audio_format == 'unknown':
-        raise ValueError("Unknown audio format. Cannot convert to PCM.")
 
-    audio = AudioSegment.from_file(io.BytesIO(audio_bytes), format=audio_format)
+    audio = AudioSegment.from_file(io.BytesIO(audio_bytes))
 
     buffer = io.BytesIO()
     audio.export(buffer, format='wav', parameters=["-ar", str(sample_rate)])
 
     buffer.seek(0)
     wav_data = buffer.read()
 
@@ -45,20 +39,16 @@
     Args:
         audio_bytes (bytes): The audio file in bytes.
         sample_rate (int, optional): The sample rate for the audio file. Default is 16000.
 
     Returns:
         bytes: The audio file in MP3 format.
     """
-    audio_format = get_format_from_magic_bytes(audio_bytes)
-
-    if audio_format == 'unknown':
-        raise ValueError("Unknown audio format. Cannot convert to MP3.")
 
-    audio = AudioSegment.from_file(io.BytesIO(audio_bytes), format=audio_format)
+    audio = AudioSegment.from_file(io.BytesIO(audio_bytes), )
 
     buffer = io.BytesIO()
     audio.export(buffer, format='mp3', parameters=["-ar", str(sample_rate)])
 
     buffer.seek(0)
     mp3_data = buffer.read()
```

### Comparing `furchain-0.1.3/furchain/audio/utils/get_format.py` & `furchain-0.1.4/furchain/audio/utils/get_format.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/utils/microphone.py` & `furchain-0.1.4/furchain/audio/utils/microphone.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/audio/utils/play.py` & `furchain-0.1.4/furchain/audio/utils/play.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/config.py` & `furchain-0.1.4/furchain/config.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/image/generation/stable_diffusion_webui.py` & `furchain-0.1.4/furchain/image/generation/stable_diffusion_webui.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/interaction/actions.py` & `furchain-0.1.4/furchain/interaction/actions.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/interaction/schema.py` & `furchain-0.1.4/furchain/interaction/schema.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/interaction/tools.py` & `furchain-0.1.4/furchain/interaction/tools.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/logger.py` & `furchain-0.1.4/furchain/logger.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/text/callbacks.py` & `furchain-0.1.4/furchain/text/callbacks.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/text/chat_format.py` & `furchain-0.1.4/furchain/text/chat_format.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/text/chat_message_history.py` & `furchain-0.1.4/furchain/text/chat_message_history.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/text/chat_prompt_templates.py` & `furchain-0.1.4/furchain/text/chat_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/text/grammars.py` & `furchain-0.1.4/furchain/text/grammars.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/text/llama_cpp_client.py` & `furchain-0.1.4/furchain/text/llama_cpp_client.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/text/output_parsers.py` & `furchain-0.1.4/furchain/text/output_parsers.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/text/schema.py` & `furchain-0.1.4/furchain/text/schema.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/utils/broadcaster.py` & `furchain-0.1.4/furchain/utils/broadcaster.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/furchain/utils/iterator.py` & `furchain-0.1.4/furchain/utils/iterator.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.3/pyproject.toml` & `furchain-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "furchain"
-version = "0.1.3"
+version = "0.1.4"
 description = "FurChain is an innovative toolkit for creating and interacting with digital personas, complete with voice cloning and role-playing capabilities. It offers a suite of tools for real-time voice manipulation, chatbot creation, and text-based RPG adventures, all while being open-source and operable offline."
 authors = ["markyfsun <mark@furchain.xyz>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 websocket-client = "^1.7.0"
```

### Comparing `furchain-0.1.3/PKG-INFO` & `furchain-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furchain
-Version: 0.1.3
+Version: 0.1.4
 Summary: FurChain is an innovative toolkit for creating and interacting with digital personas, complete with voice cloning and role-playing capabilities. It offers a suite of tools for real-time voice manipulation, chatbot creation, and text-based RPG adventures, all while being open-source and operable offline.
 Author: markyfsun
 Author-email: mark@furchain.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

