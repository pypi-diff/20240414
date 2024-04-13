# Comparing `tmp/autopipeline-0.1.98.tar.gz` & `tmp/autopipeline-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopipeline-0.1.98.tar", last modified: Tue Jan 30 03:24:26 2024, max compression
+gzip compressed data, was "autopipeline-0.1.99.tar", last modified: Tue Jan 30 17:04:07 2024, max compression
```

## Comparing `autopipeline-0.1.98.tar` & `autopipeline-0.1.99.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 chuxuanhu   (503) staff       (20)        0 2024-01-30 03:24:26.936221 autopipeline-0.1.98/
--rw-r--r--   0 chuxuanhu   (503) staff       (20)      284 2024-01-30 03:24:26.936116 autopipeline-0.1.98/PKG-INFO
-drwxr-xr-x   0 chuxuanhu   (503) staff       (20)        0 2024-01-30 03:24:26.935343 autopipeline-0.1.98/autopipeline/
--rw-r--r--   0 chuxuanhu   (503) staff       (20)    12053 2024-01-30 00:01:12.000000 autopipeline-0.1.98/autopipeline/Filter.py
--rw-r--r--   0 chuxuanhu   (503) staff       (20)     3778 2024-01-29 21:22:35.000000 autopipeline-0.1.98/autopipeline/Interactive.py
--rw-r--r--   0 chuxuanhu   (503) staff       (20)   109549 2024-01-30 03:24:16.000000 autopipeline-0.1.98/autopipeline/Mapping.py
--rw-r--r--   0 chuxuanhu   (503) staff       (20)     4385 2024-01-25 01:48:30.000000 autopipeline-0.1.98/autopipeline/NL2SQL.py
--rw-r--r--   0 chuxuanhu   (503) staff       (20)      766 2024-01-19 22:05:32.000000 autopipeline-0.1.98/autopipeline/PipelineExec.py
--rw-r--r--   0 chuxuanhu   (503) staff       (20)    21382 2024-01-25 00:49:04.000000 autopipeline-0.1.98/autopipeline/PipelineGen.py
--rw-r--r--   0 chuxuanhu   (503) staff       (20)        0 2023-12-24 05:01:47.000000 autopipeline-0.1.98/autopipeline/__init__.py
-drwxr-xr-x   0 chuxuanhu   (503) staff       (20)        0 2024-01-30 03:24:26.935981 autopipeline-0.1.98/autopipeline/data/
--rw-r--r--   0 chuxuanhu   (503) staff       (20)        0 2023-12-24 05:31:40.000000 autopipeline-0.1.98/autopipeline/data/__init__.py
-drwxr-xr-x   0 chuxuanhu   (503) staff       (20)        0 2024-01-30 03:24:26.935858 autopipeline-0.1.98/autopipeline.egg-info/
--rw-r--r--   0 chuxuanhu   (503) staff       (20)      284 2024-01-30 03:24:26.000000 autopipeline-0.1.98/autopipeline.egg-info/PKG-INFO
--rw-r--r--   0 chuxuanhu   (503) staff       (20)      397 2024-01-30 03:24:26.000000 autopipeline-0.1.98/autopipeline.egg-info/SOURCES.txt
--rw-r--r--   0 chuxuanhu   (503) staff       (20)        1 2024-01-30 03:24:26.000000 autopipeline-0.1.98/autopipeline.egg-info/dependency_links.txt
--rw-r--r--   0 chuxuanhu   (503) staff       (20)      132 2024-01-30 03:24:26.000000 autopipeline-0.1.98/autopipeline.egg-info/requires.txt
--rw-r--r--   0 chuxuanhu   (503) staff       (20)       13 2024-01-30 03:24:26.000000 autopipeline-0.1.98/autopipeline.egg-info/top_level.txt
--rw-r--r--   0 chuxuanhu   (503) staff       (20)       38 2024-01-30 03:24:26.936261 autopipeline-0.1.98/setup.cfg
--rw-r--r--   0 chuxuanhu   (503) staff       (20)      876 2024-01-30 03:24:19.000000 autopipeline-0.1.98/setup.py
+drwxr-xr-x   0 chuxuanhu   (503) staff       (20)        0 2024-01-30 17:04:07.596562 autopipeline-0.1.99/
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)      284 2024-01-30 17:04:07.596446 autopipeline-0.1.99/PKG-INFO
+drwxr-xr-x   0 chuxuanhu   (503) staff       (20)        0 2024-01-30 17:04:07.595458 autopipeline-0.1.99/autopipeline/
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)    12311 2024-01-30 17:02:41.000000 autopipeline-0.1.99/autopipeline/Filter.py
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)     3778 2024-01-29 21:22:35.000000 autopipeline-0.1.99/autopipeline/Interactive.py
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)   109974 2024-01-30 17:03:52.000000 autopipeline-0.1.99/autopipeline/Mapping.py
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)     4385 2024-01-25 01:48:30.000000 autopipeline-0.1.99/autopipeline/NL2SQL.py
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)      766 2024-01-19 22:05:32.000000 autopipeline-0.1.99/autopipeline/PipelineExec.py
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)    21382 2024-01-25 00:49:04.000000 autopipeline-0.1.99/autopipeline/PipelineGen.py
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)        0 2023-12-24 05:01:47.000000 autopipeline-0.1.99/autopipeline/__init__.py
+drwxr-xr-x   0 chuxuanhu   (503) staff       (20)        0 2024-01-30 17:04:07.596266 autopipeline-0.1.99/autopipeline/data/
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)        0 2023-12-24 05:31:40.000000 autopipeline-0.1.99/autopipeline/data/__init__.py
+drwxr-xr-x   0 chuxuanhu   (503) staff       (20)        0 2024-01-30 17:04:07.596041 autopipeline-0.1.99/autopipeline.egg-info/
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)      284 2024-01-30 17:04:07.000000 autopipeline-0.1.99/autopipeline.egg-info/PKG-INFO
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)      397 2024-01-30 17:04:07.000000 autopipeline-0.1.99/autopipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)        1 2024-01-30 17:04:07.000000 autopipeline-0.1.99/autopipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)      132 2024-01-30 17:04:07.000000 autopipeline-0.1.99/autopipeline.egg-info/requires.txt
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)       13 2024-01-30 17:04:07.000000 autopipeline-0.1.99/autopipeline.egg-info/top_level.txt
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)       38 2024-01-30 17:04:07.596618 autopipeline-0.1.99/setup.cfg
+-rw-r--r--   0 chuxuanhu   (503) staff       (20)      876 2024-01-30 17:03:57.000000 autopipeline-0.1.99/setup.py
```

### Comparing `autopipeline-0.1.98/autopipeline/Filter.py` & `autopipeline-0.1.99/autopipeline/Filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
     "get_dog_whistle_persona_ingroup": "This function takes in one of the columns of dog whistle terms, obtain the target persona/in-group of that dog whistle term, and generate an additional column to include those."
     "get_dog_whistle_type": "This function takes in one of the columns of dog whistle terms, obtain the type of that dog whistle term, and generate an additional column to include those."
     "get_positive_reframing": "This function takes in one of the columns as input, extract the positive aspects of the content of that column and transforms it into a positive reframing version, and generates an additional column of positive reframing version of the content."
     "get_premise": "This function takes in one column of figurative text, one column of figurative type, and one column of figurative term as input, extracts the literal text, i.e., the premise, of the figurative text column, and generates a new column to include those."
     "get_premise_explanation": "This function takes in one column of premise of figurative text, one column of the original figurative text, one column of figurative type, one column of figurative term as input, and one parameter labelling whether the premises entail or contract original figurative texts as input, extracts the explanations of literal texts, i.e., the premises, of the figurative text column, and generates a new column to include those."
     "get_persuasion_effect": "This function takes in one of the columns as input, calculates the (numerical) persuasion effect score of the contents in that column, and generate an additional column to include those."
     "get_change_opinion": "This function takes in one of the columns as input, classifies whether the contents in that column changes opinion, and generate an additional column to include those."
-    "get_reader_action": "This function takes in one of the columns of writers' intent as input, get the reader action inferred from the writers' intent of that column, and generate additional an column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_intent'"
-    "get_reader_perception": "This function takes in one of the columns as input, infers readers' perceptions of text in that column, and generates an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_spread_likelihood'"
-    "get_intent": "This function takes in one of the columns as input, retrieve the intent of the writer of text in that column, and generate an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_reader_action'"
-    "get_spread_likelihood": "This function takes in one of the columns of readers' perceptions as input, calculates the (numerical) spread likelihood based on readers' perceptions in that column, and generate an additional column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_reader_perception'"
+    "get_reader_action": "This function takes in one of the columns of writers' intent as input, get the reader action inferred from the writers' intent of that column, and generate additional an column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_intent' UNLESS the base table already has a column of writer's intent."
+    "get_reader_perception": "This function takes in one of the columns as input, infers readers' perceptions of text in that column, and generates an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_spread_likelihood' UNLESS the base table already has a column of reader perceptions."
+    "get_intent": "This function takes in one of the columns as input, retrieve the intent of the writer of text in that column, and generate an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_reader_action' UNLESS the base table already has a column of writer's intent."
+    "get_spread_likelihood": "This function takes in one of the columns of readers' perceptions as input, calculates the (numerical) spread likelihood based on readers' perceptions in that column, and generate an additional column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_reader_perception' UNLESS the base table already has a column of reader perceptions."
     '''
     messages = [
         {
             "role": "system",
             "content": "Given a table with columns: " + columns 
             + " where " + description 
             + " You are also given functions to be applied to different columns: " + functions
```

### Comparing `autopipeline-0.1.98/autopipeline/Interactive.py` & `autopipeline-0.1.99/autopipeline/Interactive.py`

 * *Files identical despite different names*

### Comparing `autopipeline-0.1.98/autopipeline/Mapping.py` & `autopipeline-0.1.99/autopipeline/Mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1084,18 +1084,18 @@
     function_tree = '''
     {
         "text_processors" <contains functions that process texts>:
             "para_sep": "This function takes in one of the columns as input, split the text according to paragraphs, and generates an additional rows and columns to store the list of paragraphs."
             "pdf_to_text": "This function takes in one of the columns as input, transforms the pdf in that column into plain text, and generate an additional column to store the plain text." 
         "summarizer" <contains functions that summarize texts>:
             "get_summary": "This function takes in one of the columns as input, summarizes the contents in that column, and generate an additional column to include those."
-            "get_intent": "This function takes in one of the columns as input, retrieve the intent of the writer of text in that column, and generate an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_reader_action'"
+            "get_intent": "This function takes in one of the columns as input, retrieve the intent of the writer of text in that column, and generate an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_reader_action' UNLESS the base table already has a column of writer's intent."
         "calculator" <contains functions that calculate numerical scores from text>:
             "get_persuasion_effect": "This function takes in one of the columns as input, calculates the (numerical) persuasion effect score of the contents in that column, and generate an additional column to include those."
-            "get_spread_likelihood": "This function takes in one of the columns of readers' perceptions as input, calculates the (numerical) spread likelihood based on readers' perceptions in that column, and generate an additional column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_reader_perception'"
+            "get_spread_likelihood": "This function takes in one of the columns of readers' perceptions as input, calculates the (numerical) spread likelihood based on readers' perceptions in that column, and generate an additional column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_reader_perception' UNLESS the base table already has a column of reader perception."
         "classifier" <contains functions that classify texts>:
             "get_change_opinion": "This function takes in one of the columns as input, classifies whether the contents in that column changes opinion, and generate an additional column to include those."
             "get_sentiment": "This function takes in one of the columns as input, applies sentiment analysis on the content of that column, and generates an additional column labeling the content as 'Positive', 'Negative', and/or 'Neutral'."
             "get_condition": "This function takes in one of the columns as input, checks whether the contents of that column satisfy the user query, and generates an additional column labeling the content as 'True' or 'False' or 'Undefined'."
             "get_emotion": "This function takes in one of the columns as input, applies emotion classification on the content of that column, and generates an additional column labeling the content as 'anticipation', 'anger', 'fear', 'sadness', 'joy', 'trust', or 'disgust'"
             "get_misinfo": "This function takes in one of the columns as input, applies misinformation detection on the content of that column, and generates an additional column labeling the content as 'misinfo' (misinformation detected) or 'real' (no misinformation detected)."
             "get_hate": "This function takes in one of the columns as input, applies (high-level) hate speech detection on the content of that column, and generates an additional column labeling the content as 'implicit_hate', 'explicit_hate', or 'not_hate'."
@@ -1113,16 +1113,16 @@
                 "information_extractor" <contains functions that extract high-level messages based on actual conveyed information>:
                     "get_hate_target": "This function takes in one of the columns as input, applies implicit hate speech target identification on the content of that column, and generates an additional column of free text labeling the target identified from the content."
                     "get_hate_implied": "This function takes in one of the columns as input, applies implicit hate speech implied statement extraction on the content of that column, and generates an additional column of free text labeling the implied statement extracted from the content."
                     "get_positive_reframing": "This function takes in one of the columns as input, extract the positive aspects of the content of that column and transforms it into a positive reframing version, and generates an additional column of positive reframing version of the content."
                     "get_premise": "This function takes in one column of figurative text, one column of figurative type, and one column of figurative term as input, extracts the literal text, i.e., the premise, of the figurative text column, and generates a new column to include those."
                     "get_premise_explanation": "This function takes in one column of premise of figurative text, one column of the original figurative text, one column of figurative type, one column of figurative term as input, and one parameter labelling whether the premises entail or contract original figurative texts as input, extracts the explanations of literal texts, i.e., the premises, of the figurative text column, and generates a new column to include those."
                 "causal_extractor" <contains functions that extract the causal relationships inferred from text>:
-                    "get_reader_action": "This function takes in one of the columns of writers' intent as input, get the reader action inferred from the writers' intent of that column, and generate additional an column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_intent'"
-                    "get_reader_perception": "This function takes in one of the columns as input, infers readers' perceptions of text in that column, and generates an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_spread_likelihood'"
+                    "get_reader_action": "This function takes in one of the columns of writers' intent as input, get the reader action inferred from the writers' intent of that column, and generate additional an column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_intent' UNLESS the base table already has a column of writer's intent."
+                    "get_reader_perception": "This function takes in one of the columns as input, infers readers' perceptions of text in that column, and generates an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_spread_likelihood' UNLESS the base table already has a column of reader perception."
             }
     }
     '''
     messages = [
         {
             "role": "system",
             "content": "Given a table with columns: " + str(columns) 
@@ -1248,15 +1248,15 @@
                 },
                 "required": ["column"]
             },
             {
                 "name": "get_intent",
                 "description": 
                 ''' 
-                This function takes in one of the columns as input, retrieve the intent of the writer of text in that column, and generate an additional column to include those. Don't select this if none of the columns matches the user query. IMPORTANT: this function has to be executed at least once before calling 'get_reader_action'
+                This function takes in one of the columns as input, retrieve the intent of the writer of text in that column, and generate an additional column to include those. Don't select this if none of the columns matches the user query. IMPORTANT: this function has to be executed at least once before calling 'get_reader_action' UNLESS the base table already has a column of writer intent.
                 ''',
                 "parameters": {
                     "type": "object",
                     "properties": {"column": {
                         "type": "string",
                         "description": "the column to retrieve writers' intent from, you have to select one in the 'enum' field based on the description: "+description,
                         "enum": column_description,
@@ -1284,15 +1284,15 @@
                 },
                 "required": ["column"]
             },
             {
                 "name": "get_spread_likelihood",
                 "description": 
                 ''' 
-                This function takes in one of the columns of readers' perceptions as input, calculates the (numerical) spread likelihood based on readers' perceptions in that column, and generate an additional column to include those. Don't select this if none of the columns matches the user query. If there is no column denoting readers' perceptions, this function should not be selected. IMPORTANT: this function has to be executed after at least one call of 'get_reader_perception'
+                This function takes in one of the columns of readers' perceptions as input, calculates the (numerical) spread likelihood based on readers' perceptions in that column, and generate an additional column to include those. Don't select this if none of the columns matches the user query. If there is no column denoting readers' perceptions, this function should not be selected. IMPORTANT: this function has to be executed after at least one call of 'get_reader_perception' UNLESS the base table already has a column of reader perceptions.
                 ''',
                 "parameters": {
                     "type": "object",
                     "properties": {"column": {
                         "type": "string",
                         "description": "the column that contains readers' perceptions to calculate the spread likelihood, you have to select one in the 'enum' field based on the description: "+description,
                         "enum": column_description,
@@ -1674,15 +1674,15 @@
             },
             ],
             "causal_extractor": [
             {
                 "name": "get_reader_action",
                 "description": 
                 ''' 
-                This function takes in one of the columns of writers' intent as input, get the reader action inferred from the writers' intent of that column, and generate an additional column to include those. If there is no column denoting writers' intent, this function should not be selected. IMPORTANT: this function has to be executed after at least one call of 'get_intent'.
+                This function takes in one of the columns of writers' intent as input, get the reader action inferred from the writers' intent of that column, and generate an additional column to include those. IMPORTANT: this function has to be executed after at least one call of 'get_intent' UNLESS the base table already has a column of writer's intent.
                 ''',
                 "parameters": {
                     "type": "object",
                     "properties": {"column": {
                         "type": "string",
                         "description": "the column that contains writers' intent to infer readers' action from, you have to select one column in the 'enum' field based on the description: "+description,
                         "enum": column_description,
@@ -1692,15 +1692,15 @@
                 },
                 "required": ["column"]
             },
             {
                 "name": "get_reader_perception",
                 "description": 
                 ''' 
-                This function takes in one of the columns of text as input, infers readers' perceptions of text in that column, and generates an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_spread_likelihood'
+                This function takes in one of the columns of text as input, infers readers' perceptions of text in that column, and generates an additional column to include those. IMPORTANT: this function has to be executed at least once before calling 'get_spread_likelihood' UNLESS the base table already has a column of reader perceptions.
                 ''',
                 "parameters": {
                     "type": "object",
                     "properties": {"column": {
                         "type": "string",
                         "description": "the column that contains text to infer readers' perceptions from, you have to select one column in the 'enum' field based on the description: "+description,
                         "enum": column_description,
```

### Comparing `autopipeline-0.1.98/autopipeline/NL2SQL.py` & `autopipeline-0.1.99/autopipeline/NL2SQL.py`

 * *Files identical despite different names*

### Comparing `autopipeline-0.1.98/autopipeline/PipelineExec.py` & `autopipeline-0.1.99/autopipeline/PipelineExec.py`

 * *Files identical despite different names*

### Comparing `autopipeline-0.1.98/autopipeline/PipelineGen.py` & `autopipeline-0.1.99/autopipeline/PipelineGen.py`

 * *Files identical despite different names*

### Comparing `autopipeline-0.1.98/setup.py` & `autopipeline-0.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='autopipeline',
-    version='0.1.98',
+    version='0.1.99',
     packages=find_packages(),
     package_data={
         # Include files from the "data" directory in the "autopipeline" package
         'autopipeline': ['data/*'],
     },
     include_package_data=True,
     license='LICENSE',
```

