# Comparing `tmp/PathMePy-0.5.tar.gz` & `tmp/PathMePy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PathMePy-0.5.tar", last modified: Sun Apr 14 12:26:19 2024, max compression
+gzip compressed data, was "PathMePy-0.5.1.tar", last modified: Sun Apr 14 12:29:57 2024, max compression
```

## Comparing `PathMePy-0.5.tar` & `PathMePy-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 12:26:19.723290 PathMePy-0.5/
--rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1364 2024-04-14 12:26:19.721293 PathMePy-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 12:26:19.684335 PathMePy-0.5/PathMePy/
--rw-rw-rw-   0        0        0     1718 2024-04-10 16:49:09.000000 PathMePy-0.5/PathMePy/PathMePy.py
--rw-rw-rw-   0        0        0      181 2024-04-10 15:24:15.000000 PathMePy-0.5/PathMePy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 12:26:19.718295 PathMePy-0.5/PathMePy.egg-info/
--rw-rw-rw-   0        0        0     1364 2024-04-14 12:26:19.000000 PathMePy-0.5/PathMePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-14 12:26:19.000000 PathMePy-0.5/PathMePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 12:26:19.000000 PathMePy-0.5/PathMePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 12:26:19.000000 PathMePy-0.5/PathMePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      993 2024-04-10 15:27:39.000000 PathMePy-0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 12:26:19.724292 PathMePy-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1436 2024-04-14 12:26:14.000000 PathMePy-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 12:29:56.991528 PathMePy-0.5.1/
+-rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1350 2024-04-14 12:29:56.989528 PathMePy-0.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 12:29:56.961545 PathMePy-0.5.1/PathMePy/
+-rw-rw-rw-   0        0        0     1718 2024-04-10 16:49:09.000000 PathMePy-0.5.1/PathMePy/PathMePy.py
+-rw-rw-rw-   0        0        0      181 2024-04-10 15:24:15.000000 PathMePy-0.5.1/PathMePy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 12:29:56.986530 PathMePy-0.5.1/PathMePy.egg-info/
+-rw-rw-rw-   0        0        0     1350 2024-04-14 12:29:56.000000 PathMePy-0.5.1/PathMePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-14 12:29:56.000000 PathMePy-0.5.1/PathMePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 12:29:56.000000 PathMePy-0.5.1/PathMePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 12:29:56.000000 PathMePy-0.5.1/PathMePy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      977 2024-04-14 12:29:25.000000 PathMePy-0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-14 12:29:56.992528 PathMePy-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-04-14 12:29:52.000000 PathMePy-0.5.1/setup.py
```

### Comparing `PathMePy-0.5/LICENSE.txt` & `PathMePy-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PathMePy-0.5/PKG-INFO` & `PathMePy-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PathMePy
-Version: 0.5
+Version: 0.5.1
 Summary: A tool to add scripts to Path
 Author: Gustoon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.2
@@ -12,18 +12,18 @@
 License-File: LICENSE.txt
 
 
 # PathMePy
 A tool to add scripts to Path
 
 ## Installation
-You have to install the package using pip : `pip install PathMePy-Gustoon`
+You have to install the package using pip : `pip install PathMePy`
 
 ## Content
-You need to import this package with `import PathMePy_Gustoon`
+You need to import this package with `import PathMePy`
 This packages add three functions : 
 `PathMePyDir(path)`,
 `PathMePyUserScriptFolder()`,
 `IsAlreadyOnPath(path)`,
 `UserScriptFolderIsAlreadyOnPath()`,
 two variables `Current_Path` and `Current_Path_Formated`
```

### Comparing `PathMePy-0.5/PathMePy/PathMePy.py` & `PathMePy-0.5.1/PathMePy/PathMePy.py`

 * *Files identical despite different names*

### Comparing `PathMePy-0.5/PathMePy.egg-info/PKG-INFO` & `PathMePy-0.5.1/PathMePy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PathMePy
-Version: 0.5
+Version: 0.5.1
 Summary: A tool to add scripts to Path
 Author: Gustoon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.2
@@ -12,18 +12,18 @@
 License-File: LICENSE.txt
 
 
 # PathMePy
 A tool to add scripts to Path
 
 ## Installation
-You have to install the package using pip : `pip install PathMePy-Gustoon`
+You have to install the package using pip : `pip install PathMePy`
 
 ## Content
-You need to import this package with `import PathMePy_Gustoon`
+You need to import this package with `import PathMePy`
 This packages add three functions : 
 `PathMePyDir(path)`,
 `PathMePyUserScriptFolder()`,
 `IsAlreadyOnPath(path)`,
 `UserScriptFolderIsAlreadyOnPath()`,
 two variables `Current_Path` and `Current_Path_Formated`
```

### Comparing `PathMePy-0.5/README.md` & `PathMePy-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PathMePy
 A tool to add scripts to Path
 
 ## Installation
-You have to install the package using pip : `pip install PathMePy-Gustoon`
+You have to install the package using pip : `pip install PathMePy`
 
 ## Content
-You need to import this package with `import PathMePy_Gustoon`
+You need to import this package with `import PathMePy`
 This packages add three functions : 
 `PathMePyDir(path)`,
 `PathMePyUserScriptFolder()`,
 `IsAlreadyOnPath(path)`,
 `UserScriptFolderIsAlreadyOnPath()`,
 two variables `Current_Path` and `Current_Path_Formated`
```

### Comparing `PathMePy-0.5/setup.py` & `PathMePy-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
 name='PathMePy',
-version='0.5',
+version='0.5.1',
 author='Gustoon',
 author_email='',
 description='A tool to add scripts to Path',
 long_description="""
 # PathMePy
 A tool to add scripts to Path
 
 ## Installation
-You have to install the package using pip : `pip install PathMePy-Gustoon`
+You have to install the package using pip : `pip install PathMePy`
 
 ## Content
-You need to import this package with `import PathMePy_Gustoon`
+You need to import this package with `import PathMePy`
 This packages add three functions : 
 `PathMePyDir(path)`,
 `PathMePyUserScriptFolder()`,
 `IsAlreadyOnPath(path)`,
 `UserScriptFolderIsAlreadyOnPath()`,
 two variables `Current_Path` and `Current_Path_Formated`
```

