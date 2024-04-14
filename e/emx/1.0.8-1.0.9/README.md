# Comparing `tmp/emx-1.0.8-py3-none-any.whl.zip` & `tmp/emx-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7650 bytes, number of entries: 8
+Zip file size: 7654 bytes, number of entries: 8
 -rw-r--r--  2.0 unx    20399 b- defN 24-Apr-14 05:20 emx/__init__.py
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-10 11:34 emx/__main__.py
--rw-r--r--  2.0 unx     2785 b- defN 24-Apr-14 06:48 emx/http.py
--rw-r--r--  2.0 unx      310 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/RECORD
-8 files, 24479 bytes uncompressed, 6642 bytes compressed:  72.9%
+-rw-r--r--  2.0 unx     2786 b- defN 24-Apr-14 06:58 emx/http.py
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-14 06:58 emx-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-14 06:58 emx-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-14 06:58 emx-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-14 06:58 emx-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-14 06:58 emx-1.0.9.dist-info/RECORD
+8 files, 24480 bytes uncompressed, 6646 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: emx/__main__.py
 Comment: 
 
 Filename: emx/http.py
 Comment: 
 
-Filename: emx-1.0.8.dist-info/METADATA
+Filename: emx-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: emx-1.0.8.dist-info/WHEEL
+Filename: emx-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: emx-1.0.8.dist-info/entry_points.txt
+Filename: emx-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: emx-1.0.8.dist-info/top_level.txt
+Filename: emx-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: emx-1.0.8.dist-info/RECORD
+Filename: emx-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## emx/http.py

```diff
@@ -42,15 +42,15 @@
             yield chunk
 
         progress.close()
 
     try:
         response = requests.post(url, data=gen_stream_file(), headers=headers)
     except requests.exceptions.ConnectionError as e:
-        print(f"Upload failed, maybe a invalid file posted.")
+        print("By default, the max upload file size is: 5 MB")
         return None
 
     content_string = str(response.content, encoding="utf-8")
     try:
         data = json.loads(content_string)
     except json.decoder.JSONDecodeError as e:
         print(f"Upload failed, {content_string}")
```

## Comparing `emx-1.0.8.dist-info/RECORD` & `emx-1.0.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 emx/__init__.py,sha256=BaISPjucGmd2TVc21G-wekx_uDEb-UxQ-3vAxQZmh5o,20399
 emx/__main__.py,sha256=vZwS8IKVqP_M9MaJM8AsdM93XvflohMpoLrnXYcqnpk,239
-emx/http.py,sha256=U2AnxRmUOwXYjKUOJsae_8MESDqqyn4Jg4rUufX_kPY,2785
-emx-1.0.8.dist-info/METADATA,sha256=QS8rEepiMSG2JUawdB3TGnlw_g1VdVDl5U8MvhAtHQI,310
-emx-1.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-emx-1.0.8.dist-info/entry_points.txt,sha256=Q4bfdmdN4hpNqKvXURVbkF8Q6KP0P9jykoccDI4GcI0,67
-emx-1.0.8.dist-info/top_level.txt,sha256=mAJdYxkuyZt_oZrtIM2mSBM2LadTIoXeo75v_-v-h5A,4
-emx-1.0.8.dist-info/RECORD,,
+emx/http.py,sha256=ldK1k9ck9aPfIvBo_bGSNKsnU1cLDSxYToywjeZa-9E,2786
+emx-1.0.9.dist-info/METADATA,sha256=lXpZMvRoF3eIe6bvOS0tLJsWIoZTt6G0rN5DR4w6gpA,310
+emx-1.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+emx-1.0.9.dist-info/entry_points.txt,sha256=Q4bfdmdN4hpNqKvXURVbkF8Q6KP0P9jykoccDI4GcI0,67
+emx-1.0.9.dist-info/top_level.txt,sha256=mAJdYxkuyZt_oZrtIM2mSBM2LadTIoXeo75v_-v-h5A,4
+emx-1.0.9.dist-info/RECORD,,
```

