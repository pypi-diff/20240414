# Comparing `tmp/muko-2.18-py3-none-any.whl.zip` & `tmp/muko-2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1630434 bytes, number of entries: 9
+Zip file size: 1630097 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
--rw-rw-rw-  2.0 fat   466944 b- defN 24-Apr-11 18:46 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   466432 b- defN 24-Apr-14 16:29 muko/cmuko.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-11 18:46 muko-2.18.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1181 b- defN 24-Apr-11 18:46 muko-2.18.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 18:46 muko-2.18.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-11 18:46 muko-2.18.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-11 18:46 muko-2.18.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      696 b- defN 24-Apr-11 18:46 muko-2.18.dist-info/RECORD
-9 files, 2552996 bytes uncompressed, 1629246 bytes compressed:  36.2%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-14 16:29 muko-2.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1180 b- defN 24-Apr-14 16:29 muko-2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-14 16:29 muko-2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 24-Apr-14 16:29 muko-2.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-14 16:29 muko-2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      690 b- defN 24-Apr-14 16:29 muko-2.2.dist-info/RECORD
+9 files, 2552477 bytes uncompressed, 1628921 bytes compressed:  36.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: muko/cmuko.cp38-win_amd64.pyd
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.18.dist-info/LICENSE
+Filename: muko-2.2.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.18.dist-info/METADATA
+Filename: muko-2.2.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.18.dist-info/WHEEL
+Filename: muko-2.2.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.18.dist-info/entry_points.txt
+Filename: muko-2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: muko-2.18.dist-info/top_level.txt
+Filename: muko-2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: muko-2.18.dist-info/RECORD
+Filename: muko-2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.18.dist-info/LICENSE` & `muko-2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.18.dist-info/METADATA` & `muko-2.2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 2.18
+Version: 2.2
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 Author: Milk
 Author-email: 719496375@qq.com
 License: The MIT License
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `muko-2.18.dist-info/RECORD` & `muko-2.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 muko/__init__.py,sha256=CCRGa1csLmHKI_CslhtoPnqhEJA3mszIsRjACQuz5iE,20
-muko/cmuko.cp38-win_amd64.pyd,sha256=bwhGlLHU13sMEqxyRoQ6w5pQDJ_Mb1aaDumyZvrme8c,466944
+muko/cmuko.cp38-win_amd64.pyd,sha256=TpdhsAEIkA2HdJaxs2e7xhzLevfkEyVxRXZF36upmH0,466432
 muko/font/default.otf,sha256=ZMqD7VMsbmTwwTRN4d72gVQLIekvjl5SSCvxs8-O4GA,2082964
-muko-2.18.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
-muko-2.18.dist-info/METADATA,sha256=Sb87RaOfyvl4dIJ25PC6jxewacbA3ZIAC3YJr1sHhjY,1181
-muko-2.18.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-muko-2.18.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
-muko-2.18.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
-muko-2.18.dist-info/RECORD,,
+muko-2.2.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
+muko-2.2.dist-info/METADATA,sha256=D5Ox1rq4Jp6DaudllwXOkyf2M624FFvkpk3uPawZwRo,1180
+muko-2.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+muko-2.2.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
+muko-2.2.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
+muko-2.2.dist-info/RECORD,,
```

