# Comparing `tmp/bibiflags-0.1.4.tar.gz` & `tmp/bibiflags-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibiflags-0.1.4.tar", last modified: Fri Apr 12 03:16:46 2024, max compression
+gzip compressed data, was "bibiflags-0.1.5.tar", last modified: Sun Apr 14 15:05:48 2024, max compression
```

## Comparing `bibiflags-0.1.4.tar` & `bibiflags-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.107517 bibiflags-0.1.4/
--rw-rw-rw-   0        0        0     1067 2021-10-28 05:43:21.000000 bibiflags-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      297 2024-04-10 06:25:01.000000 bibiflags-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3185 2024-04-12 03:16:46.106517 bibiflags-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2607 2024-04-12 03:15:18.000000 bibiflags-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.064516 bibiflags-0.1.4/docs/
--rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiflags-0.1.4/docs/Makefile
--rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiflags-0.1.4/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.067517 bibiflags-0.1.4/docs/source/
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.068517 bibiflags-0.1.4/docs/source/_static/
--rw-rw-rw-   0        0        0    33653 2024-04-10 06:08:59.000000 bibiflags-0.1.4/docs/source/_static/bibiflags.png
--rw-rw-rw-   0        0        0     6901 2024-04-10 05:06:41.000000 bibiflags-0.1.4/docs/source/conf.py
--rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiflags-0.1.4/docs/source/install.rst
--rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiflags-0.1.4/docs/source/quickstart.rst
--rw-rw-rw-   0        0        0      793 2024-04-12 03:15:23.000000 bibiflags-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 03:16:46.107517 bibiflags-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.059517 bibiflags-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.070518 bibiflags-0.1.4/src/bibiflags/
--rw-rw-rw-   0        0        0      104 2024-04-12 03:15:30.000000 bibiflags-0.1.4/src/bibiflags/__init__.py
--rw-rw-rw-   0        0        0     7015 2024-04-12 03:13:03.000000 bibiflags-0.1.4/src/bibiflags/bibiflags.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.4/src/bibiflags/bibiflags.yaml
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.105518 bibiflags-0.1.4/src/bibiflags.egg-info/
--rw-rw-rw-   0        0        0     3185 2024-04-12 03:16:46.000000 bibiflags-0.1.4/src/bibiflags.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2024-04-12 03:16:46.000000 bibiflags-0.1.4/src/bibiflags.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 03:16:46.000000 bibiflags-0.1.4/src/bibiflags.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-12 03:16:46.000000 bibiflags-0.1.4/src/bibiflags.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-12 03:16:46.000000 bibiflags-0.1.4/src/bibiflags.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.102517 bibiflags-0.1.4/src/examples/
--rw-rw-rw-   0        0        0      677 2024-04-12 02:15:49.000000 bibiflags-0.1.4/src/examples/config.py
--rw-rw-rw-   0        0        0      418 2024-04-12 02:15:24.000000 bibiflags-0.1.4/src/examples/config.yaml
--rw-rw-rw-   0        0        0      820 2024-04-11 23:05:14.000000 bibiflags-0.1.4/src/examples/initial.py
--rw-rw-rw-   0        0        0      286 2024-04-11 23:03:50.000000 bibiflags-0.1.4/src/examples/initial.yaml
--rw-rw-rw-   0        0        0      176 2024-04-10 08:13:56.000000 bibiflags-0.1.4/src/examples/main.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.4/src/examples/main.yaml
--rw-rw-rw-   0        0        0      376 2024-04-12 03:10:51.000000 bibiflags-0.1.4/src/examples/prog.py
--rw-rw-rw-   0        0        0        0 2024-04-10 06:01:38.000000 bibiflags-0.1.4/src/examples/prog.yaml
-drwxrwxrwx   0        0        0        0 2024-04-12 03:16:46.104517 bibiflags-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-10 04:59:44.000000 bibiflags-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0      280 2024-04-11 22:15:38.000000 bibiflags-0.1.4/tests/test_bibiflags.py
--rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.4/tests/test_bibiflags.yaml
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.322472 bibiflags-0.1.5/
+-rw-rw-rw-   0        0        0     1067 2021-10-28 05:43:21.000000 bibiflags-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      297 2024-04-10 06:25:01.000000 bibiflags-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3185 2024-04-14 15:05:48.322472 bibiflags-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2607 2024-04-14 15:01:16.000000 bibiflags-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.171850 bibiflags-0.1.5/docs/
+-rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiflags-0.1.5/docs/Makefile
+-rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiflags-0.1.5/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.174850 bibiflags-0.1.5/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.282322 bibiflags-0.1.5/docs/source/_static/
+-rw-rw-rw-   0        0        0    33653 2024-04-10 06:08:59.000000 bibiflags-0.1.5/docs/source/_static/bibiflags.png
+-rw-rw-rw-   0        0        0     6901 2024-04-10 05:06:41.000000 bibiflags-0.1.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiflags-0.1.5/docs/source/install.rst
+-rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiflags-0.1.5/docs/source/quickstart.rst
+-rw-rw-rw-   0        0        0      793 2024-04-14 15:00:58.000000 bibiflags-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:05:48.323485 bibiflags-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.164850 bibiflags-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.286321 bibiflags-0.1.5/src/bibiflags/
+-rw-rw-rw-   0        0        0      104 2024-04-14 15:01:24.000000 bibiflags-0.1.5/src/bibiflags/__init__.py
+-rw-rw-rw-   0        0        0     7204 2024-04-14 15:00:05.000000 bibiflags-0.1.5/src/bibiflags/bibiflags.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.5/src/bibiflags/bibiflags.yaml
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.320482 bibiflags-0.1.5/src/bibiflags.egg-info/
+-rw-rw-rw-   0        0        0     3185 2024-04-14 15:05:48.000000 bibiflags-0.1.5/src/bibiflags.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-04-14 15:05:48.000000 bibiflags-0.1.5/src/bibiflags.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:05:48.000000 bibiflags-0.1.5/src/bibiflags.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 15:05:48.000000 bibiflags-0.1.5/src/bibiflags.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-14 15:05:48.000000 bibiflags-0.1.5/src/bibiflags.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.317472 bibiflags-0.1.5/src/examples/
+-rw-rw-rw-   0        0        0      677 2024-04-12 02:15:49.000000 bibiflags-0.1.5/src/examples/config.py
+-rw-rw-rw-   0        0        0      418 2024-04-14 14:59:03.000000 bibiflags-0.1.5/src/examples/config.yaml
+-rw-rw-rw-   0        0        0      820 2024-04-11 23:05:14.000000 bibiflags-0.1.5/src/examples/initial.py
+-rw-rw-rw-   0        0        0      286 2024-04-11 23:03:50.000000 bibiflags-0.1.5/src/examples/initial.yaml
+-rw-rw-rw-   0        0        0      176 2024-04-10 08:13:56.000000 bibiflags-0.1.5/src/examples/main.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.5/src/examples/main.yaml
+-rw-rw-rw-   0        0        0      376 2024-04-12 03:10:51.000000 bibiflags-0.1.5/src/examples/prog.py
+-rw-rw-rw-   0        0        0      191 2024-04-14 14:59:34.000000 bibiflags-0.1.5/src/examples/prog.yaml
+drwxrwxrwx   0        0        0        0 2024-04-14 15:05:48.319493 bibiflags-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-10 04:59:44.000000 bibiflags-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-04-11 22:15:38.000000 bibiflags-0.1.5/tests/test_bibiflags.py
+-rw-rw-rw-   0        0        0      789 2024-04-10 05:43:04.000000 bibiflags-0.1.5/tests/test_bibiflags.yaml
```

### Comparing `bibiflags-0.1.4/LICENSE` & `bibiflags-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/PKG-INFO` & `bibiflags-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibiflags
-Version: 0.1.4
+Version: 0.1.5
 Summary: Import YAML configs into Arguments for Python
 Author-email: Chunqi SHI <chunqishi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bibiparrot/bibiflags
 Project-URL: Issues, https://github.com/bibiparrot/bibiflags/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -145,8 +145,8 @@
     print(flags.parameters)
 
 
 ```
 
 ## Changelog
 
-### Version 0.1.4 2024-4-12
+### Version 0.1.5 2024-4-14
```

### Comparing `bibiflags-0.1.4/README.md` & `bibiflags-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -129,8 +129,8 @@
     print(flags.parameters)
 
 
 ```
 
 ## Changelog
 
-### Version 0.1.4 2024-4-12
+### Version 0.1.5 2024-4-14
```

### Comparing `bibiflags-0.1.4/docs/Makefile` & `bibiflags-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/docs/source/_static/bibiflags.png` & `bibiflags-0.1.5/docs/source/_static/bibiflags.png`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/docs/source/conf.py` & `bibiflags-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/docs/source/quickstart.rst` & `bibiflags-0.1.5/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/pyproject.toml` & `bibiflags-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bibiflags"
-version = "0.1.4"
+version = "0.1.5"
 description = "Import YAML configs into Arguments for Python"
 authors = [
     {name = "Chunqi SHI", email = "chunqishi@gmail.com"},
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `bibiflags-0.1.4/src/bibiflags/bibiflags.py` & `bibiflags-0.1.5/src/bibiflags/bibiflags.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,15 +122,19 @@
         parser = argparse.ArgumentParser() if parser is None else parser
         for item in items:
             if item.get('type', 'str') == 'bool':
                 item['type'] = None
             else:
                 item['type'] = getattr(builtins, item.get('type', 'str'))
             if item.get('option_strings', None):
-                action = argparse.Action(**item)
+                # action = argparse.Action(**item)
+                if item.get('nargs', None) == 0:
+                    action = argparse.Action(**item)
+                else:
+                    action = argparse._StoreAction(**item)
             else:
                 item['option_strings'] = []
                 if item.get('nargs', 1):
                     action = argparse._StoreAction(**item)
                 else:
                     del item['type'], item['const'], item['nargs']
                     action = argparse._StoreTrueAction(**item)
```

### Comparing `bibiflags-0.1.4/src/bibiflags/bibiflags.yaml` & `bibiflags-0.1.5/src/bibiflags/bibiflags.yaml`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/src/bibiflags.egg-info/PKG-INFO` & `bibiflags-0.1.5/src/bibiflags.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibiflags
-Version: 0.1.4
+Version: 0.1.5
 Summary: Import YAML configs into Arguments for Python
 Author-email: Chunqi SHI <chunqishi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bibiparrot/bibiflags
 Project-URL: Issues, https://github.com/bibiparrot/bibiflags/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -145,8 +145,8 @@
     print(flags.parameters)
 
 
 ```
 
 ## Changelog
 
-### Version 0.1.4 2024-4-12
+### Version 0.1.5 2024-4-14
```

### Comparing `bibiflags-0.1.4/src/bibiflags.egg-info/SOURCES.txt` & `bibiflags-0.1.5/src/bibiflags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/src/examples/config.py` & `bibiflags-0.1.5/src/examples/config.py`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/src/examples/initial.py` & `bibiflags-0.1.5/src/examples/initial.py`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/src/examples/main.yaml` & `bibiflags-0.1.5/src/examples/main.yaml`

 * *Files identical despite different names*

### Comparing `bibiflags-0.1.4/tests/test_bibiflags.yaml` & `bibiflags-0.1.5/tests/test_bibiflags.yaml`

 * *Files identical despite different names*

