# Comparing `tmp/texttoolspy-0.0.7-py3-none-any.whl.zip` & `tmp/texttoolspy-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3569 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     2141 b- defN 24-Apr-12 20:39 texttoolspy/__init__.py
+Zip file size: 3596 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     2205 b- defN 24-Apr-14 19:34 texttoolspy/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-08 20:02 texttoolspy/main.py
--rw-rw-rw-  2.0 fat     1083 b- defN 24-Apr-12 20:46 texttoolspy-0.0.7.dist-info/Licence.txt
--rw-rw-rw-  2.0 fat     1323 b- defN 24-Apr-12 20:46 texttoolspy-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-12 20:46 texttoolspy-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-12 20:46 texttoolspy-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      563 b- defN 24-Apr-12 20:46 texttoolspy-0.0.7.dist-info/RECORD
-7 files, 5214 bytes uncompressed, 2565 bytes compressed:  50.8%
+-rw-rw-rw-  2.0 fat     1083 b- defN 24-Apr-14 19:39 texttoolspy-1.0.0.dist-info/Licence.txt
+-rw-rw-rw-  2.0 fat     1323 b- defN 24-Apr-14 19:39 texttoolspy-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-14 19:39 texttoolspy-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-14 19:39 texttoolspy-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      563 b- defN 24-Apr-14 19:39 texttoolspy-1.0.0.dist-info/RECORD
+7 files, 5278 bytes uncompressed, 2592 bytes compressed:  50.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: texttoolspy/__init__.py
 Comment: 
 
 Filename: texttoolspy/main.py
 Comment: 
 
-Filename: texttoolspy-0.0.7.dist-info/Licence.txt
+Filename: texttoolspy-1.0.0.dist-info/Licence.txt
 Comment: 
 
-Filename: texttoolspy-0.0.7.dist-info/METADATA
+Filename: texttoolspy-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: texttoolspy-0.0.7.dist-info/WHEEL
+Filename: texttoolspy-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: texttoolspy-0.0.7.dist-info/top_level.txt
+Filename: texttoolspy-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: texttoolspy-0.0.7.dist-info/RECORD
+Filename: texttoolspy-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## texttoolspy/__init__.py

```diff
@@ -40,29 +40,31 @@
       print(colored("'"+color.lower()+"'" + " is not a registerd color. Please see the github documentation for the full list of registerd colors","red"))
     elif "missing" in str(e):
       print(str(e) + "-> No string was given.")
   cursor.show()
 def LineBreak(lines):
   for x in range(0,lines):
     print("  ")
-def menu(menu_items,menu_type):
+def menu(menu_items,menu_type, header="",footer=""):
   selected_menu = 1
   answer = ""
   while answer != key.ENTER:
     os.system("cls")
+    print(header+"\n")
     for x in range(0,len(menu_items)):
       if selected_menu == x+1:
         if str(menu_type)=="1":
           print(f"> {italic}{menu_items[x]} \n")
         elif str(menu_type)=="2":
           print(colored(f"{bold}{menu_items[x]} \n","black","on_white"))
         elif str(menu_type) == "3":
           print(colored(f"{menu_items[x]} \n","red"))
       else:
         print(menu_items[x] + "\n")
+    print(footer)
     sleep(0.1)
     answer = readkey()
     if answer == key.DOWN and selected_menu < len(menu_items):
       selected_menu += 1
     elif answer == key.UP and selected_menu > 1:
       selected_menu -= 1
```

## Comparing `texttoolspy-0.0.7.dist-info/Licence.txt` & `texttoolspy-1.0.0.dist-info/Licence.txt`

 * *Files identical despite different names*

## Comparing `texttoolspy-0.0.7.dist-info/METADATA` & `texttoolspy-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: texttoolspy
-Version: 0.0.7
+Version: 1.0.0
 Summary: A tool that allows you to create responsive tools in text
 Author: MilesWK
 Author-email: your_name@example.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `texttoolspy-0.0.7.dist-info/RECORD` & `texttoolspy-1.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-texttoolspy/__init__.py,sha256=CJSM9NheOiXZQNVS9bUSUJsuyfv4yf9M9iSpx7JSJMg,2141
+texttoolspy/__init__.py,sha256=6rHrFs1Ol5EE_y4r_A670tZHWn3uUQxUOD6n2TgNAbA,2205
 texttoolspy/main.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-texttoolspy-0.0.7.dist-info/Licence.txt,sha256=xmmaISdPorZT-rPBZ0F43fqfVLcQxkrldRFyJJNQW9I,1083
-texttoolspy-0.0.7.dist-info/METADATA,sha256=_RpV1hB_jeWASnc9pKQ3kIYPf3h3jpwn1lEAg22HqoE,1323
-texttoolspy-0.0.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-texttoolspy-0.0.7.dist-info/top_level.txt,sha256=pPT7_1Oiuya1rnSvm9vrpptDLGsFrvmVBm96CS7_fxM,12
-texttoolspy-0.0.7.dist-info/RECORD,,
+texttoolspy-1.0.0.dist-info/Licence.txt,sha256=xmmaISdPorZT-rPBZ0F43fqfVLcQxkrldRFyJJNQW9I,1083
+texttoolspy-1.0.0.dist-info/METADATA,sha256=4cJM1tU0OAvvCo44IKUhstbPf_URLhnueFFP1-jeAc0,1323
+texttoolspy-1.0.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+texttoolspy-1.0.0.dist-info/top_level.txt,sha256=pPT7_1Oiuya1rnSvm9vrpptDLGsFrvmVBm96CS7_fxM,12
+texttoolspy-1.0.0.dist-info/RECORD,,
```

