# Comparing `tmp/drf-appkit-1.4.4.tar.gz` & `tmp/drf_appkit-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-appkit-1.4.4.tar", last modified: Tue Apr  9 04:21:45 2024, max compression
+gzip compressed data, was "drf_appkit-1.4.5.tar", last modified: Sun Apr 14 15:51:06 2024, max compression
```

## Comparing `drf-appkit-1.4.4.tar` & `drf_appkit-1.4.5.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.123098 drf-appkit-1.4.4/
--rw-r--r--   0 allan      (501) staff       (20)     1511 2023-10-23 02:15:18.000000 drf-appkit-1.4.4/LICENSE
--rw-r--r--   0 allan      (501) staff       (20)       34 2024-03-10 01:31:35.000000 drf-appkit-1.4.4/MANIFEST.in
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-09 04:21:45.122992 drf-appkit-1.4.4/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)       99 2024-03-07 16:15:29.000000 drf-appkit-1.4.4/README.md
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.086725 drf-appkit-1.4.4/appkit/
--rw-r--r--   0 allan      (501) staff       (20)       45 2024-03-31 16:07:10.000000 drf-appkit-1.4.4/appkit/__init__.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.090200 drf-appkit-1.4.4/appkit/api/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/api/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)     4655 2024-03-24 15:35:29.000000 drf-appkit-1.4.4/appkit/api/filters.py
--rw-r--r--   0 allan      (501) staff       (20)     7912 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/api/mixins.py
--rw-r--r--   0 allan      (501) staff       (20)      963 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/api/pagination.py
--rw-r--r--   0 allan      (501) staff       (20)      391 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/api/relations.py
--rw-r--r--   0 allan      (501) staff       (20)     1959 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/api/renderers.py
--rw-r--r--   0 allan      (501) staff       (20)    14953 2024-03-20 23:00:29.000000 drf-appkit-1.4.4/appkit/api/serializers.py
--rw-r--r--   0 allan      (501) staff       (20)     5428 2024-04-01 16:02:52.000000 drf-appkit-1.4.4/appkit/api/tests.py
--rw-r--r--   0 allan      (501) staff       (20)    11983 2024-03-17 16:31:41.000000 drf-appkit-1.4.4/appkit/api/views.py
--rw-r--r--   0 allan      (501) staff       (20)      221 2024-03-31 16:07:10.000000 drf-appkit-1.4.4/appkit/apps.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.092840 drf-appkit-1.4.4/appkit/auth/
--rw-r--r--   0 allan      (501) staff       (20)      662 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/auth/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)      889 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/auth/backends.py
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/auth/decorators.py
--rw-r--r--   0 allan      (501) staff       (20)     1538 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/auth/email.py
--rw-r--r--   0 allan      (501) staff       (20)    14197 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/auth/permissions.py
--rw-r--r--   0 allan      (501) staff       (20)     1194 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/debug.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.097960 drf-appkit-1.4.4/appkit/drf/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/drf/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)      179 2024-03-12 20:44:52.000000 drf-appkit-1.4.4/appkit/drf/adapters.py
--rw-r--r--   0 allan      (501) staff       (20)     1068 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/drf/authentication.py
--rw-r--r--   0 allan      (501) staff       (20)      271 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/drf/backends.py
--rw-r--r--   0 allan      (501) staff       (20)     2022 2024-03-12 20:51:11.000000 drf-appkit-1.4.4/appkit/drf/endpoints.py
--rw-r--r--   0 allan      (501) staff       (20)      489 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/drf/exceptions.py
--rw-r--r--   0 allan      (501) staff       (20)     4014 2024-04-08 16:05:08.000000 drf-appkit-1.4.4/appkit/drf/fields.py
--rw-r--r--   0 allan      (501) staff       (20)     7399 2024-03-17 16:26:35.000000 drf-appkit-1.4.4/appkit/drf/filters.py
--rw-r--r--   0 allan      (501) staff       (20)     2775 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/drf/mixins.py
--rw-r--r--   0 allan      (501) staff       (20)      463 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/drf/permissions.py
--rw-r--r--   0 allan      (501) staff       (20)     2211 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/drf/serializers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.101251 drf-appkit-1.4.4/appkit/drf_appkit.egg-info/
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:27:12.000000 drf-appkit-1.4.4/appkit/drf_appkit.egg-info/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)     1884 2024-03-10 01:13:13.000000 drf-appkit-1.4.4/appkit/drf_appkit.egg-info/SOURCES.txt
--rw-r--r--   0 allan      (501) staff       (20)        1 2024-03-10 01:27:12.000000 drf-appkit-1.4.4/appkit/drf_appkit.egg-info/dependency_links.txt
--rw-r--r--   0 allan      (501) staff       (20)        7 2024-03-10 01:27:12.000000 drf-appkit-1.4.4/appkit/drf_appkit.egg-info/top_level.txt
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.101739 drf-appkit-1.4.4/appkit/forms/
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/forms/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)     1519 2024-04-02 17:59:09.000000 drf-appkit-1.4.4/appkit/forms/widgets.py
--rw-r--r--   0 allan      (501) staff       (20)      367 2024-03-31 16:07:10.000000 drf-appkit-1.4.4/appkit/handlers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.078127 drf-appkit-1.4.4/appkit/jinja2/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.078216 drf-appkit-1.4.4/appkit/jinja2/appkit/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.078311 drf-appkit-1.4.4/appkit/jinja2/appkit/forms/
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.102136 drf-appkit-1.4.4/appkit/jinja2/appkit/forms/widgets/
--rw-r--r--   0 allan      (501) staff       (20)      566 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/jinja2/appkit/forms/widgets/money_widget.html
--rw-r--r--   0 allan      (501) staff       (20)     8110 2024-03-10 01:08:12.000000 drf-appkit-1.4.4/appkit/managers.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.121636 drf-appkit-1.4.4/appkit/migrations/
--rw-r--r--   0 allan      (501) staff       (20)     9145 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0001_initial.py
--rw-r--r--   0 allan      (501) staff       (20)      395 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0002_arrangement_tags.py
--rw-r--r--   0 allan      (501) staff       (20)      575 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0003_auto_20210221_0852.py
--rw-r--r--   0 allan      (501) staff       (20)      400 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0004_auto_20210309_0655.py
--rw-r--r--   0 allan      (501) staff       (20)     1973 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0005_auto_20210324_1046.py
--rw-r--r--   0 allan      (501) staff       (20)      762 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0006_sitealias.py
--rw-r--r--   0 allan      (501) staff       (20)      393 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0007_auto_20211021_1901.py
--rw-r--r--   0 allan      (501) staff       (20)     1831 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0008_update_autofields.py
--rw-r--r--   0 allan      (501) staff       (20)     1000 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py
--rw-r--r--   0 allan      (501) staff       (20)      459 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0010_arrangement_name.py
--rw-r--r--   0 allan      (501) staff       (20)      362 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0011_alter_sitealias_options.py
--rw-r--r--   0 allan      (501) staff       (20)      543 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0012_alter_sitealias_site.py
--rw-r--r--   0 allan      (501) staff       (20)     1480 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0013_usergroup.py
--rw-r--r--   0 allan      (501) staff       (20)      802 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py
--rw-r--r--   0 allan      (501) staff       (20)      810 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py
--rw-r--r--   0 allan      (501) staff       (20)      846 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py
--rw-r--r--   0 allan      (501) staff       (20)      609 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0017_alter_imageattachment_image.py
--rw-r--r--   0 allan      (501) staff       (20)      987 2024-04-09 04:01:11.000000 drf-appkit-1.4.4/appkit/migrations/0018_place_geoposition.py
--rw-r--r--   0 allan      (501) staff       (20)      465 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0019_alter_place_geoposition.py
--rw-r--r--   0 allan      (501) staff       (20)      684 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py
--rw-r--r--   0 allan      (501) staff       (20)      407 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0021_rename_content_type_arrangement_item_type.py
--rw-r--r--   0 allan      (501) staff       (20)      655 2024-04-09 03:48:48.000000 drf-appkit-1.4.4/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py
--rw-r--r--   0 allan      (501) staff       (20)      330 2024-04-09 04:11:34.000000 drf-appkit-1.4.4/appkit/migrations/0023_delete_usergroup.py
--rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:13.000000 drf-appkit-1.4.4/appkit/migrations/__init__.py
--rw-r--r--   0 allan      (501) staff       (20)    12889 2024-04-09 03:42:16.000000 drf-appkit-1.4.4/appkit/models.py
--rw-r--r--   0 allan      (501) staff       (20)     2554 2024-03-31 20:07:19.000000 drf-appkit-1.4.4/appkit/notification.py
--rw-r--r--   0 allan      (501) staff       (20)      908 2024-03-10 01:08:13.000000 drf-appkit-1.4.4/appkit/settings.py
--rw-r--r--   0 allan      (501) staff       (20)     8645 2024-03-31 16:07:10.000000 drf-appkit-1.4.4/appkit/shortcuts.py
--rw-r--r--   0 allan      (501) staff       (20)      302 2024-03-10 01:08:13.000000 drf-appkit-1.4.4/appkit/storages.py
--rw-r--r--   0 allan      (501) staff       (20)     1026 2024-03-20 16:14:15.000000 drf-appkit-1.4.4/appkit/tasks.py
--rw-r--r--   0 allan      (501) staff       (20)     4829 2024-04-01 17:37:52.000000 drf-appkit-1.4.4/appkit/tests.py
--rw-r--r--   0 allan      (501) staff       (20)      899 2024-03-23 00:43:13.000000 drf-appkit-1.4.4/appkit/transformers.py
--rw-r--r--   0 allan      (501) staff       (20)    12388 2024-03-31 16:07:10.000000 drf-appkit-1.4.4/appkit/util.py
--rw-r--r--   0 allan      (501) staff       (20)      625 2024-03-10 01:08:13.000000 drf-appkit-1.4.4/appkit/views.py
-drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-09 04:21:45.122634 drf-appkit-1.4.4/drf_appkit.egg-info/
--rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-09 04:21:45.000000 drf-appkit-1.4.4/drf_appkit.egg-info/PKG-INFO
--rw-r--r--   0 allan      (501) staff       (20)     2556 2024-04-09 04:21:45.000000 drf-appkit-1.4.4/drf_appkit.egg-info/SOURCES.txt
--rw-r--r--   0 allan      (501) staff       (20)        1 2024-04-09 04:21:45.000000 drf-appkit-1.4.4/drf_appkit.egg-info/dependency_links.txt
--rw-r--r--   0 allan      (501) staff       (20)        7 2024-04-09 04:21:45.000000 drf-appkit-1.4.4/drf_appkit.egg-info/top_level.txt
--rw-r--r--   0 allan      (501) staff       (20)      790 2024-04-09 04:21:45.123526 drf-appkit-1.4.4/setup.cfg
--rw-r--r--   0 allan      (501) staff       (20)       38 2024-03-10 01:30:06.000000 drf-appkit-1.4.4/setup.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.945448 drf_appkit-1.4.5/
+-rw-r--r--   0 allan      (501) staff       (20)     1511 2023-10-23 02:15:18.000000 drf_appkit-1.4.5/LICENSE
+-rw-r--r--   0 allan      (501) staff       (20)       34 2024-03-10 01:31:35.000000 drf_appkit-1.4.5/MANIFEST.in
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-14 15:51:06.945366 drf_appkit-1.4.5/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)       99 2024-03-07 16:15:29.000000 drf_appkit-1.4.5/README.md
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.919349 drf_appkit-1.4.5/appkit/
+-rw-r--r--   0 allan      (501) staff       (20)       45 2024-03-31 16:07:10.000000 drf_appkit-1.4.5/appkit/__init__.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.921990 drf_appkit-1.4.5/appkit/api/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/api/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)     4655 2024-03-24 15:35:29.000000 drf_appkit-1.4.5/appkit/api/filters.py
+-rw-r--r--   0 allan      (501) staff       (20)     7912 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/api/mixins.py
+-rw-r--r--   0 allan      (501) staff       (20)      963 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/api/pagination.py
+-rw-r--r--   0 allan      (501) staff       (20)      391 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/api/relations.py
+-rw-r--r--   0 allan      (501) staff       (20)     1959 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/api/renderers.py
+-rw-r--r--   0 allan      (501) staff       (20)    15022 2024-04-14 15:03:48.000000 drf_appkit-1.4.5/appkit/api/serializers.py
+-rw-r--r--   0 allan      (501) staff       (20)     5428 2024-04-01 16:02:52.000000 drf_appkit-1.4.5/appkit/api/tests.py
+-rw-r--r--   0 allan      (501) staff       (20)    11983 2024-03-17 16:31:41.000000 drf_appkit-1.4.5/appkit/api/views.py
+-rw-r--r--   0 allan      (501) staff       (20)      221 2024-03-31 16:07:10.000000 drf_appkit-1.4.5/appkit/apps.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.923652 drf_appkit-1.4.5/appkit/auth/
+-rw-r--r--   0 allan      (501) staff       (20)      662 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/auth/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)      889 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/auth/backends.py
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/auth/decorators.py
+-rw-r--r--   0 allan      (501) staff       (20)     1538 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/auth/email.py
+-rw-r--r--   0 allan      (501) staff       (20)    14197 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/auth/permissions.py
+-rw-r--r--   0 allan      (501) staff       (20)     1194 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/debug.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.927347 drf_appkit-1.4.5/appkit/drf/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/drf/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)      179 2024-03-12 20:44:52.000000 drf_appkit-1.4.5/appkit/drf/adapters.py
+-rw-r--r--   0 allan      (501) staff       (20)     1068 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/drf/authentication.py
+-rw-r--r--   0 allan      (501) staff       (20)      271 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/drf/backends.py
+-rw-r--r--   0 allan      (501) staff       (20)     2022 2024-03-12 20:51:11.000000 drf_appkit-1.4.5/appkit/drf/endpoints.py
+-rw-r--r--   0 allan      (501) staff       (20)      489 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/drf/exceptions.py
+-rw-r--r--   0 allan      (501) staff       (20)     4014 2024-04-08 16:05:08.000000 drf_appkit-1.4.5/appkit/drf/fields.py
+-rw-r--r--   0 allan      (501) staff       (20)     7399 2024-03-17 16:26:35.000000 drf_appkit-1.4.5/appkit/drf/filters.py
+-rw-r--r--   0 allan      (501) staff       (20)     2775 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/drf/mixins.py
+-rw-r--r--   0 allan      (501) staff       (20)      463 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/drf/permissions.py
+-rw-r--r--   0 allan      (501) staff       (20)     2211 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/drf/serializers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.929211 drf_appkit-1.4.5/appkit/drf_appkit.egg-info/
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-03-10 01:27:12.000000 drf_appkit-1.4.5/appkit/drf_appkit.egg-info/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)     1884 2024-03-10 01:13:13.000000 drf_appkit-1.4.5/appkit/drf_appkit.egg-info/SOURCES.txt
+-rw-r--r--   0 allan      (501) staff       (20)        1 2024-03-10 01:27:12.000000 drf_appkit-1.4.5/appkit/drf_appkit.egg-info/dependency_links.txt
+-rw-r--r--   0 allan      (501) staff       (20)        7 2024-03-10 01:27:12.000000 drf_appkit-1.4.5/appkit/drf_appkit.egg-info/top_level.txt
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.929633 drf_appkit-1.4.5/appkit/forms/
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/forms/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)     1519 2024-04-02 17:59:09.000000 drf_appkit-1.4.5/appkit/forms/widgets.py
+-rw-r--r--   0 allan      (501) staff       (20)      367 2024-03-31 16:07:10.000000 drf_appkit-1.4.5/appkit/handlers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.913112 drf_appkit-1.4.5/appkit/jinja2/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.913168 drf_appkit-1.4.5/appkit/jinja2/appkit/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.913229 drf_appkit-1.4.5/appkit/jinja2/appkit/forms/
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.929909 drf_appkit-1.4.5/appkit/jinja2/appkit/forms/widgets/
+-rw-r--r--   0 allan      (501) staff       (20)      566 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/jinja2/appkit/forms/widgets/money_widget.html
+-rw-r--r--   0 allan      (501) staff       (20)     8110 2024-03-10 01:08:12.000000 drf_appkit-1.4.5/appkit/managers.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.944461 drf_appkit-1.4.5/appkit/migrations/
+-rw-r--r--   0 allan      (501) staff       (20)     9145 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0001_initial.py
+-rw-r--r--   0 allan      (501) staff       (20)      395 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0002_arrangement_tags.py
+-rw-r--r--   0 allan      (501) staff       (20)      575 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0003_auto_20210221_0852.py
+-rw-r--r--   0 allan      (501) staff       (20)      400 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0004_auto_20210309_0655.py
+-rw-r--r--   0 allan      (501) staff       (20)     1973 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0005_auto_20210324_1046.py
+-rw-r--r--   0 allan      (501) staff       (20)      762 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0006_sitealias.py
+-rw-r--r--   0 allan      (501) staff       (20)      393 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0007_auto_20211021_1901.py
+-rw-r--r--   0 allan      (501) staff       (20)     1831 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0008_update_autofields.py
+-rw-r--r--   0 allan      (501) staff       (20)     1000 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py
+-rw-r--r--   0 allan      (501) staff       (20)      459 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0010_arrangement_name.py
+-rw-r--r--   0 allan      (501) staff       (20)      362 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0011_alter_sitealias_options.py
+-rw-r--r--   0 allan      (501) staff       (20)      543 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0012_alter_sitealias_site.py
+-rw-r--r--   0 allan      (501) staff       (20)     1480 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0013_usergroup.py
+-rw-r--r--   0 allan      (501) staff       (20)      802 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py
+-rw-r--r--   0 allan      (501) staff       (20)      810 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py
+-rw-r--r--   0 allan      (501) staff       (20)      846 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py
+-rw-r--r--   0 allan      (501) staff       (20)      609 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0017_alter_imageattachment_image.py
+-rw-r--r--   0 allan      (501) staff       (20)      987 2024-04-09 04:01:11.000000 drf_appkit-1.4.5/appkit/migrations/0018_place_geoposition.py
+-rw-r--r--   0 allan      (501) staff       (20)      465 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0019_alter_place_geoposition.py
+-rw-r--r--   0 allan      (501) staff       (20)      684 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py
+-rw-r--r--   0 allan      (501) staff       (20)      407 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0021_rename_content_type_arrangement_item_type.py
+-rw-r--r--   0 allan      (501) staff       (20)      655 2024-04-09 03:48:48.000000 drf_appkit-1.4.5/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py
+-rw-r--r--   0 allan      (501) staff       (20)      330 2024-04-09 04:11:34.000000 drf_appkit-1.4.5/appkit/migrations/0023_delete_usergroup.py
+-rw-r--r--   0 allan      (501) staff       (20)      880 2024-04-14 14:51:58.000000 drf_appkit-1.4.5/appkit/migrations/0024_place_city_place_country_place_postal_code_and_more.py
+-rw-r--r--   0 allan      (501) staff       (20)        0 2024-03-10 01:08:13.000000 drf_appkit-1.4.5/appkit/migrations/__init__.py
+-rw-r--r--   0 allan      (501) staff       (20)    12684 2024-04-14 14:51:04.000000 drf_appkit-1.4.5/appkit/models.py
+-rw-r--r--   0 allan      (501) staff       (20)     2554 2024-03-31 20:07:19.000000 drf_appkit-1.4.5/appkit/notification.py
+-rw-r--r--   0 allan      (501) staff       (20)      908 2024-03-10 01:08:13.000000 drf_appkit-1.4.5/appkit/settings.py
+-rw-r--r--   0 allan      (501) staff       (20)     8645 2024-03-31 16:07:10.000000 drf_appkit-1.4.5/appkit/shortcuts.py
+-rw-r--r--   0 allan      (501) staff       (20)      302 2024-03-10 01:08:13.000000 drf_appkit-1.4.5/appkit/storages.py
+-rw-r--r--   0 allan      (501) staff       (20)     1026 2024-03-20 16:14:15.000000 drf_appkit-1.4.5/appkit/tasks.py
+-rw-r--r--   0 allan      (501) staff       (20)     4829 2024-04-01 17:37:52.000000 drf_appkit-1.4.5/appkit/tests.py
+-rw-r--r--   0 allan      (501) staff       (20)      899 2024-03-23 00:43:13.000000 drf_appkit-1.4.5/appkit/transformers.py
+-rw-r--r--   0 allan      (501) staff       (20)    12388 2024-03-31 16:07:10.000000 drf_appkit-1.4.5/appkit/util.py
+-rw-r--r--   0 allan      (501) staff       (20)      625 2024-03-10 01:08:13.000000 drf_appkit-1.4.5/appkit/views.py
+drwxr-xr-x   0 allan      (501) staff       (20)        0 2024-04-14 15:51:06.945136 drf_appkit-1.4.5/drf_appkit.egg-info/
+-rw-r--r--   0 allan      (501) staff       (20)      923 2024-04-14 15:51:06.000000 drf_appkit-1.4.5/drf_appkit.egg-info/PKG-INFO
+-rw-r--r--   0 allan      (501) staff       (20)     2634 2024-04-14 15:51:06.000000 drf_appkit-1.4.5/drf_appkit.egg-info/SOURCES.txt
+-rw-r--r--   0 allan      (501) staff       (20)        1 2024-04-14 15:51:06.000000 drf_appkit-1.4.5/drf_appkit.egg-info/dependency_links.txt
+-rw-r--r--   0 allan      (501) staff       (20)        7 2024-04-14 15:51:06.000000 drf_appkit-1.4.5/drf_appkit.egg-info/top_level.txt
+-rw-r--r--   0 allan      (501) staff       (20)      790 2024-04-14 15:51:06.945722 drf_appkit-1.4.5/setup.cfg
+-rw-r--r--   0 allan      (501) staff       (20)       38 2024-03-10 01:30:06.000000 drf_appkit-1.4.5/setup.py
```

### Comparing `drf-appkit-1.4.4/LICENSE` & `drf_appkit-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/PKG-INFO` & `drf_appkit-1.4.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-appkit
-Version: 1.4.4
+Version: 1.4.5
 Summary: A Django app providing generic CRUD functionality
 Author: Allan Hart
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-appkit-1.4.4/appkit/api/filters.py` & `drf_appkit-1.4.5/appkit/api/filters.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/api/mixins.py` & `drf_appkit-1.4.5/appkit/api/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/api/pagination.py` & `drf_appkit-1.4.5/appkit/api/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/api/renderers.py` & `drf_appkit-1.4.5/appkit/api/renderers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/api/serializers.py` & `drf_appkit-1.4.5/appkit/api/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,18 @@
 
 class PlaceSerializer(serializers.ModelSerializer):
     info = serializers.JSONField(read_only=True)
     place_id = serializers.CharField(read_only=True)
 
     class Meta:
         model = Place
-        fields = ('city', 'info', 'place_id',)
+        fields = (
+            'place_id', 'info',
+            'city', 'state', 'country', 'postal_code',
+        )
 
 
 class RegionSerializer(serializers.HyperlinkedModelSerializer):
     children = serializers.ListSerializer(child=RecursiveField())
 
     class Meta:
         model = Region
```

### Comparing `drf-appkit-1.4.4/appkit/api/tests.py` & `drf_appkit-1.4.5/appkit/api/tests.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/api/views.py` & `drf_appkit-1.4.5/appkit/api/views.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/auth/__init__.py` & `drf_appkit-1.4.5/appkit/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/auth/backends.py` & `drf_appkit-1.4.5/appkit/auth/backends.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/auth/decorators.py` & `drf_appkit-1.4.5/appkit/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/auth/email.py` & `drf_appkit-1.4.5/appkit/auth/email.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/auth/permissions.py` & `drf_appkit-1.4.5/appkit/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/debug.py` & `drf_appkit-1.4.5/appkit/debug.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/drf/authentication.py` & `drf_appkit-1.4.5/appkit/drf/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/drf/endpoints.py` & `drf_appkit-1.4.5/appkit/drf/endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/drf/fields.py` & `drf_appkit-1.4.5/appkit/drf/fields.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/drf/filters.py` & `drf_appkit-1.4.5/appkit/drf/filters.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/drf/mixins.py` & `drf_appkit-1.4.5/appkit/drf/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/drf/serializers.py` & `drf_appkit-1.4.5/appkit/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/drf_appkit.egg-info/PKG-INFO` & `drf_appkit-1.4.5/appkit/drf_appkit.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/drf_appkit.egg-info/SOURCES.txt` & `drf_appkit-1.4.5/appkit/drf_appkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/forms/widgets.py` & `drf_appkit-1.4.5/appkit/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/jinja2/appkit/forms/widgets/money_widget.html` & `drf_appkit-1.4.5/appkit/jinja2/appkit/forms/widgets/money_widget.html`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/managers.py` & `drf_appkit-1.4.5/appkit/managers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0001_initial.py` & `drf_appkit-1.4.5/appkit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0003_auto_20210221_0852.py` & `drf_appkit-1.4.5/appkit/migrations/0003_auto_20210221_0852.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0005_auto_20210324_1046.py` & `drf_appkit-1.4.5/appkit/migrations/0005_auto_20210324_1046.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0006_sitealias.py` & `drf_appkit-1.4.5/appkit/migrations/0006_sitealias.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0008_update_autofields.py` & `drf_appkit-1.4.5/appkit/migrations/0008_update_autofields.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py` & `drf_appkit-1.4.5/appkit/migrations/0009_alter_arrangement_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0012_alter_sitealias_site.py` & `drf_appkit-1.4.5/appkit/migrations/0012_alter_sitealias_site.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0013_usergroup.py` & `drf_appkit-1.4.5/appkit/migrations/0013_usergroup.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py` & `drf_appkit-1.4.5/appkit/migrations/0014_remove_note_notes_note_content_type_note_object_id.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py` & `drf_appkit-1.4.5/appkit/migrations/0015_alter_note_content_type_alter_note_object_id.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py` & `drf_appkit-1.4.5/appkit/migrations/0016_alter_arrangementitem_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0017_alter_imageattachment_image.py` & `drf_appkit-1.4.5/appkit/migrations/0017_alter_imageattachment_image.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0018_place_geoposition.py` & `drf_appkit-1.4.5/appkit/migrations/0018_place_geoposition.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py` & `drf_appkit-1.4.5/appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py` & `drf_appkit-1.4.5/appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/models.py` & `drf_appkit-1.4.5/appkit/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,34 +163,26 @@
             context={'date_scheduled': date_scheduled}
         )
 
 
 class Place(ModelBase):
     place_id = models.CharField(max_length=255, unique=True)
     geoposition = PointField(geography=True)
+
     info = models.JSONField()
+    city = models.CharField(max_length=50, blank=True)
+    state = models.CharField(max_length=2, blank=True)
+    country = models.CharField(max_length=30, blank=True)
+    postal_code = models.CharField(max_length=7, blank=True)
 
     def __str__(self):
         if 'formatted_address' in self.info:
             return self.info['formatted_address']
         return self.place_id
 
-    @property
-    def city(self):
-        formatted_address = self.info.get('formatted_address')
-        if formatted_address:
-            try:
-                # ASSUME: address is of the form: <city>, <state>, <country>
-                # and <state> is exactly two characters
-                return formatted_address[0:formatted_address.index(',') + 4]
-            except ValueError:
-                return None
-
-        return None
-
 
 class Region(MP_Node):
     name = models.CharField(max_length=150)
     slug = models.SlugField(max_length=150, blank=False, default=None)
     code = models.CharField(max_length=4, blank=True)
     place = models.ForeignKey(Place, blank=True, null=True, on_delete=models.SET_NULL)
```

### Comparing `drf-appkit-1.4.4/appkit/notification.py` & `drf_appkit-1.4.5/appkit/notification.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/settings.py` & `drf_appkit-1.4.5/appkit/settings.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/shortcuts.py` & `drf_appkit-1.4.5/appkit/shortcuts.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/tasks.py` & `drf_appkit-1.4.5/appkit/tasks.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/tests.py` & `drf_appkit-1.4.5/appkit/tests.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/transformers.py` & `drf_appkit-1.4.5/appkit/transformers.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/util.py` & `drf_appkit-1.4.5/appkit/util.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/appkit/views.py` & `drf_appkit-1.4.5/appkit/views.py`

 * *Files identical despite different names*

### Comparing `drf-appkit-1.4.4/drf_appkit.egg-info/PKG-INFO` & `drf_appkit-1.4.5/drf_appkit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-appkit
-Version: 1.4.4
+Version: 1.4.5
 Summary: A Django app providing generic CRUD functionality
 Author: Allan Hart
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-appkit-1.4.4/drf_appkit.egg-info/SOURCES.txt` & `drf_appkit-1.4.5/drf_appkit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -69,12 +69,13 @@
 appkit/migrations/0017_alter_imageattachment_image.py
 appkit/migrations/0018_place_geoposition.py
 appkit/migrations/0019_alter_place_geoposition.py
 appkit/migrations/0020_remove_arrangement_type_arrangement_content_type.py
 appkit/migrations/0021_rename_content_type_arrangement_item_type.py
 appkit/migrations/0022_imageattachment_rendition_key_imageattachment_warm.py
 appkit/migrations/0023_delete_usergroup.py
+appkit/migrations/0024_place_city_place_country_place_postal_code_and_more.py
 appkit/migrations/__init__.py
 drf_appkit.egg-info/PKG-INFO
 drf_appkit.egg-info/SOURCES.txt
 drf_appkit.egg-info/dependency_links.txt
 drf_appkit.egg-info/top_level.txt
```

### Comparing `drf-appkit-1.4.4/setup.cfg` & `drf_appkit-1.4.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drf-appkit
-version = 1.4.4
+version = 1.4.5
 description = A Django app providing generic CRUD functionality
 license = BSD
 long_description = file: README.md
 author = Allan Hart
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

