# Comparing `tmp/htimeseries-6.0.3.tar.gz` & `tmp/htimeseries-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htimeseries-6.0.3.tar", last modified: Thu Mar 21 15:04:53 2024, max compression
+gzip compressed data, was "htimeseries-7.0.0.tar", last modified: Sun Apr 14 08:49:11 2024, max compression
```

## Comparing `htimeseries-6.0.3.tar` & `htimeseries-7.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-03-21 15:04:53.295282 htimeseries-6.0.3/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4123 2024-03-21 15:03:35.000000 htimeseries-6.0.3/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      829 2022-03-06 12:35:19.000000 htimeseries-6.0.3/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      217 2022-03-06 12:35:19.000000 htimeseries-6.0.3/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)    20657 2024-03-21 15:04:53.295282 htimeseries-6.0.3/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15678 2024-03-21 15:03:35.000000 htimeseries-6.0.3/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-03-21 15:04:53.295282 htimeseries-6.0.3/htimeseries/
--rw-r--r--   0 anthony   (1000) anthony   (1000)       96 2024-03-21 15:03:57.000000 htimeseries-6.0.3/htimeseries/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    18384 2024-03-21 15:03:35.000000 htimeseries-6.0.3/htimeseries/htimeseries.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1238 2022-11-22 18:14:13.000000 htimeseries-6.0.3/htimeseries/timezone_utils.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-03-21 15:04:53.295282 htimeseries-6.0.3/htimeseries.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    20657 2024-03-21 15:04:53.000000 htimeseries-6.0.3/htimeseries.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      423 2024-03-21 15:04:53.000000 htimeseries-6.0.3/htimeseries.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-03-21 15:04:53.000000 htimeseries-6.0.3/htimeseries.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-10-16 19:29:51.000000 htimeseries-6.0.3/htimeseries.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2024-03-21 15:04:53.000000 htimeseries-6.0.3/htimeseries.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       12 2024-03-21 15:04:53.000000 htimeseries-6.0.3/htimeseries.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-03-21 15:04:53.295282 htimeseries-6.0.3/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1729 2023-12-14 14:36:21.000000 htimeseries-6.0.3/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-03-21 15:04:53.295282 htimeseries-6.0.3/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-06 12:35:19.000000 htimeseries-6.0.3/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    28272 2024-03-21 15:03:35.000000 htimeseries-6.0.3/tests/test_htimeseries.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1084 2022-11-22 18:14:13.000000 htimeseries-6.0.3/tests/test_timezone_utils.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 08:49:11.211383 htimeseries-7.0.0/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4419 2024-04-14 08:37:54.000000 htimeseries-7.0.0/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      829 2022-03-06 12:35:19.000000 htimeseries-7.0.0/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      217 2022-03-06 12:35:19.000000 htimeseries-7.0.0/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    21041 2024-04-14 08:49:11.211383 htimeseries-7.0.0/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15766 2024-04-12 15:50:49.000000 htimeseries-7.0.0/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 08:49:11.207383 htimeseries-7.0.0/htimeseries/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       96 2024-04-14 08:48:30.000000 htimeseries-7.0.0/htimeseries/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    18892 2024-04-12 16:01:53.000000 htimeseries-7.0.0/htimeseries/htimeseries.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1238 2024-04-12 16:45:56.000000 htimeseries-7.0.0/htimeseries/timezone_utils.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 08:49:11.211383 htimeseries-7.0.0/htimeseries.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    21041 2024-04-14 08:49:11.000000 htimeseries-7.0.0/htimeseries.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      454 2024-04-14 08:49:11.000000 htimeseries-7.0.0/htimeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-14 08:49:11.000000 htimeseries-7.0.0/htimeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-10-16 19:29:51.000000 htimeseries-7.0.0/htimeseries.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2024-04-14 08:49:11.000000 htimeseries-7.0.0/htimeseries.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       12 2024-04-14 08:49:11.000000 htimeseries-7.0.0/htimeseries.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-14 08:49:11.211383 htimeseries-7.0.0/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1729 2024-04-10 07:22:05.000000 htimeseries-7.0.0/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 08:49:11.211383 htimeseries-7.0.0/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16384 2024-04-13 13:28:40.000000 htimeseries-7.0.0/tests/.test_htimeseries.py.swp
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-06 12:35:19.000000 htimeseries-7.0.0/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    29634 2024-04-12 15:45:18.000000 htimeseries-7.0.0/tests/test_htimeseries.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1084 2024-04-01 05:13:59.000000 htimeseries-7.0.0/tests/test_timezone_utils.py
```

### Comparing `htimeseries-6.0.3/HISTORY.rst` & `htimeseries-7.0.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 =======
 History
 =======
 
+7.0.0 (2024-04-14)
+==================
+
+- When saving in file format, the Timezone= parameter now merely
+  contains +HHmm.
+- The HTimeseries.timezone attribute has been abolished; use
+  HTimeseries.data.index.tz instead.
+- When initialized with a dataframe, it checks that the index is aware.
+
 6.0.3 (2024-03-21)
 ==================
 
-- Fixed error with unspecified time zone in HTimeseries objects created empty.
-  Now creating an empty object with ``HTimeseries()`` assumes
+- Fixed error with unspecified time zone in HTimeseries objects created
+  empty.  Now creating an empty object with ``HTimeseries()`` assumes
   ``default_tzinfo=ZoneInfo("UTC")``.
 
 6.0.2 (2023-12-22)
 ==================
 
 - Fixed crash when reading csv with aware timestamps.
 
@@ -18,19 +27,20 @@
 ==================
 
 - Fixed crash when reading csv with only a date column.
 
 6.0.0 (2023-12-14)
 ==================
 
-- Python 3.9 is now required (the reason for this is that backports.zoneinfo is
-  behaving differently from zoneinfo).
-- Only pandas>=1.5,<2  is now supported. Pandas<1.5 probably did not work in
-  5.0.0 either, but it had not been discovered. Pandas>=2 handles ambiguous
-  times differently and is therefore still unsupported.
+- Python 3.9 is now required (the reason for this is that
+  backports.zoneinfo is behaving differently from zoneinfo).
+- Only pandas>=1.5,<2  is now supported. Pandas<1.5 probably did not
+  work in 5.0.0 either, but it had not been discovered. Pandas>=2
+  handles ambiguous times differently and is therefore still
+  unsupported.
 - Increased CSV reading speed by two orders of magnitude.
 
 5.0.0 (2023-11-21)
 ==================
 
 - Removed compatibility with pandas<1. pandas 1 and 2 are now supported.
   This helps avoid an error when reading a data file spanning a time
```

### Comparing `htimeseries-6.0.3/LICENSE` & `htimeseries-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htimeseries-6.0.3/PKG-INFO` & `htimeseries-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htimeseries
-Version: 6.0.3
+Version: 7.0.0
 Summary: Hydrological and meteorological timeseries
 Home-page: https://github.com/openmeteo/htimeseries
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -75,20 +75,20 @@
 and dtypes.
 
 If the ``data`` argument is a filelike object, the time series is read
 from it.  There must be no newline translation in ``data`` (open it with
 ``open(..., newline='\n')``. If ``start_date`` and ``end_date`` are
 specified, it skips rows outside the range.
 
-The contents of the filelike object can be in text format or file format (see
-"formats" below). This is usually auto-detected, but a specific format can
-be specified with the ``format`` parameter.  If reading in text format,
-the returned object just has the ``data`` attribute set. If reading in
-file format , the returned object also has attributes ``unit``,
-``title``, ``comment``, ``timezone``, ``time_step``, ``interval_type``,
+The contents of the filelike object can be in text format or file format
+(see "formats" below). This is usually auto-detected, but a specific
+format can be specified with the ``format`` parameter.  If reading in
+text format, the returned object just has the ``data`` attribute set. If
+reading in file format , the returned object also has attributes
+``unit``, ``title``, ``comment``, ``time_step``, ``interval_type``,
 ``variable``, ``precision`` and ``location``. For the meaning of these
 attributes, see section "File format" below.
 
 These attributes are purely informational. In particular, ``time_step``
 and the other time-step-related attributes don't necessarily mean that
 the pandas object will have a related time step (also called
 "frequency"). In fact, raw time series may be irregular but actually
@@ -269,18 +269,21 @@
         Comment=These five lines form two paragraphs.
 
     The Comment parameter is the only parameter where a blank value is
     significant and indicates an empty line, as can be seen in the
     example above.
 
 **Timezone**
-    The time zone of the timestamps, in the format ``{XXX}
-    (UTC{+HHmm})``, where *XXX* is a time zone name and *+HHmm* is the
-    offset from UTC. Examples are ``EET (UTC+0200)`` and ``VST
-    (UTC-0430)``.
+    The time zone of the timestamps, in the format ``{+HHmm}``, where
+    *+HHmm* is the offset from UTC. Examples are ``+0200`` and
+    ``-0430``.
+
+    Format ``{XXX} (UTC{+HHmm})``, where *XXX* is a time zone name, is
+    also supported but deprecated. It exists only in order to be able to
+    read old files.
 
     The ``TzinfoFromString`` utility (described above) can be used to
     convert this string to a tzinfo_ object.
 
 **Time_step**
     In version 5, a pandas "frequency" string such as ``10min`` (10
     minutes), ``H`` (hour), or ``2M`` (two months). If missing or empty,
@@ -399,19 +402,28 @@
 .. _openhi: https://openhi.net
 
 
 =======
 History
 =======
 
+7.0.0 (2024-04-14)
+==================
+
+- When saving in file format, the Timezone= parameter now merely
+  contains +HHmm.
+- The HTimeseries.timezone attribute has been abolished; use
+  HTimeseries.data.index.tz instead.
+- When initialized with a dataframe, it checks that the index is aware.
+
 6.0.3 (2024-03-21)
 ==================
 
-- Fixed error with unspecified time zone in HTimeseries objects created empty.
-  Now creating an empty object with ``HTimeseries()`` assumes
+- Fixed error with unspecified time zone in HTimeseries objects created
+  empty.  Now creating an empty object with ``HTimeseries()`` assumes
   ``default_tzinfo=ZoneInfo("UTC")``.
 
 6.0.2 (2023-12-22)
 ==================
 
 - Fixed crash when reading csv with aware timestamps.
 
@@ -419,19 +431,20 @@
 ==================
 
 - Fixed crash when reading csv with only a date column.
 
 6.0.0 (2023-12-14)
 ==================
 
-- Python 3.9 is now required (the reason for this is that backports.zoneinfo is
-  behaving differently from zoneinfo).
-- Only pandas>=1.5,<2  is now supported. Pandas<1.5 probably did not work in
-  5.0.0 either, but it had not been discovered. Pandas>=2 handles ambiguous
-  times differently and is therefore still unsupported.
+- Python 3.9 is now required (the reason for this is that
+  backports.zoneinfo is behaving differently from zoneinfo).
+- Only pandas>=1.5,<2  is now supported. Pandas<1.5 probably did not
+  work in 5.0.0 either, but it had not been discovered. Pandas>=2
+  handles ambiguous times differently and is therefore still
+  unsupported.
 - Increased CSV reading speed by two orders of magnitude.
 
 5.0.0 (2023-11-21)
 ==================
 
 - Removed compatibility with pandas<1. pandas 1 and 2 are now supported.
   This helps avoid an error when reading a data file spanning a time
```

### Comparing `htimeseries-6.0.3/README.rst` & `htimeseries-7.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,20 +52,20 @@
 and dtypes.
 
 If the ``data`` argument is a filelike object, the time series is read
 from it.  There must be no newline translation in ``data`` (open it with
 ``open(..., newline='\n')``. If ``start_date`` and ``end_date`` are
 specified, it skips rows outside the range.
 
-The contents of the filelike object can be in text format or file format (see
-"formats" below). This is usually auto-detected, but a specific format can
-be specified with the ``format`` parameter.  If reading in text format,
-the returned object just has the ``data`` attribute set. If reading in
-file format , the returned object also has attributes ``unit``,
-``title``, ``comment``, ``timezone``, ``time_step``, ``interval_type``,
+The contents of the filelike object can be in text format or file format
+(see "formats" below). This is usually auto-detected, but a specific
+format can be specified with the ``format`` parameter.  If reading in
+text format, the returned object just has the ``data`` attribute set. If
+reading in file format , the returned object also has attributes
+``unit``, ``title``, ``comment``, ``time_step``, ``interval_type``,
 ``variable``, ``precision`` and ``location``. For the meaning of these
 attributes, see section "File format" below.
 
 These attributes are purely informational. In particular, ``time_step``
 and the other time-step-related attributes don't necessarily mean that
 the pandas object will have a related time step (also called
 "frequency"). In fact, raw time series may be irregular but actually
@@ -246,18 +246,21 @@
         Comment=These five lines form two paragraphs.
 
     The Comment parameter is the only parameter where a blank value is
     significant and indicates an empty line, as can be seen in the
     example above.
 
 **Timezone**
-    The time zone of the timestamps, in the format ``{XXX}
-    (UTC{+HHmm})``, where *XXX* is a time zone name and *+HHmm* is the
-    offset from UTC. Examples are ``EET (UTC+0200)`` and ``VST
-    (UTC-0430)``.
+    The time zone of the timestamps, in the format ``{+HHmm}``, where
+    *+HHmm* is the offset from UTC. Examples are ``+0200`` and
+    ``-0430``.
+
+    Format ``{XXX} (UTC{+HHmm})``, where *XXX* is a time zone name, is
+    also supported but deprecated. It exists only in order to be able to
+    read old files.
 
     The ``TzinfoFromString`` utility (described above) can be used to
     convert this string to a tzinfo_ object.
 
 **Time_step**
     In version 5, a pandas "frequency" string such as ``10min`` (10
     minutes), ``H`` (hour), or ``2M`` (two months). If missing or empty,
```

### Comparing `htimeseries-6.0.3/htimeseries/htimeseries.py` & `htimeseries-7.0.0/htimeseries/htimeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import csv
 import datetime as dt
 from configparser import ParsingError
 from io import StringIO
-from zoneinfo import ZoneInfo
 
 import numpy as np
 import pandas as pd
 from pandas.tseries.frequencies import to_offset
 from textbisect import text_bisect_left
 
 from .timezone_utils import TzinfoFromString
@@ -83,15 +82,15 @@
     def write_meta(self):
         if self.version == 2:
             self.f.write("Version=2\r\n")
         self.write_simple("unit")
         self.write_count()
         self.write_simple("title")
         self.write_comment()
-        self.write_simple("timezone")
+        self.write_timezone()
         self.write_time_step()
         self.write_simple("interval_type")
         self.write_simple("variable")
         self.write_simple("precision")
         self.write_location()
         self.write_altitude()
 
@@ -104,14 +103,22 @@
         self.f.write("Count={}\r\n".format(len(self.htimeseries.data)))
 
     def write_comment(self):
         if hasattr(self.htimeseries, "comment"):
             for line in self.htimeseries.comment.splitlines():
                 self.f.write("Comment={}\r\n".format(line))
 
+    def write_timezone(self):
+        offset = self.htimeseries.data.index.tz.utcoffset(None)
+        sign = "-+"[offset >= dt.timedelta(0)]
+        offset = abs(offset)
+        hours = offset.seconds // 3600
+        minutes = offset.seconds % 3600 // 60
+        self.f.write(f"Timezone={sign}{hours:02}{minutes:02}\r\n")
+
     def write_location(self):
         if self.version <= 2 or not getattr(self.htimeseries, "location", None):
             return
         self.f.write(
             "Location={:.6f} {:.6f} {}\r\n".format(
                 *[
                     self.htimeseries.location[x]
@@ -213,24 +220,26 @@
             e.args = e.args + (f.line_number,)
             raise
 
     def get_unit(self, name, value):
         self.meta[name] = value
 
     get_title = get_unit
-    get_timezone = get_unit
     get_variable = get_unit
 
     def get_time_step(self, name, value):
         if value and "," in value:
             minutes, months = self.read_minutes_months(value)
             self.meta[name] = self._time_step_from_minutes_months(minutes, months)
         else:
             self.meta[name] = value
 
+    def get_timezone(self, name, value):
+        self.meta["_timezone"] = value
+
     def _time_step_from_minutes_months(self, minutes, months):
         if minutes != 0 and months != 0:
             raise ParsingError("Invalid time step")
         elif minutes != 0:
             return str(minutes) + "min"
         else:
             return str(months) + "M"
@@ -323,26 +332,31 @@
                 "HTimeseries.__init__() got an unexpected keyword argument "
                 f"'{extra_parms.pop()}'"
             )
         for arg, default_value in self.args.items():
             kwargs.setdefault(arg, default_value)
         if data is None:
             if not kwargs["default_tzinfo"]:
-                kwargs["default_tzinfo"] = ZoneInfo("UTC")
+                kwargs["default_tzinfo"] = dt.timezone.utc
             self._read_filelike(StringIO(), **kwargs)
         elif isinstance(data, pd.DataFrame):
+            self._check_dataframe(data)
             self.data = data
         else:
             self._read_filelike(data, **kwargs)
 
+    def _check_dataframe(self, data):
+        if data.index.tz is None:
+            raise TypeError("data.index.tz must exist")
+
     def _read_filelike(self, *args, **kwargs):
         reader = TimeseriesStreamReader(*args, **kwargs)
         self.__dict__.update(reader.get_metadata())
         try:
-            tzinfo = TzinfoFromString(self.timezone)
+            tzinfo = TzinfoFromString(self._timezone)
         except AttributeError:
             tzinfo = kwargs["default_tzinfo"]
         self.data = reader.get_data(tzinfo)
         if self.data.size and (tzinfo is None):
             raise TypeError(
                 "Cannot read filelike object without timezone or default_tzinfo "
                 "specified"
```

### Comparing `htimeseries-6.0.3/htimeseries/timezone_utils.py` & `htimeseries-7.0.0/htimeseries/timezone_utils.py`

 * *Files identical despite different names*

### Comparing `htimeseries-6.0.3/htimeseries.egg-info/PKG-INFO` & `htimeseries-7.0.0/htimeseries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htimeseries
-Version: 6.0.3
+Version: 7.0.0
 Summary: Hydrological and meteorological timeseries
 Home-page: https://github.com/openmeteo/htimeseries
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -75,20 +75,20 @@
 and dtypes.
 
 If the ``data`` argument is a filelike object, the time series is read
 from it.  There must be no newline translation in ``data`` (open it with
 ``open(..., newline='\n')``. If ``start_date`` and ``end_date`` are
 specified, it skips rows outside the range.
 
-The contents of the filelike object can be in text format or file format (see
-"formats" below). This is usually auto-detected, but a specific format can
-be specified with the ``format`` parameter.  If reading in text format,
-the returned object just has the ``data`` attribute set. If reading in
-file format , the returned object also has attributes ``unit``,
-``title``, ``comment``, ``timezone``, ``time_step``, ``interval_type``,
+The contents of the filelike object can be in text format or file format
+(see "formats" below). This is usually auto-detected, but a specific
+format can be specified with the ``format`` parameter.  If reading in
+text format, the returned object just has the ``data`` attribute set. If
+reading in file format , the returned object also has attributes
+``unit``, ``title``, ``comment``, ``time_step``, ``interval_type``,
 ``variable``, ``precision`` and ``location``. For the meaning of these
 attributes, see section "File format" below.
 
 These attributes are purely informational. In particular, ``time_step``
 and the other time-step-related attributes don't necessarily mean that
 the pandas object will have a related time step (also called
 "frequency"). In fact, raw time series may be irregular but actually
@@ -269,18 +269,21 @@
         Comment=These five lines form two paragraphs.
 
     The Comment parameter is the only parameter where a blank value is
     significant and indicates an empty line, as can be seen in the
     example above.
 
 **Timezone**
-    The time zone of the timestamps, in the format ``{XXX}
-    (UTC{+HHmm})``, where *XXX* is a time zone name and *+HHmm* is the
-    offset from UTC. Examples are ``EET (UTC+0200)`` and ``VST
-    (UTC-0430)``.
+    The time zone of the timestamps, in the format ``{+HHmm}``, where
+    *+HHmm* is the offset from UTC. Examples are ``+0200`` and
+    ``-0430``.
+
+    Format ``{XXX} (UTC{+HHmm})``, where *XXX* is a time zone name, is
+    also supported but deprecated. It exists only in order to be able to
+    read old files.
 
     The ``TzinfoFromString`` utility (described above) can be used to
     convert this string to a tzinfo_ object.
 
 **Time_step**
     In version 5, a pandas "frequency" string such as ``10min`` (10
     minutes), ``H`` (hour), or ``2M`` (two months). If missing or empty,
@@ -399,19 +402,28 @@
 .. _openhi: https://openhi.net
 
 
 =======
 History
 =======
 
+7.0.0 (2024-04-14)
+==================
+
+- When saving in file format, the Timezone= parameter now merely
+  contains +HHmm.
+- The HTimeseries.timezone attribute has been abolished; use
+  HTimeseries.data.index.tz instead.
+- When initialized with a dataframe, it checks that the index is aware.
+
 6.0.3 (2024-03-21)
 ==================
 
-- Fixed error with unspecified time zone in HTimeseries objects created empty.
-  Now creating an empty object with ``HTimeseries()`` assumes
+- Fixed error with unspecified time zone in HTimeseries objects created
+  empty.  Now creating an empty object with ``HTimeseries()`` assumes
   ``default_tzinfo=ZoneInfo("UTC")``.
 
 6.0.2 (2023-12-22)
 ==================
 
 - Fixed crash when reading csv with aware timestamps.
 
@@ -419,19 +431,20 @@
 ==================
 
 - Fixed crash when reading csv with only a date column.
 
 6.0.0 (2023-12-14)
 ==================
 
-- Python 3.9 is now required (the reason for this is that backports.zoneinfo is
-  behaving differently from zoneinfo).
-- Only pandas>=1.5,<2  is now supported. Pandas<1.5 probably did not work in
-  5.0.0 either, but it had not been discovered. Pandas>=2 handles ambiguous
-  times differently and is therefore still unsupported.
+- Python 3.9 is now required (the reason for this is that
+  backports.zoneinfo is behaving differently from zoneinfo).
+- Only pandas>=1.5,<2  is now supported. Pandas<1.5 probably did not
+  work in 5.0.0 either, but it had not been discovered. Pandas>=2
+  handles ambiguous times differently and is therefore still
+  unsupported.
 - Increased CSV reading speed by two orders of magnitude.
 
 5.0.0 (2023-11-21)
 ==================
 
 - Removed compatibility with pandas<1. pandas 1 and 2 are now supported.
   This helps avoid an error when reading a data file spanning a time
```

### Comparing `htimeseries-6.0.3/setup.py` & `htimeseries-7.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `htimeseries-6.0.3/tests/test_htimeseries.py` & `htimeseries-7.0.0/tests/test_htimeseries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime as dt
 import re
 import textwrap
 from configparser import ParsingError
+from copy import copy
 from io import StringIO
 from unittest import TestCase
 from zoneinfo import ZoneInfo
 
 import numpy as np
 import pandas as pd
 from iso8601 import parse_date
@@ -29,15 +30,15 @@
     Count=5\r
     Title=A test 10-min time series\r
     Comment=This timeseries is extremely important\r
     Comment=because the comment that describes it\r
     Comment=spans five lines.\r
     Comment=\r
     Comment=These five lines form two paragraphs.\r
-    Timezone=EET (UTC+0200)\r
+    Timezone=+0200\r
     Time_step=10,0\r
     Variable=temperature\r
     Precision=1\r
     \r
     2008-02-07 11:20,1141.0,\r
     2008-02-07 11:30,1142.0,MISS\r
     2008-02-07 11:40,1154.0,\r
@@ -52,15 +53,15 @@
     Count=5\r
     Title=A test 10-min time series\r
     Comment=This timeseries is extremely important\r
     Comment=because the comment that describes it\r
     Comment=spans five lines.\r
     Comment=\r
     Comment=These five lines form two paragraphs.\r
-    Timezone=EET (UTC+0200)\r
+    Timezone=+0200\r
     Time_step=10,0\r
     Variable=temperature\r
     Precision=1\r
     Location=24.678900 38.123450 4326\r
     Altitude=219.22\r
     \r
     2008-02-07 11:20,1141.0,\r
@@ -77,15 +78,15 @@
     Count=5\r
     Title=A test 10-min time series\r
     Comment=This timeseries is extremely important\r
     Comment=because the comment that describes it\r
     Comment=spans five lines.\r
     Comment=\r
     Comment=These five lines form two paragraphs.\r
-    Timezone=EET (UTC+0200)\r
+    Timezone=+0200\r
     Time_step=10,0\r
     Variable=temperature\r
     Precision=1\r
     Location=24.678900 38.123450 4326\r
     Altitude=219.22\r
     \r
     2008-02-07 11:20,1141.0,\r
@@ -102,15 +103,15 @@
     Count=5\r
     Title=A test 10-min time series\r
     Comment=This timeseries is extremely important\r
     Comment=because the comment that describes it\r
     Comment=spans five lines.\r
     Comment=\r
     Comment=These five lines form two paragraphs.\r
-    Timezone=EET (UTC+0200)\r
+    Timezone=+0200\r
     Time_step=10,0\r
     Variable=temperature\r
     Precision=1\r
     Location=24.678900 38.123450 4326\r
     \r
     2008-02-07 11:20,1141.0,\r
     2008-02-07 11:30,1142.0,MISS\r
@@ -126,15 +127,15 @@
     Count=5\r
     Title=A test 10-min time series\r
     Comment=This timeseries is extremely important\r
     Comment=because the comment that describes it\r
     Comment=spans five lines.\r
     Comment=\r
     Comment=These five lines form two paragraphs.\r
-    Timezone=EET (UTC+0200)\r
+    Timezone=+0200\r
     Time_step=10,0\r
     Variable=temperature\r
     Precision=1\r
     \r
     2008-02-07 11:20,1141.0,\r
     2008-02-07 11:30,1142.0,MISS\r
     2008-02-07 11:40,1154.0,\r
@@ -149,15 +150,15 @@
     Count=5\r
     Title=A test 10-min time series\r
     Comment=This timeseries is extremely important\r
     Comment=because the comment that describes it\r
     Comment=spans five lines.\r
     Comment=\r
     Comment=These five lines form two paragraphs.\r
-    Timezone=EET (UTC+0200)\r
+    Timezone=+0200\r
     Time_step=10,0\r
     Variable=temperature\r
     Location=24.678900 38.123450 4326\r
     Altitude=219.22\r
     \r
     2008-02-07 11:20,1141.000000,\r
     2008-02-07 11:30,1142.010000,MISS\r
@@ -173,15 +174,15 @@
     Count=5\r
     Title=A test 10-min time series\r
     Comment=This timeseries is extremely important\r
     Comment=because the comment that describes it\r
     Comment=spans five lines.\r
     Comment=\r
     Comment=These five lines form two paragraphs.\r
-    Timezone=EET (UTC+0200)\r
+    Timezone=+0200\r
     Time_step=10,0\r
     Variable=temperature\r
     Precision=0\r
     Location=24.678900 38.123450 4326\r
     Altitude=219.22\r
     \r
     2008-02-07 11:20,1141,\r
@@ -199,15 +200,15 @@
     Count=5\r
     Title=A test 10-min time series\r
     Comment=This timeseries is extremely important\r
     Comment=because the comment that describes it\r
     Comment=spans five lines.\r
     Comment=\r
     Comment=These five lines form two paragraphs.\r
-    Timezone=EET (UTC+0200)\r
+    Timezone=+0200\r
     Time_step=10,0\r
     Variable=temperature\r
     Precision=-1\r
     Location=24.678900 38.123450 4326\r
     Altitude=219.22\r
     \r
     2008-02-07 11:20,1140,\r
@@ -216,15 +217,15 @@
     2008-02-07 11:50,,\r
     2008-02-07 12:00,1180,\r
     """
 )
 
 standard_empty_dataframe = pd.DataFrame(
     data={"value": np.array([], dtype=np.float64), "flags": np.array([], dtype=str)},
-    index=pd.DatetimeIndex([], tz=ZoneInfo("Etc/GMT-2")),
+    index=pd.DatetimeIndex([], tz=dt.timezone(dt.timedelta(hours=2))),
     columns=["value", "flags"],
 )
 standard_empty_dataframe.index.name = "date"
 
 
 class HTimeseriesArgumentsTestCase(TestCase):
     def test_raises_on_invalid_argument(self):
@@ -232,36 +233,42 @@
         with self.assertRaisesRegex(TypeError, msg):
             HTimeseries(invalid=42)
 
     def test_raises_if_timezone_unspecified(self):
         with self.assertRaises(TypeError):
             HTimeseries(StringIO(tenmin_test_timeseries))
 
+    def test_raises_if_dataframe_naive(self):
+        df = copy(standard_empty_dataframe)
+        df.index = pd.DatetimeIndex([])  # Replace with a naive index
+        with self.assertRaises(TypeError):
+            HTimeseries(df)
+
 
 class HTimeseriesEmptyTestCase(TestCase):
     def test_read_empty(self):
         s = StringIO()
-        ts = HTimeseries(s, default_tzinfo=ZoneInfo("Etc/GMT-2"))
+        ts = HTimeseries(s, default_tzinfo=dt.timezone(dt.timedelta(hours=2)))
         pd.testing.assert_frame_equal(ts.data, standard_empty_dataframe)
 
     def test_write_empty(self):
-        ts = HTimeseries(default_tzinfo=ZoneInfo("Etc/GMT-2"))
+        ts = HTimeseries(default_tzinfo=dt.timezone(dt.timedelta(hours=2)))
         s = StringIO()
         ts.write(s)
         self.assertEqual(s.getvalue(), "")
 
     def test_create_empty(self):
         pd.testing.assert_frame_equal(
-            HTimeseries(default_tzinfo=ZoneInfo("Etc/GMT-2")).data,
+            HTimeseries(default_tzinfo=dt.timezone(dt.timedelta(hours=2))).data,
             standard_empty_dataframe,
         )
 
     def test_unspecified_default_tzinfo(self):
         ts = HTimeseries()
-        self.assertEqual(ts.data.index.tz, ZoneInfo("UTC"))
+        self.assertEqual(ts.data.index.tz, dt.timezone.utc)
 
 
 class HTimeseriesWriteSimpleTestCase(TestCase):
     def test_write(self):
         anp = np.array(
             [
                 [parse_date("2005-08-23 18:53"), 93, ""],
@@ -296,20 +303,20 @@
             parse_dates=[0],
             usecols=["date", "value", "flags"],
             index_col=0,
             header=None,
             names=("date", "value", "flags"),
             dtype={"value": np.float64, "flags": str},
         ).asfreq("10T")
+        data.index = data.index.tz_localize(dt.timezone(dt.timedelta(hours=2)))
         self.reference_ts = HTimeseries(data=data)
         self.reference_ts.unit = "°C"
         self.reference_ts.title = "A test 10-min time series"
         self.reference_ts.precision = 1
         self.reference_ts.time_step = "10min"
-        self.reference_ts.timezone = "EET (UTC+0200)"
         self.reference_ts.variable = "temperature"
         self.reference_ts.comment = (
             "This timeseries is extremely important\n"
             "because the comment that describes it\n"
             "spans five lines.\n\n"
             "These five lines form two paragraphs."
         )
@@ -410,14 +417,34 @@
         self.reference_ts.precision = -1
         outstring = StringIO()
         self.reference_ts.write(outstring, format=HTimeseries.FILE, version=4)
         self.assertEqual(
             outstring.getvalue(), tenmin_test_timeseries_file_negative_precision
         )
 
+    def test_timezone_utc(self):
+        self.reference_ts.data = self.reference_ts.data.tz_convert(dt.timezone.utc)
+        outstring = StringIO()
+        self.reference_ts.write(outstring, format=HTimeseries.FILE, version=4)
+        self.assertIn("Timezone=+0000\r\n", outstring.getvalue())
+
+    def test_timezone_positive(self):
+        tz = dt.timezone(dt.timedelta(hours=2, minutes=30))
+        self.reference_ts.data = self.reference_ts.data.tz_convert(tz)
+        outstring = StringIO()
+        self.reference_ts.write(outstring, format=HTimeseries.FILE, version=4)
+        self.assertIn("Timezone=+0230\r\n", outstring.getvalue())
+
+    def test_timezone_negative(self):
+        tz = dt.timezone(-dt.timedelta(hours=3, minutes=15))
+        self.reference_ts.data = self.reference_ts.data.tz_convert(tz)
+        outstring = StringIO()
+        self.reference_ts.write(outstring, format=HTimeseries.FILE, version=4)
+        self.assertIn("Timezone=-0315\r\n", outstring.getvalue())
+
 
 class ReadFilelikeTestCaseBase:
     def test_length(self):
         self.assertEqual(len(self.ts.data), 5)
 
     def test_dates(self):
         np.testing.assert_array_equal(
@@ -501,15 +528,15 @@
     def test_metadata_was_read(self):
         self.assertEqual(self.ts.unit, "°C")
 
 
 class HTimeseriesReadFilelikeWithMissingLocationButPresentAltitudeTestCase(TestCase):
     def setUp(self):
         s = StringIO("Altitude=55\n\n")
-        self.ts = HTimeseries(s, default_tzinfo=ZoneInfo("Etc/GMT-2"))
+        self.ts = HTimeseries(s, default_tzinfo=dt.timezone(dt.timedelta(hours=2)))
 
     def test_data_is_empty(self):
         pd.testing.assert_frame_equal(self.ts.data, standard_empty_dataframe)
 
     def test_has_altitude(self):
         self.assertEqual(self.ts.location["altitude"], 55)
 
@@ -636,15 +663,15 @@
                 spans five lines.
 
                 These five lines form two paragraphs."""
             ),
         )
 
     def test_timezone(self):
-        self.assertEqual(self.ts.timezone, "EET (UTC+0200)")
+        self.assertEqual(self.ts.data.index.tz.utcoffset(None), dt.timedelta(hours=2))
 
     def test_time_step(self):
         self.assertEqual(self.ts.time_step, "10min")
 
     def test_variable(self):
         self.assertEqual(self.ts.variable, "temperature")
 
@@ -798,17 +825,18 @@
             parse_dates=[0],
             usecols=["date", "value", "flags"],
             index_col=0,
             header=None,
             names=("date", "value", "flags"),
             dtype={"value": np.float64, "flags": str},
         )
+        data.index = data.index.tz_localize(dt.timezone.utc)
         msg = (
             "Can't write time series: the following timestamps appear more than once: "
-            "2020-02-23 12:00:00, 2020-02-23 13:00:00"
+            r"2020-02-23 12:00:00\+00:00, 2020-02-23 13:00:00\+00:00"
         )
         with self.assertRaisesRegex(ValueError, msg):
             HTimeseries(data).write(StringIO())
 
 
 class HTimeseriesTimeChangeTestCase(TestCase):
     """Test what happens when we read a csv containing a time change.
```

### Comparing `htimeseries-6.0.3/tests/test_timezone_utils.py` & `htimeseries-7.0.0/tests/test_timezone_utils.py`

 * *Files identical despite different names*

