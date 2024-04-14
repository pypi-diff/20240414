# Comparing `tmp/grill-names-2.6.0.tar.gz` & `tmp/grill_names-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "B:\write\code\git\grill-names\dist\tmpi4vm9249\grill-names-2.6.0.tar", last modified: Fri Sep 23 23:45:35 2022, max compression
+gzip compressed data, was "grill_names-2.6.1.tar", last modified: Sun Apr 14 11:26:03 2024, max compression
```

## Comparing `grill-names-2.6.0.tar` & `grill_names-2.6.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-09-23 23:45:35.560110 grill-names-2.6.0/
--rw-rw-rw-   0        0        0     1087 2022-09-23 22:52:14.000000 grill-names-2.6.0/LICENSE
--rw-rw-rw-   0        0        0     1230 2022-09-23 23:45:35.560110 grill-names-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      775 2020-11-25 14:12:44.000000 grill-names-2.6.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-23 23:45:35.511124 grill-names-2.6.0/grill/
-drwxrwxrwx   0        0        0        0 2022-09-23 23:45:35.520112 grill-names-2.6.0/grill/names/
--rw-rw-rw-   0        0        0    10424 2022-09-23 22:52:20.000000 grill-names-2.6.0/grill/names/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-23 23:45:35.512108 grill-names-2.6.0/grill/tokens/
-drwxrwxrwx   0        0        0        0 2022-09-23 23:45:35.541124 grill-names-2.6.0/grill/tokens/ids/
--rw-rw-rw-   0        0        0     1559 2021-02-16 11:11:52.000000 grill-names-2.6.0/grill/tokens/ids/CGAsset.cfg
--rw-rw-rw-   0        0        0     2116 2020-07-14 08:55:01.000000 grill-names-2.6.0/grill/tokens/ids/LifeTR.cfg
--rw-rw-rw-   0        0        0      801 2021-05-15 07:41:05.000000 grill-names-2.6.0/grill/tokens/ids/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-23 23:45:35.559125 grill-names-2.6.0/grill_names.egg-info/
--rw-rw-rw-   0        0        0     1230 2022-09-23 23:45:35.000000 grill-names-2.6.0/grill_names.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2022-09-23 23:45:35.000000 grill-names-2.6.0/grill_names.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-23 23:45:35.000000 grill-names-2.6.0/grill_names.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2022-09-23 23:45:35.000000 grill-names-2.6.0/grill_names.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-09-23 23:45:35.000000 grill-names-2.6.0/grill_names.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      825 2022-09-23 23:45:35.565125 grill-names-2.6.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2020-09-20 04:59:58.000000 grill-names-2.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:26:03.124803 grill_names-2.6.1/
+-rw-rw-rw-   0        0        0     1087 2024-03-09 06:19:15.000000 grill_names-2.6.1/LICENSE
+-rw-rw-rw-   0        0        0     1804 2024-04-14 11:26:03.124803 grill_names-2.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2024-03-09 06:19:15.000000 grill_names-2.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 11:26:03.073281 grill_names-2.6.1/grill/
+drwxrwxrwx   0        0        0        0 2024-04-14 11:26:03.073281 grill_names-2.6.1/grill/names/
+-rw-rw-rw-   0        0        0    10257 2024-04-14 06:17:46.000000 grill_names-2.6.1/grill/names/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:26:03.073281 grill_names-2.6.1/grill/tokens/
+drwxrwxrwx   0        0        0        0 2024-04-14 11:26:03.089040 grill_names-2.6.1/grill/tokens/ids/
+-rw-rw-rw-   0        0        0     1559 2024-03-09 06:19:15.000000 grill_names-2.6.1/grill/tokens/ids/CGAsset.cfg
+-rw-rw-rw-   0        0        0     2116 2024-04-14 05:31:52.000000 grill_names-2.6.1/grill/tokens/ids/LifeTR.cfg
+-rw-rw-rw-   0        0        0      801 2024-04-14 05:32:05.000000 grill_names-2.6.1/grill/tokens/ids/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:26:03.124803 grill_names-2.6.1/grill_names.egg-info/
+-rw-rw-rw-   0        0        0     1804 2024-04-14 11:26:03.000000 grill_names-2.6.1/grill_names.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-14 11:26:03.000000 grill_names-2.6.1/grill_names.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 11:26:03.000000 grill_names-2.6.1/grill_names.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2024-04-14 11:26:03.000000 grill_names-2.6.1/grill_names.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-14 11:26:03.000000 grill_names-2.6.1/grill_names.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      945 2024-04-14 11:26:03.140594 grill_names-2.6.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-09 06:19:15.000000 grill_names-2.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:26:03.124803 grill_names-2.6.1/tests/
+-rw-rw-rw-   0        0        0     3865 2024-03-09 06:19:15.000000 grill_names-2.6.1/tests/test_names.py
+-rw-rw-rw-   0        0        0      358 2024-03-09 06:19:15.000000 grill_names-2.6.1/tests/test_tokens.py
```

### Comparing `grill-names-2.6.0/LICENSE` & `grill_names-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grill-names-2.6.0/README.md` & `grill_names-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `grill-names-2.6.0/grill/names/__init__.py` & `grill_names-2.6.1/grill/names/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import uuid
 import typing
+import textwrap
 import itertools
 import collections
 from datetime import datetime
 
 import naming
 try:
     from pxr import Sdf
@@ -39,15 +40,15 @@
     format_rows = []
     for r in rows:
         filler = '=<' if r == table_sep else ''
         format_rows.append(' '.join(
             f"{{:{f'{filler}'}{f'{size}'}}}".format(i)
             for size, i in zip(max_sizes, r))
         )
-    return '\n'.join(format_rows)
+    return textwrap.indent('\n'.join(format_rows), prefix="    ")
 
 
 class DefaultName(naming.Name):
     """ Inherited by: :class:`grill.names.CGAsset`
 
     Base class for any Name object that wishes to provide `default` functionality via
     the `get_default` method.
@@ -68,15 +69,15 @@
 
 class DefaultFile(DefaultName, naming.File):
     """ Inherited by: :class:`grill.names.DateTimeFile`
 
     Similar to :class:`grill.names.DefaultName`, provides File Name objects default
     creation via the `get_default` method.
 
-    Adds an extra `DEFAULT_SUFFIX='ext'` member that will be used when creating objects.
+    Adds an extra ``DEFAULT_SUFFIX='ext'`` member that will be used when creating objects.
     """
 
     DEFAULT_SUFFIX = 'ext'
 
     @property
     def _defaults(self):
         result = super()._defaults
@@ -85,27 +86,27 @@
 
 
 class DateTimeFile(DefaultFile):
     """Time based file names respecting iso standard.
 
     ============= ================
     **Config:**
-    ------------------------------
+    ==============================
     *year*        Between :py:data:`datetime.MINYEAR` and :py:data:`datetime.MAXYEAR` inclusive.
     *month*       Between 1 and 12 inclusive.
     *day*         Between 1 and the number of days in the given month of the given year.
     *hour*        In ``range(24)``.
     *minute*      In ``range(60)``.
     *second*      In ``range(60)``.
     *microsecond* In ``range(1000000)``.
     ============= ================
 
     ======  ============
     **Composed Fields:**
-    --------------------
+    ====================
     *date*  `year` `month` `day`
     *time*  `hour` `minute` `second` `microsecond`
     ======  ============
 
     .. note::
         When getting a new default name, current ISO time at the moment of execution is used.
 
@@ -246,15 +247,15 @@
         >>> asset_id.suffix = 'usdc'
         >>> asset_id.version = 42
         >>> asset_id
         UsdAsset("demo-3d-abc-entity-rnd-main-atom-lead-base-whole.42.usdc")
         >>> asset_id.suffix = 'abc'
         Traceback (most recent call last):
         ...
-        ValueError: Can't set invalid name 'demo-3d-abc-entity-rnd-main-atom-lead-base-whole.42.abc' on UsdAsset("demo-3d-abc-entity-rnd-main-atom-lead-base-whole.42.usdc"). Valid convention is: '{code}-{media}-{kingdom}-{cluster}-{area}-{stream}-{item}-{step}-{variant}-{part}.{pipe}.{suffix}' with pattern: '^(?P<code>\w+)\-(?P<media>\w+)\-(?P<kingdom>\w+)\-(?P<cluster>\w+)\-(?P<area>\w+)\-(?P<stream>\w+)\-(?P<item>\w+)\-(?P<step>\w+)\-(?P<variant>\w+)\-(?P<part>\w+)(?P<pipe>(\.(?P<output>\w+))?\.(?P<version>\d+)(\.(?P<index>\d+))?)(\.(?P<suffix>sdf|usd|usda|usdc|usdz))$'
+        ValueError: Can't set invalid name 'demo-3d-abc-entity-rnd-main-atom-lead-base-whole.42.abc' on UsdAsset("demo-3d-abc-entity-rnd-main-atom-lead-base-whole.42.usdc"). Valid convention is: '{code}-{media}-{kingdom}-{cluster}-{area}-{stream}-{item}-{step}-{variant}-{part}.{pipe}.{suffix}' with pattern: '^(?P<code>...(?P<suffix>sdf|usd|usda|usdc|usdz))$'
 
     .. seealso::
         :class:`grill.names.CGAsset` for a description of available fields, :class:`naming.Name` for an overview of the core API.
 
     """
     DEFAULT_SUFFIX = 'usd'
     file_config = naming.NameConfig(
```

### Comparing `grill-names-2.6.0/grill/tokens/ids/CGAsset.cfg` & `grill_names-2.6.1/grill/tokens/ids/CGAsset.cfg`

 * *Files identical despite different names*

### Comparing `grill-names-2.6.0/grill/tokens/ids/LifeTR.cfg` & `grill_names-2.6.1/grill/tokens/ids/LifeTR.cfg`

 * *Files identical despite different names*

### Comparing `grill-names-2.6.0/grill/tokens/ids/__init__.py` & `grill_names-2.6.1/grill/tokens/ids/__init__.py`

 * *Files identical despite different names*

