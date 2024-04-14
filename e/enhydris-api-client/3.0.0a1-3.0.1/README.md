# Comparing `tmp/enhydris-api-client-3.0.0a1.tar.gz` & `tmp/enhydris-api-client-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhydris-api-client-3.0.0a1.tar", last modified: Fri Nov  4 19:03:31 2022, max compression
+gzip compressed data, was "enhydris-api-client-3.0.1.tar", last modified: Sun Apr 14 15:04:41 2024, max compression
```

## Comparing `enhydris-api-client-3.0.0a1.tar` & `enhydris-api-client-3.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-11-04 19:03:31.954406 enhydris-api-client-3.0.0a1/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1653 2022-11-04 18:59:03.000000 enhydris-api-client-3.0.0a1/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      828 2022-03-25 09:49:03.000000 enhydris-api-client-3.0.0a1/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      143 2022-03-25 09:49:03.000000 enhydris-api-client-3.0.0a1/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8352 2022-11-04 19:03:31.954406 enhydris-api-client-3.0.0a1/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4425 2022-11-01 10:14:28.000000 enhydris-api-client-3.0.0a1/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-11-04 19:03:31.954406 enhydris-api-client-3.0.0a1/enhydris_api_client/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8891 2022-10-31 21:17:39.000000 enhydris-api-client-3.0.0a1/enhydris_api_client/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-11-04 19:03:31.954406 enhydris-api-client-3.0.0a1/enhydris_api_client.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8352 2022-11-04 19:03:31.000000 enhydris-api-client-3.0.0a1/enhydris_api_client.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      525 2022-11-04 19:03:31.000000 enhydris-api-client-3.0.0a1/enhydris_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-04 19:03:31.000000 enhydris-api-client-3.0.0a1/enhydris_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-10-30 07:17:25.000000 enhydris-api-client-3.0.0a1/enhydris_api_client.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2022-11-04 19:03:31.000000 enhydris-api-client-3.0.0a1/enhydris_api_client.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       20 2022-11-04 19:03:31.000000 enhydris-api-client-3.0.0a1/enhydris_api_client.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2022-11-04 19:03:31.954406 enhydris-api-client-3.0.0a1/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1404 2022-11-04 19:02:47.000000 enhydris-api-client-3.0.0a1/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-11-04 19:03:31.954406 enhydris-api-client-3.0.0a1/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1778 2022-10-31 07:39:21.000000 enhydris-api-client-3.0.0a1/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6745 2022-10-31 08:07:50.000000 enhydris-api-client-3.0.0a1/tests/test_e2e.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6100 2022-10-31 07:39:21.000000 enhydris-api-client-3.0.0a1/tests/test_e2e.py.orig
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5326 2022-10-31 07:39:21.000000 enhydris-api-client-3.0.0a1/tests/test_misc.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2983 2022-10-31 07:39:21.000000 enhydris-api-client-3.0.0a1/tests/test_station.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3787 2022-10-31 07:39:21.000000 enhydris-api-client-3.0.0a1/tests/test_timeseries.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3210 2022-10-31 08:07:50.000000 enhydris-api-client-3.0.0a1/tests/test_timeseriesgroup.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6232 2022-10-31 21:18:14.000000 enhydris-api-client-3.0.0a1/tests/test_tsdata.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1764 2024-04-14 15:01:34.000000 enhydris-api-client-3.0.1/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      828 2022-03-25 09:49:03.000000 enhydris-api-client-3.0.1/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      143 2022-03-25 09:49:03.000000 enhydris-api-client-3.0.1/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6839 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4146 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/enhydris_api_client/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9394 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/enhydris_api_client/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6839 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      525 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-27 19:13:39.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       20 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1500 2024-04-14 15:02:29.000000 enhydris-api-client-3.0.1/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1838 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7745 2022-12-04 15:39:55.000000 enhydris-api-client-3.0.1/tests/test_e2e.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6100 2022-10-31 07:39:21.000000 enhydris-api-client-3.0.1/tests/test_e2e.py.orig
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5326 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_misc.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2983 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_station.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3787 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_timeseries.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3210 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_timeseriesgroup.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6213 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_tsdata.py
```

### Comparing `enhydris-api-client-3.0.0a1/HISTORY.rst` & `enhydris-api-client-3.0.1/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 =======
 History
 =======
 
-DEV
-===
+3.0.1 (2024-04-14)
+==================
+
+- Compatible with htimeseries 4 to 7.
+
+3.0.0 (2022-12-04)
+==================
 
-- Requires Enhydris 4.0.
+- Requires Enhydris 4 and htimeseries 4, and therefore requires aware
+  HTimeseries objects.
+- Requires specifying time zone when downloading time series data.
 - Support for creating, retrieving, updating, and deleting time series
   groups.
-- Requires specifying time zone when uploading time series data.
-- Supports specifying time zone when downloading time series data.
 
 2.0.1 (2021-08-31)
 ==================
 
 - Updated dependences (the version of htimeseries required was too old).
 
 2.0.0 (2020-10-06)
```

### Comparing `enhydris-api-client-3.0.0a1/LICENSE` & `enhydris-api-client-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.0a1/README.rst` & `enhydris-api-client-3.0.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -89,30 +89,26 @@
 | **.get_timeseries(station_id, timeseries_group_id, timeseries_id)**
 | **.post_timeseries(station_id, timeseries_group_id, data)**
 | **.delete_timeseries(station_id, timeseries_group_id, timeseries_id)**
 
 Methods that create, retrieve or delete time series. Similar to the ones
 for station. ``list_timeseries()`` returns a list of dictionaries.
 
-| **.read_tsdata(station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None, timezone=None)**
-| **.post_tsdata(station_id, timeseries_group_id, timeseries_id, ts, default_timezone=None)**
-| **.get_ts_end_date(station_id, timeseries_group_id, timeseries_id, timezone=None)**
+| **.read_tsdata(station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None, timezone="UTC")**
+| **.post_tsdata(station_id, timeseries_group_id, timeseries_id, ts)**
+| **.get_ts_end_date(station_id, timeseries_group_id, timeseries_id, timezone="UTC")**
 
 Methods that retrieve or update time series data.
 
 ``read_ts_data()`` retrieves the time series data into a htimeseries
-object that it returns. If ``start_date`` and/or ``end_date`` are
-specified, only the part of the time series between these dates is
-retrieved. The timestamps are returned in the specified time zone; if
-unspecified, they are returned in the default display time zone for the
-station.
+object that it returns. If ``start_date`` and/or ``end_date`` (aware
+datetime objects) are specified, only the part of the time series
+between these dates is retrieved. The timestamps are returned in the
+specified time zone.
 
 ``post_tsdata() `` posts a time series to Enhydris, appending the
-records to any already existing.  ``ts`` is a htimeseries object.  If
-``ts`` has a ``timezone`` attribute, that one is used as the timezone of
-the timestamps; otherwise ``default_timezone`` is used. One of these
-must be defined, otherwise an error is raised.
+records to any already existing.  ``ts`` is a htimeseries object.
 
 ``get_ts_end_date()`` returns a ``datetime`` object which is the last
 timestamp of the time series. If the time series is empty it returns
-``None``. ``timezone`` works as with ``read_ts_data()``. The returned
-timestamp is always naive.
+``None``. The returned timestamp is always naive, but it is in the specified
+``timezone``.
```

### Comparing `enhydris-api-client-3.0.0a1/enhydris_api_client/__init__.py` & `enhydris-api-client-3.0.1/enhydris_api_client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from io import StringIO
 from urllib.parse import urljoin
 
+try:
+    from zoneinfo import ZoneInfo
+except ImportError:
+    from backports.zoneinfo import ZoneInfo
+
 import iso8601
 import requests
 from htimeseries import HTimeseries
 
 
 class EnhydrisApiClient:
     def __init__(self, base_url, token=None):
@@ -181,59 +186,68 @@
     def read_tsdata(
         self,
         station_id,
         timeseries_group_id,
         timeseries_id,
         start_date=None,
         end_date=None,
-        timezone=None,
+        timezone="UTC",
     ):
         url = urljoin(
             self.base_url,
             f"api/stations/{station_id}/timeseriesgroups/{timeseries_group_id}/"
             f"timeseries/{timeseries_id}/data/",
         )
         params = {"fmt": "hts"}
-        params["start_date"] = start_date and start_date.isoformat()
-        params["end_date"] = end_date and end_date.isoformat()
-        if timezone:
-            params["timezone"] = timezone
+        tzinfo = ZoneInfo(timezone)
+        dates_are_aware = (start_date is None or start_date.tzinfo is not None) and (
+            end_date is None or end_date.tzinfo is not None
+        )
+        if not dates_are_aware:
+            raise ValueError("start_date and end_date must be aware")
+        params["start_date"] = (
+            start_date and start_date.astimezone(tzinfo).isoformat()[:19]
+        )
+        params["end_date"] = end_date and end_date.astimezone(tzinfo).isoformat()[:19]
+        params["timezone"] = timezone
         self.response = self.session.get(url, params=params)
         self.check_response()
         if self.response.text:
-            return HTimeseries(StringIO(self.response.text))
+            return HTimeseries(
+                StringIO(self.response.text), default_tzinfo=ZoneInfo(timezone)
+            )
         else:
             return HTimeseries()
 
-    def post_tsdata(
-        self, station_id, timeseries_group_id, timeseries_id, ts, default_timezone=None
-    ):
+    def post_tsdata(self, station_id, timeseries_group_id, timeseries_id, ts):
         f = StringIO()
+        try:
+            ts.data.index = ts.data.index.tz_convert("UTC")
+        except AttributeError:
+            assert ts.data.empty
         ts.data.to_csv(f, header=False)
-        timezone = getattr(ts, "timezone", None) or default_timezone
         url = urljoin(
             self.base_url,
             f"api/stations/{station_id}/timeseriesgroups/{timeseries_group_id}/"
             f"timeseries/{timeseries_id}/data/",
         )
         self.response = self.session.post(
-            url, data={"timeseries_records": f.getvalue(), "timezone": timezone}
+            url, data={"timeseries_records": f.getvalue(), "timezone": "UTC"}
         )
         self.check_response()
         return self.response.text
 
     def get_ts_end_date(
-        self, station_id, timeseries_group_id, timeseries_id, timezone=None
+        self, station_id, timeseries_group_id, timeseries_id, timezone="UTC"
     ):
-        suffix = timezone and f"?timezone={timezone}" or ""
         url = urljoin(
             self.base_url,
             f"api/stations/{station_id}/timeseriesgroups/{timeseries_group_id}/"
-            f"timeseries/{timeseries_id}/bottom/{suffix}",
+            f"timeseries/{timeseries_id}/bottom/",
         )
-        self.response = self.session.get(url)
+        self.response = self.session.get(url, params={"timezone": timezone})
         self.check_response()
         try:
             datestring = self.response.text.strip().split(",")[0]
             return iso8601.parse_date(datestring, default_timezone=None)
         except (IndexError, iso8601.ParseError):
             return None
```

### Comparing `enhydris-api-client-3.0.0a1/enhydris_api_client.egg-info/SOURCES.txt` & `enhydris-api-client-3.0.1/enhydris_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.0a1/setup.py` & `enhydris-api-client-3.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,29 +4,31 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["iso8601", "requests>=1,<3", "htimeseries>=3,<5"]
+requirements = ["iso8601", "requests>=1,<3", "htimeseries>=4,<8"]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
     author="Antonis Christofides",
     author_email="antonis@antonischristofides.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     description="Python API client for Enhydris",
     install_requires=requirements,
     license="GNU General Public License v3",
@@ -35,10 +37,10 @@
     include_package_data=True,
     name="enhydris-api-client",
     packages=find_packages(include=["enhydris_api_client"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/openmeteo/enhydris-api-client",
-    version="3.0.0a1",
+    version="3.0.1",
     zip_safe=False,
 )
```

### Comparing `enhydris-api-client-3.0.0a1/tests/__init__.py` & `enhydris-api-client-3.0.1/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime as dt
 import textwrap
 from io import StringIO
 from unittest import mock
 
 import requests
 from htimeseries import HTimeseries
 
@@ -10,15 +11,17 @@
     2014-01-01 08:00,11.0,
     2014-01-02 08:00,12.0,
     2014-01-03 08:00,13.0,
     2014-01-04 08:00,14.0,
     2014-01-05 08:00,15.0,
     """
 )
-test_timeseries_hts = HTimeseries(StringIO(test_timeseries_csv))
+test_timeseries_hts = HTimeseries(
+    StringIO(test_timeseries_csv), default_tzinfo=dt.timezone.utc
+)
 test_timeseries_csv_top = "".join(test_timeseries_csv.splitlines(keepends=True)[:-1])
 test_timeseries_csv_bottom = test_timeseries_csv.splitlines(keepends=True)[-1]
 
 
 def mock_session(**kwargs):
     """Mock requests.Session.
```

### Comparing `enhydris-api-client-3.0.0a1/tests/test_e2e.py` & `enhydris-api-client-3.0.1/tests/test_e2e.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import datetime as dt
 import json
 import os
 import textwrap
 from io import StringIO
 from unittest import TestCase, skipUnless
 
+try:
+    from zoneinfo import ZoneInfo
+except ImportError:
+    from backports.zoneinfo import ZoneInfo
+
 import pandas as pd
 import requests
 from htimeseries import HTimeseries
 
 from enhydris_api_client import EnhydrisApiClient
 
 from . import test_timeseries_hts
@@ -123,61 +128,78 @@
 
         # Post time series data
         self.client.post_tsdata(
             tmp_station_id,
             self.timeseries_group_id,
             self.timeseries_id,
             test_timeseries_hts,
-            default_timezone="Etc/GMT-2",
         )
 
         # Get the last date and check it
         date = self.client.get_ts_end_date(
-            tmp_station_id, self.timeseries_group_id, self.timeseries_id
-        )
-        self.assertEqual(date, dt.datetime(2014, 1, 5, 7, 0))
-
-        # Change display timezone
-        self.client.patch_station(
-            tmp_station_id, data={"display_timezone": "Etc/GMT-2"}
+            tmp_station_id,
+            self.timeseries_group_id,
+            self.timeseries_id,
         )
+        self.assertEqual(date, dt.datetime(2014, 1, 5, 8, 0))
 
-        # Get the last date again and check it
+        # Get the last date in a different timezone from UTC
         date = self.client.get_ts_end_date(
-            tmp_station_id, self.timeseries_group_id, self.timeseries_id
+            tmp_station_id,
+            self.timeseries_group_id,
+            self.timeseries_id,
+            timezone="Etc/GMT-5",
         )
-        self.assertEqual(date, dt.datetime(2014, 1, 5, 8, 0))
+        self.assertEqual(date, dt.datetime(2014, 1, 5, 13, 0))
 
         # Get all time series data and check it
         hts = self.client.read_tsdata(
             tmp_station_id, self.timeseries_group_id, self.timeseries_id
         )
+        try:
+            # Compatibility with older Python or pandas versions (such as Python 3.7
+            # with pandas 0.23): comparison may fail if tzinfo, although practically the
+            # same thing, is a different object
+            if hts.data.index.tz.offset == dt.timedelta(0):
+                hts.data.index = hts.data.index.tz_convert(dt.timezone.utc)
+        except AttributeError:
+            pass
         pd.testing.assert_frame_equal(hts.data, test_timeseries_hts.data)
 
         # The other attributes should have been set too.
         self.assertTrue(hasattr(hts, "variable"))
 
         # Get part of the time series data and check it
         hts = self.client.read_tsdata(
             tmp_station_id,
             self.timeseries_group_id,
             self.timeseries_id,
-            start_date=dt.datetime(2014, 1, 3, 8, 0),
-            end_date=dt.datetime(2014, 1, 4, 8, 0),
+            start_date=dt.datetime(2014, 1, 3, 8, 0, tzinfo=dt.timezone.utc),
+            end_date=dt.datetime(2014, 1, 4, 8, 0, tzinfo=dt.timezone.utc),
+            timezone="Etc/GMT-1",
         )
         expected_result = HTimeseries(
             StringIO(
                 textwrap.dedent(
                     """\
-                    2014-01-03 08:00,13.0,
-                    2014-01-04 08:00,14.0,
+                    2014-01-03 09:00,13.0,
+                    2014-01-04 09:00,14.0,
                     """
                 )
-            )
+            ),
+            default_tzinfo=ZoneInfo("Etc/GMT-1"),
         )
+        try:
+            # Compatibility with older Python or pandas versions (such as Python 3.7
+            # with pandas 0.23): comparison may fail if tzinfo, although practically the
+            # same thing, is a different object
+            if hts.data.index.tz.offset == dt.timedelta(minutes=60):
+                hts.data.index = hts.data.index.tz_convert(ZoneInfo("Etc/GMT-1"))
+        except AttributeError:
+            pass
         pd.testing.assert_frame_equal(hts.data, expected_result.data)
 
         # Delete the time series and verify
         self.client.delete_timeseries(
             tmp_station_id, self.timeseries_group_id, self.timeseries_id
         )
         with self.assertRaises(requests.HTTPError):
```

### Comparing `enhydris-api-client-3.0.0a1/tests/test_e2e.py.orig` & `enhydris-api-client-3.0.1/tests/test_e2e.py.orig`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.0a1/tests/test_misc.py` & `enhydris-api-client-3.0.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.0a1/tests/test_station.py` & `enhydris-api-client-3.0.1/tests/test_station.py`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.0a1/tests/test_timeseries.py` & `enhydris-api-client-3.0.1/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.0a1/tests/test_timeseriesgroup.py` & `enhydris-api-client-3.0.1/tests/test_timeseriesgroup.py`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.0a1/tests/test_tsdata.py` & `enhydris-api-client-3.0.1/tests/test_tsdata.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,21 @@
     def _read_tsdata(self, **extra_args):
         self.client = EnhydrisApiClient("http://example.com")
         return self.client.read_tsdata(41, 42, 43, **extra_args)
 
     def test_makes_request(self, m):
         self._read_tsdata()
         m.return_value.get.assert_called_once_with(
-            self.url, params={"fmt": "hts", "start_date": None, "end_date": None}
+            self.url,
+            params={
+                "fmt": "hts",
+                "start_date": None,
+                "end_date": None,
+                "timezone": "UTC",
+            },
         )
 
     def test_returns_data(self, m):
         ahts = self._read_tsdata()
         pd.testing.assert_frame_equal(ahts.data, test_timeseries_hts.data)
 
     def test_uses_timezone(self, m):
@@ -48,36 +54,49 @@
 
 
 class ReadTsDataWithStartAndEndDateTestCase(TestCase):
     @mock_session(**{"get.return_value.text": test_timeseries_csv})
     def setUp(self, mock_requests_session):
         self.mock_requests_session = mock_requests_session
         self.client = EnhydrisApiClient("https://mydomain.com")
+
+    def _make_request(self, start_tzinfo, end_tzinfo):
         self.data = self.client.read_tsdata(
             41,
             42,
             43,
-            start_date=dt.datetime(2019, 6, 12, 0, 0),
-            end_date=dt.datetime(2019, 6, 13, 15, 25),
+            start_date=dt.datetime(2019, 6, 12, 0, 0, tzinfo=start_tzinfo),
+            end_date=dt.datetime(2019, 6, 13, 15, 25, tzinfo=end_tzinfo),
         )
 
     def test_makes_request(self):
+        self._make_request(dt.timezone.utc, dt.timezone.utc)
         self.mock_requests_session.return_value.get.assert_called_once_with(
             "https://mydomain.com/api/stations/41/timeseriesgroups/42/timeseries/43/"
             "data/",
             params={
                 "fmt": "hts",
                 "start_date": "2019-06-12T00:00:00",
                 "end_date": "2019-06-13T15:25:00",
+                "timezone": "UTC",
             },
         )
 
     def test_returns_data(self):
+        self._make_request(dt.timezone.utc, dt.timezone.utc)
         pd.testing.assert_frame_equal(self.data.data, test_timeseries_hts.data)
 
+    def test_checks_that_start_date_is_aware(self):
+        with self.assertRaises(ValueError):
+            self._make_request(None, dt.timezone.utc)
+
+    def test_checks_that_end_date_is_aware(self):
+        with self.assertRaises(ValueError):
+            self._make_request(dt.timezone.utc, None)
+
 
 class ReadEmptyTsDataTestCase(TestCase):
     @mock_session(**{"get.return_value.text": ""})
     def test_returns_data(self, mock_requests_session):
         self.client = EnhydrisApiClient("https://mydomain.com")
         self.data = self.client.read_tsdata(41, 42, 43)
         pd.testing.assert_frame_equal(self.data.data, HTimeseries().data)
@@ -89,42 +108,25 @@
         self.client = EnhydrisApiClient("https://mydomain.com")
         with self.assertRaises(requests.HTTPError):
             self.client.read_tsdata(41, 42, 43)
 
 
 class PostTsDataTestCase(TestCase):
     @mock_session()
-    def test_makes_request_with_default_timezone(self, mock_requests_session):
+    def test_makes_request(self, mock_requests_session):
         client = EnhydrisApiClient("https://mydomain.com")
         if hasattr(test_timeseries_hts, "timezone"):
             del test_timeseries_hts.timezone
-        client.post_tsdata(
-            41, 42, 43, test_timeseries_hts, default_timezone="Etc/GMT-2"
-        )
+        client.post_tsdata(41, 42, 43, test_timeseries_hts)
         f = StringIO()
         test_timeseries_hts.data.to_csv(f, header=False)
         mock_requests_session.return_value.post.assert_called_once_with(
             "https://mydomain.com/api/stations/41/timeseriesgroups/42/timeseries/43/"
             "data/",
-            data={"timeseries_records": f.getvalue(), "timezone": "Etc/GMT-2"},
-        )
-
-    @mock_session()
-    def test_makes_request_with_nondefault_timezone(self, mock_requests_session):
-        client = EnhydrisApiClient("https://mydomain.com")
-        test_timeseries_hts.timezone = "Etc/GMT-1"
-        client.post_tsdata(
-            41, 42, 43, test_timeseries_hts, default_timezone="Etc/GMT-2"
-        )
-        f = StringIO()
-        test_timeseries_hts.data.to_csv(f, header=False)
-        mock_requests_session.return_value.post.assert_called_once_with(
-            "https://mydomain.com/api/stations/41/timeseriesgroups/42/timeseries/43/"
-            "data/",
-            data={"timeseries_records": f.getvalue(), "timezone": "Etc/GMT-1"},
+            data={"timeseries_records": f.getvalue(), "timezone": "UTC"},
         )
 
     @mock_session(**{"post.return_value.status_code": 404})
     def test_raises_exception_on_error(self, mock_requests_session):
         client = EnhydrisApiClient("https://mydomain.com")
         with self.assertRaises(requests.HTTPError):
             client.post_tsdata(41, 42, 43, test_timeseries_hts)
@@ -136,23 +138,25 @@
 
     def _get_ts_end_date(self, **extra_args):
         self.client = EnhydrisApiClient("http://mydom.com")
         return self.client.get_ts_end_date(41, 42, 43, **extra_args)
 
     def test_makes_request(self, m):
         self._get_ts_end_date()
-        m.return_value.get.assert_called_once_with(self.url)
+        m.return_value.get.assert_called_once_with(self.url, params={"timezone": "UTC"})
 
     def test_returns_date(self, m):
         result = self._get_ts_end_date()
         self.assertEqual(result, dt.datetime(2014, 1, 5, 8, 0))
 
     def test_uses_timezone(self, m):
-        self._get_ts_end_date(timezone="UTC")
-        m.return_value.get.assert_called_once_with(self.url + "?timezone=UTC")
+        self._get_ts_end_date(timezone="Etc/GMT-2")
+        m.return_value.get.assert_called_once_with(
+            self.url, params={"timezone": "Etc/GMT-2"}
+        )
 
 
 class GetTsEndDateErrorTestCase(TestCase):
     @mock_session(**{"get.return_value.status_code": 404})
     def test_checks_response_code(self, mock_requests_session):
         client = EnhydrisApiClient("https://mydomain.com")
         with self.assertRaises(requests.HTTPError):
```

