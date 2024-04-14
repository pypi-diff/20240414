# Comparing `tmp/mystring-0.2.98-py3-none-any.whl.zip` & `tmp/mystring-0.2.99-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17860 bytes, number of entries: 7
--rw-r--r--  2.0 unx    51733 b- defN 24-Mar-17 00:35 mystring/__init__.py
--rw-r--r--  2.0 unx     2550 b- defN 24-Mar-17 00:35 mystring/py2nb.py
--rw-r--r--  2.0 unx     1074 b- defN 24-Mar-17 00:35 mystring-0.2.98.dist-info/LICENSE
--rw-r--r--  2.0 unx     1568 b- defN 24-Mar-17 00:35 mystring-0.2.98.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-17 00:35 mystring-0.2.98.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-17 00:35 mystring-0.2.98.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      547 b- defN 24-Mar-17 00:35 mystring-0.2.98.dist-info/RECORD
-7 files, 57573 bytes uncompressed, 16894 bytes compressed:  70.7%
+Zip file size: 17861 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    51754 b- defN 24-Mar-17 00:41 mystring/__init__.py
+-rw-r--r--  2.0 unx     2550 b- defN 24-Mar-17 00:41 mystring/py2nb.py
+-rw-r--r--  2.0 unx     1074 b- defN 24-Mar-17 00:41 mystring-0.2.99.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1568 b- defN 24-Mar-17 00:41 mystring-0.2.99.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-17 00:41 mystring-0.2.99.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Mar-17 00:41 mystring-0.2.99.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      547 b- defN 24-Mar-17 00:41 mystring-0.2.99.dist-info/RECORD
+7 files, 57594 bytes uncompressed, 16895 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: mystring/__init__.py
 Comment: 
 
 Filename: mystring/py2nb.py
 Comment: 
 
-Filename: mystring-0.2.98.dist-info/LICENSE
+Filename: mystring-0.2.99.dist-info/LICENSE
 Comment: 
 
-Filename: mystring-0.2.98.dist-info/METADATA
+Filename: mystring-0.2.99.dist-info/METADATA
 Comment: 
 
-Filename: mystring-0.2.98.dist-info/WHEEL
+Filename: mystring-0.2.99.dist-info/WHEEL
 Comment: 
 
-Filename: mystring-0.2.98.dist-info/top_level.txt
+Filename: mystring-0.2.99.dist-info/top_level.txt
 Comment: 
 
-Filename: mystring-0.2.98.dist-info/RECORD
+Filename: mystring-0.2.99.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mystring/__init__.py

```diff
@@ -1047,15 +1047,15 @@
 			frame_to_add = None
 			if isinstance(obj, frame):
 				frame_to_add = dc(obj)
 			elif isinstance(obj, pd.DataFrame):
 				frame_to_add = frame(obj)
 			elif isinstance(obj, str):
 				try:
-					output = frame.of(obj)
+					output = frame.of(obj, sheet_name=obj_name)
 					if output is not None:
 						frame_to_add = output
 				except:pass
 
 			if frame_to_add is not None:
 				self.dyct[obj_name or self.__nu_name()] = frame_to_add
```

## Comparing `mystring-0.2.98.dist-info/LICENSE` & `mystring-0.2.99.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mystring-0.2.98.dist-info/METADATA` & `mystring-0.2.99.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystring
-Version: 0.2.98
+Version: 0.2.99
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/mystring
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `mystring-0.2.98.dist-info/RECORD` & `mystring-0.2.99.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-mystring/__init__.py,sha256=CCiKkwBTTrBDYdanSkS4FX_8Msglm_LK5bK4fYzqIqg,51733
+mystring/__init__.py,sha256=8Hl9TkIbhzqoikn1kj5rMTrtxMxYNlkCyGH32ljpm-o,51754
 mystring/py2nb.py,sha256=3Q-8n8_9dxxwUIFzVvOJkoZGxzpJa3kMc8JJ0LhdqZ4,2550
-mystring-0.2.98.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-mystring-0.2.98.dist-info/METADATA,sha256=yg2mUwts9Gs_t210O7DYML_K9mJney7BDWESSZswWrY,1568
-mystring-0.2.98.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mystring-0.2.98.dist-info/top_level.txt,sha256=yRHZrLaa94CvAXZsscYoQvSfaSwJfqGmC_UU7eKKf1I,9
-mystring-0.2.98.dist-info/RECORD,,
+mystring-0.2.99.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+mystring-0.2.99.dist-info/METADATA,sha256=beF27f5KbwU41D91nPTo1JR0doBA9TcAQTEl9epu3wk,1568
+mystring-0.2.99.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mystring-0.2.99.dist-info/top_level.txt,sha256=yRHZrLaa94CvAXZsscYoQvSfaSwJfqGmC_UU7eKKf1I,9
+mystring-0.2.99.dist-info/RECORD,,
```

