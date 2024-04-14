# Comparing `tmp/swb-5.0.0.tar.gz` & `tmp/swb-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swb-5.0.0.tar", last modified: Fri Aug 13 10:16:37 2021, max compression
+gzip compressed data, was "swb-5.0.1.tar", last modified: Sun Apr 14 12:50:11 2024, max compression
```

## Comparing `swb-5.0.0.tar` & `swb-5.0.1.tar`

### file list

```diff
@@ -1,47 +1,33 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-08-13 10:16:37.367400 swb-5.0.0/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1962 2021-08-13 10:14:36.000000 swb-5.0.0/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      712 2018-12-12 12:59:08.000000 swb-5.0.0/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      217 2018-12-12 09:48:58.000000 swb-5.0.0/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3269 2021-08-13 10:16:37.367400 swb-5.0.0/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      705 2018-12-12 09:48:53.000000 swb-5.0.0/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-08-13 10:16:37.363400 swb-5.0.0/docs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      604 2018-12-12 13:20:33.000000 swb-5.0.0/docs/Makefile
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-08-13 10:16:37.359400 swb-5.0.0/docs/_build/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-08-13 10:16:37.359400 swb-5.0.0/docs/_build/html/
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-08-13 10:16:37.363400 swb-5.0.0/docs/_build/html/_static/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      673 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 anthony   (1000) anthony   (1000)      756 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      829 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      641 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/comment.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      222 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      202 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/down.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      286 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/file.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)       90 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)       90 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      214 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 anthony   (1000) anthony   (1000)      203 2018-10-31 06:52:17.000000 swb-5.0.0/docs/_build/html/_static/up.png
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1185 2020-02-07 14:18:00.000000 swb-5.0.0/docs/conf.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2496 2020-09-24 10:05:30.000000 swb-5.0.0/docs/crop_evapotranspiration.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      804 2020-01-31 16:32:00.000000 swb-5.0.0/docs/effective_precipitation.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      153 2020-01-31 16:32:00.000000 swb-5.0.0/docs/index.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)       24 2018-12-12 12:57:47.000000 swb-5.0.0/docs/license.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12153 2021-08-13 10:14:36.000000 swb-5.0.0/docs/swb.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2021-08-13 10:16:37.367400 swb-5.0.0/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1475 2020-02-07 14:11:23.000000 swb-5.0.0/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-08-13 10:16:37.367400 swb-5.0.0/swb/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      144 2021-08-13 10:15:40.000000 swb-5.0.0/swb/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1839 2020-09-24 10:05:30.000000 swb-5.0.0/swb/crop_evapotranspiration.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)      228 2020-01-31 16:32:00.000000 swb-5.0.0/swb/effective_precipitation.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5302 2021-08-13 10:14:36.000000 swb-5.0.0/swb/swb.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-08-13 10:16:37.367400 swb-5.0.0/swb.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3269 2021-08-13 10:16:37.000000 swb-5.0.0/swb.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      976 2021-08-13 10:16:37.000000 swb-5.0.0/swb.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2021-08-13 10:16:37.000000 swb-5.0.0/swb.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2018-12-12 17:30:00.000000 swb-5.0.0/swb.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       13 2021-08-13 10:16:37.000000 swb-5.0.0/swb.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        4 2021-08-13 10:16:37.000000 swb-5.0.0/swb.egg-info/top_level.txt
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2021-08-13 10:16:37.367400 swb-5.0.0/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2018-12-12 09:58:02.000000 swb-5.0.0/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6204 2020-09-24 10:05:30.000000 swb-5.0.0/tests/test_crop_evapotranspiration.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1000 2020-01-31 16:32:00.000000 swb-5.0.0/tests/test_effective_precipitation.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5626 2021-08-13 10:14:36.000000 swb-5.0.0/tests/test_swb.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 12:50:11.912865 swb-5.0.1/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2104 2024-04-14 12:49:02.000000 swb-5.0.1/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      712 2022-03-05 20:41:03.000000 swb-5.0.1/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      217 2022-03-05 20:41:03.000000 swb-5.0.1/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3419 2024-04-14 12:50:11.912865 swb-5.0.1/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      705 2022-03-05 20:41:03.000000 swb-5.0.1/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 12:50:11.912865 swb-5.0.1/docs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      604 2022-03-05 20:41:03.000000 swb-5.0.1/docs/Makefile
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1185 2022-03-05 20:41:03.000000 swb-5.0.1/docs/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2496 2022-03-05 20:41:03.000000 swb-5.0.1/docs/crop_evapotranspiration.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      804 2022-03-05 20:41:03.000000 swb-5.0.1/docs/effective_precipitation.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      153 2022-03-05 20:41:03.000000 swb-5.0.1/docs/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       24 2022-03-05 20:41:03.000000 swb-5.0.1/docs/license.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    12153 2022-03-05 20:41:03.000000 swb-5.0.1/docs/swb.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-14 12:50:11.912865 swb-5.0.1/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1475 2022-03-05 20:41:03.000000 swb-5.0.1/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 12:50:11.912865 swb-5.0.1/swb/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      144 2024-04-14 12:49:35.000000 swb-5.0.1/swb/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1892 2024-04-14 12:49:02.000000 swb-5.0.1/swb/crop_evapotranspiration.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      228 2022-03-05 20:41:03.000000 swb-5.0.1/swb/effective_precipitation.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5302 2022-03-05 20:41:03.000000 swb-5.0.1/swb/swb.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 12:50:11.912865 swb-5.0.1/swb.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3419 2024-04-14 12:50:11.000000 swb-5.0.1/swb.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      560 2024-04-14 12:50:11.000000 swb-5.0.1/swb.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-14 12:50:11.000000 swb-5.0.1/swb.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-13 21:12:03.000000 swb-5.0.1/swb.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       13 2024-04-14 12:50:11.000000 swb-5.0.1/swb.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        4 2024-04-14 12:50:11.000000 swb-5.0.1/swb.egg-info/top_level.txt
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 12:50:11.912865 swb-5.0.1/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:03.000000 swb-5.0.1/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6914 2024-04-14 12:49:02.000000 swb-5.0.1/tests/test_crop_evapotranspiration.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1000 2022-03-05 20:41:03.000000 swb-5.0.1/tests/test_effective_precipitation.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5626 2022-03-05 20:41:03.000000 swb-5.0.1/tests/test_swb.py
```

### Comparing `swb-5.0.0/HISTORY.rst` & `swb-5.0.1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+5.0.1 (2024-04-14)
+------------------
+
+- ``calculate_crop_evapotranspiration()`` now works with aware (as well
+  as with naive) time series.
+
 5.0.0 (2021-08-13)
 ------------------
 
 - ``mif`` has been renamed to ``refill_factor``.
 
 4.0.0 (2021-05-14)
 ------------------
```

### Comparing `swb-5.0.0/LICENSE` & `swb-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/PKG-INFO` & `swb-5.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: swb
-Version: 5.0.0
+Version: 5.0.1
 Summary: Calculation of soil water balance
 Home-page: https://github.com/openmeteo/swb
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
+Requires-Dist: pandas>=0.20
 
 =======================================
 swb - Calculation of soil water balance
 =======================================
 
 
 .. image:: https://img.shields.io/pypi/v/swb.svg
@@ -38,14 +38,20 @@
 Model for calculation of soil water balance. See https://swb.readthedocs.io.
 
 
 =======
 History
 =======
 
+5.0.1 (2024-04-14)
+------------------
+
+- ``calculate_crop_evapotranspiration()`` now works with aware (as well
+  as with naive) time series.
+
 5.0.0 (2021-08-13)
 ------------------
 
 - ``mif`` has been renamed to ``refill_factor``.
 
 4.0.0 (2021-05-14)
 ------------------
@@ -117,9 +123,7 @@
 - Added model for calculation of crop evapotranspiration from reference
   evapotranspiration.
 
 0.1.0 (2019-03-14)
 ------------------
 
 - Initial release
-
-
```

### Comparing `swb-5.0.0/README.rst` & `swb-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/docs/Makefile` & `swb-5.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/docs/conf.py` & `swb-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/docs/crop_evapotranspiration.rst` & `swb-5.0.1/docs/crop_evapotranspiration.rst`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/docs/effective_precipitation.rst` & `swb-5.0.1/docs/effective_precipitation.rst`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/docs/swb.rst` & `swb-5.0.1/docs/swb.rst`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/setup.py` & `swb-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/swb/crop_evapotranspiration.py` & `swb-5.0.1/swb/crop_evapotranspiration.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,11 +44,11 @@
         kcs = np.linspace(kc_start, stage.kc_end, num=stage.ndays + 1)[1:]
         period_length = len(self.timeseries.loc[start:end, "kc"])
         kcs = kcs[:period_length]
         self.timeseries.loc[start:end, "kc"] = kcs
 
     def _date_to_timestamp(self, date):
         try:
-            time = self.timeseries.index[0].time()
+            time = self.timeseries.index[0].timetz()
         except IndexError:
-            time = dt.time(0, 0)
+            time = dt.time(0, 0, tzinfo=getattr(self.timeseries.index, "tz", None))
         return dt.datetime.combine(date, time)
```

### Comparing `swb-5.0.0/swb/swb.py` & `swb-5.0.1/swb/swb.py`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/swb.egg-info/PKG-INFO` & `swb-5.0.1/swb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: swb
-Version: 5.0.0
+Version: 5.0.1
 Summary: Calculation of soil water balance
 Home-page: https://github.com/openmeteo/swb
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
+Requires-Dist: pandas>=0.20
 
 =======================================
 swb - Calculation of soil water balance
 =======================================
 
 
 .. image:: https://img.shields.io/pypi/v/swb.svg
@@ -38,14 +38,20 @@
 Model for calculation of soil water balance. See https://swb.readthedocs.io.
 
 
 =======
 History
 =======
 
+5.0.1 (2024-04-14)
+------------------
+
+- ``calculate_crop_evapotranspiration()`` now works with aware (as well
+  as with naive) time series.
+
 5.0.0 (2021-08-13)
 ------------------
 
 - ``mif`` has been renamed to ``refill_factor``.
 
 4.0.0 (2021-05-14)
 ------------------
@@ -117,9 +123,7 @@
 - Added model for calculation of crop evapotranspiration from reference
   evapotranspiration.
 
 0.1.0 (2019-03-14)
 ------------------
 
 - Initial release
-
-
```

### Comparing `swb-5.0.0/tests/test_crop_evapotranspiration.py` & `swb-5.0.1/tests/test_crop_evapotranspiration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime as dt
+import warnings
 from unittest import TestCase
 
 import numpy as np
 import pandas as pd
 
 from swb import KcStage, calculate_crop_evapotranspiration
 
@@ -152,14 +153,33 @@
 ):
     """Test case for timeseries that end in a time different from 00:00."""
 
     def _get_date(self, datestr):
         return datestr + " 23:59"
 
 
+class WithAwareTimestampsTestCase(CalculateCropEvapotranspirationTestMixin, TestCase):
+    """Test case for timeseries that have aware timestamps."""
+
+    def setUp(self):
+        super().setUp()
+        # Pandas throws a warning if we try to index an aware timeseries with a naive
+        # index. We convert warnings into errors in order for the test to fail if
+        # this happends.
+        warnings.filterwarnings("error")
+
+    def tearDown(self):
+        warnings.resetwarnings()
+        super().tearDown()
+
+    def _get_date(self, datestr):
+        y, m, d = [int(x) for x in datestr.split("-")]
+        return dt.datetime(y, m, d, 23, 59, tzinfo=dt.timezone(dt.timedelta(hours=2)))
+
+
 class EmptyTimeseriesTestCase(TestCase):
     def setUp(self):
         self.timeseries = pd.DataFrame(data={"ref_evapotranspiration": []}, index=[])
         calculate_crop_evapotranspiration(
             timeseries=self.timeseries,
             planting_date=dt.date(1974, 5, 22),
             kc_offseason=0.1,
```

### Comparing `swb-5.0.0/tests/test_effective_precipitation.py` & `swb-5.0.1/tests/test_effective_precipitation.py`

 * *Files identical despite different names*

### Comparing `swb-5.0.0/tests/test_swb.py` & `swb-5.0.1/tests/test_swb.py`

 * *Files identical despite different names*

