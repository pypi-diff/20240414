# Comparing `tmp/django-group-model-1.0.0.tar.gz` & `tmp/django-group-model-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-group-model-1.0.0.tar", last modified: Thu Mar 28 14:24:25 2024, max compression
+gzip compressed data, was "django-group-model-1.0.1.tar", last modified: Sun Apr 14 10:46:54 2024, max compression
```

## Comparing `django-group-model-1.0.0.tar` & `django-group-model-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-03-28 14:24:25.220630 django-group-model-1.0.0/
--rw-rw-r--   0 ankit     (1000) ankit     (1000)     1071 2024-03-28 07:48:12.000000 django-group-model-1.0.0/LICENSE
--rw-r--r--   0 ankit     (1000) ankit     (1000)       34 2024-03-28 09:40:19.000000 django-group-model-1.0.0/MANIFEST.in
--rw-r--r--   0 ankit     (1000) ankit     (1000)     8193 2024-03-28 14:24:25.220630 django-group-model-1.0.0/PKG-INFO
--rw-rw-r--   0 ankit     (1000) ankit     (1000)     6532 2024-03-28 14:22:02.000000 django-group-model-1.0.0/README.md
-drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-03-28 14:24:25.216630 django-group-model-1.0.0/django_group_model/
--rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-03-27 20:00:47.000000 django-group-model-1.0.0/django_group_model/__init__.py
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       63 2024-03-27 20:00:47.000000 django-group-model-1.0.0/django_group_model/admin.py
--rw-rw-r--   0 ankit     (1000) ankit     (1000)      925 2024-03-27 20:07:02.000000 django-group-model-1.0.0/django_group_model/apps.py
-drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-03-28 14:24:25.220630 django-group-model-1.0.0/django_group_model/migrations/
--rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-03-27 20:00:47.000000 django-group-model-1.0.0/django_group_model/migrations/__init__.py
--rw-rw-r--   0 ankit     (1000) ankit     (1000)      868 2024-03-27 20:52:53.000000 django-group-model-1.0.0/django_group_model/models.py
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       60 2024-03-27 20:00:47.000000 django-group-model-1.0.0/django_group_model/tests.py
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       63 2024-03-27 20:00:47.000000 django-group-model-1.0.0/django_group_model/views.py
-drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-03-28 14:24:25.220630 django-group-model-1.0.0/django_group_model.egg-info/
--rw-r--r--   0 ankit     (1000) ankit     (1000)     8193 2024-03-28 14:24:25.000000 django-group-model-1.0.0/django_group_model.egg-info/PKG-INFO
--rw-rw-r--   0 ankit     (1000) ankit     (1000)      475 2024-03-28 14:24:25.000000 django-group-model-1.0.0/django_group_model.egg-info/SOURCES.txt
--rw-rw-r--   0 ankit     (1000) ankit     (1000)        1 2024-03-28 14:24:25.000000 django-group-model-1.0.0/django_group_model.egg-info/dependency_links.txt
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       12 2024-03-28 14:24:25.000000 django-group-model-1.0.0/django_group_model.egg-info/requires.txt
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       19 2024-03-28 14:24:25.000000 django-group-model-1.0.0/django_group_model.egg-info/top_level.txt
--rw-r--r--   0 ankit     (1000) ankit     (1000)     1616 2024-03-28 14:17:40.000000 django-group-model-1.0.0/pyproject.toml
--rw-rw-r--   0 ankit     (1000) ankit     (1000)       38 2024-03-28 14:24:25.220630 django-group-model-1.0.0/setup.cfg
--rw-r--r--   0 ankit     (1000) ankit     (1000)       38 2024-03-28 09:14:33.000000 django-group-model-1.0.0/setup.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-14 10:46:54.963473 django-group-model-1.0.1/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     1071 2024-03-28 07:48:12.000000 django-group-model-1.0.1/LICENSE
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       34 2024-03-28 09:40:19.000000 django-group-model-1.0.1/MANIFEST.in
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     8740 2024-04-14 10:46:54.963473 django-group-model-1.0.1/PKG-INFO
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     7079 2024-04-14 10:46:27.000000 django-group-model-1.0.1/README.md
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-14 10:46:54.963473 django-group-model-1.0.1/django_group_model/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-03-27 20:00:47.000000 django-group-model-1.0.1/django_group_model/__init__.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       63 2024-03-27 20:00:47.000000 django-group-model-1.0.1/django_group_model/admin.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      924 2024-04-14 10:46:27.000000 django-group-model-1.0.1/django_group_model/apps.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-14 10:46:54.963473 django-group-model-1.0.1/django_group_model/migrations/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-03-27 20:00:47.000000 django-group-model-1.0.1/django_group_model/migrations/__init__.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     1122 2024-04-14 10:46:27.000000 django-group-model-1.0.1/django_group_model/models.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       60 2024-03-27 20:00:47.000000 django-group-model-1.0.1/django_group_model/tests.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       63 2024-03-27 20:00:47.000000 django-group-model-1.0.1/django_group_model/views.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-04-14 10:46:54.963473 django-group-model-1.0.1/django_group_model.egg-info/
+-rw-r--r--   0 ankit     (1000) ankit     (1000)     8740 2024-04-14 10:46:54.000000 django-group-model-1.0.1/django_group_model.egg-info/PKG-INFO
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      475 2024-04-14 10:46:54.000000 django-group-model-1.0.1/django_group_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        1 2024-04-14 10:46:54.000000 django-group-model-1.0.1/django_group_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       12 2024-04-14 10:46:54.000000 django-group-model-1.0.1/django_group_model.egg-info/requires.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       19 2024-04-14 10:46:54.000000 django-group-model-1.0.1/django_group_model.egg-info/top_level.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     1616 2024-04-14 10:46:27.000000 django-group-model-1.0.1/pyproject.toml
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       38 2024-04-14 10:46:54.963473 django-group-model-1.0.1/setup.cfg
+-rw-r--r--   0 ankit     (1000) ankit     (1000)       38 2024-03-28 09:14:33.000000 django-group-model-1.0.1/setup.py
```

### Comparing `django-group-model-1.0.0/LICENSE` & `django-group-model-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-group-model-1.0.0/PKG-INFO` & `django-group-model-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-group-model
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django app to override the default Group model
 Author: Ankit Chhatbar
 Project-URL: Homepage, https://github.com/ankitchhatbar/django-group-model
 Project-URL: Documentation, https://github.com/ankitchhatbar/django-group-model
 Project-URL: Repository, https://github.com/ankitchhatbar/django-group-model
 Project-URL: Issues, https://github.com/ankitchhatbar/django-group-model/issues
 Classifier: Environment :: Web Environment
@@ -52,30 +52,32 @@
 
 - When starting a project, setting a custom Group model will allow you to customize it in the future when the need arises.
 
 ## Requirements
 
 - Python: 3.6+
 
-- Django: 3.0+
+- Django: 5.0, 4.2, 4.1, 4.0, 3.2, 3.1, 3.0
 
 ## Installation
 
 Install using pip:
 
 ```bash
 pip install django-group-model
 ```
 
-Add `'django_group_model'`  to your `INSTALLED_APPS`. Make sure to place it before any apps that define the `Group` or `User` models.
+Add `'django_group_model'` to your `INSTALLED_APPS`. Make sure to place it after the default Django apps (if any) and before any custom apps that define the `Group` or `User` models.
 
 ```python
 INSTALLED_APPS = [
     ...
-    'django_group_model',
+    'django.contrib.staticfiles',
+    'django_group_model', # Add this
+    ...
 ]
 ```
 
 ## Usage
 
 ### Overriding the default Group model
 
@@ -118,14 +120,23 @@
 
     )
     ...
 ```
 
 Once again, the name of the field is important. See below on how to customize the name of the model. Also take note of the `related_name` and `related_query_name`. Most of the time, the pattern shown above should work. For a deeper understanding see [Django docs here](https://docs.djangoproject.com/en/5.0/ref/models/fields/#django.db.models.ForeignKey.related_name).
 
+Since the name of the new model is `Group`, when accessing Groups attached to a permission, you will have to use the `custom_group_set` accessor.
+
+```python
+permisssion = Permisssion.objects.first()
+groups = permission.custom_group_set.all()
+```
+
+This only applies if your custom model is called `Group`. If you name it something else (see below). It will use Django's default conventions for the reverse accessor.
+
 ### Customizing the name of the Group model
 
 Overriding the default `Group` model with a custom name involves 2 steps:
 
 1. Create a model class that extends `AbstractGroup` with any name that you like.
 
 2. Override `verbose_name` and `verbose_name_plural` attributes of the `Meta` class.
```

### Comparing `django-group-model-1.0.0/README.md` & `django-group-model-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,32 @@
 
 - When starting a project, setting a custom Group model will allow you to customize it in the future when the need arises.
 
 ## Requirements
 
 - Python: 3.6+
 
-- Django: 3.0+
+- Django: 5.0, 4.2, 4.1, 4.0, 3.2, 3.1, 3.0
 
 ## Installation
 
 Install using pip:
 
 ```bash
 pip install django-group-model
 ```
 
-Add `'django_group_model'`  to your `INSTALLED_APPS`. Make sure to place it before any apps that define the `Group` or `User` models.
+Add `'django_group_model'` to your `INSTALLED_APPS`. Make sure to place it after the default Django apps (if any) and before any custom apps that define the `Group` or `User` models.
 
 ```python
 INSTALLED_APPS = [
     ...
-    'django_group_model',
+    'django.contrib.staticfiles',
+    'django_group_model', # Add this
+    ...
 ]
 ```
 
 ## Usage
 
 ### Overriding the default Group model
 
@@ -80,14 +82,23 @@
 
     )
     ...
 ```
 
 Once again, the name of the field is important. See below on how to customize the name of the model. Also take note of the `related_name` and `related_query_name`. Most of the time, the pattern shown above should work. For a deeper understanding see [Django docs here](https://docs.djangoproject.com/en/5.0/ref/models/fields/#django.db.models.ForeignKey.related_name).
 
+Since the name of the new model is `Group`, when accessing Groups attached to a permission, you will have to use the `custom_group_set` accessor.
+
+```python
+permisssion = Permisssion.objects.first()
+groups = permission.custom_group_set.all()
+```
+
+This only applies if your custom model is called `Group`. If you name it something else (see below). It will use Django's default conventions for the reverse accessor.
+
 ### Customizing the name of the Group model
 
 Overriding the default `Group` model with a custom name involves 2 steps:
 
 1. Create a model class that extends `AbstractGroup` with any name that you like.
 
 2. Override `verbose_name` and `verbose_name_plural` attributes of the `Meta` class.
```

### Comparing `django-group-model-1.0.0/django_group_model/apps.py` & `django-group-model-1.0.1/django_group_model/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,8 @@
             group_model = settings.AUTH_GROUP_MODEL
             related_name_to_group = group_model.split('.')[-1].lower()
 
             user_groups_field = get_user_model()._meta.get_field(f"{related_name_to_group}s")
             user_groups_query = f"{related_name_to_group}__{user_groups_field.related_query_name()}"
             return Permission.objects.filter(**{user_groups_query: user_obj})
 
-
         ModelBackend._get_group_permissions = _get_group_permissions
```

### Comparing `django-group-model-1.0.0/django_group_model/models.py` & `django-group-model-1.0.1/django_group_model/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from django.contrib.auth.models import Permission, GroupManager
+from django.conf import settings
+
+group_model = settings.AUTH_GROUP_MODEL
+group_model_name = group_model.split('.')[-1]
+permissions_related_name = 'custom_group_set' if group_model_name == "Group" else None
 
 
 # This class has been copied from django.contrib.auth.models.Group
 # The only additional thing set is abstract=True in meta
 # This class should not be updated unless replacing it with a new version from django.contrib.auth.models.Group
 class AbstractGroup(models.Model):
     name = models.CharField(_("name"), max_length=150, unique=True)
     permissions = models.ManyToManyField(
         Permission,
         verbose_name=_("permissions"),
         blank=True,
+        related_name=permissions_related_name,
     )
 
     objects = GroupManager()
 
     class Meta:
         verbose_name = _("group")
         verbose_name_plural = _("groups")
```

### Comparing `django-group-model-1.0.0/django_group_model.egg-info/PKG-INFO` & `django-group-model-1.0.1/django_group_model.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-group-model
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django app to override the default Group model
 Author: Ankit Chhatbar
 Project-URL: Homepage, https://github.com/ankitchhatbar/django-group-model
 Project-URL: Documentation, https://github.com/ankitchhatbar/django-group-model
 Project-URL: Repository, https://github.com/ankitchhatbar/django-group-model
 Project-URL: Issues, https://github.com/ankitchhatbar/django-group-model/issues
 Classifier: Environment :: Web Environment
@@ -52,30 +52,32 @@
 
 - When starting a project, setting a custom Group model will allow you to customize it in the future when the need arises.
 
 ## Requirements
 
 - Python: 3.6+
 
-- Django: 3.0+
+- Django: 5.0, 4.2, 4.1, 4.0, 3.2, 3.1, 3.0
 
 ## Installation
 
 Install using pip:
 
 ```bash
 pip install django-group-model
 ```
 
-Add `'django_group_model'`  to your `INSTALLED_APPS`. Make sure to place it before any apps that define the `Group` or `User` models.
+Add `'django_group_model'` to your `INSTALLED_APPS`. Make sure to place it after the default Django apps (if any) and before any custom apps that define the `Group` or `User` models.
 
 ```python
 INSTALLED_APPS = [
     ...
-    'django_group_model',
+    'django.contrib.staticfiles',
+    'django_group_model', # Add this
+    ...
 ]
 ```
 
 ## Usage
 
 ### Overriding the default Group model
 
@@ -118,14 +120,23 @@
 
     )
     ...
 ```
 
 Once again, the name of the field is important. See below on how to customize the name of the model. Also take note of the `related_name` and `related_query_name`. Most of the time, the pattern shown above should work. For a deeper understanding see [Django docs here](https://docs.djangoproject.com/en/5.0/ref/models/fields/#django.db.models.ForeignKey.related_name).
 
+Since the name of the new model is `Group`, when accessing Groups attached to a permission, you will have to use the `custom_group_set` accessor.
+
+```python
+permisssion = Permisssion.objects.first()
+groups = permission.custom_group_set.all()
+```
+
+This only applies if your custom model is called `Group`. If you name it something else (see below). It will use Django's default conventions for the reverse accessor.
+
 ### Customizing the name of the Group model
 
 Overriding the default `Group` model with a custom name involves 2 steps:
 
 1. Create a model class that extends `AbstractGroup` with any name that you like.
 
 2. Override `verbose_name` and `verbose_name_plural` attributes of the `Meta` class.
```

### Comparing `django-group-model-1.0.0/pyproject.toml` & `django-group-model-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-group-model"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Ankit Chhatbar" },
 ]
 description = "A Django app to override the default Group model"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

