# Comparing `tmp/jklib-5.0.2.tar.gz` & `tmp/jklib-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jklib-5.0.2.tar", last modified: Sun Feb 18 13:32:41 2024, max compression
+gzip compressed data, was "jklib-5.1.0.tar", last modified: Sun Apr 14 20:05:29 2024, max compression
```

## Comparing `jklib-5.0.2.tar` & `jklib-5.1.0.tar`

### file list

```diff
@@ -1,44 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 13:32:41.174334 jklib-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-18 13:32:30.000000 jklib-5.0.2/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-18 13:32:41.174334 jklib-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-18 13:32:30.000000 jklib-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 13:32:41.170334 jklib-5.0.2/jklib/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 13:32:41.174334 jklib-5.0.2/jklib/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4919 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/dj/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 13:32:41.174334 jklib-5.0.2/jklib/std/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-18 13:32:30.000000 jklib-5.0.2/jklib/std/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 13:32:41.174334 jklib-5.0.2/jklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-18 13:32:41.000000 jklib-5.0.2/jklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-18 13:32:41.000000 jklib-5.0.2/jklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 13:32:41.000000 jklib-5.0.2/jklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-18 13:32:41.000000 jklib-5.0.2/jklib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 13:32:41.174334 jklib-5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-18 13:32:30.000000 jklib-5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.076698 jklib-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-14 20:05:21.000000 jklib-5.1.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-14 20:05:29.076698 jklib-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-14 20:05:21.000000 jklib-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.068698 jklib-5.1.0/jklib/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.072698 jklib-5.1.0/jklib/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4919 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/dj/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.072698 jklib-5.1.0/jklib/meili/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.076698 jklib-5.1.0/jklib/meili/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/dj/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/dj/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/dj/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/meili/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.076698 jklib-5.1.0/jklib/std/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-14 20:05:21.000000 jklib-5.1.0/jklib/std/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:05:29.076698 jklib-5.1.0/jklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-14 20:05:29.000000 jklib-5.1.0/jklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-14 20:05:29.000000 jklib-5.1.0/jklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:05:29.000000 jklib-5.1.0/jklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 20:05:29.000000 jklib-5.1.0/jklib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:05:29.076698 jklib-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-14 20:05:21.000000 jklib-5.1.0/setup.py
```

### Comparing `jklib-5.0.2/LICENCE.txt` & `jklib-5.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/PKG-INFO` & `jklib-5.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jklib
-Version: 5.0.2
+Version: 5.1.0
 Summary: Package with utility functions on many different subjects
 Home-page: https://github.com/Jordan-Kowal/jklib
-Download-URL: https://github.com/Jordan-Kowal/jklib/archive/v5.0.2.tar.gz
+Download-URL: https://github.com/Jordan-Kowal/jklib/archive/v5.1.0.tar.gz
 Author: Jordan Kowal
 Author-email: kowaljordan@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 # jklib
 
 ## Description
 Package with useful snippets for Django and general Python development.
 
 The snippets are split into folders/categories:
 - `dj`: Web development around **Django** and **Django Rest Framework** 
+- `meili`: Utilities to interact with **MeiliSearch** (with a subfolder for `dj` **Django**)
 - `std`: Generic utilities around the standard library that can be used in any project 
 
 
 ## Pre-commit hooks
 The project uses `pre-commit` hooks to keep a consistent file structure
 
 As such, if you want to make some changes while using the pre-commit hooks:
```

### Comparing `jklib-5.0.2/jklib/dj/admin.py` & `jklib-5.1.0/jklib/dj/admin.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/decorators.py` & `jklib-5.1.0/jklib/dj/decorators.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/emails.py` & `jklib-5.1.0/jklib/dj/emails.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/exceptions.py` & `jklib-5.1.0/jklib/dj/exceptions.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/files.py` & `jklib-5.1.0/jklib/dj/files.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/images.py` & `jklib-5.1.0/jklib/dj/images.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/managers.py` & `jklib-5.1.0/jklib/dj/managers.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/models.py` & `jklib-5.1.0/jklib/dj/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,41 @@
 
 # Django
 from django import forms
 from django.db import IntegrityError, models
 from django.utils.deconstruct import deconstructible
 
 
+class ImprovedModel(models.Model):
+    class Meta:
+        abstract = True
+
+    def save(self, *args: Any, **kwargs: Any) -> None:
+        self._pre_save()
+        super().save(*args, **kwargs)
+        self._post_save()
+
+    def delete(self, *args: Any, **kwargs: Any) -> None:
+        self._pre_delete()
+        super().delete(*args, **kwargs)
+        self._post_delete()
+
+    def _pre_save(self) -> None:
+        pass
+
+    def _post_save(self) -> None:
+        pass
+
+    def _pre_delete(self) -> None:
+        pass
+
+    def _post_delete(self) -> None:
+        pass
+
+
 class PreCleanedAbstractModel(models.Model):
     """Model that calls .full_clean() before saving."""
 
     class Meta:
         abstract = True
 
     def save(self, *args: Any, **kwargs: Any) -> None:
@@ -26,14 +53,16 @@
             self.full_clean()
         except forms.ValidationError as e:
             raise IntegrityError(e)
         except Exception as e:
             raise e
 
 
+
+
 @deconstructible
 class FileNameWithUUID(object):
     """Generates a unique file name with a UUID."""
 
     def __init__(self, path: str) -> None:
         self.path = os.path.join(path, "%s%s")
```

### Comparing `jklib-5.0.2/jklib/dj/network.py` & `jklib-5.1.0/jklib/dj/network.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/permissions.py` & `jklib-5.1.0/jklib/dj/permissions.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/serializers.py` & `jklib-5.1.0/jklib/dj/serializers.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/test_runner.py` & `jklib-5.1.0/jklib/dj/test_runner.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/tests.py` & `jklib-5.1.0/jklib/dj/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
     ByteString,
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Type,
-    Union,
+    Union, OrderedDict,
 )
+from unittest.mock import Mock
 from urllib.parse import urlencode
 from zipfile import ZipFile
 
 # Django
 from django.contrib.sessions.models import Session
 from django.core import mail
 from django.core.files.uploadedfile import SimpleUploadedFile
@@ -57,136 +58,154 @@
 
     return decorator
 
 
 class AssertionTestCase(TestCase):
     """A `TestCase` with some assertion methods."""
 
+    def assertDictEqual(
+            self,
+            d1: Union[Dict, OrderedDict],
+            d2: Union[Dict, OrderedDict],
+            msg: Optional[str] = None,
+    ):
+        """Overrides `assertDictEqual` to handle `OrderedDict` instances."""
+        if isinstance(d1, OrderedDict):
+            d1 = dict(d1)
+        if isinstance(d2, OrderedDict):
+            d2 = dict(d2)
+        super().assertDictEqual(d1, d2, msg)
+
     def assertDateEqualsString(
-        self,
-        instance_date: Optional[Union[datetime.datetime, datetime.date]],
-        string_date: Optional[str],
-        format: Optional[str] = "%Y-%m-%dT%H:%M:%S.%fZ",
+            self,
+            instance_date: Optional[Union[datetime.datetime, datetime.date]],
+            string_date: Optional[str],
+            format: Optional[str] = "%Y-%m-%dT%H:%M:%S.%fZ",
     ):
         if not instance_date:
             self.assertIsNone(string_date)
         else:
             self.assertEqual(instance_date.strftime(format), string_date)
 
     def assertDownloadFile(self, response: Response, file_name: str) -> None:
         self.assertEqual(response.status_code, 200)
         self.assertEqual(
             response.get("Content-Disposition"),
             CONTENT_DISPOSITION.format(file_name=file_name),
         )
 
     def assertDownloadZipFile(
-        self, response: Response, file_name: str, zip_content: List[str]
+            self, response: Response, file_name: str, zip_content: List[str]
     ) -> None:
         self.assertEqual(response.status_code, 200)
         self.assertEqual(
             response.get("Content-Disposition"),
             CONTENT_DISPOSITION.format(file_name=file_name),
         )
         # Check the zip content
         myzip = ZipFile(BytesIO(response.getvalue()))
         zipped_files = set(myzip.namelist())
         self.assertSetEqual(set(zip_content), zipped_files)
 
     def assertEmailWasSent(
-        self,
-        subject: str,
-        to: Optional[List[str]] = None,
-        cc: Optional[List[str]] = None,
-        bcc: Optional[List[str]] = None,
+            self,
+            subject: str,
+            to: Optional[List[str]] = None,
+            cc: Optional[List[str]] = None,
+            bcc: Optional[List[str]] = None,
     ) -> None:
         email = mail.outbox[-1]
         self.assertEqual(email.subject, subject)
         if to is not None:
             self.assertEqual(len(to), len(email.to))
             self.assertSetEqual(set(to), set(email.to))
         if cc is not None:
             self.assertEqual(len(cc), len(email.cc))
             self.assertSetEqual(set(cc), set(email.cc))
         if bcc is not None:
             self.assertEqual(len(bcc), len(email.bcc))
             self.assertSetEqual(set(bcc), set(email.bcc))
 
     def assertFieldsHaveError(
-        self,
-        response: Response,
-        key_paths: List[str],
+            self,
+            response: Response,
+            key_paths: List[str],
     ) -> None:
         self.assertEqual(response.status_code, 400)
         for key_path in key_paths:
             # key_path example: "valves.0.description"
             value = response.data
             for key in key_path.split("."):
                 if isinstance(value, list):
                     value = value[int(key)]
                 else:
                     value = value.get(key)
             self.assertIsNotNone(value)
 
     def assertFileEqual(
-        self,
-        file_1: Union[FileField, SimpleUploadedFile],
-        file_2: Union[FileField, SimpleUploadedFile],
+            self,
+            file_1: Union[FileField, SimpleUploadedFile],
+            file_2: Union[FileField, SimpleUploadedFile],
     ) -> None:
         # Reset cursor position to make sure we compare the whole file
         file_1.seek(0)
         file_2.seek(0)
         # .read() must be stored within variable or it won't work
         content_1 = file_1.read()
         content_2 = file_2.read()
         self.assertEqual(content_1, content_2)
 
     def assertFileIsNone(self, file_field: FileField) -> None:
         self.assertFalse(bool(file_field))
 
     def assertImageToBase64(
-        self, img: ImageField, data: ByteString, resize_to: Optional[int] = None
+            self, img: ImageField, data: ByteString, resize_to: Optional[int] = None
     ):
         converted_image = (
             resized_image_to_base64(img, resize_to)
             if resize_to is not None
             else image_to_base64(img)
         )
         self.assertEqual(converted_image, data)
 
     def assertIntegrityErrorOnSave(self, instance: Model) -> None:
         with self.assertRaises(IntegrityError):
             instance.save()
 
     def assertQuerySetPks(
-        self, queryset: QuerySet, expected_pks=Iterable[Any], pk="id"
+            self, queryset: QuerySet, expected_pks=Iterable[Any], pk="id"
     ) -> None:
         queryset_pks = {getattr(item, pk) for item in queryset}
         self.assertSetEqual(queryset_pks, set(expected_pks))
 
+    def assertMockCalls(self, mock: Mock, expected_args: List) -> None:
+        self.assertEqual(len(mock.call_args_list), len(expected_args))
+        for (args, _kwargs), expected in zip(mock.call_args_list, expected_args):
+            self.assertEqual(args, expected)
+
 
 class ImprovedTestCase(AssertionTestCase):
     """Base TestCase with additional assertions and methods."""
 
     @staticmethod
     def build_fake_request(
-        method: str = "get", path: str = "/", data: Dict = None
+            method: str = "get", path: str = "/", data: Dict = None
     ) -> Request:
         factory = RequestFactory()
         factory_call = getattr(factory, method.lower())
         return factory_call(path, data=data)
 
     @staticmethod
     def generate_non_existing_id(model: Type[Model]) -> Any:
         instance = model.objects.all().order_by("-id").first()
         return 1 if not instance else instance.id + 1
 
     @staticmethod
     def uploaded_file_from_path(
-        filepath: str, upload_name: Optional[str] = None
+            filepath: str, upload_name: Optional[str] = None
     ) -> SimpleUploadedFile:
         if upload_name is None:
             upload_name = filepath.split("/")[-1]
         with open(filepath, "rb") as f:
             binary_content = f.read()
         return SimpleUploadedFile(
             name=upload_name,
@@ -204,17 +223,17 @@
     @classmethod
     def setUpClass(cls) -> None:
         cls.api_client = cls.api_client_class()
         super().setUpClass()
 
     @staticmethod
     def build_url(
-        name: str,
-        kwargs: Optional[Dict] = None,
-        query_kwargs: Optional[Dict] = None,
+            name: str,
+            kwargs: Optional[Dict] = None,
+            query_kwargs: Optional[Dict] = None,
     ) -> str:
         url = reverse(name, kwargs=kwargs)
         if query_kwargs is not None:
             url += f"?{urlencode(query_kwargs)}"
         return url
 
     @staticmethod
@@ -229,20 +248,20 @@
             Session.objects.filter(pk__in=user_active_session_ids).delete()
 
     @staticmethod
     def parse_streaming_response(response: StreamingHttpResponse) -> Union[Dict, List]:
         return json.loads(b"".join(response.streaming_content).decode("utf-8"))
 
     def multipart_api_call(
-        self,
-        method: str,
-        url: str,
-        payload: Dict[str, Any],
-        *args: Any,
-        **kwargs: Any,
+            self,
+            method: str,
+            url: str,
+            payload: Dict[str, Any],
+            *args: Any,
+            **kwargs: Any,
     ) -> Response:
         """Transforms a JSON payload into a flattened form-data and performs a
         multipart request."""
         flat_dict = dict_to_flat_dict(payload)
         data = encode_multipart(data=flat_dict, boundary=BOUNDARY)
         method = getattr(self.api_client, method.lower())
         return method(url, data=data, content_type=MULTIPART_CONTENT, *args, **kwargs)
```

### Comparing `jklib-5.0.2/jklib/dj/validators.py` & `jklib-5.1.0/jklib/dj/validators.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/dj/viewsets.py` & `jklib-5.1.0/jklib/dj/viewsets.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/std/files.py` & `jklib-5.1.0/jklib/std/files.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/std/images.py` & `jklib-5.1.0/jklib/std/images.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/std/inputs.py` & `jklib-5.1.0/jklib/std/inputs.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/std/strings.py` & `jklib-5.1.0/jklib/std/strings.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib/std/transforms.py` & `jklib-5.1.0/jklib/std/transforms.py`

 * *Files identical despite different names*

### Comparing `jklib-5.0.2/jklib.egg-info/PKG-INFO` & `jklib-5.1.0/jklib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jklib
-Version: 5.0.2
+Version: 5.1.0
 Summary: Package with utility functions on many different subjects
 Home-page: https://github.com/Jordan-Kowal/jklib
-Download-URL: https://github.com/Jordan-Kowal/jklib/archive/v5.0.2.tar.gz
+Download-URL: https://github.com/Jordan-Kowal/jklib/archive/v5.1.0.tar.gz
 Author: Jordan Kowal
 Author-email: kowaljordan@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 # jklib
 
 ## Description
 Package with useful snippets for Django and general Python development.
 
 The snippets are split into folders/categories:
 - `dj`: Web development around **Django** and **Django Rest Framework** 
+- `meili`: Utilities to interact with **MeiliSearch** (with a subfolder for `dj` **Django**)
 - `std`: Generic utilities around the standard library that can be used in any project 
 
 
 ## Pre-commit hooks
 The project uses `pre-commit` hooks to keep a consistent file structure
 
 As such, if you want to make some changes while using the pre-commit hooks:
```

### Comparing `jklib-5.0.2/jklib.egg-info/SOURCES.txt` & `jklib-5.1.0/jklib.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 jklib/dj/permissions.py
 jklib/dj/serializers.py
 jklib/dj/templates.py
 jklib/dj/test_runner.py
 jklib/dj/tests.py
 jklib/dj/validators.py
 jklib/dj/viewsets.py
+jklib/meili/__init__.py
+jklib/meili/search.py
+jklib/meili/types.py
+jklib/meili/dj/__init__.py
+jklib/meili/dj/indexer.py
+jklib/meili/dj/serializers.py
+jklib/meili/dj/test_utils.py
 jklib/std/__init__.py
 jklib/std/decorators.py
 jklib/std/files.py
 jklib/std/images.py
 jklib/std/inputs.py
 jklib/std/json.py
 jklib/std/maths.py
```

### Comparing `jklib-5.0.2/setup.py` & `jklib-5.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Third-party
 from setuptools import find_packages, setup
 
 # --------------------------------------------------------------------------------
 # > Variables
 # --------------------------------------------------------------------------------
-VERSION = "5.0.2"
+VERSION = "5.1.0"
 packages = find_packages()
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 # --------------------------------------------------------------------------------
 # > Setup
 # --------------------------------------------------------------------------------
```

