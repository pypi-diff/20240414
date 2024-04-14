# Comparing `tmp/sqlite-shift-0.1.0.tar.gz` & `tmp/sqlite-shift-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/akarshts/personal/sqlite-shift/dist/tmppz812_t5/sqlite-shift-0.1.0.tar", last modified: Sun Apr 14 13:48:27 2024, max compression
+gzip compressed data, was "/Users/akarshts/personal/sqlite-shift/dist/tmpahfguxvn/sqlite-shift-0.1.1.tar", last modified: Sun Apr 14 14:35:46 2024, max compression
```

## Comparing `sqlite-shift-0.1.0.tar` & `sqlite-shift-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/
-drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/sqlite_shift.egg-info/
--rw-r--r--   0 akarshts   (501) staff       (20)     6551 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/sqlite_shift.egg-info/PKG-INFO
--rw-r--r--   0 akarshts   (501) staff       (20)      505 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/sqlite_shift.egg-info/SOURCES.txt
--rw-r--r--   0 akarshts   (501) staff       (20)       56 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/sqlite_shift.egg-info/entry_points.txt
--rw-r--r--   0 akarshts   (501) staff       (20)       19 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/sqlite_shift.egg-info/top_level.txt
--rw-r--r--   0 akarshts   (501) staff       (20)        1 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/sqlite_shift.egg-info/dependency_links.txt
--rw-r--r--   0 akarshts   (501) staff       (20)     6551 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/PKG-INFO
-drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/sqlite_shift/
--rw-r--r--   0 akarshts   (501) staff       (20)      500 2024-04-14 08:24:17.000000 sqlite-shift-0.1.0/sqlite_shift/base_migration.py
--rw-r--r--   0 akarshts   (501) staff       (20)        1 2024-04-14 13:46:46.000000 sqlite-shift-0.1.0/sqlite_shift/__init__.py
--rw-r--r--   0 akarshts   (501) staff       (20)     1359 2024-04-14 08:24:09.000000 sqlite-shift-0.1.0/sqlite_shift/main.py
--rw-r--r--   0 akarshts   (501) staff       (20)    10511 2024-04-14 09:44:01.000000 sqlite-shift-0.1.0/sqlite_shift/manager.py
--rw-r--r--   0 akarshts   (501) staff       (20)    11357 2024-04-09 03:53:29.000000 sqlite-shift-0.1.0/LICENSE
--rw-r--r--   0 akarshts   (501) staff       (20)      635 2024-04-14 13:45:32.000000 sqlite-shift-0.1.0/pyproject.toml
-drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/tests/
--rw-r--r--   0 akarshts   (501) staff       (20)      907 2024-04-14 09:28:11.000000 sqlite-shift-0.1.0/tests/conftest.py
-drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/tests/schema_migrations/
--rw-r--r--   0 akarshts   (501) staff       (20)      445 2024-04-14 09:44:32.000000 sqlite-shift-0.1.0/tests/schema_migrations/002_add_foriegn_key.py
--rw-r--r--   0 akarshts   (501) staff       (20)        0 2024-04-09 07:43:10.000000 sqlite-shift-0.1.0/tests/schema_migrations/__init__.py
--rw-r--r--   0 akarshts   (501) staff       (20)      593 2024-04-14 09:44:23.000000 sqlite-shift-0.1.0/tests/schema_migrations/001_initial.py
--rw-r--r--   0 akarshts   (501) staff       (20)        0 2024-04-09 07:36:28.000000 sqlite-shift-0.1.0/tests/__init__.py
--rw-r--r--   0 akarshts   (501) staff       (20)     1344 2024-04-14 09:45:27.000000 sqlite-shift-0.1.0/tests/test_manager.py
--rw-r--r--   0 akarshts   (501) staff       (20)     6004 2024-04-14 13:17:26.000000 sqlite-shift-0.1.0/README.md
--rw-r--r--   0 akarshts   (501) staff       (20)      867 2024-04-14 13:46:28.000000 sqlite-shift-0.1.0/setup.py
--rw-r--r--   0 akarshts   (501) staff       (20)       38 2024-04-14 13:48:27.000000 sqlite-shift-0.1.0/setup.cfg
+drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/
+drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/sqlite_shift.egg-info/
+-rw-r--r--   0 akarshts   (501) staff       (20)     6551 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/sqlite_shift.egg-info/PKG-INFO
+-rw-r--r--   0 akarshts   (501) staff       (20)      505 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/sqlite_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 akarshts   (501) staff       (20)       56 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/sqlite_shift.egg-info/entry_points.txt
+-rw-r--r--   0 akarshts   (501) staff       (20)       19 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/sqlite_shift.egg-info/top_level.txt
+-rw-r--r--   0 akarshts   (501) staff       (20)        1 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/sqlite_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 akarshts   (501) staff       (20)     6551 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/PKG-INFO
+drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/sqlite_shift/
+-rw-r--r--   0 akarshts   (501) staff       (20)      500 2024-04-14 08:24:17.000000 sqlite-shift-0.1.1/sqlite_shift/base_migration.py
+-rw-r--r--   0 akarshts   (501) staff       (20)        1 2024-04-14 13:46:46.000000 sqlite-shift-0.1.1/sqlite_shift/__init__.py
+-rw-r--r--   0 akarshts   (501) staff       (20)     1359 2024-04-14 08:24:09.000000 sqlite-shift-0.1.1/sqlite_shift/main.py
+-rw-r--r--   0 akarshts   (501) staff       (20)    10511 2024-04-14 09:44:01.000000 sqlite-shift-0.1.1/sqlite_shift/manager.py
+-rw-r--r--   0 akarshts   (501) staff       (20)    11357 2024-04-09 03:53:29.000000 sqlite-shift-0.1.1/LICENSE
+-rw-r--r--   0 akarshts   (501) staff       (20)      805 2024-04-14 14:33:41.000000 sqlite-shift-0.1.1/pyproject.toml
+drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/tests/
+-rw-r--r--   0 akarshts   (501) staff       (20)      907 2024-04-14 09:28:11.000000 sqlite-shift-0.1.1/tests/conftest.py
+drwxr-xr-x   0 akarshts   (501) staff       (20)        0 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/tests/schema_migrations/
+-rw-r--r--   0 akarshts   (501) staff       (20)      445 2024-04-14 09:44:32.000000 sqlite-shift-0.1.1/tests/schema_migrations/002_add_foriegn_key.py
+-rw-r--r--   0 akarshts   (501) staff       (20)        0 2024-04-09 07:43:10.000000 sqlite-shift-0.1.1/tests/schema_migrations/__init__.py
+-rw-r--r--   0 akarshts   (501) staff       (20)      593 2024-04-14 09:44:23.000000 sqlite-shift-0.1.1/tests/schema_migrations/001_initial.py
+-rw-r--r--   0 akarshts   (501) staff       (20)        0 2024-04-09 07:36:28.000000 sqlite-shift-0.1.1/tests/__init__.py
+-rw-r--r--   0 akarshts   (501) staff       (20)     1344 2024-04-14 09:45:27.000000 sqlite-shift-0.1.1/tests/test_manager.py
+-rw-r--r--   0 akarshts   (501) staff       (20)     6004 2024-04-14 13:17:26.000000 sqlite-shift-0.1.1/README.md
+-rw-r--r--   0 akarshts   (501) staff       (20)      867 2024-04-14 14:35:35.000000 sqlite-shift-0.1.1/setup.py
+-rw-r--r--   0 akarshts   (501) staff       (20)       38 2024-04-14 14:35:46.000000 sqlite-shift-0.1.1/setup.cfg
```

### Comparing `sqlite-shift-0.1.0/sqlite_shift.egg-info/PKG-INFO` & `sqlite-shift-0.1.1/sqlite_shift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-shift
-Version: 0.1.0
+Version: 0.1.1
 Summary: A streamlined framework for managing SQLite database migrations, inspired by Django.
 Home-page: https://github.com/Akarsh-TS/sqlite-shift
 Author: Your Name
 Author-email: ts.akarsh@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlite-shift-0.1.0/PKG-INFO` & `sqlite-shift-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-shift
-Version: 0.1.0
+Version: 0.1.1
 Summary: A streamlined framework for managing SQLite database migrations, inspired by Django.
 Home-page: https://github.com/Akarsh-TS/sqlite-shift
 Author: Your Name
 Author-email: ts.akarsh@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlite-shift-0.1.0/sqlite_shift/main.py` & `sqlite-shift-0.1.1/sqlite_shift/main.py`

 * *Files identical despite different names*

### Comparing `sqlite-shift-0.1.0/sqlite_shift/manager.py` & `sqlite-shift-0.1.1/sqlite_shift/manager.py`

 * *Files identical despite different names*

### Comparing `sqlite-shift-0.1.0/LICENSE` & `sqlite-shift-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite-shift-0.1.0/pyproject.toml` & `sqlite-shift-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [project]
 name = "sqlite-shift"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Akarsh T S", email="ts.akarsh@gmail.com" },
 ]
 description = "sqlite-shift is a streamlined framework for managing SQLite database migrations, inspired by Django's methodology."
 readme = "README.md"
 requires-python = ">=3.8"
+keywords = ["sqlite migrations","sqlite migrate", "sqllite", "sql", "migrate", "migrations"]
 classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Akarsh-TS/sqlite-shift"
```

### Comparing `sqlite-shift-0.1.0/tests/conftest.py` & `sqlite-shift-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlite-shift-0.1.0/tests/schema_migrations/001_initial.py` & `sqlite-shift-0.1.1/tests/schema_migrations/001_initial.py`

 * *Files identical despite different names*

### Comparing `sqlite-shift-0.1.0/tests/test_manager.py` & `sqlite-shift-0.1.1/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `sqlite-shift-0.1.0/README.md` & `sqlite-shift-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlite-shift-0.1.0/setup.py` & `sqlite-shift-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sqlite-shift",
-    version="0.1.0",
+    version="0.1.1",
     author="Your Name",
     author_email="ts.akarsh@gmail.com",
     description="A streamlined framework for managing SQLite database migrations, inspired by Django.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Akarsh-TS/sqlite-shift",
     license="Apache License 2.0",  # Specify the license here
```

