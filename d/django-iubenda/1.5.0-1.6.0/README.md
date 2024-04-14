# Comparing `tmp/django-iubenda-1.5.0.tar.gz` & `tmp/django_iubenda-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-1.5.0.tar", last modified: Tue Apr  9 20:17:10 2024, max compression
+gzip compressed data, was "django_iubenda-1.6.0.tar", last modified: Sun Apr 14 16:39:54 2024, max compression
```

## Comparing `django-iubenda-1.5.0.tar` & `django_iubenda-1.6.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.265572 django-iubenda-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-09 20:17:10.265572 django-iubenda-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.257573 django-iubenda-1.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py310-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py311-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py38-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py39-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-09 20:17:10.265572 django-iubenda-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.249572 django-iubenda-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/django_iubenda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.257573 django-iubenda-1.5.0/src/iubenda/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/fixtures/data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.249572 django-iubenda-1.5.0/src/iubenda/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.253573 django-iubenda-1.5.0/src/iubenda/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/sitemaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.253573 django-iubenda-1.5.0/src/iubenda/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.253573 django-iubenda-1.5.0/src/iubenda/static/iubenda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/static/iubenda/css/
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/static/iubenda/css/iubenda_badge.css
--rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/static/iubenda/css/iubenda_policy.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.253573 django-iubenda-1.5.0/src/iubenda/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/templates/iubenda/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/cookie-compress.html
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/cookie.html
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/include-content.html
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/privacy-compress.html
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/privacy.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/fixtures/data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_custom_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_default_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.875819 django_iubenda-1.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py310-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py311-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py38-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py39-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.867819 django_iubenda-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/src/django_iubenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 16:39:54.000000 django_iubenda-1.6.0/src/django_iubenda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/fixtures/data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.867819 django_iubenda-1.6.0/src/iubenda/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.867819 django_iubenda-1.6.0/src/iubenda/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/sitemaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.867819 django_iubenda-1.6.0/src/iubenda/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.871819 django_iubenda-1.6.0/src/iubenda/static/iubenda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/static/iubenda/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/static/iubenda/css/iubenda_badge.css
+-rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/static/iubenda/css/iubenda_policy.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.871819 django_iubenda-1.6.0/src/iubenda/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.879819 django_iubenda-1.6.0/src/iubenda/templates/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/cookie-compress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/cookie.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/include-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/privacy-compress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/templates/iubenda/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/src/iubenda/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/fixtures/data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:39:54.883819 django_iubenda-1.6.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_custom_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_default_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/test_iubenda_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-14 16:39:44.000000 django_iubenda-1.6.0/tox.ini
```

### Comparing `django-iubenda-1.5.0/.pre-commit-config.yaml` & `django_iubenda-1.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/LICENSE` & `django_iubenda-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/PKG-INFO` & `django_iubenda-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.5.0
+Version: 1.6.0
 Summary: Django''s application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,iubenda,privacy,cookie
 Classifier: Development Status :: 4 - Beta
@@ -141,22 +141,22 @@
 
 ## Optional
 
 ### Autoblocking
 If Iubenda autoblocking's configurations are implemented in your account,
 the variable `IUBENDA_AUTOBLOCKING` can be set to import the site's script.
 ```html
-<script type="text/javascript" src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
+<script src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
 ```
 
 ### Content Security Policy
 If Content Security Policy are implemented in your server and inline scripts are disabled,
 the variable `IUBENDA_CSP_NONCE` can be set with nonce tag will be inserted script's nonce.
 ```html
-<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
+<script {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
 ```
 Inside your webserver's configurations, a rule to dynamically replace your CONSTANT nonce in a random string is needed.
 
 To allow  external source from Iubenda domains, please implement these rules:
 ```editorconfig
 Content-Security-Policy:
     script-src-elem https://*.iubenda.com";
@@ -203,15 +203,15 @@
         "closeButtonRejects": "true",
         "customizeButtonDisplay": "true",
         "explicitWithdrawal": "true",
         "fontSize": "14px",
         "listPurposes": "true",
         "position": "float-center",
         "rejectButtonDisplay": "true",
-        "showPurposesToggles": "true"
+        "showPurposesToggles": "true",
     },
 }
 ```
 
 ### Integration with Google Tag Manager
 If Google Tag Manager is implemented in your application and all needed settings were configured inside the container,
 the variable `IUBENDA_GTM` can be set with the value `True` and the Iubenda's callback will be inserted inside the script.
```

### Comparing `django-iubenda-1.5.0/README.md` & `django_iubenda-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,22 +100,22 @@
 
 ## Optional
 
 ### Autoblocking
 If Iubenda autoblocking's configurations are implemented in your account,
 the variable `IUBENDA_AUTOBLOCKING` can be set to import the site's script.
 ```html
-<script type="text/javascript" src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
+<script src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
 ```
 
 ### Content Security Policy
 If Content Security Policy are implemented in your server and inline scripts are disabled,
 the variable `IUBENDA_CSP_NONCE` can be set with nonce tag will be inserted script's nonce.
 ```html
-<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
+<script {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
 ```
 Inside your webserver's configurations, a rule to dynamically replace your CONSTANT nonce in a random string is needed.
 
 To allow  external source from Iubenda domains, please implement these rules:
 ```editorconfig
 Content-Security-Policy:
     script-src-elem https://*.iubenda.com";
@@ -162,15 +162,15 @@
         "closeButtonRejects": "true",
         "customizeButtonDisplay": "true",
         "explicitWithdrawal": "true",
         "fontSize": "14px",
         "listPurposes": "true",
         "position": "float-center",
         "rejectButtonDisplay": "true",
-        "showPurposesToggles": "true"
+        "showPurposesToggles": "true",
     },
 }
 ```
 
 ### Integration with Google Tag Manager
 If Google Tag Manager is implemented in your application and all needed settings were configured inside the container,
 the variable `IUBENDA_GTM` can be set with the value `True` and the Iubenda's callback will be inserted inside the script.
```

#### html2text {}

```diff
@@ -73,15 +73,15 @@
 "ccpaApplies": "true", "consentOnContinuedBrowsing": "false",
 "floatingPreferencesButtonDisplay": "bottom-left",
 "invalidateConsentWithoutLog": "true", "perPurposeConsent": "true",
 "whitelabel": "false", "banner": { "acceptButtonDisplay": "true",
 "backgroundOverlay": "true", "closeButtonRejects": "true",
 "customizeButtonDisplay": "true", "explicitWithdrawal": "true", "fontSize":
 "14px", "listPurposes": "true", "position": "float-center",
-"rejectButtonDisplay": "true", "showPurposesToggles": "true" }, } ``` ###
+"rejectButtonDisplay": "true", "showPurposesToggles": "true", }, } ``` ###
 Integration with Google Tag Manager If Google Tag Manager is implemented in
 your application and all needed settings were configured inside the container,
 the variable `IUBENDA_GTM` can be set with the value `True` and the Iubenda's
 callback will be inserted inside the script. For needed configuration inside
 Google Tag Manager container, please refer to these notes: - [Google Consent
 Mode](https://www.iubenda.com/en/help/27137-google-consent-mode) - [Google
 Consent Mode setup GTM with Iubenda](https://www.iubenda.com/en/help/74198-
```

### Comparing `django-iubenda-1.5.0/mkdocs.yml` & `django_iubenda-1.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/pyproject.toml` & `django_iubenda-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   { name = "Vendored Libraries",        directory = "vendor",  showcontent = true },
   { name = "Improved Documentation",    directory = "doc",     showcontent = true },
   { name = "Trivial Changes",           directory = "trivial", showcontent = false },
 ]
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "1.5.0"
+current_version = "1.6.0"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
 
 [[tool.bumpversion.files]]
 filename = "./src/iubenda/__init__.py"
```

### Comparing `django-iubenda-1.5.0/requirements/docs.txt` & `django_iubenda-1.6.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/requirements/py310-dev.txt` & `django_iubenda-1.6.0/requirements/py310-dev.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/requirements/py310-django32.txt` & `django_iubenda-1.6.0/requirements/py39-django32.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 certifi==2024.2.2 \
     --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
@@ -119,17 +119,17 @@
     --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
     --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
     # via -r requirements/requirements.in
 django-modeltranslation==0.18.11 \
     --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
     --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
     # via -r requirements/requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 pytz==2024.1 \
     --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
     --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
 rcssmin==1.1.1 \
     --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
@@ -181,17 +181,17 @@
     --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
     --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
     --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
     --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
-sqlparse==0.4.4 \
-    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
-    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+sqlparse==0.5.0 \
+    --hash=sha256:714d0a4932c059d16189f58ef5411ec2287a4360f17cdd0edd2d09d4c5087c93 \
+    --hash=sha256:c204494cd97479d0e39f28c93d46c0b2d5959c7b9ab904762ea6c7af211c8663
     # via django
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
```

### Comparing `django-iubenda-1.5.0/requirements/py310-django42.txt` & `django_iubenda-1.6.0/requirements/py39-django42.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django42.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 certifi==2024.2.2 \
     --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
@@ -119,17 +119,17 @@
     --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
     --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
     # via -r requirements/requirements.in
 django-modeltranslation==0.18.11 \
     --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
     --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
     # via -r requirements/requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 rcssmin==1.1.1 \
     --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
     --hash=sha256:35da6a6999e9e2c5b0e691b42ed56cc479373e0ecab33ef5277dfecce625e44a \
     --hash=sha256:42576d95dfad53d77df2e68dfdec95b89b10fad320f241f1af3ca1438578254a \
     --hash=sha256:4f9400b4366d29f5f5446f58e78549afa8338e6a59740c73115e9f6ac413dc64 \
     --hash=sha256:705c9112d0ed54ea40aecf97e7fd29bdf0f1c46d278a32d8f957f31dde90778a \
@@ -177,17 +177,17 @@
     --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
     --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
     --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
     --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
-sqlparse==0.4.4 \
-    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
-    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+sqlparse==0.5.0 \
+    --hash=sha256:714d0a4932c059d16189f58ef5411ec2287a4360f17cdd0edd2d09d4c5087c93 \
+    --hash=sha256:c204494cd97479d0e39f28c93d46c0b2d5959c7b9ab904762ea6c7af211c8663
     # via django
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
```

### Comparing `django-iubenda-1.5.0/requirements/py311-dev.txt` & `django_iubenda-1.6.0/requirements/py311-dev.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/requirements/py311-django32.txt` & `django_iubenda-1.6.0/requirements/py38-django32.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 certifi==2024.2.2 \
     --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
@@ -119,17 +119,17 @@
     --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
     --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
     # via -r requirements/requirements.in
 django-modeltranslation==0.18.11 \
     --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
     --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
     # via -r requirements/requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 pytz==2024.1 \
     --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
     --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
 rcssmin==1.1.1 \
     --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
@@ -181,19 +181,21 @@
     --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
     --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
     --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
     --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
-sqlparse==0.4.4 \
-    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
-    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+sqlparse==0.5.0 \
+    --hash=sha256:714d0a4932c059d16189f58ef5411ec2287a4360f17cdd0edd2d09d4c5087c93 \
+    --hash=sha256:c204494cd97479d0e39f28c93d46c0b2d5959c7b9ab904762ea6c7af211c8663
     # via django
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
-    # via django-modeltranslation
+    # via
+    #   asgiref
+    #   django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.5.0/requirements/py311-django42.txt` & `django_iubenda-1.6.0/requirements/py311-django42.txt`

 * *Files 3% similar despite different names*

```diff
@@ -119,17 +119,17 @@
     --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
     --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
     # via -r requirements/requirements.in
 django-modeltranslation==0.18.11 \
     --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
     --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
     # via -r requirements/requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 rcssmin==1.1.1 \
     --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
     --hash=sha256:35da6a6999e9e2c5b0e691b42ed56cc479373e0ecab33ef5277dfecce625e44a \
     --hash=sha256:42576d95dfad53d77df2e68dfdec95b89b10fad320f241f1af3ca1438578254a \
     --hash=sha256:4f9400b4366d29f5f5446f58e78549afa8338e6a59740c73115e9f6ac413dc64 \
     --hash=sha256:705c9112d0ed54ea40aecf97e7fd29bdf0f1c46d278a32d8f957f31dde90778a \
@@ -177,17 +177,17 @@
     --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
     --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
     --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
     --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
-sqlparse==0.4.4 \
-    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
-    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+sqlparse==0.5.0 \
+    --hash=sha256:714d0a4932c059d16189f58ef5411ec2287a4360f17cdd0edd2d09d4c5087c93 \
+    --hash=sha256:c204494cd97479d0e39f28c93d46c0b2d5959c7b9ab904762ea6c7af211c8663
     # via django
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
```

### Comparing `django-iubenda-1.5.0/requirements/py38-dev.txt` & `django_iubenda-1.6.0/requirements/py38-dev.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/requirements/py38-django32.txt` & `django_iubenda-1.6.0/requirements/py310-django32.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py38-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django32.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 certifi==2024.2.2 \
     --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
@@ -119,17 +119,17 @@
     --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
     --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
     # via -r requirements/requirements.in
 django-modeltranslation==0.18.11 \
     --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
     --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
     # via -r requirements/requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 pytz==2024.1 \
     --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
     --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
 rcssmin==1.1.1 \
     --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
@@ -181,17 +181,17 @@
     --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
     --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
     --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
     --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
-sqlparse==0.4.4 \
-    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
-    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+sqlparse==0.5.0 \
+    --hash=sha256:714d0a4932c059d16189f58ef5411ec2287a4360f17cdd0edd2d09d4c5087c93 \
+    --hash=sha256:c204494cd97479d0e39f28c93d46c0b2d5959c7b9ab904762ea6c7af211c8663
     # via django
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
```

### Comparing `django-iubenda-1.5.0/requirements/py38-django42.txt` & `django_iubenda-1.6.0/requirements/py38-django42.txt`

 * *Files 2% similar despite different names*

```diff
@@ -137,17 +137,17 @@
     --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
     --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
     # via -r requirements/requirements.in
 django-modeltranslation==0.18.11 \
     --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
     --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
     # via -r requirements/requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 rcssmin==1.1.1 \
     --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
     --hash=sha256:35da6a6999e9e2c5b0e691b42ed56cc479373e0ecab33ef5277dfecce625e44a \
     --hash=sha256:42576d95dfad53d77df2e68dfdec95b89b10fad320f241f1af3ca1438578254a \
     --hash=sha256:4f9400b4366d29f5f5446f58e78549afa8338e6a59740c73115e9f6ac413dc64 \
     --hash=sha256:705c9112d0ed54ea40aecf97e7fd29bdf0f1c46d278a32d8f957f31dde90778a \
@@ -195,17 +195,17 @@
     --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
     --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
     --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
     --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
-sqlparse==0.4.4 \
-    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
-    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+sqlparse==0.5.0 \
+    --hash=sha256:714d0a4932c059d16189f58ef5411ec2287a4360f17cdd0edd2d09d4c5087c93 \
+    --hash=sha256:c204494cd97479d0e39f28c93d46c0b2d5959c7b9ab904762ea6c7af211c8663
     # via django
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
```

### Comparing `django-iubenda-1.5.0/requirements/py39-dev.txt` & `django_iubenda-1.6.0/requirements/py39-dev.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/requirements/py39-django32.txt` & `django_iubenda-1.6.0/requirements/py311-django32.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django32.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py311-django32.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 certifi==2024.2.2 \
     --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
@@ -119,17 +119,17 @@
     --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
     --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
     # via -r requirements/requirements.in
 django-modeltranslation==0.18.11 \
     --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
     --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
     # via -r requirements/requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 pytz==2024.1 \
     --hash=sha256:2a29735ea9c18baf14b448846bde5a48030ed267578472d8955cd0e7443a9812 \
     --hash=sha256:328171f4e3623139da4983451950b28e95ac706e13f3f2630a879749e7a8b319
     # via django
 rcssmin==1.1.1 \
     --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
@@ -181,21 +181,19 @@
     --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
     --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
     --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
     --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
-sqlparse==0.4.4 \
-    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
-    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+sqlparse==0.5.0 \
+    --hash=sha256:714d0a4932c059d16189f58ef5411ec2287a4360f17cdd0edd2d09d4c5087c93 \
+    --hash=sha256:c204494cd97479d0e39f28c93d46c0b2d5959c7b9ab904762ea6c7af211c8663
     # via django
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
-    # via
-    #   asgiref
-    #   django-modeltranslation
+    # via django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.5.0/requirements/py39-django42.txt` & `django_iubenda-1.6.0/requirements/py310-django42.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py39-django42.txt requirements/requirements.in
+#    pip-compile --allow-unsafe --generate-hashes --output-file=requirements/py310-django42.txt requirements/requirements.in
 #
 asgiref==3.8.1 \
     --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
     --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
     # via django
 certifi==2024.2.2 \
     --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
@@ -119,17 +119,17 @@
     --hash=sha256:1b0acc9cfba9f69bc38e7c41da9b0d70a20bc95587b643ffef9609cf46064f67 \
     --hash=sha256:6e2b0c0becb9607f5099c2546a824c5b84a6918a34bc37a8a622ffa250313596
     # via -r requirements/requirements.in
 django-modeltranslation==0.18.11 \
     --hash=sha256:81b68e4dc806a3b779ac88babe1cbd99d5318d374a43b3737a65fb0f4c1cffe8 \
     --hash=sha256:a6e2c459e3b31852287d030bc6e29fa28576db97455dccd399fe08ac8e9223b9
     # via -r requirements/requirements.in
-idna==3.6 \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 rcssmin==1.1.1 \
     --hash=sha256:271e3d2f8614a6d4637ed8fff3d90007f03e2a654cd9444f37d888797662ba72 \
     --hash=sha256:35da6a6999e9e2c5b0e691b42ed56cc479373e0ecab33ef5277dfecce625e44a \
     --hash=sha256:42576d95dfad53d77df2e68dfdec95b89b10fad320f241f1af3ca1438578254a \
     --hash=sha256:4f9400b4366d29f5f5446f58e78549afa8338e6a59740c73115e9f6ac413dc64 \
     --hash=sha256:705c9112d0ed54ea40aecf97e7fd29bdf0f1c46d278a32d8f957f31dde90778a \
@@ -177,17 +177,17 @@
     --hash=sha256:bd1faedc425006d9e86b23837d164f01d105b7a8b66b767a9766d0014773db2a \
     --hash=sha256:ca90630b84fe94bb07739c3e3793e87d30c6ee450dde08653121f0d9153c8d0d \
     --hash=sha256:d332e44a1b21ad63401cc7eebc81157e3d982d5fb503bb4faaea5028068d71e9 \
     --hash=sha256:eb770aaf637919b0011c4eb87b9ac6317079fb9800eb17c90dda05fc9de4ebc3 \
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
-sqlparse==0.4.4 \
-    --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
-    --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
+sqlparse==0.5.0 \
+    --hash=sha256:714d0a4932c059d16189f58ef5411ec2287a4360f17cdd0edd2d09d4c5087c93 \
+    --hash=sha256:c204494cd97479d0e39f28c93d46c0b2d5959c7b9ab904762ea6c7af211c8663
     # via django
 typing-extensions==4.11.0 \
     --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
     --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
```

### Comparing `django-iubenda-1.5.0/runtests.py` & `django_iubenda-1.6.0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/setup.cfg` & `django_iubenda-1.6.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-iubenda
-version = 1.5.0
+version = 1.6.0
 url = https://github.com/DLRSP/django-iubenda
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django''s application for handling privacy and cookie policies configured with Iubenda.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-iubenda-1.5.0/setup.py` & `django_iubenda-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/django_iubenda.egg-info/PKG-INFO` & `django_iubenda-1.6.0/src/django_iubenda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.5.0
+Version: 1.6.0
 Summary: Django''s application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,iubenda,privacy,cookie
 Classifier: Development Status :: 4 - Beta
@@ -141,22 +141,22 @@
 
 ## Optional
 
 ### Autoblocking
 If Iubenda autoblocking's configurations are implemented in your account,
 the variable `IUBENDA_AUTOBLOCKING` can be set to import the site's script.
 ```html
-<script type="text/javascript" src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
+<script src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
 ```
 
 ### Content Security Policy
 If Content Security Policy are implemented in your server and inline scripts are disabled,
 the variable `IUBENDA_CSP_NONCE` can be set with nonce tag will be inserted script's nonce.
 ```html
-<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
+<script {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
 ```
 Inside your webserver's configurations, a rule to dynamically replace your CONSTANT nonce in a random string is needed.
 
 To allow  external source from Iubenda domains, please implement these rules:
 ```editorconfig
 Content-Security-Policy:
     script-src-elem https://*.iubenda.com";
@@ -203,15 +203,15 @@
         "closeButtonRejects": "true",
         "customizeButtonDisplay": "true",
         "explicitWithdrawal": "true",
         "fontSize": "14px",
         "listPurposes": "true",
         "position": "float-center",
         "rejectButtonDisplay": "true",
-        "showPurposesToggles": "true"
+        "showPurposesToggles": "true",
     },
 }
 ```
 
 ### Integration with Google Tag Manager
 If Google Tag Manager is implemented in your application and all needed settings were configured inside the container,
 the variable `IUBENDA_GTM` can be set with the value `True` and the Iubenda's callback will be inserted inside the script.
```

### Comparing `django-iubenda-1.5.0/src/django_iubenda.egg-info/SOURCES.txt` & `django_iubenda-1.6.0/src/django_iubenda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/iubenda/context_processors.py` & `django_iubenda-1.6.0/src/iubenda/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/iubenda/locale/it/LC_MESSAGES/django.po` & `django_iubenda-1.6.0/src/iubenda/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/iubenda/migrations/0001_initial.py` & `django_iubenda-1.6.0/src/iubenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/iubenda/models.py` & `django_iubenda-1.6.0/src/iubenda/models.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/iubenda/static/iubenda/css/iubenda_badge.css` & `django_iubenda-1.6.0/src/iubenda/static/iubenda/css/iubenda_badge.css`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/iubenda/static/iubenda/css/iubenda_policy.css` & `django_iubenda-1.6.0/src/iubenda/static/iubenda/css/iubenda_policy.css`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/iubenda/templates/iubenda/cookie-compress.html` & `django_iubenda-1.6.0/src/iubenda/templates/iubenda/cookie.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'base.html' %}
-{% load i18n static compress %}
+{% load i18n static %}
 
 {% block head_canonical %}
     <link href="{{ SITE_URL }}{{ request.get_full_path }}" rel="canonical">
 {% endblock head_canonical %}
 
 {% block itemtype %}{% endblock itemtype %}
 
@@ -12,25 +12,23 @@
 {% block content %}
 <section id="cookie">
   <div class="wrapper light-wrapper">
     <div class="container inner">
       <div class="row">
         {% if req_cookie %}
           {% block css %}
-        	{% compress css file iubenda %}
             <link rel="stylesheet" type="text/css" href="{% static 'iubenda/css/iubenda_policy.css' %}">
-        	{% endcompress %}
           {% endblock css %}
 
           {{ req_cookie.content | safe }}
         {% else %}
           <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}/cookie-policy" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Cookie Policy">Cookie Policy</a>
 
           {% block js %}
-          <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
+          <script {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
           {% endblock js %}
         {% endif %}
       </div>
       <!-- /.row -->
     </div>
     <!-- /.container -->
   </div>
```

### Comparing `django-iubenda-1.5.0/src/iubenda/templates/iubenda/cookie.html` & `django_iubenda-1.6.0/src/iubenda/templates/iubenda/privacy.html`

 * *Files 11% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 
 {% block head_canonical %}
     <link href="{{ SITE_URL }}{{ request.get_full_path }}" rel="canonical">
 {% endblock head_canonical %}
 
 {% block itemtype %}{% endblock itemtype %}
 
-{% block extra_title %} - Cookie Policy{% endblock extra_title %}
+{% block extra_title %} - Privacy Policy{% endblock extra_title %}
 
 {% block content %}
-<section id="cookie">
+<section id="privacy">
   <div class="wrapper light-wrapper">
     <div class="container inner">
       <div class="row">
-        {% if req_cookie %}
+        {% if req_privacy %}
           {% block css %}
             <link rel="stylesheet" type="text/css" href="{% static 'iubenda/css/iubenda_policy.css' %}">
           {% endblock css %}
 
-          {{ req_cookie.content | safe }}
+          {{ req_privacy.content | safe }}
         {% else %}
-          <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}/cookie-policy" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Cookie Policy">Cookie Policy</a>
+          <!-- Could be added as class: "iub-legal-only" -->
+          <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Privacy Policy">Privacy Policy</a>
 
           {% block js %}
-          <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
+          <script {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
           {% endblock js %}
         {% endif %}
       </div>
       <!-- /.row -->
     </div>
     <!-- /.container -->
   </div>
   <!-- /.wrapper -->
 </section>
-<!-- /#cookie -->
+<!-- /#privacy -->
 {% endblock content %}
```

### Comparing `django-iubenda-1.5.0/src/iubenda/templates/iubenda/include-content.html` & `django_iubenda-1.6.0/src/iubenda/templates/iubenda/include-content.html`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     -
         <!--Cookie Policy-->
         <a href="{% url 'cookie' %}" class="iubenda-black no-brand iubenda-noiframe " title="Cookie Policy ">Cookie Policy</a>
     </i>
 </p>
 
 <!-- JS Cookie Solution -->
-<script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
+<script {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
     var _iub = _iub || [];
     _iub.csConfiguration = {
         "lang": "{{ LANGUAGE_CODE }}",
         "siteId": {{ cx_iubenda.iub_site_id }},
         "cookiePolicyId": {{ cx_iubenda.iub_policy_id }},
         "countryDetection": {{ cx_iubenda_options.countryDetection|default:'true' }},
         "askConsentAtCookiePolicyUpdate": {{ cx_iubenda_options.askConsentAtCookiePolicyUpdate|default:'true' }},
@@ -73,11 +73,11 @@
             }
         }{% endif %}
     };
 </script>
 
 <!-- JS Iubenda -->
 {% if cx_iubenda_autoblocking %}
-<script type="text/javascript" src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
+<script src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
 {% endif %}
-<script type="text/javascript" src="https://cdn.iubenda.com/cs/ccpa/stub.js"></script>
-<script type="text/javascript" src="https://cdn.iubenda.com/cs/iubenda_cs.js" charset="UTF-8" async></script>
+<script src="https://cdn.iubenda.com/cs/ccpa/stub.js"></script>
+<script src="https://cdn.iubenda.com/cs/iubenda_cs.js" charset="UTF-8" async></script>
```

### Comparing `django-iubenda-1.5.0/src/iubenda/templates/iubenda/privacy-compress.html` & `django_iubenda-1.6.0/src/iubenda/templates/iubenda/privacy-compress.html`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
           {{ req_privacy.content | safe }}
         {% else %}
           <!-- Could be added as class: "iub-legal-only" -->
           <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Privacy Policy">Privacy Policy</a>
 
           {% block js %}
-          <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
+          <script {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
           {% endblock js %}
         {% endif %}
       </div>
       <!-- /.row -->
     </div>
     <!-- /.container -->
   </div>
```

### Comparing `django-iubenda-1.5.0/src/iubenda/templates/iubenda/privacy.html` & `django_iubenda-1.6.0/src/iubenda/templates/iubenda/cookie-compress.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 {% extends 'base.html' %}
-{% load i18n static %}
+{% load i18n static compress %}
 
 {% block head_canonical %}
     <link href="{{ SITE_URL }}{{ request.get_full_path }}" rel="canonical">
 {% endblock head_canonical %}
 
 {% block itemtype %}{% endblock itemtype %}
 
-{% block extra_title %} - Privacy Policy{% endblock extra_title %}
+{% block extra_title %} - Cookie Policy{% endblock extra_title %}
 
 {% block content %}
-<section id="privacy">
+<section id="cookie">
   <div class="wrapper light-wrapper">
     <div class="container inner">
       <div class="row">
-        {% if req_privacy %}
+        {% if req_cookie %}
           {% block css %}
+        	{% compress css file iubenda %}
             <link rel="stylesheet" type="text/css" href="{% static 'iubenda/css/iubenda_policy.css' %}">
+        	{% endcompress %}
           {% endblock css %}
 
-          {{ req_privacy.content | safe }}
+          {{ req_cookie.content | safe }}
         {% else %}
-          <!-- Could be added as class: "iub-legal-only" -->
-          <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Privacy Policy">Privacy Policy</a>
+          <a href="https://www.iubenda.com/privacy-policy/{{ cx_iubenda.iub_policy_id }}/cookie-policy" class="iubenda-black no-brand iubenda-noiframe iubenda-embed iubenda-noiframe iub-body-embed" title="Cookie Policy">Cookie Policy</a>
 
           {% block js %}
-          <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
+          <script {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>(function (w,d) {var loader = function () {var s = d.createElement("script"), tag = d.getElementsByTagName("script")[0]; s.src="https://cdn.iubenda.com/iubenda.js"; tag.parentNode.insertBefore(s,tag);}; if(w.addEventListener){w.addEventListener("load", loader, false);}else if(w.attachEvent){w.attachEvent("onload", loader);}else{w.onload = loader;}})(window, document);</script>
           {% endblock js %}
         {% endif %}
       </div>
       <!-- /.row -->
     </div>
     <!-- /.container -->
   </div>
   <!-- /.wrapper -->
 </section>
-<!-- /#privacy -->
+<!-- /#cookie -->
 {% endblock content %}
```

### Comparing `django-iubenda-1.5.0/src/iubenda/urls.py` & `django_iubenda-1.6.0/src/iubenda/urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/src/iubenda/views.py` & `django_iubenda-1.6.0/src/iubenda/views.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/tests/settings.py` & `django_iubenda-1.6.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/tests/test_iubenda_custom_options.py` & `django_iubenda-1.6.0/tests/test_iubenda_custom_options.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/tests/test_iubenda_default_options.py` & `django_iubenda-1.6.0/tests/test_iubenda_default_options.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/tests/test_iubenda_settings.py` & `django_iubenda-1.6.0/tests/test_iubenda_settings.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/tests/test_iubenda_template.py` & `django_iubenda-1.6.0/tests/test_iubenda_template.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/tests/test_iubenda_urls.py` & `django_iubenda-1.6.0/tests/test_iubenda_urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/tests/urls.py` & `django_iubenda-1.6.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.5.0/tox.ini` & `django_iubenda-1.6.0/tox.ini`

 * *Files identical despite different names*

