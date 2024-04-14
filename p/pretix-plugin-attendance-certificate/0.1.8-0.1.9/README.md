# Comparing `tmp/pretix_plugin_attendance_certificate-0.1.8.tar.gz` & `tmp/pretix_plugin_attendance_certificate-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.8.tar", last modified: Sun Apr 14 17:44:08 2024, max compression
+gzip compressed data, was "pretix_plugin_attendance_certificate-0.1.9.tar", last modified: Sun Apr 14 17:53:49 2024, max compression
```

## Comparing `pretix_plugin_attendance_certificate-0.1.8.tar` & `pretix_plugin_attendance_certificate-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2024-04-14 17:43:53.774056 pretix_plugin_attendance_certificate-0.1.8/LICENSE
--rw-r--r--   0        0        0      136 2024-04-14 17:43:53.774056 pretix_plugin_attendance_certificate-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/apps.py
--rw-r--r--   0        0        0      313 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/locale/de_Informal/.gitkeep
--rw-r--r--   0        0        0      313 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1950 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/migrations/__init__.py
--rw-r--r--   0        0        0     1380 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/models.py
--rw-r--r--   0        0        0     1516 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/render.py
--rw-r--r--   0        0        0     3475 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/signals.py
--rw-r--r--   0        0        0        0 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0      779 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
--rw-r--r--   0        0        0     2615 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/tasks.py
--rw-r--r--   0        0        0        0 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
--rw-r--r--   0        0        0       90 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      117 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
--rw-r--r--   0        0        0      495 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/urls.py
--rw-r--r--   0        0        0        0 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/views/__init__.py
--rw-r--r--   0        0        0     3611 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/views/editor.py
--rw-r--r--   0        0        0     2319 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/views/emails.py
--rw-r--r--   0        0        0      690 2024-04-14 17:44:08.141882 pretix_plugin_attendance_certificate-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 17:43:53.778056 pretix_plugin_attendance_certificate-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/LICENSE
+-rw-r--r--   0        0        0      136 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/__init__.py
+-rw-r--r--   0        0        0     1100 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/apps.py
+-rw-r--r--   0        0        0      313 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/locale/de_Informal/.gitkeep
+-rw-r--r--   0        0        0      313 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1950 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:53:38.266177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/migrations/__init__.py
+-rw-r--r--   0        0        0     1380 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/models.py
+-rw-r--r--   0        0        0     1516 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/render.py
+-rw-r--r--   0        0        0     3475 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/signals.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/static/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0      779 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf
+-rw-r--r--   0        0        0     2615 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/templates/pretix_attendance_certificate/.gitkeep
+-rw-r--r--   0        0        0       90 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/templates/pretix_attendance_certificate/history_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      117 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/templates/pretix_attendance_certificate/send_form_fragment_attendance_certificate.html
+-rw-r--r--   0        0        0      495 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/urls.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/views/__init__.py
+-rw-r--r--   0        0        0     3611 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/views/editor.py
+-rw-r--r--   0        0        0     2319 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/views/emails.py
+-rw-r--r--   0        0        0      690 2024-04-14 17:53:49.362183 pretix_plugin_attendance_certificate-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 17:53:38.270177 pretix_plugin_attendance_certificate-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 pretix_plugin_attendance_certificate-0.1.9/PKG-INFO
```

### Comparing `pretix_plugin_attendance_certificate-0.1.8/LICENSE` & `pretix_plugin_attendance_certificate-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/migrations/0001_initial.py` & `pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/models.py` & `pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/models.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/render.py` & `pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/render.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/signals.py` & `pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/signals.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf` & `pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/static/pretix_attendance_certificate/empty_attendance_certificate.pdf`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/tasks.py` & `pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/tasks.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/views/editor.py` & `pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/views/editor.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pretix_attendance_certificate/views/emails.py` & `pretix_plugin_attendance_certificate-0.1.9/pretix_attendance_certificate/views/emails.py`

 * *Files identical despite different names*

### Comparing `pretix_plugin_attendance_certificate-0.1.8/pyproject.toml` & `pretix_plugin_attendance_certificate-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pretix-plugin-attendance-certificate"
-version = "0.1.8"
+version = "0.1.9"
 description = "Create attendance certificates"
 authors = [
     { name = "Python Italia" },
 ]
 dependencies = []
 requires-python = ">=3.9,<4.0"
 readme = "README.md"
```

