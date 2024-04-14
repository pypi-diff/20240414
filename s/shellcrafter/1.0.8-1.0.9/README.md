# Comparing `tmp/shellcrafter-1.0.8.tar.gz` & `tmp/shellcrafter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.0.8.tar", last modified: Mon May 22 17:42:44 2023, max compression
+gzip compressed data, was "shellcrafter-1.0.9.tar", last modified: Mon May 22 17:46:52 2023, max compression
```

## Comparing `shellcrafter-1.0.8.tar` & `shellcrafter-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:42:44.873062 shellcrafter-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-22 17:42:44.873062 shellcrafter-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-22 17:42:19.000000 shellcrafter-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 17:42:19.000000 shellcrafter-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:42:44.873062 shellcrafter-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-22 17:42:19.000000 shellcrafter-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:42:44.873062 shellcrafter-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:42:44.873062 shellcrafter-1.0.8/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:42:19.000000 shellcrafter-1.0.8/src/shellcrafter/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-05-22 17:42:19.000000 shellcrafter-1.0.8/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-05-22 17:42:19.000000 shellcrafter-1.0.8/src/shellcrafter/keyst_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6125 2023-05-22 17:42:19.000000 shellcrafter-1.0.8/src/shellcrafter/shellcode_procedure_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:42:44.873062 shellcrafter-1.0.8/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-22 17:42:44.000000 shellcrafter-1.0.8/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-22 17:42:44.000000 shellcrafter-1.0.8/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:42:44.000000 shellcrafter-1.0.8/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-22 17:42:44.000000 shellcrafter-1.0.8/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 17:42:44.000000 shellcrafter-1.0.8/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 17:42:44.000000 shellcrafter-1.0.8/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:52.791702 shellcrafter-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-22 17:46:52.787702 shellcrafter-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-22 17:46:24.000000 shellcrafter-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-22 17:46:24.000000 shellcrafter-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:46:52.791702 shellcrafter-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-22 17:46:24.000000 shellcrafter-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:52.787702 shellcrafter-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:52.787702 shellcrafter-1.0.9/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:24.000000 shellcrafter-1.0.9/src/shellcrafter/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11958 2023-05-22 17:46:24.000000 shellcrafter-1.0.9/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-05-22 17:46:24.000000 shellcrafter-1.0.9/src/shellcrafter/keyst_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6180 2023-05-22 17:46:24.000000 shellcrafter-1.0.9/src/shellcrafter/shellcode_procedure_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:46:52.787702 shellcrafter-1.0.9/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-22 17:46:52.000000 shellcrafter-1.0.9/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-22 17:46:52.000000 shellcrafter-1.0.9/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:46:52.000000 shellcrafter-1.0.9/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-22 17:46:52.000000 shellcrafter-1.0.9/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 17:46:52.000000 shellcrafter-1.0.9/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 17:46:52.000000 shellcrafter-1.0.9/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.0.8/PKG-INFO` & `shellcrafter-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
```

### Comparing `shellcrafter-1.0.8/README.md` & `shellcrafter-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.8/setup.py` & `shellcrafter-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-version = "1.0.8"
+version = "1.0.9"
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
```

### Comparing `shellcrafter-1.0.8/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.0.9/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.8/src/shellcrafter/keyst_api.py` & `shellcrafter-1.0.9/src/shellcrafter/keyst_api.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.0.8/src/shellcrafter/shellcode_procedure_generator.py` & `shellcrafter-1.0.9/src/shellcrafter/shellcode_procedure_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
     for index, h in enumerate(result):
         part = s[::-1][index * 4: index * 4 + 4]
         if null_free:
             for i in range(5, len(h), 2):
                 if h[i:i + 2] == '00':
                     negated_value = negate_hex(h[5:])
+                    print("xor eax, eax  ;# NULL EAX")
                     print(
                         f"mov eax, {negated_value} ;# Move the negated value of the part \"{part}\" of the string \"{s}\" to EAX to avoid NULL bytes")
                     print("neg eax ;# Negate EAX to get the original value")
                     print("push eax ;# Push EAX onto the stack")
                     break
             else:
                 print(f"{h} ;# Push the part \"{part}\" of the string \"{s}\" onto the stack")
```

### Comparing `shellcrafter-1.0.8/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.0.9/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
```

