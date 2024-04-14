# Comparing `tmp/django-trix-editor-0.2.tar.gz` & `tmp/django_trix_editor-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-trix-editor-0.2.tar", last modified: Tue Sep 26 03:59:51 2023, max compression
+gzip compressed data, was "django_trix_editor-0.3.tar", last modified: Sun Apr 14 15:38:18 2024, max compression
```

## Comparing `django-trix-editor-0.2.tar` & `django_trix_editor-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-09-26 03:59:51.279940 django-trix-editor-0.2/
--rw-rw-rw-   0        0        0     1101 2023-09-24 11:49:21.000000 django-trix-editor-0.2/LICENSE
--rw-rw-rw-   0        0        0       36 2023-09-24 12:14:39.000000 django-trix-editor-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      276 2023-09-26 03:59:51.278935 django-trix-editor-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2023-09-25 04:32:36.000000 django-trix-editor-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-09-26 03:59:51.274956 django-trix-editor-0.2/django_trix_editor.egg-info/
--rw-rw-rw-   0        0        0      276 2023-09-26 03:59:51.000000 django-trix-editor-0.2/django_trix_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-09-26 03:59:51.000000 django-trix-editor-0.2/django_trix_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-26 03:59:51.000000 django-trix-editor-0.2/django_trix_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-09-26 03:59:51.000000 django-trix-editor-0.2/django_trix_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-09-26 03:59:51.000000 django-trix-editor-0.2/django_trix_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-26 03:59:51.279940 django-trix-editor-0.2/setup.cfg
--rw-rw-rw-   0        0        0      446 2023-09-26 03:39:51.000000 django-trix-editor-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-26 03:59:51.277756 django-trix-editor-0.2/trix_editor/
--rw-rw-rw-   0        0        0        0 2023-09-24 09:59:37.000000 django-trix-editor-0.2/trix_editor/__init__.py
--rw-rw-rw-   0        0        0      251 2023-09-25 04:23:42.000000 django-trix-editor-0.2/trix_editor/fields.py
--rw-rw-rw-   0        0        0      153 2023-09-24 12:54:32.000000 django-trix-editor-0.2/trix_editor/urls.py
--rw-rw-rw-   0        0        0      941 2023-09-26 03:46:38.000000 django-trix-editor-0.2/trix_editor/views.py
--rw-rw-rw-   0        0        0     3726 2023-09-25 04:21:45.000000 django-trix-editor-0.2/trix_editor/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:38:18.915711 django_trix_editor-0.3/
+-rw-rw-rw-   0        0        0     1101 2023-09-24 11:49:21.000000 django_trix_editor-0.3/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-11-08 18:00:13.000000 django_trix_editor-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2024-04-14 15:38:18.915711 django_trix_editor-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2371 2024-04-14 15:28:22.000000 django_trix_editor-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 15:38:18.914711 django_trix_editor-0.3/django_trix_editor.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-04-14 15:38:18.000000 django_trix_editor-0.3/django_trix_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-04-14 15:38:18.000000 django_trix_editor-0.3/django_trix_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:38:18.000000 django_trix_editor-0.3/django_trix_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-14 15:38:18.000000 django_trix_editor-0.3/django_trix_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-14 15:38:18.000000 django_trix_editor-0.3/django_trix_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:38:18.915711 django_trix_editor-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      446 2024-04-14 15:28:22.000000 django_trix_editor-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:38:18.914711 django_trix_editor-0.3/trix_editor/
+-rw-rw-rw-   0        0        0        0 2023-09-24 09:59:37.000000 django_trix_editor-0.3/trix_editor/__init__.py
+-rw-rw-rw-   0        0        0      251 2023-09-25 04:23:42.000000 django_trix_editor-0.3/trix_editor/fields.py
+-rw-rw-rw-   0        0        0      153 2023-09-24 12:54:32.000000 django_trix_editor-0.3/trix_editor/urls.py
+-rw-rw-rw-   0        0        0     1126 2023-09-27 06:01:05.000000 django_trix_editor-0.3/trix_editor/views.py
+-rw-rw-rw-   0        0        0     4060 2024-04-14 15:28:22.000000 django_trix_editor-0.3/trix_editor/widgets.py
```

### Comparing `django-trix-editor-0.2/LICENSE` & `django_trix_editor-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-trix-editor-0.2/README.md` & `django_trix_editor-0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Django Trix Editor Integration
 
 This package provides a Django app that integrates the [Trix editor](https://trix-editor.org/) with your Django project.
+Requires Django 4.1+
 
 ## Installation
 
 Install the package with pip:
 
 ```bash
 pip install django-trix-editor
@@ -35,14 +36,20 @@
 urlpatterns = [
     ...
     path('trix-editor/', include('trix_editor.urls')),
     ...
 ]
 ```
 
+If you want to give a specific permission to upload attachments, you can specify it in your `settings.py`:
+
+```python
+TRIX_UPLOAD_PERMISSION = 'your_model.upload_attachment'
+```
+
 You can use the `TrixEditorField` in your models:
 
 ```python
 from django.db import models
 from trix_editor.fields import TrixEditorField
 
 class MyModel(models.Model):
@@ -75,15 +82,14 @@
 ...
 <!-- footer -->
 {{ form.media.js }}
 ```
 
 ## Django Admin Integration
 To use the Trix editor in the Django admin, you need to add the following to your `admin.py`:
-
 ```python
 from django.contrib import admin
 from django import forms
 
 from trix_editor.widgets import TrixEditorWidget
 
 class ContentForm(forms.ModelForm):
```

### Comparing `django-trix-editor-0.2/trix_editor/views.py` & `django_trix_editor-0.3/trix_editor/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+import typing as t
 from http import HTTPStatus
+from functools import wraps
 
 from django.views.decorators.http import require_POST
 from django.http.response import JsonResponse
+from django.http.request import HttpRequest
 from django.core.files.storage import default_storage
 from django.conf import settings
 
 
-def requires_permission(view_func):
-    def wrapper(request, *args, **kwargs):
+def requires_permission(view_func: t.Callable) -> t.Callable:
+    @wraps(view_func)
+    def wrapper(request: HttpRequest, *args, **kwargs):
         if permission := getattr(settings, 'TRIX_UPLOAD_PERMISSION', None):
             if not request.user.has_perm(permission):
                 return JsonResponse(
                     {'error': 'You do not have permission to upload attachments.'},
                     status=HTTPStatus.FORBIDDEN,
                 )
         return view_func(request, *args, **kwargs)
     return wrapper
 
 
 @requires_permission
 @require_POST
-def handle_upload(request):
+def handle_upload(request: HttpRequest) -> JsonResponse:
     file = request.FILES.get('file')
     filename = default_storage.save(file.name, file)
     return JsonResponse({'attachment_url': default_storage.url(filename)})
```

### Comparing `django-trix-editor-0.2/trix_editor/widgets.py` & `django_trix_editor-0.3/trix_editor/widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from django import forms
-from django.utils.html import html_safe
 from django.conf import settings
+from django.utils.safestring import mark_safe
 
-TRIX_VERSION = getattr(settings, 'TRIX_VERSION', '2.0.6')
+TRIX_VERSION = getattr(settings, 'TRIX_VERSION', '2.1.0')
 
 
-@html_safe
 class JSPath:
-    def __str__(self):
+    def __html__(self):
         return (
-            f'<script src="https://unpkg.com/trix@{TRIX_VERSION}/dist/trix.umd.min.js" rel="stylesheet">'
+            f'<script type="text/javascript" src="//unpkg.com/trix@{TRIX_VERSION}/dist/trix.umd.min.js"></script>'
         )
 
 
-@html_safe
 class JSCode:
-    def __str__(self):
+    def __html__(self):
         return (
             """
-            <script>
+            <script type="text/javascript">
                 function getCookie(name) {
                     let cookieValue = null;
                     if (document.cookie && document.cookie !== '') {
                         const cookies = document.cookie.split(';');
                         for (let i = 0; i < cookies.length; i++) {
                             let cookie = cookies[i].trim();
                             // Does this cookie string begin with the name we want?
@@ -74,27 +72,42 @@
                     xhr.send(formData)
                 }
             </script>
             """
         )
 
 
-@html_safe
 class CSSPath:
-    def __str__(self):
+    def __html__(self):
         return (
             f'<link rel="stylesheet" href="https://unpkg.com/trix@{TRIX_VERSION}/dist/trix.css">'
         )
 
 
+class CSSAdminCode:
+    def __html__(self):
+        return (
+            """
+            <style>
+                .flex-container:has(trix-editor) {
+                    display: block;
+                }
+            </style>
+            """
+        )
+
+
 class TrixEditorWidget(forms.Textarea):
     def render(self, name, value, attrs=None, renderer=None):
         attrs = attrs or {}
         attrs['hidden'] = True
         html = super().render(name, value, attrs=attrs, renderer=renderer)
-        return f'{html}<trix-editor input="{attrs["id"]}"></trix-editor>'
+        return mark_safe(f'{html}<trix-editor input="{attrs["id"]}"></trix-editor>')
 
     class Media:
-        js = [JSPath(), JSCode()]
+        js = [
+            JSCode(),
+            JSPath(),
+        ]
         css = {
-            'all': [CSSPath()],
+            'all': [CSSAdminCode(), CSSPath()],
         }
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
-from django import forms from django.utils.html import html_safe from
-django.conf import settings TRIX_VERSION = getattr(settings, 'TRIX_VERSION',
-'2.0.6') @html_safe class JSPath: def __str__(self): return ( f'
-""" ) @html_safe class CSSPath: def __str__(self): return ( f'
-' ) class TrixEditorWidget(forms.Textarea): def render(self, name, value,
+from django import forms from django.conf import settings from
+django.utils.safestring import mark_safe TRIX_VERSION = getattr(settings,
+'TRIX_VERSION', '2.1.0') class JSPath: def __html__(self): return ( f'
+' ) class JSCode: def __html__(self): return ( """
+""" ) class CSSPath: def __html__(self): return ( f'
+' ) class CSSAdminCode: def __html__(self): return ( """
+""" ) class TrixEditorWidget(forms.Textarea): def render(self, name, value,
 attrs=None, renderer=None): attrs = attrs or {} attrs['hidden'] = True html =
-super().render(name, value, attrs=attrs, renderer=renderer) return f'{html}'
-class Media: js = [JSPath(), JSCode()] css = { 'all': [CSSPath()], }
+super().render(name, value, attrs=attrs, renderer=renderer) return mark_safe(f'
+{html}') class Media: js = [ JSCode(), JSPath(), ] css = { 'all': [CSSAdminCode
+(), CSSPath()], }
```

