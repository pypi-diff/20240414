# Comparing `tmp/issx-0.0.2.tar.gz` & `tmp/issx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issx-0.0.2.tar", max compression
+gzip compressed data, was "issx-0.0.4.tar", max compression
```

## Comparing `issx-0.0.2.tar` & `issx-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1101 2024-04-01 18:14:53.508925 issx-0.0.2/LICENCE
--rw-r--r--   0        0        0     4290 2024-04-01 18:14:53.508925 issx-0.0.2/README.md
--rw-r--r--   0        0        0     2854 2024-04-01 18:14:53.508925 issx-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/__init__.py
--rw-r--r--   0        0        0     1880 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/cli.py
--rw-r--r--   0        0        0      176 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/clients/__init__.py
--rw-r--r--   0        0        0     2189 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/clients/gitlab.py
--rw-r--r--   0        0        0      291 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/clients/interfaces.py
--rw-r--r--   0        0        0        0 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/domain/__init__.py
--rw-r--r--   0        0        0      205 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/domain/issues.py
--rw-r--r--   0        0        0        0 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/py.typed
--rw-r--r--   0        0        0      588 2024-04-01 18:14:53.508925 issx-0.0.2/src/issx/services.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 issx-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-14 16:47:24.978422 issx-0.0.4/LICENCE
+-rw-r--r--   0        0        0     4568 2024-04-14 16:47:24.978422 issx-0.0.4/README.md
+-rw-r--r--   0        0        0     2959 2024-04-14 16:47:24.978422 issx-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 16:47:24.978422 issx-0.0.4/src/issx/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-14 16:47:24.978422 issx-0.0.4/src/issx/cli.py
+-rw-r--r--   0        0        0      200 2024-04-14 16:47:24.978422 issx-0.0.4/src/issx/clients/__init__.py
+-rw-r--r--   0        0        0      185 2024-04-14 16:47:24.978422 issx-0.0.4/src/issx/clients/exceptions.py
+-rw-r--r--   0        0        0     2863 2024-04-14 16:47:24.982422 issx-0.0.4/src/issx/clients/gitlab.py
+-rw-r--r--   0        0        0     1344 2024-04-14 16:47:24.982422 issx-0.0.4/src/issx/clients/interfaces.py
+-rw-r--r--   0        0        0     2929 2024-04-14 16:47:24.982422 issx-0.0.4/src/issx/clients/redmine.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:47:24.982422 issx-0.0.4/src/issx/domain/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-14 16:47:24.982422 issx-0.0.4/src/issx/domain/issues.py
+-rw-r--r--   0        0        0     2442 2024-04-14 16:47:24.982422 issx-0.0.4/src/issx/instance_managers.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:47:24.982422 issx-0.0.4/src/issx/py.typed
+-rw-r--r--   0        0        0      588 2024-04-14 16:47:24.982422 issx-0.0.4/src/issx/services.py
+-rw-r--r--   0        0        0     5628 1970-01-01 00:00:00.000000 issx-0.0.4/PKG-INFO
```

### Comparing `issx-0.0.2/LICENCE` & `issx-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `issx-0.0.2/README.md` & `issx-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -38,43 +38,51 @@
 
 ## Usage
 
 The basic functionality of `issx` is provided through the `issx` command-line interface (CLI).
 
 Currently, there is only one command available: `copy`.
 
-It allows to copy issues from one place to another.
-As for now, it supports copying issues between **projects in the same backend** (Gitlab).
+It allows to copy issues from one [configured](#configuration-file) project to another .
 
 ```shell
-issx copy --source-project-id=<id> --target-project-id=<id> <issue-id>
+issx copy --source=<project_name> --target=<project_name> <issue-id>
 ```
 
-where `source-project-id` and `target-project-id` are the IDs of the projects in the same backend and
-`issue-id` is the ID of the issue to be copied.
+where `source` and `target` are the names of the projects configured in the configuration file.
 
-### Authentication
+### Configuration file
 
-#### Gitlab
-For the Gitlab backend we use the `python-gitlab` package with file-based [configuration](https://python-gitlab.readthedocs.io/en/stable/cli-usage.html#configuration-file-format).
-`issx` will use the configured default section from the configuration file located in `~/.python-gitlab.cfg`
-(`private_instance` in the example below).
+The configuration file can be either in the working directory (`issx.toml`) or in `~/.config/issx.toml`.
 
-```
-[global]
-default = private_instance
+It should have the following structure:
 
-[private_instance]
-url = https://private-gitlab.com/
-private_token = <your_private_token>
+```toml
+[instances.INSTANCE_NAME]
+    backend = "gitlab" / "redmine"
+    url = "<absolute url to the instance>"
+    token = "<API token used for authentication>"
+
+[projects.PROJECT_NAME]
+    instance = "INSTANCE_NAME"
+    project = "<project_id>"
 ```
 
-To validate the authentication, you can use command:
+`Instances` section is used to configure the instances of the services (e.g. Gitlab, Redmine)
+that `issx` will interact with.
+
+`Projects` section is used to configure the projects that `issx` will work with. Each project should be associated with
+an instance.
+`project` field should contain the project id available in the chosen instance (usually it is a number).
+
+### Authentication
+
+To validate the authentication with a newly configured instance, you can use command `issx auth-verify`:
 ```shell
-issx auth-verify
+issx auth-verify --instance=<instance_name>
 ```
 
 ## Development
 
 * Clone this repository
 * Requirements:
   * [Poetry](https://python-poetry.org/)
```

### Comparing `issx-0.0.2/pyproject.toml` & `issx-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "issx"
-version = "0.0.2"
+version = "0.0.4"
 description = "Tool for synchronizing issues between different services"
 authors = [
     "nekeal <szymon.sc.cader@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -31,14 +31,15 @@
 issx = "issx.cli:app"
 
 [tool.poetry.dependencies]
 python = ">=3.11, <4.0"
 python-gitlab = "^4.4.0"
 attrs = "^23.2.0"
 typer = "^0.12.0"
+python-redmine = "^2.5.0"
 
 [tool.poetry.group.dev.dependencies]
 mkdocstrings = {version = ">=0.18", extras = ["python"]}
 mkdocs-material = "*"
 mypy = "*"
 pre-commit = "*"
 pymdown-extensions = "*"
@@ -122,7 +123,11 @@
 no_implicit_optional = true
 strict_equality = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 warn_return_any = true
 check_untyped_defs = true
 show_error_codes = true
+
+[[tool.mypy.overrides]]
+module = "redminelib.*"
+ignore_missing_imports = true
```

### Comparing `issx-0.0.2/src/issx/services.py` & `issx-0.0.4/src/issx/services.py`

 * *Files identical despite different names*

### Comparing `issx-0.0.2/PKG-INFO` & `issx-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issx
-Version: 0.0.2
+Version: 0.0.4
 Summary: Tool for synchronizing issues between different services
 Home-page: https://nekeal.github.io/issx
 License: MIT
 Author: nekeal
 Author-email: szymon.sc.cader@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: attrs (>=23.2.0,<24.0.0)
 Requires-Dist: python-gitlab (>=4.4.0,<5.0.0)
+Requires-Dist: python-redmine (>=2.5.0,<3.0.0)
 Requires-Dist: typer (>=0.12.0,<0.13.0)
 Project-URL: Documentation, https://nekeal.github.io/issx
 Project-URL: Repository, https://github.com/nekeal/issx
 Description-Content-Type: text/markdown
 
 # Issx
 
@@ -64,43 +65,51 @@
 
 ## Usage
 
 The basic functionality of `issx` is provided through the `issx` command-line interface (CLI).
 
 Currently, there is only one command available: `copy`.
 
-It allows to copy issues from one place to another.
-As for now, it supports copying issues between **projects in the same backend** (Gitlab).
+It allows to copy issues from one [configured](#configuration-file) project to another .
 
 ```shell
-issx copy --source-project-id=<id> --target-project-id=<id> <issue-id>
+issx copy --source=<project_name> --target=<project_name> <issue-id>
 ```
 
-where `source-project-id` and `target-project-id` are the IDs of the projects in the same backend and
-`issue-id` is the ID of the issue to be copied.
+where `source` and `target` are the names of the projects configured in the configuration file.
 
-### Authentication
+### Configuration file
 
-#### Gitlab
-For the Gitlab backend we use the `python-gitlab` package with file-based [configuration](https://python-gitlab.readthedocs.io/en/stable/cli-usage.html#configuration-file-format).
-`issx` will use the configured default section from the configuration file located in `~/.python-gitlab.cfg`
-(`private_instance` in the example below).
+The configuration file can be either in the working directory (`issx.toml`) or in `~/.config/issx.toml`.
 
-```
-[global]
-default = private_instance
+It should have the following structure:
 
-[private_instance]
-url = https://private-gitlab.com/
-private_token = <your_private_token>
+```toml
+[instances.INSTANCE_NAME]
+    backend = "gitlab" / "redmine"
+    url = "<absolute url to the instance>"
+    token = "<API token used for authentication>"
+
+[projects.PROJECT_NAME]
+    instance = "INSTANCE_NAME"
+    project = "<project_id>"
 ```
 
-To validate the authentication, you can use command:
+`Instances` section is used to configure the instances of the services (e.g. Gitlab, Redmine)
+that `issx` will interact with.
+
+`Projects` section is used to configure the projects that `issx` will work with. Each project should be associated with
+an instance.
+`project` field should contain the project id available in the chosen instance (usually it is a number).
+
+### Authentication
+
+To validate the authentication with a newly configured instance, you can use command `issx auth-verify`:
 ```shell
-issx auth-verify
+issx auth-verify --instance=<instance_name>
 ```
 
 ## Development
 
 * Clone this repository
 * Requirements:
   * [Poetry](https://python-poetry.org/)
```

