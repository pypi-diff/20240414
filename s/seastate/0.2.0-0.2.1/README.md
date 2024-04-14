# Comparing `tmp/seastate-0.2.0.tar.gz` & `tmp/seastate-0.2.1.tar.gz`

## Comparing `seastate-0.2.0.tar` & `seastate-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 seastate-0.2.0/.flake8
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 seastate-0.2.0/Makefile
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 seastate-0.2.0/requirements.txt
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/exceptions.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/models.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/settings.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/__init__.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/api_mediator.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/base.py
--rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/noaa_ndbc.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/noaa_tidesandcurrents.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/api/rest_adapter.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/data/__init__.py
--rw-r--r--   0        0        0   179607 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/data/noaa_ndbc.json
--rw-r--r--   0        0        0    96988 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/data/noaa_tidesandcurrents.json
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 seastate-0.2.0/seastate/data/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/factories.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/test_seastate.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/test_seastate_regression.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/test_api_mediator.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/test_noaa_ndbc.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/test_noaa_tidesandcurrents.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/api/test_rest_adapter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/data/__init__.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/data/test___init__.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 seastate-0.2.0/tests/data/test_parsers.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 seastate-0.2.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 seastate-0.2.0/LICENSE
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 seastate-0.2.0/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 seastate-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 seastate-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 seastate-0.2.1/.flake8
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 seastate-0.2.1/Makefile
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 seastate-0.2.1/requirements.txt
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/exceptions.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/models.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/settings.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/api/__init__.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/api/api_mediator.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/api/base.py
+-rw-r--r--   0        0        0    11227 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/api/noaa_ndbc.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/api/noaa_tidesandcurrents.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/api/rest_adapter.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/data/__init__.py
+-rw-r--r--   0        0        0   179607 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/data/noaa_ndbc.json
+-rw-r--r--   0        0        0    96988 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/data/noaa_tidesandcurrents.json
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 seastate-0.2.1/seastate/data/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/factories.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/test_seastate.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/test_seastate_regression.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/api/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/api/test_api_mediator.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/api/test_noaa_ndbc.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/api/test_noaa_tidesandcurrents.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/api/test_rest_adapter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/data/__init__.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/data/test___init__.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 seastate-0.2.1/tests/data/test_parsers.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 seastate-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 seastate-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 seastate-0.2.1/README.md
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 seastate-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3503 2020-02-02 00:00:00.000000 seastate-0.2.1/PKG-INFO
```

### Comparing `seastate-0.2.0/Makefile` & `seastate-0.2.1/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Variables
 include .env
 export
 
 PACKAGE_NAME := seastate
-VERSION := 0.2.0
+VERSION := 0.2.1
 
 # Targets
 .PHONY: install test build clean publish-test publish-prod
 .PHONY: check-git-ready
 .PHONY: update-stations
 
 check-git-ready:
```

### Comparing `seastate-0.2.0/seastate/__init__.py` & `seastate-0.2.1/seastate/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,18 @@
             start = start.replace(hour=0, minute=0, second=0)
         if isinstance(end, datetime):
             end = end.replace(microsecond=0)
             end = end.replace(hour=23, minute=59, second=59)
 
         # log warning if end is before start
         if end < start:
-            self._logger.warning("end is after start")
+            self._logger.warning("end is after start, swapping values")
+            buffer = end
+            end = start
+            start = buffer
 
         return start, end
 
     def _get_mediator(self, measurement: str) -> ApiMediator:
         return self.__getattribute__(measurement)
 
     def _set_mediator(self, measurement: str) -> None:
@@ -70,18 +73,21 @@
             self.mediator_map[measurement] = tmp
 
     def _set_api_mediators(self) -> None:
         """set APIMediator as attribute for all implemented measurements"""
         for measurement in MEASUREMENTS:
             self._set_mediator(measurement)
 
-    def _get_data(self, key: str, start: datetime, end: datetime) -> list[Dict]:
+    def _measurement_from_date_range(
+        self, key: str, start: datetime, end: datetime
+    ) -> list[Dict]:
+        # selecting and configuring correct api mediator
         mediator = self._get_mediator(key)
         data = {}
-        data = mediator.api.measurement_from_date_range(
+        data = mediator.api._measurement_from_date_range(
             measurement=mediator.measurement,
             station_id=mediator.station.id,
             start=start,
             end=end,
         )
         return data
 
@@ -90,37 +96,26 @@
         start: Union[datetime, None] = None,
         end: Union[datetime, timedelta, None] = None,
     ) -> Dict:
         # process timeframe
         start, end = self._build_date_range(start, end)
 
         # makes an api call for each measurement,
-        # the idea is that the cache absorbs duplicate calls
-        # and the actual data is small so it's ok to reprocess
-        data = {
-            key: self._get_data(key, start, end) for key in self._requested_measurements
-        }
-
-        # previously, i manually built a dict with 7 api calls
-        # for each measurement
-        # get attribute.api
-        # call api.from_date_range on measurement, station, start, end
-        # gets measurement again
-        # gets staion again
-        # data = {}
-        # for measurement_key in MEASUREMENTS:
-        #     # access the configured api to generate response with hourly method
-        #     data[measurement_key] = self.__getattribute__(
-        #         measurement_key
-        #     ).api.measurement_from_date_range(
-        #         measurement=self.__getattribute__(measurement_key).measurement,
-        #         station_id=self.__getattribute__(measurement_key).station.id,
-        #         start=start,
-        #         end=end,
-        #     )
+        # the idea is that a cache with 59 second expiration
+        # absorbs the duplicated endpoint calls during a single method call
+        data = {}
+        for key in self._requested_measurements:
+            try:
+                data[key] = self._measurement_from_date_range(key, start, end)
+            except Exception as e:
+                self._logger.error(
+                    f"Error occurred while retrieving data for measurement {key}: {str(e)}"
+                )
+                data[key] = []
+
         return data
 
     def hourly(
         self,
         start: Union[datetime, None] = None,
         end: Union[datetime, timedelta, None] = None,
     ) -> Dict:
```

### Comparing `seastate-0.2.0/seastate/models.py` & `seastate-0.2.1/seastate/models.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/seastate/utils.py` & `seastate-0.2.1/seastate/utils.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/seastate/api/api_mediator.py` & `seastate-0.2.1/seastate/api/api_mediator.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/seastate/api/base.py` & `seastate-0.2.1/seastate/api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         """filename of the API module used internally as the id"""
         id = self.__module__.split(".")[-1]
         # integration check
         if id not in DATASOURCES:
             raise SeaStateException(f"API filename {id} does not match DATASOURCES")
         return id
 
-    def measurement_from_date_range(
+    def _measurement_from_date_range(
         self, measurement: str, station_id: str, start: datetime, end: datetime
     ) -> list[Dict]:
         # build endpoint
         ep, ep_params = self._build_endpoint(measurement, station_id, start, end)
         # get result
         result = self._get_result(ep, ep_params)
         # parse result to data
```

### Comparing `seastate-0.2.0/seastate/api/noaa_ndbc.py` & `seastate-0.2.1/seastate/api/noaa_ndbc.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/seastate/api/noaa_tidesandcurrents.py` & `seastate-0.2.1/seastate/api/noaa_tidesandcurrents.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,31 +71,27 @@
         #
         if len(result) > 1:
             raise SeaStateException(
                 "TidesAndCurrentsApi doesn't support multiple results"
             )
         try:
             parse_key = self._build_parse_key(measurement)
+            # checking payload for error message first
             if result[0].data.get("error"):
-                self._logger.error("TidesAndCurrentsApi error, returning empty data")
-                self._logger.error(f"{measurement}:{result[0].data}")
+                self._logger.error(
+                    f"TidesAndCurrentsApi error, returning empty data\n{measurement}:{result[0].data}"
+                )
                 return []
+            # parsing
             data = result[0].data[parse_key]
         except KeyError as e:
-            self._logger.exception(result.data)
+            msg = f"{e} unpacking {measurement} with key: {parse_key}\n{result[0].data}"
+            self._logger.error(msg=msg)
             raise SeaStateException("TidesAndCurrentsApi unpacking error") from e
 
         if len(data) == 0:
             self._logger.warning(
                 f"No {measurement} data recovered for daterange:\
                     {str(start.date())} : {str(end.date())}"
             )
 
         return data
-
-
-if __name__ == "__main__":
-    api = TidesAndCurrentsApi()
-    result = api.hourly("wind", 9410230, datetime.today(), datetime.today())
-    print(result)
-    result = api.hourly(9410230, datetime.today(), datetime.today(), "air_temp")
-    result = api.hourly(9410230, datetime.today(), datetime.today(), "water_temp")
```

### Comparing `seastate-0.2.0/seastate/api/rest_adapter.py` & `seastate-0.2.1/seastate/api/rest_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import requests.packages
 from requests_cache import CachedSession
 from seastate.exceptions import SeaStateException
 from seastate.models import Result
 
 
 class RestAdapter:
-    session = CachedSession("seastate_cache", backend="filesystem", use_cache_dir=True)
+    session = CachedSession(
+        "seastate_cache", backend="filesystem", use_cache_dir=True, expire_after=59
+    )
 
     def __init__(
         self,
         hostname: str,
         api_key: str = None,
         ssl_verify: bool = True,
         logger: logging.Logger = None,
@@ -47,15 +49,17 @@
             Result: Simplified http.Response object with:
                 status_code
                 message
                 data
         """
         full_url = self.url + endpoint
         headers = {"x-api-key": self._api_key}
-        log_line_pre = f"method={http_method}, url={full_url}, params={ep_params}"
+        log_line_pre = (
+            f"request: method={http_method}, url={full_url}, params={ep_params}"
+        )
         log_line_post = "result: success={}, status_code={}, message={}"
         # Log HTTP params and try HTTP request
         try:
             self._logger.debug(msg=log_line_pre)
             # response = requests.request(
             response = self.session.request(
                 method=http_method,
@@ -88,17 +92,20 @@
         is_success = 299 >= response.status_code >= 200
         log_line = log_line_post.format(
             is_success, response.status_code, response.reason
         )
         # if status code in 200-299 range, return Result, else raise exception
         if is_success:
             self._logger.debug(msg=log_line)
+            self._logger.debug(msg=log_line_pre)
             return Result(response.status_code, message=response.reason, data=data_out)
+        # else, error has occured
+        log_line += f"\n{log_line_pre}"  # enrich error msg
         self._logger.error(msg=log_line)
-        raise SeaStateException(f"{response.status_code}: {response.reason}")
+        raise SeaStateException(log_line)
 
     def get(self, endpoint: str, ep_params: Union[Dict, None] = None) -> Result:
         """GET method for RestAdapter
 
         Args:
             endpoint (str): target endpoint
             ep_params (Dict, optional): key:value API parameters. Defaults to None.
```

### Comparing `seastate-0.2.0/seastate/data/__init__.py` & `seastate-0.2.1/seastate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/seastate/data/noaa_ndbc.json` & `seastate-0.2.1/seastate/data/noaa_ndbc.json`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/seastate/data/noaa_tidesandcurrents.json` & `seastate-0.2.1/seastate/data/noaa_tidesandcurrents.json`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/seastate/data/parsers.py` & `seastate-0.2.1/seastate/data/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             while " " in line:
                 line.remove(" ")
             while "" in line:
                 line.remove("")
 
             # skip corrupted lines
             if len(line) != 22:
-                self._logger.info("No station info in this line: " + str(line))
+                self._logger.info(f"No station info in this line: {str(line)}")
                 continue
 
             # parse stationID, gps, and confirm active measurement sources
             # 'MM' is NOAA's notation for missing measurement
             tmp_station = {
                 "id": line[0],
                 "lat": float(line[1]),
@@ -102,16 +102,16 @@
                     line.getElementsByTagName("lat")[0].firstChild.nodeValue
                 )
                 tmp_station["lon"] = float(
                     line.getElementsByTagName("long")[0].firstChild.nodeValue
                 )
                 tmp_station["api"] = TidesAndCurrentsApi().id
             except IndexError as e:
-                # Faulty station, skip station node
-                self._logger.warn(e + str(line))
+                # Faulty tides and currents station, skip station row
+                self._logger.warn(f"{e}: {str(line)}")
                 continue
 
             # separate loop to parse individual measurements
             for m in line.getElementsByTagName("parameter"):
                 name = m.attributes["name"].value
                 status = True if m.attributes["status"].value == "1" else False
                 if "Water Level" in name and status:
```

### Comparing `seastate-0.2.0/tests/test_seastate.py` & `seastate-0.2.1/tests/test_seastate.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/tests/test_seastate_regression.py` & `seastate-0.2.1/tests/test_seastate_regression.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/tests/api/test_noaa_ndbc.py` & `seastate-0.2.1/tests/api/test_noaa_ndbc.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/tests/api/test_rest_adapter.py` & `seastate-0.2.1/tests/api/test_rest_adapter.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/tests/data/test_parsers.py` & `seastate-0.2.1/tests/data/test_parsers.py`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/.gitignore` & `seastate-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/LICENSE` & `seastate-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/README.md` & `seastate-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `seastate-0.2.0/pyproject.toml` & `seastate-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "seastate"
-version = "0.2.0"
+version = "0.2.1"
 authors = [{ name = "Ivo Rivetta", email = "ivo@ivorivetta.com" }]
 description = "Collect ocean measurements for location and timeframe. Integrates NDBC and TidesAndCurrents datasources."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = [
     "ocean",
     "tides",
     "currents",
+    "wind",
+    "temperature",
     "ndbc",
+    "noaa",
     "weather",
     "forecast",
     "marine",
     "data",
     "api",
 ]
```

### Comparing `seastate-0.2.0/PKG-INFO` & `seastate-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: seastate
-Version: 0.2.0
+Version: 0.2.1
 Summary: Collect ocean measurements for location and timeframe. Integrates NDBC and TidesAndCurrents datasources.
 Project-URL: Homepage, https://github.com/ivorivetta/seastate
 Project-URL: Issues, https://github.com/ivorivetta/seastate/issues
 Author-email: Ivo Rivetta <ivo@ivorivetta.com>
 License-File: LICENSE
-Keywords: api,currents,data,forecast,marine,ndbc,ocean,tides,weather
+Keywords: api,currents,data,forecast,marine,ndbc,noaa,ocean,temperature,tides,weather,wind
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 
 # seastate
```

