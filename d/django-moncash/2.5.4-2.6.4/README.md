# Comparing `tmp/django_moncash-2.5.4.tar.gz` & `tmp/django_moncash-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moncash-2.5.4.tar", last modified: Wed Apr 12 13:25:04 2023, max compression
+gzip compressed data, was "django_moncash-2.6.4.tar", last modified: Sat Apr 13 22:53:41 2024, max compression
```

## Comparing `django_moncash-2.5.4.tar` & `django_moncash-2.6.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-12 13:25:04.958658 django_moncash-2.5.4/
--rw-r--r--   0 macbook    (501) staff       (20)    35149 2023-04-06 01:43:10.000000 django_moncash-2.5.4/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)    49325 2023-04-12 13:25:04.958886 django_moncash-2.5.4/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     8192 2023-04-09 15:05:54.000000 django_moncash-2.5.4/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-12 13:25:04.956313 django_moncash-2.5.4/django_moncash/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.5.4/django_moncash/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      298 2023-04-07 14:53:44.000000 django_moncash-2.5.4/django_moncash/_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      722 2023-04-07 15:50:36.000000 django_moncash-2.5.4/django_moncash/admin.py
--rw-r--r--   0 macbook    (501) staff       (20)      159 2023-04-06 01:44:10.000000 django_moncash-2.5.4/django_moncash/apps.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-12 13:25:04.958496 django_moncash-2.5.4/django_moncash/migrations/
--rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-2.5.4/django_moncash/migrations/0001_initial.py
--rw-r--r--   0 macbook    (501) staff       (20)      636 2023-04-12 13:09:41.000000 django_moncash-2.5.4/django_moncash/migrations/0002_alter_transaction_user.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.5.4/django_moncash/migrations/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1132 2023-04-12 13:03:32.000000 django_moncash-2.5.4/django_moncash/models.py
--rw-r--r--   0 macbook    (501) staff       (20)       60 2023-04-06 01:44:10.000000 django_moncash-2.5.4/django_moncash/tests.py
--rw-r--r--   0 macbook    (501) staff       (20)      148 2023-04-06 18:01:13.000000 django_moncash-2.5.4/django_moncash/urls.py
--rw-r--r--   0 macbook    (501) staff       (20)     2526 2023-04-08 04:00:18.000000 django_moncash-2.5.4/django_moncash/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      564 2023-04-08 03:20:24.000000 django_moncash-2.5.4/django_moncash/views.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-12 13:25:04.957612 django_moncash-2.5.4/django_moncash.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)    49325 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      596 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       51 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       15 2023-04-12 13:25:04.000000 django_moncash-2.5.4/django_moncash.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)      809 2023-04-12 13:19:59.000000 django_moncash-2.5.4/pyproject.toml
--rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-12 13:25:04.959308 django_moncash-2.5.4/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)       96 2023-04-08 01:26:12.000000 django_moncash-2.5.4/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2024-04-13 22:53:41.249708 django_moncash-2.6.4/
+-rw-r--r--   0 macbook    (501) staff       (20)    35149 2023-04-06 01:43:10.000000 django_moncash-2.6.4/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)    49461 2024-04-13 22:53:41.249561 django_moncash-2.6.4/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     8192 2023-04-09 15:05:54.000000 django_moncash-2.6.4/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2024-04-13 22:53:41.245248 django_moncash-2.6.4/django_moncash/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.6.4/django_moncash/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      298 2023-04-07 14:53:44.000000 django_moncash-2.6.4/django_moncash/_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      748 2024-04-13 22:45:07.000000 django_moncash-2.6.4/django_moncash/admin.py
+-rw-r--r--   0 macbook    (501) staff       (20)      159 2023-04-06 01:44:10.000000 django_moncash-2.6.4/django_moncash/apps.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2024-04-13 22:53:41.248395 django_moncash-2.6.4/django_moncash/migrations/
+-rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-2.6.4/django_moncash/migrations/0001_initial.py
+-rw-r--r--   0 macbook    (501) staff       (20)      636 2023-04-12 13:09:41.000000 django_moncash-2.6.4/django_moncash/migrations/0002_alter_transaction_user.py
+-rw-r--r--   0 macbook    (501) staff       (20)      467 2024-04-13 22:46:54.000000 django_moncash-2.6.4/django_moncash/migrations/0003_transaction_transaction_id.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.6.4/django_moncash/migrations/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1257 2024-04-13 22:49:46.000000 django_moncash-2.6.4/django_moncash/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)       60 2023-04-06 01:44:10.000000 django_moncash-2.6.4/django_moncash/tests.py
+-rw-r--r--   0 macbook    (501) staff       (20)      148 2023-04-06 18:01:13.000000 django_moncash-2.6.4/django_moncash/urls.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2526 2023-04-08 04:00:18.000000 django_moncash-2.6.4/django_moncash/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      626 2024-04-13 22:48:42.000000 django_moncash-2.6.4/django_moncash/views.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2024-04-13 22:53:41.248643 django_moncash-2.6.4/django_moncash.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)    49461 2024-04-13 22:53:41.000000 django_moncash-2.6.4/django_moncash.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      657 2024-04-13 22:53:41.000000 django_moncash-2.6.4/django_moncash.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2024-04-13 22:53:41.000000 django_moncash-2.6.4/django_moncash.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       51 2024-04-13 22:53:41.000000 django_moncash-2.6.4/django_moncash.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       15 2024-04-13 22:53:41.000000 django_moncash-2.6.4/django_moncash.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      809 2024-04-13 22:50:11.000000 django_moncash-2.6.4/pyproject.toml
+-rw-r--r--   0 macbook    (501) staff       (20)      904 2024-04-13 22:53:41.250140 django_moncash-2.6.4/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)       96 2023-04-08 01:26:12.000000 django_moncash-2.6.4/setup.py
```

### Comparing `django_moncash-2.5.4/LICENSE` & `django_moncash-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_moncash-2.5.4/PKG-INFO` & `django_moncash-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_moncash
-Version: 2.5.4
+Version: 2.6.4
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 Author-email: Freedy Meritus <meritusfreedy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,16 +682,20 @@
 Project-URL: Homepage, https://github.com/undisplay/django_moncash
 Keywords: moncash,django,payment,SDK
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Django>=2.2
+Requires-Dist: moncash>=1.0.3
+Provides-Extra: dev
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 [![moncash](https://sandbox.moncashbutton.digicelgroup.com/Moncash-middleware/resources/assets/images/MC_button.png)](https://sandbox.moncashbutton.digicelgroup.com/)
 
 # Digicel Moncash API SDK for DJANGO
 
 
 Digicel MonCash - MonCash is a mobile wallet that facilitates reliable, safe and convenient financial transactions to reduce the distance between people regardless of their location in Haiti. While providing its services to its customer base of over 1.5 million people, MonCash maintains its goal of expanding its range of available services.
```

### Comparing `django_moncash-2.5.4/README.md` & `django_moncash-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `django_moncash-2.5.4/django_moncash/admin.py` & `django_moncash-2.6.4/django_moncash/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class TransactionAdmin(admin.ModelAdmin):
 
     list_display = (
         'id',
         'user',
         'order_id',
+        'transaction_id',
         'amount',
         'status',
         'return_url',
         'meta_data',
         'created_at',
         'updated_at',
     )
```

### Comparing `django_moncash-2.5.4/django_moncash/migrations/0001_initial.py` & `django_moncash-2.6.4/django_moncash/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.5.4/django_moncash/migrations/0002_alter_transaction_user.py` & `django_moncash-2.6.4/django_moncash/migrations/0002_alter_transaction_user.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.5.4/django_moncash/models.py` & `django_moncash-2.6.4/django_moncash/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
         related_name='moncash_transaction'
     )
 
     order_id = models.CharField(_("Order id"), max_length=50,default=uuid.uuid4,unique=True, editable=False)
+    transaction_id = models.CharField(_("Transaction id"), max_length=14,default=None,blank=False,null=False,editable=False)
     amount   = models.DecimalField(_("Amount"), max_digits=11, decimal_places=2,blank=False,null=False)
     status = models.CharField(_('Status'),max_length=25,choices=Status.choices,default=Status.PENDING,blank=False)
 
     return_url = models.TextField(_("Return URL"),blank=False,null=False)
 
     meta_data = models.JSONField(_("Meta data"),null=True,blank=True)
```

### Comparing `django_moncash-2.5.4/django_moncash/utils.py` & `django_moncash-2.6.4/django_moncash/utils.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.5.4/django_moncash/views.py` & `django_moncash-2.6.4/django_moncash/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 
     payment = verify_payment(request)
 
     transaction:Transaction = payment['transaction']
 
     if transaction:
         transaction.status = Transaction.Status.COMPLETE
+        transaction.transaction_id = payment['transactionId']
         transaction.save()
 
         return redirect(add_params(resolve_url(transaction.return_url),{"transactionId":payment['transactionId']}))
     else:
         raise Http404
```

### Comparing `django_moncash-2.5.4/django_moncash.egg-info/PKG-INFO` & `django_moncash-2.6.4/django_moncash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-moncash
-Version: 2.5.4
+Name: django_moncash
+Version: 2.6.4
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 Author-email: Freedy Meritus <meritusfreedy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,16 +682,20 @@
 Project-URL: Homepage, https://github.com/undisplay/django_moncash
 Keywords: moncash,django,payment,SDK
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Django>=2.2
+Requires-Dist: moncash>=1.0.3
+Provides-Extra: dev
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 [![moncash](https://sandbox.moncashbutton.digicelgroup.com/Moncash-middleware/resources/assets/images/MC_button.png)](https://sandbox.moncashbutton.digicelgroup.com/)
 
 # Digicel Moncash API SDK for DJANGO
 
 
 Digicel MonCash - MonCash is a mobile wallet that facilitates reliable, safe and convenient financial transactions to reduce the distance between people regardless of their location in Haiti. While providing its services to its customer base of over 1.5 million people, MonCash maintains its goal of expanding its range of available services.
```

### Comparing `django_moncash-2.5.4/django_moncash.egg-info/SOURCES.txt` & `django_moncash-2.6.4/django_moncash.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 django_moncash.egg-info/PKG-INFO
 django_moncash.egg-info/SOURCES.txt
 django_moncash.egg-info/dependency_links.txt
 django_moncash.egg-info/requires.txt
 django_moncash.egg-info/top_level.txt
 django_moncash/migrations/0001_initial.py
 django_moncash/migrations/0002_alter_transaction_user.py
+django_moncash/migrations/0003_transaction_transaction_id.py
 django_moncash/migrations/__init__.py
```

### Comparing `django_moncash-2.5.4/pyproject.toml` & `django_moncash-2.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_moncash"
-version = "2.5.4"
+version = "2.6.4"
 description = "Installable django moncash"
 readme = "README.md"
 authors = [{ name = "Freedy Meritus", email = "meritusfreedy@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

### Comparing `django_moncash-2.5.4/setup.cfg` & `django_moncash-2.6.4/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_moncash
-version = 2.5.4
+version = 2.6.4
 description = Installable django moncash
 long_description = file:README.md
 url = https://github.com/undisplay/django_moncash
 license = GNU
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

