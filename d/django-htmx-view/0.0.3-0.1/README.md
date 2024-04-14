# Comparing `tmp/django_htmx_view-0.0.3.tar.gz` & `tmp/django_htmx_view-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_htmx_view-0.0.3.tar", max compression
+gzip compressed data, was "django_htmx_view-0.1.tar", max compression
```

## Comparing `django_htmx_view-0.0.3.tar` & `django_htmx_view-0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-03-31 15:36:46.278071 django_htmx_view-0.0.3/LICENSE
--rw-r--r--   0        0        0        0 2024-03-31 15:16:21.369368 django_htmx_view-0.0.3/README.md
--rw-r--r--   0        0        0       72 2024-03-31 19:29:25.579596 django_htmx_view-0.0.3/htmx_view/__init__.py
--rw-r--r--   0        0        0     2694 2024-03-31 19:48:53.620181 django_htmx_view-0.0.3/htmx_view/mixins.py
--rw-r--r--   0        0        0      864 2024-03-31 18:05:18.258563 django_htmx_view-0.0.3/htmx_view/utils.py
--rw-r--r--   0        0        0     5918 2024-03-31 19:54:14.287375 django_htmx_view-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 django_htmx_view-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-31 15:36:46.278071 django_htmx_view-0.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-31 15:16:21.369368 django_htmx_view-0.1/README.md
+-rw-r--r--   0        0        0       72 2024-03-31 19:29:25.579596 django_htmx_view-0.1/htmx_view/__init__.py
+-rw-r--r--   0        0        0     3330 2024-04-14 10:21:42.600487 django_htmx_view-0.1/htmx_view/mixins.py
+-rw-r--r--   0        0        0      864 2024-03-31 18:05:18.258563 django_htmx_view-0.1/htmx_view/utils.py
+-rw-r--r--   0        0        0     5916 2024-04-14 10:23:00.022039 django_htmx_view-0.1/pyproject.toml
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 django_htmx_view-0.1/PKG-INFO
```

### Comparing `django_htmx_view-0.0.3/LICENSE` & `django_htmx_view-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_htmx_view-0.0.3/htmx_view/utils.py` & `django_htmx_view-0.1/htmx_view/utils.py`

 * *Files identical despite different names*

### Comparing `django_htmx_view-0.0.3/pyproject.toml` & `django_htmx_view-0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-htmx-view"
-version = "0.0.3"
+version = "0.1"
 description = "Build & Manage HTMX views with ease"
 authors = ["Waseem Akram <waseem07799@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/devwaseem/django-htmx-view"
 keywords = ["django", "htmx"]
 classifiers = [
```

### Comparing `django_htmx_view-0.0.3/PKG-INFO` & `django_htmx_view-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-view
-Version: 0.0.3
+Version: 0.1
 Summary: Build & Manage HTMX views with ease
 Home-page: https://github.com/devwaseem/django-htmx-view
 License: MIT
 Keywords: django,htmx
 Author: Waseem Akram
 Author-email: waseem07799@gmail.com
 Requires-Python: >=3.9
```

