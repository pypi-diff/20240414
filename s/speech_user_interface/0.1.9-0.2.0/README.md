# Comparing `tmp/speech_user_interface-0.1.9.tar.gz` & `tmp/speech_user_interface-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speech_user_interface-0.1.9.tar", max compression
+gzip compressed data, was "speech_user_interface-0.2.0.tar", max compression
```

## Comparing `speech_user_interface-0.1.9.tar` & `speech_user_interface-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0      907 2024-04-13 08:36:01.722861 speech_user_interface-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      683 2024-04-13 08:18:10.670985 speech_user_interface-0.1.9/README.md
--rw-r--r--   0        0        0     1744 2024-04-13 08:21:20.836731 speech_user_interface-0.1.9/speech_user_interface/__init__.py
--rw-r--r--   0        0        0      191 2024-04-13 05:15:04.952636 speech_user_interface-0.1.9/speech_user_interface/compare_strings.py
--rw-r--r--   0        0        0       49 2024-04-13 04:37:33.298012 speech_user_interface-0.1.9/speech_user_interface/CONSTANTS.py
--rw-r--r--   0        0        0      630 2024-04-13 05:12:32.571540 speech_user_interface-0.1.9/speech_user_interface/load_vosk_model.py
--rw-r--r--   0        0        0     1416 2024-04-13 05:50:57.320876 speech_user_interface-0.1.9/speech_user_interface/read_in_speech.py
--rw-r--r--   0        0        0      462 2024-04-13 05:25:09.140507 speech_user_interface-0.1.9/speech_user_interface/send_text_to_chatgpt.py
--rw-r--r--   0        0        0      490 2024-04-13 04:33:28.596917 speech_user_interface-0.1.9/speech_user_interface/speak_text.py
--rw-r--r--   0        0        0     1776 1970-01-01 00:00:00.000000 speech_user_interface-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      886 2024-04-14 16:53:23.680973 speech_user_interface-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      872 2024-04-13 15:24:26.034652 speech_user_interface-0.2.0/README.md
+-rw-r--r--   0        0        0     3318 2024-04-14 16:36:31.547746 speech_user_interface-0.2.0/speech_user_interface/__init__.py
+-rw-r--r--   0        0        0      641 2024-04-14 16:19:39.459199 speech_user_interface-0.2.0/speech_user_interface/build_probabilities_for_speech.py
+-rw-r--r--   0        0        0      235 2024-04-14 16:46:48.618895 speech_user_interface-0.2.0/speech_user_interface/CommandArgs.py
+-rw-r--r--   0        0        0      148 2024-04-14 14:54:57.153419 speech_user_interface-0.2.0/speech_user_interface/CommandResults.py
+-rw-r--r--   0        0        0      191 2024-04-13 05:15:04.952636 speech_user_interface-0.2.0/speech_user_interface/compare_strings.py
+-rw-r--r--   0        0        0       42 2024-04-13 14:19:42.256375 speech_user_interface-0.2.0/speech_user_interface/CONSTANTS.py
+-rw-r--r--   0        0        0     1518 2024-04-13 14:49:25.184965 speech_user_interface-0.2.0/speech_user_interface/download_file.py
+-rw-r--r--   0        0        0     1010 2024-04-13 15:12:57.207395 speech_user_interface-0.2.0/speech_user_interface/load_vosk_model.py
+-rw-r--r--   0        0        0      494 2024-04-13 15:07:46.325044 speech_user_interface-0.2.0/speech_user_interface/move_directory_up_one_level.py
+-rw-r--r--   0        0        0     2610 2024-04-14 16:42:43.348265 speech_user_interface-0.2.0/speech_user_interface/read_in_speech.py
+-rw-r--r--   0        0        0      689 2024-04-14 16:16:50.154421 speech_user_interface-0.2.0/speech_user_interface/send_text_to_chatgpt.py
+-rw-r--r--   0        0        0      490 2024-04-13 04:33:28.596917 speech_user_interface-0.2.0/speech_user_interface/speak_text.py
+-rw-r--r--   0        0        0     1946 2024-04-13 15:05:09.517652 speech_user_interface-0.2.0/speech_user_interface/unzip_file.py
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 speech_user_interface-0.2.0/PKG-INFO
```

