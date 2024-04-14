# Comparing `tmp/ranshark-1.0.0.8-py3-none-any.whl.zip` & `tmp/ranshark-1.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 55288 bytes, number of entries: 40
+Zip file size: 55251 bytes, number of entries: 40
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-13 18:52 drawranflow/__init__.py
 -rw-r--r--  2.0 unx       66 b- defN 23-Dec-13 18:52 drawranflow/admin.py
 -rw-r--r--  2.0 unx      160 b- defN 23-Dec-13 18:52 drawranflow/apps.py
 -rw-r--r--  2.0 unx     5545 b- defN 23-Dec-13 18:52 drawranflow/models.py
 -rw-r--r--  2.0 unx       63 b- defN 23-Dec-13 18:52 drawranflow/tests.py
 -rw-r--r--  2.0 unx     1660 b- defN 23-Dec-13 18:52 drawranflow/urls.py
 -rw-r--r--  2.0 unx    18101 b- defN 23-Dec-13 18:52 drawranflow/views.py
@@ -31,12 +31,12 @@
 -rw-r--r--  2.0 unx    14496 b- defN 23-Dec-13 18:52 drawranflow/templates/draw_sequence.html
 -rw-r--r--  2.0 unx    10775 b- defN 23-Dec-13 18:52 drawranflow/templates/home.html
 -rw-r--r--  2.0 unx    15224 b- defN 23-Dec-13 18:52 drawranflow/templates/show_stats.html
 -rw-r--r--  2.0 unx     9041 b- defN 23-Dec-01 02:12 drawranflow/templates/show_stats_Nov27.html
 -rw-r--r--  2.0 unx     6528 b- defN 23-Dec-13 18:52 drawranflow/templates/show_stats_bkup.html
 -rw-r--r--  2.0 unx     2577 b- defN 23-Dec-13 18:52 drawranflow/templates/streaming_table.html
 -rw-r--r--  2.0 unx     6528 b- defN 23-Dec-13 18:52 drawranflow/templates/streaming_table_bkup.html
--rw-r--r--  2.0 unx     1595 b- defN 23-Dec-13 23:30 ranshark-1.0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-13 23:30 ranshark-1.0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Dec-13 23:30 ranshark-1.0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3812 b- defN 23-Dec-13 23:30 ranshark-1.0.0.8.dist-info/RECORD
-40 files, 219295 bytes uncompressed, 49032 bytes compressed:  77.6%
+-rw-r--r--  2.0 unx     1548 b- defN 23-Dec-14 16:12 ranshark-1.0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Dec-14 16:12 ranshark-1.0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Dec-14 16:12 ranshark-1.0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3812 b- defN 23-Dec-14 16:12 ranshark-1.0.0.9.dist-info/RECORD
+40 files, 219248 bytes uncompressed, 48995 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -102,20 +102,20 @@
 
 Filename: drawranflow/templates/streaming_table.html
 Comment: 
 
 Filename: drawranflow/templates/streaming_table_bkup.html
 Comment: 
 
-Filename: ranshark-1.0.0.8.dist-info/METADATA
+Filename: ranshark-1.0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: ranshark-1.0.0.8.dist-info/WHEEL
+Filename: ranshark-1.0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: ranshark-1.0.0.8.dist-info/top_level.txt
+Filename: ranshark-1.0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ranshark-1.0.0.8.dist-info/RECORD
+Filename: ranshark-1.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ranshark-1.0.0.8.dist-info/METADATA` & `ranshark-1.0.0.9.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: ranshark
-Version: 1.0.0.8
+Version: 1.0.0.9
 Summary: A friendly 5g o-ran packet analyzing tool with GUI interface.
 Home-page: UNKNOWN
 Author: ugandhar
 Author-email: ugandhar.nellore@gmail.com
 License: Apache-2.0
 Keywords: ran,5g,5g analyzer,ranshark
 Platform: UNKNOWN
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Requires-Dist: Django ~=4.2.7
-Requires-Dist: celery ~=5.3.4
-Requires-Dist: pandas ~=1.3.3
-Requires-Dist: pyshark ~=0.6
-Requires-Dist: psycopg2 ==2.9.9
-Requires-Dist: psycopg2-binary ==2.9.9
+Requires-Dist: Django
+Requires-Dist: pandas
+Requires-Dist: pyshark
+Requires-Dist: psycopg2
+Requires-Dist: psycopg2-binary
+Requires-Dist: numpy
 
 # ranshark
 ===========
 <p>This is the Python project that read 5g RAN packets using pyshark lib (a Tshark wrapper) and filter flows based below identities.</p>
 <ul>
 <li>C_RNTI</li>
 <li>F1AP ID's</li>
```

## Comparing `ranshark-1.0.0.8.dist-info/RECORD` & `ranshark-1.0.0.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 drawranflow/templates/draw_sequence.html,sha256=tYQC5B5LVutygMyiTLVRBXOaOluiEdA6MNlkU6oCTrI,14496
 drawranflow/templates/home.html,sha256=zZPFBlSEZDWfaIrgbaXwpMogR7Ze5GlS1CujXmVXznI,10775
 drawranflow/templates/show_stats.html,sha256=yWiDUFjMYnEfxe1Z03v4Q07clpKnd-OsL4xRoYpkmA4,15224
 drawranflow/templates/show_stats_Nov27.html,sha256=Up48FAFzPdVQBq3sI6SCCf4AVAsheHE99Nv8JpSRpms,9041
 drawranflow/templates/show_stats_bkup.html,sha256=7ZSQleV3pzhvCdjTOYWHWvnVie3mCvRit9LlXlD670o,6528
 drawranflow/templates/streaming_table.html,sha256=GYBi_oawkUtKweL1WScz-lAt5VyEwyaycJKRyUb6afQ,2577
 drawranflow/templates/streaming_table_bkup.html,sha256=7ZSQleV3pzhvCdjTOYWHWvnVie3mCvRit9LlXlD670o,6528
-ranshark-1.0.0.8.dist-info/METADATA,sha256=NYhSGx0VVrw54aDpO_dTe-rse7A5VRLlRxqMl53si0A,1595
-ranshark-1.0.0.8.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-ranshark-1.0.0.8.dist-info/top_level.txt,sha256=eKM6_mVgII-MHLpC8dkY8phUqge44EJi-RPAEui9ssk,12
-ranshark-1.0.0.8.dist-info/RECORD,,
+ranshark-1.0.0.9.dist-info/METADATA,sha256=4uPZwVrrgy_XVLmMEDENziBw3JvmKwicxaVomEkYp20,1548
+ranshark-1.0.0.9.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+ranshark-1.0.0.9.dist-info/top_level.txt,sha256=eKM6_mVgII-MHLpC8dkY8phUqge44EJi-RPAEui9ssk,12
+ranshark-1.0.0.9.dist-info/RECORD,,
```

