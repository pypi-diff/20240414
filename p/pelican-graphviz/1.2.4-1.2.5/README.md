# Comparing `tmp/pelican_graphviz-1.2.4.tar.gz` & `tmp/pelican_graphviz-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_graphviz-1.2.4.tar", last modified: Sun Apr  7 09:37:46 2024, max compression
+gzip compressed data, was "pelican_graphviz-1.2.5.tar", last modified: Sun Apr 14 11:28:54 2024, max compression
```

## Comparing `pelican_graphviz-1.2.4.tar` & `pelican_graphviz-1.2.5.tar`

### file list

```diff
@@ -1,5 +1,11 @@
--rw-r--r--   0        0        0    34523 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/LICENSE
--rw-r--r--   0        0        0     6654 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/README.md
--rw-r--r--   0        0        0     2280 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     3166 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/tasks.py
--rw-r--r--   0        0        0     8065 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1369 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0      561 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/LICENSE
+-rw-r--r--   0        0        0     6654 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/README.md
+-rw-r--r--   0        0        0     6011 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/hello-world.png
+-rw-r--r--   0        0        0       38 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/pelican/plugins/graphviz/__init__.py
+-rw-r--r--   0        0        0     2282 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/pelican/plugins/graphviz/graphviz.py
+-rw-r--r--   0        0        0     6621 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/pelican/plugins/graphviz/mdx_graphviz.py
+-rw-r--r--   0        0        0     6519 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/pelican/plugins/graphviz/test_graphviz.py
+-rw-r--r--   0        0        0     2448 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     8081 2024-04-14 11:28:48.000000 pelican_graphviz-1.2.5/PKG-INFO
```

### Comparing `pelican_graphviz-1.2.4/LICENSE` & `pelican_graphviz-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_graphviz-1.2.4/README.md` & `pelican_graphviz-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pelican_graphviz-1.2.4/pyproject.toml` & `pelican_graphviz-1.2.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pelican-graphviz"
-version = "1.2.4"
+version = "1.2.5"
 description = "Pelican plugin supporting Graphviz images in articles"
 authors = [
     { name = "Rafael Laboissière", email = "rafael@laboissiere.net" },
 ]
 readme = "README.md"
 keywords = [
     "pelican",
@@ -56,14 +56,27 @@
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
+    "hello-world.png",
+]
+includes = [
+    "pelican/",
+]
+excludes = [
+    "tasks.py",
+]
+
 [tool.autopub]
 project-name = "Graphviz"
 git-username = "botpub"
 git-email = "52496925+botpub@users.noreply.github.com"
 append-github-contributor = true
 
 [tool.ruff]
```

### Comparing `pelican_graphviz-1.2.4/PKG-INFO` & `pelican_graphviz-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pelican-graphviz
-Version: 1.2.4
+Version: 1.2.5
 Summary: Pelican plugin supporting Graphviz images in articles
-Keywords: pelican plugin graphviz
-Author-Email: Rafael Laboissière <rafael@laboissiere.net>
+Keywords: pelican,plugin,graphviz
+Author-Email: =?utf-8?q?Rafael_Laboissi=C3=A8re?= <rafael@laboissiere.net>
 License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

