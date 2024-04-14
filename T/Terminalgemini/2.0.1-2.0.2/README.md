# Comparing `tmp/terminalgemini-2.0.1.tar.gz` & `tmp/terminalgemini-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalgemini-2.0.1.tar", last modified: Sun Apr 14 20:11:32 2024, max compression
+gzip compressed data, was "terminalgemini-2.0.2.tar", last modified: Sun Apr 14 20:27:58 2024, max compression
```

## Comparing `terminalgemini-2.0.1.tar` & `terminalgemini-2.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.199194 terminalgemini-2.0.1/
--rw-rw-rw-   0        0        0     1070 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      161 2024-04-14 20:00:13.000000 terminalgemini-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5374 2024-04-14 20:11:32.198141 terminalgemini-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4382 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.197133 terminalgemini-2.0.1/Terminalgemini.egg-info/
--rw-rw-rw-   0        0        0     5374 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      709 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1015 2024-04-14 20:10:43.000000 terminalgemini-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 20:11:32.199194 terminalgemini-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1464 2024-04-14 20:07:07.000000 terminalgemini-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.188320 terminalgemini-2.0.1/terminalgpt/
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/terminalgpt/__init__.py
--rw-rw-rw-   0        0        0     8077 2024-04-14 00:01:34.000000 terminalgemini-2.0.1/terminalgpt/chat.py
--rw-rw-rw-   0        0        0     3108 2024-04-14 16:22:56.000000 terminalgemini-2.0.1/terminalgpt/config.py
--rw-rw-rw-   0        0        0     2477 2024-04-14 00:01:34.000000 terminalgemini-2.0.1/terminalgpt/conversations.py
--rw-rw-rw-   0        0        0     2368 2024-04-14 04:51:24.000000 terminalgemini-2.0.1/terminalgpt/encryption.py
--rw-rw-rw-   0        0        0    15360 2024-04-14 16:07:39.000000 terminalgemini-2.0.1/terminalgpt/main.py
--rw-rw-rw-   0        0        0     6289 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/terminalgpt/printer.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.189363 terminalgemini-2.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.190403 terminalgemini-2.0.1/tests/e2e/
--rw-rw-rw-   0        0        0     1135 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/e2e/test_new_e2e.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.191957 terminalgemini-2.0.1/tests/integration/
--rw-rw-rw-   0        0        0     1732 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/integration/test_load_integration.py
--rw-rw-rw-   0        0        0     6699 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/integration/test_new_integration.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.196126 terminalgemini-2.0.1/tests/unit/
--rw-rw-rw-   0        0        0      407 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/mocks.py
--rw-rw-rw-   0        0        0     5694 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/test_chat.py
--rw-rw-rw-   0        0        0     5574 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/test_conversations.py
--rw-rw-rw-   0        0        0      921 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/test_load_unit.py
--rw-rw-rw-   0        0        0     5127 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/test_printer.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:58.465979 terminalgemini-2.0.2/
+-rw-rw-rw-   0        0        0     1070 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0      161 2024-04-14 20:00:13.000000 terminalgemini-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5374 2024-04-14 20:27:58.463954 terminalgemini-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4382 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:58.462943 terminalgemini-2.0.2/Terminalgemini.egg-info/
+-rw-rw-rw-   0        0        0     5374 2024-04-14 20:27:58.000000 terminalgemini-2.0.2/Terminalgemini.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      709 2024-04-14 20:27:58.000000 terminalgemini-2.0.2/Terminalgemini.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 20:27:58.000000 terminalgemini-2.0.2/Terminalgemini.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-14 20:27:58.000000 terminalgemini-2.0.2/Terminalgemini.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2024-04-14 20:27:58.000000 terminalgemini-2.0.2/Terminalgemini.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 20:27:58.000000 terminalgemini-2.0.2/Terminalgemini.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1015 2024-04-14 20:10:43.000000 terminalgemini-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 20:27:58.465979 terminalgemini-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2024-04-14 20:24:30.000000 terminalgemini-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:58.454342 terminalgemini-2.0.2/terminalgpt/
+-rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/terminalgpt/__init__.py
+-rw-rw-rw-   0        0        0     8077 2024-04-14 00:01:34.000000 terminalgemini-2.0.2/terminalgpt/chat.py
+-rw-rw-rw-   0        0        0     3108 2024-04-14 16:22:56.000000 terminalgemini-2.0.2/terminalgpt/config.py
+-rw-rw-rw-   0        0        0     2477 2024-04-14 00:01:34.000000 terminalgemini-2.0.2/terminalgpt/conversations.py
+-rw-rw-rw-   0        0        0     2368 2024-04-14 04:51:24.000000 terminalgemini-2.0.2/terminalgpt/encryption.py
+-rw-rw-rw-   0        0        0    15360 2024-04-14 16:07:39.000000 terminalgemini-2.0.2/terminalgpt/main.py
+-rw-rw-rw-   0        0        0     6289 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/terminalgpt/printer.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:58.455350 terminalgemini-2.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:58.455350 terminalgemini-2.0.2/tests/e2e/
+-rw-rw-rw-   0        0        0     1135 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/e2e/test_new_e2e.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:58.457832 terminalgemini-2.0.2/tests/integration/
+-rw-rw-rw-   0        0        0     1732 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/integration/test_load_integration.py
+-rw-rw-rw-   0        0        0     6699 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/integration/test_new_integration.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:58.461937 terminalgemini-2.0.2/tests/unit/
+-rw-rw-rw-   0        0        0      407 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/unit/mocks.py
+-rw-rw-rw-   0        0        0     5694 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/unit/test_chat.py
+-rw-rw-rw-   0        0        0     5574 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/unit/test_conversations.py
+-rw-rw-rw-   0        0        0      921 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/unit/test_load_unit.py
+-rw-rw-rw-   0        0        0     5127 2024-04-13 01:32:20.000000 terminalgemini-2.0.2/tests/unit/test_printer.py
```

### Comparing `terminalgemini-2.0.1/LICENSE` & `terminalgemini-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/PKG-INFO` & `terminalgemini-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Terminalgemini
-Version: 2.0.1
+Version: 2.0.2
 Summary: AI chat assistant in your terminal powered by Gemini models.
 Author: ticklecatisback
 Author-email: alesaholder@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminalgemini-2.0.1/README.md` & `terminalgemini-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/Terminalgemini.egg-info/PKG-INFO` & `terminalgemini-2.0.2/Terminalgemini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Terminalgemini
-Version: 2.0.1
+Version: 2.0.2
 Summary: AI chat assistant in your terminal powered by Gemini models.
 Author: ticklecatisback
 Author-email: alesaholder@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminalgemini-2.0.1/Terminalgemini.egg-info/SOURCES.txt` & `terminalgemini-2.0.2/Terminalgemini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/pyproject.toml` & `terminalgemini-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/setup.py` & `terminalgemini-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Terminalgemini',
-    version='2.0.1',  # Update this as you make changes
+    version='2.0.2',  # Update this as you make changes
     author='ticklecatisback',
     author_email='alesaholder@gmail.com',
     description='AI chat assistant in your terminal powered by Gemini models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),  # Automatically find all packages in the directory
     include_package_data=True,  # Include all files specified in MANIFEST.in
     package_data={
-        'tests': ['tests/*.py', 'tests/e2e/*.py', 'tests/integration/*.py', 'tests/unit/*.py']
+        'terminalgemini': ['tests/*.py', 'tests/e2e/*.py', 'tests/integration/*.py', 'tests/unit/*.py', 'terminalgpt'
+                                                                                                        '/*.py']
     },
     install_requires=[
         'google-generativeai',
         'tiktoken',
         'colorama',
         'cryptography',
         'click',
```

### Comparing `terminalgemini-2.0.1/terminalgpt/chat.py` & `terminalgemini-2.0.2/terminalgpt/chat.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/terminalgpt/config.py` & `terminalgemini-2.0.2/terminalgpt/config.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/terminalgpt/conversations.py` & `terminalgemini-2.0.2/terminalgpt/conversations.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/terminalgpt/encryption.py` & `terminalgemini-2.0.2/terminalgpt/encryption.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/terminalgpt/main.py` & `terminalgemini-2.0.2/terminalgpt/main.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/terminalgpt/printer.py` & `terminalgemini-2.0.2/terminalgpt/printer.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/tests/e2e/test_new_e2e.py` & `terminalgemini-2.0.2/tests/e2e/test_new_e2e.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/tests/integration/test_load_integration.py` & `terminalgemini-2.0.2/tests/integration/test_load_integration.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/tests/integration/test_new_integration.py` & `terminalgemini-2.0.2/tests/integration/test_new_integration.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/tests/unit/test_chat.py` & `terminalgemini-2.0.2/tests/unit/test_chat.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/tests/unit/test_conversations.py` & `terminalgemini-2.0.2/tests/unit/test_conversations.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/tests/unit/test_load_unit.py` & `terminalgemini-2.0.2/tests/unit/test_load_unit.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-2.0.1/tests/unit/test_printer.py` & `terminalgemini-2.0.2/tests/unit/test_printer.py`

 * *Files identical despite different names*

