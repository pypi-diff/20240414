# Comparing `tmp/batchalign-0.7.0b3.tar.gz` & `tmp/batchalign-0.7.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchalign-0.7.0b3.tar", last modified: Mon Apr  8 19:16:16 2024, max compression
+gzip compressed data, was "batchalign-0.7.1b0.tar", last modified: Sun Apr 14 05:49:26 2024, max compression
```

## Comparing `batchalign-0.7.0b3.tar` & `batchalign-0.7.1b0.tar`

### file list

```diff
@@ -1,136 +1,139 @@
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.148011 batchalign-0.7.0b3/
--rw-r--r--   0 houjun     (501) staff       (20)     1464 2024-01-21 18:39:49.000000 batchalign-0.7.0b3/LICENSE
--rw-r--r--   0 houjun     (501) staff       (20)      149 2024-04-04 00:32:13.000000 batchalign-0.7.0b3/MANIFEST.in
--rw-r--r--   0 houjun     (501) staff       (20)    12261 2024-04-08 19:16:16.147718 batchalign-0.7.0b3/PKG-INFO
--rw-r--r--   0 houjun     (501) staff       (20)     9384 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/README.md
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.129665 batchalign-0.7.0b3/batchalign/
--rw-r--r--   0 houjun     (501) staff       (20)      497 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)       63 2023-12-17 23:06:14.000000 batchalign-0.7.0b3/batchalign/__main__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.130858 batchalign-0.7.0b3/batchalign/cli/
--rw-r--r--   0 houjun     (501) staff       (20)       28 2023-12-17 01:12:36.000000 batchalign-0.7.0b3/batchalign/cli/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     9340 2024-04-05 17:12:20.000000 batchalign-0.7.0b3/batchalign/cli/cli.py
--rw-r--r--   0 houjun     (501) staff       (20)     7542 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/cli/dispatch.py
--rw-r--r--   0 houjun     (501) staff       (20)      777 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/constants.py
--rw-r--r--   0 houjun     (501) staff       (20)    14798 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/document.py
--rw-r--r--   0 houjun     (501) staff       (20)      199 2023-12-17 07:10:18.000000 batchalign-0.7.0b3/batchalign/errors.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.131182 batchalign-0.7.0b3/batchalign/formats/
--rw-r--r--   0 houjun     (501) staff       (20)       62 2024-03-18 04:57:14.000000 batchalign-0.7.0b3/batchalign/formats/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      246 2023-12-18 07:14:44.000000 batchalign-0.7.0b3/batchalign/formats/base.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.132565 batchalign-0.7.0b3/batchalign/formats/chat/
--rw-r--r--   0 houjun     (501) staff       (20)       27 2024-03-18 04:57:14.000000 batchalign-0.7.0b3/batchalign/formats/chat/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     4676 2024-04-05 17:07:15.000000 batchalign-0.7.0b3/batchalign/formats/chat/file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3701 2024-04-05 17:08:43.000000 batchalign-0.7.0b3/batchalign/formats/chat/generator.py
--rw-r--r--   0 houjun     (501) staff       (20)     7481 2023-12-28 03:10:19.000000 batchalign-0.7.0b3/batchalign/formats/chat/lexer.py
--rw-r--r--   0 houjun     (501) staff       (20)    12408 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/formats/chat/parser.py
--rw-r--r--   0 houjun     (501) staff       (20)     5217 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/formats/chat/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.133493 batchalign-0.7.0b3/batchalign/formats/textgrid/
--rw-r--r--   0 houjun     (501) staff       (20)       31 2023-12-18 07:14:59.000000 batchalign-0.7.0b3/batchalign/formats/textgrid/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3340 2024-03-18 04:57:14.000000 batchalign-0.7.0b3/batchalign/formats/textgrid/file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3485 2023-12-18 07:35:03.000000 batchalign-0.7.0b3/batchalign/formats/textgrid/generator.py
--rw-r--r--   0 houjun     (501) staff       (20)     3888 2023-12-18 05:59:42.000000 batchalign-0.7.0b3/batchalign/formats/textgrid/parser.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.134054 batchalign-0.7.0b3/batchalign/models/
--rw-r--r--   0 houjun     (501) staff       (20)      195 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      454 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/models/resolve.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.134736 batchalign-0.7.0b3/batchalign/models/speaker/
--rw-r--r--   0 houjun     (501) staff       (20)       36 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/speaker/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     5583 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/speaker/config.yaml
--rw-r--r--   0 houjun     (501) staff       (20)     3246 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/speaker/infer.py
--rw-r--r--   0 houjun     (501) staff       (20)     1808 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/speaker/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.135155 batchalign-0.7.0b3/batchalign/models/training/
--rw-r--r--   0 houjun     (501) staff       (20)       22 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/models/training/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)      576 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/training/run.py
--rw-r--r--   0 houjun     (501) staff       (20)     3357 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/models/training/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     3081 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/models/utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.136168 batchalign-0.7.0b3/batchalign/models/utterance/
--rw-r--r--   0 houjun     (501) staff       (20)       39 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/utterance/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     5447 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/utterance/dataset.py
--rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/utterance/execute.py
--rw-r--r--   0 houjun     (501) staff       (20)     3179 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/utterance/infer.py
--rw-r--r--   0 houjun     (501) staff       (20)     3057 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/utterance/prep.py
--rw-r--r--   0 houjun     (501) staff       (20)     4359 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/utterance/train.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.136536 batchalign-0.7.0b3/batchalign/models/whisper/
--rw-r--r--   0 houjun     (501) staff       (20)       76 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/whisper/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     7340 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/models/whisper/infer_asr.py
--rw-r--r--   0 houjun     (501) staff       (20)     5264 2024-04-08 19:13:44.000000 batchalign-0.7.0b3/batchalign/models/whisper/infer_fa.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.137099 batchalign-0.7.0b3/batchalign/pipelines/
--rw-r--r--   0 houjun     (501) staff       (20)      404 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/pipelines/__init__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.137421 batchalign-0.7.0b3/batchalign/pipelines/analysis/
--rw-r--r--   0 houjun     (501) staff       (20)       35 2024-02-05 03:35:25.000000 batchalign-0.7.0b3/batchalign/pipelines/analysis/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     2557 2024-02-05 03:35:25.000000 batchalign-0.7.0b3/batchalign/pipelines/analysis/eval.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.138162 batchalign-0.7.0b3/batchalign/pipelines/asr/
--rw-r--r--   0 houjun     (501) staff       (20)       99 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/pipelines/asr/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3500 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/pipelines/asr/rev.py
--rw-r--r--   0 houjun     (501) staff       (20)     7227 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/pipelines/asr/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     1866 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/pipelines/asr/whisper.py
--rw-r--r--   0 houjun     (501) staff       (20)     4205 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/pipelines/asr/whisperx.py
--rw-r--r--   0 houjun     (501) staff       (20)     1994 2024-02-05 03:35:25.000000 batchalign-0.7.0b3/batchalign/pipelines/base.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.139211 batchalign-0.7.0b3/batchalign/pipelines/cleanup/
--rw-r--r--   0 houjun     (501) staff       (20)       52 2023-12-16 19:37:43.000000 batchalign-0.7.0b3/batchalign/pipelines/cleanup/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)       93 2023-12-17 00:16:09.000000 batchalign-0.7.0b3/batchalign/pipelines/cleanup/cleanup.py
--rw-r--r--   0 houjun     (501) staff       (20)      579 2024-02-05 03:35:25.000000 batchalign-0.7.0b3/batchalign/pipelines/cleanup/disfluencies.py
--rw-r--r--   0 houjun     (501) staff       (20)     2161 2023-12-08 20:58:29.000000 batchalign-0.7.0b3/batchalign/pipelines/cleanup/parse_support.py
--rw-r--r--   0 houjun     (501) staff       (20)     2624 2024-02-05 03:35:25.000000 batchalign-0.7.0b3/batchalign/pipelines/cleanup/retrace.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.139997 batchalign-0.7.0b3/batchalign/pipelines/cleanup/support/
--rw-r--r--   0 houjun     (501) staff       (20)      141 2023-12-09 06:23:35.000000 batchalign-0.7.0b3/batchalign/pipelines/cleanup/support/filled_pauses.eng
--rw-r--r--   0 houjun     (501) staff       (20)      213 2023-12-09 06:23:34.000000 batchalign-0.7.0b3/batchalign/pipelines/cleanup/support/replacements.eng
--rw-r--r--   0 houjun     (501) staff       (20)      203 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/pipelines/cleanup/support/test.test
--rw-r--r--   0 houjun     (501) staff       (20)     3786 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/pipelines/dispatch.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.140341 batchalign-0.7.0b3/batchalign/pipelines/fa/
--rw-r--r--   0 houjun     (501) staff       (20)       40 2023-12-16 01:03:14.000000 batchalign-0.7.0b3/batchalign/pipelines/fa/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     6638 2024-04-08 19:13:33.000000 batchalign-0.7.0b3/batchalign/pipelines/fa/whisper_fa.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.140676 batchalign-0.7.0b3/batchalign/pipelines/morphosyntax/
--rw-r--r--   0 houjun     (501) staff       (20)       29 2023-12-16 23:54:03.000000 batchalign-0.7.0b3/batchalign/pipelines/morphosyntax/__init__.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.140828 batchalign-0.7.0b3/batchalign/pipelines/morphosyntax/fr/
--rw-r--r--   0 houjun     (501) staff       (20)     1147 2023-12-29 00:44:35.000000 batchalign-0.7.0b3/batchalign/pipelines/morphosyntax/fr/case.py
--rw-r--r--   0 houjun     (501) staff       (20)    28591 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/pipelines/morphosyntax/ud.py
--rw-r--r--   0 houjun     (501) staff       (20)     7482 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/pipelines/pipeline.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.141155 batchalign-0.7.0b3/batchalign/pipelines/speaker/
--rw-r--r--   0 houjun     (501) staff       (20)       44 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/pipelines/speaker/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     2367 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/batchalign/pipelines/speaker/nemo_speaker.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.141860 batchalign-0.7.0b3/batchalign/pipelines/utr/
--rw-r--r--   0 houjun     (501) staff       (20)       76 2024-01-03 22:34:21.000000 batchalign-0.7.0b3/batchalign/pipelines/utr/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3525 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/pipelines/utr/rev_utr.py
--rw-r--r--   0 houjun     (501) staff       (20)     2303 2024-01-13 18:25:54.000000 batchalign-0.7.0b3/batchalign/pipelines/utr/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)     1559 2024-02-05 03:35:25.000000 batchalign-0.7.0b3/batchalign/pipelines/utr/whisper_utr.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.142409 batchalign-0.7.0b3/batchalign/tests/
--rw-r--r--   0 houjun     (501) staff       (20)        0 2023-11-18 22:44:12.000000 batchalign-0.7.0b3/batchalign/tests/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     1497 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/tests/conftest.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.127700 batchalign-0.7.0b3/batchalign/tests/formats/
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.143471 batchalign-0.7.0b3/batchalign/tests/formats/chat/
--rw-r--r--   0 houjun     (501) staff       (20)      999 2024-03-18 04:57:14.000000 batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_file.py
--rw-r--r--   0 houjun     (501) staff       (20)     3913 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_generator.py
--rw-r--r--   0 houjun     (501) staff       (20)      714 2023-12-24 23:29:13.000000 batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_lexer.py
--rw-r--r--   0 houjun     (501) staff       (20)    10624 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_parser.py
--rw-r--r--   0 houjun     (501) staff       (20)     1046 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.143638 batchalign-0.7.0b3/batchalign/tests/formats/textgrid/
--rw-r--r--   0 houjun     (501) staff       (20)     2699 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/tests/formats/textgrid/test_textgrid.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.144242 batchalign-0.7.0b3/batchalign/tests/pipelines/
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.144396 batchalign-0.7.0b3/batchalign/tests/pipelines/analysis/
--rw-r--r--   0 houjun     (501) staff       (20)      604 2024-02-05 03:35:25.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/analysis/test_eval.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.144755 batchalign-0.7.0b3/batchalign/tests/pipelines/asr/
--rw-r--r--   0 houjun     (501) staff       (20)      938 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/asr/test_asr_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)     1570 2024-01-02 20:37:42.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/asr/test_asr_utils.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.145106 batchalign-0.7.0b3/batchalign/tests/pipelines/cleanup/
--rw-r--r--   0 houjun     (501) staff       (20)     2716 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/cleanup/test_disfluency.py
--rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/cleanup/test_parse_support.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.145269 batchalign-0.7.0b3/batchalign/tests/pipelines/fa/
--rw-r--r--   0 houjun     (501) staff       (20)      261 2024-04-08 19:15:55.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/fa/test_fa_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)      977 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/fixures.py
--rw-r--r--   0 houjun     (501) staff       (20)     4441 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/test_pipeline.py
--rw-r--r--   0 houjun     (501) staff       (20)      555 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/tests/pipelines/test_pipeline_models.py
--rw-r--r--   0 houjun     (501) staff       (20)     2472 2024-03-18 04:54:03.000000 batchalign-0.7.0b3/batchalign/tests/test_document.py
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.146116 batchalign-0.7.0b3/batchalign/utils/
--rw-r--r--   0 houjun     (501) staff       (20)       21 2023-12-16 23:44:38.000000 batchalign-0.7.0b3/batchalign/utils/__init__.py
--rw-r--r--   0 houjun     (501) staff       (20)     3513 2023-12-23 18:18:28.000000 batchalign-0.7.0b3/batchalign/utils/config.py
--rw-r--r--   0 houjun     (501) staff       (20)     7689 2024-01-18 23:05:56.000000 batchalign-0.7.0b3/batchalign/utils/dp.py
--rw-r--r--   0 houjun     (501) staff       (20)     2788 2024-04-01 06:52:40.000000 batchalign-0.7.0b3/batchalign/utils/utils.py
--rw-r--r--   0 houjun     (501) staff       (20)       61 2024-04-08 19:15:34.000000 batchalign-0.7.0b3/batchalign/version
-drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-08 19:16:16.130491 batchalign-0.7.0b3/batchalign.egg-info/
--rw-r--r--   0 houjun     (501) staff       (20)    12261 2024-04-08 19:16:16.000000 batchalign-0.7.0b3/batchalign.egg-info/PKG-INFO
--rw-r--r--   0 houjun     (501) staff       (20)     3686 2024-04-08 19:16:16.000000 batchalign-0.7.0b3/batchalign.egg-info/SOURCES.txt
--rw-r--r--   0 houjun     (501) staff       (20)        1 2024-04-08 19:16:16.000000 batchalign-0.7.0b3/batchalign.egg-info/dependency_links.txt
--rw-r--r--   0 houjun     (501) staff       (20)       61 2024-04-08 19:16:16.000000 batchalign-0.7.0b3/batchalign.egg-info/entry_points.txt
--rw-r--r--   0 houjun     (501) staff       (20)      902 2024-04-08 19:16:16.000000 batchalign-0.7.0b3/batchalign.egg-info/requires.txt
--rw-r--r--   0 houjun     (501) staff       (20)       11 2024-04-08 19:16:16.000000 batchalign-0.7.0b3/batchalign.egg-info/top_level.txt
--rw-r--r--   0 houjun     (501) staff       (20)       38 2024-04-08 19:16:16.148045 batchalign-0.7.0b3/setup.cfg
--rw-r--r--   0 houjun     (501) staff       (20)     2983 2024-04-01 06:52:43.000000 batchalign-0.7.0b3/setup.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.396181 batchalign-0.7.1b0/
+-rw-r--r--   0 houjun     (501) staff       (20)     1464 2024-01-21 18:39:49.000000 batchalign-0.7.1b0/LICENSE
+-rw-r--r--   0 houjun     (501) staff       (20)      149 2024-04-04 00:32:13.000000 batchalign-0.7.1b0/MANIFEST.in
+-rw-r--r--   0 houjun     (501) staff       (20)    12261 2024-04-14 05:49:26.395880 batchalign-0.7.1b0/PKG-INFO
+-rw-r--r--   0 houjun     (501) staff       (20)     9384 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/README.md
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.382499 batchalign-0.7.1b0/batchalign/
+-rw-r--r--   0 houjun     (501) staff       (20)      497 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)       63 2023-12-17 23:06:14.000000 batchalign-0.7.1b0/batchalign/__main__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.383799 batchalign-0.7.1b0/batchalign/cli/
+-rw-r--r--   0 houjun     (501) staff       (20)       28 2023-12-17 01:12:36.000000 batchalign-0.7.1b0/batchalign/cli/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     9340 2024-04-05 17:12:20.000000 batchalign-0.7.1b0/batchalign/cli/cli.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7542 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/cli/dispatch.py
+-rw-r--r--   0 houjun     (501) staff       (20)      777 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/constants.py
+-rw-r--r--   0 houjun     (501) staff       (20)    14798 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/document.py
+-rw-r--r--   0 houjun     (501) staff       (20)      199 2023-12-17 07:10:18.000000 batchalign-0.7.1b0/batchalign/errors.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.384038 batchalign-0.7.1b0/batchalign/formats/
+-rw-r--r--   0 houjun     (501) staff       (20)       62 2024-03-18 04:57:14.000000 batchalign-0.7.1b0/batchalign/formats/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      246 2023-12-18 07:14:44.000000 batchalign-0.7.1b0/batchalign/formats/base.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.384718 batchalign-0.7.1b0/batchalign/formats/chat/
+-rw-r--r--   0 houjun     (501) staff       (20)       27 2024-03-18 04:57:14.000000 batchalign-0.7.1b0/batchalign/formats/chat/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4676 2024-04-05 17:07:15.000000 batchalign-0.7.1b0/batchalign/formats/chat/file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3701 2024-04-05 17:08:43.000000 batchalign-0.7.1b0/batchalign/formats/chat/generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7481 2023-12-28 03:10:19.000000 batchalign-0.7.1b0/batchalign/formats/chat/lexer.py
+-rw-r--r--   0 houjun     (501) staff       (20)    12408 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/formats/chat/parser.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5217 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/formats/chat/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.385285 batchalign-0.7.1b0/batchalign/formats/textgrid/
+-rw-r--r--   0 houjun     (501) staff       (20)       31 2023-12-18 07:14:59.000000 batchalign-0.7.1b0/batchalign/formats/textgrid/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3340 2024-03-18 04:57:14.000000 batchalign-0.7.1b0/batchalign/formats/textgrid/file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3485 2023-12-18 07:35:03.000000 batchalign-0.7.1b0/batchalign/formats/textgrid/generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3888 2023-12-18 05:59:42.000000 batchalign-0.7.1b0/batchalign/formats/textgrid/parser.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.385675 batchalign-0.7.1b0/batchalign/models/
+-rw-r--r--   0 houjun     (501) staff       (20)      195 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      454 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/models/resolve.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.386201 batchalign-0.7.1b0/batchalign/models/speaker/
+-rw-r--r--   0 houjun     (501) staff       (20)       36 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/speaker/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5583 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/speaker/config.yaml
+-rw-r--r--   0 houjun     (501) staff       (20)     3246 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/speaker/infer.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1808 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/speaker/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.386558 batchalign-0.7.1b0/batchalign/models/training/
+-rw-r--r--   0 houjun     (501) staff       (20)       22 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/models/training/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)      576 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/training/run.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3357 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/models/training/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3081 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/models/utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.387224 batchalign-0.7.1b0/batchalign/models/utterance/
+-rw-r--r--   0 houjun     (501) staff       (20)       39 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/utterance/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5447 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/utterance/dataset.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/utterance/execute.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3179 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/utterance/infer.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3057 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/utterance/prep.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4359 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/utterance/train.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.387546 batchalign-0.7.1b0/batchalign/models/whisper/
+-rw-r--r--   0 houjun     (501) staff       (20)       76 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/whisper/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7340 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/models/whisper/infer_asr.py
+-rw-r--r--   0 houjun     (501) staff       (20)     5264 2024-04-08 19:13:44.000000 batchalign-0.7.1b0/batchalign/models/whisper/infer_fa.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.388032 batchalign-0.7.1b0/batchalign/pipelines/
+-rw-r--r--   0 houjun     (501) staff       (20)      449 2024-04-14 00:00:03.000000 batchalign-0.7.1b0/batchalign/pipelines/__init__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.388278 batchalign-0.7.1b0/batchalign/pipelines/analysis/
+-rw-r--r--   0 houjun     (501) staff       (20)       35 2024-02-05 03:35:25.000000 batchalign-0.7.1b0/batchalign/pipelines/analysis/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2557 2024-02-05 03:35:25.000000 batchalign-0.7.1b0/batchalign/pipelines/analysis/eval.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.388863 batchalign-0.7.1b0/batchalign/pipelines/asr/
+-rw-r--r--   0 houjun     (501) staff       (20)       99 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/pipelines/asr/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3723 2024-04-14 05:49:03.000000 batchalign-0.7.1b0/batchalign/pipelines/asr/rev.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7227 2024-04-14 04:23:55.000000 batchalign-0.7.1b0/batchalign/pipelines/asr/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2063 2024-04-14 05:49:03.000000 batchalign-0.7.1b0/batchalign/pipelines/asr/whisper.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4403 2024-04-14 05:49:03.000000 batchalign-0.7.1b0/batchalign/pipelines/asr/whisperx.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1994 2024-02-05 03:35:25.000000 batchalign-0.7.1b0/batchalign/pipelines/base.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.389501 batchalign-0.7.1b0/batchalign/pipelines/cleanup/
+-rw-r--r--   0 houjun     (501) staff       (20)       52 2023-12-16 19:37:43.000000 batchalign-0.7.1b0/batchalign/pipelines/cleanup/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)       93 2023-12-17 00:16:09.000000 batchalign-0.7.1b0/batchalign/pipelines/cleanup/cleanup.py
+-rw-r--r--   0 houjun     (501) staff       (20)      579 2024-02-05 03:35:25.000000 batchalign-0.7.1b0/batchalign/pipelines/cleanup/disfluencies.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2161 2023-12-08 20:58:29.000000 batchalign-0.7.1b0/batchalign/pipelines/cleanup/parse_support.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2624 2024-02-05 03:35:25.000000 batchalign-0.7.1b0/batchalign/pipelines/cleanup/retrace.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.389949 batchalign-0.7.1b0/batchalign/pipelines/cleanup/support/
+-rw-r--r--   0 houjun     (501) staff       (20)      141 2023-12-09 06:23:35.000000 batchalign-0.7.1b0/batchalign/pipelines/cleanup/support/filled_pauses.eng
+-rw-r--r--   0 houjun     (501) staff       (20)      213 2023-12-09 06:23:34.000000 batchalign-0.7.1b0/batchalign/pipelines/cleanup/support/replacements.eng
+-rw-r--r--   0 houjun     (501) staff       (20)      203 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/pipelines/cleanup/support/test.test
+-rw-r--r--   0 houjun     (501) staff       (20)     4111 2024-04-14 05:49:03.000000 batchalign-0.7.1b0/batchalign/pipelines/dispatch.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.390168 batchalign-0.7.1b0/batchalign/pipelines/fa/
+-rw-r--r--   0 houjun     (501) staff       (20)       40 2023-12-16 01:03:14.000000 batchalign-0.7.1b0/batchalign/pipelines/fa/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     6638 2024-04-08 21:24:31.000000 batchalign-0.7.1b0/batchalign/pipelines/fa/whisper_fa.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.390385 batchalign-0.7.1b0/batchalign/pipelines/morphosyntax/
+-rw-r--r--   0 houjun     (501) staff       (20)       29 2023-12-16 23:54:03.000000 batchalign-0.7.1b0/batchalign/pipelines/morphosyntax/__init__.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.390516 batchalign-0.7.1b0/batchalign/pipelines/morphosyntax/fr/
+-rw-r--r--   0 houjun     (501) staff       (20)     1147 2023-12-29 00:44:35.000000 batchalign-0.7.1b0/batchalign/pipelines/morphosyntax/fr/case.py
+-rw-r--r--   0 houjun     (501) staff       (20)    28591 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/pipelines/morphosyntax/ud.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7482 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/pipelines/pipeline.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.390737 batchalign-0.7.1b0/batchalign/pipelines/speaker/
+-rw-r--r--   0 houjun     (501) staff       (20)       44 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/pipelines/speaker/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2367 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/batchalign/pipelines/speaker/nemo_speaker.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.391170 batchalign-0.7.1b0/batchalign/pipelines/utr/
+-rw-r--r--   0 houjun     (501) staff       (20)       76 2024-01-03 22:34:21.000000 batchalign-0.7.1b0/batchalign/pipelines/utr/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3525 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/pipelines/utr/rev_utr.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2303 2024-04-08 21:24:31.000000 batchalign-0.7.1b0/batchalign/pipelines/utr/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1559 2024-02-05 03:35:25.000000 batchalign-0.7.1b0/batchalign/pipelines/utr/whisper_utr.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.391383 batchalign-0.7.1b0/batchalign/pipelines/utterance/
+-rw-r--r--   0 houjun     (501) staff       (20)       48 2024-04-13 19:17:01.000000 batchalign-0.7.1b0/batchalign/pipelines/utterance/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10831 2024-04-14 05:49:03.000000 batchalign-0.7.1b0/batchalign/pipelines/utterance/ud_utterance.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.391684 batchalign-0.7.1b0/batchalign/tests/
+-rw-r--r--   0 houjun     (501) staff       (20)        0 2023-11-18 22:44:12.000000 batchalign-0.7.1b0/batchalign/tests/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1497 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/tests/conftest.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.380816 batchalign-0.7.1b0/batchalign/tests/formats/
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.392231 batchalign-0.7.1b0/batchalign/tests/formats/chat/
+-rw-r--r--   0 houjun     (501) staff       (20)      999 2024-03-18 04:57:14.000000 batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_file.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3913 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_generator.py
+-rw-r--r--   0 houjun     (501) staff       (20)      714 2023-12-24 23:29:13.000000 batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_lexer.py
+-rw-r--r--   0 houjun     (501) staff       (20)    10624 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_parser.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1046 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.392340 batchalign-0.7.1b0/batchalign/tests/formats/textgrid/
+-rw-r--r--   0 houjun     (501) staff       (20)     2699 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/tests/formats/textgrid/test_textgrid.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.392665 batchalign-0.7.1b0/batchalign/tests/pipelines/
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.392774 batchalign-0.7.1b0/batchalign/tests/pipelines/analysis/
+-rw-r--r--   0 houjun     (501) staff       (20)      604 2024-02-05 03:35:25.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/analysis/test_eval.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.392991 batchalign-0.7.1b0/batchalign/tests/pipelines/asr/
+-rw-r--r--   0 houjun     (501) staff       (20)      938 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/asr/test_asr_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1570 2024-01-02 20:37:42.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/asr/test_asr_utils.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.393222 batchalign-0.7.1b0/batchalign/tests/pipelines/cleanup/
+-rw-r--r--   0 houjun     (501) staff       (20)     2716 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/cleanup/test_disfluency.py
+-rw-r--r--   0 houjun     (501) staff       (20)     1410 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/cleanup/test_parse_support.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.393330 batchalign-0.7.1b0/batchalign/tests/pipelines/fa/
+-rw-r--r--   0 houjun     (501) staff       (20)      261 2024-04-08 19:15:55.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/fa/test_fa_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)      977 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/fixures.py
+-rw-r--r--   0 houjun     (501) staff       (20)     4441 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/test_pipeline.py
+-rw-r--r--   0 houjun     (501) staff       (20)      555 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/tests/pipelines/test_pipeline_models.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2472 2024-03-18 04:54:03.000000 batchalign-0.7.1b0/batchalign/tests/test_document.py
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.393762 batchalign-0.7.1b0/batchalign/utils/
+-rw-r--r--   0 houjun     (501) staff       (20)       21 2023-12-16 23:44:38.000000 batchalign-0.7.1b0/batchalign/utils/__init__.py
+-rw-r--r--   0 houjun     (501) staff       (20)     3513 2023-12-23 18:18:28.000000 batchalign-0.7.1b0/batchalign/utils/config.py
+-rw-r--r--   0 houjun     (501) staff       (20)     7689 2024-01-18 23:05:56.000000 batchalign-0.7.1b0/batchalign/utils/dp.py
+-rw-r--r--   0 houjun     (501) staff       (20)     2788 2024-04-01 06:52:40.000000 batchalign-0.7.1b0/batchalign/utils/utils.py
+-rw-r--r--   0 houjun     (501) staff       (20)       55 2024-04-14 05:49:11.000000 batchalign-0.7.1b0/batchalign/version
+drwxr-xr-x   0 houjun     (501) staff       (20)        0 2024-04-14 05:49:26.383380 batchalign-0.7.1b0/batchalign.egg-info/
+-rw-r--r--   0 houjun     (501) staff       (20)    12261 2024-04-14 05:49:26.000000 batchalign-0.7.1b0/batchalign.egg-info/PKG-INFO
+-rw-r--r--   0 houjun     (501) staff       (20)     3776 2024-04-14 05:49:26.000000 batchalign-0.7.1b0/batchalign.egg-info/SOURCES.txt
+-rw-r--r--   0 houjun     (501) staff       (20)        1 2024-04-14 05:49:26.000000 batchalign-0.7.1b0/batchalign.egg-info/dependency_links.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       61 2024-04-14 05:49:26.000000 batchalign-0.7.1b0/batchalign.egg-info/entry_points.txt
+-rw-r--r--   0 houjun     (501) staff       (20)      902 2024-04-14 05:49:26.000000 batchalign-0.7.1b0/batchalign.egg-info/requires.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       11 2024-04-14 05:49:26.000000 batchalign-0.7.1b0/batchalign.egg-info/top_level.txt
+-rw-r--r--   0 houjun     (501) staff       (20)       38 2024-04-14 05:49:26.396217 batchalign-0.7.1b0/setup.cfg
+-rw-r--r--   0 houjun     (501) staff       (20)     2983 2024-04-01 06:52:43.000000 batchalign-0.7.1b0/setup.py
```

### Comparing `batchalign-0.7.0b3/LICENSE` & `batchalign-0.7.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/PKG-INFO` & `batchalign-0.7.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchalign
-Version: 0.7.0b3
+Version: 0.7.1b0
 Summary: Python Speech Language Sample Analysis
 Author: Brian MacWhinney, Houjun Liu
 Author-email: macw@cmu.edu, houjun@cmu.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `batchalign-0.7.0b3/README.md` & `batchalign-0.7.1b0/README.md`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/cli/cli.py` & `batchalign-0.7.1b0/batchalign/cli/cli.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/cli/dispatch.py` & `batchalign-0.7.1b0/batchalign/cli/dispatch.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/constants.py` & `batchalign-0.7.1b0/batchalign/constants.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/document.py` & `batchalign-0.7.1b0/batchalign/document.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/formats/chat/file.py` & `batchalign-0.7.1b0/batchalign/formats/chat/file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/formats/chat/generator.py` & `batchalign-0.7.1b0/batchalign/formats/chat/generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/formats/chat/lexer.py` & `batchalign-0.7.1b0/batchalign/formats/chat/lexer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/formats/chat/parser.py` & `batchalign-0.7.1b0/batchalign/formats/chat/parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/formats/chat/utils.py` & `batchalign-0.7.1b0/batchalign/formats/chat/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/formats/textgrid/file.py` & `batchalign-0.7.1b0/batchalign/formats/textgrid/file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/formats/textgrid/generator.py` & `batchalign-0.7.1b0/batchalign/formats/textgrid/generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/formats/textgrid/parser.py` & `batchalign-0.7.1b0/batchalign/formats/textgrid/parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/speaker/config.yaml` & `batchalign-0.7.1b0/batchalign/models/speaker/config.yaml`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/speaker/infer.py` & `batchalign-0.7.1b0/batchalign/models/speaker/infer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/speaker/utils.py` & `batchalign-0.7.1b0/batchalign/models/speaker/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/training/run.py` & `batchalign-0.7.1b0/batchalign/models/training/run.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/training/utils.py` & `batchalign-0.7.1b0/batchalign/models/training/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/utils.py` & `batchalign-0.7.1b0/batchalign/models/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/utterance/dataset.py` & `batchalign-0.7.1b0/batchalign/models/utterance/dataset.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/utterance/execute.py` & `batchalign-0.7.1b0/batchalign/models/utterance/execute.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/utterance/infer.py` & `batchalign-0.7.1b0/batchalign/models/utterance/infer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/utterance/prep.py` & `batchalign-0.7.1b0/batchalign/models/utterance/prep.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/utterance/train.py` & `batchalign-0.7.1b0/batchalign/models/utterance/train.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/whisper/infer_asr.py` & `batchalign-0.7.1b0/batchalign/models/whisper/infer_asr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/models/whisper/infer_fa.py` & `batchalign-0.7.1b0/batchalign/models/whisper/infer_fa.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/analysis/eval.py` & `batchalign-0.7.1b0/batchalign/pipelines/analysis/eval.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/asr/rev.py` & `batchalign-0.7.1b0/batchalign/pipelines/asr/rev.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,23 @@
 
 from rev_ai import apiclient, JobStatus
 
 import logging
 L = logging.getLogger("batchalign")
 
 class RevEngine(BatchalignEngine):
-    tasks = [ Task.ASR, Task.SPEAKER_RECOGNITION, Task.UTTERANCE_SEGMENTATION ]
+
+    @property
+    def tasks(self):
+        # if there is no utterance segmentation scheme, we only
+        # run ASR
+        if self.__engine:
+            return [ Task.ASR, Task.SPEAKER_RECOGNITION, Task.UTTERANCE_SEGMENTATION ]
+        else:
+            return [ Task.ASR, Task.SPEAKER_RECOGNITION ]
 
     def __init__(self, key:str=None, lang="eng", num_speakers=2):
 
         if key == None or key.strip() == "":
             config = config_read()
             try:
                 key = config["asr"]["engine.rev.key"]
```

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/asr/utils.py` & `batchalign-0.7.1b0/batchalign/pipelines/asr/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/asr/whisper.py` & `batchalign-0.7.1b0/batchalign/pipelines/asr/whisper.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,23 @@
 L = logging.getLogger("batchalign")
 
 from batchalign.utils.utils import correct_timing
 from batchalign.models import resolve
 
 
 class WhisperEngine(BatchalignEngine):
-    tasks = [ Task.ASR, Task.UTTERANCE_SEGMENTATION ]
+
+    @property
+    def tasks(self):
+        # if there is no utterance segmentation scheme, we only
+        # run ASR
+        if self.__engine:
+            return [ Task.ASR, Task.UTTERANCE_SEGMENTATION ]
+        else:
+            return [ Task.ASR ]
 
     def __init__(self, model=None, lang="eng"):
 
         # try to resolve our internal model
         res = resolve("whisper", lang)
         if res:
             model, base = res
```

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/asr/whisperx.py` & `batchalign-0.7.1b0/batchalign/pipelines/asr/whisperx.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,24 @@
 
 import gc 
 import torch
 
 DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
 
 class WhisperXEngine(BatchalignEngine):
-    tasks = [ Task.ASR, Task.UTTERANCE_SEGMENTATION ]
+
+    @property
+    def tasks(self):
+        # if there is no utterance segmentation scheme, we only
+        # run ASR
+        if self.__engine:
+            return [ Task.ASR, Task.UTTERANCE_SEGMENTATION ]
+        else:
+            return [ Task.ASR ]
+
 
     def __init__(self, lang="eng"):
 
         try:
             import whisperx
             print("Batchalign: If you got a warning about pyannote versioning, bad things will not happen. Please disregard.")
         except ImportError:
```

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/base.py` & `batchalign-0.7.1b0/batchalign/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/cleanup/disfluencies.py` & `batchalign-0.7.1b0/batchalign/pipelines/cleanup/disfluencies.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/cleanup/parse_support.py` & `batchalign-0.7.1b0/batchalign/pipelines/cleanup/parse_support.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/cleanup/retrace.py` & `batchalign-0.7.1b0/batchalign/pipelines/cleanup/retrace.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/dispatch.py` & `batchalign-0.7.1b0/batchalign/pipelines/dispatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 dispatch.py
 Tabulate default packages and options.
 """
 
 from batchalign import (WhisperEngine, WhisperFAEngine, StanzaEngine, RevEngine,
                         NgramRetraceEngine, DisfluencyReplacementEngine, WhisperUTREngine,
-                        RevUTREngine, EvaluationEngine, WhisperXEngine, NemoSpeakerEngine)
+                        RevUTREngine, EvaluationEngine, WhisperXEngine, NemoSpeakerEngine,
+                        StanzaUtteranceEngine)
 from batchalign import BatchalignPipeline
+from batchalign.models import resolve
 
 from batchalign.utils.config import config_read
 from batchalign.errors import *
 
 import logging
 L = logging.getLogger("batchalign")
 
@@ -20,14 +22,15 @@
     "utr": "whisper_utr",
     "fa": "whisper_fa",
     "speaker": "nemo_speaker",
     "morphosyntax": "stanza",
     "disfluency": "replacement",
     "retracing": "ngram",
     "eval": "evaluation",
+    "utterance": "stanza_utt",
 }
 
 LANGUAGE_OVERRIDE_PACKAGES = {
     "eng": {
     }
 }
 
@@ -66,14 +69,16 @@
     # if asr is in engines but disfluency or retracing is not
     # add them
     if "asr" in packages:
         if "disfluency" not in packages:
             packages.append("disfluency")
         if "retracing" not in packages:
             packages.append("retracing")
+        if "utterance" not in packages and resolve("utterance", lang) == None:
+            packages.append("utterance")
     if "fa" in packages:
         if "utr" not in packages:
             packages.append("utr")
 
     L.info(f"Initializing engines...")
     L.info(f"-------------------------------")
     for key in packages:
@@ -112,11 +117,13 @@
             engines.append(WhisperUTREngine(lang=lang))
         elif engine == "rev_utr":
             engines.append(RevUTREngine(lang=lang))
         elif engine == "evaluation":
             engines.append(EvaluationEngine())
         elif engine == "nemo_speaker":
             engines.append(NemoSpeakerEngine(num_speakers=num_speakers))
+        elif engine == "stanza_utt":
+            engines.append(StanzaUtteranceEngine())
 
     L.debug(f"Done initalizing packages.")
     return BatchalignPipeline(*engines)
```

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/fa/whisper_fa.py` & `batchalign-0.7.1b0/batchalign/pipelines/fa/whisper_fa.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/morphosyntax/fr/case.py` & `batchalign-0.7.1b0/batchalign/pipelines/morphosyntax/fr/case.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/morphosyntax/ud.py` & `batchalign-0.7.1b0/batchalign/pipelines/morphosyntax/ud.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/pipeline.py` & `batchalign-0.7.1b0/batchalign/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/speaker/nemo_speaker.py` & `batchalign-0.7.1b0/batchalign/pipelines/speaker/nemo_speaker.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/utr/rev_utr.py` & `batchalign-0.7.1b0/batchalign/pipelines/utr/rev_utr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/utr/utils.py` & `batchalign-0.7.1b0/batchalign/pipelines/utr/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/pipelines/utr/whisper_utr.py` & `batchalign-0.7.1b0/batchalign/pipelines/utr/whisper_utr.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/conftest.py` & `batchalign-0.7.1b0/batchalign/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_file.py` & `batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_file.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_generator.py` & `batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_generator.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_lexer.py` & `batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_lexer.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_parser.py` & `batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_parser.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/formats/chat/test_chat_utils.py` & `batchalign-0.7.1b0/batchalign/tests/formats/chat/test_chat_utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/formats/textgrid/test_textgrid.py` & `batchalign-0.7.1b0/batchalign/tests/formats/textgrid/test_textgrid.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/pipelines/analysis/test_eval.py` & `batchalign-0.7.1b0/batchalign/tests/pipelines/analysis/test_eval.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/pipelines/asr/test_asr_pipeline.py` & `batchalign-0.7.1b0/batchalign/tests/pipelines/asr/test_asr_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/pipelines/asr/test_asr_utils.py` & `batchalign-0.7.1b0/batchalign/tests/pipelines/asr/test_asr_utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/pipelines/cleanup/test_disfluency.py` & `batchalign-0.7.1b0/batchalign/tests/pipelines/cleanup/test_disfluency.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/pipelines/cleanup/test_parse_support.py` & `batchalign-0.7.1b0/batchalign/tests/pipelines/cleanup/test_parse_support.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/pipelines/fixures.py` & `batchalign-0.7.1b0/batchalign/tests/pipelines/fixures.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/pipelines/test_pipeline.py` & `batchalign-0.7.1b0/batchalign/tests/pipelines/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/pipelines/test_pipeline_models.py` & `batchalign-0.7.1b0/batchalign/tests/pipelines/test_pipeline_models.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/tests/test_document.py` & `batchalign-0.7.1b0/batchalign/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/utils/config.py` & `batchalign-0.7.1b0/batchalign/utils/config.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/utils/dp.py` & `batchalign-0.7.1b0/batchalign/utils/dp.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign/utils/utils.py` & `batchalign-0.7.1b0/batchalign/utils/utils.py`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/batchalign.egg-info/PKG-INFO` & `batchalign-0.7.1b0/batchalign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchalign
-Version: 0.7.0b3
+Version: 0.7.1b0
 Summary: Python Speech Language Sample Analysis
 Author: Brian MacWhinney, Houjun Liu
 Author-email: macw@cmu.edu, houjun@cmu.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `batchalign-0.7.0b3/batchalign.egg-info/SOURCES.txt` & `batchalign-0.7.1b0/batchalign.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
 batchalign/pipelines/morphosyntax/fr/case.py
 batchalign/pipelines/speaker/__init__.py
 batchalign/pipelines/speaker/nemo_speaker.py
 batchalign/pipelines/utr/__init__.py
 batchalign/pipelines/utr/rev_utr.py
 batchalign/pipelines/utr/utils.py
 batchalign/pipelines/utr/whisper_utr.py
+batchalign/pipelines/utterance/__init__.py
+batchalign/pipelines/utterance/ud_utterance.py
 batchalign/tests/__init__.py
 batchalign/tests/conftest.py
 batchalign/tests/test_document.py
 batchalign/tests/formats/chat/test_chat_file.py
 batchalign/tests/formats/chat/test_chat_generator.py
 batchalign/tests/formats/chat/test_chat_lexer.py
 batchalign/tests/formats/chat/test_chat_parser.py
```

### Comparing `batchalign-0.7.0b3/batchalign.egg-info/requires.txt` & `batchalign-0.7.1b0/batchalign.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `batchalign-0.7.0b3/setup.py` & `batchalign-0.7.1b0/setup.py`

 * *Files identical despite different names*

