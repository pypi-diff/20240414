# Comparing `tmp/RealTimeSTT-0.1.8.tar.gz` & `tmp/RealTimeSTT-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RealTimeSTT-0.1.8.tar", last modified: Fri Dec 15 12:32:59 2023, max compression
+gzip compressed data, was "RealTimeSTT-0.1.9.tar", last modified: Mon Jan 29 17:07:55 2024, max compression
```

## Comparing `RealTimeSTT-0.1.8.tar` & `RealTimeSTT-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 12:32:59.941244 RealTimeSTT-0.1.8/
--rw-rw-rw-   0        0        0    15491 2023-12-15 12:32:59.940244 RealTimeSTT-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    14523 2023-11-10 18:33:57.000000 RealTimeSTT-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-15 12:32:59.936240 RealTimeSTT-0.1.8/RealTimeSTT.egg-info/
--rw-rw-rw-   0        0        0    15491 2023-12-15 12:32:59.000000 RealTimeSTT-0.1.8/RealTimeSTT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-12-15 12:32:59.000000 RealTimeSTT-0.1.8/RealTimeSTT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-15 12:32:59.000000 RealTimeSTT-0.1.8/RealTimeSTT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-12-15 12:32:59.000000 RealTimeSTT-0.1.8/RealTimeSTT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-12-15 12:32:59.000000 RealTimeSTT-0.1.8/RealTimeSTT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-15 12:32:59.938242 RealTimeSTT-0.1.8/RealtimeSTT/
--rw-rw-rw-   0        0        0       47 2023-08-27 18:40:31.000000 RealTimeSTT-0.1.8/RealtimeSTT/__init__.py
--rw-rw-rw-   0        0        0    63623 2023-12-15 12:31:25.000000 RealTimeSTT-0.1.8/RealtimeSTT/audio_recorder.py
--rw-rw-rw-   0        0        0       42 2023-12-15 12:32:59.941244 RealTimeSTT-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-12-15 12:30:06.000000 RealTimeSTT-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-29 17:07:55.780884 RealTimeSTT-0.1.9/
+-rw-rw-rw-   0        0        0     1090 2023-12-15 12:45:51.000000 RealTimeSTT-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    16971 2024-01-29 17:07:55.779883 RealTimeSTT-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15980 2024-01-29 17:07:44.000000 RealTimeSTT-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-29 17:07:55.775880 RealTimeSTT-0.1.9/RealTimeSTT.egg-info/
+-rw-rw-rw-   0        0        0    16971 2024-01-29 17:07:55.000000 RealTimeSTT-0.1.9/RealTimeSTT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-01-29 17:07:55.000000 RealTimeSTT-0.1.9/RealTimeSTT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-29 17:07:55.000000 RealTimeSTT-0.1.9/RealTimeSTT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-01-29 17:07:55.000000 RealTimeSTT-0.1.9/RealTimeSTT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-01-29 17:07:55.000000 RealTimeSTT-0.1.9/RealTimeSTT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-29 17:07:55.778882 RealTimeSTT-0.1.9/RealtimeSTT/
+-rw-rw-rw-   0        0        0       47 2023-08-27 18:40:31.000000 RealTimeSTT-0.1.9/RealtimeSTT/__init__.py
+-rw-rw-rw-   0        0        0    66519 2024-01-29 16:56:32.000000 RealTimeSTT-0.1.9/RealtimeSTT/audio_recorder.py
+-rw-rw-rw-   0        0        0       42 2024-01-29 17:07:55.780884 RealTimeSTT-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2024-01-29 17:03:45.000000 RealTimeSTT-0.1.9/setup.py
```

### Comparing `RealTimeSTT-0.1.8/PKG-INFO` & `RealTimeSTT-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: RealTimeSTT
-Version: 0.1.8
+Version: 0.1.9
 Summary: A fast Voice Activity Detection and Transcription System
 Home-page: https://github.com/KoljaB/RealTimeSTT
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,audio,transcription,speech-to-text,voice-activity-detection,VAD,real-time-transcription,ambient-noise-detection,microphone-input,faster_whisper,speech-recognition,voice-assistants,audio-processing,buffered-transcription,pyaudio,ambient-noise-level,voice-deactivity
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: PyAudio==0.2.14
 Requires-Dist: faster-whisper==0.10.0
 Requires-Dist: pvporcupine==1.9.5
 Requires-Dist: webrtcvad==2.0.10
 Requires-Dist: halo==0.0.31
-Requires-Dist: torch==2.1.1
-Requires-Dist: torchaudio==2.1.1
+Requires-Dist: torch==2.1.2
+Requires-Dist: torchaudio==2.1.2
 
 
 # RealtimeSTT
 
 *Easy-to-use, low-latency speech-to-text library for realtime applications*
 
 ## About the Project
@@ -33,25 +34,35 @@
 - **Voice Assistants**
 - Applications requiring **fast and precise** speech-to-text conversion
 
 https://github.com/KoljaB/RealtimeSTT/assets/7604638/207cb9a2-4482-48e7-9d2b-0722c3ee6d14
 
 ### Updates
 
+#### v0.1.9
+- switched to torch.multiprocessing
+- added compute_type, input_device_index and gpu_device_index parameters
+- recorder.text() interruptable with recorder.abort()
+- fix for #20
+
+#### v0.1.8
+- added [example](https://github.com/KoljaB/RealtimeSTT/tree/master/example_browserclient) how to realtime transcribe from browser microphone
+- large-v3 whisper model now supported (upgrade to faster_whisper 0.10.0)
+- added feed_audio() and use_microphone parameter to feed chunks
+
 #### v0.1.7
 - Bugfix for Mac OS Installation (multiprocessing / queue.size())
 - KeyboardInterrupt handling (now abortable with CTRL+C)
 - Bugfix for spinner handling (could lead to exception in some cases)
 
 #### v0.1.6
 - Implements context manager protocol (recorder can be used in a `with` statement)
 - Bugfix for resource management in shutdown method
 
 #### v0.1.5
-
 - Bugfix for detection of short speech right after sentence detection (the problem mentioned in the video)
 - Main transcription and recording moved into separate process contexts with multiprocessing
 
 > **Hint:** *Since we use the `multiprocessing` module now, ensure to include the `if __name__ == '__main__':` protection in your code to prevent unexpected behavior, especially on platforms like Windows. For a detailed explanation on why this is important, visit the [official Python documentation on `multiprocessing`](https://docs.python.org/3/library/multiprocessing.html#multiprocessing-programming).*
 
 ### Features
 
@@ -196,14 +207,22 @@
 def my_stop_callback():
     print("Recording stopped!")
 
 recorder = AudioToTextRecorder(on_recording_start=my_start_callback,
                                on_recording_stop=my_stop_callback)
 ```
 
+### Feed chunks
+
+If you don't want to use the local microphone set use_microphone parameter to false and provide raw PCM audiochunks in 16-bit mono (samplerate 16000) with this method:
+
+```python
+recorder.feed_audio(audio_chunk)
+```
+
 ### Shutdown
 
 You can shutdown the recorder safely by using the context manager protocol:
 
 ```python
 with AudioToTextRecorder() as recorder:
     [...]
@@ -257,26 +276,34 @@
 
 #### General Parameters
 
 - **model** (str, default="tiny"): Model size or path for transcription.
     - Options: 'tiny', 'tiny.en', 'base', 'base.en', 'small', 'small.en', 'medium', 'medium.en', 'large-v1', 'large-v2'.
     - Note: If a size is provided, the model will be downloaded from the Hugging Face Hub.
 
-- **language** (str, default=""): Language code for transcription. If left empty, the model will try to auto-detect the language.
+- **language** (str, default=""): Language code for transcription. If left empty, the model will try to auto-detect the language. Supported language codes are listed in [Whisper Tokenizer library](https://github.com/openai/whisper/blob/main/whisper/tokenizer.py).
+
+- **compute_type** (str, default="default"): Specifies the type of computation to be used for transcription. See [Whisper Quantization](https://opennmt.net/CTranslate2/quantization.html)
+
+- **input_device_index** (int, default=0): Audio Input Device Index to use.
+
+- **gpu_device_index** (int, default=0): GPU Device Index to use. The model can also be loaded on multiple GPUs by passing a list of IDs (e.g. [0, 1, 2, 3]).
 
 - **on_recording_start**: A callable function triggered when recording starts.
 
 - **on_recording_stop**: A callable function triggered when recording ends.
 
 - **on_transcription_start**: A callable function triggered when transcription starts.
 
 - **ensure_sentence_starting_uppercase** (bool, default=True): Ensures that every sentence detected by the algorithm starts with an uppercase letter.
 
 - **ensure_sentence_ends_with_period** (bool, default=True): Ensures that every sentence that doesn't end with punctuation such as "?", "!" ends with a period
 
+- **use_microphone** (bool, default=True): Usage of local microphone for transcription. Set to False if you want to provide chunks with feed_audio method.
+
 - **spinner** (bool, default=True): Provides a spinner animation text with information about the current recorder state.
 
 - **level** (int, default=logging.WARNING): Logging level.
 
 #### Real-time Transcription Parameters
 
 > **Note**: *When enabling realtime description a GPU installation is strongly advised. Using realtime transcription may create high GPU loads.*
```

### Comparing `RealTimeSTT-0.1.8/README.md` & `RealTimeSTT-0.1.9/RealTimeSTT.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: RealTimeSTT
+Version: 0.1.9
+Summary: A fast Voice Activity Detection and Transcription System
+Home-page: https://github.com/KoljaB/RealTimeSTT
+Author: Kolja Beigel
+Author-email: kolja.beigel@web.de
+Keywords: real-time,audio,transcription,speech-to-text,voice-activity-detection,VAD,real-time-transcription,ambient-noise-detection,microphone-input,faster_whisper,speech-recognition,voice-assistants,audio-processing,buffered-transcription,pyaudio,ambient-noise-level,voice-deactivity
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: PyAudio==0.2.14
+Requires-Dist: faster-whisper==0.10.0
+Requires-Dist: pvporcupine==1.9.5
+Requires-Dist: webrtcvad==2.0.10
+Requires-Dist: halo==0.0.31
+Requires-Dist: torch==2.1.2
+Requires-Dist: torchaudio==2.1.2
+
 
 # RealtimeSTT
 
 *Easy-to-use, low-latency speech-to-text library for realtime applications*
 
 ## About the Project
 
@@ -12,25 +34,35 @@
 - **Voice Assistants**
 - Applications requiring **fast and precise** speech-to-text conversion
 
 https://github.com/KoljaB/RealtimeSTT/assets/7604638/207cb9a2-4482-48e7-9d2b-0722c3ee6d14
 
 ### Updates
 
+#### v0.1.9
+- switched to torch.multiprocessing
+- added compute_type, input_device_index and gpu_device_index parameters
+- recorder.text() interruptable with recorder.abort()
+- fix for #20
+
+#### v0.1.8
+- added [example](https://github.com/KoljaB/RealtimeSTT/tree/master/example_browserclient) how to realtime transcribe from browser microphone
+- large-v3 whisper model now supported (upgrade to faster_whisper 0.10.0)
+- added feed_audio() and use_microphone parameter to feed chunks
+
 #### v0.1.7
 - Bugfix for Mac OS Installation (multiprocessing / queue.size())
 - KeyboardInterrupt handling (now abortable with CTRL+C)
 - Bugfix for spinner handling (could lead to exception in some cases)
 
 #### v0.1.6
 - Implements context manager protocol (recorder can be used in a `with` statement)
 - Bugfix for resource management in shutdown method
 
 #### v0.1.5
-
 - Bugfix for detection of short speech right after sentence detection (the problem mentioned in the video)
 - Main transcription and recording moved into separate process contexts with multiprocessing
 
 > **Hint:** *Since we use the `multiprocessing` module now, ensure to include the `if __name__ == '__main__':` protection in your code to prevent unexpected behavior, especially on platforms like Windows. For a detailed explanation on why this is important, visit the [official Python documentation on `multiprocessing`](https://docs.python.org/3/library/multiprocessing.html#multiprocessing-programming).*
 
 ### Features
 
@@ -175,14 +207,22 @@
 def my_stop_callback():
     print("Recording stopped!")
 
 recorder = AudioToTextRecorder(on_recording_start=my_start_callback,
                                on_recording_stop=my_stop_callback)
 ```
 
+### Feed chunks
+
+If you don't want to use the local microphone set use_microphone parameter to false and provide raw PCM audiochunks in 16-bit mono (samplerate 16000) with this method:
+
+```python
+recorder.feed_audio(audio_chunk)
+```
+
 ### Shutdown
 
 You can shutdown the recorder safely by using the context manager protocol:
 
 ```python
 with AudioToTextRecorder() as recorder:
     [...]
@@ -236,26 +276,34 @@
 
 #### General Parameters
 
 - **model** (str, default="tiny"): Model size or path for transcription.
     - Options: 'tiny', 'tiny.en', 'base', 'base.en', 'small', 'small.en', 'medium', 'medium.en', 'large-v1', 'large-v2'.
     - Note: If a size is provided, the model will be downloaded from the Hugging Face Hub.
 
-- **language** (str, default=""): Language code for transcription. If left empty, the model will try to auto-detect the language.
+- **language** (str, default=""): Language code for transcription. If left empty, the model will try to auto-detect the language. Supported language codes are listed in [Whisper Tokenizer library](https://github.com/openai/whisper/blob/main/whisper/tokenizer.py).
+
+- **compute_type** (str, default="default"): Specifies the type of computation to be used for transcription. See [Whisper Quantization](https://opennmt.net/CTranslate2/quantization.html)
+
+- **input_device_index** (int, default=0): Audio Input Device Index to use.
+
+- **gpu_device_index** (int, default=0): GPU Device Index to use. The model can also be loaded on multiple GPUs by passing a list of IDs (e.g. [0, 1, 2, 3]).
 
 - **on_recording_start**: A callable function triggered when recording starts.
 
 - **on_recording_stop**: A callable function triggered when recording ends.
 
 - **on_transcription_start**: A callable function triggered when transcription starts.
 
 - **ensure_sentence_starting_uppercase** (bool, default=True): Ensures that every sentence detected by the algorithm starts with an uppercase letter.
 
 - **ensure_sentence_ends_with_period** (bool, default=True): Ensures that every sentence that doesn't end with punctuation such as "?", "!" ends with a period
 
+- **use_microphone** (bool, default=True): Usage of local microphone for transcription. Set to False if you want to provide chunks with feed_audio method.
+
 - **spinner** (bool, default=True): Provides a spinner animation text with information about the current recorder state.
 
 - **level** (int, default=logging.WARNING): Logging level.
 
 #### Real-time Transcription Parameters
 
 > **Note**: *When enabling realtime description a GPU installation is strongly advised. Using realtime transcription may create high GPU loads.*
@@ -318,8 +366,8 @@
 
 MIT
 
 ## Author
 
 Kolja Beigel  
 Email: kolja.beigel@web.de  
-[GitHub](https://github.com/KoljaB/RealtimeSTT)
+[GitHub](https://github.com/KoljaB/RealtimeSTT)
```

### Comparing `RealTimeSTT-0.1.8/RealTimeSTT.egg-info/PKG-INFO` & `RealTimeSTT-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: RealTimeSTT
-Version: 0.1.8
-Summary: A fast Voice Activity Detection and Transcription System
-Home-page: https://github.com/KoljaB/RealTimeSTT
-Author: Kolja Beigel
-Author-email: kolja.beigel@web.de
-Keywords: real-time,audio,transcription,speech-to-text,voice-activity-detection,VAD,real-time-transcription,ambient-noise-detection,microphone-input,faster_whisper,speech-recognition,voice-assistants,audio-processing,buffered-transcription,pyaudio,ambient-noise-level,voice-deactivity
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: PyAudio==0.2.14
-Requires-Dist: faster-whisper==0.10.0
-Requires-Dist: pvporcupine==1.9.5
-Requires-Dist: webrtcvad==2.0.10
-Requires-Dist: halo==0.0.31
-Requires-Dist: torch==2.1.1
-Requires-Dist: torchaudio==2.1.1
-
 
 # RealtimeSTT
 
 *Easy-to-use, low-latency speech-to-text library for realtime applications*
 
 ## About the Project
 
@@ -33,25 +12,35 @@
 - **Voice Assistants**
 - Applications requiring **fast and precise** speech-to-text conversion
 
 https://github.com/KoljaB/RealtimeSTT/assets/7604638/207cb9a2-4482-48e7-9d2b-0722c3ee6d14
 
 ### Updates
 
+#### v0.1.9
+- switched to torch.multiprocessing
+- added compute_type, input_device_index and gpu_device_index parameters
+- recorder.text() interruptable with recorder.abort()
+- fix for #20
+
+#### v0.1.8
+- added [example](https://github.com/KoljaB/RealtimeSTT/tree/master/example_browserclient) how to realtime transcribe from browser microphone
+- large-v3 whisper model now supported (upgrade to faster_whisper 0.10.0)
+- added feed_audio() and use_microphone parameter to feed chunks
+
 #### v0.1.7
 - Bugfix for Mac OS Installation (multiprocessing / queue.size())
 - KeyboardInterrupt handling (now abortable with CTRL+C)
 - Bugfix for spinner handling (could lead to exception in some cases)
 
 #### v0.1.6
 - Implements context manager protocol (recorder can be used in a `with` statement)
 - Bugfix for resource management in shutdown method
 
 #### v0.1.5
-
 - Bugfix for detection of short speech right after sentence detection (the problem mentioned in the video)
 - Main transcription and recording moved into separate process contexts with multiprocessing
 
 > **Hint:** *Since we use the `multiprocessing` module now, ensure to include the `if __name__ == '__main__':` protection in your code to prevent unexpected behavior, especially on platforms like Windows. For a detailed explanation on why this is important, visit the [official Python documentation on `multiprocessing`](https://docs.python.org/3/library/multiprocessing.html#multiprocessing-programming).*
 
 ### Features
 
@@ -196,14 +185,22 @@
 def my_stop_callback():
     print("Recording stopped!")
 
 recorder = AudioToTextRecorder(on_recording_start=my_start_callback,
                                on_recording_stop=my_stop_callback)
 ```
 
+### Feed chunks
+
+If you don't want to use the local microphone set use_microphone parameter to false and provide raw PCM audiochunks in 16-bit mono (samplerate 16000) with this method:
+
+```python
+recorder.feed_audio(audio_chunk)
+```
+
 ### Shutdown
 
 You can shutdown the recorder safely by using the context manager protocol:
 
 ```python
 with AudioToTextRecorder() as recorder:
     [...]
@@ -257,26 +254,34 @@
 
 #### General Parameters
 
 - **model** (str, default="tiny"): Model size or path for transcription.
     - Options: 'tiny', 'tiny.en', 'base', 'base.en', 'small', 'small.en', 'medium', 'medium.en', 'large-v1', 'large-v2'.
     - Note: If a size is provided, the model will be downloaded from the Hugging Face Hub.
 
-- **language** (str, default=""): Language code for transcription. If left empty, the model will try to auto-detect the language.
+- **language** (str, default=""): Language code for transcription. If left empty, the model will try to auto-detect the language. Supported language codes are listed in [Whisper Tokenizer library](https://github.com/openai/whisper/blob/main/whisper/tokenizer.py).
+
+- **compute_type** (str, default="default"): Specifies the type of computation to be used for transcription. See [Whisper Quantization](https://opennmt.net/CTranslate2/quantization.html)
+
+- **input_device_index** (int, default=0): Audio Input Device Index to use.
+
+- **gpu_device_index** (int, default=0): GPU Device Index to use. The model can also be loaded on multiple GPUs by passing a list of IDs (e.g. [0, 1, 2, 3]).
 
 - **on_recording_start**: A callable function triggered when recording starts.
 
 - **on_recording_stop**: A callable function triggered when recording ends.
 
 - **on_transcription_start**: A callable function triggered when transcription starts.
 
 - **ensure_sentence_starting_uppercase** (bool, default=True): Ensures that every sentence detected by the algorithm starts with an uppercase letter.
 
 - **ensure_sentence_ends_with_period** (bool, default=True): Ensures that every sentence that doesn't end with punctuation such as "?", "!" ends with a period
 
+- **use_microphone** (bool, default=True): Usage of local microphone for transcription. Set to False if you want to provide chunks with feed_audio method.
+
 - **spinner** (bool, default=True): Provides a spinner animation text with information about the current recorder state.
 
 - **level** (int, default=logging.WARNING): Logging level.
 
 #### Real-time Transcription Parameters
 
 > **Note**: *When enabling realtime description a GPU installation is strongly advised. Using realtime transcription may create high GPU loads.*
@@ -339,8 +344,8 @@
 
 MIT
 
 ## Author
 
 Kolja Beigel  
 Email: kolja.beigel@web.de  
-[GitHub](https://github.com/KoljaB/RealtimeSTT)
+[GitHub](https://github.com/KoljaB/RealtimeSTT)
```

### Comparing `RealTimeSTT-0.1.8/RealtimeSTT/audio_recorder.py` & `RealTimeSTT-0.1.9/RealtimeSTT/audio_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 - Fast Transcription: Returns the transcribed text from the audio as fast
   as possible.
 
 Author: Kolja Beigel
 
 """
 
-from multiprocessing import Process, Pipe, Event, Manager
+import torch.multiprocessing as mp
+from typing import List, Union
 import faster_whisper
 import collections
 import numpy as np
 import pvporcupine
 import traceback
 import threading
 import webrtcvad
@@ -39,14 +40,15 @@
 import logging
 import struct
 import torch
 import halo
 import time
 import os
 import re
+import gc
 
 INIT_MODEL_TRANSCRIPTION = "tiny"
 INIT_MODEL_TRANSCRIPTION_REALTIME = "tiny"
 INIT_REALTIME_PROCESSING_PAUSE = 0.2
 INIT_SILERO_SENSITIVITY = 0.4
 INIT_WEBRTC_SENSITIVITY = 3
 INIT_POST_SPEECH_SILENCE_DURATION = 0.6
@@ -70,14 +72,17 @@
     voice activity, and then transcribing the captured audio using the
     `faster_whisper` model.
     """
 
     def __init__(self,
                  model: str = INIT_MODEL_TRANSCRIPTION,
                  language: str = "",
+                 compute_type: str = "default",
+                 input_device_index: int = 0,
+                 gpu_device_index: Union[int, List[int]] = 0,
                  on_recording_start=None,
                  on_recording_stop=None,
                  on_transcription_start=None,
                  ensure_sentence_starting_uppercase=True,
                  ensure_sentence_ends_with_period=True,
                  use_microphone=True,
                  spinner=True,
@@ -132,14 +137,24 @@
                 'small', 'small.en', 'medium', 'medium.en', 'large-v1',
                 'large-v2'.
                 If a specific size is provided, the model is downloaded
                 from the Hugging Face Hub.
         - language (str, default=""): Language code for speech-to-text engine.
             If not specified, the model will attempt to detect the language
             automatically.
+        - compute_type (str, default="default"): Specifies the type of
+            computation to be used for transcription.
+            See https://opennmt.net/CTranslate2/quantization.html.
+        - input_device_index (int, default=0): The index of the audio input
+            device to use.
+        - gpu_device_index (int, default=0): Device ID to use.
+            The model can also be loaded on multiple GPUs by passing a list of
+            IDs (e.g. [0, 1, 2, 3]). In that case, multiple transcriptions can
+            run in parallel when transcribe() is called from multiple Python
+            threads
         - on_recording_start (callable, default=None): Callback function to be
             called when recording of audio to be transcripted starts.
         - on_recording_stop (callable, default=None): Callback function to be
             called when recording of audio to be transcripted stops.
         - on_transcription_start (callable, default=None): Callback function
             to be called when transcription of audio to text starts.
         - ensure_sentence_starting_uppercase (bool, default=True): Ensures
@@ -234,23 +249,27 @@
 
         Raises:
             Exception: Errors related to initializing transcription
             model, wake word detection, or audio recording.
         """
 
         self.language = language
+        self.compute_type = compute_type
+        self.input_device_index = input_device_index
+        self.gpu_device_index = gpu_device_index
         self.wake_words = wake_words
         self.wake_word_activation_delay = wake_word_activation_delay
         self.wake_word_timeout = wake_word_timeout
         self.ensure_sentence_starting_uppercase = (
             ensure_sentence_starting_uppercase
         )
         self.ensure_sentence_ends_with_period = (
             ensure_sentence_ends_with_period
         )
+        self.use_microphone = use_microphone
         self.min_gap_between_recordings = min_gap_between_recordings
         self.min_length_of_recording = min_length_of_recording
         self.pre_recording_buffer_duration = pre_recording_buffer_duration
         self.post_speech_silence_duration = post_speech_silence_duration
         self.on_recording_start = on_recording_start
         self.on_recording_stop = on_recording_stop
         self.on_wakeword_detected = on_wakeword_detected
@@ -268,16 +287,15 @@
         )
         self.on_realtime_transcription_stabilized = (
             on_realtime_transcription_stabilized
         )
         self.allowed_latency_limit = ALLOWED_LATENCY_LIMIT
 
         self.level = level
-        manager = Manager()
-        self.audio_queue = manager.Queue()
+        self.audio_queue = mp.Queue()
         self.buffer_size = BUFFER_SIZE
         self.sample_rate = SAMPLE_RATE
         self.recording_start_time = 0
         self.recording_stop_time = 0
         self.wake_word_detect_time = 0
         self.silero_check_time = 0
         self.silero_working = False
@@ -319,58 +337,71 @@
         console_handler.setFormatter(logging.Formatter(log_format))
 
         # Add the handlers to the logger
         logger.addHandler(file_handler)
         logger.addHandler(console_handler)
 
         self.is_shut_down = False
-        self.shutdown_event = Event()
+        self.shutdown_event = mp.Event()
 
         logging.info("Starting RealTimeSTT")
 
-        # Start transcription process
-        self.interrupt_stop_event = Event()
-        self.main_transcription_ready_event = Event()
-        self.parent_transcription_pipe, child_transcription_pipe = Pipe()
+        # Start transcription worker process
+        try:
+            # Only set the start method if it hasn't been set already
+            if mp.get_start_method(allow_none=True) is None:
+                mp.set_start_method("spawn")
+        except RuntimeError as e:
+            print("Start method has already been set. Details:", e)
+
+        self.interrupt_stop_event = mp.Event()
+        self.was_interrupted = mp.Event()
+        self.main_transcription_ready_event = mp.Event()
+        self.parent_transcription_pipe, child_transcription_pipe = mp.Pipe()
 
-        self.transcript_process = Process(
+        self.transcript_process = mp.Process(
             target=AudioToTextRecorder._transcription_worker,
             args=(
                 child_transcription_pipe,
                 model,
+                self.compute_type,
+                self.gpu_device_index,
                 self.main_transcription_ready_event,
                 self.shutdown_event,
                 self.interrupt_stop_event
             )
         )
         self.transcript_process.start()
 
         # Start audio data reading process
         if use_microphone:
-            self.reader_process = Process(
+            self.reader_process = mp.Process(
                 target=AudioToTextRecorder._audio_data_worker,
                 args=(
                     self.audio_queue,
                     self.sample_rate,
                     self.buffer_size,
+                    self.input_device_index,
                     self.shutdown_event,
                     self.interrupt_stop_event
                 )
             )
             self.reader_process.start()
 
         # Initialize the realtime transcription model
         if self.enable_realtime_transcription:
             try:
                 logging.info("Initializing faster_whisper realtime "
                              f"transcription model {self.realtime_model_type}"
                              )
                 self.realtime_model_type = faster_whisper.WhisperModel(
                     model_size_or_path=self.realtime_model_type,
-                    device='cuda' if torch.cuda.is_available() else 'cpu'
+                    device='cuda' if torch.cuda.is_available() else 'cpu',
+                    compute_type=self.compute_type,
+                    device_index=self.gpu_device_index
                 )
 
             except Exception as e:
                 logging.exception("Error initializing faster_whisper "
                                   f"realtime transcription model: {e}"
                                   )
                 raise
@@ -469,20 +500,19 @@
         # Wait for transcription models to start
         logging.debug('Waiting for main transcription model to start')
         self.main_transcription_ready_event.wait()
         logging.debug('Main transcription model ready')
 
         logging.debug('RealtimeSTT initialization completed successfully')
 
-        print(f"buffer_size: {self.buffer_size}")
-        print(f"samplerate: {self.sample_rate}")
-
     @staticmethod
     def _transcription_worker(conn,
                               model_path,
+                              compute_type,
+                              gpu_device_index,
                               ready_event,
                               shutdown_event,
                               interrupt_stop_event):
         """
         Worker method that handles the continuous
         process of transcribing audio data.
 
@@ -495,14 +525,17 @@
           terminate the transcription process.
 
         Args:
             conn (multiprocessing.Connection): The connection endpoint used
               for receiving audio data and sending transcription results.
             model_path (str): The path to the pre-trained faster_whisper model
               for transcription.
+            compute_type (str): Specifies the type of computation to be used
+                for transcription.
+            gpu_device_index (int): Device ID to use.
             ready_event (threading.Event): An event that is set when the
               transcription model is successfully initialized and ready.
             shutdown_event (threading.Event): An event that, when set,
               signals this worker method to terminate.
 
         Raises:
             Exception: If there is an error while initializing the
@@ -512,15 +545,17 @@
         logging.info("Initializing faster_whisper "
                      f"main transcription model {model_path}"
                      )
 
         try:
             model = faster_whisper.WhisperModel(
                 model_size_or_path=model_path,
-                device='cuda' if torch.cuda.is_available() else 'cpu'
+                device='cuda' if torch.cuda.is_available() else 'cpu',
+                compute_type=compute_type,
+                device_index=gpu_device_index
             )
 
         except Exception as e:
             logging.exception("Error initializing main "
                               f"faster_whisper transcription model: {e}"
                               )
             raise
@@ -559,14 +594,15 @@
                               )
                 break
 
     @staticmethod
     def _audio_data_worker(audio_queue,
                            sample_rate,
                            buffer_size,
+                           input_device_index,
                            shutdown_event,
                            interrupt_stop_event):
         """
         Worker method that handles the audio recording process.
 
         This method runs in a separate process and is responsible for:
         - Setting up the audio input stream for recording.
@@ -579,14 +615,15 @@
 
         Args:
             audio_queue (queue.Queue): A queue where recorded audio
               data is placed.
             sample_rate (int): The sample rate of the audio input stream.
             buffer_size (int): The size of the buffer used in the audio
               input stream.
+            input_device_index (int): The index of the audio input device
             shutdown_event (threading.Event): An event that, when set, signals
               this worker method to terminate.
 
         Raises:
             Exception: If there is an error while initializing the audio
               recording.
         """
@@ -596,15 +633,16 @@
 
         try:
             audio_interface = pyaudio.PyAudio()
             stream = audio_interface.open(rate=sample_rate,
                                           format=pyaudio.paInt16,
                                           channels=1,
                                           input=True,
-                                          frames_per_buffer=buffer_size
+                                          frames_per_buffer=buffer_size,
+                                          input_device_index=input_device_index,
                                           )
 
         except Exception as e:
             logging.exception("Error initializing pyaudio "
                               f"audio recording: {e}"
                               )
             raise
@@ -643,14 +681,28 @@
                           "finished due to KeyboardInterrupt"
                           )
         finally:
             stream.stop_stream()
             stream.close()
             audio_interface.terminate()
 
+    def wakeup(self):
+        """
+        If in wake work modus, wake up as if a wake word was spoken.
+        """
+        self.listen_start = time.time()
+
+    def abort(self):
+        self.start_recording_on_voice_activity = False
+        self.stop_recording_on_voice_deactivity = False
+        self._set_state("inactive")
+        self.interrupt_stop_event.set()
+        self.was_interrupted.wait()
+        self.was_interrupted.clear()
+
     def wait_audio(self):
         """
         Waits for the start and completion of the audio recording process.
 
         This method is responsible for:
         - Waiting for voice activity to begin recording if not yet started.
         - Waiting for voice inactivity to complete the recording.
@@ -667,25 +719,25 @@
         # If not yet started recording, wait for voice activity to initiate.
         if not self.is_recording and not self.frames:
             self._set_state("listening")
             self.start_recording_on_voice_activity = True
 
             # Wait until recording starts
             while not self.interrupt_stop_event.is_set():
-                if self.start_recording_event.wait(timeout=0.5):
+                if self.start_recording_event.wait(timeout=0.02):
                     break
 
         # If recording is ongoing, wait for voice inactivity
         # to finish recording.
         if self.is_recording:
             self.stop_recording_on_voice_deactivity = True
 
             # Wait until recording stops
             while not self.interrupt_stop_event.is_set():
-                if (self.stop_recording_event.wait(timeout=0.5)):
+                if (self.stop_recording_event.wait(timeout=0.02)):
                     break
 
         # Convert recorded frames to the appropriate audio format.
         audio_array = np.frombuffer(b''.join(self.frames), dtype=np.int16)
         self.audio = audio_array.astype(np.float32) / INT16_MAX_ABS_VALUE
         self.frames.clear()
 
@@ -752,17 +804,22 @@
               If omitted, the transcription will be performed synchronously,
               and the result will be returned.
 
         Returns (if not callback is set):
             str: The transcription of the recorded audio
         """
 
+        self.interrupt_stop_event.clear()
+        self.was_interrupted.clear()
+
         self.wait_audio()
 
         if self.is_shut_down or self.interrupt_stop_event.is_set():
+            if self.interrupt_stop_event.is_set():
+                self.was_interrupted.set()
             return ""
 
         if on_transcription_finished:
             threading.Thread(target=on_transcription_finished,
                              args=(self.transcribe(),)).start()
         else:
             return self.transcribe()
@@ -869,15 +926,16 @@
 
         logging.debug('Finishing recording thread')
         if self.recording_thread:
             self.recording_thread.join()
 
         logging.debug('Terminating reader process')
         # Give it some time to finish the loop and cleanup.
-        self.reader_process.join(timeout=10)
+        if self.use_microphone:
+            self.reader_process.join(timeout=10)
 
         if self.reader_process.is_alive():
             logging.warning("Reader process did not terminate "
                             "in time. Terminating forcefully."
                             )
             self.reader_process.terminate()
 
@@ -892,14 +950,20 @@
 
         self.parent_transcription_pipe.close()
 
         logging.debug('Finishing realtime thread')
         if self.realtime_thread:
             self.realtime_thread.join()
 
+        if self.enable_realtime_transcription:
+            if self.realtime_model_type:
+                del self.realtime_model_type
+                self.realtime_model_type = None
+        gc.collect()
+
     def _recording_worker(self):
         """
         The main worker method which constantly monitors the audio
         input for voice activity and accordingly starts/stops the recording.
         """
 
         logging.debug('Starting recording worker')
```

### Comparing `RealTimeSTT-0.1.8/setup.py` & `RealTimeSTT-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="RealTimeSTT",
-    version="0.1.8",
+    version="0.1.9",
     author="Kolja Beigel",
     author_email="kolja.beigel@web.de",
     description="A fast Voice Activity Detection and Transcription System",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KoljaB/RealTimeSTT",
     packages=setuptools.find_packages(),
```

