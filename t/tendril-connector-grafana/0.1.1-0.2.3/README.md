# Comparing `tmp/tendril-connector-grafana-0.1.1.tar.gz` & `tmp/tendril_connector_grafana-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-connector-grafana-0.1.1.tar", last modified: Wed Apr 10 20:54:18 2024, max compression
+gzip compressed data, was "tendril_connector_grafana-0.2.3.tar", last modified: Sun Apr 14 11:51:52 2024, max compression
```

## Comparing `tendril-connector-grafana-0.1.1.tar` & `tendril_connector_grafana-0.2.3.tar`

### file list

```diff
@@ -1,69 +1,76 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3697 2024-04-10 20:54:18.811783 tendril-connector-grafana-0.1.1/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2352 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.803783 tendril-connector-grafana-0.1.1/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.803783 tendril-connector-grafana-0.1.1/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-connector-grafana-0.1.1/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13480 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      915 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1596 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-10 20:54:18.811783 tendril-connector-grafana-0.1.1/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3221 2024-04-10 20:53:32.000000 tendril-connector-grafana-0.1.1/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.803783 tendril-connector-grafana-0.1.1/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril-connector-grafana-0.1.1/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/authz/domains/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      245 2024-04-08 19:48:32.000000 tendril-connector-grafana-0.1.1/src/tendril/authz/domains/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2332 2024-04-10 15:33:51.000000 tendril-connector-grafana-0.1.1/src/tendril/authz/domains/grafana.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-08-20 06:43:27.000000 tendril-connector-grafana-0.1.1/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3579 2024-04-10 13:20:13.000000 tendril-connector-grafana-0.1.1/src/tendril/config/grafana.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/connectors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-20 10:40:24.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-09 09:37:51.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-09 09:49:05.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      114 2024-04-10 18:21:20.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/datasources.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1076 2024-04-10 17:46:49.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/folders.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      289 2024-04-09 12:23:46.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/health.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      918 2024-04-10 15:27:47.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/teams.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2363 2024-04-09 16:21:32.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/users.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      993 2024-04-09 12:18:27.000000 tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/aio.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril-connector-grafana-0.1.1/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/core/topology/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril-connector-grafana-0.1.1/src/tendril/core/topology/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril/core/topology/grafana/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril-connector-grafana-0.1.1/src/tendril/core/topology/grafana/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1152 2024-04-10 17:54:30.000000 tendril-connector-grafana-0.1.1/src/tendril/core/topology/grafana/folders.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      679 2024-04-10 15:17:50.000000 tendril-connector-grafana-0.1.1/src/tendril/core/topology/grafana/teams.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/src/tendril_connector_grafana.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3697 2024-04-10 20:54:18.000000 tendril-connector-grafana-0.1.1/src/tendril_connector_grafana.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1478 2024-04-10 20:54:18.000000 tendril-connector-grafana-0.1.1/src/tendril_connector_grafana.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-10 20:54:18.000000 tendril-connector-grafana-0.1.1/src/tendril_connector_grafana.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      527 2024-04-10 20:54:18.000000 tendril-connector-grafana-0.1.1/src/tendril_connector_grafana.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-10 20:54:18.000000 tendril-connector-grafana-0.1.1/src/tendril_connector_grafana.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-10 20:54:18.807783 tendril-connector-grafana-0.1.1/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2024-04-08 21:57:25.000000 tendril-connector-grafana-0.1.1/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.871618 tendril_connector_grafana-0.2.3/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5479 2024-04-14 11:51:52.871618 tendril_connector_grafana-0.2.3/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2352 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.859618 tendril_connector_grafana-0.2.3/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_connector_grafana-0.2.3/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13480 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      915 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1596 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-14 11:51:52.875618 tendril_connector_grafana-0.2.3/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3221 2024-04-14 11:51:30.000000 tendril_connector_grafana-0.2.3/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.859618 tendril_connector_grafana-0.2.3/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2022-11-28 19:30:01.000000 tendril_connector_grafana-0.2.3/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/src/tendril/authz/domains/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      245 2024-04-08 19:48:32.000000 tendril_connector_grafana-0.2.3/src/tendril/authz/domains/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2332 2024-04-10 15:33:51.000000 tendril_connector_grafana-0.2.3/src/tendril/authz/domains/grafana.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-08-20 06:43:27.000000 tendril_connector_grafana-0.2.3/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5117 2024-04-14 11:10:41.000000 tendril_connector_grafana-0.2.3/src/tendril/config/grafana.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/src/tendril/connectors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-20 10:40:24.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-09 09:37:51.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.863618 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-09 09:49:05.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1861 2024-04-14 11:28:36.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/dashboards.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1095 2024-04-12 09:41:13.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/datasources.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1276 2024-04-14 11:28:36.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/folders.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      289 2024-04-09 12:23:46.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/health.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1720 2024-04-14 06:23:35.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/libraries.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      918 2024-04-10 15:27:47.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/teams.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2363 2024-04-09 16:21:32.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/users.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      978 2024-04-12 16:22:44.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/aio.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.867618 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-11 17:27:43.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1642 2024-04-14 10:15:16.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/models/dashboard.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      884 2024-04-14 06:23:35.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/models/panel.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1059 2024-04-14 05:39:35.000000 tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/models/variables.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.867618 tendril_connector_grafana-0.2.3/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_connector_grafana-0.2.3/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.867618 tendril_connector_grafana-0.2.3/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_connector_grafana-0.2.3/src/tendril/core/topology/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.867618 tendril_connector_grafana-0.2.3/src/tendril/core/topology/grafana/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_connector_grafana-0.2.3/src/tendril/core/topology/grafana/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1152 2024-04-10 17:54:30.000000 tendril_connector_grafana-0.2.3/src/tendril/core/topology/grafana/folders.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      679 2024-04-10 15:17:50.000000 tendril_connector_grafana-0.2.3/src/tendril/core/topology/grafana/teams.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.867618 tendril_connector_grafana-0.2.3/src/tendril_connector_grafana.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5479 2024-04-14 11:51:52.000000 tendril_connector_grafana-0.2.3/src/tendril_connector_grafana.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1782 2024-04-14 11:51:52.000000 tendril_connector_grafana-0.2.3/src/tendril_connector_grafana.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-14 11:51:52.000000 tendril_connector_grafana-0.2.3/src/tendril_connector_grafana.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      527 2024-04-14 11:51:52.000000 tendril_connector_grafana-0.2.3/src/tendril_connector_grafana.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-14 11:51:52.000000 tendril_connector_grafana-0.2.3/src/tendril_connector_grafana.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 11:51:52.867618 tendril_connector_grafana-0.2.3/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2024-04-08 21:57:25.000000 tendril_connector_grafana-0.2.3/tox.ini
```

### Comparing `tendril-connector-grafana-0.1.1/.gitignore` & `tendril_connector_grafana-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/.readthedocs.yml` & `tendril_connector_grafana-0.2.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/.travis.yml` & `tendril_connector_grafana-0.2.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/LICENSE` & `tendril_connector_grafana-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/README.rst` & `tendril_connector_grafana-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/Makefile` & `tendril_connector_grafana-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/_static/custom.css` & `tendril_connector_grafana-0.2.3/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/_static/favicon.ico` & `tendril_connector_grafana-0.2.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/_static/logo.png` & `tendril_connector_grafana-0.2.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/_static/logo_packed.png` & `tendril_connector_grafana-0.2.3/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/_templates/about.html` & `tendril_connector_grafana-0.2.3/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/conf.py` & `tendril_connector_grafana-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/index.rst` & `tendril_connector_grafana-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/docs/installation.rst` & `tendril_connector_grafana-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/setup.py` & `tendril_connector_grafana-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/src/tendril/authz/domains/grafana.py` & `tendril_connector_grafana-0.2.3/src/tendril/authz/domains/grafana.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/src/tendril/config/__init__.py` & `tendril_connector_grafana-0.2.3/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/src/tendril/config/grafana.py` & `tendril_connector_grafana-0.2.3/src/tendril/config/grafana.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,28 +40,36 @@
     ),
     ConfigOption(
         'GRAFANA_SERVER_SSL',
         "True",
         "Whether to use SSL (https)."
     ),
     ConfigOption(
+        'GRAFANA_BASE_URL',
+        "''",
+        "Base URL to use for Grafana Embed Links. This is technically the same as the "
+        "server pointed to by GRAFANA_SERVER-*, but must be spearately configured for quirky "
+        "reasons related to deployment topologies."
+    ),
+    ConfigOption(
         'GRAFANA_ORG',
         "1",
         "Grafana Organization to use. This is normally 1, unless the Grafana is multi-tenant. "
         "What should happen if Tendril itself is multi-tenant is unclear."
     ),
     ConfigOption(
         'GRAFANA_ADMIN_USER',
         "'admin'",
         "User to use with Grafana Admin API interfaces needing Basic Auth."
     ),
 ConfigOption(
         'GRAFANA_ADMIN_PASSWORD',
         "'admin'",
-        "Password to use with Grafana Admin API interfaces needing Basic Auth."
+        "Password to use with Grafana Admin API interfaces needing Basic Auth.",
+        masked=True
     ),
     ConfigOption(
         'GRAFANA_PROVISIONER_TOKEN',
         "''",
         "Grafana Service Account token which allows creation and management of "
         "Teams and dashboards",
         masked=True
@@ -84,15 +92,37 @@
             "Members of ancestor interests always get access. "
     ),
     ConfigOption(
         'GRAFANA_TEAM_EMAIL_DOMAIN',
         default='.tendril.link',
         doc="Domain suffix to use for team emails. This is not particularly "
             "important, it just is."
-    )
+    ),
+    ConfigOption(
+        'GRAFANA_DATASOURCE_INFLUXDB_MONITORS',
+        default='None',
+        doc="InfluxDB datasource to use for Grafana for Tendril Monitors. This should be separately be "
+            "configured and prepared, and only the Name should be provided here."
+    ),
+    ConfigOption(
+        'GRAFANA_DATASOURCE_BACKEND_READER',
+        default='None',
+        doc="PostgreSQL datasource to use for Grafana for Tendril Backend Read. This should be "
+            "separately be configured and prepared, and only the Name should be provided here. "
+            "Typically, this would be a user on the primary database with Read Only access. "
+            "Currently, we only use the Interest table."
+    ),
+    ConfigOption(
+        'GRAFANA_LIBRARIES_FOLDER',
+        default='"Library"',
+        doc="Top level folder for Grafana Library panels. Generally, users are expected to have full "
+            "read acces to this folder and everything beneath this. The actual folder structure within "
+            "is somewhat implementation / instance dependent. Presently, we are implementing for folders "
+            "to have the lowercase singular name of the interest type they apply to."
+    ),
 ]
 
 
 def load(manager):
     logger.debug("Loading {0}".format(__name__))
     manager.load_elements(config_elements_grafana,
                           doc="Tendril Grafana Configuration")
```

### Comparing `tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/teams.py` & `tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/teams.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/actions/users.py` & `tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/actions/users.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/src/tendril/connectors/grafana/aio.py` & `tendril_connector_grafana-0.2.3/src/tendril/connectors/grafana/aio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 
 
-import asyncio
 from grafana_client import AsyncGrafanaApi
 from grafana_client import TokenAuth
 
 from tendril.config import GRAFANA_SERVER_HOST
 from tendril.config import GRAFANA_SERVER_PORT
 from tendril.config import GRAFANA_SERVER_SSL
 from tendril.config import GRAFANA_PROVISIONER_TOKEN
```

### Comparing `tendril-connector-grafana-0.1.1/src/tendril/core/topology/grafana/folders.py` & `tendril_connector_grafana-0.2.3/src/tendril/core/topology/grafana/folders.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/src/tendril/core/topology/grafana/teams.py` & `tendril_connector_grafana-0.2.3/src/tendril/core/topology/grafana/teams.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/src/tendril_connector_grafana.egg-info/SOURCES.txt` & `tendril_connector_grafana-0.2.3/src/tendril_connector_grafana.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -26,19 +26,25 @@
 src/tendril/authz/domains/grafana.py
 src/tendril/config/__init__.py
 src/tendril/config/grafana.py
 src/tendril/connectors/__init__.py
 src/tendril/connectors/grafana/__init__.py
 src/tendril/connectors/grafana/aio.py
 src/tendril/connectors/grafana/actions/__init__.py
+src/tendril/connectors/grafana/actions/dashboards.py
 src/tendril/connectors/grafana/actions/datasources.py
 src/tendril/connectors/grafana/actions/folders.py
 src/tendril/connectors/grafana/actions/health.py
+src/tendril/connectors/grafana/actions/libraries.py
 src/tendril/connectors/grafana/actions/teams.py
 src/tendril/connectors/grafana/actions/users.py
+src/tendril/connectors/grafana/models/__init__.py
+src/tendril/connectors/grafana/models/dashboard.py
+src/tendril/connectors/grafana/models/panel.py
+src/tendril/connectors/grafana/models/variables.py
 src/tendril/core/__init__.py
 src/tendril/core/topology/__init__.py
 src/tendril/core/topology/grafana/__init__.py
 src/tendril/core/topology/grafana/folders.py
 src/tendril/core/topology/grafana/teams.py
 src/tendril_connector_grafana.egg-info/PKG-INFO
 src/tendril_connector_grafana.egg-info/SOURCES.txt
```

### Comparing `tendril-connector-grafana-0.1.1/src/tendril_connector_grafana.egg-info/requires.txt` & `tendril_connector_grafana-0.2.3/src/tendril_connector_grafana.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/tests/coveralls.py` & `tendril_connector_grafana-0.2.3/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-connector-grafana-0.1.1/tox.ini` & `tendril_connector_grafana-0.2.3/tox.ini`

 * *Files identical despite different names*

