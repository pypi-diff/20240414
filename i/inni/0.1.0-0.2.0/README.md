# Comparing `tmp/inni-0.1.0.tar.gz` & `tmp/inni-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inni-0.1.0.tar", max compression
+gzip compressed data, was "inni-0.2.0.tar", max compression
```

## Comparing `inni-0.1.0.tar` & `inni-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,16 @@
--rw-r--r--   0        0        0    34580 2024-03-31 18:16:37.639008 inni-0.1.0/LICENSE
--rw-r--r--   0        0        0       72 2024-03-31 18:16:37.639008 inni-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-31 18:16:37.639008 inni-0.1.0/inni/__init__.py
--rw-r--r--   0        0        0      344 2024-03-31 18:16:37.639008 inni-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 inni-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34580 2024-03-31 17:04:25.743804 inni-0.2.0/LICENSE
+-rw-r--r--   0        0        0       72 2024-03-31 17:04:25.743804 inni-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-31 17:05:35.833524 inni-0.2.0/inni/__init__.py
+-rw-r--r--   0        0        0     3079 2024-04-10 09:44:17.476489 inni-0.2.0/inni/cli.py
+-rw-r--r--   0        0        0      846 2024-04-01 18:30:02.973972 inni-0.2.0/inni/config.py
+-rw-r--r--   0        0        0      302 2024-04-01 16:40:38.551065 inni-0.2.0/inni/loader.py
+-rw-r--r--   0        0        0        0 2024-03-31 19:25:36.344130 inni-0.2.0/inni/modules/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-07 14:41:37.839809 inni-0.2.0/inni/modules/base.py
+-rw-r--r--   0        0        0     2782 2024-04-14 20:51:50.506469 inni-0.2.0/inni/modules/bitrix.py
+-rw-r--r--   0        0        0      495 2024-04-09 08:17:52.592982 inni-0.2.0/inni/modules/dummy.py
+-rw-r--r--   0        0        0     1558 2024-04-08 19:28:25.219466 inni-0.2.0/inni/modules/email.py
+-rw-r--r--   0        0        0     3631 2024-04-10 21:18:35.144206 inni-0.2.0/inni/modules/jira.py
+-rw-r--r--   0        0        0     1027 2024-04-07 14:25:00.952306 inni-0.2.0/inni/modules/skype.py
+-rw-r--r--   0        0        0      407 2024-04-01 18:29:29.514140 inni-0.2.0/inni/template.py
+-rw-r--r--   0        0        0      632 2024-04-14 20:53:31.316493 inni-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 inni-0.2.0/PKG-INFO
```

### Comparing `inni-0.1.0/LICENSE` & `inni-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inni-0.1.0/PKG-INFO` & `inni-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: inni
-Version: 0.1.0
+Version: 0.2.0
 Summary: Modular system to perform tasks surrounding log-in and log-out.
 License: GPL-3.0
 Author: Ceda EI
 Author-email: ceda_ei@webionite.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: jira (>=3.8.0,<4.0.0)
+Requires-Dist: playwright (>=1.43.0,<2.0.0)
+Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: skpy (>=0.10.6,<0.11.0)
 Description-Content-Type: text/markdown
 
 # inni
 
 Modular system to perform tasks surrounding log-in and log-out.
```

