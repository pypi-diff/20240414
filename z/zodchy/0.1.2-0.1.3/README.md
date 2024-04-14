# Comparing `tmp/zodchy-0.1.2.tar.gz` & `tmp/zodchy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy-0.1.2.tar", max compression
+gzip compressed data, was "zodchy-0.1.3.tar", max compression
```

## Comparing `zodchy-0.1.2.tar` & `zodchy-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy-0.1.2/README.md
--rw-r--r--   0        0        0      263 2024-04-13 11:49:18.573964 zodchy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-11 07:57:07.719271 zodchy-0.1.2/zodchy/__init__.py
--rw-r--r--   0        0        0      459 2024-04-11 07:57:07.719421 zodchy-0.1.2/zodchy/codex/__init__.py
--rw-r--r--   0        0        0       65 2024-04-02 15:23:42.894657 zodchy-0.1.2/zodchy/codex/base.py
--rw-r--r--   0        0        0     1084 2024-04-02 15:23:42.894771 zodchy-0.1.2/zodchy/codex/communication.py
--rw-r--r--   0        0        0      390 2024-04-05 16:20:59.839302 zodchy-0.1.2/zodchy/codex/cqrs.py
--rw-r--r--   0        0        0     1468 2024-04-11 07:57:07.719538 zodchy-0.1.2/zodchy/codex/di.py
--rw-r--r--   0        0        0      161 2024-04-02 15:23:42.895433 zodchy-0.1.2/zodchy/codex/identity.py
--rw-r--r--   0        0        0     2475 2024-04-02 15:23:42.895562 zodchy-0.1.2/zodchy/codex/query.py
--rw-r--r--   0        0        0       19 2024-04-02 15:23:42.895673 zodchy-0.1.2/zodchy/notations/__init__.py
--rw-r--r--   0        0        0     7589 2024-04-02 15:23:42.895777 zodchy-0.1.2/zodchy/notations/math.py
--rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 zodchy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy-0.1.3/README.md
+-rw-r--r--   0        0        0      290 2024-04-14 12:49:14.155252 zodchy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-11 07:57:07.719271 zodchy-0.1.3/zodchy/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-11 07:57:07.719421 zodchy-0.1.3/zodchy/codex/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-02 15:23:42.894657 zodchy-0.1.3/zodchy/codex/base.py
+-rw-r--r--   0        0        0     1084 2024-04-02 15:23:42.894771 zodchy-0.1.3/zodchy/codex/communication.py
+-rw-r--r--   0        0        0      390 2024-04-05 16:20:59.839302 zodchy-0.1.3/zodchy/codex/cqrs.py
+-rw-r--r--   0        0        0     1468 2024-04-11 07:57:07.719538 zodchy-0.1.3/zodchy/codex/di.py
+-rw-r--r--   0        0        0      161 2024-04-02 15:23:42.895433 zodchy-0.1.3/zodchy/codex/identity.py
+-rw-r--r--   0        0        0     2475 2024-04-02 15:23:42.895562 zodchy-0.1.3/zodchy/codex/query.py
+-rw-r--r--   0        0        0       19 2024-04-02 15:23:42.895673 zodchy-0.1.3/zodchy/notations/__init__.py
+-rw-r--r--   0        0        0     7589 2024-04-02 15:23:42.895777 zodchy-0.1.3/zodchy/notations/math.py
+-rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 zodchy-0.1.3/PKG-INFO
```

### Comparing `zodchy-0.1.2/zodchy/codex/communication.py` & `zodchy-0.1.3/zodchy/codex/communication.py`

 * *Files identical despite different names*

### Comparing `zodchy-0.1.2/zodchy/codex/di.py` & `zodchy-0.1.3/zodchy/codex/di.py`

 * *Files identical despite different names*

### Comparing `zodchy-0.1.2/zodchy/codex/query.py` & `zodchy-0.1.3/zodchy/codex/query.py`

 * *Files identical despite different names*

### Comparing `zodchy-0.1.2/zodchy/notations/math.py` & `zodchy-0.1.3/zodchy/notations/math.py`

 * *Files identical despite different names*

