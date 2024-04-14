# Comparing `tmp/django-flasky-0.1.3.tar.gz` & `tmp/django_flasky-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-flasky-0.1.3.tar", last modified: Thu Oct 19 18:44:55 2023, max compression
+gzip compressed data, was "django_flasky-0.1.5.tar", last modified: Sun Apr 14 19:30:34 2024, max compression
```

## Comparing `django-flasky-0.1.3.tar` & `django_flasky-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:44:55.546524 django-flasky-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2023-10-19 18:44:55.546524 django-flasky-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2023-10-19 18:44:48.000000 django-flasky-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:44:55.546524 django-flasky-0.1.3/django_flasky/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/app_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:44:55.546524 django-flasky-0.1.3/django_flasky/django_glue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/django_glue/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/django_glue/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-10-19 18:44:48.000000 django-flasky-0.1.3/django_flasky/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:44:55.546524 django-flasky-0.1.3/django_flasky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2023-10-19 18:44:55.000000 django-flasky-0.1.3/django_flasky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-10-19 18:44:55.000000 django-flasky-0.1.3/django_flasky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 18:44:55.000000 django-flasky-0.1.3/django_flasky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-19 18:44:55.000000 django-flasky-0.1.3/django_flasky.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 18:44:55.000000 django-flasky-0.1.3/django_flasky.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-19 18:44:55.000000 django-flasky-0.1.3/django_flasky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-19 18:44:55.000000 django-flasky-0.1.3/django_flasky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-10-19 18:44:55.550524 django-flasky-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-10-19 18:44:48.000000 django-flasky-0.1.3/setup.py
+drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2024-04-14 19:30:34.370965 django_flasky-0.1.5/
+-rw-r--r--   0 radiac    (1000) radiac    (1000)      367 2024-04-14 19:30:34.370965 django_flasky-0.1.5/PKG-INFO
+-rw-rw-r--   0 radiac    (1000) radiac    (1000)      155 2024-04-14 19:28:18.000000 django_flasky-0.1.5/README.md
+drwxrwxr-x   0 radiac    (1000) radiac    (1000)        0 2024-04-14 19:30:34.370965 django_flasky-0.1.5/django_flasky.egg-info/
+-rw-r--r--   0 radiac    (1000) radiac    (1000)      367 2024-04-14 19:30:34.000000 django_flasky-0.1.5/django_flasky.egg-info/PKG-INFO
+-rw-rw-r--   0 radiac    (1000) radiac    (1000)      202 2024-04-14 19:30:34.000000 django_flasky-0.1.5/django_flasky.egg-info/SOURCES.txt
+-rw-rw-r--   0 radiac    (1000) radiac    (1000)        1 2024-04-14 19:30:34.000000 django_flasky-0.1.5/django_flasky.egg-info/dependency_links.txt
+-rw-rw-r--   0 radiac    (1000) radiac    (1000)       11 2024-04-14 19:30:34.000000 django_flasky-0.1.5/django_flasky.egg-info/requires.txt
+-rw-rw-r--   0 radiac    (1000) radiac    (1000)        1 2024-04-14 19:30:34.000000 django_flasky-0.1.5/django_flasky.egg-info/top_level.txt
+-rw-rw-r--   0 radiac    (1000) radiac    (1000)       38 2024-04-14 19:30:34.374965 django_flasky-0.1.5/setup.cfg
+-rw-rw-r--   0 radiac    (1000) radiac    (1000)      544 2024-04-14 19:29:33.000000 django_flasky-0.1.5/setup.py
```

