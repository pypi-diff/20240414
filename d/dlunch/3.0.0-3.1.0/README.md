# Comparing `tmp/dlunch-3.0.0.tar.gz` & `tmp/dlunch-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlunch-3.0.0.tar", last modified: Sun Mar 17 16:04:12 2024, max compression
+gzip compressed data, was "dlunch-3.1.0.tar", last modified: Sun Apr 14 13:36:57 2024, max compression
```

## Comparing `dlunch-3.0.0.tar` & `dlunch-3.1.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.075867 dlunch-3.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)    20268 2024-03-17 16:04:04.000000 dlunch-3.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-17 16:04:04.000000 dlunch-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-03-17 16:04:12.075867 dlunch-3.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    13318 2024-03-17 16:04:04.000000 dlunch-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.063867 dlunch-3.0.0/dlunch/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5265 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4645 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18436 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/auth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9333 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.063867 dlunch-3.0.0/dlunch/conf/
--rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.067867 dlunch-3.0.0/dlunch/conf/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/auth/default.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/auth/development.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/auth/production.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.067867 dlunch-3.0.0/dlunch/conf/basic_auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/basic_auth/basic_auth.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.067867 dlunch-3.0.0/dlunch/conf/db/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/db/common.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      216 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/db/development.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/db/postgresql.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/db/production.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/db/sqlite.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.059867 dlunch-3.0.0/dlunch/conf/hydra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.067867 dlunch-3.0.0/dlunch/conf/hydra/job_logging/
--rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/hydra/job_logging/custom.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.067867 dlunch-3.0.0/dlunch/conf/panel/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3118 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.067867 dlunch-3.0.0/dlunch/conf/panel/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/gui/1st_of_april.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/gui/4th_of_may.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/gui/backup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/gui/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/gui/easter.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/gui/major_release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/gui/women_day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/no_sched_clean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/panel/quality.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.071867 dlunch-3.0.0/dlunch/conf/server/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/server/azure_oauth.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/server/basic_auth.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/server/common.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/server/development.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/server/github_oauth.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/server/no_oauth.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/conf/server/production.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    44618 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    46139 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13534 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/quotes.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/scheduled_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.059867 dlunch-3.0.0/dlunch/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.071867 dlunch-3.0.0/dlunch/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/css/app_header.css
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/css/custom_tabulator.css
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/css/guest_override.css
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/css/labels.css
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/css/no_more_orders.css
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/css/stats_and_info.css
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/css/stats_tabulator.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.071867 dlunch-3.0.0/dlunch/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    15538 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)  2189685 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/static/images/no_menu.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.075867 dlunch-3.0.0/dlunch/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/templates/login_basic.html
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/templates/login_oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-17 16:04:04.000000 dlunch-3.0.0/dlunch/templates/logout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.075867 dlunch-3.0.0/dlunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-03-17 16:04:12.000000 dlunch-3.0.0/dlunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-17 16:04:12.000000 dlunch-3.0.0/dlunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 16:04:12.000000 dlunch-3.0.0/dlunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-17 16:04:12.000000 dlunch-3.0.0/dlunch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-17 16:04:12.000000 dlunch-3.0.0/dlunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-17 16:04:12.000000 dlunch-3.0.0/dlunch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1458 2024-03-17 16:04:04.000000 dlunch-3.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:04:12.075867 dlunch-3.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-17 16:04:04.000000 dlunch-3.0.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 16:04:12.075867 dlunch-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.092725 dlunch-3.1.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20268 2024-04-14 13:36:48.000000 dlunch-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-14 13:36:48.000000 dlunch-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-14 13:36:57.092725 dlunch-3.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13318 2024-04-14 13:36:48.000000 dlunch-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.080725 dlunch-3.1.0/dlunch/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5224 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4645 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18436 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/auth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9333 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.080725 dlunch-3.1.0/dlunch/conf/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.080725 dlunch-3.1.0/dlunch/conf/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/auth/default.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/auth/development.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/auth/production.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.080725 dlunch-3.1.0/dlunch/conf/basic_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/basic_auth/basic_auth.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      633 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.084725 dlunch-3.1.0/dlunch/conf/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/db/common.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      216 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/db/development.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/db/postgresql.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/db/production.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/db/sqlite.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.076725 dlunch-3.1.0/dlunch/conf/hydra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.084725 dlunch-3.1.0/dlunch/conf/hydra/job_logging/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/hydra/job_logging/custom.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.084725 dlunch-3.1.0/dlunch/conf/panel/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3118 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.084725 dlunch-3.1.0/dlunch/conf/panel/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/gui/1st_of_april.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/gui/4th_of_may.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/gui/backup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/gui/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/gui/easter.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/gui/major_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/gui/women_day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/no_sched_clean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/panel/quality.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.084725 dlunch-3.1.0/dlunch/conf/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/server/azure_oauth.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/server/basic_auth.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/server/common.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/server/development.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/server/github_oauth.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/server/no_oauth.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/conf/server/production.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    48294 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46636 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22059 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13534 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/quotes.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/scheduled_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.076725 dlunch-3.1.0/dlunch/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.088725 dlunch-3.1.0/dlunch/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/css/app_header.css
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/css/custom_tabulator.css
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/css/guest_override.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/css/labels.css
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/css/no_more_orders.css
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/css/stats_and_info.css
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/css/stats_tabulator.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.088725 dlunch-3.1.0/dlunch/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    15538 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)  2189685 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/static/images/no_menu.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.092725 dlunch-3.1.0/dlunch/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/templates/login_basic.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/templates/login_oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-14 13:36:48.000000 dlunch-3.1.0/dlunch/templates/logout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.092725 dlunch-3.1.0/dlunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-04-14 13:36:57.000000 dlunch-3.1.0/dlunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-14 13:36:57.000000 dlunch-3.1.0/dlunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:36:57.000000 dlunch-3.1.0/dlunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 13:36:57.000000 dlunch-3.1.0/dlunch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-14 13:36:57.000000 dlunch-3.1.0/dlunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 13:36:57.000000 dlunch-3.1.0/dlunch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1458 2024-04-14 13:36:48.000000 dlunch-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:36:57.092725 dlunch-3.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-14 13:36:48.000000 dlunch-3.1.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:36:57.092725 dlunch-3.1.0/setup.cfg
```

### Comparing `dlunch-3.0.0/LICENSE.md` & `dlunch-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/PKG-INFO` & `dlunch-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: dlunch
-Version: 3.0.0
+Version: 3.1.0
 Summary: The ultimate web app for a well organized lunch.
 Author-email: Michele Alberti <michele.alberti90@gmail.com>
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
 Project-URL: Homepage, https://github.com/Michele-Alberti/data-lunch
 Project-URL: Issues, https://github.com/Michele-Alberti/data-lunch/issues
 Keywords: python,webapp,lunch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: setuptools==69.1.1
+Requires-Dist: setuptools==69.2.0
 Requires-Dist: click==8.1.7
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: ipykernel==6.29.3
 Requires-Dist: ipywidgets==8.1.2
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.2.1
 Requires-Dist: passlib==1.7.4
 Requires-Dist: tenacity==8.2.3
 Requires-Dist: tqdm==4.66.2
-Requires-Dist: panel==1.3.8
-Requires-Dist: sqlalchemy==2.0.28
+Requires-Dist: panel==1.4.0
+Requires-Dist: sqlalchemy==2.0.29
 Requires-Dist: psycopg==3.1.18
 Requires-Dist: hydra-core==1.3.2
-Requires-Dist: google-cloud-storage==2.14.0
+Requires-Dist: google-cloud-storage==2.16.0
 Requires-Dist: pytesseract==0.3.10
 
 # Data Lunch <!-- omit in toc -->
 
 The ultimate web app for a well organized lunch.
 
 ## 1. Table of contents
```

### Comparing `dlunch-3.0.0/README.md` & `dlunch-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/__init__.py` & `dlunch-3.1.0/dlunch/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # App metadata
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 
 import importlib.resources
 import pathlib
 import hydra
 import logging
 import panel as pn
 from omegaconf import DictConfig, OmegaConf
@@ -98,15 +98,14 @@
     app.main.append(gi.quote)
     app.main.append(pn.Spacer(height=15))
     app.main.append(gi.menu_flexbox)
     app.main.append(gi.buttons_flexbox)
     app.main.append(gi.results_divider)
     app.main.append(gi.res_col)
     app.modal.append(gi.error_message)
-    app.modal.append(gi.confirm_message)
 
     # Set components visibility based on no_more_order_button state
     # and reload menu
     gi.reload_on_no_more_order(
         toggle=models.get_flag(config=config, id="no_more_orders"),
         reload=False,
     )
```

### Comparing `dlunch-3.0.0/dlunch/__main__.py` & `dlunch-3.1.0/dlunch/__main__.py`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/auth.py` & `dlunch-3.1.0/dlunch/auth.py`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/cli.py` & `dlunch-3.1.0/dlunch/cli.py`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/cloud.py` & `dlunch-3.1.0/dlunch/cloud.py`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/auth/default.yaml` & `dlunch-3.1.0/dlunch/conf/auth/default.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/basic_auth/basic_auth.yaml` & `dlunch-3.1.0/dlunch/conf/basic_auth/basic_auth.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/config.yaml` & `dlunch-3.1.0/dlunch/conf/config.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/db/common.yaml` & `dlunch-3.1.0/dlunch/conf/db/common.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/db/postgresql.yaml` & `dlunch-3.1.0/dlunch/conf/db/postgresql.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 database: ${oc.env:DATA_LUNCH_DB_DATABASE, data_lunch_database}
 schema: ${oc.env:DATA_LUNCH_DB_SCHEMA, webapp}
 url: ${db.dialect}+${db.driver}://${db.username}:${db.password}@${db.host}:${db.port}/${db.database}
 
 # QUERIES
 # Orders
 orders_query: |-
-  SELECT o.user, o.lunch_time, m.item, o.note
+  SELECT o.user, u.lunch_time, m.item, o.note
   FROM {schema}.orders o
   LEFT JOIN {schema}.menu m
-  ON m.id = o.menu_item_id;
+  ON m.id = o.menu_item_id
+  LEFT JOIN {schema}.users u
+  ON u.id = o.user;
 # Stats
 stats_query: |-
   SELECT EXTRACT(YEAR FROM date)::varchar(4) AS "Year", 
     EXTRACT(MONTH FROM date)::varchar(2) AS "Month",
     guest AS "Guest",
     SUM(hungry_people) AS "Hungry People"
   FROM {schema}.stats
```

### Comparing `dlunch-3.0.0/dlunch/conf/db/sqlite.yaml` & `dlunch-3.1.0/dlunch/conf/db/sqlite.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 name: lunch
 db_path: ${db.shared_data_folder}/${db.name}.db
 url: ${db.dialect}:///${db.db_path}
 
 # QUERIES
 # Orders
 orders_query: |-
-  SELECT o.user, o.lunch_time, m.item, o.note
+  SELECT o.user, u.lunch_time, m.item, o.note
   FROM orders o
   LEFT JOIN menu m
-  ON m.id = o.menu_item_id;
+  ON m.id = o.menu_item_id
+  LEFT JOIN users u
+  ON u.id = o.user;
 # Stats
 stats_query: |-
   SELECT STRFTIME('%Y', date) AS "Year", 
     STRFTIME('%m', date) AS "Month",
     guest AS "Guest",
     SUM(hungry_people) AS "Hungry People"
   FROM stats
```

### Comparing `dlunch-3.0.0/dlunch/conf/panel/default.yaml` & `dlunch-3.1.0/dlunch/conf/panel/default.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/gui/1st_of_april.yaml` & `dlunch-3.1.0/dlunch/conf/panel/gui/1st_of_april.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/gui/4th_of_may.yaml` & `dlunch-3.1.0/dlunch/conf/panel/gui/4th_of_may.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/gui/backup.yaml` & `dlunch-3.1.0/dlunch/conf/panel/gui/backup.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/gui/default.yaml` & `dlunch-3.1.0/dlunch/conf/panel/gui/default.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/gui/easter.yaml` & `dlunch-3.1.0/dlunch/conf/panel/gui/easter.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/gui/major_release.yaml` & `dlunch-3.1.0/dlunch/conf/panel/gui/major_release.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/gui/women_day.yaml` & `dlunch-3.1.0/dlunch/conf/panel/gui/women_day.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/no_sched_clean.yaml` & `dlunch-3.1.0/dlunch/conf/panel/no_sched_clean.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/panel/quality.yaml` & `dlunch-3.1.0/dlunch/conf/panel/quality.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/conf/server/common.yaml` & `dlunch-3.1.0/dlunch/conf/server/common.yaml`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/core.py` & `dlunch-3.1.0/dlunch/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from openpyxl.styles import Alignment, Font
 from bokeh.models.widgets.tables import CheckboxEditor
 from io import BytesIO
 from PIL import Image
 from pytesseract import pytesseract
 import random
 import re
-from sqlalchemy import func, select, delete
+from sqlalchemy import func, select, delete, update
 from sqlalchemy.sql.expression import true as sql_true
 from time import sleep
 
 # Graphic interface imports (after class definition)
 from . import gui
 
 # Authentication
@@ -162,15 +162,14 @@
     event,
     config: DictConfig,
     app: pn.Template,
     gi: gui.GraphicInterface,
 ) -> pd.DataFrame:
     # Hide messages
     gi.error_message.visible = False
-    gi.confirm_message.visible = False
 
     # Build image path
     menu_filename = str(
         pathlib.Path(config.db.shared_data_folder) / config.panel.file_name
     )
 
     # Delete menu file if exist (every extension)
@@ -312,25 +311,32 @@
         # Check guest override button status (if not in table use False)
         gi.toggle_guest_override_button.value = models.get_flag(
             config=config,
             id=f"{pn_user(config)}_guest_override",
             value_if_missing=False,
         )
 
-        # Set no more orders toggle button visibility and activation
+        # Set no more orders toggle button and the change order time button
+        # visibility and activation
         if auth.is_guest(
             user=pn_user(config), config=config, allow_override=False
         ):
-            # Deactivate the no_more_orders button for guest users
+            # Deactivate the no_more_orders_button for guest users
             gi.toggle_no_more_order_button.disabled = True
             gi.toggle_no_more_order_button.visible = False
+            # Deactivate the change_order_time_button for guest users
+            gi.change_order_time_takeaway_button.disabled = True
+            gi.change_order_time_takeaway_button.visible = False
         else:
-            # Activate the no_more_orders button for privileged users
+            # Activate the no_more_orders_button for privileged users
             gi.toggle_no_more_order_button.disabled = False
             gi.toggle_no_more_order_button.visible = True
+            # Show the change_order_time_button for privileged users
+            # It is disabled by the no more order button if necessary
+            gi.change_order_time_takeaway_button.visible = True
 
         # Guest graphic configuration
         if auth.is_guest(user=pn_user(config), config=config):
             # If guest show guest type selection group
             gi.person_widget.widgets["guest"].disabled = False
             gi.person_widget.widgets["guest"].visible = True
         else:
@@ -582,15 +588,14 @@
     gi: gui.GraphicInterface,
 ) -> None:
     # Get username updated at each key press
     username_key_press = gi.person_widget._widgets["username"].value_input
 
     # Hide messages
     gi.error_message.visible = False
-    gi.confirm_message.visible = False
 
     # Create session
     session = models.create_session(config)
 
     with session:
         # Check if the "no more order" toggle button is pressed
         if models.get_flag(config=config, id="no_more_orders"):
@@ -673,29 +678,30 @@
                 try:
                     # Add User
                     # Do not pass guest for privileged users (default to NotAGuest)
                     if auth.is_guest(user=pn_user(config), config=config):
                         new_user = models.Users(
                             id=username_key_press,
                             guest=person.guest,
+                            lunch_time=person.lunch_time,
                             takeaway=person.takeaway,
                         )
                     else:
                         new_user = models.Users(
                             id=username_key_press,
+                            lunch_time=person.lunch_time,
                             takeaway=person.takeaway,
                         )
                     session.add(new_user)
                     session.commit()
                     # Add orders as long table (one row for each item selected by a user)
                     for row in df_order.itertuples(name="OrderTuple"):
                         # Order
                         new_order = models.Orders(
                             user=username_key_press,
-                            lunch_time=person.lunch_time,
                             menu_item_id=row.Index,
                             note=getattr(
                                 row, config.panel.gui.note_column_name
                             ).lower(),
                         )
                         session.add(new_order)
                         session.commit()
@@ -718,15 +724,15 @@
                         "Database error",
                         duration=config.panel.notifications.duration,
                     )
                     gi.error_message.object = (
                         f"DATABASE ERROR<br><br>ERROR:<br>{str(e)}"
                     )
                     gi.error_message.visible = True
-                    log.warning("database error")
+                    log.error("database error")
                     # Open modal window
                     app.open_modal()
         else:
             if not username_key_press:
                 pn.state.notifications.warning(
                     "Please insert user name",
                     duration=config.panel.notifications.duration,
@@ -740,23 +746,21 @@
                 log.warning("no selection made")
 
 
 def delete_order(
     event,
     config: DictConfig,
     app: pn.Template,
-    person: gui.Person,
     gi: gui.GraphicInterface,
 ) -> None:
     # Get username, updated on every keypress
     username_key_press = gi.person_widget._widgets["username"].value_input
 
     # Hide messages
     gi.error_message.visible = False
-    gi.confirm_message.visible = False
 
     # Create session
     session = models.create_session(config)
 
     with session:
         # Check if the "no more order" toggle button is pressed
         if models.get_flag(config=config, id="no_more_orders"):
@@ -793,41 +797,134 @@
                     config,
                     gi,
                 )
 
                 return
 
             # Delete user
-            num_rows_deleted_users = session.execute(
-                delete(models.Users).where(
-                    models.Users.id == username_key_press
+            try:
+                num_rows_deleted_users = session.execute(
+                    delete(models.Users).where(
+                        models.Users.id == username_key_press
+                    )
                 )
-            )
-            # Delete also orders (hotfix for Debian)
-            num_rows_deleted_orders = session.execute(
-                delete(models.Orders).where(
-                    models.Orders.user == username_key_press
+                # Delete also orders (hotfix for Debian)
+                num_rows_deleted_orders = session.execute(
+                    delete(models.Orders).where(
+                        models.Orders.user == username_key_press
+                    )
                 )
+                session.commit()
+                if (num_rows_deleted_users.rowcount > 0) or (
+                    num_rows_deleted_orders.rowcount > 0
+                ):
+                    # Update dataframe widget
+                    reload_menu(
+                        None,
+                        config,
+                        gi,
+                    )
+
+                    pn.state.notifications.success(
+                        "Order canceled",
+                        duration=config.panel.notifications.duration,
+                    )
+                    log.info(f"{username_key_press}'s order canceled")
+                else:
+                    pn.state.notifications.warning(
+                        f'No order for user named<br>"{username_key_press}"',
+                        duration=config.panel.notifications.duration,
+                    )
+                    log.info(f"no order for user named {username_key_press}")
+            except Exception as e:
+                # Any exception here is a database fault
+                pn.state.notifications.error(
+                    "Database error",
+                    duration=config.panel.notifications.duration,
+                )
+                gi.error_message.object = (
+                    f"DATABASE ERROR<br><br>ERROR:<br>{str(e)}"
+                )
+                gi.error_message.visible = True
+                log.error("database error")
+                # Open modal window
+                app.open_modal()
+        else:
+            pn.state.notifications.warning(
+                "Please insert user name",
+                duration=config.panel.notifications.duration,
+            )
+            log.warning("missing username")
+
+
+def change_order_time_takeaway(
+    event,
+    config: DictConfig,
+    person: gui.Person,
+    gi: gui.GraphicInterface,
+) -> None:
+    # Get username, updated on every keypress
+    username_key_press = gi.person_widget._widgets["username"].value_input
+
+    # Create session
+    session = models.create_session(config)
+
+    with session:
+        # Check if the "no more order" toggle button is pressed
+        if models.get_flag(config=config, id="no_more_orders"):
+            pn.state.notifications.error(
+                "It is not possible to update orders (time)",
+                duration=config.panel.notifications.duration,
             )
+
+            # Reload the menu
+            reload_menu(
+                None,
+                config,
+                gi,
+            )
+
+            return
+
+        if username_key_press:
+            # Build and execute the update statement
+            update_statement = (
+                update(models.Users)
+                .where(models.Users.id == username_key_press)
+                .values(lunch_time=person.lunch_time, takeaway=person.takeaway)
+                .returning(models.Users)
+            )
+
+            updated_user = session.scalars(update_statement).one_or_none()
+
             session.commit()
-            if (num_rows_deleted_users.rowcount > 0) or (
-                num_rows_deleted_orders.rowcount > 0
-            ):
+
+            if updated_user:
+                # Find updated values
+                updated_time = updated_user.lunch_time
+                updated_takeaway = (
+                    (" " + config.panel.gui.takeaway_id)
+                    if updated_user.takeaway
+                    else ""
+                )
+                updated_items_names = [
+                    order.menu_item.item for order in updated_user.orders
+                ]
                 # Update dataframe widget
                 reload_menu(
                     None,
                     config,
                     gi,
                 )
 
                 pn.state.notifications.success(
-                    "Order canceled",
+                    f"{username_key_press}'s<br>lunch time changed to<br>{updated_time}{updated_takeaway}<br>({', '.join(updated_items_names)})",
                     duration=config.panel.notifications.duration,
                 )
-                log.info(f"{username_key_press}'s order canceled")
+                log.info(f"{username_key_press}'s order updated")
             else:
                 pn.state.notifications.warning(
                     f'No order for user named<br>"{username_key_press}"',
                     duration=config.panel.notifications.duration,
                 )
                 log.info(f"no order for user named {username_key_press}")
         else:
@@ -948,20 +1045,16 @@
             )
 
     return df_dict
 
 
 def download_dataframe(
     config: DictConfig,
-    app: pn.Template,
     gi: gui.GraphicInterface,
 ) -> None:
-    # Hide messages
-    gi.error_message.visible = False
-    gi.confirm_message.visible = False
 
     # Build a dict of dataframes, one for each lunch time (the key contains
     # a lunch time)
     df_dict = df_list_by_lunch_time(config)
     # Export one dataframe for each lunch time
     bytes_io = BytesIO()
     writer = pd.ExcelWriter(bytes_io)
```

### Comparing `dlunch-3.0.0/dlunch/gui.py` & `dlunch-3.1.0/dlunch/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -379,15 +379,25 @@
         # Create toggle button that stop orders (used in time column)
         # Initialized to False, but checked on app creation
         self.toggle_no_more_order_button = pnw.Toggle(
             name="Stop Orders",
             button_style="outline",
             button_type="warning",
             height=generic_button_height,
-            icon="alarm",
+            icon="hand-stop",
+            icon_size="2em",
+            sizing_mode="stretch_width",
+        )
+        # Create change time
+        self.change_order_time_takeaway_button = pnw.Button(
+            name="Change Time/Takeaway",
+            button_type="primary",
+            button_style="outline",
+            height=generic_button_height,
+            icon="clock-edit",
             icon_size="2em",
             sizing_mode="stretch_width",
         )
         # Create delete order
         self.delete_order_button = pnw.Button(
             name="Delete Order",
             button_type="danger",
@@ -428,14 +438,15 @@
             ],
             min_width=main_area_min_width,
         )
         self.buttons_flexbox = pn.FlexBox(
             *[
                 self.send_order_button,
                 self.toggle_no_more_order_button,
+                self.change_order_time_takeaway_button,
                 self.delete_order_button,
             ],
             flex_wrap="nowrap",
             min_width=main_area_min_width,
             sizing_mode="stretch_width",
         )
         self.results_divider = pn.layout.Divider(
@@ -450,17 +461,18 @@
         ):
             # Update global variable
             models.set_flag(config=config, id="no_more_orders", value=toggle)
 
             # Show "no more order" text
             self.no_more_order_alert.visible = toggle
 
-            # Deactivate send order and delete order buttons
+            # Deactivate send, delete and change order buttons
             self.send_order_button.disabled = toggle
             self.delete_order_button.disabled = toggle
+            self.change_order_time_takeaway_button.disabled = toggle
 
             # Simply reload the menu when the toggle button value changes
             if reload:
                 core.reload_menu(
                     None,
                     config,
                     self,
@@ -489,32 +501,34 @@
         )
         # Delete order button callback
         self.delete_order_button.on_click(
             lambda e: core.delete_order(
                 e,
                 config,
                 app,
+                self,
+            )
+        )
+        # Change order time button callback
+        self.change_order_time_takeaway_button.on_click(
+            lambda e: core.change_order_time_takeaway(
+                e,
+                config,
                 person,
                 self,
             )
         )
 
         # MODAL WINDOW --------------------------------------------------------
         # Error message
         self.error_message = pn.pane.HTML(
             styles={"color": "red", "font-weight": "bold"},
             sizing_mode="stretch_width",
         )
         self.error_message.visible = False
-        # Confirm message
-        self.confirm_message = pn.pane.HTML(
-            styles={"color": "green", "font-weight": "bold"},
-            sizing_mode="stretch_width",
-        )
-        self.confirm_message.visible = False
 
         # SIDEBAR -------------------------------------------------------------
         # TEXTS
         # Foldable additional item details dropdown menu
         jinja_template = jinja2.Environment(
             loader=jinja2.BaseLoader
         ).from_string(config.panel.gui.additional_item_details_template)
@@ -606,15 +620,15 @@
             button_type="primary",
             sizing_mode="stretch_width",
             icon="tools-kitchen-2",
             icon_size="2em",
         )
         # Download button and callback
         self.download_button = pn.widgets.FileDownload(
-            callback=lambda: core.download_dataframe(config, app, self),
+            callback=lambda: core.download_dataframe(config, self),
             filename=config.panel.file_name + ".xlsx",
             sizing_mode="stretch_width",
             icon="download",
             icon_size="2em",
         )
         # Password button
         self.submit_password_button = pnw.Button(
```

### Comparing `dlunch-3.0.0/dlunch/models.py` & `dlunch-3.1.0/dlunch/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     id = Column(Integer, Identity(start=1, cycle=True), primary_key=True)
     user = Column(
         String(100),
         ForeignKey("users.id", ondelete="CASCADE"),
         index=True,
         nullable=False,
     )
-    lunch_time = Column(String(7), index=True, nullable=False)
+    user_record = relationship("Users", back_populates="orders", uselist=False)
     menu_item_id = Column(
         Integer,
         ForeignKey("menu.id", ondelete="CASCADE"),
         nullable=False,
     )
     menu_item = relationship("Menu", back_populates="orders")
     note = Column(String(300), unique=False, nullable=True)
@@ -261,17 +261,24 @@
     )
     guest = Column(
         String(20),
         nullable=False,
         default="NotAGuest",
         server_default="NotAGuest",
     )
+    lunch_time = Column(String(7), index=True, nullable=False)
     takeaway = Column(
         Boolean, nullable=False, default=False, server_default=sql_false()
     )
+    orders = relationship(
+        "Orders",
+        back_populates="user_record",
+        cascade="all, delete-orphan",
+        passive_deletes=True,
+    )
 
     @classmethod
     def clear(self, config: DictConfig) -> int:
         """Clear table and return deleted rows"""
 
         session = create_session(config)
         with session:
```

### Comparing `dlunch-3.0.0/dlunch/quotes.xlsx` & `dlunch-3.1.0/dlunch/quotes.xlsx`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/scheduled_tasks.py` & `dlunch-3.1.0/dlunch/scheduled_tasks.py`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/static/css/guest_override.css` & `dlunch-3.1.0/dlunch/static/css/guest_override.css`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/static/css/labels.css` & `dlunch-3.1.0/dlunch/static/css/labels.css`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/static/images/favicon.ico` & `dlunch-3.1.0/dlunch/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/static/images/logo.png` & `dlunch-3.1.0/dlunch/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/static/images/no_menu.jpg` & `dlunch-3.1.0/dlunch/static/images/no_menu.jpg`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/templates/error.html` & `dlunch-3.1.0/dlunch/templates/error.html`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/templates/login_basic.html` & `dlunch-3.1.0/dlunch/templates/login_basic.html`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/templates/login_oauth.html` & `dlunch-3.1.0/dlunch/templates/login_oauth.html`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch/templates/logout.html` & `dlunch-3.1.0/dlunch/templates/logout.html`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/dlunch.egg-info/PKG-INFO` & `dlunch-3.1.0/dlunch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: dlunch
-Version: 3.0.0
+Version: 3.1.0
 Summary: The ultimate web app for a well organized lunch.
 Author-email: Michele Alberti <michele.alberti90@gmail.com>
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
 Project-URL: Homepage, https://github.com/Michele-Alberti/data-lunch
 Project-URL: Issues, https://github.com/Michele-Alberti/data-lunch/issues
 Keywords: python,webapp,lunch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: setuptools==69.1.1
+Requires-Dist: setuptools==69.2.0
 Requires-Dist: click==8.1.7
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: ipykernel==6.29.3
 Requires-Dist: ipywidgets==8.1.2
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: pandas==2.2.1
 Requires-Dist: passlib==1.7.4
 Requires-Dist: tenacity==8.2.3
 Requires-Dist: tqdm==4.66.2
-Requires-Dist: panel==1.3.8
-Requires-Dist: sqlalchemy==2.0.28
+Requires-Dist: panel==1.4.0
+Requires-Dist: sqlalchemy==2.0.29
 Requires-Dist: psycopg==3.1.18
 Requires-Dist: hydra-core==1.3.2
-Requires-Dist: google-cloud-storage==2.14.0
+Requires-Dist: google-cloud-storage==2.16.0
 Requires-Dist: pytesseract==0.3.10
 
 # Data Lunch <!-- omit in toc -->
 
 The ultimate web app for a well organized lunch.
 
 ## 1. Table of contents
```

### Comparing `dlunch-3.0.0/dlunch.egg-info/SOURCES.txt` & `dlunch-3.1.0/dlunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlunch-3.0.0/pyproject.toml` & `dlunch-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dlunch"
-version = "3.0.0"
+version = "3.1.0"
 authors = [
   { name="Michele Alberti", email="michele.alberti90@gmail.com" },
 ]
 description = "The ultimate web app for a well organized lunch."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["python", "webapp", "lunch"]
@@ -48,15 +48,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.0.0"
+version = "3.1.0"
 version_files = [
     "dlunch/__init__.py",
     "pyproject.toml:version",
 ]
 tag_format = "v$version"
 changelog_file = "changelog.md"
 update_changelog_on_bump = true
```

