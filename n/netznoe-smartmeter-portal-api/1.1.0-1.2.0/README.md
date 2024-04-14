# Comparing `tmp/netznoe_smartmeter_portal_api-1.1.0.tar.gz` & `tmp/netznoe_smartmeter_portal_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netznoe_smartmeter_portal_api-1.1.0.tar", last modified: Sat Apr 13 13:58:15 2024, max compression
+gzip compressed data, was "netznoe_smartmeter_portal_api-1.2.0.tar", last modified: Sun Apr 14 21:15:56 2024, max compression
```

## Comparing `netznoe_smartmeter_portal_api-1.1.0.tar` & `netznoe_smartmeter_portal_api-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:15.497273 netznoe_smartmeter_portal_api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-13 13:58:15.497273 netznoe_smartmeter_portal_api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-13 13:58:15.497273 netznoe_smartmeter_portal_api-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:15.493273 netznoe_smartmeter_portal_api-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:15.493273 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-13 13:58:10.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:58:15.493273 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-13 13:58:15.000000 netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:56.264837 netznoe_smartmeter_portal_api-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 21:15:51.000000 netznoe_smartmeter_portal_api-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-14 21:15:51.000000 netznoe_smartmeter_portal_api-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-14 21:15:56.264837 netznoe_smartmeter_portal_api-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-14 21:15:51.000000 netznoe_smartmeter_portal_api-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-14 21:15:51.000000 netznoe_smartmeter_portal_api-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-14 21:15:56.264837 netznoe_smartmeter_portal_api-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-14 21:15:51.000000 netznoe_smartmeter_portal_api-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:56.260837 netznoe_smartmeter_portal_api-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:56.260837 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-14 21:15:51.000000 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-14 21:15:51.000000 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-14 21:15:51.000000 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:56.264837 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-14 21:15:56.000000 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-14 21:15:56.000000 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:15:56.000000 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 21:15:56.000000 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-14 21:15:56.000000 netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api.egg-info/top_level.txt
```

### Comparing `netznoe_smartmeter_portal_api-1.1.0/LICENSE` & `netznoe_smartmeter_portal_api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netznoe_smartmeter_portal_api-1.1.0/PKG-INFO` & `netznoe_smartmeter_portal_api-1.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netznoe-smartmeter-portal-api
-Version: 1.1.0
+Version: 1.2.0
 Summary: An unofficial python implementation of the NetzNÖ Smartmeter Portal API
 Home-page: https://github.com/schue30/NetzNoe-SmartmeterPortal-Api
 Author: Mathias Schuepany
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,75 +27,78 @@
 ```bash
 pip3 install netznoe-smartmeter-portal-api
 ```
 
 ## Usage example
 
 ```python
-from pendulum import Date
-
+from datetime import date
 from netznoe_smartmeter_portal_api import NetzNoeSmartmeterPortalApi
 
 meter_id = 'AT0020000000000000000000020xxxxxx'
 api = NetzNoeSmartmeterPortalApi(username='username', password='password')
 api.do_login()
 
 # ---
 # API Methods:
 
+# returns all metering points (meter_ids) of the user
+metering_points = api.get_metering_points()
+# meter_id = metering_points[0].metering_point_id  # get meter_id dynamically via API
+
 # returns monthly aggregated data
 yearly_values = api.get_year(meter_id, 2023)
 # SmartmeterResultYearly(
-#   values={
-#     datetime.date(2023, 1, 1): 100.001,
+#   values=[
+#     (datetime.date(2023, 1, 1), 100.001),
 #     ...
-#   },
-#   peak_demands={
-#     datetime.datetime(2023, 2, 18, 17, 15, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): 2.101, 
+#   ],
+#   peak_demands=[
+#     (datetime.datetime(2023, 2, 18, 17, 15, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), 2.101), 
 #     ...
-#   },
-#   self_coverage={},
-#   self_coverage_renewable_energy={},
-#   grid_usage_leftover={},
-#   joint_tenancy_proportion={}
-#   blind_consumption={},
-#   blind_power_feed={},
+#   ],
+#   self_coverage=[],
+#   self_coverage_renewable_energy=[],
+#   grid_usage_leftover=[],
+#   joint_tenancy_proportion=[],
+#   blind_consumption=[],
+#   blind_power_feed=[]
 # )
 
 # returns daily aggregated data for the requested month
 monthly_values = api.get_month(meter_id, 2023, 3)
 # SmartmeterResult(
-#   metered={
-#     datetime.date(2023, 3, 1): 1.810, 
+#   metered=[
+#     (datetime.date(2023, 3, 1), 1.810), 
 #     ...
-#   },
-#   metered_peak_demands={
-#     datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): 0.012,
+#   ],
+#   metered_peak_demands=[
+#     (datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), 0.012),
 #     ...
-#   },
-#   peak_demand_data_qualities={
-#     datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): SmartmeterDataQuality.L1,
-#   },
-#   estimated={},
-#   estimated_qualities={},
-#   estimated_peak_demands={},
-#   self_coverage={}, 
-#   self_coverage_renewable_energy={}, 
-#   grid_usage_leftover={},
-#   joint_tenancy_proportion={}, 
-#   quality_ec={},
-#   blind_consumption={},
-#   blind_power_feed={}
+#   ],
+#   peak_demand_data_qualities=[
+#     (datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), SmartmeterDataQuality.L1),
+#   ],
+#   estimated=[],
+#   estimated_qualities=[],
+#   estimated_peak_demands=[],
+#   self_coverage=[],
+#   self_coverage_renewable_energy=[], 
+#   grid_usage_leftover=[],
+#   joint_tenancy_proportion=[], 
+#   quality_ec=[],
+#   blind_consumption=[],
+#   blind_power_feed=[]
 # )
 
 # returns daily aggregated data for the requested time range
-weekly_values = api.get_week(meter_id, start_date=Date(2023, 1, 2), end_date=Date(2023, 1, 8))
+weekly_values = api.get_week(meter_id, start_date=date(2023, 1, 2), end_date=date(2023, 1, 8))
 
 # returns 15min values of the requested day
-daily_values = api.get_day(meter_id, day=Date(2023, 4, 1))
+daily_values = api.get_day(meter_id, day=date(2023, 4, 1))
 
 # logout of the api
 api.do_logout()
 ```
 
 ## Mapping between API fields and model fields
```

### Comparing `netznoe_smartmeter_portal_api-1.1.0/README.md` & `netznoe_smartmeter_portal_api-1.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -10,75 +10,78 @@
 ```bash
 pip3 install netznoe-smartmeter-portal-api
 ```
 
 ## Usage example
 
 ```python
-from pendulum import Date
-
+from datetime import date
 from netznoe_smartmeter_portal_api import NetzNoeSmartmeterPortalApi
 
 meter_id = 'AT0020000000000000000000020xxxxxx'
 api = NetzNoeSmartmeterPortalApi(username='username', password='password')
 api.do_login()
 
 # ---
 # API Methods:
 
+# returns all metering points (meter_ids) of the user
+metering_points = api.get_metering_points()
+# meter_id = metering_points[0].metering_point_id  # get meter_id dynamically via API
+
 # returns monthly aggregated data
 yearly_values = api.get_year(meter_id, 2023)
 # SmartmeterResultYearly(
-#   values={
-#     datetime.date(2023, 1, 1): 100.001,
+#   values=[
+#     (datetime.date(2023, 1, 1), 100.001),
 #     ...
-#   },
-#   peak_demands={
-#     datetime.datetime(2023, 2, 18, 17, 15, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): 2.101, 
+#   ],
+#   peak_demands=[
+#     (datetime.datetime(2023, 2, 18, 17, 15, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), 2.101), 
 #     ...
-#   },
-#   self_coverage={},
-#   self_coverage_renewable_energy={},
-#   grid_usage_leftover={},
-#   joint_tenancy_proportion={}
-#   blind_consumption={},
-#   blind_power_feed={},
+#   ],
+#   self_coverage=[],
+#   self_coverage_renewable_energy=[],
+#   grid_usage_leftover=[],
+#   joint_tenancy_proportion=[],
+#   blind_consumption=[],
+#   blind_power_feed=[]
 # )
 
 # returns daily aggregated data for the requested month
 monthly_values = api.get_month(meter_id, 2023, 3)
 # SmartmeterResult(
-#   metered={
-#     datetime.date(2023, 3, 1): 1.810, 
+#   metered=[
+#     (datetime.date(2023, 3, 1), 1.810), 
 #     ...
-#   },
-#   metered_peak_demands={
-#     datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): 0.012,
+#   ],
+#   metered_peak_demands=[
+#     (datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), 0.012),
 #     ...
-#   },
-#   peak_demand_data_qualities={
-#     datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): SmartmeterDataQuality.L1,
-#   },
-#   estimated={},
-#   estimated_qualities={},
-#   estimated_peak_demands={},
-#   self_coverage={}, 
-#   self_coverage_renewable_energy={}, 
-#   grid_usage_leftover={},
-#   joint_tenancy_proportion={}, 
-#   quality_ec={},
-#   blind_consumption={},
-#   blind_power_feed={}
+#   ],
+#   peak_demand_data_qualities=[
+#     (datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), SmartmeterDataQuality.L1),
+#   ],
+#   estimated=[],
+#   estimated_qualities=[],
+#   estimated_peak_demands=[],
+#   self_coverage=[],
+#   self_coverage_renewable_energy=[], 
+#   grid_usage_leftover=[],
+#   joint_tenancy_proportion=[], 
+#   quality_ec=[],
+#   blind_consumption=[],
+#   blind_power_feed=[]
 # )
 
 # returns daily aggregated data for the requested time range
-weekly_values = api.get_week(meter_id, start_date=Date(2023, 1, 2), end_date=Date(2023, 1, 8))
+weekly_values = api.get_week(meter_id, start_date=date(2023, 1, 2), end_date=date(2023, 1, 8))
 
 # returns 15min values of the requested day
-daily_values = api.get_day(meter_id, day=Date(2023, 4, 1))
+daily_values = api.get_day(meter_id, day=date(2023, 4, 1))
 
 # logout of the api
 api.do_logout()
 ```
 
 ## Mapping between API fields and model fields
```

### Comparing `netznoe_smartmeter_portal_api-1.1.0/pyproject.toml` & `netznoe_smartmeter_portal_api-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `netznoe_smartmeter_portal_api-1.1.0/setup.cfg` & `netznoe_smartmeter_portal_api-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `netznoe_smartmeter_portal_api-1.1.0/setup.py` & `netznoe_smartmeter_portal_api-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def get_long_description():
     return open(os.path.join(ROOT_DIR, "README.md"), encoding="utf-8").read()
 
 
 setup(
     name="netznoe-smartmeter-portal-api",
-    version="1.1.0",
+    version="1.2.0",
     license="MIT",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     packages=find_packages("src"),
     include_package_data=True,
     package_dir={"": "src"},
     description="An unofficial python implementation of the NetzNÖ Smartmeter Portal API",
```

### Comparing `netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/api.py` & `netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-import logging
-import typing
 from datetime import date, datetime, timedelta
-from typing import Dict, List, Union
+from typing import Dict, List, Union, no_type_check, Tuple
 from zoneinfo import ZoneInfo
 
 import itertools
 from requests import Session
 
 from .models import (
     SmartmeterDataQuality,
     SmartmeterEnergyCommunity,
     SmartmeterMeteringPoint,
     SmartmeterResult,
     SmartmeterResultYearly,
 )
 
-LOGGER = logging.getLogger('NetzNoeSmartmeterPortalApi')
-
 
 class NetzNoeSmartmeterPortalAuthError(Exception):
     pass
 
 
 class NetzNoeSmartmeterPortalDataError(Exception):
     pass
@@ -49,15 +45,16 @@
 
     def get_day_per_energy_community(self, meter_id: str, day: date) -> Dict[str, SmartmeterResult]:
         resp = self.__session.get(f'{self.__domain}/orchestration/ConsumptionRecord/Day',
                                   params={'meterId': meter_id, 'day': day.strftime('%Y-%-m-%-d')})
         if resp.status_code != 200:
             raise NetzNoeSmartmeterPortalDataError('Fetching daily data failed')
 
-        base_time = datetime(day.year, day.month, day.day, hour=0, minute=15, tzinfo=ZoneInfo('Europe/Vienna'))
+        base_time = datetime(day.year, day.month, day.day, hour=0, minute=15,
+                             tzinfo=ZoneInfo('Europe/Vienna')).astimezone(ZoneInfo('UTC'))
         return dict(map(
             lambda e: (
                 e.get('ec_id') if e.get('ec_id') else 'total',
                 self.__to_smartmeter_result(base_time, e, time_increase={'minutes': 15})
             ), resp.json()
         ))
 
@@ -148,49 +145,60 @@
             type_of_relation=meter.get('typeOfRelation'),
             energy_communities=list(map(lambda ec: SmartmeterEnergyCommunity(
                 id=ec.get('ecid'),
                 name=ec.get('name')
             ), meter.get('energyCommunities', [])))
         ), resp.json()))
 
-    @staticmethod
-    def __get_values(data: dict, field: str, base_time: Union[date, datetime],
-                     time_increase: Dict[str, int]) -> Dict[Union[date, datetime], Union[float, SmartmeterDataQuality]]:
-        results: Dict[Union[date, datetime], Union[float, SmartmeterDataQuality]] = {}
+    def __get_values(self, data: dict, field: str, base_time: Union[date, datetime],
+                     time_increase: Dict[str, int]
+                     ) -> List[Tuple[Union[date, datetime], Union[float, SmartmeterDataQuality]]]:
+        results: List[Tuple[Union[date, datetime], Union[float, SmartmeterDataQuality]]] = []
         for value in data.get(field, []):
             if value is not None:
+                converted_time = base_time
+                if isinstance(converted_time, datetime):
+                    converted_time = converted_time.astimezone(ZoneInfo('Europe/Vienna'))
                 if value in ('L1', 'L2', 'L3'):
-                    results[base_time] = SmartmeterDataQuality(value)
+                    results.append((converted_time, SmartmeterDataQuality(value)))
                 else:
-                    results[base_time] = value
+                    results.append((converted_time, value))
 
             # increase base_time for next value
-            if 'months' in time_increase and isinstance(base_time, date):
-                if base_time.month < 12:
-                    base_time = date(base_time.year, base_time.month + time_increase['months'], base_time.day)
-            else:
-                base_time += timedelta(**time_increase)
+            base_time = self._calc_next_datetime(base_time, time_increase)
         return results
 
     @staticmethod
-    def __process_peak_demand(data: dict, field: str) -> Dict[datetime, Union[float, SmartmeterDataQuality]]:
-        results: Dict[datetime, Union[float, SmartmeterDataQuality]] = {}
+    def __process_peak_demand(data: dict, field: str) -> List[Tuple[datetime, Union[float, SmartmeterDataQuality]]]:
+        results: List[Tuple[datetime, Union[float, SmartmeterDataQuality]]] = []
         for cnt, value in enumerate(data.get(field, [])):
             if value is not None:
                 timestamp = datetime.strptime(
                     data['peakDemandTimes'][cnt], '%Y-%m-%dT%H:%M:%S'
-                ).replace(tzinfo=ZoneInfo('Europe/Vienna'))
+                ).replace(tzinfo=ZoneInfo('UTC')).astimezone(ZoneInfo('Europe/Vienna'))
 
                 if value in ('L1', 'L2', 'L3'):
-                    results[timestamp] = SmartmeterDataQuality(value)
+                    results.append((timestamp, SmartmeterDataQuality(value)))
                 else:
-                    results[timestamp] = value
+                    results.append((timestamp, value))
         return results
 
-    @typing.no_type_check
+    def _calc_next_datetime(self, current_time: Union[date, datetime],
+                            time_increase: Dict[str, int]) -> Union[date, datetime]:
+        if 'months' in time_increase and isinstance(current_time, date):
+            next_month = current_time.month + time_increase['months']
+            next_year = current_time.year + int(next_month / 12) if next_month > 12 else current_time.year
+            next_month = 12 if next_month % 12 == 0 else next_month % 12
+            return date(next_year, next_month, current_time.day)
+        elif 'days' in time_increase or 'minutes' in time_increase:
+            return current_time + timedelta(**time_increase)
+        else:
+            raise ValueError('Unsupported time_increase interval')
+
+    @no_type_check
     def __to_smartmeter_result(self, base_time: Union[date, datetime], data: dict,
                                time_increase: dict) -> SmartmeterResult:
         return SmartmeterResult(
             metered=self.__get_values(data, 'meteredValues', base_time, time_increase),
             estimated=self.__get_values(data, 'estimatedValues', base_time, time_increase),
             estimated_qualities=self.__get_values(data, 'estimatedQualities', base_time, time_increase),
             grid_usage_leftover=self.__get_values(data, 'gridUsageLeftoverValues', base_time, time_increase),
@@ -202,15 +210,15 @@
             peak_demand_data_qualities=self.__process_peak_demand(data, 'peakDemandDataQualities'),
             self_coverage_renewable_energy=self.__get_values(data, 'selfCoverageRenewableEnergyValue',
                                                              base_time, time_increase),
             blind_consumption=self.__get_values(data, 'blindConsumptionValue', base_time, time_increase),
             blind_power_feed=self.__get_values(data, 'blindPowerFeedValue', base_time, time_increase)
         )
 
-    @typing.no_type_check
+    @no_type_check
     def __to_smartmeter_result_yearly(self, base_time: date, data: dict, time_increase: dict) -> SmartmeterResultYearly:
         return SmartmeterResultYearly(
             values=self.__get_values(data, 'values', base_time, time_increase),
             grid_usage_leftover=self.__get_values(data, 'gridUsageLeftoverValues', base_time, time_increase),
             blind_consumption=self.__get_values(data, 'blindConsumptionValue', base_time, time_increase),
             blind_power_feed=self.__get_values(data, 'blindPowerFeedValue', base_time, time_increase),
             self_coverage=self.__get_values(data, 'selfCoverageValues', base_time, time_increase),
```

### Comparing `netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api/models.py` & `netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from datetime import date, datetime
 from enum import Enum
-from typing import Dict, List, Union
+from typing import List, Union, Tuple
 
 
 @dataclass
 class SmartmeterEnergyCommunity:
     id: str
     name: str
 
@@ -28,156 +28,131 @@
 @dataclass
 class SmartmeterResult:
     # Description:
     #   Production: Einspeisung gemessen
     #   Consumption: Verbrauch gemessen
     # Unit: kWh
     # API: meteredValues
-    metered: Dict[Union[date, datetime], float]
+    metered: List[Tuple[Union[date, datetime], float]]
 
     # Description: Ersatzwert
     #   Production: Einspeisung Ersatzwert
     #   Consumption: Verbrauch Ersatzwert
     # Unit: kWh
     # API: estimatedValues
-    estimated: Dict[Union[date, datetime], float]
+    estimated: List[Tuple[Union[date, datetime], float]]
 
     # Description:
     # Unit:
     # API: estimatedQualities
-    estimated_qualities: Dict[Union[date, datetime], SmartmeterDataQuality]
+    estimated_qualities: List[Tuple[Union[date, datetime], SmartmeterDataQuality]]
 
     # Description:
     #   Production: Gemeinschaftsüberschuss
     #   Consumption: Restnetzbezug
     # Unit: kWh
     # API: gridUsageLeftoverValues
-    grid_usage_leftover: Dict[Union[date, datetime], float]
+    grid_usage_leftover: List[Tuple[Union[date, datetime], float]]
 
     # Description:
     # Unit:
     # API: qualityEC
-    quality_ec: Dict[Union[date, datetime], SmartmeterDataQuality]
+    quality_ec: List[Tuple[Union[date, datetime], SmartmeterDataQuality]]
 
     # Description:
     #   Production: Eigendeckung Teilnehmer
-    #   Consumption: Eigendeckung (kWh)
+    #   Consumption: Eigendeckung
     #   Ren. Energy: Eigendeckung erneuerbare Energie
     # Unit: kWh
     # API: selfCoverageValues
-    self_coverage: Dict[Union[date, datetime], float]
+    self_coverage: List[Tuple[Union[date, datetime], float]]
 
     # Description: Ideeller Anteil
     # Unit: kWh
     # API: jointTenancyProportionValues
-    joint_tenancy_proportion: Dict[Union[date, datetime], float]
+    joint_tenancy_proportion: List[Tuple[Union[date, datetime], float]]
 
     # Description: Leistung gemessen
     # Unit: kW
     # API: meteredPeakDemands
-    metered_peak_demands: Dict[datetime, float]
+    metered_peak_demands: List[Tuple[datetime, float]]
 
     # Description: Leistung Ersatzwert
     # Unit: kW
     # API: estimatedPeakDemands
-    estimated_peak_demands: Dict[datetime, float]
+    estimated_peak_demands: List[Tuple[datetime, float]]
 
     # Description:
     # Unit:
     # API: peakDemandDataQualities
-    peak_demand_data_qualities: Dict[Union[date, datetime], SmartmeterDataQuality]
+    peak_demand_data_qualities: List[Tuple[Union[date, datetime], SmartmeterDataQuality]]
 
     # Description: Eigendeckung erneuerbare Energie
     # Unit: kWh
     # API: selfCoverageRenewableEnergyValue
-    self_coverage_renewable_energy: Dict[Union[date, datetime], float]
+    self_coverage_renewable_energy: List[Tuple[Union[date, datetime], float]]
 
     # Description: Blindverbrauch
     # Unit: kvarh
     # API: blindConsumptionValue
-    blind_consumption: Dict[Union[date, datetime], float]
+    blind_consumption: List[Tuple[Union[date, datetime], float]]
 
     # Description: Blindeinspeisung
     # Unit: kvarh
     # API: blindPowerFeedValue
-    blind_power_feed: Dict[Union[date, datetime], float]
+    blind_power_feed: List[Tuple[Union[date, datetime], float]]
 
     # other API fields:
     #   ec_id, peakDemandTimes
 
-    # deprecated: implemented for backward compatibility
-    @property
-    def consumption_metered(self) -> Dict[Union[date, datetime], float]:  # pragma: no cover
-        return self.metered
-
-    # deprecated: implemented for backward compatibility
-    @property
-    def consumption_estimated(self) -> Dict[Union[date, datetime], float]:  # pragma: no cover
-        return self.estimated
-
-    # deprecated: implemented for backward compatibility
-    @property
-    def peak_demands_metered(self) -> Dict[datetime, float]:  # pragma: no cover
-        return self.metered_peak_demands
-
-    # deprecated: implemented for backward compatibility
-    @property
-    def peak_demands_estimated(self) -> Dict[datetime, float]:  # pragma: no cover
-        return self.estimated_peak_demands
-
 
 @dataclass
 class SmartmeterResultYearly:
     # Description:
     #   Production: Einspeisung
     #   Consumption: Verbrauch
     # Unit: kWh
     # API: values
-    values: Dict[date, float]
+    values: List[Tuple[date, float]]
 
     # Description:
     #   Production: Gemeinschaftsüberschuss
     #   Consumption: Restnetzbezug
     # Unit: kWh
     # API: gridUsageLeftoverValues
-    grid_usage_leftover: Dict[date, float]
+    grid_usage_leftover: List[Tuple[date, float]]
 
     # Description: Blindverbrauch
     # Unit: kvarh
     # API: blindConsumptionValue
-    blind_consumption: Dict[date, float]
+    blind_consumption: List[Tuple[date, float]]
 
     # Description: Blindeinspeisung
     # Unit: kvarh
     # API: blindPowerFeedValue
-    blind_power_feed: Dict[date, float]
+    blind_power_feed: List[Tuple[date, float]]
 
     # Description:
     #   Production: Eigendeckung Teilnehmer
-    #   Consumption: Eigendeckung (kWh)
+    #   Consumption: Eigendeckung
     #   Ren. Energy: Eigendeckung erneuerbare Energie
     # Unit: kWh
     # API: selfCoverageValues
-    self_coverage: Dict[date, float]
+    self_coverage: List[Tuple[date, float]]
 
     # Description: Ideeller Anteil
     # Unit: kWh
     # API: jointTenancyProportionValues
-    joint_tenancy_proportion: Dict[date, float]
+    joint_tenancy_proportion: List[Tuple[date, float]]
 
     # Description:
     # Unit: kW
     # API: peakDemands
-    peak_demands: Dict[datetime, float]
+    peak_demands: List[Tuple[datetime, float]]
 
     # Description: Eigendeckung erneuerbare Energie
     # Unit: kWh
     # API: selfCoverageRenewableEnergyValue
-    self_coverage_renewable_energy: Dict[date, float]
+    self_coverage_renewable_energy: List[Tuple[date, float]]
 
     # other API fields:
     #   ec_id, peakDemandTimes, isMixed
-
-    # deprecated: implemented for backward compatibility
-    @property
-    def consumption(self) -> Dict[date, float]:  # pragma: no cover
-        return self.values
```

### Comparing `netznoe_smartmeter_portal_api-1.1.0/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO` & `netznoe_smartmeter_portal_api-1.2.0/src/netznoe_smartmeter_portal_api.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netznoe-smartmeter-portal-api
-Version: 1.1.0
+Version: 1.2.0
 Summary: An unofficial python implementation of the NetzNÖ Smartmeter Portal API
 Home-page: https://github.com/schue30/NetzNoe-SmartmeterPortal-Api
 Author: Mathias Schuepany
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,75 +27,78 @@
 ```bash
 pip3 install netznoe-smartmeter-portal-api
 ```
 
 ## Usage example
 
 ```python
-from pendulum import Date
-
+from datetime import date
 from netznoe_smartmeter_portal_api import NetzNoeSmartmeterPortalApi
 
 meter_id = 'AT0020000000000000000000020xxxxxx'
 api = NetzNoeSmartmeterPortalApi(username='username', password='password')
 api.do_login()
 
 # ---
 # API Methods:
 
+# returns all metering points (meter_ids) of the user
+metering_points = api.get_metering_points()
+# meter_id = metering_points[0].metering_point_id  # get meter_id dynamically via API
+
 # returns monthly aggregated data
 yearly_values = api.get_year(meter_id, 2023)
 # SmartmeterResultYearly(
-#   values={
-#     datetime.date(2023, 1, 1): 100.001,
+#   values=[
+#     (datetime.date(2023, 1, 1), 100.001),
 #     ...
-#   },
-#   peak_demands={
-#     datetime.datetime(2023, 2, 18, 17, 15, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): 2.101, 
+#   ],
+#   peak_demands=[
+#     (datetime.datetime(2023, 2, 18, 17, 15, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), 2.101), 
 #     ...
-#   },
-#   self_coverage={},
-#   self_coverage_renewable_energy={},
-#   grid_usage_leftover={},
-#   joint_tenancy_proportion={}
-#   blind_consumption={},
-#   blind_power_feed={},
+#   ],
+#   self_coverage=[],
+#   self_coverage_renewable_energy=[],
+#   grid_usage_leftover=[],
+#   joint_tenancy_proportion=[],
+#   blind_consumption=[],
+#   blind_power_feed=[]
 # )
 
 # returns daily aggregated data for the requested month
 monthly_values = api.get_month(meter_id, 2023, 3)
 # SmartmeterResult(
-#   metered={
-#     datetime.date(2023, 3, 1): 1.810, 
+#   metered=[
+#     (datetime.date(2023, 3, 1), 1.810), 
 #     ...
-#   },
-#   metered_peak_demands={
-#     datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): 0.012,
+#   ],
+#   metered_peak_demands=[
+#     (datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), 0.012),
 #     ...
-#   },
-#   peak_demand_data_qualities={
-#     datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')): SmartmeterDataQuality.L1,
-#   },
-#   estimated={},
-#   estimated_qualities={},
-#   estimated_peak_demands={},
-#   self_coverage={}, 
-#   self_coverage_renewable_energy={}, 
-#   grid_usage_leftover={},
-#   joint_tenancy_proportion={}, 
-#   quality_ec={},
-#   blind_consumption={},
-#   blind_power_feed={}
+#   ],
+#   peak_demand_data_qualities=[
+#     (datetime.datetime(2023, 3, 1, 22, 0, 0, tzinfo=zoneinfo.ZoneInfo(key='Europe/Vienna')), SmartmeterDataQuality.L1),
+#   ],
+#   estimated=[],
+#   estimated_qualities=[],
+#   estimated_peak_demands=[],
+#   self_coverage=[],
+#   self_coverage_renewable_energy=[], 
+#   grid_usage_leftover=[],
+#   joint_tenancy_proportion=[], 
+#   quality_ec=[],
+#   blind_consumption=[],
+#   blind_power_feed=[]
 # )
 
 # returns daily aggregated data for the requested time range
-weekly_values = api.get_week(meter_id, start_date=Date(2023, 1, 2), end_date=Date(2023, 1, 8))
+weekly_values = api.get_week(meter_id, start_date=date(2023, 1, 2), end_date=date(2023, 1, 8))
 
 # returns 15min values of the requested day
-daily_values = api.get_day(meter_id, day=Date(2023, 4, 1))
+daily_values = api.get_day(meter_id, day=date(2023, 4, 1))
 
 # logout of the api
 api.do_logout()
 ```
 
 ## Mapping between API fields and model fields
```

