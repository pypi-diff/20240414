# Comparing `tmp/django-field-logger-0.0.26.tar.gz` & `tmp/django_field_logger-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-field-logger-0.0.26.tar", last modified: Fri Apr 12 04:48:05 2024, max compression
+gzip compressed data, was "django_field_logger-0.0.27.tar", last modified: Sun Apr 14 05:55:18 2024, max compression
```

## Comparing `django-field-logger-0.0.26.tar` & `django_field_logger-0.0.27.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 04:48:05.104840 django-field-logger-0.0.26/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.26/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.26/MANIFEST.in
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9914 2024-04-12 04:48:05.104840 django-field-logger-0.0.26/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7679 2024-04-12 03:39:00.000000 django-field-logger-0.0.26/README.rst
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 04:48:05.104840 django-field-logger-0.0.26/django_field_logger.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9914 2024-04-12 04:48:05.000000 django-field-logger-0.0.26/django_field_logger.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      530 2024-04-12 04:48:05.000000 django-field-logger-0.0.26/django_field_logger.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-12 04:48:05.000000 django-field-logger-0.0.26/django_field_logger.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-12 04:48:05.000000 django-field-logger-0.0.26/django_field_logger.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-12 04:48:05.000000 django-field-logger-0.0.26/django_field_logger.egg-info/top_level.txt
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 04:48:05.104840 django-field-logger-0.0.26/fieldlogger/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.26/fieldlogger/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.26/fieldlogger/apps.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3135 2024-04-08 14:39:49.000000 django-field-logger-0.0.26/fieldlogger/config.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      862 2024-04-01 09:39:30.000000 django-field-logger-0.0.26/fieldlogger/fieldlogger.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-01-17 04:38:48.000000 django-field-logger-0.0.26/fieldlogger/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2622 2024-04-12 03:07:50.000000 django-field-logger-0.0.26/fieldlogger/models.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-08 14:41:10.000000 django-field-logger-0.0.26/fieldlogger/signals.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      296 2024-03-27 00:36:10.000000 django-field-logger-0.0.26/fieldlogger/utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      497 2024-04-12 04:14:01.000000 django-field-logger-0.0.26/pyproject.toml
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1136 2024-04-12 04:48:05.104840 django-field-logger-0.0.26/setup.cfg
--rwxr-xr-x   0 nibblex   (1000) nibblex   (1000)       96 2024-04-12 04:05:44.000000 django-field-logger-0.0.26/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 04:48:05.104840 django-field-logger-0.0.26/tests/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-03-27 02:22:33.000000 django-field-logger-0.0.26/tests/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-11 07:12:55.000000 django-field-logger-0.0.26/tests/settings.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-11 07:23:31.000000 django-field-logger-0.0.26/tests/test_utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1788 2024-04-11 07:26:07.000000 django-field-logger-0.0.26/tests/tests.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-14 05:55:18.289301 django_field_logger-0.0.27/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django_field_logger-0.0.27/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django_field_logger-0.0.27/MANIFEST.in
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9914 2024-04-14 05:55:18.289301 django_field_logger-0.0.27/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7679 2024-04-12 03:39:00.000000 django_field_logger-0.0.27/README.rst
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-14 05:55:18.279302 django_field_logger-0.0.27/django_field_logger.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9914 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      554 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-14 05:55:18.000000 django_field_logger-0.0.27/django_field_logger.egg-info/top_level.txt
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-14 05:55:18.279302 django_field_logger-0.0.27/fieldlogger/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:51.000000 django_field_logger-0.0.27/fieldlogger/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-04-12 05:21:51.000000 django_field_logger-0.0.27/fieldlogger/apps.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2012 2024-04-14 05:54:20.000000 django_field_logger-0.0.27/fieldlogger/config.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1385 2024-04-14 05:50:25.000000 django_field_logger-0.0.27/fieldlogger/encoding.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      969 2024-04-14 05:37:12.000000 django_field_logger-0.0.27/fieldlogger/fieldlogger.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-04-12 05:21:51.000000 django_field_logger-0.0.27/fieldlogger/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2816 2024-04-14 05:50:03.000000 django_field_logger-0.0.27/fieldlogger/models.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-12 05:21:51.000000 django_field_logger-0.0.27/fieldlogger/signals.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      381 2024-04-14 05:36:16.000000 django_field_logger-0.0.27/fieldlogger/utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      497 2024-04-12 04:14:01.000000 django_field_logger-0.0.27/pyproject.toml
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1136 2024-04-14 05:55:18.289301 django_field_logger-0.0.27/setup.cfg
+-rwxr-xr-x   0 nibblex   (1000) nibblex   (1000)       96 2024-04-12 04:05:44.000000 django_field_logger-0.0.27/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-14 05:55:18.279302 django_field_logger-0.0.27/tests/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 05:21:35.000000 django_field_logger-0.0.27/tests/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-12 05:21:35.000000 django_field_logger-0.0.27/tests/settings.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-12 05:21:35.000000 django_field_logger-0.0.27/tests/test_utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1783 2024-04-14 05:52:42.000000 django_field_logger-0.0.27/tests/tests.py
```

### Comparing `django-field-logger-0.0.26/LICENSE` & `django_field_logger-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.26/PKG-INFO` & `django_field_logger-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.26
+Version: 0.0.27
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
```

### Comparing `django-field-logger-0.0.26/README.rst` & `django_field_logger-0.0.27/README.rst`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.26/django_field_logger.egg-info/PKG-INFO` & `django_field_logger-0.0.27/django_field_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.26
+Version: 0.0.27
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
```

### Comparing `django-field-logger-0.0.26/django_field_logger.egg-info/SOURCES.txt` & `django_field_logger-0.0.27/django_field_logger.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 django_field_logger.egg-info/SOURCES.txt
 django_field_logger.egg-info/dependency_links.txt
 django_field_logger.egg-info/requires.txt
 django_field_logger.egg-info/top_level.txt
 fieldlogger/__init__.py
 fieldlogger/apps.py
 fieldlogger/config.py
+fieldlogger/encoding.py
 fieldlogger/fieldlogger.py
 fieldlogger/mixins.py
 fieldlogger/models.py
 fieldlogger/signals.py
 fieldlogger/utils.py
 tests/__init__.py
 tests/settings.py
```

### Comparing `django-field-logger-0.0.26/fieldlogger/fieldlogger.py` & `django_field_logger-0.0.27/fieldlogger/fieldlogger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from typing import FrozenSet
+
 from django.core.exceptions import FieldDoesNotExist
 
-from .models import FieldLog
+from .models import FieldLog, LoggableModel
 from .utils import rgetattr
 
 
-def log_fields(instance, fields, pre_instance=None):
+def log_fields(
+    instance: LoggableModel, fields: FrozenSet[str], pre_instance: LoggableModel = None
+) -> dict:
     logs = {}
 
     instance.refresh_from_db(fields=fields)
 
     for field in fields:
         try:
             new_value = rgetattr(instance, field)
```

### Comparing `django-field-logger-0.0.26/fieldlogger/models.py` & `django_field_logger-0.0.27/fieldlogger/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import Callable, Dict, FrozenSet, NewType
+
 from django.apps import apps
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
-from .config import DECODER, ENCODER
+from .encoding import DECODER, ENCODER
 
 
 class FieldLog(models.Model):
     app_label = models.CharField(max_length=100, editable=False)
     model = models.CharField(_("model class name"), max_length=100, editable=False)
     instance_id = models.CharField(max_length=255, editable=False)
     field = models.CharField(_("field name"), max_length=100, editable=False)
@@ -66,7 +68,11 @@
                 instance_id=self.instance_id,
                 field=self.field,
             )
             .exclude(pk=self.pk)
             .order_by("pk")
             .last()
         )
+
+
+LoggableModel = NewType("LoggableModel", models.Model)
+Callback = Callable[[LoggableModel, FrozenSet[str], Dict[str, FieldLog]], None]
```

### Comparing `django-field-logger-0.0.26/fieldlogger/signals.py` & `django_field_logger-0.0.27/fieldlogger/signals.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.26/setup.cfg` & `django_field_logger-0.0.27/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-field-logger
-version = 0.0.26
+version = 0.0.27
 description = A Django app for logging changes in model fields.
 long_description = file: README.rst, LICENSE
 author = Sergio Rodríguez
 author_email = srodriguez3441@gmail.com
 maintainer = Sergio Rodríguez
 maintainer_email = srodriguez3441@gmail.com
 url = https://github.com/nibblex/django-field-logger
```

### Comparing `django-field-logger-0.0.26/tests/settings.py` & `django_field_logger-0.0.27/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.26/tests/test_utils.py` & `django_field_logger-0.0.27/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.26/tests/tests.py` & `django_field_logger-0.0.27/tests/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from importlib import reload
 
 import pytest
 
 from django.conf import settings
 
 from fieldlogger import config
-from tests.testapp.models import TestModel
 
 from .test_utils import (
     CREATE_FORM,
     UPDATE_FORM,
     _set_config,
     check_logs,
     set_attributes,
 )
+from .testapp.models import TestModel
 
 ORIGINAL_SETTINGS = settings.FIELD_LOGGER_SETTINGS.copy()
 
 
 @pytest.fixture
 def test_instance():
     # Create two instances for the foreign key field
```

