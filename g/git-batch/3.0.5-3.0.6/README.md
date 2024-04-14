# Comparing `tmp/git_batch-3.0.5.tar.gz` & `tmp/git_batch-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_batch-3.0.5.tar", max compression
+gzip compressed data, was "git_batch-3.0.6.tar", max compression
```

## Comparing `git_batch-3.0.5.tar` & `git_batch-3.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1123 2024-03-02 13:55:13.138630 git_batch-3.0.5/LICENSE
--rw-r--r--   0        0        0     1731 2024-03-02 13:55:13.138630 git_batch-3.0.5/README.md
--rw-r--r--   0        0        0       46 2024-03-02 13:55:31.466552 git_batch-3.0.5/gitbatch/__init__.py
--rw-r--r--   0        0        0     6481 2024-03-02 13:55:13.138630 git_batch-3.0.5/gitbatch/cli.py
--rw-r--r--   0        0        0     5712 2024-03-02 13:55:13.138630 git_batch-3.0.5/gitbatch/logging.py
--rw-r--r--   0        0        0     1023 2024-03-02 13:55:13.138630 git_batch-3.0.5/gitbatch/utils/__init__.py
--rw-r--r--   0        0        0     5768 2024-03-02 13:55:13.138630 git_batch-3.0.5/gitbatch/utils/copy.py
--rw-r--r--   0        0        0     2858 2024-03-02 13:55:31.466552 git_batch-3.0.5/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 git_batch-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1123 2024-04-14 09:47:45.672670 git_batch-3.0.6/LICENSE
+-rw-r--r--   0        0        0     1731 2024-04-14 09:47:45.672670 git_batch-3.0.6/README.md
+-rw-r--r--   0        0        0       46 2024-04-14 09:48:10.220682 git_batch-3.0.6/gitbatch/__init__.py
+-rw-r--r--   0        0        0     6481 2024-04-14 09:47:45.672670 git_batch-3.0.6/gitbatch/cli.py
+-rw-r--r--   0        0        0     5712 2024-04-14 09:47:45.672670 git_batch-3.0.6/gitbatch/logging.py
+-rw-r--r--   0        0        0     1023 2024-04-14 09:47:45.672670 git_batch-3.0.6/gitbatch/utils/__init__.py
+-rw-r--r--   0        0        0     5768 2024-04-14 09:47:45.672670 git_batch-3.0.6/gitbatch/utils/copy.py
+-rw-r--r--   0        0        0     2858 2024-04-14 09:48:10.216683 git_batch-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 git_batch-3.0.6/PKG-INFO
```

### Comparing `git_batch-3.0.5/LICENSE` & `git_batch-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `git_batch-3.0.5/README.md` & `git_batch-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `git_batch-3.0.5/gitbatch/cli.py` & `git_batch-3.0.6/gitbatch/cli.py`

 * *Files identical despite different names*

### Comparing `git_batch-3.0.5/gitbatch/logging.py` & `git_batch-3.0.6/gitbatch/logging.py`

 * *Files identical despite different names*

### Comparing `git_batch-3.0.5/gitbatch/utils/__init__.py` & `git_batch-3.0.6/gitbatch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `git_batch-3.0.5/gitbatch/utils/copy.py` & `git_batch-3.0.6/gitbatch/utils/copy.py`

 * *Files identical despite different names*

### Comparing `git_batch-3.0.5/pyproject.toml` & `git_batch-3.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 include = ["LICENSE"]
 keywords = ["git", "batch", "automation"]
 license = "MIT"
 name = "git-batch"
 packages = [{ include = "gitbatch" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/git-batch/"
-version = "3.0.5"
+version = "3.0.6"
 
 [tool.poetry.dependencies]
-GitPython = "3.1.42"
+GitPython = "3.1.43"
 colorama = "0.4.6"
 python = "^3.8.0"
 python-json-logger = "2.0.7"
 
 [tool.poetry.scripts]
 git-batch = "gitbatch.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.2.2"
-pytest = "8.0.2"
-pytest-mock = "3.12.0"
-pytest-cov = "4.1.0"
+ruff = "0.3.5"
+pytest = "8.1.1"
+pytest-mock = "3.14.0"
+pytest-cov = "5.0.0"
 toml = "0.10.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
```

### Comparing `git_batch-3.0.5/PKG-INFO` & `git_batch-3.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-batch
-Version: 3.0.5
+Version: 3.0.6
 Summary: Clone single branch from all repositories listed in a file.
 Home-page: https://github.com/thegeeklab/git-batch/
 License: MIT
 Keywords: git,batch,automation
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.8.0,<4.0.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Dist: GitPython (==3.1.42)
+Requires-Dist: GitPython (==3.1.43)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: python-json-logger (==2.0.7)
 Project-URL: Documentation, https://github.com/thegeeklab/git-batch/
 Project-URL: Repository, https://github.com/thegeeklab/git-batch/
 Description-Content-Type: text/markdown
 
 # git-batch
```

