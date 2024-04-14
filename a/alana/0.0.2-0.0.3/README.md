# Comparing `tmp/alana-0.0.2.tar.gz` & `tmp/alana-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alana-0.0.2.tar", last modified: Sat Apr 13 09:24:23 2024, max compression
+gzip compressed data, was "alana-0.0.3.tar", last modified: Sat Apr 13 15:00:50 2024, max compression
```

## Comparing `alana-0.0.2.tar` & `alana-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:24:23.558023 alana-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-13 09:24:19.000000 alana-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-13 09:24:23.558023 alana-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-13 09:24:19.000000 alana-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:24:23.558023 alana-0.0.2/alana/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-13 09:24:19.000000 alana-0.0.2/alana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-13 09:24:19.000000 alana-0.0.2/alana/alana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-13 09:24:19.000000 alana-0.0.2/alana/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-13 09:24:19.000000 alana-0.0.2/alana/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:24:23.558023 alana-0.0.2/alana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 09:24:23.000000 alana-0.0.2/alana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 09:24:23.558023 alana-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-13 09:24:19.000000 alana-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:00:50.387466 alana-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-13 15:00:44.000000 alana-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-13 15:00:50.387466 alana-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-13 15:00:44.000000 alana-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:00:50.383466 alana-0.0.3/alana/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-13 15:00:44.000000 alana-0.0.3/alana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-13 15:00:44.000000 alana-0.0.3/alana/alana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-13 15:00:44.000000 alana-0.0.3/alana/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-04-13 15:00:44.000000 alana-0.0.3/alana/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:00:50.387466 alana-0.0.3/alana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:00:50.387466 alana-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-13 15:00:44.000000 alana-0.0.3/setup.py
```

### Comparing `alana-0.0.2/LICENSE` & `alana-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alana-0.0.2/PKG-INFO` & `alana-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alana
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.
 Home-page: https://github.com/alat-rights/alana-utilities
 Author: Alana
 Author-email: hi@alana.computer
 Keywords: LLM,utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alana-0.0.2/README.md` & `alana-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alana-0.0.2/alana/color.py` & `alana-0.0.3/alana/color.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Optional
 import logging
 
 # A hacky utils library I put together for myself to write code faster. Please don't judge!
 # Feedback always welcome.
 
 # Debugging and logging!
-def log(loud: bool, output: str, logger: Optional[logging.Logger]):
+def log(loud: bool, output: str, logger: Optional[logging.Logger] = None) -> None:
     if loud:
         print(output)
     if logger:
         logger.info(output)
 
 def red(var: Any, loud: bool = True, logger: Optional[logging.Logger] = None) -> str:
     output = f"{Fore.RED} {var} {Style.RESET_ALL}"
@@ -31,8 +31,9 @@
     output = f"{Fore.YELLOW} {var} {Style.RESET_ALL}"
     log(loud, output, logger)
     return output
 
 def cyan(var: Any, loud: bool = True, logger: Optional[logging.Logger] = None) -> str:
     output = f"{Fore.CYAN} {var} {Style.RESET_ALL}"
     log(loud, output, logger)
-    return output
+    return output
+
```

### Comparing `alana-0.0.2/alana.egg-info/PKG-INFO` & `alana-0.0.3/alana.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alana
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.
 Home-page: https://github.com/alat-rights/alana-utilities
 Author: Alana
 Author-email: hi@alana.computer
 Keywords: LLM,utilities
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alana-0.0.2/setup.py` & `alana-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
    name='alana',
-   version='0.0.2',  # Update the version number as needed
+   version='0.0.3',  # Update the version number as needed
    author='Alana',
    author_email='hi@alana.computer',
    description='Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.',
    long_description=long_description,
    long_description_content_type="text/markdown",
    url='https://github.com/alat-rights/alana-utilities',
    packages=find_packages(),
```

