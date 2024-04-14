# Comparing `tmp/dekdjtools-0.1.6.tar.gz` & `tmp/dekdjtools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekdjtools-0.1.6.tar", last modified: Sun Apr  7 11:35:49 2024, max compression
+gzip compressed data, was "dekdjtools-0.1.7.tar", last modified: Sun Apr 14 15:48:38 2024, max compression
```

## Comparing `dekdjtools-0.1.6.tar` & `dekdjtools-0.1.7.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0       25 2024-04-07 11:35:47.823335 dekdjtools-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/admin/__init__.py
--rw-r--r--   0        0        0     2215 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/admin/base/__init__.py
--rw-r--r--   0        0        0      152 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/apps.py
--rw-r--r--   0        0        0      217 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/console.py
--rw-r--r--   0        0        0      117 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/dekshellplugin/__init__.py
--rw-r--r--   0        0        0     1663 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/dekshellplugin/markers/__init__.py
--rw-r--r--   0        0        0       93 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/fields/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/fields/data.py
--rw-r--r--   0        0        0      484 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/fields/image.py
--rw-r--r--   0        0        0      966 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/fields/snowflake.py
--rw-r--r--   0        0        0      967 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/fields/snowflakeid.py
--rw-r--r--   0        0        0        0 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/management/__init__.py
--rw-r--r--   0        0        0      255 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/management/base/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/management/commands/__init__.py
--rw-r--r--   0        0        0      328 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/management/commands/ddtdbreset.py
--rw-r--r--   0        0        0      782 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/management/commands/ddtdelmigrations.py
--rw-r--r--   0        0        0        0 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/migrations/__init__.py
--rw-r--r--   0        0        0       43 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/models/__init__.py
--rw-r--r--   0        0        0     2652 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/models/base/__init__.py
--rw-r--r--   0        0        0       34 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/settings.py
--rw-r--r--   0        0        0     1298 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/settings_app.py
--rw-r--r--   0        0        0     4473 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/snowflake.py
--rw-r--r--   0        0        0     1137 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/unionid.py
--rw-r--r--   0        0        0        0 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/utils/__init__.py
--rw-r--r--   0        0        0      558 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/utils/common.py
--rw-r--r--   0        0        0     1883 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/utils/finder.py
--rw-r--r--   0        0        0      862 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/utils/format.py
--rw-r--r--   0        0        0      914 2024-04-07 11:35:47.827335 dekdjtools-0.1.6/dekdjtools/utils/media.py
--rw-r--r--   0        0        0      799 2024-04-07 11:35:47.831335 dekdjtools-0.1.6/dekdjtools/utils/migration.py
--rw-r--r--   0        0        0     2918 2024-04-07 11:35:47.831335 dekdjtools-0.1.6/dekdjtools/utils/model.py
--rw-r--r--   0        0        0     2807 2024-04-07 11:35:47.831335 dekdjtools-0.1.6/dekdjtools/utils/query.py
--rw-r--r--   0        0        0     6473 2024-04-07 11:35:47.831335 dekdjtools-0.1.6/dekdjtools/utils/req.py
--rw-r--r--   0        0        0      441 2024-04-07 11:35:47.831335 dekdjtools-0.1.6/dekdjtools/utils/user.py
--rw-r--r--   0        0        0      655 2024-04-07 11:35:47.831335 dekdjtools-0.1.6/dekdjtools/validators.py
--rw-r--r--   0        0        0      632 2024-04-07 11:35:49.323367 dekdjtools-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 dekdjtools-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       25 2024-04-14 15:48:37.020076 dekdjtools-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 15:48:37.020076 dekdjtools-0.1.7/dekdjtools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 15:48:37.020076 dekdjtools-0.1.7/dekdjtools/admin/__init__.py
+-rw-r--r--   0        0        0     2215 2024-04-14 15:48:37.020076 dekdjtools-0.1.7/dekdjtools/admin/base/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-14 15:48:37.020076 dekdjtools-0.1.7/dekdjtools/apps.py
+-rw-r--r--   0        0        0      217 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/console.py
+-rw-r--r--   0        0        0      117 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/dekshellplugin/__init__.py
+-rw-r--r--   0        0        0     1663 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/dekshellplugin/markers/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/fields/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/fields/data.py
+-rw-r--r--   0        0        0      484 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/fields/image.py
+-rw-r--r--   0        0        0      966 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/fields/snowflake.py
+-rw-r--r--   0        0        0      967 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/fields/snowflakeid.py
+-rw-r--r--   0        0        0        0 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/management/__init__.py
+-rw-r--r--   0        0        0      255 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/management/base/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/management/commands/__init__.py
+-rw-r--r--   0        0        0      328 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/management/commands/ddtdbreset.py
+-rw-r--r--   0        0        0      782 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/management/commands/ddtdelmigrations.py
+-rw-r--r--   0        0        0        0 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/migrations/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/models/__init__.py
+-rw-r--r--   0        0        0     2652 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/models/base/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/settings.py
+-rw-r--r--   0        0        0     1298 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/settings_app.py
+-rw-r--r--   0        0        0     1528 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/settings_generate.py
+-rw-r--r--   0        0        0     4473 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/snowflake.py
+-rw-r--r--   0        0        0     1137 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/unionid.py
+-rw-r--r--   0        0        0        0 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/__init__.py
+-rw-r--r--   0        0        0      558 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/common.py
+-rw-r--r--   0        0        0     1883 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/finder.py
+-rw-r--r--   0        0        0      862 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/format.py
+-rw-r--r--   0        0        0      914 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/media.py
+-rw-r--r--   0        0        0      799 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/migration.py
+-rw-r--r--   0        0        0     2918 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/model.py
+-rw-r--r--   0        0        0     2807 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/query.py
+-rw-r--r--   0        0        0     6473 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/req.py
+-rw-r--r--   0        0        0      441 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/utils/user.py
+-rw-r--r--   0        0        0      655 2024-04-14 15:48:37.024076 dekdjtools-0.1.7/dekdjtools/validators.py
+-rw-r--r--   0        0        0      632 2024-04-14 15:48:38.272076 dekdjtools-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 dekdjtools-0.1.7/PKG-INFO
```

### Comparing `dekdjtools-0.1.6/dekdjtools/admin/base/__init__.py` & `dekdjtools-0.1.7/dekdjtools/admin/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/dekshellplugin/markers/__init__.py` & `dekdjtools-0.1.7/dekdjtools/dekshellplugin/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/fields/data.py` & `dekdjtools-0.1.7/dekdjtools/fields/data.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/fields/snowflake.py` & `dekdjtools-0.1.7/dekdjtools/fields/snowflake.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/fields/snowflakeid.py` & `dekdjtools-0.1.7/dekdjtools/fields/snowflakeid.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/management/commands/ddtdelmigrations.py` & `dekdjtools-0.1.7/dekdjtools/management/commands/ddtdelmigrations.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/models/base/__init__.py` & `dekdjtools-0.1.7/dekdjtools/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/settings_app.py` & `dekdjtools-0.1.7/dekdjtools/settings_app.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/snowflake.py` & `dekdjtools-0.1.7/dekdjtools/snowflake.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/unionid.py` & `dekdjtools-0.1.7/dekdjtools/unionid.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/utils/common.py` & `dekdjtools-0.1.7/dekdjtools/utils/common.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/utils/finder.py` & `dekdjtools-0.1.7/dekdjtools/utils/finder.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/utils/format.py` & `dekdjtools-0.1.7/dekdjtools/utils/format.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/utils/media.py` & `dekdjtools-0.1.7/dekdjtools/utils/media.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/utils/migration.py` & `dekdjtools-0.1.7/dekdjtools/utils/migration.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/utils/model.py` & `dekdjtools-0.1.7/dekdjtools/utils/model.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/utils/query.py` & `dekdjtools-0.1.7/dekdjtools/utils/query.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/utils/req.py` & `dekdjtools-0.1.7/dekdjtools/utils/req.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/dekdjtools/validators.py` & `dekdjtools-0.1.7/dekdjtools/validators.py`

 * *Files identical despite different names*

### Comparing `dekdjtools-0.1.6/pyproject.toml` & `dekdjtools-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dekdjtools"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = [
     { name = "sanzenwin", email = "sanzenwin@gmail.com" },
 ]
 dependencies = [
     "django<=3.2.18",
     "django-extensions<=2.1.6",
```

