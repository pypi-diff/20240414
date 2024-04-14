# Comparing `tmp/cornsnake-0.0.8.tar.gz` & `tmp/cornsnake-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornsnake-0.0.8.tar", last modified: Sun Jan 14 13:22:34 2024, max compression
+gzip compressed data, was "cornsnake-0.0.9.tar", last modified: Sun Jan 14 13:24:50 2024, max compression
```

## Comparing `cornsnake-0.0.8.tar` & `cornsnake-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-01-14 13:22:34.447352 cornsnake-0.0.8/
--rw-rw-rw-   0        0        0     1066 2024-01-14 10:30:12.000000 cornsnake-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     2615 2024-01-14 13:22:34.446336 cornsnake-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      638 2024-01-14 13:06:24.000000 cornsnake-0.0.8/README.md
--rw-rw-rw-   0        0        0     1286 2024-01-14 13:22:20.000000 cornsnake-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-14 13:22:34.447352 cornsnake-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-14 13:22:34.307341 cornsnake-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-01-14 13:22:34.415277 cornsnake-0.0.8/src/cornsnake/
--rw-rw-rw-   0        0        0      606 2024-01-14 13:22:20.000000 cornsnake-0.0.8/src/cornsnake/__init__.py
--rw-rw-rw-   0        0        0      746 2024-01-14 11:38:25.000000 cornsnake-0.0.8/src/cornsnake/config.py
--rw-rw-rw-   0        0        0       39 2024-01-14 10:53:17.000000 cornsnake-0.0.8/src/cornsnake/setup.py
--rw-rw-rw-   0        0        0     3984 2024-01-14 11:15:42.000000 cornsnake-0.0.8/src/cornsnake/test_util_list.py
--rw-rw-rw-   0        0        0      622 2024-01-14 11:16:08.000000 cornsnake-0.0.8/src/cornsnake/test_util_string.py
--rw-rw-rw-   0        0        0      482 2024-01-14 13:21:03.000000 cornsnake-0.0.8/src/cornsnake/util_color.py
--rw-rw-rw-   0        0        0      259 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_date.py
--rw-rw-rw-   0        0        0     1498 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_dependencies.py
--rw-rw-rw-   0        0        0     1460 2024-01-14 10:30:41.000000 cornsnake-0.0.8/src/cornsnake/util_dir.py
--rw-rw-rw-   0        0        0     1411 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_file.py
--rw-rw-rw-   0        0        0     4349 2024-01-14 13:21:24.000000 cornsnake-0.0.8/src/cornsnake/util_git.py
--rw-rw-rw-   0        0        0     3490 2024-01-14 13:21:24.000000 cornsnake-0.0.8/src/cornsnake/util_input.py
--rw-rw-rw-   0        0        0      299 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_json.py
--rw-rw-rw-   0        0        0     1110 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_list.py
--rw-rw-rw-   0        0        0      912 2024-01-14 13:21:24.000000 cornsnake-0.0.8/src/cornsnake/util_log.py
--rw-rw-rw-   0        0        0      447 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_markdown_table.py
--rw-rw-rw-   0        0        0       60 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_os.py
--rw-rw-rw-   0        0        0      258 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_pdf.py
--rw-rw-rw-   0        0        0      333 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_pick.py
--rw-rw-rw-   0        0        0     1699 2024-01-14 13:21:24.000000 cornsnake-0.0.8/src/cornsnake/util_proc.py
--rw-rw-rw-   0        0        0      896 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_progress.py
--rw-rw-rw-   0        0        0     1762 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_robust_delete.py
--rw-rw-rw-   0        0        0      134 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_string.py
--rw-rw-rw-   0        0        0       16 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_text.py
--rw-rw-rw-   0        0        0      358 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_time.py
--rw-rw-rw-   0        0        0     3929 2024-01-14 13:21:24.000000 cornsnake-0.0.8/src/cornsnake/util_validate.py
--rw-rw-rw-   0        0        0      104 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/util_wait.py
--rw-rw-rw-   0        0        0      574 2024-01-14 10:30:12.000000 cornsnake-0.0.8/src/cornsnake/zip_dir.py
-drwxrwxrwx   0        0        0        0 2024-01-14 13:22:34.444334 cornsnake-0.0.8/src/cornsnake.egg-info/
--rw-rw-rw-   0        0        0     2615 2024-01-14 13:22:34.000000 cornsnake-0.0.8/src/cornsnake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2024-01-14 13:22:34.000000 cornsnake-0.0.8/src/cornsnake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-14 13:22:34.000000 cornsnake-0.0.8/src/cornsnake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-01-14 13:22:34.000000 cornsnake-0.0.8/src/cornsnake.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-14 13:22:34.000000 cornsnake-0.0.8/src/cornsnake.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-14 13:24:50.880715 cornsnake-0.0.9/
+-rw-rw-rw-   0        0        0     1066 2024-01-14 10:30:12.000000 cornsnake-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2615 2024-01-14 13:24:50.878606 cornsnake-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2024-01-14 13:06:24.000000 cornsnake-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1286 2024-01-14 13:24:37.000000 cornsnake-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-01-14 13:24:50.880715 cornsnake-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-01-14 13:24:50.806995 cornsnake-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-01-14 13:24:50.853838 cornsnake-0.0.9/src/cornsnake/
+-rw-rw-rw-   0        0        0      606 2024-01-14 13:24:37.000000 cornsnake-0.0.9/src/cornsnake/__init__.py
+-rw-rw-rw-   0        0        0      746 2024-01-14 11:38:25.000000 cornsnake-0.0.9/src/cornsnake/config.py
+-rw-rw-rw-   0        0        0       39 2024-01-14 10:53:17.000000 cornsnake-0.0.9/src/cornsnake/setup.py
+-rw-rw-rw-   0        0        0     3984 2024-01-14 11:15:42.000000 cornsnake-0.0.9/src/cornsnake/test_util_list.py
+-rw-rw-rw-   0        0        0      622 2024-01-14 11:16:08.000000 cornsnake-0.0.9/src/cornsnake/test_util_string.py
+-rw-rw-rw-   0        0        0      489 2024-01-14 13:24:08.000000 cornsnake-0.0.9/src/cornsnake/util_color.py
+-rw-rw-rw-   0        0        0      259 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_date.py
+-rw-rw-rw-   0        0        0     1498 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_dependencies.py
+-rw-rw-rw-   0        0        0     1460 2024-01-14 10:30:41.000000 cornsnake-0.0.9/src/cornsnake/util_dir.py
+-rw-rw-rw-   0        0        0     1411 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_file.py
+-rw-rw-rw-   0        0        0     4349 2024-01-14 13:21:24.000000 cornsnake-0.0.9/src/cornsnake/util_git.py
+-rw-rw-rw-   0        0        0     3490 2024-01-14 13:21:24.000000 cornsnake-0.0.9/src/cornsnake/util_input.py
+-rw-rw-rw-   0        0        0      299 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_json.py
+-rw-rw-rw-   0        0        0     1110 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_list.py
+-rw-rw-rw-   0        0        0      912 2024-01-14 13:21:24.000000 cornsnake-0.0.9/src/cornsnake/util_log.py
+-rw-rw-rw-   0        0        0      447 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_markdown_table.py
+-rw-rw-rw-   0        0        0       60 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_os.py
+-rw-rw-rw-   0        0        0      258 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_pdf.py
+-rw-rw-rw-   0        0        0      333 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_pick.py
+-rw-rw-rw-   0        0        0     1699 2024-01-14 13:21:24.000000 cornsnake-0.0.9/src/cornsnake/util_proc.py
+-rw-rw-rw-   0        0        0      896 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_progress.py
+-rw-rw-rw-   0        0        0     1762 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_robust_delete.py
+-rw-rw-rw-   0        0        0      134 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_string.py
+-rw-rw-rw-   0        0        0       16 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_text.py
+-rw-rw-rw-   0        0        0      358 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_time.py
+-rw-rw-rw-   0        0        0     3929 2024-01-14 13:21:24.000000 cornsnake-0.0.9/src/cornsnake/util_validate.py
+-rw-rw-rw-   0        0        0      104 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/util_wait.py
+-rw-rw-rw-   0        0        0      574 2024-01-14 10:30:12.000000 cornsnake-0.0.9/src/cornsnake/zip_dir.py
+drwxrwxrwx   0        0        0        0 2024-01-14 13:24:50.877606 cornsnake-0.0.9/src/cornsnake.egg-info/
+-rw-rw-rw-   0        0        0     2615 2024-01-14 13:24:50.000000 cornsnake-0.0.9/src/cornsnake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2024-01-14 13:24:50.000000 cornsnake-0.0.9/src/cornsnake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-14 13:24:50.000000 cornsnake-0.0.9/src/cornsnake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-01-14 13:24:50.000000 cornsnake-0.0.9/src/cornsnake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-01-14 13:24:50.000000 cornsnake-0.0.9/src/cornsnake.egg-info/top_level.txt
```

### Comparing `cornsnake-0.0.8/LICENSE` & `cornsnake-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/PKG-INFO` & `cornsnake-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornsnake
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrap common Python utilities for working with files, lists, processes, dates and times.
 Author-email: Sean Ryan <mr.sean.ryan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sean Ryan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cornsnake-0.0.8/README.md` & `cornsnake-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/pyproject.toml` & `cornsnake-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cornsnake"
-version = "0.0.8"
+version = "0.0.9"
 description = "Wrap common Python utilities for working with files, lists, processes, dates and times."
 readme = "README.md"
 authors = [{ name = "Sean Ryan", email = "mr.sean.ryan@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,15 +23,15 @@
 [project.optional-dependencies]
 dev = ["bumpver", "parameterized"]
 
 [project.urls]
 Homepage = "https://github.com/mrseanryan/cornsnake"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `cornsnake-0.0.8/src/cornsnake/__init__.py` & `cornsnake-0.0.9/src/cornsnake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 from . import util_color
 from . import util_dependencies
 from . import util_dir
 from . import util_file
 from . import util_git
 from . import util_input
```

### Comparing `cornsnake-0.0.8/src/cornsnake/config.py` & `cornsnake-0.0.9/src/cornsnake/config.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/test_util_list.py` & `cornsnake-0.0.9/src/cornsnake/test_util_list.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/test_util_string.py` & `cornsnake-0.0.9/src/cornsnake/test_util_string.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_dependencies.py` & `cornsnake-0.0.9/src/cornsnake/util_dependencies.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_dir.py` & `cornsnake-0.0.9/src/cornsnake/util_dir.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_file.py` & `cornsnake-0.0.9/src/cornsnake/util_file.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_git.py` & `cornsnake-0.0.9/src/cornsnake/util_git.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_input.py` & `cornsnake-0.0.9/src/cornsnake/util_input.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_list.py` & `cornsnake-0.0.9/src/cornsnake/util_list.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_log.py` & `cornsnake-0.0.9/src/cornsnake/util_log.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_proc.py` & `cornsnake-0.0.9/src/cornsnake/util_proc.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_progress.py` & `cornsnake-0.0.9/src/cornsnake/util_progress.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_robust_delete.py` & `cornsnake-0.0.9/src/cornsnake/util_robust_delete.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/util_validate.py` & `cornsnake-0.0.9/src/cornsnake/util_validate.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake/zip_dir.py` & `cornsnake-0.0.9/src/cornsnake/zip_dir.py`

 * *Files identical despite different names*

### Comparing `cornsnake-0.0.8/src/cornsnake.egg-info/PKG-INFO` & `cornsnake-0.0.9/src/cornsnake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornsnake
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrap common Python utilities for working with files, lists, processes, dates and times.
 Author-email: Sean Ryan <mr.sean.ryan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sean Ryan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cornsnake-0.0.8/src/cornsnake.egg-info/SOURCES.txt` & `cornsnake-0.0.9/src/cornsnake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

