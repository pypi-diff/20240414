# Comparing `tmp/emx-1.0.7-py3-none-any.whl.zip` & `tmp/emx-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7585 bytes, number of entries: 8
--rw-r--r--  2.0 unx    20387 b- defN 24-Apr-12 16:25 emx/__init__.py
+Zip file size: 7650 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    20399 b- defN 24-Apr-14 05:20 emx/__init__.py
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-10 11:34 emx/__main__.py
--rw-r--r--  2.0 unx     2470 b- defN 24-Apr-12 16:28 emx/http.py
--rw-r--r--  2.0 unx      310 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      583 b- defN 24-Apr-13 01:00 emx-1.0.7.dist-info/RECORD
-8 files, 24152 bytes uncompressed, 6577 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx     2785 b- defN 24-Apr-14 06:48 emx/http.py
+-rw-r--r--  2.0 unx      310 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      583 b- defN 24-Apr-14 06:53 emx-1.0.8.dist-info/RECORD
+8 files, 24479 bytes uncompressed, 6642 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: emx/__main__.py
 Comment: 
 
 Filename: emx/http.py
 Comment: 
 
-Filename: emx-1.0.7.dist-info/METADATA
+Filename: emx-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: emx-1.0.7.dist-info/WHEEL
+Filename: emx-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: emx-1.0.7.dist-info/entry_points.txt
+Filename: emx-1.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: emx-1.0.7.dist-info/top_level.txt
+Filename: emx-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: emx-1.0.7.dist-info/RECORD
+Filename: emx-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## emx/__init__.py

```diff
@@ -459,17 +459,17 @@
                     raw_size += os.path.getsize(file)
                     zf.write(file, name)
 
                 zf.close()
                 new_size = fp.tell()
                 print(f"raw_size = {format_size(raw_size)}, compress_size = {format_size(new_size)}, compress ratio: {abs(1 - new_size / raw_size) * 100:.2f} %")
 
-                if new_size >= 5 * 1024 * 1024:
-                    print(f"Over of limit for uploaded file size: {new_size / 1024 / 1024:.3f} MB, maximum = 5MB")
-                    return
+                # if new_size >= 5 * 1024 * 1024:
+                #     print(f"Over of limit for uploaded file size: {new_size / 1024 / 1024:.3f} MB, maximum = 5MB")
+                #     return
 
                 headers = {
                     "save": remote,
                     "file_size": str(new_size),
                     "raw_size": str(raw_size),
                     "descript": desc,
                     "is_directory": str(isdir),
@@ -479,17 +479,17 @@
                     "user_name": self.cfg.get_cfg("UserName"),
                     "user_token": self.cfg.get_cfg("UserToken")
                 }
                 fp.seek(0)
                 resp = http.upload_file(f"{self.cfg.SERVER}/upload", fp, headers, f"Upload: {remote}")
         else:
             size = os.path.getsize(local)
-            if size >= 5 * 1024 * 1024:
-                print(f"Over of limit for uploaded file size: {size / 1024 / 1024:.3f} MB, maximum = 5MB")
-                return
+            # if size >= 5 * 1024 * 1024:
+            #     print(f"Over of limit for uploaded file size: {size / 1024 / 1024:.3f} MB, maximum = 5MB")
+            #     return
 
             headers = {
                 "save": remote,
                 "file_size": str(size),
                 "raw_size": str(size),
                 "descript": desc,
                 "is_directory": str(isdir),
```

## emx/http.py

```diff
@@ -39,16 +39,27 @@
             if len(chunk) == 0:
                 break
             
             yield chunk
 
         progress.close()
 
-    response = requests.post(url, data=gen_stream_file(), headers=headers)
-    data = json.loads(str(response.content, encoding="utf-8"))
+    try:
+        response = requests.post(url, data=gen_stream_file(), headers=headers)
+    except requests.exceptions.ConnectionError as e:
+        print(f"Upload failed, maybe a invalid file posted.")
+        return None
+
+    content_string = str(response.content, encoding="utf-8")
+    try:
+        data = json.loads(content_string)
+    except json.decoder.JSONDecodeError as e:
+        print(f"Upload failed, {content_string}")
+        return None
+
     if response.status_code != 200:
         msg = data["detail"]
         print(f"Upload failed, {msg}")
         return None
     
     return data
```

## Comparing `emx-1.0.7.dist-info/RECORD` & `emx-1.0.8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-emx/__init__.py,sha256=6Rrzm8I7zNxLqtjXOHKbcNrP2YHJ2C2X1W9o515gZ-0,20387
+emx/__init__.py,sha256=BaISPjucGmd2TVc21G-wekx_uDEb-UxQ-3vAxQZmh5o,20399
 emx/__main__.py,sha256=vZwS8IKVqP_M9MaJM8AsdM93XvflohMpoLrnXYcqnpk,239
-emx/http.py,sha256=cf_i9KofEN0pduRFcyvjJzNAGCYcVMA0lVfv-joNS7M,2470
-emx-1.0.7.dist-info/METADATA,sha256=YTEDcnD1iUvugWiUhW8llXEuoObMM1qk5g_UpoeI0Xg,310
-emx-1.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-emx-1.0.7.dist-info/entry_points.txt,sha256=Q4bfdmdN4hpNqKvXURVbkF8Q6KP0P9jykoccDI4GcI0,67
-emx-1.0.7.dist-info/top_level.txt,sha256=mAJdYxkuyZt_oZrtIM2mSBM2LadTIoXeo75v_-v-h5A,4
-emx-1.0.7.dist-info/RECORD,,
+emx/http.py,sha256=U2AnxRmUOwXYjKUOJsae_8MESDqqyn4Jg4rUufX_kPY,2785
+emx-1.0.8.dist-info/METADATA,sha256=QS8rEepiMSG2JUawdB3TGnlw_g1VdVDl5U8MvhAtHQI,310
+emx-1.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+emx-1.0.8.dist-info/entry_points.txt,sha256=Q4bfdmdN4hpNqKvXURVbkF8Q6KP0P9jykoccDI4GcI0,67
+emx-1.0.8.dist-info/top_level.txt,sha256=mAJdYxkuyZt_oZrtIM2mSBM2LadTIoXeo75v_-v-h5A,4
+emx-1.0.8.dist-info/RECORD,,
```

