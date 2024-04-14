# Comparing `tmp/vs-colabi-1.1.3.tar.gz` & `tmp/vs-colabi-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vs-colabi-1.1.3.tar", last modified: Sat Apr 13 05:40:14 2024, max compression
+gzip compressed data, was "vs-colabi-1.1.4.tar", last modified: Sat Apr 13 07:35:43 2024, max compression
```

## Comparing `vs-colabi-1.1.3.tar` & `vs-colabi-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:40:14.167562 vs-colabi-1.1.3/
--rw-r--r--   0 root         (0) root         (0)     1105 2024-04-13 05:40:14.167562 vs-colabi-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-13 05:40:05.000000 vs-colabi-1.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 05:40:14.167562 vs-colabi-1.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2599 2024-04-13 05:40:05.000000 vs-colabi-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:40:14.166562 vs-colabi-1.1.3/vs_colabi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1105 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-13 05:40:14.000000 vs-colabi-1.1.3/vs_colabi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 05:40:14.166562 vs-colabi-1.1.3/vscolabi/
--rw-rw-rw-   0 root         (0) root         (0)     3347 2024-04-13 05:40:05.000000 vs-colabi-1.1.3/vscolabi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:35:43.953583 vs-colabi-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-13 07:35:43.953583 vs-colabi-1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-13 07:35:35.000000 vs-colabi-1.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 07:35:43.953583 vs-colabi-1.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2024-04-13 07:35:35.000000 vs-colabi-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:35:43.953583 vs-colabi-1.1.4/vs_colabi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-13 07:35:43.000000 vs-colabi-1.1.4/vs_colabi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2024-04-13 07:35:43.000000 vs-colabi-1.1.4/vs_colabi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 07:35:43.000000 vs-colabi-1.1.4/vs_colabi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 07:35:43.000000 vs-colabi-1.1.4/vs_colabi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-13 07:35:43.000000 vs-colabi-1.1.4/vs_colabi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 07:35:43.952583 vs-colabi-1.1.4/vscolabi/
+-rw-rw-rw-   0 root         (0) root         (0)     3414 2024-04-13 07:35:35.000000 vs-colabi-1.1.4/vscolabi/__init__.py
```

### Comparing `vs-colabi-1.1.3/PKG-INFO` & `vs-colabi-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vs-colabi
-Version: 1.1.3
+Version: 1.1.4
 Summary: Run vs code tunnel inside colab notebook
 Home-page: https://gitlab.com/isampypi/vs-colabi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vs-colabi-1.1.3/README.md` & `vs-colabi-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vs-colabi-1.1.3/setup.py` & `vs-colabi-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `vs-colabi-1.1.3/vs_colabi.egg-info/PKG-INFO` & `vs-colabi-1.1.4/vs_colabi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vs-colabi
-Version: 1.1.3
+Version: 1.1.4
 Summary: Run vs code tunnel inside colab notebook
 Home-page: https://gitlab.com/isampypi/vs-colabi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vs-colabi-1.1.3/vscolabi/__init__.py` & `vs-colabi-1.1.4/vscolabi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     vs_code_btn  = """
       <!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <title>Section with Button</title> <style> body {{ margin: 0; padding: 0; font-family: Arial, sans-serif; }} .section {{background-color: #fff; padding: 50px; text-align: center; }} .button {{display: inline-block; padding: 20px 40px; /* Adjust padding to make the button bigger */ font-size: 25px; /* Increase font size */ background-color: #007bff; color: #fff; border: none; border-radius: 5px; cursor: pointer; width: 80%; font-weight: 400; letter-spacing: 2px ; }} </style> </head> <body> <section class="section"> <button onclick="window.open('{openpath}', '_blank' {singletab});" class = "button" >Open vs-code .</button> </section> </body> </html>    
     """.format(openpath = openpath, singletab = singletab )
     if not os.path.exists("./code") : 
         assert b.bash('''
         curl -Lk 'https://code.visualstudio.com/sha/download?build=stable&os=cli-alpine-x64' --output vscode_cli.tar.gz && tar -xf vscode_cli.tar.gz && rm vscode_cli.tar.gz
         ''').ok
+    else : 
+      subprocess.Popen("./code tunnel prune ").wait() 
     process = subprocess.Popen("./code tunnel user login --provider microsoft", stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, shell=True)
     Message = process.stdout.readline()
     code_to_authenticate = [i.strip() for i in Message.strip().split() if i.strip() == i.strip().upper()][0]
     clear_output()
     display(HTML(html_code.format(code_to_authenticate = code_to_authenticate)))
     process.wait()
     clear_output()
```

