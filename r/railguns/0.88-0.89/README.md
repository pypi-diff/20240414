# Comparing `tmp/railguns-0.88.tar.gz` & `tmp/railguns-0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "railguns-0.88.tar", last modified: Sun Mar 24 08:46:08 2024, max compression
+gzip compressed data, was "railguns-0.89.tar", last modified: Sun Apr 14 20:16:18 2024, max compression
```

## Comparing `railguns-0.88.tar` & `railguns-0.89.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.724924 railguns-0.88/
--rw-r--r--   0 ny         (501) staff       (20)     1089 2022-06-18 13:16:59.000000 railguns-0.88/LICENSE
--rw-r--r--   0 ny         (501) staff       (20)      109 2022-06-18 13:16:59.000000 railguns-0.88/MANIFEST.in
--rw-r--r--   0 ny         (501) staff       (20)     3898 2024-03-24 08:46:08.724739 railguns-0.88/PKG-INFO
--rw-r--r--   0 ny         (501) staff       (20)     1277 2024-03-15 10:46:58.000000 railguns-0.88/README.md
--rw-r--r--   0 ny         (501) staff       (20)     1602 2024-03-24 08:45:45.000000 railguns-0.88/pyproject.toml
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.717801 railguns-0.88/railguns/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/__init__.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.718726 railguns-0.88/railguns/cloudfile/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/cloudfile/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      470 2024-03-03 23:42:05.000000 railguns-0.88/railguns/cloudfile/fields.py
--rw-r--r--   0 ny         (501) staff       (20)     1137 2024-03-03 23:42:05.000000 railguns-0.88/railguns/cloudfile/widgets.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.718967 railguns-0.88/railguns/django/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/django/__init__.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.719210 railguns-0.88/railguns/django/contrib/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/django/contrib/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     2324 2024-03-03 23:48:32.000000 railguns-0.88/railguns/django/contrib/admin.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.719422 railguns-0.88/railguns/django/contrib/auth/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/django/contrib/auth/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      855 2024-03-03 23:42:05.000000 railguns-0.88/railguns/django/contrib/auth/backends.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.719741 railguns-0.88/railguns/django/db/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/django/db/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     3140 2024-03-03 23:42:05.000000 railguns-0.88/railguns/django/db/models.py
--rw-r--r--   0 ny         (501) staff       (20)     2190 2024-03-03 23:42:05.000000 railguns-0.88/railguns/django/db/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     1778 2024-03-04 13:14:48.000000 railguns-0.88/railguns/django/generics.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.720062 railguns-0.88/railguns/django/utils/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/django/utils/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      459 2024-03-03 23:42:05.000000 railguns-0.88/railguns/django/utils/html.py
--rw-r--r--   0 ny         (501) staff       (20)      777 2024-03-03 23:42:05.000000 railguns-0.88/railguns/django/utils/translation.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.720985 railguns-0.88/railguns/rest_framework/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/rest_framework/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     1614 2024-03-03 23:42:05.000000 railguns-0.88/railguns/rest_framework/generics.py
--rw-r--r--   0 ny         (501) staff       (20)     2762 2024-03-03 23:42:05.000000 railguns-0.88/railguns/rest_framework/mixins.py
--rw-r--r--   0 ny         (501) staff       (20)      306 2024-03-03 23:42:05.000000 railguns-0.88/railguns/rest_framework/pagination.py
--rw-r--r--   0 ny         (501) staff       (20)     1750 2024-03-03 23:42:05.000000 railguns-0.88/railguns/rest_framework/permissions.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.721225 railguns-0.88/railguns/rest_framework/schemas/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/rest_framework/schemas/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      948 2024-03-03 23:42:05.000000 railguns-0.88/railguns/rest_framework/schemas/openapi.py
--rw-r--r--   0 ny         (501) staff       (20)      746 2022-06-18 13:16:59.000000 railguns-0.88/railguns/rest_framework/serializers.py
--rw-r--r--   0 ny         (501) staff       (20)      128 2024-03-03 23:42:05.000000 railguns-0.88/railguns/rest_framework/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     6642 2024-03-03 23:42:05.000000 railguns-0.88/railguns/rest_framework/views.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.716528 railguns-0.88/railguns/static/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.716467 railguns-0.88/railguns/static/cloudfile/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.721344 railguns-0.88/railguns/static/cloudfile/js/
--rw-r--r--   0 ny         (501) staff       (20)     5251 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/cloudfile/js/scripts.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.716759 railguns-0.88/railguns/static/railguns/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.722038 railguns-0.88/railguns/static/railguns/es2015/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.722302 railguns-0.88/railguns/static/railguns/es2015/components/
--rw-r--r--   0 ny         (501) staff       (20)    16351 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/railguns/es2015/components/weui-components.js
--rw-r--r--   0 ny         (501) staff       (20)     1691 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/railguns/es2015/mixins.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.722539 railguns-0.88/railguns/static/railguns/es2015/util/
--rw-r--r--   0 ny         (501) staff       (20)     2000 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/railguns/es2015/util/http-utils.js
--rw-r--r--   0 ny         (501) staff       (20)      555 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/railguns/es2015/vendor.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.722848 railguns-0.88/railguns/static/railguns/js/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.722987 railguns-0.88/railguns/static/railguns/js/components/
--rw-r--r--   0 ny         (501) staff       (20)    13372 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/railguns/js/components/weui-components.js
--rw-r--r--   0 ny         (501) staff       (20)     1160 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/railguns/js/mixins.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.723301 railguns-0.88/railguns/static/railguns/js/util/
--rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/railguns/js/util/http-utils.js
--rw-r--r--   0 ny         (501) staff       (20)      346 2022-06-18 13:16:59.000000 railguns-0.88/railguns/static/railguns/js/vendor.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.716996 railguns-0.88/railguns/templates/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.723571 railguns-0.88/railguns/templates/railguns/
--rw-r--r--   0 ny         (501) staff       (20)      583 2022-06-18 13:16:59.000000 railguns-0.88/railguns/templates/railguns/base.html
--rw-r--r--   0 ny         (501) staff       (20)     1738 2022-06-18 13:16:59.000000 railguns-0.88/railguns/templates/railguns/base_quick.html
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.723982 railguns-0.88/railguns/templates/railguns/ui/
--rw-r--r--   0 ny         (501) staff       (20)     1325 2022-06-18 13:16:59.000000 railguns-0.88/railguns/templates/railguns/ui/base.html
--rw-r--r--   0 ny         (501) staff       (20)      740 2022-06-18 13:16:59.000000 railguns-0.88/railguns/templates/railguns/ui/detail.html
--rw-r--r--   0 ny         (501) staff       (20)      775 2022-06-18 13:16:59.000000 railguns-0.88/railguns/templates/railguns/ui/list.html
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.724202 railguns-0.88/railguns/tools/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.88/railguns/tools/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      238 2024-03-03 23:42:05.000000 railguns-0.88/railguns/tools/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     1653 2024-03-03 23:42:05.000000 railguns-0.88/railguns/urls.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-03-24 08:46:08.724358 railguns-0.88/railguns.egg-info/
--rw-r--r--   0 ny         (501) staff       (20)     3898 2024-03-24 08:46:08.000000 railguns-0.88/railguns.egg-info/PKG-INFO
--rw-r--r--   0 ny         (501) staff       (20)     1778 2024-03-24 08:46:08.000000 railguns-0.88/railguns.egg-info/SOURCES.txt
--rw-r--r--   0 ny         (501) staff       (20)        1 2024-03-24 08:46:08.000000 railguns-0.88/railguns.egg-info/dependency_links.txt
--rw-r--r--   0 ny         (501) staff       (20)      255 2024-03-24 08:46:08.000000 railguns-0.88/railguns.egg-info/requires.txt
--rw-r--r--   0 ny         (501) staff       (20)        9 2024-03-24 08:46:08.000000 railguns-0.88/railguns.egg-info/top_level.txt
--rw-r--r--   0 ny         (501) staff       (20)       38 2024-03-24 08:46:08.724962 railguns-0.88/setup.cfg
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.923193 railguns-0.89/
+-rw-r--r--   0 ny         (501) staff       (20)     1089 2022-06-18 13:16:59.000000 railguns-0.89/LICENSE
+-rw-r--r--   0 ny         (501) staff       (20)      109 2022-06-18 13:16:59.000000 railguns-0.89/MANIFEST.in
+-rw-r--r--   0 ny         (501) staff       (20)     3898 2024-04-14 20:16:18.922997 railguns-0.89/PKG-INFO
+-rw-r--r--   0 ny         (501) staff       (20)     1277 2024-03-15 10:46:58.000000 railguns-0.89/README.md
+-rw-r--r--   0 ny         (501) staff       (20)     1602 2024-04-14 20:15:27.000000 railguns-0.89/pyproject.toml
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.915913 railguns-0.89/railguns/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/__init__.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.917112 railguns-0.89/railguns/cloudfile/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/cloudfile/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      470 2024-03-03 23:42:05.000000 railguns-0.89/railguns/cloudfile/fields.py
+-rw-r--r--   0 ny         (501) staff       (20)     1137 2024-03-03 23:42:05.000000 railguns-0.89/railguns/cloudfile/widgets.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.917333 railguns-0.89/railguns/django/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/django/__init__.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.917565 railguns-0.89/railguns/django/contrib/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/django/contrib/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     2324 2024-03-03 23:48:32.000000 railguns-0.89/railguns/django/contrib/admin.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.917799 railguns-0.89/railguns/django/contrib/auth/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/django/contrib/auth/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      855 2024-03-03 23:42:05.000000 railguns-0.89/railguns/django/contrib/auth/backends.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.918126 railguns-0.89/railguns/django/db/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/django/db/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     3140 2024-03-03 23:42:05.000000 railguns-0.89/railguns/django/db/models.py
+-rw-r--r--   0 ny         (501) staff       (20)     2190 2024-03-03 23:42:05.000000 railguns-0.89/railguns/django/db/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     1778 2024-03-04 13:14:48.000000 railguns-0.89/railguns/django/generics.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.918475 railguns-0.89/railguns/django/utils/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/django/utils/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      459 2024-03-03 23:42:05.000000 railguns-0.89/railguns/django/utils/html.py
+-rw-r--r--   0 ny         (501) staff       (20)      777 2024-03-03 23:42:05.000000 railguns-0.89/railguns/django/utils/translation.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.919378 railguns-0.89/railguns/rest_framework/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/rest_framework/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     1614 2024-03-03 23:42:05.000000 railguns-0.89/railguns/rest_framework/generics.py
+-rw-r--r--   0 ny         (501) staff       (20)     2762 2024-03-03 23:42:05.000000 railguns-0.89/railguns/rest_framework/mixins.py
+-rw-r--r--   0 ny         (501) staff       (20)      306 2024-03-03 23:42:05.000000 railguns-0.89/railguns/rest_framework/pagination.py
+-rw-r--r--   0 ny         (501) staff       (20)     1750 2024-03-03 23:42:05.000000 railguns-0.89/railguns/rest_framework/permissions.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.919579 railguns-0.89/railguns/rest_framework/schemas/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/rest_framework/schemas/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      948 2024-03-03 23:42:05.000000 railguns-0.89/railguns/rest_framework/schemas/openapi.py
+-rw-r--r--   0 ny         (501) staff       (20)      746 2022-06-18 13:16:59.000000 railguns-0.89/railguns/rest_framework/serializers.py
+-rw-r--r--   0 ny         (501) staff       (20)      128 2024-03-03 23:42:05.000000 railguns-0.89/railguns/rest_framework/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     6642 2024-03-03 23:42:05.000000 railguns-0.89/railguns/rest_framework/views.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.914608 railguns-0.89/railguns/static/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.914542 railguns-0.89/railguns/static/cloudfile/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.919695 railguns-0.89/railguns/static/cloudfile/js/
+-rw-r--r--   0 ny         (501) staff       (20)     5251 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/cloudfile/js/scripts.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.914846 railguns-0.89/railguns/static/railguns/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.920231 railguns-0.89/railguns/static/railguns/es2015/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.920681 railguns-0.89/railguns/static/railguns/es2015/components/
+-rw-r--r--   0 ny         (501) staff       (20)    16351 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/railguns/es2015/components/weui-components.js
+-rw-r--r--   0 ny         (501) staff       (20)     1691 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/railguns/es2015/mixins.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.920891 railguns-0.89/railguns/static/railguns/es2015/util/
+-rw-r--r--   0 ny         (501) staff       (20)     2000 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/railguns/es2015/util/http-utils.js
+-rw-r--r--   0 ny         (501) staff       (20)      555 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/railguns/es2015/vendor.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.921169 railguns-0.89/railguns/static/railguns/js/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.921323 railguns-0.89/railguns/static/railguns/js/components/
+-rw-r--r--   0 ny         (501) staff       (20)    13372 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/railguns/js/components/weui-components.js
+-rw-r--r--   0 ny         (501) staff       (20)     1160 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/railguns/js/mixins.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.921532 railguns-0.89/railguns/static/railguns/js/util/
+-rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/railguns/js/util/http-utils.js
+-rw-r--r--   0 ny         (501) staff       (20)      346 2022-06-18 13:16:59.000000 railguns-0.89/railguns/static/railguns/js/vendor.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.915083 railguns-0.89/railguns/templates/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.921810 railguns-0.89/railguns/templates/railguns/
+-rw-r--r--   0 ny         (501) staff       (20)      583 2022-06-18 13:16:59.000000 railguns-0.89/railguns/templates/railguns/base.html
+-rw-r--r--   0 ny         (501) staff       (20)     1738 2022-06-18 13:16:59.000000 railguns-0.89/railguns/templates/railguns/base_quick.html
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.922219 railguns-0.89/railguns/templates/railguns/ui/
+-rw-r--r--   0 ny         (501) staff       (20)     1325 2022-06-18 13:16:59.000000 railguns-0.89/railguns/templates/railguns/ui/base.html
+-rw-r--r--   0 ny         (501) staff       (20)      740 2022-06-18 13:16:59.000000 railguns-0.89/railguns/templates/railguns/ui/detail.html
+-rw-r--r--   0 ny         (501) staff       (20)      775 2022-06-18 13:16:59.000000 railguns-0.89/railguns/templates/railguns/ui/list.html
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.922477 railguns-0.89/railguns/tools/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.89/railguns/tools/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      238 2024-03-03 23:42:05.000000 railguns-0.89/railguns/tools/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     1653 2024-03-03 23:42:05.000000 railguns-0.89/railguns/urls.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2024-04-14 20:16:18.922643 railguns-0.89/railguns.egg-info/
+-rw-r--r--   0 ny         (501) staff       (20)     3898 2024-04-14 20:16:18.000000 railguns-0.89/railguns.egg-info/PKG-INFO
+-rw-r--r--   0 ny         (501) staff       (20)     1778 2024-04-14 20:16:18.000000 railguns-0.89/railguns.egg-info/SOURCES.txt
+-rw-r--r--   0 ny         (501) staff       (20)        1 2024-04-14 20:16:18.000000 railguns-0.89/railguns.egg-info/dependency_links.txt
+-rw-r--r--   0 ny         (501) staff       (20)      255 2024-04-14 20:16:18.000000 railguns-0.89/railguns.egg-info/requires.txt
+-rw-r--r--   0 ny         (501) staff       (20)        9 2024-04-14 20:16:18.000000 railguns-0.89/railguns.egg-info/top_level.txt
+-rw-r--r--   0 ny         (501) staff       (20)       38 2024-04-14 20:16:18.923232 railguns-0.89/setup.cfg
```

### Comparing `railguns-0.88/LICENSE` & `railguns-0.89/LICENSE`

 * *Files identical despite different names*

### Comparing `railguns-0.88/PKG-INFO` & `railguns-0.89/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: railguns
-Version: 0.88
+Version: 0.89
 Summary: Only My Railgun
 Author-email: NY <nyssance@icloud.com>
 License: MIT License
         
         Copyright (c) 2018-present NY <nyssance@icloud.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,21 +37,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django[argon2]==5.0.3
+Requires-Dist: django[argon2]==5.0.4
 Requires-Dist: djangorestframework==3.15.1
 Requires-Dist: djangorestframework_simplejwt==5.3.1
 Requires-Dist: gunicorn==21.2.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: django-ckeditor==6.7.1
-Requires-Dist: django-filter==24.1
+Requires-Dist: django-filter==24.2
 Requires-Dist: django-htmlmin==0.11.0
 Requires-Dist: mysqlclient==2.2.4
 Requires-Dist: redis==5.0.3
 Provides-Extra: test
 Requires-Dist: pytest>8.0.0; extra == "test"
 Requires-Dist: pytest-cov[all]; extra == "test"
```

### Comparing `railguns-0.88/README.md` & `railguns-0.89/README.md`

 * *Files identical despite different names*

### Comparing `railguns-0.88/pyproject.toml` & `railguns-0.89/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "railguns"
-version = "0.88"
+version = "0.89"
 description = "Only My Railgun"
 readme = "README.md"
 authors = [
   {name = "NY", email = "nyssance@icloud.com"}
 ]
 license = {file = "LICENSE"}
 keywords = ["django", "railguns"]
@@ -20,22 +20,22 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.12",
   "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
-  "django[argon2]==5.0.3",
+  "django[argon2]==5.0.4",
   "djangorestframework==3.15.1",
   "djangorestframework_simplejwt==5.3.1",
   "gunicorn==21.2.0",
   "uvicorn==0.29.0",
   #
   "django-ckeditor==6.7.1",
-  "django-filter==24.1",
+  "django-filter==24.2",
   "django-htmlmin==0.11.0",
   "mysqlclient==2.2.4",
   "redis==5.0.3"
 ]
 
 [project.optional-dependencies]
 test = [
```

### Comparing `railguns-0.88/railguns/cloudfile/widgets.py` & `railguns-0.89/railguns/cloudfile/widgets.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/django/contrib/admin.py` & `railguns-0.89/railguns/django/contrib/admin.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/django/contrib/auth/backends.py` & `railguns-0.89/railguns/django/contrib/auth/backends.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/django/db/models.py` & `railguns-0.89/railguns/django/db/models.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/django/db/utils.py` & `railguns-0.89/railguns/django/db/utils.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/django/generics.py` & `railguns-0.89/railguns/django/generics.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/django/utils/translation.py` & `railguns-0.89/railguns/django/utils/translation.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/rest_framework/generics.py` & `railguns-0.89/railguns/rest_framework/generics.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/rest_framework/mixins.py` & `railguns-0.89/railguns/rest_framework/mixins.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/rest_framework/permissions.py` & `railguns-0.89/railguns/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/rest_framework/schemas/openapi.py` & `railguns-0.89/railguns/rest_framework/schemas/openapi.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/rest_framework/serializers.py` & `railguns-0.89/railguns/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/rest_framework/views.py` & `railguns-0.89/railguns/rest_framework/views.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/static/cloudfile/js/scripts.js` & `railguns-0.89/railguns/static/cloudfile/js/scripts.js`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/static/railguns/es2015/components/weui-components.js` & `railguns-0.89/railguns/static/railguns/es2015/components/weui-components.js`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/static/railguns/es2015/mixins.js` & `railguns-0.89/railguns/static/railguns/es2015/mixins.js`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/static/railguns/es2015/util/http-utils.js` & `railguns-0.89/railguns/static/railguns/es2015/util/http-utils.js`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/static/railguns/es2015/vendor.js` & `railguns-0.89/railguns/static/railguns/es2015/vendor.js`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/static/railguns/js/components/weui-components.js` & `railguns-0.89/railguns/static/railguns/js/components/weui-components.js`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/static/railguns/js/mixins.js` & `railguns-0.89/railguns/static/railguns/js/mixins.js`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/static/railguns/js/util/http-utils.js` & `railguns-0.89/railguns/static/railguns/js/util/http-utils.js`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/templates/railguns/base.html` & `railguns-0.89/railguns/templates/railguns/base.html`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/templates/railguns/base_quick.html` & `railguns-0.89/railguns/templates/railguns/base_quick.html`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/templates/railguns/ui/base.html` & `railguns-0.89/railguns/templates/railguns/ui/base.html`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/templates/railguns/ui/detail.html` & `railguns-0.89/railguns/templates/railguns/ui/detail.html`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/templates/railguns/ui/list.html` & `railguns-0.89/railguns/templates/railguns/ui/list.html`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns/urls.py` & `railguns-0.89/railguns/urls.py`

 * *Files identical despite different names*

### Comparing `railguns-0.88/railguns.egg-info/PKG-INFO` & `railguns-0.89/railguns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: railguns
-Version: 0.88
+Version: 0.89
 Summary: Only My Railgun
 Author-email: NY <nyssance@icloud.com>
 License: MIT License
         
         Copyright (c) 2018-present NY <nyssance@icloud.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,21 +37,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django[argon2]==5.0.3
+Requires-Dist: django[argon2]==5.0.4
 Requires-Dist: djangorestframework==3.15.1
 Requires-Dist: djangorestframework_simplejwt==5.3.1
 Requires-Dist: gunicorn==21.2.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: django-ckeditor==6.7.1
-Requires-Dist: django-filter==24.1
+Requires-Dist: django-filter==24.2
 Requires-Dist: django-htmlmin==0.11.0
 Requires-Dist: mysqlclient==2.2.4
 Requires-Dist: redis==5.0.3
 Provides-Extra: test
 Requires-Dist: pytest>8.0.0; extra == "test"
 Requires-Dist: pytest-cov[all]; extra == "test"
```

### Comparing `railguns-0.88/railguns.egg-info/SOURCES.txt` & `railguns-0.89/railguns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

