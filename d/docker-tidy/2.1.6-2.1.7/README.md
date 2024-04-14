# Comparing `tmp/docker_tidy-2.1.6.tar.gz` & `tmp/docker_tidy-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_tidy-2.1.6.tar", max compression
+gzip compressed data, was "docker_tidy-2.1.7.tar", max compression
```

## Comparing `docker_tidy-2.1.6.tar` & `docker_tidy-2.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11366 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/LICENSE
--rw-r--r--   0        0        0     1748 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/README.md
--rw-r--r--   0        0        0       46 2024-03-07 11:03:21.576329 docker_tidy-2.1.6/dockertidy/__init__.py
--rw-r--r--   0        0        0     3046 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/autostop.py
--rw-r--r--   0        0        0     4807 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/cli.py
--rw-r--r--   0        0        0     8555 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/config.py
--rw-r--r--   0        0        0      384 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/exception.py
--rw-r--r--   0        0        0    11649 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/garbage_collector.py
--rw-r--r--   0        0        0     5866 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/logger.py
--rw-r--r--   0        0        0     1206 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/parser.py
--rw-r--r--   0        0        0        0 2024-03-07 11:03:00.276419 docker_tidy-2.1.6/dockertidy/test/__init__.py
--rw-r--r--   0        0        0        0 2024-03-07 11:03:00.288418 docker_tidy-2.1.6/dockertidy/test/fixtures/__init__.py
--rw-r--r--   0        0        0     1942 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/test/fixtures/fixtures.py
--rw-r--r--   0        0        0     1244 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/test/unit/test_autostop.py
--rw-r--r--   0        0        0    12327 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/test/unit/test_garbagecollector.py
--rw-r--r--   0        0        0     1065 2024-03-07 11:02:59.676421 docker_tidy-2.1.6/dockertidy/utils.py
--rw-r--r--   0        0        0     3235 2024-03-07 11:03:21.572329 docker_tidy-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 docker_tidy-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11366 2024-04-14 09:48:03.261774 docker_tidy-2.1.7/LICENSE
+-rw-r--r--   0        0        0     1748 2024-04-14 09:48:03.261774 docker_tidy-2.1.7/README.md
+-rw-r--r--   0        0        0       46 2024-04-14 09:48:17.037833 docker_tidy-2.1.7/dockertidy/__init__.py
+-rw-r--r--   0        0        0     3046 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/autostop.py
+-rw-r--r--   0        0        0     4807 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/cli.py
+-rw-r--r--   0        0        0     8462 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/config.py
+-rw-r--r--   0        0        0      384 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/exception.py
+-rw-r--r--   0        0        0    11649 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/garbage_collector.py
+-rw-r--r--   0        0        0     5866 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/logger.py
+-rw-r--r--   0        0        0     1206 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/parser.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:48:03.713777 docker_tidy-2.1.7/dockertidy/test/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 09:48:03.713777 docker_tidy-2.1.7/dockertidy/test/fixtures/__init__.py
+-rw-r--r--   0        0        0     1942 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/test/fixtures/fixtures.py
+-rw-r--r--   0        0        0     1244 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/test/unit/test_autostop.py
+-rw-r--r--   0        0        0    12327 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/test/unit/test_garbagecollector.py
+-rw-r--r--   0        0        0     1065 2024-04-14 09:48:03.265774 docker_tidy-2.1.7/dockertidy/utils.py
+-rw-r--r--   0        0        0     3235 2024-04-14 09:48:17.033833 docker_tidy-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 docker_tidy-2.1.7/PKG-INFO
```

### Comparing `docker_tidy-2.1.6/LICENSE` & `docker_tidy-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/README.md` & `docker_tidy-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/autostop.py` & `docker_tidy-2.1.7/dockertidy/autostop.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/cli.py` & `docker_tidy-2.1.7/dockertidy/cli.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/config.py` & `docker_tidy-2.1.7/dockertidy/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,19 +230,16 @@
 
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
             raise dockertidy.exception.ConfigError("Configuration error", schema_error) from e
 
         return True
 
     def _add_dict_branch(self, tree, vector, value):
         key = vector[0]
         tree[key] = (
```

### Comparing `docker_tidy-2.1.6/dockertidy/garbage_collector.py` & `docker_tidy-2.1.7/dockertidy/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/logger.py` & `docker_tidy-2.1.7/dockertidy/logger.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/parser.py` & `docker_tidy-2.1.7/dockertidy/parser.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/test/fixtures/fixtures.py` & `docker_tidy-2.1.7/dockertidy/test/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/test/unit/test_autostop.py` & `docker_tidy-2.1.7/dockertidy/test/unit/test_autostop.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/test/unit/test_garbagecollector.py` & `docker_tidy-2.1.7/dockertidy/test/unit/test_garbagecollector.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/dockertidy/utils.py` & `docker_tidy-2.1.7/dockertidy/utils.py`

 * *Files identical despite different names*

### Comparing `docker_tidy-2.1.6/pyproject.toml` & `docker_tidy-2.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,46 +25,46 @@
 include = ["LICENSE"]
 keywords = ["docker", "gc", "prune", "garbage"]
 license = "Apache-2.0"
 name = "docker-tidy"
 packages = [{ include = "dockertidy" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/docker-tidy/"
-version = "2.1.6"
+version = "2.1.7"
 
 [tool.poetry.dependencies]
 anyconfig = "0.14.0"
 appdirs = "1.4.4"
 certifi = "2024.2.2"
 colorama = "0.4.6"
 dateparser = "1.2.0"
 docker = "7.0.0"
 docker-pycreds = "0.4.0"
 environs = "11.0.0"
-idna = "3.6"
+idna = "3.7"
 ipaddress = "1.0.23"
 jsonschema = "4.21.1"
 nested-lookup = "0.2.25"
 pathspec = "0.12.1"
 python = "^3.8.0"
 python-dateutil = "2.9.0.post0"
 python-json-logger = "2.0.7"
 requests = "2.31.0"
 "ruamel.yaml" = "0.18.6"
 websocket_client = "1.7.0"
-zipp = "3.17.0"
+zipp = "3.18.1"
 
 [tool.poetry.scripts]
 docker-tidy = "dockertidy.cli:main"
 
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

### Comparing `docker_tidy-2.1.6/PKG-INFO` & `docker_tidy-2.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-tidy
-Version: 2.1.6
+Version: 2.1.7
 Summary: Keep docker hosts tidy.
 Home-page: https://docker-tidy.geekdocs.de/
 License: Apache-2.0
 Keywords: docker,gc,prune,garbage
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.8.0,<4.0.0
@@ -29,25 +29,25 @@
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: certifi (==2024.2.2)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: dateparser (==1.2.0)
 Requires-Dist: docker (==7.0.0)
 Requires-Dist: docker-pycreds (==0.4.0)
 Requires-Dist: environs (==11.0.0)
-Requires-Dist: idna (==3.6)
+Requires-Dist: idna (==3.7)
 Requires-Dist: ipaddress (==1.0.23)
 Requires-Dist: jsonschema (==4.21.1)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: pathspec (==0.12.1)
 Requires-Dist: python-dateutil (==2.9.0.post0)
 Requires-Dist: python-json-logger (==2.0.7)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: ruamel.yaml (==0.18.6)
 Requires-Dist: websocket_client (==1.7.0)
-Requires-Dist: zipp (==3.17.0)
+Requires-Dist: zipp (==3.18.1)
 Project-URL: Documentation, https://docker-tidy.geekdocs.de/
 Project-URL: Repository, https://github.com/thegeeklab/docker-tidy/
 Description-Content-Type: text/markdown
 
 # docker-tidy
 
 Keep docker hosts tidy
```

