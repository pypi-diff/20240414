# Comparing `tmp/stabilizer_timelime-0.0.8.tar.gz` & `tmp/stabilizer_timelime-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilizer_timelime-0.0.8.tar", max compression
+gzip compressed data, was "stabilizer_timelime-0.0.9.tar", max compression
```

## Comparing `stabilizer_timelime-0.0.8.tar` & `stabilizer_timelime-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.0.8/LICENSE
--rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.0.8/README.md
--rw-r--r--   0        0        0      630 2024-04-11 20:14:48.439021 stabilizer_timelime-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 18:41:51.440222 stabilizer_timelime-0.0.8/stabilizer_timelime/src/__init__.py
--rw-r--r--   0        0        0     7378 2024-04-11 20:14:15.355834 stabilizer_timelime-0.0.8/stabilizer_timelime/src/slurpdata.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 stabilizer_timelime-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.0.9/LICENSE
+-rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.0.9/README.md
+-rw-r--r--   0        0        0      648 2024-04-11 20:16:44.430968 stabilizer_timelime-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 18:41:51.440222 stabilizer_timelime-0.0.9/stabilizer_timelime/src/__init__.py
+-rw-r--r--   0        0        0     7378 2024-04-11 20:14:15.355834 stabilizer_timelime-0.0.9/stabilizer_timelime/src/slurpdata.py
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 stabilizer_timelime-0.0.9/PKG-INFO
```

### Comparing `stabilizer_timelime-0.0.8/LICENSE` & `stabilizer_timelime-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.0.8/pyproject.toml` & `stabilizer_timelime-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "stabilizer_timelime"
-version = "0.0.8"
+version = "0.0.9"
 authors = ["Sukhad Joshi <sjoshi32@ncsu.edu>"]
 description = "Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 readme = "README.md"
-dependencies = {python = "^3.7", python-dateutil = "^2.9.0", pillow = "^10.2.0", pandas = "^1.3.5", PyGithub = "^2.2.0"}
+dependencies = {python = "^3.7", python-dateutil = "^2.9.0", pillow = "^10.2.0", pandas = "^1.3.5", PyGithub = "^2.2.0", tqdm = "^4.66.2"}
```

### Comparing `stabilizer_timelime-0.0.8/stabilizer_timelime/src/slurpdata.py` & `stabilizer_timelime-0.0.9/stabilizer_timelime/src/slurpdata.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.0.8/PKG-INFO` & `stabilizer_timelime-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilizer_timelime
-Version: 0.0.8
+Version: 0.0.9
 Summary: Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline
 Author: Sukhad Joshi
 Author-email: sjoshi32@ncsu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -14,10 +14,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyGithub (>=2.2.0,<3.0.0)
 Requires-Dist: pandas (>=1.3.5,<2.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # STABILIZER + TIMELIME
```

