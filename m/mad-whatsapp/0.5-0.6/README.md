# Comparing `tmp/mad_whatsapp-0.5.tar.gz` & `tmp/mad_whatsapp-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mad_whatsapp-0.5.tar", last modified: Wed Oct 18 13:10:22 2023, max compression
+gzip compressed data, was "mad_whatsapp-0.6.tar", last modified: Sun Apr 14 09:57:37 2024, max compression
```

## Comparing `mad_whatsapp-0.5.tar` & `mad_whatsapp-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dobrescu  (1000) dobrescu  (1000)        0 2023-10-18 13:10:22.746806 mad_whatsapp-0.5/
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)     1075 2023-09-18 13:22:22.000000 mad_whatsapp-0.5/LICENSE
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)       18 2023-09-18 13:31:07.000000 mad_whatsapp-0.5/MANIFEST.in
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      841 2023-10-18 13:10:22.746806 mad_whatsapp-0.5/PKG-INFO
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      326 2023-10-17 09:42:47.000000 mad_whatsapp-0.5/README.md
-drwxr-xr-x   0 dobrescu  (1000) dobrescu  (1000)        0 2023-10-18 13:10:22.746806 mad_whatsapp-0.5/mad_whatsapp/
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)       81 2023-09-18 15:07:25.000000 mad_whatsapp-0.5/mad_whatsapp/__init__.py
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)     2802 2023-10-18 10:23:52.000000 mad_whatsapp-0.5/mad_whatsapp/wap.py
-drwxr-xr-x   0 dobrescu  (1000) dobrescu  (1000)        0 2023-10-18 13:10:22.746806 mad_whatsapp-0.5/mad_whatsapp.egg-info/
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      841 2023-10-18 13:10:22.000000 mad_whatsapp-0.5/mad_whatsapp.egg-info/PKG-INFO
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      227 2023-10-18 13:10:22.000000 mad_whatsapp-0.5/mad_whatsapp.egg-info/SOURCES.txt
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)        1 2023-10-18 13:10:22.000000 mad_whatsapp-0.5/mad_whatsapp.egg-info/dependency_links.txt
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)       13 2023-10-18 13:10:22.000000 mad_whatsapp-0.5/mad_whatsapp.egg-info/top_level.txt
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)       38 2023-10-18 13:10:22.746806 mad_whatsapp-0.5/setup.cfg
--rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      961 2023-10-18 13:10:07.000000 mad_whatsapp-0.5/setup.py
+drwxr-xr-x   0 dobrescu  (1000) dobrescu  (1000)        0 2024-04-14 09:57:37.608199 mad_whatsapp-0.6/
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)     1075 2023-09-18 13:22:22.000000 mad_whatsapp-0.6/LICENSE
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)       18 2023-09-18 13:31:07.000000 mad_whatsapp-0.6/MANIFEST.in
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      842 2024-04-14 09:57:37.608199 mad_whatsapp-0.6/PKG-INFO
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      327 2024-04-14 09:57:36.000000 mad_whatsapp-0.6/README.md
+drwxr-xr-x   0 dobrescu  (1000) dobrescu  (1000)        0 2024-04-14 09:57:37.608199 mad_whatsapp-0.6/mad_whatsapp/
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)       81 2023-09-18 15:07:25.000000 mad_whatsapp-0.6/mad_whatsapp/__init__.py
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)     3092 2024-04-14 09:57:10.000000 mad_whatsapp-0.6/mad_whatsapp/wap.py
+drwxr-xr-x   0 dobrescu  (1000) dobrescu  (1000)        0 2024-04-14 09:57:37.608199 mad_whatsapp-0.6/mad_whatsapp.egg-info/
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      842 2024-04-14 09:57:37.000000 mad_whatsapp-0.6/mad_whatsapp.egg-info/PKG-INFO
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      227 2024-04-14 09:57:37.000000 mad_whatsapp-0.6/mad_whatsapp.egg-info/SOURCES.txt
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)        1 2024-04-14 09:57:37.000000 mad_whatsapp-0.6/mad_whatsapp.egg-info/dependency_links.txt
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)       13 2024-04-14 09:57:37.000000 mad_whatsapp-0.6/mad_whatsapp.egg-info/top_level.txt
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)       38 2024-04-14 09:57:37.608199 mad_whatsapp-0.6/setup.cfg
+-rw-r--r--   0 dobrescu  (1000) dobrescu  (1000)      961 2024-04-14 09:56:39.000000 mad_whatsapp-0.6/setup.py
```

### Comparing `mad_whatsapp-0.5/LICENSE` & `mad_whatsapp-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mad_whatsapp-0.5/PKG-INFO` & `mad_whatsapp-0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad_whatsapp
-Version: 0.5
+Version: 0.6
 Summary: Parses Whatsapp conversations
 Home-page: https://github.com/dobrescu/mad-whatsapp
 Author: Dan Dobrescu
 Author-email: d4n.dobrescu@gmail.com
 License: MIT License
 Keywords: parse whatsapp conversations
 Classifier: Programming Language :: Python
@@ -24,15 +24,15 @@
   "message": "Hello world!"
 }
 ```
 
 ## Build
 
 ```bash
-python setup.py sdist bdist_wheel
+python3 setup.py sdist bdist_wheel
 ```
 
 ## Publish
 
 ```bash
 twine upload dist/*
 ```
```

### Comparing `mad_whatsapp-0.5/mad_whatsapp/wap.py` & `mad_whatsapp-0.6/mad_whatsapp/wap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,99 @@
 import re
 import datetime
 
-IGNORE_MESSAGES = ['<Media Omitted>','<Multimedia omitido>', 'null']
-DATE_PATTERN = r'(?P<date>\d{1,2}/\d{1,2}/\d{2,4}), (?P<time>\d{1,2}:\d{2})'
-AUTHOR_PATTERN = r'- (?P<author>.*?):'
-CONTENT_PATTERN = r'- .*?: (?P<content>.*)'
+
+IGNORE_MESSAGES = [
+    "<Media Omitted>",
+    "<Multimedia omitido>",
+    "<Video message omitted>",
+    "Missed voice call",
+    "Missed video call",
+    "null",
+]
+DATE_PATTERN = r"(?P<date>\d{1,2}/\d{1,2}/\d{2,4}), (?P<time>\d{1,2}:\d{2})"
+AUTHOR_PATTERN = r"- (?P<author>.*?):"
+CONTENT_PATTERN = r"- .*?: (?P<content>.*)"
+
 
 def parse_whatsapp_conversation(conversation):
     if isinstance(conversation, str):
-        conversation = conversation.split('\n')
+        conversation = conversation.split("\n")
 
     messages = []
     buffer = []
     format_type = infer_date_format(conversation)
 
     for line in conversation:
         match = re.match(DATE_PATTERN, line)
         if match:
             if buffer:
-                parsed_message = parse_message(''.join(buffer), format_type)
-                if parsed_message['content']:
+                parsed_message = parse_message("".join(buffer), format_type)
+                if parsed_message["content"]:
                     messages.append(parsed_message)
                 buffer = []
         buffer.append(line)
 
     if buffer:
-        parsed_message = parse_message(''.join(buffer), format_type)
-        if parsed_message['content']:
+        parsed_message = parse_message("".join(buffer), format_type)
+        if parsed_message["content"]:
             messages.append(parsed_message)
     return messages
 
+
 def parse_whatsapp_file(filename):
-    with open(filename, 'r', encoding='utf-8') as f:
+    with open(filename, "r", encoding="utf-8") as f:
         lines = f.readlines()
     return parse_whatsapp_conversation(lines)
 
+
 def parse_message(message, format_type):
     date_match = re.search(DATE_PATTERN, message)
     author_match = re.search(AUTHOR_PATTERN, message)
     content_match = re.search(CONTENT_PATTERN, message)
 
-    content = content_match.group('content').strip() if content_match else None
+    content = content_match.group("content").strip() if content_match else None
     for phrase in IGNORE_MESSAGES:
         content = re.sub(re.escape(phrase), "", content, flags=re.IGNORECASE)
 
-    normalized_date = normalize_date_format(date_match.group('date'), format_type) if date_match else None
-    time_string = date_match.group('time') if date_match else None
+    normalized_date = (
+        normalize_date_format(date_match.group("date"), format_type)
+        if date_match
+        else None
+    )
+    time_string = date_match.group("time") if date_match else None
     if time_string:
-        hour, minute = time_string.split(':')
+        hour, minute = time_string.split(":")
         time_string = f"{int(hour):02d}:{int(minute):02d}"
 
     return {
-        'timestamp': f"{normalized_date} {time_string}" if normalized_date and time_string else None,
-        'author': author_match.group('author') if author_match else None,
-        'content': content
+        "timestamp": f"{normalized_date} {time_string}"
+        if normalized_date and time_string
+        else None,
+        "author": author_match.group("author") if author_match else None,
+        "content": content,
     }
 
+
 def normalize_date_format(date_string, format_type):
-    if format_type == 'DMY':
-        date_format = '%d/%m/%y'
+    year_length = 2 if len(date_string.split('/')[-1]) == 2 else 4
+    if format_type == "DMY":
+        date_format = "%d/%m/%Y" if year_length == 4 else "%d/%m/%y"
     else:
-        date_format = '%m/%d/%y'
+        date_format = "%m/%d/%Y" if year_length == 4 else "%m/%d/%y"
     date_obj = datetime.datetime.strptime(date_string, date_format)
-    return date_obj.strftime('%d/%m/%y')
+    return date_obj.strftime("%d/%m/%Y")
+
 
 def infer_date_format(conversation):
     day_first_count = 0
     month_first_count = 0
 
     for line in conversation:
         match = re.match(DATE_PATTERN, line)
         if match:
-            date_parts = match.group('date').split('/')
+            date_parts = match.group("date").split("/")
             if int(date_parts[0]) > 12:
                 day_first_count += 1
             else:
                 month_first_count += 1
-
-    return 'DMY' if day_first_count > month_first_count else 'MDY'
+    return "DMY" if day_first_count > month_first_count else "MDY"
```

### Comparing `mad_whatsapp-0.5/mad_whatsapp.egg-info/PKG-INFO` & `mad_whatsapp-0.6/mad_whatsapp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mad-whatsapp
-Version: 0.5
+Version: 0.6
 Summary: Parses Whatsapp conversations
 Home-page: https://github.com/dobrescu/mad-whatsapp
 Author: Dan Dobrescu
 Author-email: d4n.dobrescu@gmail.com
 License: MIT License
 Keywords: parse whatsapp conversations
 Classifier: Programming Language :: Python
@@ -24,15 +24,15 @@
   "message": "Hello world!"
 }
 ```
 
 ## Build
 
 ```bash
-python setup.py sdist bdist_wheel
+python3 setup.py sdist bdist_wheel
 ```
 
 ## Publish
 
 ```bash
 twine upload dist/*
 ```
```

### Comparing `mad_whatsapp-0.5/setup.py` & `mad_whatsapp-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import find_packages
 
 setuptools.setup(name='mad_whatsapp',
-                 version='0.5',
+                 version='0.6',
                  description='Parses Whatsapp conversations',
                  long_description_content_type="text/markdown",
                  long_description=open('README.md', encoding='utf-8').read().strip(),
                  author='Dan Dobrescu',
                  author_email='d4n.dobrescu@gmail.com',
                  url='https://github.com/dobrescu/mad-whatsapp',
                  install_requires=[],
```

