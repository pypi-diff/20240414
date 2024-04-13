# Comparing `tmp/jb_news-2.1.0-py3-none-any.whl.zip` & `tmp/jb_news-2.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2035 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2739 b- defN 24-Apr-03 23:45 jb_news-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 23:45 jb_news-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 23:45 jb_news-2.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      297 b- defN 24-Apr-03 23:45 jb_news-2.1.0.dist-info/RECORD
-4 files, 3129 bytes uncompressed, 1453 bytes compressed:  53.6%
+Zip file size: 2072 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2796 b- defN 24-Apr-13 22:47 jb_news-2.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 22:47 jb_news-2.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-13 22:47 jb_news-2.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      297 b- defN 24-Apr-13 22:47 jb_news-2.1.1.dist-info/RECORD
+4 files, 3186 bytes uncompressed, 1490 bytes compressed:  53.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: jb_news-2.1.0.dist-info/METADATA
+Filename: jb_news-2.1.1.dist-info/METADATA
 Comment: 
 
-Filename: jb_news-2.1.0.dist-info/WHEEL
+Filename: jb_news-2.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: jb_news-2.1.0.dist-info/top_level.txt
+Filename: jb_news-2.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jb_news-2.1.0.dist-info/RECORD
+Filename: jb_news-2.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `jb_news-2.1.0.dist-info/METADATA` & `jb_news-2.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jb-news
-Version: 2.1.0
+Version: 2.1.1
 Summary: A comprehensive wrapper for JBlanked's News API, leveraging OpenAI, Machine Learning, and MQL5's Calendar.
 Home-page: https://jblanked.com/news/api/docs/
 Author: JBlanked
 License: MIT
 Description-Content-Type: text/markdown
 
 # JB-News
@@ -37,15 +37,18 @@
 ```
 A list of Event IDs are found on https://www.jblanked.com/news/api/docs/.
 
 Next, set your API key and Event ID:
 
 ```python
 api_key = "YOUR_API_KEY_HERE" 
+
 event_id = 756020001 # CHF CPI
+
+jb.offset = 7  # GMT-3 = 0, GMT = 3, EST = 7, PST = 10
 ```
 
 Next step is to connect to the API by using the get method. 
 ```python
 if jb.get(api_key):  
 ```
```

