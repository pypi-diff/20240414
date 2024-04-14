# Comparing `tmp/notion2pandas-0.9.2-py3-none-any.whl.zip` & `tmp/notion2pandas-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8135 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      215 b- defN 24-Apr-07 22:52 notion2pandas/__init__.py
+Zip file size: 8397 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      215 b- defN 24-Apr-13 23:12 notion2pandas/__init__.py
 -rw-rw-rw-  2.0 fat    19012 b- defN 24-Apr-08 22:05 notion2pandas/notion2pandas.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6587 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      585 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/RECORD
-7 files, 27596 bytes uncompressed, 7093 bytes compressed:  74.3%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-14 21:43 notion2pandas-1.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7350 b- defN 24-Apr-14 21:43 notion2pandas-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-14 21:43 notion2pandas-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-14 21:43 notion2pandas-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      585 b- defN 24-Apr-14 21:43 notion2pandas-1.0.0.dist-info/RECORD
+7 files, 28359 bytes uncompressed, 7355 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: notion2pandas/__init__.py
 Comment: 
 
 Filename: notion2pandas/notion2pandas.py
 Comment: 
 
-Filename: notion2pandas-0.9.2.dist-info/LICENSE
+Filename: notion2pandas-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: notion2pandas-0.9.2.dist-info/METADATA
+Filename: notion2pandas-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: notion2pandas-0.9.2.dist-info/WHEEL
+Filename: notion2pandas-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: notion2pandas-0.9.2.dist-info/top_level.txt
+Filename: notion2pandas-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: notion2pandas-0.9.2.dist-info/RECORD
+Filename: notion2pandas-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## notion2pandas/__init__.py

```diff
@@ -2,9 +2,9 @@
 Package notion2pandas.
 
 Notion Client extension to import notion Database into pandas Dataframe.
 """
 
 from .notion2pandas import Notion2PandasClient
 
-__version__ = "0.9.2"
+__version__ = "1.0.0"
 __author__ = 'Andrea Rosati'
```

## Comparing `notion2pandas-0.9.2.dist-info/LICENSE` & `notion2pandas-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `notion2pandas-0.9.2.dist-info/METADATA` & `notion2pandas-1.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: notion2pandas
-Version: 0.9.2
+Version: 1.0.0
 Summary: Notion Client extension to import notion Database into pandas Dataframe
 Home-page: https://gitlab.com/Jaeger87/notion2pandas
 Author: Andrea Rosati
 Author-email: rosati.1595834@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: notion-client
 Requires-Dist: pandas
 
 # Notion2Pandas
 <p align="center">
@@ -36,29 +38,41 @@
 
 ## Usage
 
 <p align="center">
 <img src="https://gitlab.com/Jaeger87/notion2pandas/-/raw/main/readme_assets/notiondb2pandas.gif?ref_type=heads"  class="center">
 </p> <p align="left">
 
-* As shown in the gif, you just need to import the Notion2PandasClient class, 
+* As shown in the gif, you just need to import the Notion2PandasClient class. 
 ```python
 from notion2pandas import Notion2PandasClient
 ```
-* create an instance by passing your authentication token 
+* Create an instance by passing your authentication token. 
 ```python
 n2p = Notion2PandasClient(auth=os.environ["NOTION_TOKEN"])
 ```
-* use the 'from_notion_DB_to_dataframe' method to get the data into a dataframe. 
+* Use the 'from_notion_DB_to_dataframe' method to get the data into a dataframe. 
 ```python
-n2p.update_notion_DB_from_dataframe(os.environ["DATABASE_ID"], df)
+df = n2p.from_notion_DB_to_dataframe(os.environ["DATABASE_ID"])
 ```
 * When you're done working with your dataframe, use the 'update_notion_DB_from_dataframe' method to save the data back to Notion.
 ```python
-n2p.update_notion_DB_from_dataframe(databaseID, df)
+n2p.update_notion_DB_from_dataframe(os.environ["DATABASE_ID"], df)
+```
+* If you need a queried or sorted database, you can create your filter / sort object [with this structure](https://developers.notion.com/reference/post-database-query) and pass it to the from_notion_DB_to_dataframe method:
+
+```python
+published_filter = {"filter": {
+            "property": "Published",
+            "checkbox": {
+                "equals": True
+            }
+        }}
+
+df = n2p.from_notion_DB_to_dataframe(os.environ["DATABASE_ID"], published_filter)
 ```
 
 ## PageID and Row_Hash
 
 As you can see, in the pandas dataframe there are two additional columns compared to those in the original database, PageID and Row_Hash. As you can imagine, PageID it's the ID related to the page of that entry in Notion. Row_Hash is a value calculated based on the fields' values of the entry, this value is used by the update_notion_DB_from_dataframe function to determine if a row in the dataframe has been modified, and if not, it avoids making the API call to Notion for that row. Any change to those functions can lead to malfunctions, so please do not change them!
 
 ## Utility functions
@@ -119,12 +133,18 @@
 Last edited by | last_edited_by_read_write_lambdas
 Last edited time | last_edited_time_read_write_lambdas
 
 ## Adding and removes rows
 
 If you add a row to the dataframe and then update the Notion database from it, Notion2Pandas is capable of adding the new row to the database. On the contrary, if a row is removed, Notion2Pandas will not automatically delete the row during the update. In this case, you need to use the delete_page method manually.
 
+# Roadmap
+For the upcoming releases, I plan to release:
+
+* Managing the limit of 2700 API calls in 15 minutes
+* Asynchronous client version of notion2pandas
+
 # Support
 Notion2Pandas is an open-source project; anyone can contribute to the project by reporting issues or proposing merge requests. I will commit to evaluating every proposal and responding to all. If you disagree with the decisions made and the direction the project may take, you are free to fork the project, and you will have my blessing!
```

