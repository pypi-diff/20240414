# Comparing `tmp/ansible_doctor-4.0.3.tar.gz` & `tmp/ansible_doctor-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_doctor-4.0.3.tar", max compression
+gzip compressed data, was "ansible_doctor-4.0.4.tar", max compression
```

## Comparing `ansible_doctor-4.0.3.tar` & `ansible_doctor-4.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    32460 2024-03-07 11:02:53.124455 ansible_doctor-4.0.3/LICENSE
--rw-r--r--   0        0        0     2717 2024-03-07 11:02:53.124455 ansible_doctor-4.0.3/README.md
--rw-r--r--   0        0        0      205 2024-03-07 11:03:18.372341 ansible_doctor-4.0.3/ansibledoctor/__init__.py
--rw-r--r--   0        0        0     6210 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/annotation.py
--rw-r--r--   0        0        0     4042 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/cli.py
--rw-r--r--   0        0        0    12050 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/config.py
--rw-r--r--   0        0        0      120 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/contstants.py
--rw-r--r--   0        0        0     7261 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/doc_generator.py
--rw-r--r--   0        0        0     4072 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/doc_parser.py
--rw-r--r--   0        0        0      558 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/exception.py
--rw-r--r--   0        0        0     1670 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/file_registry.py
--rw-r--r--   0        0        0      377 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/_meta.j2
--rw-r--r--   0        0        0      172 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/_requirements.j2
--rw-r--r--   0        0        0      318 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/_tag.j2
--rw-r--r--   0        0        0      371 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/_toc.j2
--rw-r--r--   0        0        0      583 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/_todo.j2
--rw-r--r--   0        0        0     1558 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/_vars.j2
--rw-r--r--   0        0        0      848 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/index.md.j2
--rw-r--r--   0        0        0      697 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/readme/README.md.j2
--rw-r--r--   0        0        0      691 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/readme/_meta.j2
--rw-r--r--   0        0        0      172 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/readme/_requirements.j2
--rw-r--r--   0        0        0      365 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/readme/_tag.j2
--rw-r--r--   0        0        0      434 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/readme/_toc.j2
--rw-r--r--   0        0        0      583 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/readme/_todo.j2
--rw-r--r--   0        0        0     1558 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/templates/readme/_vars.j2
--rw-r--r--   0        0        0     9463 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/utils/__init__.py
--rw-r--r--   0        0        0     2412 2024-03-07 11:02:53.132455 ansible_doctor-4.0.3/ansibledoctor/utils/yamlhelper.py
--rw-r--r--   0        0        0     3174 2024-03-07 11:03:18.368341 ansible_doctor-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ansible_doctor-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0    32460 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/LICENSE
+-rw-r--r--   0        0        0     2717 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/README.md
+-rw-r--r--   0        0        0      205 2024-04-14 09:47:31.484658 ansible_doctor-4.0.4/ansibledoctor/__init__.py
+-rw-r--r--   0        0        0     6210 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/annotation.py
+-rw-r--r--   0        0        0     4042 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/cli.py
+-rw-r--r--   0        0        0    11957 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/config.py
+-rw-r--r--   0        0        0      120 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/contstants.py
+-rw-r--r--   0        0        0     7261 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/doc_generator.py
+-rw-r--r--   0        0        0     4072 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/doc_parser.py
+-rw-r--r--   0        0        0      558 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/exception.py
+-rw-r--r--   0        0        0     1670 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/file_registry.py
+-rw-r--r--   0        0        0      377 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_meta.j2
+-rw-r--r--   0        0        0      172 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_requirements.j2
+-rw-r--r--   0        0        0      318 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_tag.j2
+-rw-r--r--   0        0        0      371 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_toc.j2
+-rw-r--r--   0        0        0      583 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_todo.j2
+-rw-r--r--   0        0        0     1558 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_vars.j2
+-rw-r--r--   0        0        0      848 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/index.md.j2
+-rw-r--r--   0        0        0      697 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/README.md.j2
+-rw-r--r--   0        0        0      691 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_meta.j2
+-rw-r--r--   0        0        0      172 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_requirements.j2
+-rw-r--r--   0        0        0      365 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_tag.j2
+-rw-r--r--   0        0        0      434 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_toc.j2
+-rw-r--r--   0        0        0      583 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_todo.j2
+-rw-r--r--   0        0        0     1558 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/templates/readme/_vars.j2
+-rw-r--r--   0        0        0     9463 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/utils/__init__.py
+-rw-r--r--   0        0        0     2412 2024-04-14 09:47:16.028640 ansible_doctor-4.0.4/ansibledoctor/utils/yamlhelper.py
+-rw-r--r--   0        0        0     3174 2024-04-14 09:47:31.484658 ansible_doctor-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ansible_doctor-4.0.4/PKG-INFO
```

### Comparing `ansible_doctor-4.0.3/LICENSE` & `ansible_doctor-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/README.md` & `ansible_doctor-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/annotation.py` & `ansible_doctor-4.0.4/ansibledoctor/annotation.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/cli.py` & `ansible_doctor-4.0.4/ansibledoctor/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/config.py` & `ansible_doctor-4.0.4/ansibledoctor/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -308,19 +308,16 @@
 
         return path
 
     def _validate(self, config):
         try:
             anyconfig.validate(config, self.schema, ac_schema_safe=False)
         except jsonschema.exceptions.ValidationError as e:
-            schema_error = "Failed validating '{validator}' in schema{schema}\n{message}".format(
-                validator=e.validator,
-                schema=format_as_index(list(e.relative_schema_path)[:-1]),
-                message=e.message,
-            )
+            schema = format_as_index(list(e.relative_schema_path)[:-1])
+            schema_error = f"Failed validating '{e.validator}' in schema {schema}\n{e.message}"
             raise ansibledoctor.exception.ConfigError("Configuration error", schema_error) from e
 
         return True
 
     def _add_dict_branch(self, tree, vector, value):
         key = vector[0]
         tree[key] = (
```

### Comparing `ansible_doctor-4.0.3/ansibledoctor/doc_generator.py` & `ansible_doctor-4.0.4/ansibledoctor/doc_generator.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/doc_parser.py` & `ansible_doctor-4.0.4/ansibledoctor/doc_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/exception.py` & `ansible_doctor-4.0.4/ansibledoctor/exception.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/file_registry.py` & `ansible_doctor-4.0.4/ansibledoctor/file_registry.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/_todo.j2` & `ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_todo.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/_vars.j2` & `ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/_vars.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/templates/hugo-book/index.md.j2` & `ansible_doctor-4.0.4/ansibledoctor/templates/hugo-book/index.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/templates/readme/README.md.j2` & `ansible_doctor-4.0.4/ansibledoctor/templates/readme/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/templates/readme/_meta.j2` & `ansible_doctor-4.0.4/ansibledoctor/templates/readme/_meta.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/templates/readme/_todo.j2` & `ansible_doctor-4.0.4/ansibledoctor/templates/readme/_todo.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/templates/readme/_vars.j2` & `ansible_doctor-4.0.4/ansibledoctor/templates/readme/_vars.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/utils/__init__.py` & `ansible_doctor-4.0.4/ansibledoctor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/ansibledoctor/utils/yamlhelper.py` & `ansible_doctor-4.0.4/ansibledoctor/utils/yamlhelper.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-4.0.3/pyproject.toml` & `ansible_doctor-4.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,40 +24,40 @@
 include = ["LICENSE"]
 keywords = ["ansible", "role", "documentation"]
 license = "GPL-3.0-only"
 name = "ansible-doctor"
 packages = [{ include = "ansibledoctor" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-doctor/"
-version = "4.0.3"
+version = "4.0.4"
 
 [tool.poetry.dependencies]
 Jinja2 = "3.1.3"
 anyconfig = "0.14.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 environs = "11.0.0"
 jsonschema = "4.21.1"
 pathspec = "0.12.1"
 python = "^3.9.0"
 python-json-logger = "2.0.7"
 "ruamel.yaml" = "0.18.6"
-ansible-core = { version = "2.14.14", optional = true }
+ansible-core = { version = "2.14.15", optional = true }
 
 [tool.poetry.extras]
 ansible-core = ["ansible-core"]
 
 [tool.poetry.scripts]
 ansible-doctor = "ansibledoctor.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.3.0"
-pytest = "8.1.0"
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

### Comparing `ansible_doctor-4.0.3/PKG-INFO` & `ansible_doctor-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-doctor
-Version: 4.0.3
+Version: 4.0.4
 Summary: Generate documentation from annotated Ansible roles using templates.
 Home-page: https://ansible-doctor.geekdocs.de/
 License: GPL-3.0-only
 Keywords: ansible,role,documentation
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Provides-Extra: ansible-core
 Requires-Dist: Jinja2 (==3.1.3)
-Requires-Dist: ansible-core (==2.14.14) ; extra == "ansible-core"
+Requires-Dist: ansible-core (==2.14.15) ; extra == "ansible-core"
 Requires-Dist: anyconfig (==0.14.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: environs (==11.0.0)
 Requires-Dist: jsonschema (==4.21.1)
 Requires-Dist: pathspec (==0.12.1)
 Requires-Dist: python-json-logger (==2.0.7)
```

