# Comparing `tmp/document_ingestor-0.0.9.tar.gz` & `tmp/document_ingestor-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_ingestor-0.0.9.tar", last modified: Wed Apr 10 12:13:12 2024, max compression
+gzip compressed data, was "document_ingestor-0.1.0.tar", last modified: Sun Apr 14 15:51:25 2024, max compression
```

## Comparing `document_ingestor-0.0.9.tar` & `document_ingestor-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:13:12.093800 document_ingestor-0.0.9/
--rw-rw-rw-   0        0        0     1091 2024-03-24 16:55:37.000000 document_ingestor-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0     2387 2024-04-10 12:13:12.088534 document_ingestor-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-03-24 16:55:37.000000 document_ingestor-0.0.9/README.md
--rw-rw-rw-   0        0        0      869 2024-04-10 12:12:56.000000 document_ingestor-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 12:13:12.094865 document_ingestor-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 12:13:11.952494 document_ingestor-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 12:13:12.011983 document_ingestor-0.0.9/src/document_ingestor/
--rw-rw-rw-   0        0        0        0 2024-03-24 16:55:37.000000 document_ingestor-0.0.9/src/document_ingestor/__init__.py
--rw-rw-rw-   0        0        0     5779 2024-04-09 20:53:03.000000 document_ingestor-0.0.9/src/document_ingestor/embedding_process.py
--rw-rw-rw-   0        0        0     2474 2024-04-09 20:50:23.000000 document_ingestor-0.0.9/src/document_ingestor/genericParser.py
--rw-rw-rw-   0        0        0     6095 2024-04-09 20:45:08.000000 document_ingestor-0.0.9/src/document_ingestor/pdf_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:13:12.082130 document_ingestor-0.0.9/src/document_ingestor.egg-info/
--rw-rw-rw-   0        0        0     2387 2024-04-10 12:13:11.000000 document_ingestor-0.0.9/src/document_ingestor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2024-04-10 12:13:11.000000 document_ingestor-0.0.9/src/document_ingestor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:13:11.000000 document_ingestor-0.0.9/src/document_ingestor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-10 12:13:11.000000 document_ingestor-0.0.9/src/document_ingestor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-10 12:13:11.000000 document_ingestor-0.0.9/src/document_ingestor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 15:51:25.485863 document_ingestor-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-03-24 16:55:37.000000 document_ingestor-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2387 2024-04-14 15:51:25.481865 document_ingestor-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-03-24 16:55:37.000000 document_ingestor-0.1.0/README.md
+-rw-rw-rw-   0        0        0      869 2024-04-14 15:50:58.000000 document_ingestor-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:51:25.487917 document_ingestor-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 15:51:25.314776 document_ingestor-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 15:51:25.398017 document_ingestor-0.1.0/src/document_ingestor/
+-rw-rw-rw-   0        0        0        0 2024-03-24 16:55:37.000000 document_ingestor-0.1.0/src/document_ingestor/__init__.py
+-rw-rw-rw-   0        0        0     5779 2024-04-09 20:53:03.000000 document_ingestor-0.1.0/src/document_ingestor/embedding_process.py
+-rw-rw-rw-   0        0        0     1865 2024-04-14 15:41:27.000000 document_ingestor-0.1.0/src/document_ingestor/eu_data_parser.py
+-rw-rw-rw-   0        0        0     2744 2024-04-14 15:49:18.000000 document_ingestor-0.1.0/src/document_ingestor/genericParser.py
+-rw-rw-rw-   0        0        0     6095 2024-04-09 20:45:08.000000 document_ingestor-0.1.0/src/document_ingestor/pdf_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:51:25.477334 document_ingestor-0.1.0/src/document_ingestor.egg-info/
+-rw-rw-rw-   0        0        0     2387 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 15:51:25.000000 document_ingestor-0.1.0/src/document_ingestor.egg-info/top_level.txt
```

### Comparing `document_ingestor-0.0.9/LICENSE.txt` & `document_ingestor-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `document_ingestor-0.0.9/PKG-INFO` & `document_ingestor-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document_ingestor
-Version: 0.0.9
+Version: 0.1.0
 Summary: This package consumes one or more Spanish constitution PDFs and then processes them to generate embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors.
 Author-email: Milan Anand Raj <manandraj20@iitk.ac.in>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `document_ingestor-0.0.9/pyproject.toml` & `document_ingestor-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "document_ingestor"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name = "Milan Anand Raj", email = "manandraj20@iitk.ac.in" },
 ]
 description = "This package consumes one or more Spanish constitution PDFs and then processes them to generate embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `document_ingestor-0.0.9/src/document_ingestor/embedding_process.py` & `document_ingestor-0.1.0/src/document_ingestor/embedding_process.py`

 * *Files identical despite different names*

### Comparing `document_ingestor-0.0.9/src/document_ingestor/genericParser.py` & `document_ingestor-0.1.0/src/document_ingestor/genericParser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import json
 import fitz
-
+import re
 # global variables
 threshold_content_block= 10
 
+
+
+
 def get_blocks(pdf_document, start_page_number):
     complete_list_blocks = []
     for i in range(start_page_number, pdf_document.page_count):
         page = pdf_document[i-1]
         curr_page_list_blocks = [[block[4], i]
                                  for block in page.get_text("blocks", sort=False)[:-3]]  # last 3 blocks removed to remove headers and footers
         # if the first block of the current page is a continuation of the last block of the previous page
@@ -16,23 +19,30 @@
                 if curr_page_list_blocks[0][0][0].islower():
                     curr_page_list_blocks[0][0] = complete_list_blocks[-1][0]+curr_page_list_blocks[0][0]
                     curr_page_list_blocks.pop()
             except:
                 pass
         
         complete_list_blocks.extend(curr_page_list_blocks)
+
     return complete_list_blocks
 
-def partition_data(complete_list_blocks):
+def label_contents(complete_list_blocks):
     most_recent_heading_block = ["the associated first text was supposed to be the heading of the first content block", 0]
     headings_list = []
     contents_list = []
     last_content_window_list =[]
     for block in complete_list_blocks:
+        if block[0].strip() == "": 
+            continue
         num_words = len(block[0].split(" "))
+        # block[0] starts with the a natural number followed by a period
+        if re.match(r"^\d+\.", block[0]):
+            last_content_window_list.append(block[0])
+            continue
         if num_words < threshold_content_block:
             if last_content_window_list and most_recent_heading_block:
                 headings_list.append(most_recent_heading_block)
                 contents_list.append(last_content_window_list)
                 last_content_window_list = []
             most_recent_heading_block = block
         else:
@@ -47,15 +57,15 @@
     # #
     # #
     toc = pdf_document.get_toc()[2:]
     # #
     # # 
    
     complete_list_blocks = get_blocks(pdf_document, start_page_number) 
-    headings_list, contents_list = partition_data(complete_list_blocks)
+    headings_list, contents_list = label_contents(complete_list_blocks)
     json_list = []
     
 
     for heading, content in zip(headings_list, contents_list):
         json_data = {
         "level1": [book_title, 0],
         "level2": heading,
```

### Comparing `document_ingestor-0.0.9/src/document_ingestor/pdf_parser.py` & `document_ingestor-0.1.0/src/document_ingestor/pdf_parser.py`

 * *Files identical despite different names*

### Comparing `document_ingestor-0.0.9/src/document_ingestor.egg-info/PKG-INFO` & `document_ingestor-0.1.0/src/document_ingestor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document_ingestor
-Version: 0.0.9
+Version: 0.1.0
 Summary: This package consumes one or more Spanish constitution PDFs and then processes them to generate embedding vectors. The vectors are generated with OpenAI service and PineCone is used to store and retrieve embedding vectors.
 Author-email: Milan Anand Raj <manandraj20@iitk.ac.in>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

