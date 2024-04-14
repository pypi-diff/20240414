# Comparing `tmp/ondewo-t2s-client-5.2.0.tar.gz` & `tmp/ondewo-t2s-client-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-t2s-client-5.2.0.tar", last modified: Tue Jan 23 17:45:00 2024, max compression
+gzip compressed data, was "ondewo-t2s-client-5.3.0.tar", last modified: Sun Apr 14 17:30:51 2024, max compression
```

## Comparing `ondewo-t2s-client-5.2.0.tar` & `ondewo-t2s-client-5.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 17:45:00.923643 ondewo-t2s-client-5.2.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6442 2024-01-23 17:45:00.923643 ondewo-t2s-client-5.2.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5861 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 17:45:00.923643 ondewo-t2s-client-5.2.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 17:45:00.923643 ondewo-t2s-client-5.2.0/ondewo/t2s/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 17:45:00.923643 ondewo-t2s-client-5.2.0/ondewo/t2s/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      756 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      262 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 17:45:00.923643 ondewo-t2s-client-5.2.0/ondewo/t2s/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3954 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/client/services/text_to_speech.py
--rw-rw-r--   0 root         (0) root         (0)      265 2024-01-23 17:44:14.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    30945 2024-01-23 17:44:26.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/text_to_speech_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    30251 2024-01-23 17:44:26.000000 ondewo-t2s-client-5.2.0/ondewo/t2s/text_to_speech_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-23 17:45:00.923643 ondewo-t2s-client-5.2.0/ondewo_t2s_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6442 2024-01-23 17:45:00.000000 ondewo-t2s-client-5.2.0/ondewo_t2s_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2024-01-23 17:45:00.000000 ondewo-t2s-client-5.2.0/ondewo_t2s_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-23 17:45:00.000000 ondewo-t2s-client-5.2.0/ondewo_t2s_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      204 2024-01-23 17:45:00.000000 ondewo-t2s-client-5.2.0/ondewo_t2s_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-23 17:45:00.000000 ondewo-t2s-client-5.2.0/ondewo_t2s_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2024-01-23 17:45:00.927643 ondewo-t2s-client-5.2.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1099 2024-01-23 17:44:35.000000 ondewo-t2s-client-5.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 17:30:51.136082 ondewo-t2s-client-5.3.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6442 2024-04-14 17:30:51.136082 ondewo-t2s-client-5.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5861 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 17:30:51.132083 ondewo-t2s-client-5.3.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 17:30:51.136082 ondewo-t2s-client-5.3.0/ondewo/t2s/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 17:30:51.136082 ondewo-t2s-client-5.3.0/ondewo/t2s/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      756 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      262 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 17:30:51.136082 ondewo-t2s-client-5.3.0/ondewo/t2s/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3954 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/client/services/text_to_speech.py
+-rw-rw-r--   0 root         (0) root         (0)      265 2024-04-14 17:30:05.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    33668 2024-04-14 17:30:15.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/text_to_speech_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    30251 2024-04-14 17:30:15.000000 ondewo-t2s-client-5.3.0/ondewo/t2s/text_to_speech_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 17:30:51.136082 ondewo-t2s-client-5.3.0/ondewo_t2s_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6442 2024-04-14 17:30:51.000000 ondewo-t2s-client-5.3.0/ondewo_t2s_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-14 17:30:51.000000 ondewo-t2s-client-5.3.0/ondewo_t2s_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 17:30:51.000000 ondewo-t2s-client-5.3.0/ondewo_t2s_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2024-04-14 17:30:51.000000 ondewo-t2s-client-5.3.0/ondewo_t2s_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-14 17:30:51.000000 ondewo-t2s-client-5.3.0/ondewo_t2s_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-04-14 17:30:51.136082 ondewo-t2s-client-5.3.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1099 2024-04-14 17:30:25.000000 ondewo-t2s-client-5.3.0/setup.py
```

### Comparing `ondewo-t2s-client-5.2.0/LICENSE` & `ondewo-t2s-client-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-t2s-client-5.2.0/PKG-INFO` & `ondewo-t2s-client-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-t2s-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: provides endpoints and messages for gRPC communication with the ONDEWO T2S server
 Home-page: https://github.com/ondewo/ondewo-t2s-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-t2s-client Version: 5.2.0 Summary: provides
+Metadata-Version: 2.1 Name: ondewo-t2s-client Version: 5.3.0 Summary: provides
 endpoints and messages for gRPC communication with the ONDEWO T2S server Home-
 page: https://github.com/ondewo/ondewo-t2s-client-python Author: Ondewo GbmH
 Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-t2s-client-5.2.0/README.md` & `ondewo-t2s-client-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-t2s-client-5.2.0/ondewo/t2s/client/client.py` & `ondewo-t2s-client-5.3.0/ondewo/t2s/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-t2s-client-5.2.0/ondewo/t2s/client/services/text_to_speech.py` & `ondewo-t2s-client-5.3.0/ondewo/t2s/client/services/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `ondewo-t2s-client-5.2.0/ondewo/t2s/text_to_speech_pb2.py` & `ondewo-t2s-client-5.3.0/ondewo/t2s/text_to_speech_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/t2s/text-to-speech.proto\x12\nondewo.t2s\x1a\x1bgoogle/protobuf/empty.proto\"L\n\x11SynthesizeRequest\x12\x0c\n\x04text\x18\x01 \x01(\t\x12)\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\"N\n\x16\x42\x61tchSynthesizeRequest\x12\x34\n\rbatch_request\x18\x01 \x03(\x0b\x32\x1d.ondewo.t2s.SynthesizeRequest\"Q\n\x17\x42\x61tchSynthesizeResponse\x12\x36\n\x0e\x62\x61tch_response\x18\x01 \x03(\x0b\x32\x1e.ondewo.t2s.SynthesizeResponse\"\xf3\x02\n\rRequestConfig\x12\x17\n\x0ft2s_pipeline_id\x18\x01 \x01(\t\x12\x16\n\x0clength_scale\x18\x02 \x01(\x02H\x00\x12\x15\n\x0bnoise_scale\x18\x03 \x01(\x02H\x01\x12\x15\n\x0bsample_rate\x18\x04 \x01(\x05H\x02\x12\x1e\n\x03pcm\x18\x05 \x01(\x0e\x32\x0f.ondewo.t2s.PcmH\x03\x12/\n\x0c\x61udio_format\x18\x06 \x01(\x0e\x32\x17.ondewo.t2s.AudioFormatH\x04\x12\x13\n\tuse_cache\x18\x07 \x01(\x08H\x05\x12\x14\n\nnormalizer\x18\x08 \x01(\tH\x06\x42\x14\n\x12oneof_length_scaleB\x13\n\x11oneof_noise_scaleB\x13\n\x11oneof_sample_rateB\x0b\n\toneof_PcmB\x13\n\x11oneof_AudioFormatB\x11\n\x0foneof_use_cacheB\x12\n\x10oneof_normalizer\"\xb8\x01\n\x12SynthesizeResponse\x12\x12\n\naudio_uuid\x18\x01 \x01(\t\x12\r\n\x05\x61udio\x18\x02 \x01(\x0c\x12\x17\n\x0fgeneration_time\x18\x03 \x01(\x02\x12\x14\n\x0c\x61udio_length\x18\x04 \x01(\x02\x12\x0c\n\x04text\x18\x05 \x01(\t\x12)\n\x06\x63onfig\x18\x06 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\x12\x17\n\x0fnormalized_text\x18\x07 \x01(\t\"=\n\x14NormalizeTextRequest\x12\x17\n\x0ft2s_pipeline_id\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"0\n\x15NormalizeTextResponse\x12\x17\n\x0fnormalized_text\x18\x01 \x01(\t\",\n\x19T2SGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\x84\x01\n\x17ListT2sPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x15\n\rspeaker_sexes\x18\x02 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x03 \x03(\t\x12\x15\n\rspeaker_names\x18\x04 \x03(\t\x12\x0f\n\x07\x64omains\x18\x05 \x03(\t\"L\n\x18ListT2sPipelinesResponse\x12\x30\n\tpipelines\x18\x01 \x03(\x0b\x32\x1d.ondewo.t2s.Text2SpeechConfig\"q\n\x17ListT2sLanguagesRequest\x12\x15\n\rspeaker_sexes\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x15\n\rspeaker_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64omains\x18\x04 \x03(\t\"-\n\x18ListT2sLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"q\n\x15ListT2sDomainsRequest\x12\x15\n\rspeaker_sexes\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x15\n\rspeaker_names\x18\x03 \x03(\t\x12\x11\n\tlanguages\x18\x04 \x03(\t\")\n\x16ListT2sDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\"\x1b\n\rT2sPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"\xf6\x01\n\x11Text2SpeechConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.t2s.T2SDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.t2s.T2SInference\x12\x33\n\rnormalization\x18\x05 \x01(\x0b\x32\x1c.ondewo.t2s.T2SNormalization\x12\x32\n\x0epostprocessing\x18\x06 \x01(\x0b\x32\x1a.ondewo.t2s.Postprocessing\"\x87\x01\n\x0eT2SDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x13\n\x0bspeaker_sex\x18\x02 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x05 \x01(\t\x12\x0e\n\x06\x64omain\x18\x06 \x01(\t\"\x7f\n\x0cT2SInference\x12\x0c\n\x04type\x18\x01 \x01(\t\x12;\n\x13\x63omposite_inference\x18\x02 \x01(\x0b\x32\x1e.ondewo.t2s.CompositeInference\x12$\n\x07\x63\x61\x63hing\x18\x03 \x01(\x0b\x32\x13.ondewo.t2s.Caching\"f\n\x12\x43ompositeInference\x12&\n\x08text2mel\x18\x01 \x01(\x0b\x32\x14.ondewo.t2s.Text2Mel\x12(\n\tmel2audio\x18\x02 \x01(\x0b\x32\x15.ondewo.t2s.Mel2Audio\"s\n\x08Text2Mel\x12\x0c\n\x04type\x18\x01 \x01(\t\x12%\n\x08glow_tts\x18\x02 \x01(\x0b\x32\x13.ondewo.t2s.GlowTTS\x12\x32\n\x0fglow_tts_triton\x18\x03 \x01(\x0b\x32\x19.ondewo.t2s.GlowTTSTriton\"\x94\x01\n\x07GlowTTS\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x14\n\x0clength_scale\x18\x03 \x01(\x02\x12\x13\n\x0bnoise_scale\x18\x04 \x01(\x02\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x10\n\x08\x63leaners\x18\x06 \x03(\t\x12\x19\n\x11param_config_path\x18\x07 \x01(\t\"\xe7\x01\n\rGlowTTSTriton\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\x14\n\x0clength_scale\x18\x02 \x01(\x02\x12\x13\n\x0bnoise_scale\x18\x03 \x01(\x02\x12\x10\n\x08\x63leaners\x18\x04 \x03(\t\x12\x17\n\x0fmax_text_length\x18\x05 \x01(\x03\x12\x19\n\x11param_config_path\x18\x06 \x01(\t\x12\x19\n\x11triton_model_name\x18\x07 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x08 \x01(\t\x12\x1a\n\x12triton_server_port\x18\t \x01(\x03\"\xaa\x01\n\tMel2Audio\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x34\n\x10mb_melgan_triton\x18\x02 \x01(\x0b\x32\x1a.ondewo.t2s.MbMelganTriton\x12%\n\x08hifi_gan\x18\x03 \x01(\x0b\x32\x13.ondewo.t2s.HiFiGan\x12\x32\n\x0fhifi_gan_triton\x18\x04 \x01(\x0b\x32\x19.ondewo.t2s.HiFiGanTriton\"W\n\x07HiFiGan\x12\x0f\n\x07use_gpu\x18\x01 \x01(\x08\x12\x12\n\nbatch_size\x18\x02 \x01(\x03\x12\x13\n\x0b\x63onfig_path\x18\x03 \x01(\t\x12\x12\n\nmodel_path\x18\x04 \x01(\t\"w\n\rHiFiGanTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x03 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x04 \x01(\x03\"\x8c\x01\n\x0eMbMelganTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x12\n\nstats_path\x18\x02 \x01(\t\x12\x19\n\x11triton_model_name\x18\x03 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x04 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x05 \x01(\x03\"\x8f\x01\n\x07\x43\x61\x63hing\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\x1d\n\x15memory_cache_max_size\x18\x02 \x01(\x03\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x12\n\nload_cache\x18\x04 \x01(\x08\x12\x12\n\nsave_cache\x18\x05 \x01(\x08\x12\x16\n\x0e\x63\x61\x63he_save_dir\x18\x06 \x01(\t\"\xe2\x01\n\x10T2SNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x10\n\x08pipeline\x18\x02 \x03(\t\x12\x1c\n\x14\x63ustom_phonemizer_id\x18\x03 \x01(\t\x12?\n\x14\x63ustom_length_scales\x18\x04 \x01(\x0b\x32!.ondewo.t2s.T2SCustomLengthScales\x12\x17\n\x0f\x61rpabet_mapping\x18\x05 \x01(\t\x12\x17\n\x0fnumeric_mapping\x18\x06 \x01(\t\x12\x19\n\x11\x63\x61llsigns_mapping\x18\x07 \x01(\t\"\xb0\x01\n\x0ePostprocessing\x12\x14\n\x0csilence_secs\x18\x01 \x01(\x02\x12\x10\n\x08pipeline\x18\x02 \x03(\t\x12$\n\x07logmmse\x18\x03 \x01(\x0b\x32\x13.ondewo.t2s.Logmnse\x12\"\n\x06wiener\x18\x04 \x01(\x0b\x32\x12.ondewo.t2s.Wiener\x12,\n\x0b\x61podization\x18\x05 \x01(\x0b\x32\x17.ondewo.t2s.Apodization\"N\n\x07Logmnse\x12\x15\n\rinitial_noise\x18\x01 \x01(\x03\x12\x13\n\x0bwindow_size\x18\x02 \x01(\x03\x12\x17\n\x0fnoise_threshold\x18\x03 \x01(\x02\"a\n\x06Wiener\x12\x11\n\tframe_len\x18\x01 \x01(\x03\x12\x11\n\tlpc_order\x18\x02 \x01(\x03\x12\x12\n\niterations\x18\x03 \x01(\x03\x12\r\n\x05\x61lpha\x18\x04 \x01(\x02\x12\x0e\n\x06thresh\x18\x05 \x01(\x02\"\'\n\x0b\x41podization\x12\x18\n\x10\x61podization_secs\x18\x01 \x01(\x02\"\xa8\x01\n\x15T2SCustomLengthScales\x12\x0c\n\x04text\x18\x01 \x01(\x02\x12\r\n\x05\x65mail\x18\x02 \x01(\x02\x12\x0b\n\x03url\x18\x03 \x01(\x02\x12\r\n\x05phone\x18\x04 \x01(\x02\x12\r\n\x05spell\x18\x05 \x01(\x02\x12\x18\n\x10spell_with_names\x18\x06 \x01(\x02\x12\x15\n\rcallsign_long\x18\x07 \x01(\x02\x12\x16\n\x0e\x63\x61llsign_short\x18\x08 \x01(\x02\"\x1a\n\x0cPhonemizerId\x12\n\n\x02id\x18\x01 \x01(\t\"B\n\x15\x43ustomPhonemizerProto\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1d\n\x04maps\x18\x02 \x03(\x0b\x32\x0f.ondewo.t2s.Map\"+\n\x03Map\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\x16\n\x0ephoneme_groups\x18\x02 \x01(\t\"V\n\x1cListCustomPhonemizerResponse\x12\x36\n\x0bphonemizers\x18\x01 \x03(\x0b\x32!.ondewo.t2s.CustomPhonemizerProto\"3\n\x1bListCustomPhonemizerRequest\x12\x14\n\x0cpipeline_ids\x18\x01 \x03(\t\"\xd8\x01\n\x1dUpdateCustomPhonemizerRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12M\n\rupdate_method\x18\x02 \x01(\x0e\x32\x36.ondewo.t2s.UpdateCustomPhonemizerRequest.UpdateMethod\x12\x1d\n\x04maps\x18\x03 \x03(\x0b\x32\x0f.ondewo.t2s.Map\"=\n\x0cUpdateMethod\x12\x0f\n\x0b\x65xtend_hard\x10\x00\x12\x0f\n\x0b\x65xtend_soft\x10\x01\x12\x0b\n\x07replace\x10\x02\"N\n\x1d\x43reateCustomPhonemizerRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x1d\n\x04maps\x18\x02 \x03(\x0b\x32\x0f.ondewo.t2s.Map*X\n\x03Pcm\x12\n\n\x06PCM_16\x10\x00\x12\n\n\x06PCM_24\x10\x01\x12\n\n\x06PCM_32\x10\x02\x12\n\n\x06PCM_S8\x10\x03\x12\n\n\x06PCM_U8\x10\x04\x12\t\n\x05\x46LOAT\x10\x05\x12\n\n\x06\x44OUBLE\x10\x06*M\n\x0b\x41udioFormat\x12\x07\n\x03wav\x10\x00\x12\x08\n\x04\x66lac\x10\x01\x12\x07\n\x03\x63\x61\x66\x10\x02\x12\x07\n\x03mp3\x10\x03\x12\x07\n\x03\x61\x61\x63\x10\x04\x12\x07\n\x03ogg\x10\x05\x12\x07\n\x03wma\x10\x06\x32\xf5\n\n\x0bText2Speech\x12K\n\nSynthesize\x12\x1d.ondewo.t2s.SynthesizeRequest\x1a\x1e.ondewo.t2s.SynthesizeResponse\x12Z\n\x0f\x42\x61tchSynthesize\x12\".ondewo.t2s.BatchSynthesizeRequest\x1a#.ondewo.t2s.BatchSynthesizeResponse\x12T\n\rNormalizeText\x12 .ondewo.t2s.NormalizeTextRequest\x1a!.ondewo.t2s.NormalizeTextResponse\x12J\n\x0eGetT2sPipeline\x12\x19.ondewo.t2s.T2sPipelineId\x1a\x1d.ondewo.t2s.Text2SpeechConfig\x12M\n\x11\x43reateT2sPipeline\x12\x1d.ondewo.t2s.Text2SpeechConfig\x1a\x19.ondewo.t2s.T2sPipelineId\x12\x46\n\x11\x44\x65leteT2sPipeline\x12\x19.ondewo.t2s.T2sPipelineId\x1a\x16.google.protobuf.Empty\x12J\n\x11UpdateT2sPipeline\x12\x1d.ondewo.t2s.Text2SpeechConfig\x1a\x16.google.protobuf.Empty\x12]\n\x10ListT2sPipelines\x12#.ondewo.t2s.ListT2sPipelinesRequest\x1a$.ondewo.t2s.ListT2sPipelinesResponse\x12]\n\x10ListT2sLanguages\x12#.ondewo.t2s.ListT2sLanguagesRequest\x1a$.ondewo.t2s.ListT2sLanguagesResponse\x12W\n\x0eListT2sDomains\x12!.ondewo.t2s.ListT2sDomainsRequest\x1a\".ondewo.t2s.ListT2sDomainsResponse\x12O\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.t2s.T2SGetServiceInfoResponse\x12R\n\x13GetCustomPhonemizer\x12\x18.ondewo.t2s.PhonemizerId\x1a!.ondewo.t2s.CustomPhonemizerProto\x12]\n\x16\x43reateCustomPhonemizer\x12).ondewo.t2s.CreateCustomPhonemizerRequest\x1a\x18.ondewo.t2s.PhonemizerId\x12J\n\x16\x44\x65leteCustomPhonemizer\x12\x18.ondewo.t2s.PhonemizerId\x1a\x16.google.protobuf.Empty\x12\x66\n\x16UpdateCustomPhonemizer\x12).ondewo.t2s.UpdateCustomPhonemizerRequest\x1a!.ondewo.t2s.CustomPhonemizerProto\x12i\n\x14ListCustomPhonemizer\x12\'.ondewo.t2s.ListCustomPhonemizerRequest\x1a(.ondewo.t2s.ListCustomPhonemizerResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fondewo/t2s/text-to-speech.proto\x12\nondewo.t2s\x1a\x1bgoogle/protobuf/empty.proto\"L\n\x11SynthesizeRequest\x12\x0c\n\x04text\x18\x01 \x01(\t\x12)\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\"N\n\x16\x42\x61tchSynthesizeRequest\x12\x34\n\rbatch_request\x18\x01 \x03(\x0b\x32\x1d.ondewo.t2s.SynthesizeRequest\"Q\n\x17\x42\x61tchSynthesizeResponse\x12\x36\n\x0e\x62\x61tch_response\x18\x01 \x03(\x0b\x32\x1e.ondewo.t2s.SynthesizeResponse\"\xf3\x02\n\rRequestConfig\x12\x17\n\x0ft2s_pipeline_id\x18\x01 \x01(\t\x12\x16\n\x0clength_scale\x18\x02 \x01(\x02H\x00\x12\x15\n\x0bnoise_scale\x18\x03 \x01(\x02H\x01\x12\x15\n\x0bsample_rate\x18\x04 \x01(\x05H\x02\x12\x1e\n\x03pcm\x18\x05 \x01(\x0e\x32\x0f.ondewo.t2s.PcmH\x03\x12/\n\x0c\x61udio_format\x18\x06 \x01(\x0e\x32\x17.ondewo.t2s.AudioFormatH\x04\x12\x13\n\tuse_cache\x18\x07 \x01(\x08H\x05\x12\x14\n\nnormalizer\x18\x08 \x01(\tH\x06\x42\x14\n\x12oneof_length_scaleB\x13\n\x11oneof_noise_scaleB\x13\n\x11oneof_sample_rateB\x0b\n\toneof_PcmB\x13\n\x11oneof_AudioFormatB\x11\n\x0foneof_use_cacheB\x12\n\x10oneof_normalizer\"\xb8\x01\n\x12SynthesizeResponse\x12\x12\n\naudio_uuid\x18\x01 \x01(\t\x12\r\n\x05\x61udio\x18\x02 \x01(\x0c\x12\x17\n\x0fgeneration_time\x18\x03 \x01(\x02\x12\x14\n\x0c\x61udio_length\x18\x04 \x01(\x02\x12\x0c\n\x04text\x18\x05 \x01(\t\x12)\n\x06\x63onfig\x18\x06 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\x12\x17\n\x0fnormalized_text\x18\x07 \x01(\t\"=\n\x14NormalizeTextRequest\x12\x17\n\x0ft2s_pipeline_id\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"0\n\x15NormalizeTextResponse\x12\x17\n\x0fnormalized_text\x18\x01 \x01(\t\",\n\x19T2SGetServiceInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\x84\x01\n\x17ListT2sPipelinesRequest\x12\x11\n\tlanguages\x18\x01 \x03(\t\x12\x15\n\rspeaker_sexes\x18\x02 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x03 \x03(\t\x12\x15\n\rspeaker_names\x18\x04 \x03(\t\x12\x0f\n\x07\x64omains\x18\x05 \x03(\t\"L\n\x18ListT2sPipelinesResponse\x12\x30\n\tpipelines\x18\x01 \x03(\x0b\x32\x1d.ondewo.t2s.Text2SpeechConfig\"q\n\x17ListT2sLanguagesRequest\x12\x15\n\rspeaker_sexes\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x15\n\rspeaker_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64omains\x18\x04 \x03(\t\"-\n\x18ListT2sLanguagesResponse\x12\x11\n\tlanguages\x18\x01 \x03(\t\"q\n\x15ListT2sDomainsRequest\x12\x15\n\rspeaker_sexes\x18\x01 \x03(\t\x12\x17\n\x0fpipeline_owners\x18\x02 \x03(\t\x12\x15\n\rspeaker_names\x18\x03 \x03(\t\x12\x11\n\tlanguages\x18\x04 \x03(\t\")\n\x16ListT2sDomainsResponse\x12\x0f\n\x07\x64omains\x18\x01 \x03(\t\"\x1b\n\rT2sPipelineId\x12\n\n\x02id\x18\x01 \x01(\t\"\xf6\x01\n\x11Text2SpeechConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12/\n\x0b\x64\x65scription\x18\x02 \x01(\x0b\x32\x1a.ondewo.t2s.T2SDescription\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\x12+\n\tinference\x18\x04 \x01(\x0b\x32\x18.ondewo.t2s.T2SInference\x12\x33\n\rnormalization\x18\x05 \x01(\x0b\x32\x1c.ondewo.t2s.T2SNormalization\x12\x32\n\x0epostprocessing\x18\x06 \x01(\x0b\x32\x1a.ondewo.t2s.Postprocessing\"\x87\x01\n\x0eT2SDescription\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x13\n\x0bspeaker_sex\x18\x02 \x01(\t\x12\x16\n\x0epipeline_owner\x18\x03 \x01(\t\x12\x10\n\x08\x63omments\x18\x04 \x01(\t\x12\x14\n\x0cspeaker_name\x18\x05 \x01(\t\x12\x0e\n\x06\x64omain\x18\x06 \x01(\t\"\xb6\x01\n\x0cT2SInference\x12\x0c\n\x04type\x18\x01 \x01(\t\x12;\n\x13\x63omposite_inference\x18\x02 \x01(\x0b\x32\x1e.ondewo.t2s.CompositeInference\x12\x35\n\x10single_inference\x18\x03 \x01(\x0b\x32\x1b.ondewo.t2s.SingleInference\x12$\n\x07\x63\x61\x63hing\x18\x04 \x01(\x0b\x32\x13.ondewo.t2s.Caching\"f\n\x12\x43ompositeInference\x12&\n\x08text2mel\x18\x01 \x01(\x0b\x32\x14.ondewo.t2s.Text2Mel\x12(\n\tmel2audio\x18\x02 \x01(\x0b\x32\x15.ondewo.t2s.Mel2Audio\"=\n\x0fSingleInference\x12*\n\ntext2audio\x18\x01 \x01(\x0b\x32\x16.ondewo.t2s.Text2Audio\"s\n\x08Text2Mel\x12\x0c\n\x04type\x18\x01 \x01(\t\x12%\n\x08glow_tts\x18\x02 \x01(\x0b\x32\x13.ondewo.t2s.GlowTTS\x12\x32\n\x0fglow_tts_triton\x18\x03 \x01(\x0b\x32\x19.ondewo.t2s.GlowTTSTriton\"g\n\nText2Audio\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x1e\n\x04vits\x18\x02 \x01(\x0b\x32\x10.ondewo.t2s.Vits\x12+\n\x0bvits_triton\x18\x03 \x01(\x0b\x32\x16.ondewo.t2s.VitsTriton\"\x94\x01\n\x07GlowTTS\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x14\n\x0clength_scale\x18\x03 \x01(\x02\x12\x13\n\x0bnoise_scale\x18\x04 \x01(\x02\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x10\n\x08\x63leaners\x18\x06 \x03(\t\x12\x19\n\x11param_config_path\x18\x07 \x01(\t\"\xe7\x01\n\rGlowTTSTriton\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\x14\n\x0clength_scale\x18\x02 \x01(\x02\x12\x13\n\x0bnoise_scale\x18\x03 \x01(\x02\x12\x10\n\x08\x63leaners\x18\x04 \x03(\t\x12\x17\n\x0fmax_text_length\x18\x05 \x01(\x03\x12\x19\n\x11param_config_path\x18\x06 \x01(\t\x12\x19\n\x11triton_model_name\x18\x07 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x08 \x01(\t\x12\x1a\n\x12triton_server_port\x18\t \x01(\x03\"\x91\x01\n\x04Vits\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\x0f\n\x07use_gpu\x18\x02 \x01(\x08\x12\x14\n\x0clength_scale\x18\x03 \x01(\x02\x12\x13\n\x0bnoise_scale\x18\x04 \x01(\x02\x12\x0c\n\x04path\x18\x05 \x01(\t\x12\x10\n\x08\x63leaners\x18\x06 \x03(\t\x12\x19\n\x11param_config_path\x18\x07 \x01(\t\"\xe4\x01\n\nVitsTriton\x12\x12\n\nbatch_size\x18\x01 \x01(\x03\x12\x14\n\x0clength_scale\x18\x02 \x01(\x02\x12\x13\n\x0bnoise_scale\x18\x03 \x01(\x02\x12\x10\n\x08\x63leaners\x18\x04 \x03(\t\x12\x17\n\x0fmax_text_length\x18\x05 \x01(\x03\x12\x19\n\x11param_config_path\x18\x06 \x01(\t\x12\x19\n\x11triton_model_name\x18\x07 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x08 \x01(\t\x12\x1a\n\x12triton_server_port\x18\t \x01(\x03\"\xaa\x01\n\tMel2Audio\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x34\n\x10mb_melgan_triton\x18\x02 \x01(\x0b\x32\x1a.ondewo.t2s.MbMelganTriton\x12%\n\x08hifi_gan\x18\x03 \x01(\x0b\x32\x13.ondewo.t2s.HiFiGan\x12\x32\n\x0fhifi_gan_triton\x18\x04 \x01(\x0b\x32\x19.ondewo.t2s.HiFiGanTriton\"W\n\x07HiFiGan\x12\x0f\n\x07use_gpu\x18\x01 \x01(\x08\x12\x12\n\nbatch_size\x18\x02 \x01(\x03\x12\x13\n\x0b\x63onfig_path\x18\x03 \x01(\t\x12\x12\n\nmodel_path\x18\x04 \x01(\t\"w\n\rHiFiGanTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x19\n\x11triton_model_name\x18\x02 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x03 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x04 \x01(\x03\"\x8c\x01\n\x0eMbMelganTriton\x12\x13\n\x0b\x63onfig_path\x18\x01 \x01(\t\x12\x12\n\nstats_path\x18\x02 \x01(\t\x12\x19\n\x11triton_model_name\x18\x03 \x01(\t\x12\x1a\n\x12triton_server_host\x18\x04 \x01(\t\x12\x1a\n\x12triton_server_port\x18\x05 \x01(\x03\"\x8f\x01\n\x07\x43\x61\x63hing\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\x1d\n\x15memory_cache_max_size\x18\x02 \x01(\x03\x12\x15\n\rsampling_rate\x18\x03 \x01(\x03\x12\x12\n\nload_cache\x18\x04 \x01(\x08\x12\x12\n\nsave_cache\x18\x05 \x01(\x08\x12\x16\n\x0e\x63\x61\x63he_save_dir\x18\x06 \x01(\t\"\xe2\x01\n\x10T2SNormalization\x12\x10\n\x08language\x18\x01 \x01(\t\x12\x10\n\x08pipeline\x18\x02 \x03(\t\x12\x1c\n\x14\x63ustom_phonemizer_id\x18\x03 \x01(\t\x12?\n\x14\x63ustom_length_scales\x18\x04 \x01(\x0b\x32!.ondewo.t2s.T2SCustomLengthScales\x12\x17\n\x0f\x61rpabet_mapping\x18\x05 \x01(\t\x12\x17\n\x0fnumeric_mapping\x18\x06 \x01(\t\x12\x19\n\x11\x63\x61llsigns_mapping\x18\x07 \x01(\t\"\xb0\x01\n\x0ePostprocessing\x12\x14\n\x0csilence_secs\x18\x01 \x01(\x02\x12\x10\n\x08pipeline\x18\x02 \x03(\t\x12$\n\x07logmmse\x18\x03 \x01(\x0b\x32\x13.ondewo.t2s.Logmnse\x12\"\n\x06wiener\x18\x04 \x01(\x0b\x32\x12.ondewo.t2s.Wiener\x12,\n\x0b\x61podization\x18\x05 \x01(\x0b\x32\x17.ondewo.t2s.Apodization\"N\n\x07Logmnse\x12\x15\n\rinitial_noise\x18\x01 \x01(\x03\x12\x13\n\x0bwindow_size\x18\x02 \x01(\x03\x12\x17\n\x0fnoise_threshold\x18\x03 \x01(\x02\"a\n\x06Wiener\x12\x11\n\tframe_len\x18\x01 \x01(\x03\x12\x11\n\tlpc_order\x18\x02 \x01(\x03\x12\x12\n\niterations\x18\x03 \x01(\x03\x12\r\n\x05\x61lpha\x18\x04 \x01(\x02\x12\x0e\n\x06thresh\x18\x05 \x01(\x02\"\'\n\x0b\x41podization\x12\x18\n\x10\x61podization_secs\x18\x01 \x01(\x02\"\xa8\x01\n\x15T2SCustomLengthScales\x12\x0c\n\x04text\x18\x01 \x01(\x02\x12\r\n\x05\x65mail\x18\x02 \x01(\x02\x12\x0b\n\x03url\x18\x03 \x01(\x02\x12\r\n\x05phone\x18\x04 \x01(\x02\x12\r\n\x05spell\x18\x05 \x01(\x02\x12\x18\n\x10spell_with_names\x18\x06 \x01(\x02\x12\x15\n\rcallsign_long\x18\x07 \x01(\x02\x12\x16\n\x0e\x63\x61llsign_short\x18\x08 \x01(\x02\"\x1a\n\x0cPhonemizerId\x12\n\n\x02id\x18\x01 \x01(\t\"B\n\x15\x43ustomPhonemizerProto\x12\n\n\x02id\x18\x01 \x01(\t\x12\x1d\n\x04maps\x18\x02 \x03(\x0b\x32\x0f.ondewo.t2s.Map\"+\n\x03Map\x12\x0c\n\x04word\x18\x01 \x01(\t\x12\x16\n\x0ephoneme_groups\x18\x02 \x01(\t\"V\n\x1cListCustomPhonemizerResponse\x12\x36\n\x0bphonemizers\x18\x01 \x03(\x0b\x32!.ondewo.t2s.CustomPhonemizerProto\"3\n\x1bListCustomPhonemizerRequest\x12\x14\n\x0cpipeline_ids\x18\x01 \x03(\t\"\xd8\x01\n\x1dUpdateCustomPhonemizerRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12M\n\rupdate_method\x18\x02 \x01(\x0e\x32\x36.ondewo.t2s.UpdateCustomPhonemizerRequest.UpdateMethod\x12\x1d\n\x04maps\x18\x03 \x03(\x0b\x32\x0f.ondewo.t2s.Map\"=\n\x0cUpdateMethod\x12\x0f\n\x0b\x65xtend_hard\x10\x00\x12\x0f\n\x0b\x65xtend_soft\x10\x01\x12\x0b\n\x07replace\x10\x02\"N\n\x1d\x43reateCustomPhonemizerRequest\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x1d\n\x04maps\x18\x02 \x03(\x0b\x32\x0f.ondewo.t2s.Map*X\n\x03Pcm\x12\n\n\x06PCM_16\x10\x00\x12\n\n\x06PCM_24\x10\x01\x12\n\n\x06PCM_32\x10\x02\x12\n\n\x06PCM_S8\x10\x03\x12\n\n\x06PCM_U8\x10\x04\x12\t\n\x05\x46LOAT\x10\x05\x12\n\n\x06\x44OUBLE\x10\x06*M\n\x0b\x41udioFormat\x12\x07\n\x03wav\x10\x00\x12\x08\n\x04\x66lac\x10\x01\x12\x07\n\x03\x63\x61\x66\x10\x02\x12\x07\n\x03mp3\x10\x03\x12\x07\n\x03\x61\x61\x63\x10\x04\x12\x07\n\x03ogg\x10\x05\x12\x07\n\x03wma\x10\x06\x32\xf5\n\n\x0bText2Speech\x12K\n\nSynthesize\x12\x1d.ondewo.t2s.SynthesizeRequest\x1a\x1e.ondewo.t2s.SynthesizeResponse\x12Z\n\x0f\x42\x61tchSynthesize\x12\".ondewo.t2s.BatchSynthesizeRequest\x1a#.ondewo.t2s.BatchSynthesizeResponse\x12T\n\rNormalizeText\x12 .ondewo.t2s.NormalizeTextRequest\x1a!.ondewo.t2s.NormalizeTextResponse\x12J\n\x0eGetT2sPipeline\x12\x19.ondewo.t2s.T2sPipelineId\x1a\x1d.ondewo.t2s.Text2SpeechConfig\x12M\n\x11\x43reateT2sPipeline\x12\x1d.ondewo.t2s.Text2SpeechConfig\x1a\x19.ondewo.t2s.T2sPipelineId\x12\x46\n\x11\x44\x65leteT2sPipeline\x12\x19.ondewo.t2s.T2sPipelineId\x1a\x16.google.protobuf.Empty\x12J\n\x11UpdateT2sPipeline\x12\x1d.ondewo.t2s.Text2SpeechConfig\x1a\x16.google.protobuf.Empty\x12]\n\x10ListT2sPipelines\x12#.ondewo.t2s.ListT2sPipelinesRequest\x1a$.ondewo.t2s.ListT2sPipelinesResponse\x12]\n\x10ListT2sLanguages\x12#.ondewo.t2s.ListT2sLanguagesRequest\x1a$.ondewo.t2s.ListT2sLanguagesResponse\x12W\n\x0eListT2sDomains\x12!.ondewo.t2s.ListT2sDomainsRequest\x1a\".ondewo.t2s.ListT2sDomainsResponse\x12O\n\x0eGetServiceInfo\x12\x16.google.protobuf.Empty\x1a%.ondewo.t2s.T2SGetServiceInfoResponse\x12R\n\x13GetCustomPhonemizer\x12\x18.ondewo.t2s.PhonemizerId\x1a!.ondewo.t2s.CustomPhonemizerProto\x12]\n\x16\x43reateCustomPhonemizer\x12).ondewo.t2s.CreateCustomPhonemizerRequest\x1a\x18.ondewo.t2s.PhonemizerId\x12J\n\x16\x44\x65leteCustomPhonemizer\x12\x18.ondewo.t2s.PhonemizerId\x1a\x16.google.protobuf.Empty\x12\x66\n\x16UpdateCustomPhonemizer\x12).ondewo.t2s.UpdateCustomPhonemizerRequest\x1a!.ondewo.t2s.CustomPhonemizerProto\x12i\n\x14ListCustomPhonemizer\x12\'.ondewo.t2s.ListCustomPhonemizerRequest\x1a(.ondewo.t2s.ListCustomPhonemizerResponseb\x06proto3')
 
 _PCM = DESCRIPTOR.enum_types_by_name['Pcm']
 Pcm = enum_type_wrapper.EnumTypeWrapper(_PCM)
 _AUDIOFORMAT = DESCRIPTOR.enum_types_by_name['AudioFormat']
 AudioFormat = enum_type_wrapper.EnumTypeWrapper(_AUDIOFORMAT)
 PCM_16 = 0
 PCM_24 = 1
@@ -53,17 +53,21 @@
 _LISTT2SDOMAINSREQUEST = DESCRIPTOR.message_types_by_name['ListT2sDomainsRequest']
 _LISTT2SDOMAINSRESPONSE = DESCRIPTOR.message_types_by_name['ListT2sDomainsResponse']
 _T2SPIPELINEID = DESCRIPTOR.message_types_by_name['T2sPipelineId']
 _TEXT2SPEECHCONFIG = DESCRIPTOR.message_types_by_name['Text2SpeechConfig']
 _T2SDESCRIPTION = DESCRIPTOR.message_types_by_name['T2SDescription']
 _T2SINFERENCE = DESCRIPTOR.message_types_by_name['T2SInference']
 _COMPOSITEINFERENCE = DESCRIPTOR.message_types_by_name['CompositeInference']
+_SINGLEINFERENCE = DESCRIPTOR.message_types_by_name['SingleInference']
 _TEXT2MEL = DESCRIPTOR.message_types_by_name['Text2Mel']
+_TEXT2AUDIO = DESCRIPTOR.message_types_by_name['Text2Audio']
 _GLOWTTS = DESCRIPTOR.message_types_by_name['GlowTTS']
 _GLOWTTSTRITON = DESCRIPTOR.message_types_by_name['GlowTTSTriton']
+_VITS = DESCRIPTOR.message_types_by_name['Vits']
+_VITSTRITON = DESCRIPTOR.message_types_by_name['VitsTriton']
 _MEL2AUDIO = DESCRIPTOR.message_types_by_name['Mel2Audio']
 _HIFIGAN = DESCRIPTOR.message_types_by_name['HiFiGan']
 _HIFIGANTRITON = DESCRIPTOR.message_types_by_name['HiFiGanTriton']
 _MBMELGANTRITON = DESCRIPTOR.message_types_by_name['MbMelganTriton']
 _CACHING = DESCRIPTOR.message_types_by_name['Caching']
 _T2SNORMALIZATION = DESCRIPTOR.message_types_by_name['T2SNormalization']
 _POSTPROCESSING = DESCRIPTOR.message_types_by_name['Postprocessing']
@@ -208,35 +212,63 @@
 CompositeInference = _reflection.GeneratedProtocolMessageType('CompositeInference', (_message.Message,), {
   'DESCRIPTOR' : _COMPOSITEINFERENCE,
   '__module__' : 'ondewo.t2s.text_to_speech_pb2'
   # @@protoc_insertion_point(class_scope:ondewo.t2s.CompositeInference)
   })
 _sym_db.RegisterMessage(CompositeInference)
 
+SingleInference = _reflection.GeneratedProtocolMessageType('SingleInference', (_message.Message,), {
+  'DESCRIPTOR' : _SINGLEINFERENCE,
+  '__module__' : 'ondewo.t2s.text_to_speech_pb2'
+  # @@protoc_insertion_point(class_scope:ondewo.t2s.SingleInference)
+  })
+_sym_db.RegisterMessage(SingleInference)
+
 Text2Mel = _reflection.GeneratedProtocolMessageType('Text2Mel', (_message.Message,), {
   'DESCRIPTOR' : _TEXT2MEL,
   '__module__' : 'ondewo.t2s.text_to_speech_pb2'
   # @@protoc_insertion_point(class_scope:ondewo.t2s.Text2Mel)
   })
 _sym_db.RegisterMessage(Text2Mel)
 
+Text2Audio = _reflection.GeneratedProtocolMessageType('Text2Audio', (_message.Message,), {
+  'DESCRIPTOR' : _TEXT2AUDIO,
+  '__module__' : 'ondewo.t2s.text_to_speech_pb2'
+  # @@protoc_insertion_point(class_scope:ondewo.t2s.Text2Audio)
+  })
+_sym_db.RegisterMessage(Text2Audio)
+
 GlowTTS = _reflection.GeneratedProtocolMessageType('GlowTTS', (_message.Message,), {
   'DESCRIPTOR' : _GLOWTTS,
   '__module__' : 'ondewo.t2s.text_to_speech_pb2'
   # @@protoc_insertion_point(class_scope:ondewo.t2s.GlowTTS)
   })
 _sym_db.RegisterMessage(GlowTTS)
 
 GlowTTSTriton = _reflection.GeneratedProtocolMessageType('GlowTTSTriton', (_message.Message,), {
   'DESCRIPTOR' : _GLOWTTSTRITON,
   '__module__' : 'ondewo.t2s.text_to_speech_pb2'
   # @@protoc_insertion_point(class_scope:ondewo.t2s.GlowTTSTriton)
   })
 _sym_db.RegisterMessage(GlowTTSTriton)
 
+Vits = _reflection.GeneratedProtocolMessageType('Vits', (_message.Message,), {
+  'DESCRIPTOR' : _VITS,
+  '__module__' : 'ondewo.t2s.text_to_speech_pb2'
+  # @@protoc_insertion_point(class_scope:ondewo.t2s.Vits)
+  })
+_sym_db.RegisterMessage(Vits)
+
+VitsTriton = _reflection.GeneratedProtocolMessageType('VitsTriton', (_message.Message,), {
+  'DESCRIPTOR' : _VITSTRITON,
+  '__module__' : 'ondewo.t2s.text_to_speech_pb2'
+  # @@protoc_insertion_point(class_scope:ondewo.t2s.VitsTriton)
+  })
+_sym_db.RegisterMessage(VitsTriton)
+
 Mel2Audio = _reflection.GeneratedProtocolMessageType('Mel2Audio', (_message.Message,), {
   'DESCRIPTOR' : _MEL2AUDIO,
   '__module__' : 'ondewo.t2s.text_to_speech_pb2'
   # @@protoc_insertion_point(class_scope:ondewo.t2s.Mel2Audio)
   })
 _sym_db.RegisterMessage(Mel2Audio)
 
@@ -359,18 +391,18 @@
   })
 _sym_db.RegisterMessage(CreateCustomPhonemizerRequest)
 
 _TEXT2SPEECH = DESCRIPTOR.services_by_name['Text2Speech']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _PCM._serialized_start=4773
-  _PCM._serialized_end=4861
-  _AUDIOFORMAT._serialized_start=4863
-  _AUDIOFORMAT._serialized_end=4940
+  _PCM._serialized_start=5376
+  _PCM._serialized_end=5464
+  _AUDIOFORMAT._serialized_start=5466
+  _AUDIOFORMAT._serialized_end=5543
   _SYNTHESIZEREQUEST._serialized_start=76
   _SYNTHESIZEREQUEST._serialized_end=152
   _BATCHSYNTHESIZEREQUEST._serialized_start=154
   _BATCHSYNTHESIZEREQUEST._serialized_end=232
   _BATCHSYNTHESIZERESPONSE._serialized_start=234
   _BATCHSYNTHESIZERESPONSE._serialized_end=315
   _REQUESTCONFIG._serialized_start=318
@@ -397,58 +429,66 @@
   _LISTT2SDOMAINSRESPONSE._serialized_end=1568
   _T2SPIPELINEID._serialized_start=1570
   _T2SPIPELINEID._serialized_end=1597
   _TEXT2SPEECHCONFIG._serialized_start=1600
   _TEXT2SPEECHCONFIG._serialized_end=1846
   _T2SDESCRIPTION._serialized_start=1849
   _T2SDESCRIPTION._serialized_end=1984
-  _T2SINFERENCE._serialized_start=1986
-  _T2SINFERENCE._serialized_end=2113
-  _COMPOSITEINFERENCE._serialized_start=2115
-  _COMPOSITEINFERENCE._serialized_end=2217
-  _TEXT2MEL._serialized_start=2219
-  _TEXT2MEL._serialized_end=2334
-  _GLOWTTS._serialized_start=2337
-  _GLOWTTS._serialized_end=2485
-  _GLOWTTSTRITON._serialized_start=2488
-  _GLOWTTSTRITON._serialized_end=2719
-  _MEL2AUDIO._serialized_start=2722
-  _MEL2AUDIO._serialized_end=2892
-  _HIFIGAN._serialized_start=2894
-  _HIFIGAN._serialized_end=2981
-  _HIFIGANTRITON._serialized_start=2983
-  _HIFIGANTRITON._serialized_end=3102
-  _MBMELGANTRITON._serialized_start=3105
-  _MBMELGANTRITON._serialized_end=3245
-  _CACHING._serialized_start=3248
-  _CACHING._serialized_end=3391
-  _T2SNORMALIZATION._serialized_start=3394
-  _T2SNORMALIZATION._serialized_end=3620
-  _POSTPROCESSING._serialized_start=3623
-  _POSTPROCESSING._serialized_end=3799
-  _LOGMNSE._serialized_start=3801
-  _LOGMNSE._serialized_end=3879
-  _WIENER._serialized_start=3881
-  _WIENER._serialized_end=3978
-  _APODIZATION._serialized_start=3980
-  _APODIZATION._serialized_end=4019
-  _T2SCUSTOMLENGTHSCALES._serialized_start=4022
-  _T2SCUSTOMLENGTHSCALES._serialized_end=4190
-  _PHONEMIZERID._serialized_start=4192
-  _PHONEMIZERID._serialized_end=4218
-  _CUSTOMPHONEMIZERPROTO._serialized_start=4220
-  _CUSTOMPHONEMIZERPROTO._serialized_end=4286
-  _MAP._serialized_start=4288
-  _MAP._serialized_end=4331
-  _LISTCUSTOMPHONEMIZERRESPONSE._serialized_start=4333
-  _LISTCUSTOMPHONEMIZERRESPONSE._serialized_end=4419
-  _LISTCUSTOMPHONEMIZERREQUEST._serialized_start=4421
-  _LISTCUSTOMPHONEMIZERREQUEST._serialized_end=4472
-  _UPDATECUSTOMPHONEMIZERREQUEST._serialized_start=4475
-  _UPDATECUSTOMPHONEMIZERREQUEST._serialized_end=4691
-  _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_start=4630
-  _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_end=4691
-  _CREATECUSTOMPHONEMIZERREQUEST._serialized_start=4693
-  _CREATECUSTOMPHONEMIZERREQUEST._serialized_end=4771
-  _TEXT2SPEECH._serialized_start=4943
-  _TEXT2SPEECH._serialized_end=6340
+  _T2SINFERENCE._serialized_start=1987
+  _T2SINFERENCE._serialized_end=2169
+  _COMPOSITEINFERENCE._serialized_start=2171
+  _COMPOSITEINFERENCE._serialized_end=2273
+  _SINGLEINFERENCE._serialized_start=2275
+  _SINGLEINFERENCE._serialized_end=2336
+  _TEXT2MEL._serialized_start=2338
+  _TEXT2MEL._serialized_end=2453
+  _TEXT2AUDIO._serialized_start=2455
+  _TEXT2AUDIO._serialized_end=2558
+  _GLOWTTS._serialized_start=2561
+  _GLOWTTS._serialized_end=2709
+  _GLOWTTSTRITON._serialized_start=2712
+  _GLOWTTSTRITON._serialized_end=2943
+  _VITS._serialized_start=2946
+  _VITS._serialized_end=3091
+  _VITSTRITON._serialized_start=3094
+  _VITSTRITON._serialized_end=3322
+  _MEL2AUDIO._serialized_start=3325
+  _MEL2AUDIO._serialized_end=3495
+  _HIFIGAN._serialized_start=3497
+  _HIFIGAN._serialized_end=3584
+  _HIFIGANTRITON._serialized_start=3586
+  _HIFIGANTRITON._serialized_end=3705
+  _MBMELGANTRITON._serialized_start=3708
+  _MBMELGANTRITON._serialized_end=3848
+  _CACHING._serialized_start=3851
+  _CACHING._serialized_end=3994
+  _T2SNORMALIZATION._serialized_start=3997
+  _T2SNORMALIZATION._serialized_end=4223
+  _POSTPROCESSING._serialized_start=4226
+  _POSTPROCESSING._serialized_end=4402
+  _LOGMNSE._serialized_start=4404
+  _LOGMNSE._serialized_end=4482
+  _WIENER._serialized_start=4484
+  _WIENER._serialized_end=4581
+  _APODIZATION._serialized_start=4583
+  _APODIZATION._serialized_end=4622
+  _T2SCUSTOMLENGTHSCALES._serialized_start=4625
+  _T2SCUSTOMLENGTHSCALES._serialized_end=4793
+  _PHONEMIZERID._serialized_start=4795
+  _PHONEMIZERID._serialized_end=4821
+  _CUSTOMPHONEMIZERPROTO._serialized_start=4823
+  _CUSTOMPHONEMIZERPROTO._serialized_end=4889
+  _MAP._serialized_start=4891
+  _MAP._serialized_end=4934
+  _LISTCUSTOMPHONEMIZERRESPONSE._serialized_start=4936
+  _LISTCUSTOMPHONEMIZERRESPONSE._serialized_end=5022
+  _LISTCUSTOMPHONEMIZERREQUEST._serialized_start=5024
+  _LISTCUSTOMPHONEMIZERREQUEST._serialized_end=5075
+  _UPDATECUSTOMPHONEMIZERREQUEST._serialized_start=5078
+  _UPDATECUSTOMPHONEMIZERREQUEST._serialized_end=5294
+  _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_start=5233
+  _UPDATECUSTOMPHONEMIZERREQUEST_UPDATEMETHOD._serialized_end=5294
+  _CREATECUSTOMPHONEMIZERREQUEST._serialized_start=5296
+  _CREATECUSTOMPHONEMIZERREQUEST._serialized_end=5374
+  _TEXT2SPEECH._serialized_start=5546
+  _TEXT2SPEECH._serialized_end=6943
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-t2s-client-5.2.0/ondewo/t2s/text_to_speech_pb2_grpc.py` & `ondewo-t2s-client-5.3.0/ondewo/t2s/text_to_speech_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-t2s-client-5.2.0/ondewo_t2s_client.egg-info/PKG-INFO` & `ondewo-t2s-client-5.3.0/ondewo_t2s_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-t2s-client
-Version: 5.2.0
+Version: 5.3.0
 Summary: provides endpoints and messages for gRPC communication with the ONDEWO T2S server
 Home-page: https://github.com/ondewo/ondewo-t2s-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-t2s-client Version: 5.2.0 Summary: provides
+Metadata-Version: 2.1 Name: ondewo-t2s-client Version: 5.3.0 Summary: provides
 endpoints and messages for gRPC communication with the ONDEWO T2S server Home-
 page: https://github.com/ondewo/ondewo-t2s-client-python Author: Ondewo GbmH
 Author-email: office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-t2s-client-5.2.0/ondewo_t2s_client.egg-info/SOURCES.txt` & `ondewo-t2s-client-5.3.0/ondewo_t2s_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-t2s-client-5.2.0/setup.py` & `ondewo-t2s-client-5.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requires = f.read().splitlines()
 
 setup(
     name="ondewo-t2s-client",
-    version='5.2.0',
+    version='5.3.0',
     author="Ondewo GbmH",
     author_email="office@ondewo.com",
     description="provides endpoints and messages for gRPC communication with the ONDEWO T2S server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-t2s-client-python",
     packages=[
```

