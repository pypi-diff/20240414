# Comparing `tmp/sprinko-0.0.14.tar.gz` & `tmp/sprinko-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprinko-0.0.14.tar", last modified: Thu Mar 14 19:50:59 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sprinko-0.0.14.tar` & `sprinko-0.9.0b1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 19:50:59.762679 sprinko-0.0.14/
--rw-rw-rw-   0        0        0     1085 2024-03-13 15:27:07.000000 sprinko-0.0.14/LICENSE
--rw-rw-rw-   0        0        0      209 2024-03-14 19:50:59.762679 sprinko-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0       10 2024-03-14 19:28:42.000000 sprinko-0.0.14/README.md
--rw-rw-rw-   0        0        0       75 2024-03-14 19:40:34.000000 sprinko-0.0.14/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 19:50:59.762679 sprinko-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0      802 2024-03-14 19:42:20.000000 sprinko-0.0.14/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:50:59.756677 sprinko-0.0.14/sprinko/
--rw-rw-rw-   0        0        0     3009 2024-03-14 19:44:16.000000 sprinko-0.0.14/sprinko/cli.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:50:59.761679 sprinko-0.0.14/sprinko/core/
--rw-rw-rw-   0        0        0      172 2024-03-13 18:39:49.000000 sprinko-0.0.14/sprinko/core/__base__.py
--rw-rw-rw-   0        0        0      106 2024-03-14 19:50:22.000000 sprinko-0.0.14/sprinko/core/__init__.py
--rw-rw-rw-   0        0        0     1553 2024-03-14 19:45:30.000000 sprinko-0.0.14/sprinko/core/ctx.py
--rw-rw-rw-   0        0        0     8300 2024-03-14 18:50:42.000000 sprinko-0.0.14/sprinko/core/ko.py
--rw-rw-rw-   0        0        0     3676 2024-03-14 19:32:59.000000 sprinko-0.0.14/sprinko/core/sprinko.py
--rw-rw-rw-   0        0        0     1193 2024-03-13 21:55:31.000000 sprinko-0.0.14/sprinko/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:50:59.761679 sprinko-0.0.14/sprinko.egg-info/
--rw-rw-rw-   0        0        0      209 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/top_level.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.gitattributes
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.python-version
+-rw-r--r--   0        0        0    35802 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/LICENSE
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/requirements-dev.lock
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/requirements.lock
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.vscode/launch.json
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.vscode/tasks.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/__init__.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/__main__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/_query.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/generate.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/info.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/run.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/cmds/setup.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/core/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/core/ctx.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/core/mselect.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/utils/__init__.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/utils/selection.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/src/sprinko/utils/std.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/pyproject.toml
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 sprinko-0.9.0b1/PKG-INFO
```

