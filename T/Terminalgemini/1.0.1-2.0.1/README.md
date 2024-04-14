# Comparing `tmp/terminalgemini-1.0.1.tar.gz` & `tmp/terminalgemini-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalgemini-1.0.1.tar", last modified: Sun Apr 14 16:17:54 2024, max compression
+gzip compressed data, was "terminalgemini-2.0.1.tar", last modified: Sun Apr 14 20:11:32 2024, max compression
```

## Comparing `terminalgemini-1.0.1.tar` & `terminalgemini-2.0.1.tar`

### file list

```diff
@@ -1,24 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 16:17:54.509726 terminalgemini-1.0.1/
--rw-rw-rw-   0        0        0     1070 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     5435 2024-04-14 16:17:54.508123 terminalgemini-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4382 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 16:17:54.507573 terminalgemini-1.0.1/Terminalgemini.egg-info/
--rw-rw-rw-   0        0        0     5435 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      104 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 16:17:54.000000 terminalgemini-1.0.1/Terminalgemini.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1012 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 16:17:54.509726 terminalgemini-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1871 2024-04-14 16:17:03.000000 terminalgemini-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 16:17:54.505502 terminalgemini-1.0.1/terminalgpt/
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/terminalgpt/__init__.py
--rw-rw-rw-   0        0        0     8077 2024-04-14 00:01:34.000000 terminalgemini-1.0.1/terminalgpt/chat.py
--rw-rw-rw-   0        0        0     3108 2024-04-13 23:53:04.000000 terminalgemini-1.0.1/terminalgpt/config.py
--rw-rw-rw-   0        0        0     2477 2024-04-14 00:01:34.000000 terminalgemini-1.0.1/terminalgpt/conversations.py
--rw-rw-rw-   0        0        0     2368 2024-04-14 04:51:24.000000 terminalgemini-1.0.1/terminalgpt/encryption.py
--rw-rw-rw-   0        0        0    15360 2024-04-14 16:07:39.000000 terminalgemini-1.0.1/terminalgpt/main.py
--rw-rw-rw-   0        0        0     6289 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/terminalgpt/printer.py
-drwxrwxrwx   0        0        0        0 2024-04-14 16:17:54.505502 terminalgemini-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-1.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.199194 terminalgemini-2.0.1/
+-rw-rw-rw-   0        0        0     1070 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0      161 2024-04-14 20:00:13.000000 terminalgemini-2.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5374 2024-04-14 20:11:32.198141 terminalgemini-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4382 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.197133 terminalgemini-2.0.1/Terminalgemini.egg-info/
+-rw-rw-rw-   0        0        0     5374 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      709 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      104 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 20:11:32.000000 terminalgemini-2.0.1/Terminalgemini.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1015 2024-04-14 20:10:43.000000 terminalgemini-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 20:11:32.199194 terminalgemini-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1464 2024-04-14 20:07:07.000000 terminalgemini-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.188320 terminalgemini-2.0.1/terminalgpt/
+-rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/terminalgpt/__init__.py
+-rw-rw-rw-   0        0        0     8077 2024-04-14 00:01:34.000000 terminalgemini-2.0.1/terminalgpt/chat.py
+-rw-rw-rw-   0        0        0     3108 2024-04-14 16:22:56.000000 terminalgemini-2.0.1/terminalgpt/config.py
+-rw-rw-rw-   0        0        0     2477 2024-04-14 00:01:34.000000 terminalgemini-2.0.1/terminalgpt/conversations.py
+-rw-rw-rw-   0        0        0     2368 2024-04-14 04:51:24.000000 terminalgemini-2.0.1/terminalgpt/encryption.py
+-rw-rw-rw-   0        0        0    15360 2024-04-14 16:07:39.000000 terminalgemini-2.0.1/terminalgpt/main.py
+-rw-rw-rw-   0        0        0     6289 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/terminalgpt/printer.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.189363 terminalgemini-2.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.190403 terminalgemini-2.0.1/tests/e2e/
+-rw-rw-rw-   0        0        0     1135 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/e2e/test_new_e2e.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.191957 terminalgemini-2.0.1/tests/integration/
+-rw-rw-rw-   0        0        0     1732 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/integration/test_load_integration.py
+-rw-rw-rw-   0        0        0     6699 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/integration/test_new_integration.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:11:32.196126 terminalgemini-2.0.1/tests/unit/
+-rw-rw-rw-   0        0        0      407 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/mocks.py
+-rw-rw-rw-   0        0        0     5694 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/test_chat.py
+-rw-rw-rw-   0        0        0     5574 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/test_conversations.py
+-rw-rw-rw-   0        0        0      921 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/test_load_unit.py
+-rw-rw-rw-   0        0        0     5127 2024-04-13 01:32:20.000000 terminalgemini-2.0.1/tests/unit/test_printer.py
```

### Comparing `terminalgemini-1.0.1/LICENSE` & `terminalgemini-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalgemini-1.0.1/PKG-INFO` & `terminalgemini-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: Terminalgemini
-Version: 1.0.1
+Version: 2.0.1
 Summary: AI chat assistant in your terminal powered by Gemini models.
-Home-page: https://github.com/yourusername/TerminalGPT-main
 Author: ticklecatisback
 Author-email: alesaholder@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `terminalgemini-1.0.1/README.md` & `terminalgemini-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `terminalgemini-1.0.1/Terminalgemini.egg-info/PKG-INFO` & `terminalgemini-2.0.1/Terminalgemini.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: Terminalgemini
-Version: 1.0.1
+Version: 2.0.1
 Summary: AI chat assistant in your terminal powered by Gemini models.
-Home-page: https://github.com/yourusername/TerminalGPT-main
 Author: ticklecatisback
 Author-email: alesaholder@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `terminalgemini-1.0.1/pyproject.toml` & `terminalgemini-2.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-name = "terminalgpt"
-version = "2.1.3"
+name = "Terminalgemini"
+version = "2.0.1"
 description = "AI chat assistant in your terminal powered by OpenAI ChatGPT models."
 authors = ["Adam Yodinsky <27074934+adamyodinsky@users.noreply.github.com>"]
 keywords = [
   "ai",
   "chat",
   "terminal",
   "openai",
```

### Comparing `terminalgemini-1.0.1/setup.py` & `terminalgemini-2.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='Terminalgemini',  # Name of your package
-    version='1.0.1',  # Version of your package
-    author='ticklecatisback',  # Your name or your organization's name
-    author_email='alesaholder@gmail.com',  # Your email or your organization's contact email
-    description='AI chat assistant in your terminal powered by Gemini models.',  # Short description of your package
-    long_description=open('README.md').read(),  # Long description read from the README.md file
-    long_description_content_type='text/markdown',  # Type of the long description, here markdown
-    url='https://github.com/yourusername/TerminalGPT-main',  # Link to your project's GitHub repo
-    packages=find_packages(),  # Automatically find all packages and subpackages
-    include_package_data=True,  # Include everything in source control
+    name='Terminalgemini',
+    version='2.0.1',  # Update this as you make changes
+    author='ticklecatisback',
+    author_email='alesaholder@gmail.com',
+    description='AI chat assistant in your terminal powered by Gemini models.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    packages=find_packages(),  # Automatically find all packages in the directory
+    include_package_data=True,  # Include all files specified in MANIFEST.in
+    package_data={
+        'tests': ['tests/*.py', 'tests/e2e/*.py', 'tests/integration/*.py', 'tests/unit/*.py']
+    },
     install_requires=[
         'google-generativeai',
         'tiktoken',
         'colorama',
         'cryptography',
         'click',
         'prompt-toolkit',
         'yaspin',
         'rich',
         'isort',
         'pytest',
         'pylint'
-    ],  # List of packages required to run your project, installed by pip install your-package
+    ],
     entry_points={
         'console_scripts': [
-            'terminalgpt=terminalgpt.main:cli'  # Provide a command line script
+            'terminalgpt=terminalgpt.main:cli'
         ],
     },
     classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
     ],
-    python_requires='>=3.10',  # Minimum version requirement of Python
-)
+    python_requires='>=3.10',  # Specify the minimum required Python version
+)
```

### Comparing `terminalgemini-1.0.1/terminalgpt/chat.py` & `terminalgemini-2.0.1/terminalgpt/chat.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-1.0.1/terminalgpt/config.py` & `terminalgemini-2.0.1/terminalgpt/config.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-1.0.1/terminalgpt/conversations.py` & `terminalgemini-2.0.1/terminalgpt/conversations.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-1.0.1/terminalgpt/encryption.py` & `terminalgemini-2.0.1/terminalgpt/encryption.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-1.0.1/terminalgpt/main.py` & `terminalgemini-2.0.1/terminalgpt/main.py`

 * *Files identical despite different names*

### Comparing `terminalgemini-1.0.1/terminalgpt/printer.py` & `terminalgemini-2.0.1/terminalgpt/printer.py`

 * *Files identical despite different names*

