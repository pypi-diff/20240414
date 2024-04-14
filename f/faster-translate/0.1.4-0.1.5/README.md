# Comparing `tmp/faster_translate-0.1.4.tar.gz` & `tmp/faster_translate-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_translate-0.1.4.tar", last modified: Sat Apr 13 21:15:23 2024, max compression
+gzip compressed data, was "faster_translate-0.1.5.tar", last modified: Sat Apr 13 21:19:19 2024, max compression
```

## Comparing `faster_translate-0.1.4.tar` & `faster_translate-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:15:23.000898 faster_translate-0.1.4/
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     1069 2024-04-13 18:30:01.000000 faster_translate-0.1.4/LICENSE
--rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-13 21:15:23.000898 faster_translate-0.1.4/PKG-INFO
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2974 2024-04-13 18:30:01.000000 faster_translate-0.1.4/README.md
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:15:23.000898 faster_translate-0.1.4/faster_translate/
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       75 2024-04-13 18:35:30.000000 faster_translate-0.1.4/faster_translate/__init__.py
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     6764 2024-04-13 20:26:22.000000 faster_translate-0.1.4/faster_translate/model.py
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2057 2024-04-13 18:35:30.000000 faster_translate-0.1.4/faster_translate/utils.py
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:15:23.000898 faster_translate-0.1.4/faster_translate.egg-info/
--rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/PKG-INFO
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      312 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/SOURCES.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)        1 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/dependency_links.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       91 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/requires.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       17 2024-04-13 21:15:22.000000 faster_translate-0.1.4/faster_translate.egg-info/top_level.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      676 2024-04-13 21:15:16.000000 faster_translate-0.1.4/pyproject.toml
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       38 2024-04-13 21:15:23.000898 faster_translate-0.1.4/setup.cfg
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:19:19.309220 faster_translate-0.1.5/
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     1069 2024-04-13 18:30:01.000000 faster_translate-0.1.5/LICENSE
+-rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-13 21:19:19.309220 faster_translate-0.1.5/PKG-INFO
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2974 2024-04-13 18:30:01.000000 faster_translate-0.1.5/README.md
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:19:19.309220 faster_translate-0.1.5/faster_translate/
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       75 2024-04-13 18:35:30.000000 faster_translate-0.1.5/faster_translate/__init__.py
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     6728 2024-04-13 21:18:13.000000 faster_translate-0.1.5/faster_translate/model.py
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2057 2024-04-13 18:35:30.000000 faster_translate-0.1.5/faster_translate/utils.py
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:19:19.309220 faster_translate-0.1.5/faster_translate.egg-info/
+-rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/PKG-INFO
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      312 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/SOURCES.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)        1 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/dependency_links.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       91 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/requires.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       17 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/top_level.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      676 2024-04-13 21:19:08.000000 faster_translate-0.1.5/pyproject.toml
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       38 2024-04-13 21:19:19.309220 faster_translate-0.1.5/setup.cfg
```

### Comparing `faster_translate-0.1.4/LICENSE` & `faster_translate-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.4/PKG-INFO` & `faster_translate-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `faster_translate-0.1.4/README.md` & `faster_translate-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.4/faster_translate/model.py` & `faster_translate-0.1.5/faster_translate/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,14 @@
         translated_batch = self.translate_batch(text_batch)
         return translated_batch[0]
 
 
     def translate_batch(self, text_batch):
         normalized_text_batch = self.normalizer_func(text_batch)
         tokenized_text_batch = self.source_tokenize_batch(normalized_text_batch)
-        print(tokenized_text_batch)
         translated_tokens_batch = self.translator.translate_batch(tokenized_text_batch)
         translated_batch = self.detokenize_batch(translated_tokens_batch)
         return translated_batch
     
     
     def translate_bulk(self, text_list, batch_size=1):
         text_batches = [text_list[i:i + batch_size] for i in range(0, len(text_list), batch_size)]
```

### Comparing `faster_translate-0.1.4/faster_translate/utils.py` & `faster_translate-0.1.5/faster_translate/utils.py`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.4/faster_translate.egg-info/PKG-INFO` & `faster_translate-0.1.5/faster_translate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `faster_translate-0.1.4/pyproject.toml` & `faster_translate-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faster_translate"
-version = "0.1.4"
+version = "0.1.5"
 description = "A simple translation utility using Hugging Face models."
 readme = "README.md"
 authors = [{name = "Sawradip Saha", email = "sawradip0@gmail.com"}]
 license = {file = "LICENSE"}
 keywords = ["translation", "huggingface", "nlp"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

