# Comparing `tmp/faster_translate-0.1.5.tar.gz` & `tmp/faster_translate-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_translate-0.1.5.tar", last modified: Sat Apr 13 21:19:19 2024, max compression
+gzip compressed data, was "faster_translate-0.1.7.tar", last modified: Sun Apr 14 18:55:31 2024, max compression
```

## Comparing `faster_translate-0.1.5.tar` & `faster_translate-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:19:19.309220 faster_translate-0.1.5/
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     1069 2024-04-13 18:30:01.000000 faster_translate-0.1.5/LICENSE
--rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-13 21:19:19.309220 faster_translate-0.1.5/PKG-INFO
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2974 2024-04-13 18:30:01.000000 faster_translate-0.1.5/README.md
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:19:19.309220 faster_translate-0.1.5/faster_translate/
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       75 2024-04-13 18:35:30.000000 faster_translate-0.1.5/faster_translate/__init__.py
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     6728 2024-04-13 21:18:13.000000 faster_translate-0.1.5/faster_translate/model.py
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2057 2024-04-13 18:35:30.000000 faster_translate-0.1.5/faster_translate/utils.py
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-13 21:19:19.309220 faster_translate-0.1.5/faster_translate.egg-info/
--rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/PKG-INFO
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      312 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/SOURCES.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)        1 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/dependency_links.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       91 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/requires.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       17 2024-04-13 21:19:19.000000 faster_translate-0.1.5/faster_translate.egg-info/top_level.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      676 2024-04-13 21:19:08.000000 faster_translate-0.1.5/pyproject.toml
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       38 2024-04-13 21:19:19.309220 faster_translate-0.1.5/setup.cfg
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-14 18:55:31.898257 faster_translate-0.1.7/
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     1069 2024-04-13 18:30:01.000000 faster_translate-0.1.7/LICENSE
+-rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-14 18:55:31.898257 faster_translate-0.1.7/PKG-INFO
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2974 2024-04-13 18:30:01.000000 faster_translate-0.1.7/README.md
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-14 18:55:31.898257 faster_translate-0.1.7/faster_translate/
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       75 2024-04-13 18:35:30.000000 faster_translate-0.1.7/faster_translate/__init__.py
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     7350 2024-04-14 18:54:36.000000 faster_translate-0.1.7/faster_translate/model.py
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2244 2024-04-14 18:54:44.000000 faster_translate-0.1.7/faster_translate/utils.py
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-14 18:55:31.898257 faster_translate-0.1.7/faster_translate.egg-info/
+-rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-14 18:55:31.000000 faster_translate-0.1.7/faster_translate.egg-info/PKG-INFO
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      312 2024-04-14 18:55:31.000000 faster_translate-0.1.7/faster_translate.egg-info/SOURCES.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)        1 2024-04-14 18:55:31.000000 faster_translate-0.1.7/faster_translate.egg-info/dependency_links.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       91 2024-04-14 18:55:31.000000 faster_translate-0.1.7/faster_translate.egg-info/requires.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       17 2024-04-14 18:55:31.000000 faster_translate-0.1.7/faster_translate.egg-info/top_level.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      676 2024-04-14 18:54:59.000000 faster_translate-0.1.7/pyproject.toml
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       38 2024-04-14 18:55:31.898257 faster_translate-0.1.7/setup.cfg
```

### Comparing `faster_translate-0.1.5/LICENSE` & `faster_translate-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.5/PKG-INFO` & `faster_translate-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.5
+Version: 0.1.7
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `faster_translate-0.1.5/README.md` & `faster_translate-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.5/faster_translate/model.py` & `faster_translate-0.1.7/faster_translate/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,33 +24,45 @@
         return True
 
     return False
 
 device_name = "cuda" if is_cuda_available() else "cpu"
 
 class TranslateModel:
-    def __init__(self, model_dir, source_token_list = None, normalizer_func=None, device = device_name):
+    def __init__(self, model_dir, source_token_list = None, tokenizer_filename = None, normalizer_func=None, device = device_name):
         self.model_dir = model_dir
         self.translator = ctranslate2.Translator(model_dir, device=device)
         
         if normalizer_func is None:
             self.normalizer_func = lambda x: x
         elif isinstance(normalizer_func, str):
             self.normalizer_func = self.get_text_normalizer(normalizer_func)
         else:
             self.normalizer_func = normalizer_func
             
             
         if source_token_list is None:
-            self.source_tokenizer_json = os.path.join(model_dir, "source_vocabulary.json")
-            with open(self.source_tokenizer_json, 'r', encoding='utf-8') as file:
-                source_token_list = json.load(file)
-            
+            source_token_list = self.get_token_list(tokenizer_filename)
         self.source_tokenizer = self.get_bpe_tokenizer(source_token_list)
         
+    def get_token_list(tokenizer_filename):
+        if tokenizer_filename is not None:
+            tokenizer_filepath  = os.path.join(self.model_dir, tokenizer_filename)
+        elif os.path.isfile(os.path.join(self.model_dir, "source_vocabulary.json")):
+            tokenizer_filepath  = os.path.join(self.model_dir, "source_vocabulary.json")
+        elif os.path.isfile(os.path.join(self.model_dir, "shared_vocabulary.json")):
+            tokenizer_filepath  = os.path.join(self.model_dir, "shared_vocabulary.json")
+        else:
+            raise Exception("Vocabulary file was not found.")
+        
+            # self.source_tokenizer_json = os.path.join(model_dir, "source_vocabulary.json")
+        with open(tokenizer_filepath, 'r', encoding='utf-8') as file:
+            source_token_list = json.load(file)
+        return source_token_list
+    
         
     def get_bpe_tokenizer(self, token_list):
         
         # Initialize a tokenizer
         tokenizer = Tokenizer(BPE(unk_token="<unk>"))
         tokenizer.pre_tokenizer = Whitespace()
         
@@ -150,15 +162,14 @@
             
         # Check if model_identifier is a local directory
         if os.path.isdir(model_name_or_path):
             print(f"Loading model from local directory: {model_name_or_path}")
             model_path = model_name_or_path
         else:
             # Download the model using the utility function from faster_translate/utils.py
-            print(f"Downloading model from Hugging Face repository: {model_name_or_path}")
             model_path = download_model_hf(model_name_or_path, save_path, revision, token)
         
         return TranslateModel(model_path, **kwargs)
```

### Comparing `faster_translate-0.1.5/faster_translate/utils.py` & `faster_translate-0.1.7/faster_translate/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 _MODELS = {
     "banglanmt_bn2en": {
         "model_repo": "sawradip/faster-translate-banglanmt-bn2en-t5",
         "normalizer_func":"buetnlpnormalizer"
     },
     "banglanmt_en2bn": {
         "model_repo": "sawradip/faster-translate-banglanmt-en2bn-t5"
+    },
+    "banglabertv1_en2bn": {
+        "model_repo": "sawradip/faster-translate-banglabart-en2bn-v1"
     }
 }
 def upload_model_hf(repo_name, folder_path, token ):
     """
     Upload all files from a folder to a Hugging Face repository.
 
     Parameters:
@@ -41,15 +44,16 @@
     - revision: The specific repository revision to download. If None, the latest version is downloaded.
     - token: An optional Hugging Face authentication token for private repositories.
     """
     # Use snapshot_download to download the repository or a specific snapshot of it
     if repo_name in _MODELS:
         model_args = _MODELS[repo_name]
         repo_name = model_args["model_repo"]
-
+        
+    print(f"Downloading model from Hugging Face repository: {repo_name}")
     downloaded_path = snapshot_download(
         repo_id=repo_name,
         cache_dir=save_path,  
         revision=revision,
         token=token if token else None  
     )
```

### Comparing `faster_translate-0.1.5/faster_translate.egg-info/PKG-INFO` & `faster_translate-0.1.7/faster_translate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.5
+Version: 0.1.7
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `faster_translate-0.1.5/pyproject.toml` & `faster_translate-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faster_translate"
-version = "0.1.5"
+version = "0.1.7"
 description = "A simple translation utility using Hugging Face models."
 readme = "README.md"
 authors = [{name = "Sawradip Saha", email = "sawradip0@gmail.com"}]
 license = {file = "LICENSE"}
 keywords = ["translation", "huggingface", "nlp"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

