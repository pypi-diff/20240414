# Comparing `tmp/Errome-0.2.2.tar.gz` & `tmp/Errome-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Errome-0.2.2.tar", last modified: Fri Apr 12 12:13:31 2024, max compression
+gzip compressed data, was "Errome-0.3.tar", last modified: Sun Apr 14 11:50:28 2024, max compression
```

## Comparing `Errome-0.2.2.tar` & `Errome-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 12:13:31.822168 Errome-0.2.2/
-drwxrwxrwx   0        0        0        0 2024-04-12 12:13:31.814166 Errome-0.2.2/Errome/
--rw-rw-rw-   0        0        0     3101 2024-04-12 11:12:53.000000 Errome-0.2.2/Errome/Errome.py
--rw-rw-rw-   0        0        0        0 2024-04-08 17:11:09.000000 Errome-0.2.2/Errome/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 12:13:31.821166 Errome-0.2.2/Errome/templates/
--rw-rw-rw-   0        0        0     1851 2024-04-08 16:46:21.000000 Errome-0.2.2/Errome/templates/erro.html
--rw-rw-rw-   0        0        0     1451 2024-04-08 16:38:51.000000 Errome-0.2.2/Errome/templates/ok.html
-drwxrwxrwx   0        0        0        0 2024-04-12 12:13:31.820166 Errome-0.2.2/Errome.egg-info/
--rw-rw-rw-   0        0        0     2241 2024-04-12 12:13:31.000000 Errome-0.2.2/Errome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-04-12 12:13:31.000000 Errome-0.2.2/Errome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 12:13:31.000000 Errome-0.2.2/Errome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 12:13:31.000000 Errome-0.2.2/Errome.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       47 2024-04-12 11:06:28.000000 Errome-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2241 2024-04-12 12:13:31.821166 Errome-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1975 2024-04-12 12:05:45.000000 Errome-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 12:13:31.822168 Errome-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      532 2024-04-12 12:09:00.000000 Errome-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:50:28.284399 Errome-0.3/
+drwxrwxrwx   0        0        0        0 2024-04-14 11:50:28.276399 Errome-0.3/Errome/
+-rw-rw-rw-   0        0        0     3186 2024-04-14 11:43:27.000000 Errome-0.3/Errome/Errome.py
+-rw-rw-rw-   0        0        0        0 2024-04-08 17:11:09.000000 Errome-0.3/Errome/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:50:28.282399 Errome-0.3/Errome/templates/
+-rw-rw-rw-   0        0        0     1851 2024-04-08 16:46:21.000000 Errome-0.3/Errome/templates/erro.html
+-rw-rw-rw-   0        0        0     1451 2024-04-08 16:38:51.000000 Errome-0.3/Errome/templates/ok.html
+drwxrwxrwx   0        0        0        0 2024-04-14 11:50:28.281400 Errome-0.3/Errome.egg-info/
+-rw-rw-rw-   0        0        0     2239 2024-04-14 11:50:28.000000 Errome-0.3/Errome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-04-14 11:50:28.000000 Errome-0.3/Errome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 11:50:28.000000 Errome-0.3/Errome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-14 11:50:28.000000 Errome-0.3/Errome.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       47 2024-04-12 11:06:28.000000 Errome-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2239 2024-04-14 11:50:28.283399 Errome-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1975 2024-04-12 12:05:45.000000 Errome-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-14 11:50:28.284399 Errome-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-04-14 11:50:17.000000 Errome-0.3/setup.py
```

### Comparing `Errome-0.2.2/Errome/Errome.py` & `Errome-0.3/Errome/Errome.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import smtplib
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 import datetime
+from pkg_resources import resource_filename
 from functools import wraps
 import traceback
 
 
 class Errome:
     def __init__(self,sender_email, password,recever):
         self.sender_email = sender_email
@@ -23,24 +24,24 @@
         
         message["From"] = f"{self.sender_name}"
         message["To"] = self.recever
         current_time = datetime.datetime.now()
         time_cost = current_time - self.start_time
         if statu == "ok":
             message["Subject"] = "运行完成"
-            with open(r'Errome\templates\ok.html', 'r', encoding='utf-8') as file:
+            with open(resource_filename('Errome','templates\ok.html'), 'r', encoding='utf-8') as file:
                 html_content = file.read()
             html_content = html_content.replace(f"NowTime", current_time.strftime("%Y-%m-%d %H:%M:%S"))
             html_content = html_content.replace(f"Timeuse", str(time_cost.seconds)+"秒")
 
             part = MIMEText(html_content, "html")
             message.attach(part)
         else:
             message["Subject"] = "运行错误"
-            with open(r'Errome\templates\erro.html', 'r', encoding='utf-8') as file:
+            with open(resource_filename('Errome','templates\erro.html'), 'r', encoding='utf-8') as file:
                 html_content = file.read()
             html_content = html_content.replace(f"NowTime", current_time.strftime("%Y-%m-%d %H:%M:%S"))
             html_content = html_content.replace(f"Timeuse", str(time_cost.seconds)+"秒")
             html_content = html_content.replace(f"erro_code", statu)
             part = MIMEText(html_content, "html")
             message.attach(part)
```

### Comparing `Errome-0.2.2/Errome/templates/erro.html` & `Errome-0.3/Errome/templates/erro.html`

 * *Files identical despite different names*

### Comparing `Errome-0.2.2/Errome/templates/ok.html` & `Errome-0.3/Errome/templates/ok.html`

 * *Files identical despite different names*

### Comparing `Errome-0.2.2/Errome.egg-info/PKG-INFO` & `Errome-0.3/Errome.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Errome
-Version: 0.2.2
+Version: 0.3
 Summary: A program error or completion email notification tool.
 Home-page: https://github.com/Becomingw/Errome.git
 Author: BecomingW
 Author-email: Becomingw@qq.com
 Description-Content-Type: text/markdown
 
 # Errome
```

### Comparing `Errome-0.2.2/PKG-INFO` & `Errome-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Errome
-Version: 0.2.2
+Version: 0.3
 Summary: A program error or completion email notification tool.
 Home-page: https://github.com/Becomingw/Errome.git
 Author: BecomingW
 Author-email: Becomingw@qq.com
 Description-Content-Type: text/markdown
 
 # Errome
```

### Comparing `Errome-0.2.2/README.md` & `Errome-0.3/README.md`

 * *Files identical despite different names*

### Comparing `Errome-0.2.2/setup.py` & `Errome-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 setup(
     name='Errome',
-    version='0.2.2',
+    version='0.3',
     packages=find_packages(),
     description='A program error or completion email notification tool.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='BecomingW',
     author_email='Becomingw@qq.com',
     url='https://github.com/Becomingw/Errome.git',
```

