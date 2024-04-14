# Comparing `tmp/pelican_avatar-1.0.8.tar.gz` & `tmp/pelican_avatar-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_avatar-1.0.8.tar", last modified: Thu Apr 11 09:52:16 2024, max compression
+gzip compressed data, was "pelican_avatar-1.0.9.tar", last modified: Sun Apr 14 11:25:05 2024, max compression
```

## Comparing `pelican_avatar-1.0.8.tar` & `pelican_avatar-1.0.9.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0    34523 2024-04-11 09:52:10.000000 pelican_avatar-1.0.8/LICENSE
--rw-r--r--   0        0        0     5345 2024-04-11 09:52:10.000000 pelican_avatar-1.0.8/README.md
--rw-r--r--   0        0        0     2311 2024-04-11 09:52:10.000000 pelican_avatar-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3164 2024-04-11 09:52:10.000000 pelican_avatar-1.0.8/tasks.py
--rw-r--r--   0        0        0     6813 2024-04-11 09:52:10.000000 pelican_avatar-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1121 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      559 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/LICENSE
+-rw-r--r--   0        0        0     5345 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/README.md
+-rw-r--r--   0        0        0   123104 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/avatar-example.png
+-rw-r--r--   0        0        0       36 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/pelican/plugins/avatar/__init__.py
+-rw-r--r--   0        0        0     3065 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/pelican/plugins/avatar/avatar.py
+-rw-r--r--   0        0        0     5512 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/pelican/plugins/avatar/test_avatar.py
+-rw-r--r--   0        0        0     2482 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6829 2024-04-14 11:24:59.000000 pelican_avatar-1.0.9/PKG-INFO
```

### Comparing `pelican_avatar-1.0.8/LICENSE` & `pelican_avatar-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_avatar-1.0.8/README.md` & `pelican_avatar-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pelican_avatar-1.0.8/pyproject.toml` & `pelican_avatar-1.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pelican-avatar"
-version = "1.0.8"
+version = "1.0.9"
 description = "Libravatar/Gravatar plugin for Pelican"
 authors = [
     { name = "Rafael Laboissière", email = "rafael@laboissiere.net" },
 ]
 readme = "README.md"
 keywords = [
     "pelican",
@@ -59,14 +59,27 @@
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
+    "avatar-example.png",
+]
+includes = [
+    "pelican/",
+]
+excludes = [
+    "tasks.py",
+]
+
 [tool.autopub]
 project-name = "Avatar"
 git-username = "botpub"
 git-email = "52496925+botpub@users.noreply.github.com"
 append-github-contributor = true
 
 [tool.ruff]
```

### Comparing `pelican_avatar-1.0.8/PKG-INFO` & `pelican_avatar-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pelican-avatar
-Version: 1.0.8
+Version: 1.0.9
 Summary: Libravatar/Gravatar plugin for Pelican
-Keywords: pelican plugin libravatar gravatar
-Author-Email: Rafael Laboissière <rafael@laboissiere.net>
+Keywords: pelican,plugin,libravatar,gravatar
+Author-Email: =?utf-8?q?Rafael_Laboissi=C3=A8re?= <rafael@laboissiere.net>
 License: AGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

