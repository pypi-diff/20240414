# Comparing `tmp/pelican_linkclass-2.1.3.tar.gz` & `tmp/pelican_linkclass-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_linkclass-2.1.3.tar", last modified: Sun Apr  7 09:25:56 2024, max compression
+gzip compressed data, was "pelican_linkclass-2.1.4.tar", last modified: Sun Apr 14 10:01:01 2024, max compression
```

## Comparing `pelican_linkclass-2.1.3.tar` & `pelican_linkclass-2.1.4.tar`

### file list

```diff
@@ -1,5 +1,12 @@
--rw-r--r--   0        0        0    34523 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/LICENSE
--rw-r--r--   0        0        0     3902 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/README.md
--rw-r--r--   0        0        0     2322 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     3167 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/tasks.py
--rw-r--r--   0        0        0     5368 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1374 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/CHANGELOG.md
+-rw-r--r--   0        0        0      562 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/LICENSE
+-rw-r--r--   0        0        0     3902 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/README.md
+-rw-r--r--   0        0        0      184 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/external-link.png
+-rw-r--r--   0        0        0     2585 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/linkclass-example.png
+-rw-r--r--   0        0        0       39 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/pelican/plugins/linkclass/__init__.py
+-rw-r--r--   0        0        0     1790 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/pelican/plugins/linkclass/linkclass.py
+-rw-r--r--   0        0        0     3978 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/pelican/plugins/linkclass/mdx_linkclass.py
+-rw-r--r--   0        0        0     7013 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/pelican/plugins/linkclass/test_linkclass.py
+-rw-r--r--   0        0        0     2521 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5384 2024-04-14 10:00:55.000000 pelican_linkclass-2.1.4/PKG-INFO
```

### Comparing `pelican_linkclass-2.1.3/LICENSE` & `pelican_linkclass-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_linkclass-2.1.3/README.md` & `pelican_linkclass-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pelican_linkclass-2.1.3/pyproject.toml` & `pelican_linkclass-2.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pelican-linkclass"
-version = "2.1.3"
+version = "2.1.4"
 description = "Pelican plugin to set anchor tag's class attribute to differentiate between internal and external links"
 authors = [
     { name = "Rafael Laboissière", email = "rafael@laboissiere.net" },
 ]
 readme = "README.md"
 keywords = [
     "pelican",
@@ -56,14 +56,28 @@
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
+    "external-link.png",
+    "linkclass-example.png",
+]
+includes = [
+    "pelican/",
+]
+excludes = [
+    "tasks.py",
+]
+
 [tool.autopub]
 project-name = "Link Class"
 git-username = "botpub"
 git-email = "52496925+botpub@users.noreply.github.com"
 append-github-contributor = true
 
 [tool.ruff]
```

### Comparing `pelican_linkclass-2.1.3/PKG-INFO` & `pelican_linkclass-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pelican-linkclass
-Version: 2.1.3
+Version: 2.1.4
 Summary: Pelican plugin to set anchor tag's class attribute to differentiate between internal and external links
-Keywords: pelican plugin link class
-Author-Email: Rafael Laboissière <rafael@laboissiere.net>
+Keywords: pelican,plugin,link class
+Author-Email: =?utf-8?q?Rafael_Laboissi=C3=A8re?= <rafael@laboissiere.net>
 License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

