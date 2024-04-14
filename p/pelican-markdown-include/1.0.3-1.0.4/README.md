# Comparing `tmp/pelican_markdown_include-1.0.3.tar.gz` & `tmp/pelican_markdown_include-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_markdown_include-1.0.3.tar", last modified: Sun Apr  7 09:33:36 2024, max compression
+gzip compressed data, was "pelican_markdown_include-1.0.4.tar", last modified: Sun Apr 14 11:31:40 2024, max compression
```

## Comparing `pelican_markdown_include-1.0.3.tar` & `pelican_markdown_include-1.0.4.tar`

### file list

```diff
@@ -1,4 +1,8 @@
--rw-r--r--   0        0        0     4099 2024-04-07 09:33:30.000000 pelican_markdown_include-1.0.3/README.md
--rw-r--r--   0        0        0     2357 2024-04-07 09:33:30.000000 pelican_markdown_include-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3168 2024-04-07 09:33:30.000000 pelican_markdown_include-1.0.3/tasks.py
--rw-r--r--   0        0        0     5610 2024-04-07 09:33:30.000000 pelican_markdown_include-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      526 2024-04-14 11:31:35.000000 pelican_markdown_include-1.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      569 2024-04-14 11:31:35.000000 pelican_markdown_include-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4099 2024-04-14 11:31:35.000000 pelican_markdown_include-1.0.4/README.md
+-rw-r--r--   0        0        0       40 2024-04-14 11:31:35.000000 pelican_markdown_include-1.0.4/pelican/plugins/md_include/__init__.py
+-rw-r--r--   0        0        0     2583 2024-04-14 11:31:35.000000 pelican_markdown_include-1.0.4/pelican/plugins/md_include/md_include.py
+-rw-r--r--   0        0        0     5126 2024-04-14 11:31:35.000000 pelican_markdown_include-1.0.4/pelican/plugins/md_include/test_md_include.py
+-rw-r--r--   0        0        0     2502 2024-04-14 11:31:35.000000 pelican_markdown_include-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5626 2024-04-14 11:31:35.000000 pelican_markdown_include-1.0.4/PKG-INFO
```

### Comparing `pelican_markdown_include-1.0.3/README.md` & `pelican_markdown_include-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,13 +63,13 @@
 Thanks to [Justin Mayer][] for helping with migration of this plugin under the Pelican Plugins organization.
 
 [Justin Mayer]: https://justinmayer.com
 
 Author
 ------
 
-Copyright © 2015, 2021-2023 Rafael Laboissière (<rafael@laboissiere.net>)
+Copyright © 2015, 2021-2024 Rafael Laboissière (<rafael@laboissiere.net>)
 
 License
 -------
 
 This project is licensed under the terms of the the AGPL-3.0 license.
```

### Comparing `pelican_markdown_include-1.0.3/pyproject.toml` & `pelican_markdown_include-1.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pelican-markdown-include"
-version = "1.0.3"
+version = "1.0.4"
 description = "Pelican plugin for using the Markdown-Include extension"
 authors = [
     { name = "Rafael Laboissière", email = "rafael@laboissiere.net" },
 ]
 readme = "README.md"
 keywords = [
     "pelican",
@@ -58,14 +58,26 @@
 test = [
     "markdown>=3.4",
     "pytest>=7.0",
     "pytest-cov>=4.0",
     "pytest-sugar>=0.9.7",
 ]
 
+[tool.pdm.build]
+source-includes = [
+    "CHANGELOG.md",
+    "CONTRIBUTING.md",
+]
+includes = [
+    "pelican/",
+]
+excludes = [
+    "tasks.py",
+]
+
 [tool.autopub]
 project-name = "Markdown Include"
 git-username = "botpub"
 git-email = "52496925+botpub@users.noreply.github.com"
 append-github-contributor = true
 
 [tool.ruff]
```

### Comparing `pelican_markdown_include-1.0.3/PKG-INFO` & `pelican_markdown_include-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pelican-markdown-include
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pelican plugin for using the Markdown-Include extension
-Keywords: pelican plugin markdown include
-Author-Email: Rafael Laboissière <rafael@laboissiere.net>
+Keywords: pelican,plugin,markdown include
+Author-Email: =?utf-8?q?Rafael_Laboissi=C3=A8re?= <rafael@laboissiere.net>
 License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -97,13 +97,13 @@
 Thanks to [Justin Mayer][] for helping with migration of this plugin under the Pelican Plugins organization.
 
 [Justin Mayer]: https://justinmayer.com
 
 Author
 ------
 
-Copyright © 2015, 2021-2023 Rafael Laboissière (<rafael@laboissiere.net>)
+Copyright © 2015, 2021-2024 Rafael Laboissière (<rafael@laboissiere.net>)
 
 License
 -------
 
 This project is licensed under the terms of the the AGPL-3.0 license.
```

