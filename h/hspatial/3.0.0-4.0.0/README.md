# Comparing `tmp/hspatial-3.0.0.tar.gz` & `tmp/hspatial-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspatial-3.0.0.tar", last modified: Mon Apr  1 05:29:25 2024, max compression
+gzip compressed data, was "hspatial-4.0.0.tar", last modified: Sun Apr 14 14:16:40 2024, max compression
```

## Comparing `hspatial-3.0.0.tar` & `hspatial-4.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 05:29:25.170979 hspatial-3.0.0/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3431 2024-04-01 05:26:15.000000 hspatial-3.0.0/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      710 2022-03-05 20:41:09.000000 hspatial-3.0.0/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:09.000000 hspatial-3.0.0/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5006 2024-04-01 05:29:25.170979 hspatial-3.0.0/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      723 2022-03-05 20:41:09.000000 hspatial-3.0.0/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 05:29:25.166979 hspatial-3.0.0/docs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9209 2022-03-05 20:41:09.000000 hspatial-3.0.0/docs/api.rst
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1370 2022-03-05 20:41:09.000000 hspatial-3.0.0/docs/conf.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:09.000000 hspatial-3.0.0/docs/history.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      214 2022-03-05 20:41:09.000000 hspatial-3.0.0/docs/index.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1013 2022-03-05 20:41:09.000000 hspatial-3.0.0/docs/testutils.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5336 2022-03-05 20:41:09.000000 hspatial-3.0.0/docs/usage.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 05:29:25.170979 hspatial-3.0.0/hspatial/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      141 2024-04-01 05:28:37.000000 hspatial-3.0.0/hspatial/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    10333 2022-03-05 20:41:09.000000 hspatial-3.0.0/hspatial/cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    14843 2024-04-01 05:23:57.000000 hspatial-3.0.0/hspatial/hspatial.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1023 2022-03-05 20:41:09.000000 hspatial-3.0.0/hspatial/test.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 05:29:25.170979 hspatial-3.0.0/hspatial.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5006 2024-04-01 05:29:24.000000 hspatial-3.0.0/hspatial.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      512 2024-04-01 05:29:25.000000 hspatial-3.0.0/hspatial.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-01 05:29:24.000000 hspatial-3.0.0/hspatial.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       49 2024-04-01 05:29:24.000000 hspatial-3.0.0/hspatial.egg-info/entry_points.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-03-31 20:38:47.000000 hspatial-3.0.0/hspatial.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       84 2024-04-01 05:29:24.000000 hspatial-3.0.0/hspatial.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        9 2024-04-01 05:29:24.000000 hspatial-3.0.0/hspatial.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-01 05:29:25.170979 hspatial-3.0.0/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1711 2024-04-01 05:23:57.000000 hspatial-3.0.0/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 05:29:25.170979 hspatial-3.0.0/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:09.000000 hspatial-3.0.0/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    23026 2022-03-05 20:41:09.000000 hspatial-3.0.0/tests/test_cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    27329 2024-04-01 05:23:57.000000 hspatial-3.0.0/tests/test_hspatial.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 14:16:40.523608 hspatial-4.0.0/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3577 2024-04-14 13:42:15.000000 hspatial-4.0.0/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      710 2022-03-05 20:41:09.000000 hspatial-4.0.0/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:09.000000 hspatial-4.0.0/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5152 2024-04-14 14:16:40.523608 hspatial-4.0.0/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      723 2022-03-05 20:41:09.000000 hspatial-4.0.0/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 14:16:40.523608 hspatial-4.0.0/docs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9376 2024-04-13 14:14:35.000000 hspatial-4.0.0/docs/api.rst
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1370 2022-03-05 20:41:09.000000 hspatial-4.0.0/docs/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:09.000000 hspatial-4.0.0/docs/history.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      214 2022-03-05 20:41:09.000000 hspatial-4.0.0/docs/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1013 2022-03-05 20:41:09.000000 hspatial-4.0.0/docs/testutils.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5336 2022-03-05 20:41:09.000000 hspatial-4.0.0/docs/usage.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 14:16:40.523608 hspatial-4.0.0/hspatial/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      141 2024-04-14 14:15:49.000000 hspatial-4.0.0/hspatial/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    10333 2022-03-05 20:41:09.000000 hspatial-4.0.0/hspatial/cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15422 2024-04-14 14:13:33.000000 hspatial-4.0.0/hspatial/hspatial.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1023 2022-03-05 20:41:09.000000 hspatial-4.0.0/hspatial/test.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 14:16:40.523608 hspatial-4.0.0/hspatial.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5152 2024-04-14 14:16:40.000000 hspatial-4.0.0/hspatial.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      512 2024-04-14 14:16:40.000000 hspatial-4.0.0/hspatial.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-14 14:16:40.000000 hspatial-4.0.0/hspatial.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       49 2024-04-14 14:16:40.000000 hspatial-4.0.0/hspatial.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-03-31 20:38:47.000000 hspatial-4.0.0/hspatial.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       84 2024-04-14 14:16:40.000000 hspatial-4.0.0/hspatial.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        9 2024-04-14 14:16:40.000000 hspatial-4.0.0/hspatial.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-14 14:16:40.523608 hspatial-4.0.0/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1711 2024-04-13 14:27:03.000000 hspatial-4.0.0/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 14:16:40.523608 hspatial-4.0.0/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:09.000000 hspatial-4.0.0/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    23026 2022-03-05 20:41:09.000000 hspatial-4.0.0/tests/test_cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    29125 2024-04-14 14:08:06.000000 hspatial-4.0.0/tests/test_hspatial.py
```

### Comparing `hspatial-3.0.0/HISTORY.rst` & `hspatial-4.0.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+4.0.0 (2024-04-14)
+==================
+
+- Now works with htimeseries 6 and 7.
+- PointTimeseries() has changed in that default_time must be aware.
+
 3.0.0 (2024-04-01)
 ==================
 
 - Now requires htimeseries 6. This recent htimeseries version works with
   aware time zones, and hspatial, which works with naive, internally
   handles them as UTC.
```

### Comparing `hspatial-3.0.0/LICENSE` & `hspatial-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/PKG-INFO` & `hspatial-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspatial
-Version: 3.0.0
+Version: 4.0.0
 Summary: Utilities for spatial integration of time series
 Home-page: https://github.com/openmeteo/hspatial
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: hspatial
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Click>=7.0
 Requires-Dist: iso8601
-Requires-Dist: htimeseries<7,>=6
+Requires-Dist: htimeseries<8,>=6
 Requires-Dist: affine
 Requires-Dist: simpletail
 Requires-Dist: gdal<4,>=1.10
 Requires-Dist: django<4,>=2.2
 
 ========
 hspatial
@@ -49,14 +49,20 @@
 * Documentation: https://hspatial.readthedocs.io.
 
 
 =======
 History
 =======
 
+4.0.0 (2024-04-14)
+==================
+
+- Now works with htimeseries 6 and 7.
+- PointTimeseries() has changed in that default_time must be aware.
+
 3.0.0 (2024-04-01)
 ==================
 
 - Now requires htimeseries 6. This recent htimeseries version works with
   aware time zones, and hspatial, which works with naive, internally
   handles them as UTC.
```

### Comparing `hspatial-3.0.0/README.rst` & `hspatial-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/docs/api.rst` & `hspatial-4.0.0/docs/api.rst`

 * *Files 5% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
    *point* and *data_source* need not be in the same reference system,
    but they must both have an appropriate spatial reference defined.
 
    If the *point* does not fall in the raster, :exc:`RuntimeError` is
    raised.
 
-.. class:: hspatial.PointTimeseries(point, filenames=None, prefix=None, date_fmt=None, start_date=None, end_date=None, default_time=dt.time(0, 0))
+.. class:: hspatial.PointTimeseries(point, filenames=None, prefix=None, date_fmt=None, start_date=None, end_date=None, default_time=dt.time(0, 0, tzinfo=dt.timezone.utc))
 
    A class that can extract a point timeseries from a set of rasters.
 
    The set of rasters is specified either with *filenames* or with
    *prefix*.  Exactly one of these must be ``None``. *filenames*, if
    specified, must be a sequence or set of names of raster files which
    should contain the same variable in different times; for example, the
@@ -136,15 +136,17 @@
 
    If *start_date* or *end_date* are specified, only that part of the
    time series is read from the rasters. This is only valid when the
    class has been initialized with a prefix (not with a list of
    filenames).
 
    If the ``TIMESTAMP`` GDAL metadata item of the raster does not
-   contain a time, then *default_time* is assumed.
+   contain a time, then *default_time* is assumed. *default_time* must
+   be aware. If ``TIMESTAMP`` does contain a time, but not a time zone,
+   then the time zone from *default_time* is used.
 
    .. method:: hspatial.PointTimeseries.get()
 
       Extracts and returns a HTimeseries_ object that corresponds to the
       values of the point in the rasters.
 
       Usage example::
```

### Comparing `hspatial-3.0.0/docs/conf.py` & `hspatial-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/docs/testutils.rst` & `hspatial-4.0.0/docs/testutils.rst`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/docs/usage.rst` & `hspatial-4.0.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/hspatial/cli.py` & `hspatial-4.0.0/hspatial/cli.py`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/hspatial/hspatial.py` & `hspatial-4.0.0/hspatial/hspatial.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,17 @@
         target_sr.SetAxisMappingStrategy(osr.OAMS_TRADITIONAL_GIS_ORDER)
     transform = osr.CoordinateTransformation(source_sr, target_sr)
 
     layer = data_source.CreateLayer("stations", target_sr)
     layer.CreateField(ogr.FieldDefn("filename", ogr.OFTString))
     for filename in filenames:
         with open(filename, newline="\n") as f:
-            ts = HTimeseries(f, default_tzinfo=dt.UTC)
+            # The default_tzinfo doesn't matter because we don't care about the data,
+            # we only use the location.
+            ts = HTimeseries(f, default_tzinfo=dt.timezone.utc)
         point = ogr.Geometry(ogr.wkbPoint)
         point.AddPoint(ts.location["abscissa"], ts.location["ordinate"])
         point.Transform(transform)
         f = ogr.Feature(layer.GetLayerDefn())
         f.SetGeometry(point)
         f.SetField("filename", filename)
         layer.CreateFeature(f)
@@ -292,37 +294,43 @@
         filenames = kwargs.pop("filenames", None)
         self.prefix = kwargs.pop("prefix", None)
         assert filenames is None or self.prefix is None
         assert filenames is not None or self.prefix is not None
         self.date_fmt = kwargs.pop("date_fmt", None)
         self.start_date = kwargs.pop("start_date", None)
         self.end_date = kwargs.pop("end_date", None)
-        self.default_time = kwargs.pop("default_time", dt.time(0, 0, tzinfo=dt.UTC))
-        if self.start_date:
-            self.start_date = self.start_date.replace(tzinfo=dt.UTC)
-        if self.end_date:
-            self.end_date = self.end_date.replace(tzinfo=dt.UTC)
+        self.default_time = kwargs.pop(
+            "default_time", dt.time(0, 0, tzinfo=dt.timezone.utc)
+        )
+        if self.default_time.tzinfo is None:
+            raise TypeError("default_time must be aware")
+        if self.start_date and self.start_date.tzinfo is None:
+            self.start_date = self.start_date.replace(tzinfo=self.default_time.tzinfo)
+        if self.end_date and self.end_date.tzinfo is None:
+            self.end_date = self.end_date.replace(tzinfo=self.default_time.tzinfo)
         self.filenames = self._get_filenames(filenames)
 
     def _get_filenames(self, filenames):
         if self.prefix is None:
             return filenames
         filenames = glob(self.prefix + "-*.tif")
-        self.filename_format = FilenameWithDateFormat(self.prefix, self.date_fmt)
+        self.filename_format = FilenameWithDateFormat(
+            self.prefix, date_fmt=self.date_fmt, tzinfo=self.default_time.tzinfo
+        )
         result = []
         for filename in filenames:
             date = self.filename_format.get_date(filename)
             is_after_start_date = (self.start_date is None) or (date >= self.start_date)
             is_before_end_date = (self.end_date is None) or (date <= self.end_date)
             if is_after_start_date and is_before_end_date:
                 result.append(filename)
         return result
 
     def get(self):
-        result = HTimeseries()
+        result = HTimeseries(default_tzinfo=self.default_time.tzinfo)
         for filename in self.filenames:
             f = gdal.Open(filename)
             try:
                 timestamp = self._get_timestamp(f)
                 self._get_unit_of_measurement(f, result)
                 value = extract_point_from_raster(self.point, f)
                 result.data.loc[timestamp, "value"] = value
@@ -330,15 +338,17 @@
             finally:
                 f = None
         result.data = result.data.sort_index()
         return result
 
     def _get_timestamp(self, f):
         isostring = f.GetMetadata()["TIMESTAMP"]
-        timestamp = iso8601.parse_date(isostring, default_timezone=dt.UTC)
+        timestamp = iso8601.parse_date(
+            isostring, default_timezone=self.default_time.tzinfo
+        )
         if len(isostring) <= 10:
             timestamp = dt.datetime.combine(timestamp.date(), self.default_time)
         return timestamp
 
     def _get_unit_of_measurement(self, f, ahtimeseries):
         if hasattr(ahtimeseries, "unit"):
             return
@@ -359,30 +369,31 @@
         if force or not os.path.exists(dest):
             return None
         else:
             return self._get_timeseries_if_file_is_up_to_date_else_none(dest)
 
     def _get_timeseries_if_file_is_up_to_date_else_none(self, dest):
         with open(dest, "r", newline="") as f:
-            ts = HTimeseries(f, default_tzinfo=dt.UTC)
+            ts = HTimeseries(f, default_tzinfo=self.default_time.tzinfo)
         for filename in self.filenames:
             if not self.filename_format.get_date(filename) in ts.data.index:
                 return None
         return ts
 
 
 class FilenameWithDateFormat:
-    def __init__(self, prefix, date_fmt=None):
+    def __init__(self, prefix, *, date_fmt=None, tzinfo):
         self.prefix = prefix
         self.date_fmt = date_fmt
+        self.tzinfo = tzinfo
 
     def get_date(self, filename):
         datestr = self._extract_datestr(filename)
         self._ensure_we_have_date_fmt(datestr)
-        return dt.datetime.strptime(datestr, self.date_fmt).replace(tzinfo=dt.UTC)
+        return dt.datetime.strptime(datestr, self.date_fmt).replace(tzinfo=self.tzinfo)
 
     def _ensure_we_have_date_fmt(self, datestr):
         if self.date_fmt is not None:
             pass
         elif datestr.count("-") == 4:
             self.date_fmt = "%Y-%m-%d-%H-%M"
         elif datestr.count("-") == 2:
```

### Comparing `hspatial-3.0.0/hspatial/test.py` & `hspatial-4.0.0/hspatial/test.py`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/hspatial.egg-info/PKG-INFO` & `hspatial-4.0.0/hspatial.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspatial
-Version: 3.0.0
+Version: 4.0.0
 Summary: Utilities for spatial integration of time series
 Home-page: https://github.com/openmeteo/hspatial
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: hspatial
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,15 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Click>=7.0
 Requires-Dist: iso8601
-Requires-Dist: htimeseries<7,>=6
+Requires-Dist: htimeseries<8,>=6
 Requires-Dist: affine
 Requires-Dist: simpletail
 Requires-Dist: gdal<4,>=1.10
 Requires-Dist: django<4,>=2.2
 
 ========
 hspatial
@@ -49,14 +49,20 @@
 * Documentation: https://hspatial.readthedocs.io.
 
 
 =======
 History
 =======
 
+4.0.0 (2024-04-14)
+==================
+
+- Now works with htimeseries 6 and 7.
+- PointTimeseries() has changed in that default_time must be aware.
+
 3.0.0 (2024-04-01)
 ==================
 
 - Now requires htimeseries 6. This recent htimeseries version works with
   aware time zones, and hspatial, which works with naive, internally
   handles them as UTC.
```

### Comparing `hspatial-3.0.0/hspatial.egg-info/SOURCES.txt` & `hspatial-4.0.0/hspatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/setup.py` & `hspatial-4.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
 requirements = [
     "Click>=7.0",
     "iso8601",
-    "htimeseries>=6,<7",
+    "htimeseries>=6,<8",
     "affine",
     "simpletail",
     "gdal>=1.10,<4",
     "django>=2.2,<4",
 ]
 
 test_requirements = []
```

### Comparing `hspatial-3.0.0/tests/test_cli.py` & `hspatial-4.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hspatial-3.0.0/tests/test_hspatial.py` & `hspatial-4.0.0/tests/test_hspatial.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from osgeo import gdal, ogr, osr
 
 import hspatial
 from hspatial.test import setup_test_raster
 
 gdal.UseExceptions()
 
+UTC_PLUS_2 = dt.timezone(dt.timedelta(hours=2))
+
 
 def add_point_to_layer(layer, x, y, value):
     p = ogr.Geometry(ogr.wkbPoint)
     p.AddPoint(x, y)
     f = ogr.Feature(layer.GetLayerDefn())
     f.SetGeometry(p)
     f.SetField("value", value)
@@ -68,15 +70,14 @@
         )
         self.assertAlmostEqual(
             hspatial.idw(self.point, self.data_layer, alpha=2.0), 64.188, places=3
         )
 
 
 class IntegrateTestCase(TestCase):
-
     # The calculations for this test have been made manually in
     # data/spatial_calculations.ods, tab test_integrate_idw.
 
     def setUp(self):
         # We will test on a 7x15 grid
         self.mask = np.zeros((7, 15), np.int8)
         self.mask[3, 3] = 1
@@ -498,67 +499,86 @@
         if self.include_time:
             result += "-16-1"
         result += ".tif"
         return os.path.join(self.tempdir, result)
 
     def _create_timestamp(self, date):
         if self.include_time:
-            return dt.datetime.combine(date, dt.time(16, 1))
+            return dt.datetime.combine(date, dt.time(16, 1, tzinfo=UTC_PLUS_2))
         else:
             return date
 
     def _check_against_expected(self, ts):
         expected = pd.DataFrame(
             data={"value": [2.2, 22.1, 220.1], "flags": ["", "", ""]},
             index=self.expected_index,
             columns=["value", "flags"],
         )
         expected.index.name = "date"
-        pd.testing.assert_frame_equal(ts.data, expected)
+        self.assertEqual(
+            ts.data.index.tz.utcoffset(None), expected.index.tz.utcoffset(None)
+        )
+        pd.testing.assert_frame_equal(ts.data, expected, check_index_type=False)
 
     @property
     def expected_index(self):
         hour, minute = self.include_time and (16, 1) or (23, 58)
         return [
-            dt.datetime(2014, 11, 21, hour, minute, tzinfo=dt.UTC),
-            dt.datetime(2014, 11, 22, hour, minute, tzinfo=dt.UTC),
-            dt.datetime(2014, 11, 23, hour, minute, tzinfo=dt.UTC),
+            dt.datetime(2014, 11, 21, hour, minute, tzinfo=UTC_PLUS_2),
+            dt.datetime(2014, 11, 22, hour, minute, tzinfo=UTC_PLUS_2),
+            dt.datetime(2014, 11, 23, hour, minute, tzinfo=UTC_PLUS_2),
         ]
 
 
 class PointTimeseriesGetTestCase(SetupTestRastersMixin, TestCase):
     def test_with_list_of_files(self):
         # Use co-ordinates almost to the common corner of the four lower left points,
         # and only a little bit towards the center.
         point = hspatial.coordinates2point(22.01001, 37.98001)
         filenames = [
             os.path.join(self.tempdir, "test-2014-11-22-16-1.tif"),
             os.path.join(self.tempdir, "test-2014-11-21-16-1.tif"),
             os.path.join(self.tempdir, "test-2014-11-23-16-1.tif"),
         ]
-        ts = hspatial.PointTimeseries(point, filenames=filenames).get()
+        ts = hspatial.PointTimeseries(
+            point, filenames=filenames, default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2)
+        ).get()
         self._check_against_expected(ts)
 
+    def test_raises_when_no_timezone(self):
+        point = hspatial.coordinates2point(22.01001, 37.98001)
+        filenames = [os.path.join(self.tempdir, "test-2014-11-22-16-1.tif")]
+        with self.assertRaises(TypeError):
+            hspatial.PointTimeseries(
+                point, filenames=filenames, default_time=dt.time(0, 0)
+            )
+
     def test_with_prefix(self):
         # Same as test_with_list_of_files(), but with prefix.
         point = hspatial.coordinates2point(22.01001, 37.98001)
         prefix = os.path.join(self.tempdir, "test")
-        ts = hspatial.PointTimeseries(point, prefix=prefix).get()
+        ts = hspatial.PointTimeseries(
+            point, prefix=prefix, default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2)
+        ).get()
         self._check_against_expected(ts)
 
     def test_with_prefix_and_geodjango(self):
         point = hspatial.coordinates2point(22.01001, 37.98001)
         prefix = os.path.join(self.tempdir, "test")
-        ts = hspatial.PointTimeseries(point, prefix=prefix).get()
+        ts = hspatial.PointTimeseries(
+            point, prefix=prefix, default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2)
+        ).get()
         self._check_against_expected(ts)
 
     def test_unit_of_measurement(self):
         point = hspatial.coordinates2point(22.01001, 37.98001)
         prefix = os.path.join(self.tempdir, "test")
-        ts = hspatial.PointTimeseries(point, prefix=prefix).get()
+        ts = hspatial.PointTimeseries(
+            point, prefix=prefix, default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2)
+        ).get()
         self.assertEqual(ts.unit, "microkernels")
 
 
 class PointTimeseriesGetDailyTestCase(SetupTestRastersMixin, TestCase):
     include_time = False
 
     def test_with_list_of_files(self):
@@ -567,138 +587,170 @@
         point = hspatial.coordinates2point(22.01001, 37.98001)
         filenames = [
             os.path.join(self.tempdir, "test-2014-11-22.tif"),
             os.path.join(self.tempdir, "test-2014-11-21.tif"),
             os.path.join(self.tempdir, "test-2014-11-23.tif"),
         ]
         ts = hspatial.PointTimeseries(
-            point, filenames=filenames, default_time=dt.time(23, 58, tzinfo=dt.UTC)
+            point, filenames=filenames, default_time=dt.time(23, 58, tzinfo=UTC_PLUS_2)
         ).get()
         self._check_against_expected(ts)
 
     def test_with_prefix(self):
         # Same as test_with_list_of_files(), but with prefix.
         point = hspatial.coordinates2point(22.01001, 37.98001)
         prefix = os.path.join(self.tempdir, "test")
         ts = hspatial.PointTimeseries(
-            point, prefix=prefix, default_time=dt.time(23, 58, tzinfo=dt.UTC)
+            point, prefix=prefix, default_time=dt.time(23, 58, tzinfo=UTC_PLUS_2)
         ).get()
         self._check_against_expected(ts)
 
     def test_with_prefix_and_geodjango(self):
         point = GeoDjangoPoint(22.01001, 37.98001)
         prefix = os.path.join(self.tempdir, "test")
         ts = hspatial.PointTimeseries(
-            point, prefix=prefix, default_time=dt.time(23, 58, tzinfo=dt.UTC)
+            point, prefix=prefix, default_time=dt.time(23, 58, tzinfo=UTC_PLUS_2)
         ).get()
         self._check_against_expected(ts)
 
 
 class PointTimeseriesGetCachedTestCase(SetupTestRastersMixin, TestCase):
     def setUp(self):
         super().setUp()
         self.point = hspatial.coordinates2point(22.01001, 37.98001)
         self.prefix = os.path.join(self.tempdir, "test")
         self.dest = os.path.join(self.tempdir, "dest.hts")
 
     def test_result(self):
-        result = hspatial.PointTimeseries(self.point, prefix=self.prefix).get_cached(
-            self.dest
-        )
+        result = hspatial.PointTimeseries(
+            self.point,
+            prefix=self.prefix,
+            default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
+        ).get_cached(self.dest)
         self._check_against_expected(result)
 
     def test_file(self):
-        hspatial.PointTimeseries(self.point, prefix=self.prefix).get_cached(self.dest)
+        hspatial.PointTimeseries(
+            self.point,
+            prefix=self.prefix,
+            default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
+        ).get_cached(self.dest)
         with open(self.dest, "r", newline="\n") as f:
-            self._check_against_expected(HTimeseries(f, default_tzinfo=dt.UTC))
+            self._check_against_expected(HTimeseries(f, default_tzinfo=UTC_PLUS_2))
 
     def test_version(self):
-        hspatial.PointTimeseries(self.point, prefix=self.prefix).get_cached(
-            self.dest, version=2
-        )
+        hspatial.PointTimeseries(
+            self.point,
+            prefix=self.prefix,
+            default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
+        ).get_cached(self.dest, version=2)
         with open(self.dest, "r") as f:
             first_line = f.readline()
         self.assertEqual(first_line, "Version=2\n")
 
     def test_file_is_not_recreated(self):
-        hspatial.PointTimeseries(self.point, prefix=self.prefix).get_cached(self.dest)
+        hspatial.PointTimeseries(
+            self.point,
+            prefix=self.prefix,
+            default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
+        ).get_cached(self.dest)
 
         # Make existing file read-only
         os.chmod(self.dest, S_IREAD | S_IRGRP | S_IROTH)
 
         # Try again—it shouldn't try to write, therefore it shouldn't raise exception
-        hspatial.PointTimeseries(self.point, prefix=self.prefix).get_cached(self.dest)
+        hspatial.PointTimeseries(
+            self.point,
+            prefix=self.prefix,
+            default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
+        ).get_cached(self.dest)
         with open(self.dest, "r", newline="\n") as f:
-            self._check_against_expected(HTimeseries(f, default_tzinfo=dt.UTC))
+            self._check_against_expected(HTimeseries(f, default_tzinfo=UTC_PLUS_2))
 
     def test_file_is_recreated_when_out_of_date(self):
-        hspatial.PointTimeseries(self.point, prefix=self.prefix).get_cached(self.dest)
+        hspatial.PointTimeseries(
+            self.point,
+            prefix=self.prefix,
+            default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
+        ).get_cached(self.dest)
         self._setup_additional_raster()
 
         # Make existing file read-only
         os.chmod(self.dest, S_IREAD | S_IRGRP | S_IROTH)
 
         # Try again—it should raise exception
         with self.assertRaises(PermissionError):
-            hspatial.PointTimeseries(self.point, prefix=self.prefix).get_cached(
-                self.dest
-            )
+            hspatial.PointTimeseries(
+                self.point,
+                prefix=self.prefix,
+                default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
+            ).get_cached(self.dest)
 
     def _setup_additional_raster(self):
         filename = os.path.join(self.tempdir, "test-2014-11-24-16-1.tif")
         setup_test_raster(
             filename,
             np.array(
                 [[110.1, 120.1, 130.1], [210.1, 220.1, 230.1], [310.1, 320.1, 330.1]]
             ),
             dt.datetime(2014, 11, 24, 16, 1),
         )
 
     def test_start_date(self):
         start_date = dt.datetime(2014, 11, 22, 16, 1)
         result = hspatial.PointTimeseries(
-            self.point, prefix=self.prefix, start_date=start_date
+            self.point,
+            prefix=self.prefix,
+            start_date=start_date,
+            default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
         ).get_cached(self.dest)
-        self.assertEqual(result.data.index[0], start_date.replace(tzinfo=dt.UTC))
+        self.assertEqual(result.data.index[0], start_date.replace(tzinfo=UTC_PLUS_2))
 
     def test_end_date(self):
         end_date = dt.datetime(2014, 11, 22, 16, 1)
         result = hspatial.PointTimeseries(
-            self.point, prefix=self.prefix, end_date=end_date
+            self.point,
+            prefix=self.prefix,
+            end_date=end_date,
+            default_time=dt.time(0, 0, tzinfo=UTC_PLUS_2),
         ).get_cached(self.dest)
-        self.assertEqual(result.data.index[-1], end_date.replace(tzinfo=dt.UTC))
+        self.assertEqual(result.data.index[-1], end_date.replace(tzinfo=UTC_PLUS_2))
 
 
 class FilenameWithDateFormatTestCase(TestCase):
     def test_with_given_datetime_format(self):
-        format = hspatial.FilenameWithDateFormat("myprefix", "%d-%m-%Y-%H-%M")
+        format = hspatial.FilenameWithDateFormat(
+            "myprefix", date_fmt="%d-%m-%Y-%H-%M", tzinfo=UTC_PLUS_2
+        )
         self.assertEqual(
             format.get_date("myprefix-4-8-2019-10-41.tif"),
-            dt.datetime(2019, 8, 4, 10, 41, tzinfo=dt.UTC),
+            dt.datetime(2019, 8, 4, 10, 41, tzinfo=UTC_PLUS_2),
         )
 
     def test_with_given_date_format(self):
-        format = hspatial.FilenameWithDateFormat("myprefix", "%d-%m-%Y")
+        format = hspatial.FilenameWithDateFormat(
+            "myprefix", date_fmt="%d-%m-%Y", tzinfo=UTC_PLUS_2
+        )
         self.assertEqual(
             format.get_date("myprefix-4-8-2019.tif"),
-            dt.datetime(2019, 8, 4, tzinfo=dt.UTC),
+            dt.datetime(2019, 8, 4, tzinfo=UTC_PLUS_2),
         )
 
     def test_datetime_with_auto_format(self):
-        format = hspatial.FilenameWithDateFormat("myprefix")
+        format = hspatial.FilenameWithDateFormat("myprefix", tzinfo=UTC_PLUS_2)
         self.assertEqual(
             format.get_date("myprefix-2019-8-4-10-41.tif"),
-            dt.datetime(2019, 8, 4, 10, 41, tzinfo=dt.UTC),
+            dt.datetime(2019, 8, 4, 10, 41, tzinfo=UTC_PLUS_2),
         )
 
     def test_date_with_auto_format(self):
-        format = hspatial.FilenameWithDateFormat("myprefix")
+        format = hspatial.FilenameWithDateFormat("myprefix", tzinfo=UTC_PLUS_2)
         self.assertEqual(
             format.get_date("myprefix-2019-8-4.tif"),
-            dt.datetime(2019, 8, 4, tzinfo=dt.UTC),
+            dt.datetime(2019, 8, 4, tzinfo=UTC_PLUS_2),
         )
 
 
 class PassepartoutPointTestCase(TestCase):
     def test_transform_does_not_modify_srid_of_gdal_point(self):
         pppoint = hspatial.PassepartoutPoint(
             hspatial.coordinates2point(324651, 4205742, srid=2100)
```

