# Comparing `tmp/packaging-demo-hubzar-1.0.2.tar.gz` & `tmp/packaging_demo_hubzar-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging-demo-hubzar-1.0.2.tar", last modified: Sat Mar 30 09:41:46 2024, max compression
+gzip compressed data, was "packaging_demo_hubzar-1.1.0.tar", last modified: Sun Apr 14 15:30:30 2024, max compression
```

## Comparing `packaging-demo-hubzar-1.0.2.tar` & `packaging_demo_hubzar-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:41:46.694308 packaging-demo-hubzar-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-30 09:41:46.690308 packaging-demo-hubzar-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:41:46.690308 packaging-demo-hubzar-1.0.2/packaging_demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/colorized_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/my_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:41:46.690308 packaging-demo-hubzar-1.0.2/packaging_demo/my_folder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/my_folder/cities.json
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/my_folder/my_nested_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:41:46.690308 packaging-demo-hubzar-1.0.2/packaging_demo/my_folder/sub_package/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/my_folder/sub_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/my_folder/sub_package/some_deeply_netsed_file.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/my_other_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/packaging_demo/states_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:41:46.690308 packaging-demo-hubzar-1.0.2/packaging_demo_hubzar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-30 09:41:46.000000 packaging-demo-hubzar-1.0.2/packaging_demo_hubzar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-30 09:41:46.000000 packaging-demo-hubzar-1.0.2/packaging_demo_hubzar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 09:41:46.000000 packaging-demo-hubzar-1.0.2/packaging_demo_hubzar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-30 09:41:46.000000 packaging-demo-hubzar-1.0.2/packaging_demo_hubzar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 09:41:46.000000 packaging-demo-hubzar-1.0.2/packaging_demo_hubzar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 09:41:46.694308 packaging-demo-hubzar-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-30 09:41:41.000000 packaging-demo-hubzar-1.0.2/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:30:30.659265 packaging_demo_hubzar-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-14 15:30:30.659265 packaging_demo_hubzar-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:30:30.655265 packaging_demo_hubzar-1.1.0/packaging_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/packaging_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/packaging_demo/colorized_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/packaging_demo/my_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/packaging_demo/my_other_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/packaging_demo/slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/packaging_demo/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:30:30.655265 packaging_demo_hubzar-1.1.0/packaging_demo_hubzar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-14 15:30:30.000000 packaging_demo_hubzar-1.1.0/packaging_demo_hubzar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 15:30:30.000000 packaging_demo_hubzar-1.1.0/packaging_demo_hubzar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:30:30.000000 packaging_demo_hubzar-1.1.0/packaging_demo_hubzar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-14 15:30:30.000000 packaging_demo_hubzar-1.1.0/packaging_demo_hubzar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 15:30:30.000000 packaging_demo_hubzar-1.1.0/packaging_demo_hubzar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:30:30.659265 packaging_demo_hubzar-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:30:30.655265 packaging_demo_hubzar-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/tests/test_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/tests/test_states_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 15:30:26.000000 packaging_demo_hubzar-1.1.0/version.txt
```

### Comparing `packaging-demo-hubzar-1.0.2/PKG-INFO` & `packaging_demo_hubzar-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-hubzar
-Version: 1.0.2
+Version: 1.1.0
 Summary: My package description
 Author-email: HubZar <your_email@example.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `packaging-demo-hubzar-1.0.2/packaging_demo_hubzar.egg-info/PKG-INFO` & `packaging_demo_hubzar-1.1.0/packaging_demo_hubzar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-hubzar
-Version: 1.0.2
+Version: 1.1.0
 Summary: My package description
 Author-email: HubZar <your_email@example.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `packaging-demo-hubzar-1.0.2/pyproject.toml` & `packaging_demo_hubzar-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+packages = ["packaging_demo"]
+
 [tool.setuptools.package-data]
 "packaging_demo.my_folder" = ["*.json"]
 
 [project]
 name = "packaging-demo-hubzar"
 authors = [{ name = "HubZar", email = "your_email@example.com" }]
 description = "My package description"
@@ -38,16 +41,19 @@
 exclude = "venv"
 
 [tool.ruff]
 # 1. Enable flake8-bugbear (`B`) rules, in addition to the defaults.
 lint.select = ["E4", "E7", "E9", "F", "B", "ERA"]
 
 # 2. Avoid enforcing line-length violations (`E501`)
-lint.ignore = ["E501", 'F401']
+lint.ignore = ["E501", 'F401', "ERA001"]
 
 # 3. Avoid trying to fix flake8-bugbear (`B`) violations.
 lint.unfixable = ["B"]
 
 # 4. Ignore `E402` (import violations) in all `__init__.py` files, and in select subdirectories.
 [tool.lint.per-file-ignores]
 "__init__.py" = ["E402"]
 "**/{tests,docs,tools}/*" = ["E402"]
+
+[tool.pytest.ini_options]
+markers = ["slow: marks tests as slow (deselect with '-m \"not slow\"')"]
```

