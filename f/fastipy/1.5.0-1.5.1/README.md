# Comparing `tmp/fastipy-1.5.0.tar.gz` & `tmp/fastipy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastipy-1.5.0.tar", last modified: Mon Jan 29 02:56:31 2024, max compression
+gzip compressed data, was "fastipy-1.5.1.tar", last modified: Sun Apr 14 19:38:18 2024, max compression
```

## Comparing `fastipy-1.5.0.tar` & `fastipy-1.5.1.tar`

### file list

```diff
@@ -1,69 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.234434 fastipy-1.5.0/
--rw-rw-rw-   0        0        0    35823 2024-01-24 23:42:42.000000 fastipy-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     7166 2024-01-29 02:56:31.233429 fastipy-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     6022 2024-01-29 02:49:58.000000 fastipy-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.179097 fastipy-1.5.0/app/
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.186097 fastipy-1.5.0/app/fastipy/
--rw-rw-rw-   0        0        0      416 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.192155 fastipy-1.5.0/app/fastipy/src/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.193155 fastipy-1.5.0/app/fastipy/src/classes/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/classes/__init__.py
--rw-rw-rw-   0        0        0      437 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/classes/decorators_base.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.200512 fastipy-1.5.0/app/fastipy/src/constants/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/constants/__init__.py
--rw-rw-rw-   0        0        0      744 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/constants/content_types.py
--rw-rw-rw-   0        0        0       40 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/constants/decorators.py
--rw-rw-rw-   0        0        0      106 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/constants/events.py
--rw-rw-rw-   0        0        0      162 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/constants/hooks.py
--rw-rw-rw-   0        0        0      169 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/constants/http_methods.py
--rw-rw-rw-   0        0        0     1355 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/constants/http_status_code.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.204646 fastipy-1.5.0/app/fastipy/src/core/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/core/__init__.py
--rw-rw-rw-   0        0        0    10760 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/core/fastipy.py
--rw-rw-rw-   0        0        0    14414 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/core/reply.py
--rw-rw-rw-   0        0        0     2893 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/core/request.py
--rw-rw-rw-   0        0        0     4591 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/core/request_handler.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.207160 fastipy-1.5.0/app/fastipy/src/database/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/database/__init__.py
--rw-rw-rw-   0        0        0     2162 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/database/json_database.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.218262 fastipy-1.5.0/app/fastipy/src/exceptions/
--rw-rw-rw-   0        0        0      374 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/__init__.py
--rw-rw-rw-   0        0        0      128 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/decorator_already_exists_exception.py
--rw-rw-rw-   0        0        0      120 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/duplicate_route_exception.py
--rw-rw-rw-   0        0        0     1598 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/exception_handler.py
--rw-rw-rw-   0        0        0       98 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/fastipy_base_exception.py
--rw-rw-rw-   0        0        0      110 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/file_exception.py
--rw-rw-rw-   0        0        0      117 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/invalid_path_exception.py
--rw-rw-rw-   0        0        0      117 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/no_event_type.py
--rw-rw-rw-   0        0        0      116 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/no_hook_type.py
--rw-rw-rw-   0        0        0      118 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/no_http_method_exception.py
--rw-rw-rw-   0        0        0      110 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/exceptions/reply_exception.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.221347 fastipy-1.5.0/app/fastipy/src/helpers/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/helpers/__init__.py
--rw-rw-rw-   0        0        0      529 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/helpers/async_sync_helpers.py
--rw-rw-rw-   0        0        0      752 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/helpers/route_helpers.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.222931 fastipy-1.5.0/app/fastipy/src/middlewares/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/middlewares/__init__.py
--rw-rw-rw-   0        0        0     1435 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/middlewares/cors.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.227131 fastipy-1.5.0/app/fastipy/src/models/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/models/__init__.py
--rw-rw-rw-   0        0        0     1435 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/models/body.py
--rw-rw-rw-   0        0        0     2028 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/models/file.py
--rw-rw-rw-   0        0        0     1560 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/models/form.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.230435 fastipy-1.5.0/app/fastipy/src/routes/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/routes/__init__.py
--rw-rw-rw-   0        0        0      956 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/routes/plugin_tree.py
--rw-rw-rw-   0        0        0     2834 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/routes/router.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.232744 fastipy-1.5.0/app/fastipy/src/types/
--rw-rw-rw-   0        0        0        0 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/types/__init__.py
--rw-rw-rw-   0        0        0      215 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/types/plugins.py
--rw-rw-rw-   0        0        0      539 2024-01-28 21:50:11.000000 fastipy-1.5.0/app/fastipy/src/types/routes.py
-drwxrwxrwx   0        0        0        0 2024-01-29 02:56:31.191157 fastipy-1.5.0/app/fastipy.egg-info/
--rw-rw-rw-   0        0        0     7166 2024-01-29 02:56:30.000000 fastipy-1.5.0/app/fastipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1936 2024-01-29 02:56:31.000000 fastipy-1.5.0/app/fastipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 02:56:30.000000 fastipy-1.5.0/app/fastipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-01-29 02:56:30.000000 fastipy-1.5.0/app/fastipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-29 02:56:30.000000 fastipy-1.5.0/app/fastipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-29 02:56:31.234434 fastipy-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1491 2024-01-29 02:56:28.000000 fastipy-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.711053 fastipy-1.5.1/
+-rw-rw-rw-   0        0        0    35823 2024-04-14 01:52:52.000000 fastipy-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     7908 2024-04-14 19:38:18.709200 fastipy-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6656 2024-04-14 19:33:49.000000 fastipy-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.648155 fastipy-1.5.1/app/
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.656710 fastipy-1.5.1/app/fastipy/
+-rw-rw-rw-   0        0        0      694 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.662756 fastipy-1.5.1/app/fastipy/src/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.667752 fastipy-1.5.1/app/fastipy/src/classes/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/classes/__init__.py
+-rw-rw-rw-   0        0        0      484 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/classes/decorators_base.py
+-rw-rw-rw-   0        0        0     2892 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/classes/json_database.py
+-rw-rw-rw-   0        0        0     4071 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/classes/mailer.py
+-rw-rw-rw-   0        0        0     1764 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/classes/template_render.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.675113 fastipy-1.5.1/app/fastipy/src/constants/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/constants/__init__.py
+-rw-rw-rw-   0        0        0      802 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/content_types.py
+-rw-rw-rw-   0        0        0       42 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/decorators.py
+-rw-rw-rw-   0        0        0      108 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/events.py
+-rw-rw-rw-   0        0        0      164 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/hooks.py
+-rw-rw-rw-   0        0        0      171 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/http_methods.py
+-rw-rw-rw-   0        0        0     1443 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/http_status_code.py
+-rw-rw-rw-   0        0        0     1024 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/constants/serializers.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.680149 fastipy-1.5.1/app/fastipy/src/core/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/core/__init__.py
+-rw-rw-rw-   0        0        0    11795 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/core/fastipy.py
+-rw-rw-rw-   0        0        0    15888 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/core/reply.py
+-rw-rw-rw-   0        0        0     3113 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/core/request.py
+-rw-rw-rw-   0        0        0     5043 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/core/request_handler.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.691490 fastipy-1.5.1/app/fastipy/src/exceptions/
+-rw-rw-rw-   0        0        0      860 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      134 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/decorator_already_exists_exception.py
+-rw-rw-rw-   0        0        0      126 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/duplicate_route_exception.py
+-rw-rw-rw-   0        0        0     1645 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/exception_handler.py
+-rw-rw-rw-   0        0        0      411 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/fastipy_base_exception.py
+-rw-rw-rw-   0        0        0      116 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/file_exception.py
+-rw-rw-rw-   0        0        0      123 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/invalid_path_exception.py
+-rw-rw-rw-   0        0        0      123 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/no_event_type.py
+-rw-rw-rw-   0        0        0      122 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/no_hook_type.py
+-rw-rw-rw-   0        0        0      124 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/no_http_method_exception.py
+-rw-rw-rw-   0        0        0      117 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/exceptions/reply_exception.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.696502 fastipy-1.5.1/app/fastipy/src/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/helpers/__init__.py
+-rw-rw-rw-   0        0        0      531 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/helpers/async_sync_helpers.py
+-rw-rw-rw-   0        0        0      318 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/helpers/content_type.py
+-rw-rw-rw-   0        0        0     1144 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/helpers/route_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.698502 fastipy-1.5.1/app/fastipy/src/middlewares/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     1686 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/middlewares/cors.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.701199 fastipy-1.5.1/app/fastipy/src/models/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/models/__init__.py
+-rw-rw-rw-   0        0        0     1575 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/models/body.py
+-rw-rw-rw-   0        0        0     2127 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/models/file.py
+-rw-rw-rw-   0        0        0     2030 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/models/form.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.704198 fastipy-1.5.1/app/fastipy/src/routes/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/routes/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/routes/plugin_tree.py
+-rw-rw-rw-   0        0        0     4212 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/routes/router.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.707190 fastipy-1.5.1/app/fastipy/src/types/
+-rw-rw-rw-   0        0        0        0 2024-04-14 01:52:52.000000 fastipy-1.5.1/app/fastipy/src/types/__init__.py
+-rw-rw-rw-   0        0        0      225 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/types/plugins.py
+-rw-rw-rw-   0        0        0      557 2024-04-14 19:33:49.000000 fastipy-1.5.1/app/fastipy/src/types/routes.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:38:18.708190 fastipy-1.5.1/app/fastipy.egg-info/
+-rw-rw-rw-   0        0        0     7908 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2056 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-14 19:38:18.000000 fastipy-1.5.1/app/fastipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 19:38:18.711053 fastipy-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2024-04-14 19:33:49.000000 fastipy-1.5.1/setup.py
```

### Comparing `fastipy-1.5.0/LICENSE` & `fastipy-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastipy-1.5.0/PKG-INFO` & `fastipy-1.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastipy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.
 Home-page: https://github.com/Bielgomes/Fastipy
 Author: Bielgomes
 Author-email: bielgomesdasilva@hotmail.com
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/Bielgomes/Fastipy/issues
 Classifier: Development Status :: 4 - Beta
@@ -17,19 +17,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: uvicorn[standard]
+Requires-Dist: starlette
+Requires-Dist: nest-asyncio
+Requires-Dist: Jinja2
 
 # Fastipy
 
 <div>
-  <img src="https://media.discordapp.net/attachments/887158781832749086/1187385388571037778/fastipy-extended.png">
+  <img src="https://i.imgur.com/KCi8IUS.png">
 </div>
 
 ## What is it and what is it for
 
 [Fastipy](https://pypi.org/project/Fastipy/) is a fast and easy-to-use open source Python library for developing RESTful APIs.
 
 Powered by **[uvicorn](https://www.uvicorn.org/)**
@@ -38,109 +42,144 @@
 
 ```bash
 pip install fastipy
 ```
 
 ## Examples
 
-### Example for GET Route with Query Params and debug mode
+### Example for GET Route with Query Params
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
-# Debug mode is False by default
 app = Fastipy()
 
 # Routes can be async or sync functions, but reply send functions are async
 # The handler returns the default HTTP status code 200
 @app.get('/')
-def home(req: Request, reply: Reply):
+def home(req: Request, _):
   # Get query params age
   age = req.query['age']
   # Example: Recovery all persons from database with this age and print the html
-  print("<h1>Listing all persons</h1><ul><li>A Person</li></ul>")
+  print("<h1>Retrieving all persons</h1><ul><li>A Person</li></ul>")
 ```
 
 ### Example for GET Route with Params, CORS and multiple methods
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy().cors()
 
 @app.get('/user/:id')
 @app.post('/user/:id')
 async def getUser(req: Request, reply: Reply):
   # get users from database
   for i in users:
     if i["id"] == req.params["id"]:
-      await reply.json(i).send()
-      return
+      # All response functions are asynchronous
+      return await reply.send(i)
+
   await reply.send_code(404)
 ```
 
 ### Example for POST Route with Body
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 @app.post('/user')
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Save user in database
-  await reply.text("Created").code(201).send()
+  await reply.code(201).send("Created")
 ```
 
 ### Example for PUT Route with Body
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 @app.put('/user')
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Update user in database
-  await reply.html('<h1>Created</h1>').code(201).send()
+  await reply.type("text/html").code(201).send("<h1>Created</h1>")
+```
+
+### Example for GET Route with file stream
+
+```py
+from fastipy import Fastipy, Request, Reply
+
+app = Fastipy()
+
+@app.get('/stream')
+async def streamFile(_, reply: Reply):
+  # It could be an asynchronous generator
+  def generator():
+    with open("file.txt") as f:
+        for line in f:
+            yield line
+
+  await reply.send(generator())
+```
+
+### Adding custom serializer to Reply send
+
+```py
+from fastipy import Fastipy, Request, Reply
+
+app = Fastipy()
+
+app.add_serializer(
+    validation=lambda data: isinstance(data, str),
+    serializer=lambda data: ("application/json", json.dumps({"error": data})),
+)
+
+@app.get("/")
+async def customSerializer(_, reply: Reply):
+    await reply.code(404).send("Field not found")
 ```
 
 ### See more examples in **[examples](https://github.com/Bielgomes/Fastipy/tree/main/examples)** folder
 
 ## Creating plugins
 
 ```py
 # chat.py
 from fastipy import FastipyInstance, Reply
 
 # Plugins can be asynchronous or synchronized functions
-# Plugins have the main instance as a parameter, which means they can use all of Fastipy's functions
+# Plugins have access to the main instance, which means they can use all of Fastipy's functions
 def chatRoutes(app: FastipyInstance, options: dict):
   @app.get('/')
-  async def index(req: Request, reply: Reply):
+  async def index(_, reply: Reply):
     await reply.send_code(200)
 
   @app.get('/chat')
-  async def test(req: Request, reply: Reply):
+  async def test(_, reply: Reply):
     await reply.send_code(200)
 ```
 
 ```py
 # message.py
 from fastipy import FastipyInstance, Reply
 
 async def messageRoutes(app: FastipyInstance, options: dict):
   @message.get('/')
-  async def index(req: Request, reply: Reply):
+  async def index(_, reply: Reply):
     await reply.send_code(200)
 
   @message.get('/message')
-  async def test(req: Request, reply: Reply):
+  async def test(_, reply: Reply):
     await reply.send_code(200)
 
   app.name('custom plugin name')
 ```
 
 ```py
 # main.py
@@ -175,27 +214,41 @@
 # The onResponse hook is called when the reply sends a response
 @app.hook('onResponse')
 def onResponse(req: Request, reply: Reply):
   print('onResponse hook')
 
 # The onError hook is called when an error occurs
 @app.hook('onError')
-def onError(req: Request, reply: Reply, error):
-  print('onError hook')
+def onError(error: Exception, req: Request, reply: Reply):
+  print(f'onError hook exception: {error}')
 
 # A hook will only be linked to a route if its declaration precedes the route
 # The order of hooks of the same type is important
 @app.get('/')
-async def index(req: Request, reply: Reply):
+async def index(_, reply: Reply):
   await reply.send_code(200)
 ```
 
+## End to End tests
+
+```py
+# See more in https://www.starlette.io/testclient/
+from fastipy import TestClient
+from main import app
+
+client = TestClient(app)
+
+response = client.post("/")
+assert response.status_code == 200
+assert response.text == "Hello World"
+```
+
 ## Running
 
-Run Fastipy application in development is easy
+Running Fastipy application in development is easy
 
 ```py
 import uvicorn
 
 if __name__ == "__main__":
   # main:app indicates the FILE:VARIABLE
 
@@ -211,45 +264,33 @@
 
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Version 1.5.0
+## Development Version 1.5.1
 
 ### Added
 
-- [x] Request method PATCH
-- [x] More security in CORS
-- [x] JSON Database module
-- [x] Add support to hooks (onRequest, onResponse, onError)
-- [x] Add support to plugins
-- [x] Add decorators to routes (decorator, decorate_request, decorate_reply)
-- [x] Add support to middlewares
-- [x] Add support for lifespan events (startup, shutdown)
-- [x] New preHandler hook
-- [x] Add stream file support
-- [x] Automatic OPTIONS method response for routes
-- [x] Custom global error handler
+- [X] Added the possibility of printing middleware routes in the router's print tree.
+- [X] Added a customizable mail module.
+- [X] Added jinja2 lib to render templates.
+- [x] Add integration to end-to-end tests.
 
 ### Changed
 
-- [x] Better params and query params recovery in routes
-- [x] Improved route logging
-- [x] Refactor structure of project
-- [x] Refactor Routes class
-- [x] Routes handler can be a sync function
-- [x] Better route search algorithm and structure
-- [x] It is now possible to add specific hooks and middlewares to a route
-- [x] Implementation of uvicorn HTTP web server
-- [x] Better error handler
+- [X] Error imports are now centralized in the exceptions module.
+- [X] Improved error handling flow, now error handling hooks are executed first rather than the default error handling.
+- [X] Apply code reuse to generate logs.
+- [X] Refactored file stream in reply send file function.
+- [X] Reply send function now automatically serializes the value sent to it and sets a content type
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
 
 ## How to Contributing
 
-Open pull request ðŸ˜Ž
+Open pull request
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastipy-1.5.0/README.md` & `fastipy-1.5.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Fastipy
 
 <div>
-  <img src="https://media.discordapp.net/attachments/887158781832749086/1187385388571037778/fastipy-extended.png">
+  <img src="https://i.imgur.com/KCi8IUS.png">
 </div>
 
 ## What is it and what is it for
 
 [Fastipy](https://pypi.org/project/Fastipy/) is a fast and easy-to-use open source Python library for developing RESTful APIs.
 
 Powered by **[uvicorn](https://www.uvicorn.org/)**
@@ -14,109 +14,144 @@
 
 ```bash
 pip install fastipy
 ```
 
 ## Examples
 
-### Example for GET Route with Query Params and debug mode
+### Example for GET Route with Query Params
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
-# Debug mode is False by default
 app = Fastipy()
 
 # Routes can be async or sync functions, but reply send functions are async
 # The handler returns the default HTTP status code 200
 @app.get('/')
-def home(req: Request, reply: Reply):
+def home(req: Request, _):
   # Get query params age
   age = req.query['age']
   # Example: Recovery all persons from database with this age and print the html
-  print("<h1>Listing all persons</h1><ul><li>A Person</li></ul>")
+  print("<h1>Retrieving all persons</h1><ul><li>A Person</li></ul>")
 ```
 
 ### Example for GET Route with Params, CORS and multiple methods
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy().cors()
 
 @app.get('/user/:id')
 @app.post('/user/:id')
 async def getUser(req: Request, reply: Reply):
   # get users from database
   for i in users:
     if i["id"] == req.params["id"]:
-      await reply.json(i).send()
-      return
+      # All response functions are asynchronous
+      return await reply.send(i)
+
   await reply.send_code(404)
 ```
 
 ### Example for POST Route with Body
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 @app.post('/user')
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Save user in database
-  await reply.text("Created").code(201).send()
+  await reply.code(201).send("Created")
 ```
 
 ### Example for PUT Route with Body
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 @app.put('/user')
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Update user in database
-  await reply.html('<h1>Created</h1>').code(201).send()
+  await reply.type("text/html").code(201).send("<h1>Created</h1>")
+```
+
+### Example for GET Route with file stream
+
+```py
+from fastipy import Fastipy, Request, Reply
+
+app = Fastipy()
+
+@app.get('/stream')
+async def streamFile(_, reply: Reply):
+  # It could be an asynchronous generator
+  def generator():
+    with open("file.txt") as f:
+        for line in f:
+            yield line
+
+  await reply.send(generator())
+```
+
+### Adding custom serializer to Reply send
+
+```py
+from fastipy import Fastipy, Request, Reply
+
+app = Fastipy()
+
+app.add_serializer(
+    validation=lambda data: isinstance(data, str),
+    serializer=lambda data: ("application/json", json.dumps({"error": data})),
+)
+
+@app.get("/")
+async def customSerializer(_, reply: Reply):
+    await reply.code(404).send("Field not found")
 ```
 
 ### See more examples in **[examples](https://github.com/Bielgomes/Fastipy/tree/main/examples)** folder
 
 ## Creating plugins
 
 ```py
 # chat.py
 from fastipy import FastipyInstance, Reply
 
 # Plugins can be asynchronous or synchronized functions
-# Plugins have the main instance as a parameter, which means they can use all of Fastipy's functions
+# Plugins have access to the main instance, which means they can use all of Fastipy's functions
 def chatRoutes(app: FastipyInstance, options: dict):
   @app.get('/')
-  async def index(req: Request, reply: Reply):
+  async def index(_, reply: Reply):
     await reply.send_code(200)
 
   @app.get('/chat')
-  async def test(req: Request, reply: Reply):
+  async def test(_, reply: Reply):
     await reply.send_code(200)
 ```
 
 ```py
 # message.py
 from fastipy import FastipyInstance, Reply
 
 async def messageRoutes(app: FastipyInstance, options: dict):
   @message.get('/')
-  async def index(req: Request, reply: Reply):
+  async def index(_, reply: Reply):
     await reply.send_code(200)
 
   @message.get('/message')
-  async def test(req: Request, reply: Reply):
+  async def test(_, reply: Reply):
     await reply.send_code(200)
 
   app.name('custom plugin name')
 ```
 
 ```py
 # main.py
@@ -151,27 +186,41 @@
 # The onResponse hook is called when the reply sends a response
 @app.hook('onResponse')
 def onResponse(req: Request, reply: Reply):
   print('onResponse hook')
 
 # The onError hook is called when an error occurs
 @app.hook('onError')
-def onError(req: Request, reply: Reply, error):
-  print('onError hook')
+def onError(error: Exception, req: Request, reply: Reply):
+  print(f'onError hook exception: {error}')
 
 # A hook will only be linked to a route if its declaration precedes the route
 # The order of hooks of the same type is important
 @app.get('/')
-async def index(req: Request, reply: Reply):
+async def index(_, reply: Reply):
   await reply.send_code(200)
 ```
 
+## End to End tests
+
+```py
+# See more in https://www.starlette.io/testclient/
+from fastipy import TestClient
+from main import app
+
+client = TestClient(app)
+
+response = client.post("/")
+assert response.status_code == 200
+assert response.text == "Hello World"
+```
+
 ## Running
 
-Run Fastipy application in development is easy
+Running Fastipy application in development is easy
 
 ```py
 import uvicorn
 
 if __name__ == "__main__":
   # main:app indicates the FILE:VARIABLE
 
@@ -187,45 +236,33 @@
 
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Version 1.5.0
+## Development Version 1.5.1
 
 ### Added
 
-- [x] Request method PATCH
-- [x] More security in CORS
-- [x] JSON Database module
-- [x] Add support to hooks (onRequest, onResponse, onError)
-- [x] Add support to plugins
-- [x] Add decorators to routes (decorator, decorate_request, decorate_reply)
-- [x] Add support to middlewares
-- [x] Add support for lifespan events (startup, shutdown)
-- [x] New preHandler hook
-- [x] Add stream file support
-- [x] Automatic OPTIONS method response for routes
-- [x] Custom global error handler
+- [X] Added the possibility of printing middleware routes in the router's print tree.
+- [X] Added a customizable mail module.
+- [X] Added jinja2 lib to render templates.
+- [x] Add integration to end-to-end tests.
 
 ### Changed
 
-- [x] Better params and query params recovery in routes
-- [x] Improved route logging
-- [x] Refactor structure of project
-- [x] Refactor Routes class
-- [x] Routes handler can be a sync function
-- [x] Better route search algorithm and structure
-- [x] It is now possible to add specific hooks and middlewares to a route
-- [x] Implementation of uvicorn HTTP web server
-- [x] Better error handler
+- [X] Error imports are now centralized in the exceptions module.
+- [X] Improved error handling flow, now error handling hooks are executed first rather than the default error handling.
+- [X] Apply code reuse to generate logs.
+- [X] Refactored file stream in reply send file function.
+- [X] Reply send function now automatically serializes the value sent to it and sets a content type
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
 
 ## How to Contributing
 
-Open pull request 😎
+Open pull request
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastipy-1.5.0/app/fastipy/src/core/fastipy.py` & `fastipy-1.5.1/app/fastipy/src/core/fastipy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,289 +1,360 @@
-from typing import Dict, Optional, Self
-from uvicorn.main import logger
 import re, copy, click, nest_asyncio
-
-from ..types.plugins import PluginOptions
-from ..types.routes import FunctionType, RouteHookType, RouteMiddlewareType
+from typing import Callable, Dict, Optional, Self
+from uvicorn.main import logger
 
 from ..constants.hooks import HOOKS, hookType
 from ..constants.http_methods import HTTP_METHODS, httpMethodType
 from ..constants.decorators import DECORATORS
 from ..constants.events import EVENTS, eventType
+from ..constants.serializers import SERIALIZERS
 
-from ..exceptions.invalid_path_exception import InvalidPathException
-from ..exceptions.duplicate_route_exception import DuplicateRouteException
-from ..exceptions.no_hook_type import NoHookTypeException
-from ..exceptions.no_http_method_exception import NoHTTPMethodException
-from ..exceptions.decorator_already_exists_exception import DecoratorAlreadyExistsException
-from ..exceptions.no_event_type import NoEventTypeException
+from ..types.plugins import PluginOptions
+from ..types.routes import FunctionType, RouteHookType, RouteMiddlewareType
+
+from ..exceptions import (
+    InvalidPathException,
+    DuplicateRouteException,
+    NoHookTypeException,
+    NoHTTPMethodException,
+    DecoratorAlreadyExistsException,
+    NoEventTypeException,
+)
 
 from ..helpers.async_sync_helpers import run_sync_or_async
 
 from ..classes.decorators_base import DecoratorsBase
 from .request_handler import RequestHandler
 
 from .request import Request
 from .reply import Reply
 
 from ..routes.router import Router
 from ..routes.plugin_tree import PluginTree, PluginNode
 
 from ..middlewares.cors import CORSGenerator
 
+
 class Fastipy(RequestHandler, DecoratorsBase):
-  def __init__(self, static_path: str = None) -> None:
-    self._router        = Router()
-    self._plugins       = PluginTree()
-    self._cors          = None
-    self._prefix        = '/'
-    self._name          = None
-    self._static_path   = static_path
-    self._error_handler = None
-
-    self._decorators    = {decorator: {} for decorator in DECORATORS}
-    self._hooks         = {hook_type: [] for hook_type in HOOKS}
-    self._middlewares   = []
-    self._events        = {event_type: [] for event_type in EVENTS}
-
-    self._instance_decorators = self._decorators['app']
-
-    nest_asyncio.apply()
-
-  @property
-  def prefix(self) -> str:
-    return self._prefix
-
-  @property
-  def name(self) -> str:
-    return self._name
-
-  @property
-  def cors(self) -> CORSGenerator:
-    return self._cors
-
-  @property
-  def static(self) -> str:
-    return self._static_path
-  
-  def set_name(self, name: str) -> None:
-    self._name = name
-  
-  def print_routes(self, options: Dict[str, any] = {}) -> None:
-    self._router.print_tree(options=options)
-
-  def print_plugins(self) -> None:
-    self._plugins.print_tree()
-  
-  def set_error_handler(self, handler: FunctionType) -> None:
-    self._error_handler = handler
-
-  def error_handler(self) -> FunctionType:
-    def internal(handler: FunctionType) -> FunctionType:
-      self.set_error_handler(handler)
-      return handler
-    return internal
-  
-  def add_event(self, event_type: eventType, event: FunctionType) -> None:
-    if event_type not in EVENTS:
-      message = f"Failed to register event [{event_type}] >> Type not supported"
-      logger.error(NoEventTypeException(message))
-      raise NoEventTypeException(message)
-    
-    self._events[event_type].append(event)
-  
-  def on(self, event_type: eventType) -> FunctionType:
-    def internal(event: FunctionType) -> FunctionType:
-      self.add_event(event_type, event)
-      return event
-    return internal
-
-  def register(self, plugin: FunctionType, options: PluginOptions = {}) -> Self:
-    instance = FastipyInstance()
-
-    instance._router = self._router
-    instance._static_path = self._static_path
-    instance._plugins = PluginNode(plugin.__name__)
-    instance._decorators = self._decorators
-    instance._hooks = self._hooks
-    instance._middlewares = self._middlewares
-    instance._events = self._events
-    instance._instance_decorators = self._instance_decorators
-
-    instance._prefix = options.get('prefix', '/')
-    
-    run_sync_or_async(plugin, instance, options)
-
-    self._error_handler = instance._error_handler
-
-    if instance._name is not None: instance._plugins.name = instance._name
-    self._plugins.add_child(instance._plugins)
-
-    return self
-
-  def cors(
-    self,
-    allow_origin: str = '*',
-    allow_headers: str = '*',
-    allow_methods: str = '*',
-    allow_credentials: bool = True,
-    expose_headers: Optional[str] = None,
-    max_age: Optional[int] = None,
-    content_security_policy: str = "default-src 'self'",
-    custom_headers: dict = {}
-  ) -> 'Fastipy':
-    self._cors = CORSGenerator(
-      allow_origin,
-      allow_headers,
-      allow_methods,
-      allow_credentials,
-      expose_headers,
-      max_age,
-      content_security_policy,
-      custom_headers
-    )
-    return self
-
-  def decorate(self, name: str, value: any) -> None:
-    if hasattr(self, name) or self.has_decorator(name):
-      message = f"Failed to register decorator '{name}' >> Duplicate decorator"
-      logger.error(DecoratorAlreadyExistsException(message))
-      raise DecoratorAlreadyExistsException(message)
-    
-    self._decorators['app'][name] = value
-
-  def decorate_request(self, name: str, value: any) -> None:
-    if hasattr(Request, name) or self.has_request_decorator(name):
-      message = f"Failed to register request decorator '{name}' >> Duplicate decorator"
-      logger.error(DecoratorAlreadyExistsException(message))
-      raise DecoratorAlreadyExistsException(message)
-    
-    self._decorators['request'][name] = value
-
-  def decorate_reply(self, name: str, value: any) -> None:
-    if hasattr(Reply, name) or self.has_reply_decorator(name):
-      message = f"Failed to register reply decorator '{name}' >> Duplicate decorator"
-      logger.error(DecoratorAlreadyExistsException(message))
-      raise DecoratorAlreadyExistsException(message)
-    
-    self._decorators['reply'][name] = value
-
-  def has_decorator(self, name: str) -> bool:
-    return name in self._decorators['app']
-  
-  def has_request_decorator(self, name: str) -> bool:
-    return name in self._decorators['request']
-  
-  def has_reply_decorator(self, name: str) -> bool:
-    return name in self._decorators['reply']
-
-  def add_hook(self, hook_type: hookType, hook: FunctionType) -> None:
-    if hook_type not in HOOKS:
-      message = f"Failed to register hook [{hook_type}] >> Type not supported"
-      logger.error(NoHookTypeException(message))
-      raise NoHookTypeException(message)
-    
-    self._hooks[hook_type].append(hook)
-
-  def hook(self, hook_type: hookType) -> FunctionType:
-    def internal(hook: FunctionType) -> FunctionType:
-      self.add_hook(hook_type, hook)
-      return hook
-    return internal
-
-  def add_middleware(self, middleware: FunctionType) -> None:
-    self._middlewares.append(middleware)
-
-  def use(self) -> FunctionType:
-    def internal(middleware: FunctionType) -> FunctionType:
-      self.add_middleware(middleware)
-      return middleware
-    return internal
-
-  def add_route(
-    self, 
-    method: httpMethodType,
-    path: str,
-    handler: FunctionType,
-    route_hooks: RouteHookType = {},
-    route_middlewares: RouteMiddlewareType = []
-  ) -> None:
-    if self.prefix != '/':
-      path = f"{self.prefix}{path if path != '/' else ''}"
-    if method not in HTTP_METHODS:
-      message = f"Failed to register route [{method}] '{path}' >> Method not supported"
-      logger.error(NoHTTPMethodException(message))
-      raise NoHTTPMethodException(message)
-
-    if (not re.fullmatch(r"^(\/:?[_a-zA-Z0-9]+)*$|^\/$", path) or re.search(r':(\d)\w+', path) or len(re.findall(r':(\w+)', path)) != len(set(re.findall(r':(\w+)', path)))):
-      message = f"Failed to register route [{method}] '{path}' >> Invalid path"
-      logger.error(InvalidPathException(message))
-      raise InvalidPathException(message)
-
-    routeAlreadyExists = self._router.find_route(method, path) is not None
-    if routeAlreadyExists:
-      message = f"Failed to register route [{method}] '{path}' >> Duplicate route"
-      logger.error(DuplicateRouteException(message))
-      raise DuplicateRouteException(message)
-    
-    hooks = copy.deepcopy(self._hooks)
-    hooks.update(route_hooks)
-
-    middlewares = copy.deepcopy(self._middlewares)
-    middlewares.extend(route_middlewares)
-    
-    self._router.add_route(method, path, {
-      'handler': handler,
-      'hooks': hooks,
-      'middlewares': middlewares,
-      'raw_path': path
-    })
-
-    message = f"Route registered [%s] '{path}'"
-    color_message = "Route registered [" + click.style("%s", fg="cyan") + f"] '{path}'"
-    logger.debug(message, method, extra={"color_message": color_message})
-
-  def get(self, path: str, route_hooks: RouteHookType = {}, route_middlewares: RouteMiddlewareType = []) -> FunctionType:
-    def internal(handler: FunctionType) -> FunctionType:
-      self.add_route('GET', path, handler, route_hooks, route_middlewares)
-      return handler
-    return internal
-
-  def post(self, path: str, route_hooks: RouteHookType = {}, route_middlewares: RouteMiddlewareType = []) -> FunctionType:
-    def internal(handler: FunctionType) -> FunctionType:
-      self.add_route('POST', path, handler, route_hooks, route_middlewares)
-      return handler
-    return internal
-
-  def put(self, path: str, route_hooks: RouteHookType = {}, route_middlewares: RouteMiddlewareType = []) -> FunctionType:
-    def internal(handler: FunctionType) -> FunctionType:
-      self.add_route('PUT', path, handler, route_hooks, route_middlewares)
-      return handler
-    return internal
-
-  def patch(self, path: str, route_hooks: RouteHookType = {}, route_middlewares: RouteMiddlewareType = []) -> FunctionType:
-    def internal(handler: FunctionType) -> FunctionType:
-      self.add_route('PATCH', path, handler, route_hooks, route_middlewares)
-      return handler
-    return internal
-
-  def delete(self, path: str, route_hooks: RouteHookType = {}, route_middlewares: RouteMiddlewareType = []) -> FunctionType:
-    def internal(handler: FunctionType) -> FunctionType:
-      self.add_route('DELETE', path, handler, route_hooks, route_middlewares)
-      return handler
-    return internal
-
-  def head(self, path: str, route_hooks: RouteHookType = {}, route_middlewares: RouteMiddlewareType = []) -> FunctionType:
-    def internal(handler: FunctionType) -> FunctionType:
-      self.add_route('HEAD', path, handler, route_hooks, route_middlewares)
-      return handler
-    return internal
+    def __init__(self, static_path: str = None) -> None:
+        self._router = Router()
+        self._plugins = PluginTree()
+        self._cors = None
+        self._prefix = "/"
+        self._name = None
+        self._static_path = static_path
+        self._error_handler = None
+
+        self._decorators = {decorator: {} for decorator in DECORATORS}
+        self._hooks = {hook_type: [] for hook_type in HOOKS}
+        self._middlewares = []
+        self._events = {event_type: [] for event_type in EVENTS}
+        self._serializers = SERIALIZERS
+
+        self._instance_decorators = self._decorators["app"]
+
+        nest_asyncio.apply()
+
+    @property
+    def prefix(self) -> str:
+        return self._prefix
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def cors(self) -> CORSGenerator:
+        return self._cors
+
+    @property
+    def static(self) -> str:
+        return self._static_path
+
+    def set_name(self, name: str) -> None:
+        self._name = name
+
+    def print_routes(self, options: Dict[str, any] = {}) -> None:
+        self._router.print_tree(options=options)
+
+    def print_plugins(self) -> None:
+        self._plugins.print_tree()
+
+    def set_error_handler(self, handler: FunctionType) -> None:
+        self._error_handler = handler
+
+    def error_handler(self) -> FunctionType:
+        def internal(handler: FunctionType) -> FunctionType:
+            self.set_error_handler(handler)
+            return handler
+
+        return internal
+
+    def add_event(self, event_type: eventType, event: FunctionType) -> None:
+        if event_type not in EVENTS:
+            raise NoEventTypeException(
+                f"Failed to register event [{event_type}] >> Type not supported",
+                logger.error,
+            )
+
+        self._events[event_type].append(event)
+
+    def on(self, event_type: eventType) -> FunctionType:
+        def internal(event: FunctionType) -> FunctionType:
+            self.add_event(event_type, event)
+            return event
+
+        return internal
+
+    def register(self, plugin: FunctionType, options: PluginOptions = {}) -> Self:
+        instance = FastipyInstance()
+
+        instance._router = self._router
+        instance._static_path = self._static_path
+        instance._plugins = PluginNode(plugin.__name__)
+        instance._decorators = self._decorators
+        instance._hooks = self._hooks
+        instance._middlewares = self._middlewares
+        instance._events = self._events
+        instance._instance_decorators = self._instance_decorators
+
+        instance._prefix = options.get("prefix", "/")
+
+        run_sync_or_async(plugin, instance, options)
+
+        self._error_handler = instance._error_handler
+
+        if instance._name is not None:
+            instance._plugins.name = instance._name
+        self._plugins.add_child(instance._plugins)
+
+        return self
+
+    def cors(
+        self,
+        allow_origin: str = "*",
+        allow_headers: str = "*",
+        allow_methods: str = "*",
+        allow_credentials: bool = True,
+        expose_headers: Optional[str] = None,
+        max_age: Optional[int] = None,
+        content_security_policy: str = "default-src 'self'",
+        custom_headers: dict = {},
+    ) -> "Fastipy":
+        self._cors = CORSGenerator(
+            allow_origin,
+            allow_headers,
+            allow_methods,
+            allow_credentials,
+            expose_headers,
+            max_age,
+            content_security_policy,
+            custom_headers,
+        )
+        return self
+
+    def decorate(self, name: str, value: any) -> None:
+        if hasattr(self, name) or self.has_decorator(name):
+            raise DecoratorAlreadyExistsException(
+                f"Failed to register decorator '{name}' >> Duplicate decorator",
+                logger.error,
+            )
+
+        self._decorators["app"][name] = value
+
+    def decorate_request(self, name: str, value: any) -> None:
+        if hasattr(Request, name) or self.has_request_decorator(name):
+            raise DecoratorAlreadyExistsException(
+                f"Failed to register request decorator '{name}' >> Duplicate decorator",
+                logger.error,
+            )
+
+        self._decorators["request"][name] = value
+
+    def decorate_reply(self, name: str, value: any) -> None:
+        if hasattr(Reply, name) or self.has_reply_decorator(name):
+            raise DecoratorAlreadyExistsException(
+                f"Failed to register reply decorator '{name}' >> Duplicate decorator",
+                logger.error,
+            )
+
+        self._decorators["reply"][name] = value
+
+    def has_decorator(self, name: str) -> bool:
+        return name in self._decorators["app"]
+
+    def has_request_decorator(self, name: str) -> bool:
+        return name in self._decorators["request"]
+
+    def has_reply_decorator(self, name: str) -> bool:
+        return name in self._decorators["reply"]
+
+    def add_hook(self, hook_type: hookType, hook: FunctionType) -> None:
+        if hook_type not in HOOKS:
+            raise NoHookTypeException(
+                f"Failed to register hook [{hook_type}] >> Type not supported",
+                logger.error,
+            )
+
+        self._hooks[hook_type].append(hook)
+
+    def hook(self, hook_type: hookType) -> FunctionType:
+        def internal(hook: FunctionType) -> FunctionType:
+            self.add_hook(hook_type, hook)
+            return hook
+
+        return internal
+
+    def add_middleware(self, middleware: FunctionType) -> None:
+        self._middlewares.append(middleware)
+
+    def use(self) -> FunctionType:
+        def internal(middleware: FunctionType) -> FunctionType:
+            self.add_middleware(middleware)
+            return middleware
+
+        return internal
+
+    def add_serializer(
+        self,
+        validation: Callable[[any], bool],
+        serializer: Callable[[any], any],
+    ):
+        self._serializers.append({"validate": validation, "serialize": serializer})
+
+    def add_route(
+        self,
+        method: httpMethodType,
+        path: str,
+        handler: FunctionType,
+        route_hooks: RouteHookType = {},
+        route_middlewares: RouteMiddlewareType = [],
+    ) -> None:
+        if self.prefix != "/":
+            path = f"{self.prefix}{path if path != '/' else ''}"
+        if method not in HTTP_METHODS:
+            raise NoHTTPMethodException(
+                f"Failed to register route [{method}] '{path}' >> Method not supported",
+                logger.error,
+            )
+
+        if (
+            not re.fullmatch(r"^(\/:?[_a-zA-Z0-9]+)*$|^\/$", path)
+            or re.search(r":(\d)\w+", path)
+            or len(re.findall(r":(\w+)", path)) != len(set(re.findall(r":(\w+)", path)))
+        ):
+            raise InvalidPathException(
+                f"Failed to register route [{method}] '{path}' >> Invalid path",
+                logger.error,
+            )
+
+        routeAlreadyExists = self._router.find_route(method, path) is not None
+        if routeAlreadyExists:
+            raise DuplicateRouteException(
+                f"Failed to register route [{method}] '{path}' >> Duplicate route",
+                logger.error,
+            )
+
+        hooks = copy.deepcopy(self._hooks)
+        hooks.update(route_hooks)
+
+        middlewares = copy.deepcopy(self._middlewares)
+        middlewares.extend(route_middlewares)
+
+        self._router.add_route(
+            method,
+            path,
+            {
+                "handler": handler,
+                "hooks": hooks,
+                "middlewares": middlewares,
+                "raw_path": path,
+            },
+        )
+        message = f"Route registered [%s] '{path}'"
+        color_message = (
+            "Route registered [" + click.style("%s", fg="cyan") + f"] '{path}'"
+        )
+        logger.debug(message, method, extra={"color_message": color_message})
+
+    def get(
+        self,
+        path: str,
+        route_hooks: RouteHookType = {},
+        route_middlewares: RouteMiddlewareType = [],
+    ) -> FunctionType:
+        def internal(handler: FunctionType) -> FunctionType:
+            self.add_route("GET", path, handler, route_hooks, route_middlewares)
+            return handler
+
+        return internal
+
+    def post(
+        self,
+        path: str,
+        route_hooks: RouteHookType = {},
+        route_middlewares: RouteMiddlewareType = [],
+    ) -> FunctionType:
+        def internal(handler: FunctionType) -> FunctionType:
+            self.add_route("POST", path, handler, route_hooks, route_middlewares)
+            return handler
+
+        return internal
+
+    def put(
+        self,
+        path: str,
+        route_hooks: RouteHookType = {},
+        route_middlewares: RouteMiddlewareType = [],
+    ) -> FunctionType:
+        def internal(handler: FunctionType) -> FunctionType:
+            self.add_route("PUT", path, handler, route_hooks, route_middlewares)
+            return handler
+
+        return internal
+
+    def patch(
+        self,
+        path: str,
+        route_hooks: RouteHookType = {},
+        route_middlewares: RouteMiddlewareType = [],
+    ) -> FunctionType:
+        def internal(handler: FunctionType) -> FunctionType:
+            self.add_route("PATCH", path, handler, route_hooks, route_middlewares)
+            return handler
+
+        return internal
+
+    def delete(
+        self,
+        path: str,
+        route_hooks: RouteHookType = {},
+        route_middlewares: RouteMiddlewareType = [],
+    ) -> FunctionType:
+        def internal(handler: FunctionType) -> FunctionType:
+            self.add_route("DELETE", path, handler, route_hooks, route_middlewares)
+            return handler
+
+        return internal
+
+    def head(
+        self,
+        path: str,
+        route_hooks: RouteHookType = {},
+        route_middlewares: RouteMiddlewareType = [],
+    ) -> FunctionType:
+        def internal(handler: FunctionType) -> FunctionType:
+            self.add_route("HEAD", path, handler, route_hooks, route_middlewares)
+            return handler
+
+        return internal
+
+    def __getattr__(self, name) -> any:
+        return super().__getattr__(name)
 
-  def __getattr__(self, name) -> any:
-    return super().__getattr__(name)
+    def __setattr__(self, name, value) -> None:
+        return super().__setattr__(name, value)
 
-  def __setattr__(self, name, value) -> None:
-    return super().__setattr__(name, value)
 
 class FastipyInstance(Fastipy):
-  def cors(self, *args, **kwargs) -> None:
-    logger.warn(NotImplementedError('FastipyInstance.cors() is not implemented'))
+    def cors(self, *args, **kwargs) -> None:
+        logger.warn("FastipyInstance.cors() is not implemented")
```

### Comparing `fastipy-1.5.0/app/fastipy/src/core/reply.py` & `fastipy-1.5.1/app/fastipy/src/core/reply.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,464 +1,508 @@
-from typing import Dict, Iterator, List, Union, Optional, Set
+import json
+import os, io
+from typing import (
+    AsyncGenerator,
+    Callable,
+    Dict,
+    Generator,
+    Iterator,
+    List,
+    Union,
+    Optional,
+    Set,
+)
 from http.cookies import SimpleCookie
 from time import perf_counter
-from logging import Logger
-import mimetypes, os, json, io
-
-from ..constants.content_types import CONTENT_TYPES
+from uvicorn.main import logger
 
 from ..types.routes import FunctionType
 
-from ..exceptions.file_exception import FileException
-from ..exceptions.reply_exception import ReplyException
+from ..exceptions import FileException, ReplyException
 
 from ..classes.decorators_base import DecoratorsBase
 
-from ..helpers.route_helpers import handler_hooks
+from ..helpers.route_helpers import handler_hooks, serializer_handler
+from ..helpers.content_type import get_content_type
 
 from .request import Request
 
+
 class Reply(DecoratorsBase):
-  def __init__(
-    self,
-    send,
-    logger: Logger,
-    request: Request = None,
-    cors: Dict = {},
-    static_path: Union[str, None] = None,
-    decorators: Dict[str, List[FunctionType]] = {},
-    hooks: Dict[str, List[FunctionType]] = {},
-  ) -> None:
-    self.__send               = send
-    self.__request            = request
-    self.__on_response_hooks  = hooks.get('onResponse', [])
-
-    self._log                 = logger
-    self._cors                = cors
-    self._static_path         = static_path
-    self._headers             = {}
-    self._status_code         = 200
-    self._content             = None
-    self._cookies             = SimpleCookie()
-    self._response_time       = perf_counter()
-    self._response_sent       = False
-
-    self._instance_decorators = decorators.get('reply', [])
-
-  @property
-  def status_code(self) -> int:
-    return self._status_code
-
-  @status_code.setter
-  def status_code(self, code: int) -> None:
-    if code < 100 or code > 599:
-      message = 'Status code must be a number between 100 and 599'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-    
-    self._status_code = code
-
-  @property
-  def content_type(self) -> Union[str, None]:
-    return self._headers.get('Content-Type', None)
-  
-  @content_type.setter
-  def content_type(self, content_type: str) -> None:
-    self._headers['Content-Type'] = content_type
-
-  @property
-  def is_sent(self) -> bool:
-    return self._response_sent
-  
-  @property
-  def cookies(self) -> SimpleCookie:
-    return self._cookies
-  
-  @property
-  def headers(self) -> Dict[str, str]:
-    return self._headers
-  
-  def type(self, content_type: str) -> 'Reply':
-    self._headers['Content-Type'] = content_type
-    return self
-  
-  def code(self, code: int) -> 'Reply':
-    self._status_code = code
-    return self
-  
-  def json(self, response: dict) -> 'Reply':
-    self._content = json.dumps(response)
-    self._headers['Content-Type'] = 'application/json'
-    return self
-
-  def text(self, response: str) -> 'Reply':
-    self._content = response
-    self._headers['Content-Type'] = 'text/plain'
-    return self
-
-  def html(self, response: str) -> 'Reply':
-    self._content = response
-    self._headers['Content-Type'] = 'text/html'
-    return self
-
-  def header(self, key: str, value: str) -> 'Reply':
-    self._headers[key] = value
-    return self
-
-  def get_header(self, key: str) -> str:
-    return self._headers[key]
-
-  def remove_header(self, key: str) -> 'Reply':
-    del self._headers[key]
-    return self
-
-  def cookie(
-    self,
-    name: str,
-    value: str,
-    path="/",
-    expires=None,
-    domain: str = None,
-    secure: bool = False,
-    httpOnly: bool = False
-  ) -> 'Reply':
-    self._cookies[name] = value
-    self._cookies[name]['path'] = path
-    self._cookies[name]['secure'] = secure
-    self._cookies[name]['httpOnly'] = httpOnly
-
-    if expires is not None: self._cookies[name]['expires'] = expires
-    if domain is not None: self._cookies[name]['domain'] = domain
-    return self
-  
-  def getResponseTime(self) -> float:
-    return perf_counter() - self._response_time
-
-  async def send(self) -> None:
-    if self._response_sent:
-      message = 'Reply already sent'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-
-    await self._send_headers()
-    await self._send_body()
-
-    await self.__on_response_sent()
-
-  async def send_code(self, code: int) -> None:
-    if self._response_sent:
-      message = 'Reply already sent'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-    
-    self._status_code = code
-
-    await self._send_headers()
-    await self._send_body(send_blank=True)
-
-    await self.__on_response_sent()
-
-  async def send_cookie(self) -> None:
-    if self._response_sent:
-      message = 'Reply already sent'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-    
-    headers = [[b'Set-Cookie', cookie.OutputString().decode('utf-8')] for cookie in self._cookies.values()]
-    
-    await self._send_headers(headers)
-    await self._send_body(send_blank=True)
-
-    await self.__on_response_sent()
-
-  async def send_file(self, path: str, stream: bool = False, block_size: int = 1024) -> None:
-    if self._response_sent:
-      message = 'Reply already sent'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-    
-    try:
-      with io.open(path, 'rb') as file:
-        file_size = os.path.getsize(path)
-        content_type = self._get_content_type(path)
+    def __init__(
+        self,
+        send,
+        request: Request = None,
+        cors: Dict = {},
+        static_path: Union[str, None] = None,
+        decorators: Dict[str, List[FunctionType]] = {},
+        hooks: Dict[str, List[FunctionType]] = {},
+        serializers: List[Dict[str, Callable[[any], Union[bool, any]]]] = [],
+    ) -> None:
+        self.__send = send
+        self.__request = request
+        self.__on_response_hooks = hooks.get("onResponse", [])
+
+        self._cors = cors
+        self._static_path = static_path
+        self._headers = {}
+        self._status_code = 200
+        self._content = None
+        self._cookies = SimpleCookie()
+        self._response_time = perf_counter()
+        self._response_sent = False
+        self._serializers = reversed(serializers)
+
+        self._instance_decorators = decorators.get("reply", [])
+
+    @property
+    def status_code(self) -> int:
+        return self._status_code
+
+    @status_code.setter
+    def status_code(self, code: int) -> None:
+        if code < 100 or code > 599:
+            raise ReplyException(
+                "Status code must be a number between 100 and 599",
+                logger.error,
+            )
+
+        self._status_code = code
+
+    @property
+    def content_type(self) -> Union[str, None]:
+        return self._headers.get("Content-Type", None)
+
+    @content_type.setter
+    def content_type(self, content_type: str) -> None:
+        self._headers["Content-Type"] = content_type
+
+    @property
+    def is_sent(self) -> bool:
+        return self._response_sent
+
+    @property
+    def cookies(self) -> SimpleCookie:
+        return self._cookies
+
+    @property
+    def headers(self) -> Dict[str, str]:
+        return self._headers
+
+    def type(self, content_type: str) -> "Reply":
+        self._headers["Content-Type"] = content_type
+        return self
+
+    def code(self, code: int) -> "Reply":
+        self._status_code = code
+        return self
+
+    def header(self, key: str, value: str) -> "Reply":
+        self._headers[key] = value
+        return self
+
+    def get_header(self, key: str) -> str:
+        return self._headers[key]
+
+    def remove_header(self, key: str) -> "Reply":
+        del self._headers[key]
+        return self
+
+    def cookie(
+        self,
+        name: str,
+        value: str,
+        path="/",
+        expires=None,
+        domain: str = None,
+        secure: bool = False,
+        httpOnly: bool = False,
+    ) -> "Reply":
+        self._cookies[name] = value
+        self._cookies[name]["path"] = path
+        self._cookies[name]["secure"] = secure
+        self._cookies[name]["httpOnly"] = httpOnly
+
+        if expires is not None:
+            self._cookies[name]["expires"] = expires
+        if domain is not None:
+            self._cookies[name]["domain"] = domain
+        return self
+
+    def get_response_time(self) -> float:
+        return perf_counter() - self._response_time
+
+    async def send(self, value: any = None) -> None:
+        if self._response_sent:
+            raise ReplyException("Reply already sent", logger.error)
+
+        content_type, serialized_value = serializer_handler(self._serializers, value)
+        if not self.content_type and content_type:
+            self.content_type = content_type
 
-        headers = self._parse_headers()
-        headers.append((b'Content-type', content_type.encode('utf-8')))
-        headers.append((b'Content-Disposition', f'attachment; filename="{path.split("/")[-1]}"'.encode('utf-8')))
-        headers.append((b'Content-Length', str(file_size).encode('utf-8')))
+        if isinstance(serialized_value, (Generator, AsyncGenerator)):
+            return await self.__stream(serialized_value)
+
+        self._content = serialized_value
+
+        await self._send_headers()
+        await self._send_body(send_blank=False if serialized_value else True)
+
+        await self.__on_response_sent()
+
+    async def send_code(self, code: int) -> None:
+        if self._response_sent:
+            raise ReplyException("Reply already sent", logger.error)
+
+        self._status_code = code
+
+        await self._send_headers()
+        await self._send_body(send_blank=True)
+
+        await self.__on_response_sent()
+
+    async def send_cookie(self) -> None:
+        if self._response_sent:
+            raise ReplyException("Reply already sent", logger.error)
+
+        headers = [
+            [b"Set-Cookie", cookie.OutputString().decode("utf-8")]
+            for cookie in self._cookies.values()
+        ]
+
+        await self._send_headers(headers)
+        await self._send_body(send_blank=True)
+
+        await self.__on_response_sent()
+
+    async def send_file(
+        self, path: str, stream: bool = False, block_size: int = 1024
+    ) -> None:
+        if self._response_sent:
+            raise ReplyException("Reply already sent", logger.error)
+
+        try:
+            with io.open(path, "rb") as file:
+                file_size = os.path.getsize(path)
+                content_type = get_content_type(path)
+
+                headers = self._parse_headers()
+                headers.append((b"Content-type", content_type.encode("utf-8")))
+                headers.append(
+                    (
+                        b"Content-Disposition",
+                        f'attachment; filename="{path.split("/")[-1]}"'.encode("utf-8"),
+                    )
+                )
+                headers.append((b"Content-Length", str(file_size).encode("utf-8")))
+
+                await self._send_headers(headers=headers)
+
+                if stream:
+                    while True:
+                        chunk = file.read(block_size)
+                        if not chunk:
+                            await self._send_body(send_blank=True)
+                            break
+
+                        self._content = chunk
+                        await self._send_body(more_body=True)
+                else:
+                    self._content = file.read()
+                    await self._send_body()
+
+                await self.__on_response_sent()
+        except FileNotFoundError:
+            raise FileException(
+                f"Failed to send file '{path}' >> File not found", logger.error
+            )
+
+    async def _send_error(self, message: str, code: int) -> None:
+        if self._response_sent:
+            raise ReplyException("Reply already sent", logger.error)
+
+        if code < 100 or code > 599:
+            raise ReplyException(
+                "Status code must be a number between 100 and 599",
+                logger.error,
+            )
+
+        self._status_code = code
+        self._headers["Content-Type"] = "application/json"
+        self._content = json.dumps({"error": message})
+
+        await self._send_headers()
+        await self._send_body()
+
+        await self.__on_response_sent()
 
+    async def __stream(self, stream: Iterator[str]) -> None:
+        if self._response_sent:
+            raise ReplyException("Reply already sent", logger.error)
+
+        if not isinstance(stream, (AsyncGenerator, Generator)):
+            raise ReplyException(
+                "Stream must be an async generator or generator", logger.error
+            )
+
+        headers = self._parse_headers()
         await self._send_headers(headers=headers)
 
-        if stream:
-          while True:
-            chunk = file.read(block_size)
-            if not chunk:
-              await self._send_body(send_blank=True)
-              break
+        if isinstance(stream, AsyncGenerator):
+            while True:
+                try:
+                    chunk = await anext(stream)
+                except StopAsyncIteration:
+                    break
 
-            self._content = chunk
-            await self._send_body(more_body=True)
+                self._content = chunk
+                await self._send_body(more_body=True)
         else:
-          self._content = file.read()
-          await self._send_body()
+            while True:
+                try:
+                    chunk = next(stream)
+                except StopIteration:
+                    break
+
+                self._content = chunk
+                await self._send_body(more_body=True)
 
+        await self._send_body(send_blank=True)
         await self.__on_response_sent()
-    except FileNotFoundError:
-      message = f"Failed to send file '{path}' >> File not found"
-      self._log.error(FileException(message))
-      raise FileException(message)
-
-  async def stream(self, stream: Iterator[str], media_type: str = 'application/octet-stream') -> None:
-    if self._response_sent:
-      message = 'Reply already sent'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-    
-    headers = self._parse_headers()
-    headers.append((b'Content-type', media_type.encode('utf-8')))
-
-    await self._send_headers(headers=headers)
-
-    while True:
-      try:
-        if hasattr(stream, '__anext__'): 
-          chunk = await anext(stream)
-        else:
-          chunk = next(stream)
 
-        self._content = chunk
-        await self._send_body(more_body=True)
-      except (StopIteration, StopAsyncIteration):
+    async def redirect(
+        self,
+        location: str,
+        code: int = 302,
+        cache_control: Optional[str] = "no-store, no-cache, must-revalidate",
+    ) -> None:
+        if self._response_sent:
+            raise ReplyException("Reply already sent", logger.error)
+
+        self._status_code = code
+
+        headers = self._parse_headers()
+        headers.append((b"Location", location.encode("utf-8")))
+
+        if cache_control:
+            headers.append((b"Cache-Control", cache_control.encode("utf-8")))
+
+        await self._send_headers(headers=headers)
         await self._send_body(send_blank=True)
-        break
 
-    await self.__on_response_sent()
+        await self.__on_response_sent()
+
+    def render_page(self, path: str) -> "Reply":
+        if not path.endswith(".html"):
+            raise FileException(
+                f"Failed to render page '{path}' >> File not a html", logger.error
+            )
+
+        if self._static_path:
+            path = f"{self._static_path}/{path}"
+
+        try:
+            with io.open(f"{path}", "r") as file:
+                self._content = file.read()
+            self._headers["Content-Type"] = "text/html"
+        except FileNotFoundError:
+            raise FileException(
+                f"Failed to render page '{path}' >> File not found", logger.error
+            )
+
+        return self
+
+    async def _options(self, allowed_methods: List[str]) -> None:
+        if self._response_sent:
+            raise ReplyException("Reply already sent", logger.error)
+
+        headers = [
+            (key.encode("utf-8"), value.encode("utf-8"))
+            for key, value in self._cors.items()
+        ]
+        headers.append(
+            (
+                b"Allow",
+                b", ".join([method.encode("utf-8") for method in allowed_methods]),
+            )
+        )
+
+        await self._send_headers(headers)
+        await self._send_body(send_blank=True)
+
+        await self.__on_response_sent()
+
+    async def _send_headers(self, headers: List[bytes] = None) -> None:
+        await self.__send(
+            {
+                "type": "http.response.start",
+                "status": self._status_code,
+                "headers": self._parse_headers() if headers is None else headers,
+            }
+        )
+
+    async def _send_body(
+        self, send_blank: bool = False, more_body: bool = False
+    ) -> None:
+        if not send_blank and self._content is None:
+            raise ReplyException(
+                "Reply content is not set, use 'send' method to set content",
+                logger.error,
+            )
+
+        try:
+            body = self._content.encode("utf-8") if not send_blank else b""
+        except AttributeError:
+            body = self._content if not send_blank else b""
+
+        await self.__send(
+            {
+                "type": "http.response.body",
+                "body": body,
+                **({"more_body": True} if more_body else {}),
+            }
+        )
+
+    def _parse_headers(self) -> List[Set[bytes]]:
+        headers = [
+            (header.encode("utf-8"), value.encode("utf-8"))
+            for header, value in self._headers.items()
+        ]
+        for header, value in self._cors.items():
+            headers.append((header.encode("utf-8"), value.encode("utf-8")))
+        for cookie in self._cookies.values():
+            headers.append((b"Set-Cookie", cookie.OutputString().encode("utf-8")))
+
+        return headers
+
+    async def _send_archive(self, path: str = None) -> None:
+        content_type = get_content_type(path)
+
+        if self._static_path:
+            path = f"{self._static_path}/{path}"
+
+        try:
+            with io.open(path, "rb") as file:
+                self._content = file.read()
+            self._headers["Content-Type"] = content_type
+
+            await self._send_headers()
+            await self._send_body()
+        except FileNotFoundError:
+            self._status_code = 404
+
+            await self._send_headers()
+            await self._send_body(send_blank=True)
+
+    async def __on_response_sent(self) -> None:
+        self._response_sent = True
+        await handler_hooks(
+            self.__on_response_hooks,
+            self.__request,
+            RestrictReply(self),
+            check_response_sent=False,
+        )
 
-  async def redirect(
-    self,
-    location: str,
-    code: int = 302,
-    cache_control: Optional[str] = 'no-store, no-cache, must-revalidate'
-  ) -> None:
-    if self._response_sent:
-      message = 'Reply already sent'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-
-    self._status_code = code
-
-    headers = self._parse_headers()
-    headers.append((b'Location', location.encode('utf-8')))
-
-    if cache_control:
-      headers.append((b'Cache-Control', cache_control.encode('utf-8')))
-
-    await self._send_headers(headers=headers)
-    await self._send_body(send_blank=True)
-
-    await self.__on_response_sent()
-
-  def render_page(self, path: str) -> 'Reply':
-    if not path.endswith('.html'):
-      message = f"Failed to render page '{path}' >> File not a html"
-      self._log.error(FileException(message))
-      raise FileException(message)
-
-    if self._static_path:
-      path = f"{self._static_path}/{path}"
-
-    try:
-      with io.open(f"{path}", 'r') as file:
-        self._content = file.read()
-      self._headers['Content-Type'] = 'text/html'
-    except FileNotFoundError:
-      message = f"Failed to render page '{path}' >> File not found"
-      self._log.error(FileException(message))
-      raise FileException(message)
-
-    return self
-  
-  async def _options(self, allowed_methods: List[str]) -> None:
-    if self._response_sent:
-      message = 'Reply already sent'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-    
-    headers = [(key.encode('utf-8'), value.encode('utf-8')) for key, value in self._cors.items()]
-    headers.append((b'Allow', b', '.join([method.encode('utf-8') for method in allowed_methods])))
-
-    await self._send_headers(headers)
-    await self._send_body(send_blank=True)
-
-    await self.__on_response_sent()
-  
-  async def _send_headers(self, headers: List[bytes] = None) -> None:
-    await self.__send({
-      'type': 'http.response.start',
-      'status': self._status_code,
-      'headers': self._parse_headers() if headers is None else headers,
-    })
-
-  async def _send_body(self, send_blank: bool = False, more_body: bool = False) -> None:
-    if not send_blank and self._content is None:
-      message = 'Reply is not set, try send_code() instead'
-      self._log.error(ReplyException(message))
-      raise ReplyException(message)
-    
-    try:
-      body = self._content.encode('utf-8') if not send_blank else b''
-    except AttributeError:
-      body = self._content if not send_blank else b''
-
-    await self.__send({
-      'type': 'http.response.body',
-      'body': body,
-      **({'more_body': True} if more_body else {})
-    })
-
-  def _parse_headers(self) -> List[Set[bytes]]:
-    headers = [(header.encode('utf-8'), value.encode('utf-8')) for header, value in self._headers.items()]
-    for header, value in self._cors.items():
-      headers.append((header.encode('utf-8'), value.encode('utf-8')))
-    for cookie in self._cookies.values():
-      headers.append((b'Set-Cookie', cookie.OutputString().encode('utf-8')))
-
-    return headers
-  
-  def _get_content_type(self, path: str) -> str:
-    try:
-      content_type = CONTENT_TYPES[path.split('.')[-1]]
-    except KeyError:
-      content_type = mimetypes.guess_type(path)[0]
-
-    return content_type or 'application/octet-stream'
-  
-  async def _send_archive(self, path: str = None) -> None:
-    content_type = self._get_content_type(path)
-
-    if self._static_path:
-      path = f"{self._static_path}/{path}"
-
-    try:
-      with io.open(path, 'rb') as file:
-        self._content = file.read()
-      self._headers['Content-Type'] = content_type
-
-      await self._send_headers()
-      await self._send_body()
-    except FileNotFoundError:
-      self._status_code = 404
-      
-      await self._send_headers()
-      await self._send_body(send_blank=True)
-
-  async def __on_response_sent(self) -> None:
-    self._response_sent = True
-    await handler_hooks(
-      self.__on_response_hooks,
-      self.__request,
-      RestrictReply(self),
-      check_response_sent=False
-    )
+    def __getattr__(self, name) -> any:
+        return super().__getattr__(name)
 
-  def __getattr__(self, name) -> any:
-    return super().__getattr__(name)
+    def __setattr__(self, name, value) -> None:
+        return super().__setattr__(name, value)
 
-  def __setattr__(self, name, value) -> None:
-    return super().__setattr__(name, value)
 
 class RestrictReply:
-  def __init__(self, reply: Reply):
-    self._reply = reply
+    def __init__(self, reply: Reply):
+        self._reply = reply
+
+    @property
+    def status_code(self) -> int:
+        return self._reply.status_code
+
+    @status_code.setter
+    def status_code(self, code: int) -> None:
+        self._reply.status_code = code
+
+    @property
+    def content_type(self) -> str:
+        return self._reply.content_type
+
+    @content_type.setter
+    def content_type(self, content_type: str) -> None:
+        self._reply.content_type = content_type
+
+    @property
+    def is_sent(self) -> bool:
+        return self._reply.is_sent
+
+    @property
+    def cookies(self) -> SimpleCookie:
+        return self._reply.cookies
+
+    @property
+    def headers(self) -> Dict[str, str]:
+        return self._reply.headers
+
+    def type(self, content_type: str) -> "Reply":
+        return self._reply.type(content_type)
+
+    def code(self, code: int) -> "Reply":
+        return self._reply.code(code)
+
+    def header(self, key: str, value: str) -> "Reply":
+        return self._reply.header(key, value)
+
+    def get_header(self, key: str) -> str:
+        return self._reply.get_header(key)
+
+    def remove_header(self, key: str) -> "Reply":
+        return self._reply.remove_header(key)
+
+    def cookie(
+        self,
+        name: str,
+        value: str,
+        path="/",
+        expires=None,
+        domain: str = None,
+        secure: bool = False,
+        httpOnly: bool = False,
+    ) -> "Reply":
+        return self._reply.cookie(name, value, path, expires, domain, secure, httpOnly)
+
+    def send(self, value: any) -> None:
+        self._reply._log.warn(
+            ReplyException('Function "send" is not allowed in this context')
+        )
+
+    def send_code(self, code: int) -> None:
+        self._reply._log.warn(
+            ReplyException('Function "send_code" is not allowed in this context')
+        )
+
+    def send_cookie(self) -> None:
+        self._reply._log.warn(
+            ReplyException('Function "send_cookie" is not allowed in this context')
+        )
+
+    def send_file(self, path: str) -> None:
+        self._reply._log.warn(
+            ReplyException('Function "send_file" is not allowed in this context')
+        )
+
+    def redirect(
+        self,
+        location: str,
+        code: int = 302,
+        cache_control: Optional[str] = "no-store, no-cache, must-revalidate",
+    ) -> None:
+        self._reply._log.warn(
+            ReplyException('Function "redirect" is not allowed in this context')
+        )
+
+    def render_page(self, path: str) -> "Reply":
+        return self._reply.render_page(path)
+
+    def __getattr__(self, name) -> any:
+        return super().__getattr__(name)
 
-  @property
-  def status_code(self) -> int:
-    return self._reply.status_code
-  
-  @status_code.setter
-  def status_code(self, code: int) -> None:
-    self._reply.status_code = code
-
-  @property
-  def content_type(self) -> str:
-    return self._reply.content_type
-  
-  @content_type.setter
-  def content_type(self, content_type: str) -> None:
-    self._reply.content_type = content_type
-
-  @property
-  def is_sent(self) -> bool:
-    return self._reply.is_sent
-  
-  @property
-  def cookies(self) -> SimpleCookie:
-    return self._reply.cookies
-  
-  @property
-  def headers(self) -> Dict[str, str]:
-    return self._reply.headers
-  
-  def type(self, content_type: str) -> 'Reply':
-    return self._reply.type(content_type)
-  
-  def code(self, code: int) -> 'Reply':
-    return self._reply.code(code)
-  
-  def json(self, response: dict) -> None:
-    self._reply._log.warn(ReplyException('Function "json" is not allowed in this context'))
-
-  def text(self, response: str) -> None:
-    self._reply._log.warn(ReplyException('Function "text" is not allowed in this context'))
-  
-  def html(self, response: str) -> None:
-    self._reply._log.warn(ReplyException('Function "html" is not allowed in this context'))
-  
-  def header(self, key: str, value: str) -> 'Reply':
-    return self._reply.header(key, value)
-  
-  def get_header(self, key: str) -> str:
-    return self._reply.get_header(key)
-  
-  def remove_header(self, key: str) -> 'Reply':
-    return self._reply.remove_header(key)
-  
-  def cookie(
-    self,
-    name: str,
-    value: str,
-    path="/",
-    expires=None,
-    domain: str = None,
-    secure: bool = False,
-    httpOnly: bool = False
-  ) -> 'Reply':
-    return self._reply.cookie(name, value, path, expires, domain, secure, httpOnly)
-
-  def send(self) -> None:
-    self._reply._log.warn(ReplyException('Function "send" is not allowed in this context'))
-  
-  def send_code(self, code: int) -> None:
-    self._reply._log.warn(ReplyException('Function "send_code" is not allowed in this context'))
-  
-  def send_cookie(self) -> None:
-    self._reply._log.warn(ReplyException('Function "send_cookie" is not allowed in this context'))
-  
-  def send_file(self, path: str) -> None:
-    self._reply._log.warn(ReplyException('Function "send_file" is not allowed in this context'))
-  
-  def redirect(
-    self,
-    location: str,
-    code: int = 302,
-    cache_control: Optional[str] = 'no-store, no-cache, must-revalidate'
-  ) -> None:
-    self._reply._log.warn(ReplyException('Function "redirect" is not allowed in this context'))
-  
-  def render_page(self, path: str) -> 'Reply':
-    return self._reply.render_page(path)
-  
-  def __getattr__(self, name) -> any:
-    return super().__getattr__(name)
-  
-  def __setattr__(self, name, value) -> None:
-    return super().__setattr__(name, value)
+    def __setattr__(self, name, value) -> None:
+        return super().__setattr__(name, value)
```

### Comparing `fastipy-1.5.0/app/fastipy/src/core/request.py` & `fastipy-1.5.1/app/fastipy/src/core/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,108 +5,114 @@
 
 from ..types.routes import FunctionType
 
 from ..classes.decorators_base import DecoratorsBase
 
 from ..models.body import Body
 
+
 class Request(DecoratorsBase):
-  def __init__(
-    self,
-    scope,
-    receive,
-    logger: Logger,
-    decorators: Dict[str, List[FunctionType]] = {}
-  ) -> None:
-    self.__scope              = scope
-    self.__receive            = receive
-    self._instance_decorators = decorators.get('request', [])
-    self._log                 = logger
-    self._body                = None
-
-    self.__headers()
-    self.__query_params()
-    self._cookies = SimpleCookie(self.__scope['headers'].get('cookie', None))
-    
-  @property
-  def type(self) -> str:
-    return self.__scope['type']
-
-  @property
-  def asgi(self) -> Dict[str, str]:
-    return self.__scope['asgi']
-  
-  @property
-  def http_version(self) -> str:
-    return self.__scope['http_version']
-  
-  @property
-  def client(self) -> Tuple[str, int]:
-    return self.__scope['client']
-  
-  @property
-  def scheme(self) -> str:
-    return self.__scope['scheme']
-  
-  @property
-  def root_path(self) -> str:
-    return self.__scope['root_path']
-  
-  @property
-  def headers(self) -> Dict[str, str]:
-    return self.__scope['headers']
-  
-  @property
-  def raw_headers(self) -> Dict[str, str]:
-    return self.__scope['raw_headers']
-  
-  @property
-  def method(self) -> str:
-    return self.__scope['method']
-  
-  @property
-  def path(self) -> str:
-    return self.__scope['path']
-  
-  @property
-  def raw_path(self) -> bytes:
-    return self.__scope['raw_path']
-  
-  @property
-  def raw_query(self) -> bytes:
-    return self.__scope['query_string']
-  
-  @property
-  def body(self) -> Union[Body, None]:
-    return self._body
-  
-  @property
-  def query(self) -> Dict[str, str]:
-    return self._query_params
-  
-  @property
-  def params(self) -> Dict[str, str]:
-    return self.__scope['params']
-  
-  @property
-  def cookies(self) -> SimpleCookie:
-    return self._cookies
-  
-  def __query_params(self) -> None:
-    self._query_params = dict(parse_qsl(self.__scope['query_string'].decode('utf-8')))
-
-  def __headers(self) -> None:
-    headers = {}
-    for key, value in self.__scope['headers']:
-      headers[key.decode('utf-8')] = value.decode('utf-8')
-    self.__scope['headers'], self.__scope['raw_headers'] = headers, self.__scope['headers']
-
-  async def _load_body(self) -> None:
-    if self._body is None:
-      self._body = Body(self.__scope, self.__receive)
-      await self._body.load()
+    def __init__(
+        self,
+        scope,
+        receive,
+        logger: Logger,
+        decorators: Dict[str, List[FunctionType]] = {},
+    ) -> None:
+        self.__scope = scope
+        self.__receive = receive
+        self._instance_decorators = decorators.get("request", [])
+        self._log = logger
+        self._body = None
+
+        self.__headers()
+        self.__query_params()
+        self._cookies = SimpleCookie(self.__scope["headers"].get("cookie", None))
+
+    @property
+    def type(self) -> str:
+        return self.__scope["type"]
+
+    @property
+    def asgi(self) -> Dict[str, str]:
+        return self.__scope["asgi"]
+
+    @property
+    def http_version(self) -> str:
+        return self.__scope["http_version"]
+
+    @property
+    def client(self) -> Tuple[str, int]:
+        return self.__scope["client"]
+
+    @property
+    def scheme(self) -> str:
+        return self.__scope["scheme"]
+
+    @property
+    def root_path(self) -> str:
+        return self.__scope["root_path"]
+
+    @property
+    def headers(self) -> Dict[str, str]:
+        return self.__scope["headers"]
+
+    @property
+    def raw_headers(self) -> Dict[str, str]:
+        return self.__scope["raw_headers"]
+
+    @property
+    def method(self) -> str:
+        return self.__scope["method"]
+
+    @property
+    def path(self) -> str:
+        return self.__scope["path"]
+
+    @property
+    def raw_path(self) -> bytes:
+        return self.__scope["raw_path"]
+
+    @property
+    def raw_query(self) -> bytes:
+        return self.__scope["query_string"]
+
+    @property
+    def body(self) -> Union[Body, None]:
+        return self._body
+
+    @property
+    def query(self) -> Dict[str, str]:
+        return self._query_params
+
+    @property
+    def params(self) -> Dict[str, str]:
+        return self.__scope["params"]
+
+    @property
+    def cookies(self) -> SimpleCookie:
+        return self._cookies
+
+    def __query_params(self) -> None:
+        self._query_params = dict(
+            parse_qsl(self.__scope["query_string"].decode("utf-8"))
+        )
+
+    def __headers(self) -> None:
+        headers = {}
+        for key, value in self.__scope["headers"]:
+            headers[key.decode("utf-8")] = value.decode("utf-8")
+        self.__scope["headers"], self.__scope["raw_headers"] = (
+            headers,
+            self.__scope["headers"],
+        )
+
+    async def _load_body(self) -> None:
+        if self._body is None:
+            self._body = Body(self.__scope, self.__receive)
+            await self._body.load()
 
-  def __getattr__(self, name) -> any:
-    return super().__getattr__(name)
+    def __getattr__(self, name) -> any:
+        return super().__getattr__(name)
 
-  def __setattr__(self, name, value) -> None:
-    return super().__setattr__(name, value)
+    def __setattr__(self, name, value) -> None:
+        return super().__setattr__(name, value)
```

### Comparing `fastipy-1.5.0/app/fastipy/src/core/request_handler.py` & `fastipy-1.5.1/app/fastipy/src/core/request_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,138 @@
-from uvicorn.main import logger
 import traceback
 
-from ..exceptions.exception_handler import ExceptionHandler
-from ..exceptions.fastipy_base_exception import FastipyBaseException
+from ..exceptions import ExceptionHandler, FastipyBaseException
 
 from ..helpers.route_helpers import handler_hooks, handler_middlewares
 from ..helpers.async_sync_helpers import run_async_or_sync
 
 from .request import Request
 from .reply import Reply, RestrictReply
 
+
 class RequestHandler:
-  async def __call__(self, scope, receive, send):
-    if scope['type'] == 'http':
-      cors = self._cors.generate_headers() if self._cors else {}
-
-      if scope['method'] in ['POST', 'GET', 'PUT', 'PATCH', 'DELETE', 'HEAD']:
-        await self._handle_http_request(scope, receive, send, cors)
-        return
-
-      elif scope['method'] == 'OPTIONS':
-        allowed_methods = self._router.get_methods(scope['path'])
-        if len(allowed_methods) == 0:
-          await self._handle_404(send, cors)
-          return
-
-        await Reply(send, logger, cors=cors)._options(allowed_methods)
-        return
-
-      await Reply(send, logger, cors=cors).code(405).json({'error': 'Method not allowed'}).send()
-  
-    elif scope['type'] == 'lifespan':
-      await self._handle_lifespan(receive, send)
-
-  async def _handle_lifespan(self, receive, send):
-    while True:
-      message = await receive()
-      if message['type'] == 'lifespan.startup':
-        for startup_event in self._events['startup']:
-          await run_async_or_sync(startup_event)
-        
-        await send({'type': 'lifespan.startup.complete'})
-
-      elif message['type'] == 'lifespan.shutdown':
-        for shutdown_event in self._events['shutdown']:
-          await run_async_or_sync(shutdown_event)
-
-        await send({'type': 'lifespan.shutdown.complete'})
-        return
-
-  async def _handle_http_request(self, scope, receive, send, cors):
-    if '.' in scope['path'].split('/')[-1]:
-      await Reply(send, logger, cors=cors, static_path=self._static_path)._send_archive(scope['path'])
-      return
-    
-    route, params = self._router.find_route(scope['method'], scope['path'], return_params=True)
-    if route is None:
-      await self._handle_404(send, cors)
-      return
-
-    scope['params'] = params
-    request = Request(scope, receive, logger, self._decorators)
-    reply = Reply(send, logger, request, cors, self._static_path, self._decorators, route['hooks'])
-
-    try:
-      await self._handle_request_lifecycle(route, request, reply)
-
-    except Exception as e:
-      await self._handle_exception(route['hooks'], request, reply, e)
-
-  async def _handle_request_lifecycle(self, route, request, reply):
-    route_hooks = route['hooks']
-    route_middlewares = route['middlewares']
-
-    await handler_middlewares(route_middlewares, request, RestrictReply(reply))
-    await handler_hooks(route_hooks['onRequest'], request, reply)
-    if reply.is_sent:
-      return
-    
-    await request._load_body()
-    await handler_hooks(route_hooks['preHandler'], request, reply)
-    if reply.is_sent:
-      return
-    
-    await run_async_or_sync(route['handler'], request, reply)
-    if not reply.is_sent:
-      await reply.send_code(200)
-
-  async def _handle_exception(self, route_hooks, request, reply, exception):
-    exception_handler = ExceptionHandler(exception)
-
-    try:
-      if self._error_handler:
-        await run_async_or_sync(self._error_handler, exception, request, reply)
-        return
-      
-      await self._default_error_handling(exception, reply, exception_handler)
-
-    except Exception as exception:
-      exception_handler = ExceptionHandler(exception)
-
-      if not route_hooks['onError']:
-        await self._default_error_handling(exception, reply, exception_handler, internal=False)
-        return
-
-      try:
-        await handler_hooks(route_hooks['onError'], request, reply, exception)
-
-      except Exception as exception:
-        exception_handler = ExceptionHandler(exception)
-        await self._default_error_handling(exception, reply, exception_handler, internal=False)
-
-  async def _default_error_handling(self, exception, reply, exception_handler, internal = True):
-    if not internal or issubclass(type(exception), FastipyBaseException):
-      await reply.code(500).json({'error': f'{exception_handler.type}: {exception_handler.message}'}).send()
-      print(traceback.format_exc())
-    else:
-      raise exception
+    async def __call__(self, scope, receive, send):
+        if scope["type"] == "http":
+            cors = self._cors.generate_headers() if self._cors else {}
+
+            if scope["method"] in ["POST", "GET", "PUT", "PATCH", "DELETE", "HEAD"]:
+                await self._handle_http_request(scope, receive, send, cors)
+                return
+
+            elif scope["method"] == "OPTIONS":
+                allowed_methods = self._router.get_methods(scope["path"])
+                if len(allowed_methods) == 0:
+                    await self._handle_404(send, cors)
+                    return
+
+                await Reply(send, cors=cors)._options(allowed_methods)
+                return
+
+            await Reply(send, cors=cors).code(405).json(
+                {"error": "Method not allowed"}
+            ).send()
+
+        elif scope["type"] == "lifespan":
+            await self._handle_lifespan(receive, send)
+
+    async def _handle_lifespan(self, receive, send):
+        while True:
+            message = await receive()
+            if message["type"] == "lifespan.startup":
+                for startup_event in self._events["startup"]:
+                    await run_async_or_sync(startup_event)
+
+                await send({"type": "lifespan.startup.complete"})
+
+            elif message["type"] == "lifespan.shutdown":
+                for shutdown_event in self._events["shutdown"]:
+                    await run_async_or_sync(shutdown_event)
+
+                await send({"type": "lifespan.shutdown.complete"})
+                return
+
+    async def _handle_http_request(self, scope, receive, send, cors):
+        if "." in scope["path"].split("/")[-1]:
+            await Reply(send, cors=cors, static_path=self._static_path)._send_archive(
+                scope["path"]
+            )
+            return
+
+        route, params = self._router.find_route(
+            scope["method"], scope["path"], return_params=True
+        )
+        if route is None:
+            await self._handle_404(send, cors)
+            return
+
+        scope["params"] = params
+        request = Request(scope, receive, self._decorators)
+        self._serializers: list = self._serializers
+        reply = Reply(
+            send,
+            request,
+            cors,
+            self._static_path,
+            self._decorators,
+            route["hooks"],
+            self._serializers,
+        )
+
+        try:
+            await self._handle_request_lifecycle(route, request, reply)
+
+        except Exception as e:
+            await self._handle_exception(route["hooks"], request, reply, e)
+
+    async def _handle_request_lifecycle(self, route, request, reply):
+        route_hooks = route["hooks"]
+        route_middlewares = route["middlewares"]
+
+        await handler_middlewares(route_middlewares, request, RestrictReply(reply))
+        await handler_hooks(route_hooks["onRequest"], request, reply)
+        if reply.is_sent:
+            return
+
+        await request._load_body()
+        await handler_hooks(route_hooks["preHandler"], request, reply)
+        if reply.is_sent:
+            return
+
+        await run_async_or_sync(route["handler"], request, reply)
+        if not reply.is_sent:
+            await reply.send_code(200)
+
+    async def _handle_exception(self, route_hooks, request, reply, exception):
+        try:
+            exception_handler = ExceptionHandler(exception)
+
+            await handler_hooks(route_hooks["onError"], request, reply, exception)
+            if reply.is_sent:
+                return
+
+            if self._error_handler:
+                await run_async_or_sync(self._error_handler, exception, request, reply)
+                if reply.is_sent:
+                    return
+
+            await self._default_error_handling(exception, reply, exception_handler)
+        except Exception as exception:
+            exception_handler = ExceptionHandler(exception)
+
+            await self._default_error_handling(
+                exception, reply, exception_handler, internal=True
+            )
+
+    async def _default_error_handling(
+        self, exception, reply: Reply, exception_handler, internal=False
+    ):
+        if internal or issubclass(type(exception), FastipyBaseException):
+            await reply._send_error(
+                message=f"{exception_handler.type}: {exception_handler.message.replace('\"', "'")}",
+                code=500,
+            )
+            print(traceback.format_exc())
+        else:
+            raise exception
 
-  async def _handle_404(self, send, cors):
-    await Reply(send, logger, cors=cors).code(404).json({'error': 'Route not found'}).send()
+    async def _handle_404(self, send, cors):
+        await Reply(send, cors=cors)._send_error(message="Route not found", code=404)
```

### Comparing `fastipy-1.5.0/app/fastipy/src/database/json_database.py` & `fastipy-1.5.1/app/fastipy/src/classes/json_database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,100 @@
 from pathlib import Path
 import json, uuid
 
+
 class Database:
-  def __init__(self):
-    self.database = {}
-    self.path     = Path(__file__).parent.parent / 'db.json'
-    
-    self.__load()
-
-  def __load(self) -> None:
-    if not self.path.exists():
-      self.__persist()
-      return
-
-    with open(self.path, 'r') as f:
-      self.database = json.load(f)
-
-  def __persist(self) -> None:
-    with open(self.path, 'w') as f:
-      json.dump(self.database, f, indent=2)
-
-  def select(self, table: dict, search: dict = None) -> list:
-    try:
-      return [row for row in self.database[table] if all(
-        (row.get(key) == value if not isinstance(value, str) else value.lower() in str(row.get(key, '')).lower())
-        for key, value in search.items()
-      )] if search else self.database[table]
-    except KeyError:
-      return []
-    
-  def find_by_id(self, table: str, _id: str) -> dict:
-    for row in self.database[table]:
-      if row['_id'] == _id:
-        return row
-
-    return {}
-    
-  def find_unique(self, table: str, search: dict) -> dict:
-    try:
-      return next(row for row in self.database[table] if all(
-        (row.get(key) == value if not isinstance(value, str) else value.lower() in str(row.get(key, '')).lower())
-        for key, value in search.items()
-      ))
-    except StopIteration:
-      return {}
-      
-  def insert(self, table: str, data: dict) -> dict:
-    if data == {}:
-      raise Exception("Data cannot be empty")
-
-    data = {'_id': str(uuid.uuid4()), **data}
-
-    try:
-      self.database[table].append(data)
-    except:
-      self.database[table] = [data]
-
-    self.__persist()
-
-    return data
-
-  def delete(self, table: str, _id: str) -> bool:
-    for row in self.database[table]:
-      if row['_id'] == _id:
-        self.database[table].remove(row)
+    def __init__(self):
+        self.database = {}
+        self.path = Path(__file__).parent.parent / "db.json"
+
+        self.__load()
+
+    def __load(self) -> None:
+        if not self.path.exists():
+            self.__persist()
+            return
+
+        with open(self.path, "r") as f:
+            self.database = json.load(f)
+
+    def __persist(self) -> None:
+        with open(self.path, "w") as f:
+            json.dump(self.database, f, indent=2)
+
+    def select(self, table: dict, search: dict = None) -> list:
+        try:
+            return (
+                [
+                    row
+                    for row in self.database[table]
+                    if all(
+                        (
+                            row.get(key) == value
+                            if not isinstance(value, str)
+                            else value.lower() in str(row.get(key, "")).lower()
+                        )
+                        for key, value in search.items()
+                    )
+                ]
+                if search
+                else self.database[table]
+            )
+        except KeyError:
+            return []
+
+    def find_by_id(self, table: str, _id: str) -> dict:
+        for row in self.database[table]:
+            if row["_id"] == _id:
+                return row
+
+        return {}
+
+    def find_unique(self, table: str, search: dict) -> dict:
+        try:
+            return next(
+                row
+                for row in self.database[table]
+                if all(
+                    (
+                        row.get(key) == value
+                        if not isinstance(value, str)
+                        else value.lower() in str(row.get(key, "")).lower()
+                    )
+                    for key, value in search.items()
+                )
+            )
+        except StopIteration:
+            return {}
+
+    def insert(self, table: str, data: dict) -> dict:
+        if data == {}:
+            raise Exception("Data cannot be empty")
+
+        data = {"_id": str(uuid.uuid4()), **data}
+
+        try:
+            self.database[table].append(data)
+        except:
+            self.database[table] = [data]
+
         self.__persist()
-        return True
 
-    return False
+        return data
 
-  def update(self, table: str, _id: str, data: dict) -> bool:
-    for row in self.database[table]:
-      if row['_id'] == _id:
-        row.update(data)
-        self.__persist()
-        return True
+    def delete(self, table: str, _id: str) -> bool:
+        for row in self.database[table]:
+            if row["_id"] == _id:
+                self.database[table].remove(row)
+                self.__persist()
+                return True
+
+        return False
+
+    def update(self, table: str, _id: str, data: dict) -> bool:
+        for row in self.database[table]:
+            if row["_id"] == _id:
+                row.update(data)
+                self.__persist()
+                return True
 
-    return False
-  
+        return False
```

### Comparing `fastipy-1.5.0/app/fastipy/src/exceptions/exception_handler.py` & `fastipy-1.5.1/app/fastipy/src/models/file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,89 @@
-import traceback
+import uuid, json, io
+from uvicorn.main import logger
 
-class ExceptionHandler:
-  def __init__(self, error: Exception):
-    self._error     = error
-    self._type      = type(error).__name__
-    self._message   = str(error)
-    self._traceback = traceback.format_exc()
-
-  def __str__(self) -> str:
-    return f"{self.type}: {self.message}"
-
-  @property
-  def error(self) -> Exception:
-    return self._error
-  
-  @property
-  def type(self) -> str:
-    return self._type
-  
-  @property
-  def message(self) -> str:
-    return self._message
-  
-  @property
-  def traceback(self) -> str:
-    return self._traceback
-  
-  def __html__(self) -> str:
-    return f"""
-    <html>
-      <head>
-        <title>{self._type}</title>
-        <style type="text/css">
-        {'''
-          * {
-            box-sizing: border-box;
-            padding: 0;
-            margin: 0;
-          }
-
-          body {
-            background-color: #8B5CF6;
-            font-family: 'Roboto', sans-serif;
-            color: #E2E8F0;
-            font-weight: 700;
-            padding: 2.625rem;
-          }
-
-          h1 {
-            font-size: 4rem;
-            color: #FFF;
-          }
-
-          h2 {
-            font-size: 2.25rem;
-            margin-bottom: 2rem;
-          }
-
-          pre {
-            font-size: 1.25rem;
-            margin-bottom: 1rem;
-          }
-        '''}
-        </style>
-      </head>
-      <body>
-        <h1>{self._type}</h1>
-        <h2>{self._message}</h2>
-        <h1>Traceback</h1>
-        <pre>{self._traceback}</pre>
-      </body>
-    </html>
-    """
+from ..exceptions import FileException
+
+
+class File:
+    def __init__(self, filename: str, type: str, data: bytes):
+        self._filename = filename
+        self._type = type
+        self._data = data
+
+        self._text = None
+        self._json = None
+
+        self.__text()
+        self.__json()
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def filename(self) -> str:
+        return self._filename
+
+    @property
+    def type(self) -> str:
+        return self._type
+
+    @property
+    def data(self) -> bytes:
+        return self._data
+
+    @property
+    def size(self) -> int:
+        return len(self._data)
+
+    @property
+    def text(self) -> str:
+        return self._text
+
+    @property
+    def json(self) -> dict:
+        return self._json
+
+    def __text(self) -> None:
+        try:
+            self._text = self._data.decode()
+        except:
+            pass
+
+    def __json(self) -> None:
+        if self._type == "application/json":
+            try:
+                self._json = json.loads(self._data)
+            except:
+                pass
+
+    def save(self, path=None) -> None:
+        if path is None:
+            path = self._filename
+
+        try:
+            with io.open(path, "wb") as file:
+                file.write(self._data)
+        except:
+            raise FileException(f"Could not save file in '{path}'", logger.error)
+
+    def safe_save(self, path=None) -> str:
+        if path is None:
+            path = self._filename
+
+        filename = path.split("/")[-1]
+
+        id = str(uuid.uuid4())
+
+        name = filename.split(".")[0]
+        extension = filename.split(".")[-1] if len(filename.split(".")) > 1 else None
+
+        path = f"{name}_{id}{f'.{extension}' if extension else ''}"
+
+        try:
+            with io.open(path, "wb") as file:
+                file.write(self._data)
+        except:
+            raise FileException(f"Could not save file in '{path}'", logger.error)
+
+        return path
```

### Comparing `fastipy-1.5.0/app/fastipy/src/models/body.py` & `fastipy-1.5.1/app/fastipy/src/models/body.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 from typing import Union
 import json
 
 from .form import Form
 
-class Body():
-  def __init__(self, scope, receive) -> None:
-    self.__scope         = scope
-    self.__receive       = receive
-
-    self._content        = None
-    self._raw_content    = None
-    self._content_type   = self.__scope['headers'].get('content-type', None)
-    self._content_length = int(self.__scope['headers'].get('content-length', 0))
-    self._json           = None
-
-  @property
-  def type(self) -> Union[str, None]:
-    return self._content_type
-  
-  @property
-  def length(self) -> int:
-    return self._content_length
-  
-  @property
-  def content(self) -> str:
-    return self._content
-  
-  @property
-  def raw_content(self) -> bytes:
-    return self._raw_content
-  
-  @property
-  def json(self) -> dict:
-    return self._json
-  
-  @property
-  def form(self) -> 'Form':
-    return self._form
-  
-  async def load(self):
-    content = await self.__receive()
-    self._raw_content = content['body']
-
-    while content['more_body']:
-      content = await self.__receive()
-      self._raw_content += content['body']
-
-    try:
-      self._content = self._raw_content.decode()
-    except: pass
-
-    self.__json()
-
-    self._form = Form(self)
-
-  def __json(self) -> None:
-    if self._content_type == 'application/json':
-      try:
-        self._json = json.loads(self._raw_content)
-      except: pass
+
+class Body:
+    def __init__(self, scope, receive) -> None:
+        self.__scope = scope
+        self.__receive = receive
+
+        self._content = None
+        self._raw_content = None
+        self._content_type = self.__scope["headers"].get("content-type", None)
+        self._content_length = int(self.__scope["headers"].get("content-length", 0))
+        self._json = None
+
+    @property
+    def type(self) -> Union[str, None]:
+        return self._content_type
+
+    @property
+    def length(self) -> int:
+        return self._content_length
+
+    @property
+    def content(self) -> str:
+        return self._content
+
+    @property
+    def raw_content(self) -> bytes:
+        return self._raw_content
+
+    @property
+    def json(self) -> dict:
+        return self._json
+
+    @property
+    def form(self) -> "Form":
+        return self._form
+
+    async def load(self):
+        content = await self.__receive()
+        self._raw_content = content["body"]
+
+        while content.get("more_body"):
+            content = await self.__receive()
+            self._raw_content += content["body"]
+
+        try:
+            self._content = self._raw_content.decode()
+        except:
+            pass
+
+        self.__json()
+
+        self._form = Form(self)
+
+    def __json(self) -> None:
+        if self._content_type == "application/json":
+            try:
+                self._json = json.loads(self._raw_content)
+            except:
+                pass
```

### Comparing `fastipy-1.5.0/app/fastipy/src/models/form.py` & `fastipy-1.5.1/app/fastipy/src/models/form.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,62 @@
 from typing import TYPE_CHECKING, Dict
 
 from .file import File
 
 if TYPE_CHECKING:
-  from .body import Body
+    from .body import Body
+
 
 class Form:
-  def __init__(self, body: 'Body'):
-    self._body    = body
-    self._fields  = {}
-    self._files   = {}
-    
-    self.__get_variables()
-
-  @property
-  def fields(self) -> Dict[str, str]:
-    return self._fields
-  
-  @property
-  def files(self) -> Dict[str, File]:
-    return self._files
-  
-  def __get_variables(self) -> None:
-    if self._body.type is None:
-      return
-
-    if 'multipart/form-data' in self._body.type:
-      body_parts = self._body.raw_content.split(b'Content-Disposition: form-data; name="')
-      for i in range(1, len(body_parts)):
-        name = body_parts[i].split(b'"')[0].decode()
-        filename = body_parts[i].split(b'filename="')[1].split(b'"')[0].decode() if b'filename="' in body_parts[i] else None
-        filetype = body_parts[i].split(b'Content-Type: ')[1].split(b'\r\n')[0].decode() if b'Content-Type: ' in body_parts[i] else None
-        data = body_parts[i].split(b'\r\n\r\n')[1].split(b'\r\n----------------------------')[0].split(b'\r\n--')[0]
-
-        if filename:
-          self._files[name] = File(filename, filetype, data)
-        else:
-          self._fields[name] = data.decode()
-
-    elif 'application/x-www-form-urlencoded' in self._body.type:
-      body_parts = self._body.raw_content.split(b'&')
-      for i in body_parts:
-        name = i.split(b'=')[0].decode()
-        value = i.split(b'=')[1].decode()
-        self._fields[name] = value
+    def __init__(self, body: "Body"):
+        self._body = body
+        self._fields = {}
+        self._files = {}
+
+        self.__get_variables()
+
+    @property
+    def fields(self) -> Dict[str, str]:
+        return self._fields
+
+    @property
+    def files(self) -> Dict[str, File]:
+        return self._files
+
+    def __get_variables(self) -> None:
+        if self._body.type is None:
+            return
+
+        if "multipart/form-data" in self._body.type:
+            body_parts = self._body.raw_content.split(
+                b'Content-Disposition: form-data; name="'
+            )
+            for i in range(1, len(body_parts)):
+                name = body_parts[i].split(b'"')[0].decode()
+                filename = (
+                    body_parts[i].split(b'filename="')[1].split(b'"')[0].decode()
+                    if b'filename="' in body_parts[i]
+                    else None
+                )
+                filetype = (
+                    body_parts[i].split(b"Content-Type: ")[1].split(b"\r\n")[0].decode()
+                    if b"Content-Type: " in body_parts[i]
+                    else None
+                )
+                data = (
+                    body_parts[i]
+                    .split(b"\r\n\r\n")[1]
+                    .split(b"\r\n----------------------------")[0]
+                    .split(b"\r\n--")[0]
+                )
+
+                if filename:
+                    self._files[name] = File(filename, filetype, data)
+                else:
+                    self._fields[name] = data.decode()
+
+        elif "application/x-www-form-urlencoded" in self._body.type:
+            body_parts = self._body.raw_content.split(b"&")
+            for i in body_parts:
+                name = i.split(b"=")[0].decode()
+                value = i.split(b"=")[1].decode()
+                self._fields[name] = value
```

### Comparing `fastipy-1.5.0/app/fastipy/src/routes/plugin_tree.py` & `fastipy-1.5.1/app/fastipy/src/routes/plugin_tree.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from typing import List, Optional
 
+
 class PluginNode:
-  def __init__(self, name: str = ''):
-    self.name = name
-    self.children: List['PluginNode'] = []
-
-  def add_child(self, child: 'PluginNode'):
-    self.children.append(child)
-
-  def print_tree(self, node: Optional['PluginNode'] = None, indent: str = ""):
-    if node is None:
-      node = self
-
-    for idx, child in enumerate(node.children):
-      symbol = "└──" if idx == len(node.children) - 1 else "├──"
-      
-      if not child.children:
-        print(f"{indent}{symbol} {child.name}")
-      else:
-        print(f"{indent}{symbol} {child.name}")
-        self.print_tree(child, indent + ("    " if symbol == "└──" else "│   "))
+    def __init__(self, name: str = ""):
+        self.name = name
+        self.children: List["PluginNode"] = []
+
+    def add_child(self, child: "PluginNode"):
+        self.children.append(child)
+
+    def print_tree(self, node: Optional["PluginNode"] = None, indent: str = ""):
+        if node is None:
+            node = self
+
+        for idx, child in enumerate(node.children):
+            symbol = "└──" if idx == len(node.children) - 1 else "├──"
+
+            if not child.children:
+                print(f"{indent}{symbol} {child.name}")
+            else:
+                print(f"{indent}{symbol} {child.name}")
+                self.print_tree(child, indent + ("    " if symbol == "└──" else "│   "))
+
 
 class PluginTree(PluginNode):
-  def __init__(self):
-    super().__init__()
-    self.root = PluginNode("root")
-    self.children = [self.root]
+    def __init__(self):
+        super().__init__()
+        self.root = PluginNode("root")
+        self.children = [self.root]
 
-  def add_child(self, child: PluginNode):
-    self.root.add_child(child)
+    def add_child(self, child: PluginNode):
+        self.root.add_child(child)
```

### Comparing `fastipy-1.5.0/app/fastipy/src/types/routes.py` & `fastipy-1.5.1/app/fastipy/src/types/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Callable, Coroutine, Union
 import sys
 
 if sys.version_info < (3, 11):
-  from typing_extensions import TypedDict, NotRequired, List, Callable
+    from typing_extensions import TypedDict, NotRequired, List, Callable
 else:
-  from typing import TypedDict, NotRequired, List, Callable
+    from typing import TypedDict, NotRequired, List, Callable
 
 FunctionType = Union[Callable, Coroutine]
 
+
 class RouteHookType(TypedDict):
-  onRequest: NotRequired[List[FunctionType]]
-  preHandler: NotRequired[List[FunctionType]]
-  onResponse: NotRequired[List[FunctionType]]
-  onError: NotRequired[List[FunctionType]]
+    onRequest: NotRequired[List[FunctionType]]
+    preHandler: NotRequired[List[FunctionType]]
+    onResponse: NotRequired[List[FunctionType]]
+    onError: NotRequired[List[FunctionType]]
+
 
-RouteMiddlewareType = List[FunctionType]
+RouteMiddlewareType = List[FunctionType]
```

### Comparing `fastipy-1.5.0/app/fastipy.egg-info/PKG-INFO` & `fastipy-1.5.1/app/fastipy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastipy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.
 Home-page: https://github.com/Bielgomes/Fastipy
 Author: Bielgomes
 Author-email: bielgomesdasilva@hotmail.com
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/Bielgomes/Fastipy/issues
 Classifier: Development Status :: 4 - Beta
@@ -17,19 +17,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: uvicorn[standard]
+Requires-Dist: starlette
+Requires-Dist: nest-asyncio
+Requires-Dist: Jinja2
 
 # Fastipy
 
 <div>
-  <img src="https://media.discordapp.net/attachments/887158781832749086/1187385388571037778/fastipy-extended.png">
+  <img src="https://i.imgur.com/KCi8IUS.png">
 </div>
 
 ## What is it and what is it for
 
 [Fastipy](https://pypi.org/project/Fastipy/) is a fast and easy-to-use open source Python library for developing RESTful APIs.
 
 Powered by **[uvicorn](https://www.uvicorn.org/)**
@@ -38,109 +42,144 @@
 
 ```bash
 pip install fastipy
 ```
 
 ## Examples
 
-### Example for GET Route with Query Params and debug mode
+### Example for GET Route with Query Params
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
-# Debug mode is False by default
 app = Fastipy()
 
 # Routes can be async or sync functions, but reply send functions are async
 # The handler returns the default HTTP status code 200
 @app.get('/')
-def home(req: Request, reply: Reply):
+def home(req: Request, _):
   # Get query params age
   age = req.query['age']
   # Example: Recovery all persons from database with this age and print the html
-  print("<h1>Listing all persons</h1><ul><li>A Person</li></ul>")
+  print("<h1>Retrieving all persons</h1><ul><li>A Person</li></ul>")
 ```
 
 ### Example for GET Route with Params, CORS and multiple methods
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy().cors()
 
 @app.get('/user/:id')
 @app.post('/user/:id')
 async def getUser(req: Request, reply: Reply):
   # get users from database
   for i in users:
     if i["id"] == req.params["id"]:
-      await reply.json(i).send()
-      return
+      # All response functions are asynchronous
+      return await reply.send(i)
+
   await reply.send_code(404)
 ```
 
 ### Example for POST Route with Body
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 @app.post('/user')
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Save user in database
-  await reply.text("Created").code(201).send()
+  await reply.code(201).send("Created")
 ```
 
 ### Example for PUT Route with Body
 
-```python
+```py
 from fastipy import Fastipy, Request, Reply
 
 app = Fastipy()
 
 @app.put('/user')
 async def createUser(req: Request, reply: Reply):
   user = req.body.json
   # Update user in database
-  await reply.html('<h1>Created</h1>').code(201).send()
+  await reply.type("text/html").code(201).send("<h1>Created</h1>")
+```
+
+### Example for GET Route with file stream
+
+```py
+from fastipy import Fastipy, Request, Reply
+
+app = Fastipy()
+
+@app.get('/stream')
+async def streamFile(_, reply: Reply):
+  # It could be an asynchronous generator
+  def generator():
+    with open("file.txt") as f:
+        for line in f:
+            yield line
+
+  await reply.send(generator())
+```
+
+### Adding custom serializer to Reply send
+
+```py
+from fastipy import Fastipy, Request, Reply
+
+app = Fastipy()
+
+app.add_serializer(
+    validation=lambda data: isinstance(data, str),
+    serializer=lambda data: ("application/json", json.dumps({"error": data})),
+)
+
+@app.get("/")
+async def customSerializer(_, reply: Reply):
+    await reply.code(404).send("Field not found")
 ```
 
 ### See more examples in **[examples](https://github.com/Bielgomes/Fastipy/tree/main/examples)** folder
 
 ## Creating plugins
 
 ```py
 # chat.py
 from fastipy import FastipyInstance, Reply
 
 # Plugins can be asynchronous or synchronized functions
-# Plugins have the main instance as a parameter, which means they can use all of Fastipy's functions
+# Plugins have access to the main instance, which means they can use all of Fastipy's functions
 def chatRoutes(app: FastipyInstance, options: dict):
   @app.get('/')
-  async def index(req: Request, reply: Reply):
+  async def index(_, reply: Reply):
     await reply.send_code(200)
 
   @app.get('/chat')
-  async def test(req: Request, reply: Reply):
+  async def test(_, reply: Reply):
     await reply.send_code(200)
 ```
 
 ```py
 # message.py
 from fastipy import FastipyInstance, Reply
 
 async def messageRoutes(app: FastipyInstance, options: dict):
   @message.get('/')
-  async def index(req: Request, reply: Reply):
+  async def index(_, reply: Reply):
     await reply.send_code(200)
 
   @message.get('/message')
-  async def test(req: Request, reply: Reply):
+  async def test(_, reply: Reply):
     await reply.send_code(200)
 
   app.name('custom plugin name')
 ```
 
 ```py
 # main.py
@@ -175,27 +214,41 @@
 # The onResponse hook is called when the reply sends a response
 @app.hook('onResponse')
 def onResponse(req: Request, reply: Reply):
   print('onResponse hook')
 
 # The onError hook is called when an error occurs
 @app.hook('onError')
-def onError(req: Request, reply: Reply, error):
-  print('onError hook')
+def onError(error: Exception, req: Request, reply: Reply):
+  print(f'onError hook exception: {error}')
 
 # A hook will only be linked to a route if its declaration precedes the route
 # The order of hooks of the same type is important
 @app.get('/')
-async def index(req: Request, reply: Reply):
+async def index(_, reply: Reply):
   await reply.send_code(200)
 ```
 
+## End to End tests
+
+```py
+# See more in https://www.starlette.io/testclient/
+from fastipy import TestClient
+from main import app
+
+client = TestClient(app)
+
+response = client.post("/")
+assert response.status_code == 200
+assert response.text == "Hello World"
+```
+
 ## Running
 
-Run Fastipy application in development is easy
+Running Fastipy application in development is easy
 
 ```py
 import uvicorn
 
 if __name__ == "__main__":
   # main:app indicates the FILE:VARIABLE
 
@@ -211,45 +264,33 @@
 
 # Application Deploy
 
 For production deployment, please refer to this **[uvicorn guide](https://www.uvicorn.org/deployment/)**.
 
 # Change Log
 
-## Version 1.5.0
+## Development Version 1.5.1
 
 ### Added
 
-- [x] Request method PATCH
-- [x] More security in CORS
-- [x] JSON Database module
-- [x] Add support to hooks (onRequest, onResponse, onError)
-- [x] Add support to plugins
-- [x] Add decorators to routes (decorator, decorate_request, decorate_reply)
-- [x] Add support to middlewares
-- [x] Add support for lifespan events (startup, shutdown)
-- [x] New preHandler hook
-- [x] Add stream file support
-- [x] Automatic OPTIONS method response for routes
-- [x] Custom global error handler
+- [X] Added the possibility of printing middleware routes in the router's print tree.
+- [X] Added a customizable mail module.
+- [X] Added jinja2 lib to render templates.
+- [x] Add integration to end-to-end tests.
 
 ### Changed
 
-- [x] Better params and query params recovery in routes
-- [x] Improved route logging
-- [x] Refactor structure of project
-- [x] Refactor Routes class
-- [x] Routes handler can be a sync function
-- [x] Better route search algorithm and structure
-- [x] It is now possible to add specific hooks and middlewares to a route
-- [x] Implementation of uvicorn HTTP web server
-- [x] Better error handler
+- [X] Error imports are now centralized in the exceptions module.
+- [X] Improved error handling flow, now error handling hooks are executed first rather than the default error handling.
+- [X] Apply code reuse to generate logs.
+- [X] Refactored file stream in reply send file function.
+- [X] Reply send function now automatically serializes the value sent to it and sets a content type
 
 # Contributors
 
 <a href="https://github.com/Bielgomes/Fastipy/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Bielgomes/Fastipy"/>
 </a>
 
 ## How to Contributing
 
-Open pull request ðŸ˜Ž
+Open pull request
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastipy-1.5.0/app/fastipy.egg-info/SOURCES.txt` & `fastipy-1.5.1/app/fastipy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,41 +6,44 @@
 app/fastipy.egg-info/SOURCES.txt
 app/fastipy.egg-info/dependency_links.txt
 app/fastipy.egg-info/requires.txt
 app/fastipy.egg-info/top_level.txt
 app/fastipy/src/__init__.py
 app/fastipy/src/classes/__init__.py
 app/fastipy/src/classes/decorators_base.py
+app/fastipy/src/classes/json_database.py
+app/fastipy/src/classes/mailer.py
+app/fastipy/src/classes/template_render.py
 app/fastipy/src/constants/__init__.py
 app/fastipy/src/constants/content_types.py
 app/fastipy/src/constants/decorators.py
 app/fastipy/src/constants/events.py
 app/fastipy/src/constants/hooks.py
 app/fastipy/src/constants/http_methods.py
 app/fastipy/src/constants/http_status_code.py
+app/fastipy/src/constants/serializers.py
 app/fastipy/src/core/__init__.py
 app/fastipy/src/core/fastipy.py
 app/fastipy/src/core/reply.py
 app/fastipy/src/core/request.py
 app/fastipy/src/core/request_handler.py
-app/fastipy/src/database/__init__.py
-app/fastipy/src/database/json_database.py
 app/fastipy/src/exceptions/__init__.py
 app/fastipy/src/exceptions/decorator_already_exists_exception.py
 app/fastipy/src/exceptions/duplicate_route_exception.py
 app/fastipy/src/exceptions/exception_handler.py
 app/fastipy/src/exceptions/fastipy_base_exception.py
 app/fastipy/src/exceptions/file_exception.py
 app/fastipy/src/exceptions/invalid_path_exception.py
 app/fastipy/src/exceptions/no_event_type.py
 app/fastipy/src/exceptions/no_hook_type.py
 app/fastipy/src/exceptions/no_http_method_exception.py
 app/fastipy/src/exceptions/reply_exception.py
 app/fastipy/src/helpers/__init__.py
 app/fastipy/src/helpers/async_sync_helpers.py
+app/fastipy/src/helpers/content_type.py
 app/fastipy/src/helpers/route_helpers.py
 app/fastipy/src/middlewares/__init__.py
 app/fastipy/src/middlewares/cors.py
 app/fastipy/src/models/__init__.py
 app/fastipy/src/models/body.py
 app/fastipy/src/models/file.py
 app/fastipy/src/models/form.py
```

### Comparing `fastipy-1.5.0/setup.py` & `fastipy-1.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="fastipy",
-    version="1.5.0",
+    version="1.5.1",
     description="Fastipy is a fast and easy-to-use open source Python library for developing RESTful APIs. Inspired by the FastAPI and Fastify syntax and powered by uvicorn ASGI web server.",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bielgomes/Fastipy",
     author="Bielgomes",
     author_email="bielgomesdasilva@hotmail.com",
     license="GNU Affero General Public License v3",
-    project_urls={
-        "Bug Tracker": "https://github.com/Bielgomes/Fastipy/issues"
-    },
+    project_urls={"Bug Tracker": "https://github.com/Bielgomes/Fastipy/issues"},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    install_requires=["uvicorn[standard]", "nest-asyncio"],
+    install_requires=[
+        "uvicorn[standard]",
+        "starlette",
+        "nest-asyncio",
+        "Jinja2",
+    ],
     python_requires=">=3.10",
-)
+)
```

