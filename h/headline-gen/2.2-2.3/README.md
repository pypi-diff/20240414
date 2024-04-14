# Comparing `tmp/headline-gen-2.2.tar.gz` & `tmp/headline-gen-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headline-gen-2.2.tar", last modified: Thu Apr 11 07:43:23 2024, max compression
+gzip compressed data, was "headline-gen-2.3.tar", last modified: Sun Apr 14 04:15:56 2024, max compression
```

## Comparing `headline-gen-2.2.tar` & `headline-gen-2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 07:43:23.078470 headline-gen-2.2/
--rw-r--r--   0 root         (0) root         (0)     1313 2024-04-11 07:43:23.077469 headline-gen-2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2024-04-11 07:40:19.000000 headline-gen-2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 07:43:23.076470 headline-gen-2.2/headline_gen/
--rw-r--r--   0 root         (0) root         (0)    13160 2024-04-11 07:34:45.000000 headline-gen-2.2/headline_gen/Control.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 07:34:12.000000 headline-gen-2.2/headline_gen/__Init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 07:43:23.077469 headline-gen-2.2/headline_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1313 2024-04-11 07:43:22.000000 headline-gen-2.2/headline_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-11 07:43:23.000000 headline-gen-2.2/headline_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 07:43:22.000000 headline-gen-2.2/headline_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-11 07:43:22.000000 headline-gen-2.2/headline_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-11 07:43:22.000000 headline-gen-2.2/headline_gen.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 07:43:23.078470 headline-gen-2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      753 2024-04-11 07:43:06.000000 headline-gen-2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:15:56.885376 headline-gen-2.3/
+-rw-r--r--   0 root         (0) root         (0)     1817 2024-04-14 04:15:56.885376 headline-gen-2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-14 04:11:58.000000 headline-gen-2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:15:56.883376 headline-gen-2.3/headline_gen/
+-rw-r--r--   0 root         (0) root         (0)    13480 2024-04-14 04:03:22.000000 headline-gen-2.3/headline_gen/Control.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 04:02:19.000000 headline-gen-2.3/headline_gen/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:15:56.885376 headline-gen-2.3/headline_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1817 2024-04-14 04:15:56.000000 headline-gen-2.3/headline_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-14 04:15:56.000000 headline-gen-2.3/headline_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 04:15:56.000000 headline-gen-2.3/headline_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-14 04:15:56.000000 headline-gen-2.3/headline_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-14 04:15:56.000000 headline-gen-2.3/headline_gen.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 04:15:56.886376 headline-gen-2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      812 2024-04-14 04:15:39.000000 headline-gen-2.3/setup.py
```

### Comparing `headline-gen-2.2/PKG-INFO` & `headline-gen-2.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 Metadata-Version: 2.1
 Name: headline-gen
-Version: 2.2
-Summary: This package provides functionality to generate headlines from articles using natural language processing techniques.
+Version: 2.3
+Summary: Provides functionality to generate headlines from articles using natural language processing techniques.
 Author: venkatchoudharyala
 Author-email: venkatchoudhary.ala@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 
 # Headline Generation Package
 
-This is a Python package for generating headlines from article text.
+This is a Python package for generating headlines from Articles.
+
+## Installation
+
+You can install the package using pip:
+
+```bash
+pip install headline-gen
+```
 
 ## Usage
 
 ```python
-from headline_gen.Control import ServerInit, Generate
+from headline_gen.Control import ServerCntrl, Generate
 
 # Run this once to start the server
-Server = ServerInit("Start")
+Server = ServerCntrl("Start")
 
 # Generate headline from article text
 headline = Generate("Your article text goes here...", Server)
 print(headline)
 
 # Stop the server when done
-ServerInit("Stop", Server)
+ServerCntrl("Stop", Server)
 ```
 
 ## Description
 
 This package provides functionality to generate headlines from article text using natural language processing techniques.
 
-## Installation
-
-You can install the package using pip:
-
-```bash
-pip install headline-gen
-```
-
 ## Usage Instructions
 
-1. Import the `ServerInit` and `Generate` functions from the `Control` module.
-2. Start the server using `ServerInit("Start")`. This only needs to be done once.
+1. Import the `ServerCntrl` and `Generate` functions from the `Control` module.
+2. Start the server using `ServerCntrl("Start")`. This only needs to be done once.
 3. Generate headlines using the `Generate` function, passing the article text as an argument.
-4. Stop the server when done using `ServerInit("Stop", Server)`.
+4. Stop the server when done using `ServerCntrl("Stop", Server)`.
+
+## New Release Features (v2.3) and Bug Fixes
+
+1. Fixed a corner case issue causing a ZeroDivisionError when processing irregular parameters for phrase extraction. The package now gracefully handles such scenarios without disrupting functionality.
+2. Renamed the function `ServerInit` to `ServerCntrl` for improved clarity and consistency within the codebase.
+3. Additionally, streamlined the dependency management by directly including `en_core_web_sm` in the downloader module.
+4. Output made more Comprehensive.
```

### Comparing `headline-gen-2.2/headline_gen/Control.py` & `headline-gen-2.3/headline_gen/Control.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import zipfile
 import os
 import nltk
 
 from nltk.parse.corenlp import CoreNLPServer
 
+from spacy_download import load_spacy
 import textacy
 from textacy import *
 import string
 
 import re
 import numpy as np
 from nltk.tokenize import sent_tokenize
@@ -32,14 +33,15 @@
 # Downloader
 
 def Downloader():
   directory_path = "Parser/stanford-corenlp-4.5.6"
   if os.path.exists(directory_path) and os.listdir(directory_path):
     pass
   else:
+    nlp = load_spacy("en_core_web_sm") 
     nltk.download('punkt')
     nltk.download('stopwords')
     url = "https://nlp.stanford.edu/software/stanford-corenlp-4.5.6.zip"
 
     filename = "stanford-corenlp-4.5.6.zip"
     directory = "./Parser/"
 
@@ -54,15 +56,15 @@
 
         with zipfile.ZipFile(os.path.join(directory, filename), 'r') as zip_ref:
             zip_ref.extractall(directory)
         print("Extraction successful.")
     else:
         print("Failed to download file.")
 
-def ServerInit(Mode, Server = None):
+def ServerCntrl(Mode, Server = None):
   Path = 'Parser/'
   os.environ['CLASSPATH'] = os.path.join(Path, 'stanford-corenlp-4.5.6')
 
   directory_path = "Parser/stanford-corenlp-4.5.6"
   if os.path.exists(directory_path) and os.listdir(directory_path):
     if Mode == "Start":
       server = CoreNLPServer()
@@ -76,15 +78,15 @@
     else:
       print("Un defined Operation")
   else:
     print("Parser Files Not Found")
     print("Attempting to Install Parser Files (This may take a Min or Two!!)")
     Downloader()
     if Mode == "Start":
-      server = ServerInit("Start")
+      server = ServerCntrl("Start")
       return server
 
 # Key Phrase Extraction
 
 def remove_punctuation(text):
   table = str.maketrans('', '', string.punctuation)
   return text.translate(table)
@@ -93,16 +95,21 @@
   en = textacy.load_spacy_lang("en_core_web_sm")
 
   Article = remove_punctuation(Article)
 
   doc = textacy.make_spacy_doc(Article, lang=en)
 
   TopPhrases = [kps for kps, weights in textacy.extract.keyterms.sgrank(doc, ngrams = (1, 3), topn=1.0)]
-  print(TopPhrases)
-  return TopPhrases
+  if len(TopPhrases) != 0:
+    print("...Key Phrases Found...")
+    print(TopPhrases)
+    return TopPhrases
+  else:
+    print("No Specific Key Phrases Found, Terminating the Execution...")
+    exit()
 
 # Lead Sentence Extraction
 
 class LeadSentencesOOPS:
   def __init__(self, df):
     self.df = df
     self.sentences = sent_tokenize(self.df)
@@ -395,31 +402,33 @@
     for text in slices:
         corrected = process_segment(text, tokenizer, model, start_word, encoder_max_length)
         result += corrected + ' '
         start_word = overlap
     return result
 
 def PostProcess(Sentence):
-  checkpoint = "unikei/distilbert-base-re-punctuate"
+  checkpoint = "venkatchoudharyala/Punctuate"
   tokenizer = DistilBertTokenizerFast.from_pretrained(checkpoint)
   model = DistilBertForTokenClassification.from_pretrained(checkpoint)
   encoder_max_length = 256
   return punctuate(Sentence, tokenizer, model, encoder_max_length)
 
 def Generate(Article, Server):
   cleaned_article = re.sub(r'\([^)]*\)', '', Article)
 
   KeyPhrases = KeyPhraseSGRank(cleaned_article)
 
   LSG = LeadSentencesOOPS(cleaned_article)
   LeadingSentences  = LSG.leading_sentences()
   #LeadingSentences = leading_sentences(cleaned_article)
   #LeadingSentences = get_first_sentences(cleaned_article)
+  print("...Leading Sentences Found...")
   print(LeadingSentences)
 
   CompressedSentences = CompressionAlgorithm(LeadingSentences, KeyPhrases, Server)
 
   ResultDict = Ranking(CompressedSentences, KeyPhrases)
 
   max_key = max(ResultDict, key=lambda k: ResultDict[k])
+  print("...Scores of Sentences...")
   print(ResultDict)
   return PostProcess(max_key)
```

### Comparing `headline-gen-2.2/headline_gen.egg-info/PKG-INFO` & `headline-gen-2.3/headline_gen.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 Metadata-Version: 2.1
 Name: headline-gen
-Version: 2.2
-Summary: This package provides functionality to generate headlines from articles using natural language processing techniques.
+Version: 2.3
+Summary: Provides functionality to generate headlines from articles using natural language processing techniques.
 Author: venkatchoudharyala
 Author-email: venkatchoudhary.ala@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 
 # Headline Generation Package
 
-This is a Python package for generating headlines from article text.
+This is a Python package for generating headlines from Articles.
+
+## Installation
+
+You can install the package using pip:
+
+```bash
+pip install headline-gen
+```
 
 ## Usage
 
 ```python
-from headline_gen.Control import ServerInit, Generate
+from headline_gen.Control import ServerCntrl, Generate
 
 # Run this once to start the server
-Server = ServerInit("Start")
+Server = ServerCntrl("Start")
 
 # Generate headline from article text
 headline = Generate("Your article text goes here...", Server)
 print(headline)
 
 # Stop the server when done
-ServerInit("Stop", Server)
+ServerCntrl("Stop", Server)
 ```
 
 ## Description
 
 This package provides functionality to generate headlines from article text using natural language processing techniques.
 
-## Installation
-
-You can install the package using pip:
-
-```bash
-pip install headline-gen
-```
-
 ## Usage Instructions
 
-1. Import the `ServerInit` and `Generate` functions from the `Control` module.
-2. Start the server using `ServerInit("Start")`. This only needs to be done once.
+1. Import the `ServerCntrl` and `Generate` functions from the `Control` module.
+2. Start the server using `ServerCntrl("Start")`. This only needs to be done once.
 3. Generate headlines using the `Generate` function, passing the article text as an argument.
-4. Stop the server when done using `ServerInit("Stop", Server)`.
+4. Stop the server when done using `ServerCntrl("Stop", Server)`.
+
+## New Release Features (v2.3) and Bug Fixes
+
+1. Fixed a corner case issue causing a ZeroDivisionError when processing irregular parameters for phrase extraction. The package now gracefully handles such scenarios without disrupting functionality.
+2. Renamed the function `ServerInit` to `ServerCntrl` for improved clarity and consistency within the codebase.
+3. Additionally, streamlined the dependency management by directly including `en_core_web_sm` in the downloader module.
+4. Output made more Comprehensive.
```

### Comparing `headline-gen-2.2/setup.py` & `headline-gen-2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='headline-gen',
-    version='2.2',
+    version='2.3',
     author='venkatchoudharyala',
     author_email='venkatchoudhary.ala@gmail.com',
-    description='This package provides functionality to generate headlines from articles using natural language processing techniques.',
+    description='Provides functionality to generate headlines from articles using natural language processing techniques.',
     long_description=open('README.md').read(),  # Read the contents of README.md
     long_description_content_type='text/markdown',  # Specify the content type of the l
     install_requires=[
-        'requests',
-        'nltk',
-        'string',
-        'numpy',
-        'scipy',
-        'gensim',
-        'networkx',
-        'textacy',
-        'transformers',
-        'torch'
+        'requests==2.31.0',
+        'nltk==3.8.1',
+        'numpy==1.26.4',
+        'scipy==1.12.0',
+        'gensim==4.3.2',
+        'networkx==3.3',
+        'textacy==0.13.0',
+        'transformers==4.39.3',
+        'torch==2.2.2',
+        'spacy==1.1.0'
     ],
     python_requires='>=3.6',
 )
```

