# Comparing `tmp/icodes-0.1.1.tar.gz` & `tmp/icodes-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icodes-0.1.1.tar", max compression
+gzip compressed data, was "icodes-0.1.2.tar", max compression
```

## Comparing `icodes-0.1.1.tar` & `icodes-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7048 2024-03-31 18:37:25.121754 icodes-0.1.1/LICENSE
--rw-r--r--   0        0        0     2883 2024-04-14 10:21:32.481639 icodes-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-06 19:55:00.301396 icodes-0.1.1/icds/__init__.py
--rw-r--r--   0        0        0     1935 2024-04-14 09:52:58.273822 icodes-0.1.1/icds/data.py
--rw-r--r--   0        0        0     1285 2024-04-14 09:43:58.775498 icodes-0.1.1/icds/git_helpers.py
--rw-r--r--   0        0        0     3124 2024-04-06 19:55:00.301396 icodes-0.1.1/icds/llm_interface.py
--rw-r--r--   0        0        0      797 2024-04-14 09:43:58.775498 icodes-0.1.1/icds/models.py
--rw-r--r--   0        0        0      241 2024-04-06 19:55:00.301396 icodes-0.1.1/icds/settings.py
--rw-r--r--   0        0        0     4495 2024-04-14 09:52:31.214089 icodes-0.1.1/icodes.py
--rw-r--r--   0        0        0     1145 2024-04-14 11:23:28.352088 icodes-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 icodes-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7048 2024-03-31 18:37:25.121754 icodes-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2883 2024-04-14 10:21:32.481639 icodes-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 19:55:00.301396 icodes-0.1.2/icds/__init__.py
+-rw-r--r--   0        0        0     1935 2024-04-14 09:52:58.273822 icodes-0.1.2/icds/data.py
+-rw-r--r--   0        0        0     1285 2024-04-14 09:43:58.775498 icodes-0.1.2/icds/git_helpers.py
+-rw-r--r--   0        0        0     3124 2024-04-06 19:55:00.301396 icodes-0.1.2/icds/llm_interface.py
+-rw-r--r--   0        0        0      797 2024-04-14 09:43:58.775498 icodes-0.1.2/icds/models.py
+-rw-r--r--   0        0        0      241 2024-04-06 19:55:00.301396 icodes-0.1.2/icds/settings.py
+-rw-r--r--   0        0        0     4520 2024-04-14 11:28:48.808145 icodes-0.1.2/icodes.py
+-rw-r--r--   0        0        0     1145 2024-04-14 11:29:22.631732 icodes-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 icodes-0.1.2/PKG-INFO
```

### Comparing `icodes-0.1.1/LICENSE` & `icodes-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icodes-0.1.1/README.md` & `icodes-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `icodes-0.1.1/icds/data.py` & `icodes-0.1.2/icds/data.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.1/icds/git_helpers.py` & `icodes-0.1.2/icds/git_helpers.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.1/icds/llm_interface.py` & `icodes-0.1.2/icds/llm_interface.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.1/icds/models.py` & `icodes-0.1.2/icds/models.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.1/icodes.py` & `icodes-0.1.2/icodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,10 +119,14 @@
             echo(f"Author: {commit.author}")
             echo(f"Date: {commit.datetime}")
             echo(f"Summary: {commit.summary}")
             echo(f"Details: {commit.details}")
             echo("\n")
 
 
-if __name__ == "__main__":
+def main():
     create_db_and_tables()
     app()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `icodes-0.1.1/pyproject.toml` & `icodes-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "icodes"
-version = "0.1.1"
+version = "0.1.2"
 description = "LLM-powered Git archeology tool (a.k.a. Intelligent Commit Ontology Distiller and Enhanced Search)"
 authors = ["Jordan Dimov <jdimov@a115.co.uk>", "Bayo Ade <bayo.300@gmail.com>"]
 license = "CC0-1.0"
 readme = "README.md"
 packages = [
     { include = "icodes.py" },
     { include = "icds/**/*.py" },
```

### Comparing `icodes-0.1.1/PKG-INFO` & `icodes-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icodes
-Version: 0.1.1
+Version: 0.1.2
 Summary: LLM-powered Git archeology tool (a.k.a. Intelligent Commit Ontology Distiller and Enhanced Search)
 Home-page: https://github.com/a115/iCODES
 License: CC0-1.0
 Keywords: git,llm,archeology,commit,search
 Author: Jordan Dimov
 Author-email: jdimov@a115.co.uk
 Requires-Python: >=3.11,<4.0
```

