# Comparing `tmp/solaredge2mqtt-1.0.8.tar.gz` & `tmp/solaredge2mqtt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solaredge2mqtt-1.0.8.tar", last modified: Mon Apr  8 20:47:16 2024, max compression
+gzip compressed data, was "solaredge2mqtt-1.0.9.tar", last modified: Sun Apr 14 13:08:57 2024, max compression
```

## Comparing `solaredge2mqtt-1.0.8.tar` & `solaredge2mqtt-1.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12338 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/THIRD-PARTY-NOTICES
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.523429 solaredge2mqtt-1.0.8/solaredge2mqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/solaredge2mqtt/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.527429 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/actual_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/aggregate.flux
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.527429 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/fix_0.20.1.flux
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/import-historic-monitoring_data_1.0.8.flux
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/refactor_money_fields_1.0.8.flux
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/forecast_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/historic_unit.flux
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/production.flux
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/reduce.flux
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/flux/training_data.flux
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.527429 solaredge2mqtt-1.0.8/solaredge2mqtt/models/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/historic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/powerflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/wallbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/models/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/solaredge2mqtt/service/
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23450 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/wallbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/service/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/solaredge2mqtt/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:47:16.531429 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13604 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 20:47:16.000000 solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-08 20:47:07.000000 solaredge2mqtt-1.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/THIRD-PARTY-NOTICES
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.370267 solaredge2mqtt-1.0.9/solaredge2mqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/solaredge2mqtt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.370267 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/actual_unit.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/aggregate.flux
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.370267 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/fix_0.20.1.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/import-historic-monitoring_data_1.0.8.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/refactor_money_fields_1.0.8.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/forecast_unit.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/historic_unit.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/production.flux
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/reduce.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/flux/training_data.flux
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/solaredge2mqtt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/historic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/powerflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/wallbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/models/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/solaredge2mqtt/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23676 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/wallbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/service/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/solaredge2mqtt/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:08:57.374266 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 13:08:57.000000 solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-14 13:08:52.000000 solaredge2mqtt-1.0.9/versioneer.py
```

### Comparing `solaredge2mqtt-1.0.8/LICENSE` & `solaredge2mqtt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/PKG-INFO` & `solaredge2mqtt-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge2mqtt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Read data from SolarEdge Inverter and publish it to MQTT
 Home-page: https://github.com/deroetzi/solaredge2mqtt
 Author: Johannes Ott
 Author-email: info@johannes-ott.net
 Project-URL: Bug Reports, https://github.com/deroetzi/solaredge2mqtt/issues
 Keywords: smart home
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,40 +14,41 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: solaredge_modbus==0.8.0
-Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic==2.7.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: influxdb-client==1.41.0
 Requires-Dist: pyjwt==2.8.0
 Requires-Dist: aiomqtt==2.0.1
 Requires-Dist: numpy==1.26.4
-Requires-Dist: pandas==2.2.1
-Requires-Dist: scikit-learn==1.4.1.post1
+Requires-Dist: pandas==2.2.2
+Requires-Dist: scikit-learn==1.4.2
 Requires-Dist: scipy==1.13.0rc1
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.4
 Requires-Dist: aiocsv==1.3.1
 Requires-Dist: astral==3.2
 Requires-Dist: ephem==4.1.5
 Requires-Dist: tzlocal==5.2
 
 # SolarEdge 2 MQTT Service
+
 [![License](https://img.shields.io/github/license/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/blob/main/LICENSE) [![Release](https://img.shields.io/github/v/release/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/releases/latest) [![Build Status](https://img.shields.io/github/actions/workflow/status/DerOetzi/solaredge2mqtt/build_project.yml?branch=main)](https://github.com/DerOetzi/solaredge2mqtt/actions/workflows/build_project.yml) [![PyPI version](https://img.shields.io/pypi/v/solaredge2mqtt.svg)](https://pypi.org/project/solaredge2mqtt/) [![Discord Chat](https://img.shields.io/discord/1196540254686032014)](https://discord.gg/QXfghc93pY)
 
 The SolarEdge2MQTT service facilitates the retrieval of power data from SolarEdge inverters and its publication to an MQTT broker. Ideal for integrating SolarEdge inverters into home automation systems, this service supports real-time monitoring of power flow and additional parameters via Modbus.
 
 Users can optionally collect panel energy production data directly from the SolarEdge monitoring site, without employing the API, by leveraging their monitoring platform account.
 
 It also enables the monitoring of SolarEdge Wallbox via the REST API and supports saving all values into InfluxDB for advanced visualization.
 
-*Please note: The SolarEdge2MQTT service is in its early development stages. Although operational for reading and publishing data from a SolarEdge inverter, active development may introduce changes to features, potential removals, or bugs. Users are advised to proceed with caution. As an open-source project, contributions are highly encouraged.*
+_Please note: The SolarEdge2MQTT service is in its early development stages. Although operational for reading and publishing data from a SolarEdge inverter, active development may introduce changes to features, potential removals, or bugs. Users are advised to proceed with caution. As an open-source project, contributions are highly encouraged._
 
 ## Contact and Feedback
 
 For inquiries, feel free to reach out on Discord.
 
 [![Discord Banner](https://discordapp.com/api/guilds/1196540254686032014/widget.png?style=banner2)](https://discord.gg/QXfghc93pY)
 
@@ -59,87 +60,92 @@
 
 Configure the service using environment variables. The available options are listed below for customization:
 
 ### Basic configuration
 
 - **SE2MQTT_INTERVAL**: The frequency (in seconds) of data retrieval requests. Default is every 5 seconds.
 - **SE2MQTT_LOGGING_LEVEL**: Adjust the verbosity of logs. Options include DEBUG, INFO, WARNING, ERROR, and CRITICAL.
-- **SE2MQTT_LOCATION__LATITUDE** and **SE2MQTT_LOCATION__LONGITUDE**: Specify your location to enable weather and forecast services. These settings are essential for accurate environmental data and PV production forecasts.
+- **SE2MQTT_LOCATION\_\_LATITUDE** and **SE2MQTT_LOCATION\_\_LONGITUDE**: Specify your location to enable weather and forecast services. These settings are essential for accurate environmental data and PV production forecasts.
 
 ### Modbus configuration
 
-- **SE2MQTT_MODBUS__HOST**: The IP address of your SolarEdge inverter.
-- **SE2MQTT_MODBUS__PORT**: The port on which your inverter's Modbus is accessible. Default is 1502.
-- **SE2MQTT_MODBUS__TIMEOUT**: The timeout (in seconds) for Modbus connections. A lower value makes the system more responsive but may lead to incomplete data in environments with poor network conditions.
-- **SE2MQTT_MODBUS__UNIT**: The unit address for Modbus communication. Default is 1.
+- **SE2MQTT_MODBUS\_\_HOST**: The IP address of your SolarEdge inverter.
+- **SE2MQTT_MODBUS\_\_PORT**: The port on which your inverter's Modbus is accessible. Default is 1502.
+- **SE2MQTT_MODBUS\_\_TIMEOUT**: The timeout (in seconds) for Modbus connections. A lower value makes the system more responsive but may lead to incomplete data in environments with poor network conditions.
+- **SE2MQTT_MODBUS\_\_UNIT**: The unit address for Modbus communication. Default is 1.
 
 ### MQTT configuration
 
-- **SE2MQTT_MQTT__CLIENT_ID**: Identifier for the MQTT client, defaults to 'solaredge2mqtt'.
-- **SE2MQTT_MQTT__BROKER**: The IP address of your MQTT broker.
-- **SE2MQTT_MQTT__PORT**: The port your MQTT broker listens on. Default is 1883.
-- **SE2MQTT_MQTT__USERNAME** and **SE2MQTT_MQTT__PASSWORD**: Credentials for connecting to your MQTT broker. It's recommended to use secrets for the password if deploying with Docker.
-- **SE2MQTT_MQTT__TOPIC_PREFIX**: The prefix used for MQTT topics. Defaults to 'solaredge'.
+- **SE2MQTT_MQTT\_\_CLIENT_ID**: Identifier for the MQTT client, defaults to 'solaredge2mqtt'.
+- **SE2MQTT_MQTT\_\_BROKER**: The IP address of your MQTT broker.
+- **SE2MQTT_MQTT\_\_PORT**: The port your MQTT broker listens on. Default is 1883.
+- **SE2MQTT_MQTT\_\_USERNAME** and **SE2MQTT_MQTT\_\_PASSWORD**: Credentials for connecting to your MQTT broker. It's recommended to use secrets for the password if deploying with Docker.
+- **SE2MQTT_MQTT\_\_TOPIC_PREFIX**: The prefix used for MQTT topics. Defaults to 'solaredge'.
 
 ### Monitoring
 
 To enable panel energy value retrieval from the SolarEdge monitoring platform, you must configure:
 
-- **SE2MQTT_MONITORING__SITE_ID**: Your site ID as registered on the SolarEdge platform.
-- **SE2MQTT_MONITORING__USERNAME**: Your username for the SolarEdge monitoring platform.
-- **SE2MQTT_MONITORING__PASSWORD**: Your password. Ensure to use Docker secrets or a secure method to protect this information.
+- **SE2MQTT_MONITORING\_\_SITE_ID**: Your site ID as registered on the SolarEdge platform.
+- **SE2MQTT_MONITORING\_\_USERNAME**: Your username for the SolarEdge monitoring platform.
+- **SE2MQTT_MONITORING\_\_PASSWORD**: Your password. Ensure to use Docker secrets or a secure method to protect this information.
 
 ### Wallbox
 
 For monitoring SolarEdge Wallbox, provide:
 
-- **SE2MQTT_WALLBOX__HOST**: The IP address of your Wallbox.
-- **SE2MQTT_WALLBOX__PASSWORD**: The admin password for Wallbox web UI access.
-- **SE2MQTT_WALLBOX__SERIAL**: The serial number of your Wallbox.
+- **SE2MQTT_WALLBOX\_\_HOST**: The IP address of your Wallbox.
+- **SE2MQTT_WALLBOX\_\_PASSWORD**: The admin password for Wallbox web UI access.
+- **SE2MQTT_WALLBOX\_\_SERIAL**: The serial number of your Wallbox.
 
 ### InfluxDB
 
 Configure your InfluxDB settings with these environment variables to store monitoring data effectively:
 
-- **SE2MQTT_INFLUXDB__HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
-- **SE2MQTT_INFLUXDB__PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
-- **SE2MQTT_INFLUXDB__TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
-- **SE2MQTT_INFLUXDB__ORG**: The ID of your organization within InfluxDB. Default is None.
-- **SE2MQTT_INFLUXDB__BUCKET**: The name of the bucket where the data will be saved. Default bucket name is solaredge.
-- **SE2MQTT_INFLUXDB__RETENTION_RAW**: The retention policy for raw data in hours. This setting defines how long the raw power values are stored in InfluxDB. Default is 25 hours.
-- **SE2MQTT_INFLUXDB__RETENTION**: The retention policy for aggregated data in seconds. This sets how long the aggregated data will be stored in InfluxDB, with the default being 2 years (63072000 seconds).
-These configurations allow you to tailor the InfluxDB storage for your SolarEdge monitoring data, ensuring that you have the flexibility to define how long the data should be retained both in raw and aggregated forms.
+- **SE2MQTT_INFLUXDB\_\_HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
+- **SE2MQTT_INFLUXDB\_\_PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
+- **SE2MQTT_INFLUXDB\_\_TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
+- **SE2MQTT_INFLUXDB\_\_ORG**: The ID of your organization within InfluxDB. Default is None.
+- **SE2MQTT_INFLUXDB\_\_BUCKET**: The name of the bucket where the data will be saved. Default bucket name is solaredge.
+- **SE2MQTT_INFLUXDB\_\_RETENTION_RAW**: The retention policy for raw data in hours. This setting defines how long the raw power values are stored in InfluxDB. Default is 25 hours.
+- **SE2MQTT_INFLUXDB\_\_RETENTION**: The retention policy for aggregated data in seconds. This sets how long the aggregated data will be stored in InfluxDB, with the default being 2 years (63072000 seconds).
+  These configurations allow you to tailor the InfluxDB storage for your SolarEdge monitoring data, ensuring that you have the flexibility to define how long the data should be retained both in raw and aggregated forms.
 
 ### Price Configuration
+
 To calculate your savings and earnings, you can specify the amount you pay for consumption and the amount you receive for delivery per kilowatt-hour (kWh). Please note, this feature is only operational in conjunction with InfluxDB.
 
-- **SE2MQTT_PRICES__CONSUMPTION**: Set the price you pay per 1 kWh for energy received from the grid.
-- **SE2MQTT_PRICES__DELIVERY**: Set the price you receive per 1 kWh for energy delivered to the grid.
+- **SE2MQTT_PRICES\_\_CONSUMPTION**: Set the price you pay per 1 kWh for energy received from the grid.
+- **SE2MQTT_PRICES\_\_DELIVERY**: Set the price you receive per 1 kWh for energy delivered to the grid.
 
 These additional settings allow for a comprehensive analysis of your energy production and usage, enabling you not just to monitor energy flow but also understand the financial aspects of your energy generation and consumption.
 
 ### Weather
 
 Leverage real-time weather data in your SolarEdge2MQTT service by integrating with OpenWeatherMap. This feature enriches your service with accurate environmental conditions, which can be essential for detailed energy production analysis.
 
-- **SE2MQTT_WEATHER__API_KEY**: Securely set your OpenWeatherMap OneCall API key here. For enhanced security, it's recommended to use this key as a secret within Docker environments.
-- **SE2MQTT_WEATHER__LANGUAGE**: Customize the language for weather data retrieved from the API. The default setting is English (en).
+- **SE2MQTT_WEATHER\_\_API_KEY**: Securely set your OpenWeatherMap OneCall API key here. For enhanced security, it's recommended to use this key as a secret within Docker environments.
+- **SE2MQTT_WEATHER\_\_LANGUAGE**: Customize the language for weather data retrieved from the API. The default setting is English (en).
 
-To access current weather data, ensure you have an OpenWeatherMap account, an API key, and a subscription to the One-Call API. Visit [OpenWeatherMap](https://openweathermap.org/) for more information on obtaining these prerequisites.
+To access current weather data, ensure you have an OpenWeatherMap account, an API key, and a [subscription](https://home.openweathermap.org/subscriptions) to the One-Call API. Visit [OpenWeatherMap](https://openweathermap.org/) for more information on obtaining these prerequisites.
 
 ### Forecast
 
 The SolarEdge2MQTT service features an integrated machine learning component designed to forecast PV production for the current and following day. For optimal functionality, confirm that your settings for [location](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#basic-configuration), [InfluxDB](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#influxdb) and [weather](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#weather) are correctly configured.
 
-- **SE2MQTT_FORECAST__ENABLE**: Activate the machine learning-based forecast feature by setting this to true. The default is false.
-- **SE2MQTT_FORECAST__HYPERPARAMETERTUNING**: Optimize forecast accuracy by enabling hyperparameter tuning. Note that this process is computationally intensive and may not be suitable for devices with limited processing power, such as Raspberry Pi. The default setting is false.
+- **SE2MQTT_FORECAST\_\_ENABLE**: Activate the machine learning-based forecast feature by setting this to true. The default is false.
+- **SE2MQTT_FORECAST\_\_HYPERPARAMETERTUNING**: Optimize forecast accuracy by enabling hyperparameter tuning. Note that this process is computationally intensive and may not be suitable for devices with limited processing power, such as Raspberry Pi. The default setting is false.
+
+**Precondition for Forecasting**: Before a forecast can be made, a minimum of 60 hours of training data must be collected. These data serve as the basis for model training and are crucial for prediction accuracy. Ensure that the service has had sufficient time to collect data before expecting forecast activation.
+
+**Note on Training Data Collection**: If the service goes without recording production data for longer than an hour, it will be unable to save training data. It's essential to ensure consistent data recording to maintain the integrity of the training process and ensure accurate forecasting.
 
-*Your experience and feedback, especially regarding forecast accuracy and performance on low-powered devices, are highly valued. This continuous improvement effort aims to enhance the predictive capabilities of the SolarEdge2MQTT service for all users.*
+_Your experience and feedback, especially regarding forecast accuracy and performance on low-powered devices, are highly valued. This continuous improvement effort aims to enhance the predictive capabilities of the SolarEdge2MQTT service for all users._
 
-## Running the service 
+## Running the service
 
 Each of these methods provides a different level of control and isolation, catering to various use cases from development and testing to full-scale production deployment.
 
 ### In the Console
 
 For users looking to run SolarEdge2MQTT directly within their console, which is ideal for testing or development environments, follow these steps:
```

### Comparing `solaredge2mqtt-1.0.8/README.md` & `solaredge2mqtt-1.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SolarEdge 2 MQTT Service
+
 [![License](https://img.shields.io/github/license/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/blob/main/LICENSE) [![Release](https://img.shields.io/github/v/release/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/releases/latest) [![Build Status](https://img.shields.io/github/actions/workflow/status/DerOetzi/solaredge2mqtt/build_project.yml?branch=main)](https://github.com/DerOetzi/solaredge2mqtt/actions/workflows/build_project.yml) [![PyPI version](https://img.shields.io/pypi/v/solaredge2mqtt.svg)](https://pypi.org/project/solaredge2mqtt/) [![Discord Chat](https://img.shields.io/discord/1196540254686032014)](https://discord.gg/QXfghc93pY)
 
 The SolarEdge2MQTT service facilitates the retrieval of power data from SolarEdge inverters and its publication to an MQTT broker. Ideal for integrating SolarEdge inverters into home automation systems, this service supports real-time monitoring of power flow and additional parameters via Modbus.
 
 Users can optionally collect panel energy production data directly from the SolarEdge monitoring site, without employing the API, by leveraging their monitoring platform account.
 
 It also enables the monitoring of SolarEdge Wallbox via the REST API and supports saving all values into InfluxDB for advanced visualization.
 
-*Please note: The SolarEdge2MQTT service is in its early development stages. Although operational for reading and publishing data from a SolarEdge inverter, active development may introduce changes to features, potential removals, or bugs. Users are advised to proceed with caution. As an open-source project, contributions are highly encouraged.*
+_Please note: The SolarEdge2MQTT service is in its early development stages. Although operational for reading and publishing data from a SolarEdge inverter, active development may introduce changes to features, potential removals, or bugs. Users are advised to proceed with caution. As an open-source project, contributions are highly encouraged._
 
 ## Contact and Feedback
 
 For inquiries, feel free to reach out on Discord.
 
 [![Discord Banner](https://discordapp.com/api/guilds/1196540254686032014/widget.png?style=banner2)](https://discord.gg/QXfghc93pY)
 
@@ -23,87 +24,92 @@
 
 Configure the service using environment variables. The available options are listed below for customization:
 
 ### Basic configuration
 
 - **SE2MQTT_INTERVAL**: The frequency (in seconds) of data retrieval requests. Default is every 5 seconds.
 - **SE2MQTT_LOGGING_LEVEL**: Adjust the verbosity of logs. Options include DEBUG, INFO, WARNING, ERROR, and CRITICAL.
-- **SE2MQTT_LOCATION__LATITUDE** and **SE2MQTT_LOCATION__LONGITUDE**: Specify your location to enable weather and forecast services. These settings are essential for accurate environmental data and PV production forecasts.
+- **SE2MQTT_LOCATION\_\_LATITUDE** and **SE2MQTT_LOCATION\_\_LONGITUDE**: Specify your location to enable weather and forecast services. These settings are essential for accurate environmental data and PV production forecasts.
 
 ### Modbus configuration
 
-- **SE2MQTT_MODBUS__HOST**: The IP address of your SolarEdge inverter.
-- **SE2MQTT_MODBUS__PORT**: The port on which your inverter's Modbus is accessible. Default is 1502.
-- **SE2MQTT_MODBUS__TIMEOUT**: The timeout (in seconds) for Modbus connections. A lower value makes the system more responsive but may lead to incomplete data in environments with poor network conditions.
-- **SE2MQTT_MODBUS__UNIT**: The unit address for Modbus communication. Default is 1.
+- **SE2MQTT_MODBUS\_\_HOST**: The IP address of your SolarEdge inverter.
+- **SE2MQTT_MODBUS\_\_PORT**: The port on which your inverter's Modbus is accessible. Default is 1502.
+- **SE2MQTT_MODBUS\_\_TIMEOUT**: The timeout (in seconds) for Modbus connections. A lower value makes the system more responsive but may lead to incomplete data in environments with poor network conditions.
+- **SE2MQTT_MODBUS\_\_UNIT**: The unit address for Modbus communication. Default is 1.
 
 ### MQTT configuration
 
-- **SE2MQTT_MQTT__CLIENT_ID**: Identifier for the MQTT client, defaults to 'solaredge2mqtt'.
-- **SE2MQTT_MQTT__BROKER**: The IP address of your MQTT broker.
-- **SE2MQTT_MQTT__PORT**: The port your MQTT broker listens on. Default is 1883.
-- **SE2MQTT_MQTT__USERNAME** and **SE2MQTT_MQTT__PASSWORD**: Credentials for connecting to your MQTT broker. It's recommended to use secrets for the password if deploying with Docker.
-- **SE2MQTT_MQTT__TOPIC_PREFIX**: The prefix used for MQTT topics. Defaults to 'solaredge'.
+- **SE2MQTT_MQTT\_\_CLIENT_ID**: Identifier for the MQTT client, defaults to 'solaredge2mqtt'.
+- **SE2MQTT_MQTT\_\_BROKER**: The IP address of your MQTT broker.
+- **SE2MQTT_MQTT\_\_PORT**: The port your MQTT broker listens on. Default is 1883.
+- **SE2MQTT_MQTT\_\_USERNAME** and **SE2MQTT_MQTT\_\_PASSWORD**: Credentials for connecting to your MQTT broker. It's recommended to use secrets for the password if deploying with Docker.
+- **SE2MQTT_MQTT\_\_TOPIC_PREFIX**: The prefix used for MQTT topics. Defaults to 'solaredge'.
 
 ### Monitoring
 
 To enable panel energy value retrieval from the SolarEdge monitoring platform, you must configure:
 
-- **SE2MQTT_MONITORING__SITE_ID**: Your site ID as registered on the SolarEdge platform.
-- **SE2MQTT_MONITORING__USERNAME**: Your username for the SolarEdge monitoring platform.
-- **SE2MQTT_MONITORING__PASSWORD**: Your password. Ensure to use Docker secrets or a secure method to protect this information.
+- **SE2MQTT_MONITORING\_\_SITE_ID**: Your site ID as registered on the SolarEdge platform.
+- **SE2MQTT_MONITORING\_\_USERNAME**: Your username for the SolarEdge monitoring platform.
+- **SE2MQTT_MONITORING\_\_PASSWORD**: Your password. Ensure to use Docker secrets or a secure method to protect this information.
 
 ### Wallbox
 
 For monitoring SolarEdge Wallbox, provide:
 
-- **SE2MQTT_WALLBOX__HOST**: The IP address of your Wallbox.
-- **SE2MQTT_WALLBOX__PASSWORD**: The admin password for Wallbox web UI access.
-- **SE2MQTT_WALLBOX__SERIAL**: The serial number of your Wallbox.
+- **SE2MQTT_WALLBOX\_\_HOST**: The IP address of your Wallbox.
+- **SE2MQTT_WALLBOX\_\_PASSWORD**: The admin password for Wallbox web UI access.
+- **SE2MQTT_WALLBOX\_\_SERIAL**: The serial number of your Wallbox.
 
 ### InfluxDB
 
 Configure your InfluxDB settings with these environment variables to store monitoring data effectively:
 
-- **SE2MQTT_INFLUXDB__HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
-- **SE2MQTT_INFLUXDB__PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
-- **SE2MQTT_INFLUXDB__TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
-- **SE2MQTT_INFLUXDB__ORG**: The ID of your organization within InfluxDB. Default is None.
-- **SE2MQTT_INFLUXDB__BUCKET**: The name of the bucket where the data will be saved. Default bucket name is solaredge.
-- **SE2MQTT_INFLUXDB__RETENTION_RAW**: The retention policy for raw data in hours. This setting defines how long the raw power values are stored in InfluxDB. Default is 25 hours.
-- **SE2MQTT_INFLUXDB__RETENTION**: The retention policy for aggregated data in seconds. This sets how long the aggregated data will be stored in InfluxDB, with the default being 2 years (63072000 seconds).
-These configurations allow you to tailor the InfluxDB storage for your SolarEdge monitoring data, ensuring that you have the flexibility to define how long the data should be retained both in raw and aggregated forms.
+- **SE2MQTT_INFLUXDB\_\_HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
+- **SE2MQTT_INFLUXDB\_\_PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
+- **SE2MQTT_INFLUXDB\_\_TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
+- **SE2MQTT_INFLUXDB\_\_ORG**: The ID of your organization within InfluxDB. Default is None.
+- **SE2MQTT_INFLUXDB\_\_BUCKET**: The name of the bucket where the data will be saved. Default bucket name is solaredge.
+- **SE2MQTT_INFLUXDB\_\_RETENTION_RAW**: The retention policy for raw data in hours. This setting defines how long the raw power values are stored in InfluxDB. Default is 25 hours.
+- **SE2MQTT_INFLUXDB\_\_RETENTION**: The retention policy for aggregated data in seconds. This sets how long the aggregated data will be stored in InfluxDB, with the default being 2 years (63072000 seconds).
+  These configurations allow you to tailor the InfluxDB storage for your SolarEdge monitoring data, ensuring that you have the flexibility to define how long the data should be retained both in raw and aggregated forms.
 
 ### Price Configuration
+
 To calculate your savings and earnings, you can specify the amount you pay for consumption and the amount you receive for delivery per kilowatt-hour (kWh). Please note, this feature is only operational in conjunction with InfluxDB.
 
-- **SE2MQTT_PRICES__CONSUMPTION**: Set the price you pay per 1 kWh for energy received from the grid.
-- **SE2MQTT_PRICES__DELIVERY**: Set the price you receive per 1 kWh for energy delivered to the grid.
+- **SE2MQTT_PRICES\_\_CONSUMPTION**: Set the price you pay per 1 kWh for energy received from the grid.
+- **SE2MQTT_PRICES\_\_DELIVERY**: Set the price you receive per 1 kWh for energy delivered to the grid.
 
 These additional settings allow for a comprehensive analysis of your energy production and usage, enabling you not just to monitor energy flow but also understand the financial aspects of your energy generation and consumption.
 
 ### Weather
 
 Leverage real-time weather data in your SolarEdge2MQTT service by integrating with OpenWeatherMap. This feature enriches your service with accurate environmental conditions, which can be essential for detailed energy production analysis.
 
-- **SE2MQTT_WEATHER__API_KEY**: Securely set your OpenWeatherMap OneCall API key here. For enhanced security, it's recommended to use this key as a secret within Docker environments.
-- **SE2MQTT_WEATHER__LANGUAGE**: Customize the language for weather data retrieved from the API. The default setting is English (en).
+- **SE2MQTT_WEATHER\_\_API_KEY**: Securely set your OpenWeatherMap OneCall API key here. For enhanced security, it's recommended to use this key as a secret within Docker environments.
+- **SE2MQTT_WEATHER\_\_LANGUAGE**: Customize the language for weather data retrieved from the API. The default setting is English (en).
 
-To access current weather data, ensure you have an OpenWeatherMap account, an API key, and a subscription to the One-Call API. Visit [OpenWeatherMap](https://openweathermap.org/) for more information on obtaining these prerequisites.
+To access current weather data, ensure you have an OpenWeatherMap account, an API key, and a [subscription](https://home.openweathermap.org/subscriptions) to the One-Call API. Visit [OpenWeatherMap](https://openweathermap.org/) for more information on obtaining these prerequisites.
 
 ### Forecast
 
 The SolarEdge2MQTT service features an integrated machine learning component designed to forecast PV production for the current and following day. For optimal functionality, confirm that your settings for [location](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#basic-configuration), [InfluxDB](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#influxdb) and [weather](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#weather) are correctly configured.
 
-- **SE2MQTT_FORECAST__ENABLE**: Activate the machine learning-based forecast feature by setting this to true. The default is false.
-- **SE2MQTT_FORECAST__HYPERPARAMETERTUNING**: Optimize forecast accuracy by enabling hyperparameter tuning. Note that this process is computationally intensive and may not be suitable for devices with limited processing power, such as Raspberry Pi. The default setting is false.
+- **SE2MQTT_FORECAST\_\_ENABLE**: Activate the machine learning-based forecast feature by setting this to true. The default is false.
+- **SE2MQTT_FORECAST\_\_HYPERPARAMETERTUNING**: Optimize forecast accuracy by enabling hyperparameter tuning. Note that this process is computationally intensive and may not be suitable for devices with limited processing power, such as Raspberry Pi. The default setting is false.
+
+**Precondition for Forecasting**: Before a forecast can be made, a minimum of 60 hours of training data must be collected. These data serve as the basis for model training and are crucial for prediction accuracy. Ensure that the service has had sufficient time to collect data before expecting forecast activation.
+
+**Note on Training Data Collection**: If the service goes without recording production data for longer than an hour, it will be unable to save training data. It's essential to ensure consistent data recording to maintain the integrity of the training process and ensure accurate forecasting.
 
-*Your experience and feedback, especially regarding forecast accuracy and performance on low-powered devices, are highly valued. This continuous improvement effort aims to enhance the predictive capabilities of the SolarEdge2MQTT service for all users.*
+_Your experience and feedback, especially regarding forecast accuracy and performance on low-powered devices, are highly valued. This continuous improvement effort aims to enhance the predictive capabilities of the SolarEdge2MQTT service for all users._
 
-## Running the service 
+## Running the service
 
 Each of these methods provides a different level of control and isolation, catering to various use cases from development and testing to full-scale production deployment.
 
 ### In the Console
 
 For users looking to run SolarEdge2MQTT directly within their console, which is ideal for testing or development environments, follow these steps:
```

### Comparing `solaredge2mqtt-1.0.8/THIRD-PARTY-NOTICES` & `solaredge2mqtt-1.0.9/THIRD-PARTY-NOTICES`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/setup.py` & `solaredge2mqtt-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/actual_unit.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/actual_unit.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/aggregate.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/aggregate.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/fix_0.20.1.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/fix_0.20.1.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/import-historic-monitoring_data_1.0.8.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/import-historic-monitoring_data_1.0.8.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/fixes/refactor_money_fields_1.0.8.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/fixes/refactor_money_fields_1.0.8.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/forecast_unit.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/forecast_unit.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/historic_unit.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/historic_unit.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/production.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/production.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/flux/reduce.flux` & `solaredge2mqtt-1.0.9/solaredge2mqtt/flux/reduce.flux`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/logging.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/logging.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/__init__.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/base.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/base.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/forecast.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/forecast.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/historic.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/historic.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/modbus.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/modbus.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/monitoring.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/monitoring.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/powerflow.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/powerflow.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/wallbox.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/wallbox.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/models/weather.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/models/weather.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/mqtt.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/__init__.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     from a SolarEdge inverter and publishes it to an MQTT broker. It uses the asyncio 
     library for asynchronous I/O and the aiomqtt library for MQTT communication. 
     The module also includes a run function to initialize and start the service.
 """
 
 import asyncio as aio
 import signal
+import platform
 from time import time
 from typing import Callable
 
 from aiomqtt import MqttError
 
 from solaredge2mqtt import __version__
 from solaredge2mqtt.exceptions import ConfigurationException, InvalidDataException
@@ -84,14 +85,17 @@
         self.cancel_request.set()
         for loop in self.loops:
             loop.cancel()
 
     async def main_loop(self):
         logger.info("Starting SolarEdge2MQTT service...")
         logger.info("Version: {version}", version=__version__)
+        logger.info(
+            f"Operationg system: {platform.platform()} ({platform.system()}/{platform.machine()})"
+        )
         logger.debug(self.settings)
         logger.info("Timezone: {timezone}", timezone=LOCAL_TZ)
 
         if self.settings.is_influxdb_configured:
             self.influxdb.initialize_buckets()
 
         while not self.cancel_request.is_set():
```

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/base.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/base.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/forecast.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,18 @@
 
     def add_last_hour_pv_production(
         self, trainings_data
     ) -> dict[str, str | float | int | None]:
         production_data = self.influxdb.query_first("production")
 
         if production_data is None:
-            raise InvalidDataException("Missing production data for last 10 minutes")
+            raise InvalidDataException(
+                "Missing production data of last hour for forecast training."
+                + " Did the service write power information to InfluxDB?"
+            )
 
         trainings_data[ForecasterType.POWER.target_column] = round(
             production_data[ForecasterType.POWER.target_column]
         )
         trainings_data[ForecasterType.ENERGY.target_column] = round(
             production_data[ForecasterType.ENERGY.target_column], 2
         )
@@ -150,15 +153,15 @@
         if (
             not self.forecasters[ForecasterType.ENERGY].is_trained
             or not self.forecasters[ForecasterType.POWER].is_trained
         ):
             raise InvalidDataException("Forecast model is not trained yet")
 
         if self.last_weather_forecast is None:
-            raise InvalidDataException("Missing weather forecast for forecast")
+            raise InvalidDataException("Missing weather forecast for production forecast")
 
         estimation_data_list = [
             {
                 "time": datetime(
                     year=weather_forecast.year,
                     month=weather_forecast.month,
                     day=weather_forecast.day,
@@ -281,18 +284,22 @@
         self.location = location
         self.enable_hyperparameter_tuning = enable_hyperparameter_tuning
         self.model_pipeline: Pipeline = None
         self.training_completed: Event = Event()
 
     def train(self, data: DataFrame) -> None:
         data_count = len(data)
-        if data_count < 60:
-            raise InvalidDataException("Not enough data to train the model")
+        logger.info(
+            f"Training model {self.typed} with {data_count} hours of data points"
+        )
 
-        logger.info(f"Training model {self.typed} with {data_count} data points")
+        if data_count < 60:
+            raise InvalidDataException(
+                "Forecast needs at least 60 hours of data at least to start training",
+            )
 
         self.training_completed.clear()
         start_time = time.time()
         y_vector = data[self.typed.target_column]
 
         pipeline = self._prepare_model_pipeline(data.columns.to_list())
```

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/http.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/http.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/influxdb.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/influxdb.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/modbus.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/modbus.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/monitoring.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/monitoring.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/wallbox.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/wallbox.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/service/weather.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/service/weather.py`

 * *Files 23% similar despite different names*

```diff
@@ -38,14 +38,24 @@
                 },
                 timeout=7,
             )
 
             logger.trace(result)
 
             if result is None:
-                raise InvalidDataException("Unable to read weather data")
+                raise InvalidDataException(
+                    "Unable to read weather data from OpenWeatherMap"
+                )
 
             weather = OpenWeatherMapOneCall(**result)
 
             return weather
         except HTTPError as error:
-            raise InvalidDataException("Unable to read weather data") from error
+            status_code = error.response.status_code
+            if status_code == 401:
+                error_msg = (
+                    "Invalid OpenWeatherMap API key or no subscription to OneCall-API"
+                )
+            else:
+                error_msg = "Unable to read weather data from OpenWeatherMap (HTTP {status_code})"
+
+            raise InvalidDataException(error_msg) from error
```

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt/settings.py` & `solaredge2mqtt-1.0.9/solaredge2mqtt/settings.py`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/PKG-INFO` & `solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaredge2mqtt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Read data from SolarEdge Inverter and publish it to MQTT
 Home-page: https://github.com/deroetzi/solaredge2mqtt
 Author: Johannes Ott
 Author-email: info@johannes-ott.net
 Project-URL: Bug Reports, https://github.com/deroetzi/solaredge2mqtt/issues
 Keywords: smart home
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,40 +14,41 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: solaredge_modbus==0.8.0
-Requires-Dist: pydantic==2.6.4
+Requires-Dist: pydantic==2.7.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: influxdb-client==1.41.0
 Requires-Dist: pyjwt==2.8.0
 Requires-Dist: aiomqtt==2.0.1
 Requires-Dist: numpy==1.26.4
-Requires-Dist: pandas==2.2.1
-Requires-Dist: scikit-learn==1.4.1.post1
+Requires-Dist: pandas==2.2.2
+Requires-Dist: scikit-learn==1.4.2
 Requires-Dist: scipy==1.13.0rc1
-Requires-Dist: aiohttp==3.9.3
+Requires-Dist: aiohttp==3.9.4
 Requires-Dist: aiocsv==1.3.1
 Requires-Dist: astral==3.2
 Requires-Dist: ephem==4.1.5
 Requires-Dist: tzlocal==5.2
 
 # SolarEdge 2 MQTT Service
+
 [![License](https://img.shields.io/github/license/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/blob/main/LICENSE) [![Release](https://img.shields.io/github/v/release/DerOetzi/solaredge2mqtt)](https://github.com/DerOetzi/solaredge2mqtt/releases/latest) [![Build Status](https://img.shields.io/github/actions/workflow/status/DerOetzi/solaredge2mqtt/build_project.yml?branch=main)](https://github.com/DerOetzi/solaredge2mqtt/actions/workflows/build_project.yml) [![PyPI version](https://img.shields.io/pypi/v/solaredge2mqtt.svg)](https://pypi.org/project/solaredge2mqtt/) [![Discord Chat](https://img.shields.io/discord/1196540254686032014)](https://discord.gg/QXfghc93pY)
 
 The SolarEdge2MQTT service facilitates the retrieval of power data from SolarEdge inverters and its publication to an MQTT broker. Ideal for integrating SolarEdge inverters into home automation systems, this service supports real-time monitoring of power flow and additional parameters via Modbus.
 
 Users can optionally collect panel energy production data directly from the SolarEdge monitoring site, without employing the API, by leveraging their monitoring platform account.
 
 It also enables the monitoring of SolarEdge Wallbox via the REST API and supports saving all values into InfluxDB for advanced visualization.
 
-*Please note: The SolarEdge2MQTT service is in its early development stages. Although operational for reading and publishing data from a SolarEdge inverter, active development may introduce changes to features, potential removals, or bugs. Users are advised to proceed with caution. As an open-source project, contributions are highly encouraged.*
+_Please note: The SolarEdge2MQTT service is in its early development stages. Although operational for reading and publishing data from a SolarEdge inverter, active development may introduce changes to features, potential removals, or bugs. Users are advised to proceed with caution. As an open-source project, contributions are highly encouraged._
 
 ## Contact and Feedback
 
 For inquiries, feel free to reach out on Discord.
 
 [![Discord Banner](https://discordapp.com/api/guilds/1196540254686032014/widget.png?style=banner2)](https://discord.gg/QXfghc93pY)
 
@@ -59,87 +60,92 @@
 
 Configure the service using environment variables. The available options are listed below for customization:
 
 ### Basic configuration
 
 - **SE2MQTT_INTERVAL**: The frequency (in seconds) of data retrieval requests. Default is every 5 seconds.
 - **SE2MQTT_LOGGING_LEVEL**: Adjust the verbosity of logs. Options include DEBUG, INFO, WARNING, ERROR, and CRITICAL.
-- **SE2MQTT_LOCATION__LATITUDE** and **SE2MQTT_LOCATION__LONGITUDE**: Specify your location to enable weather and forecast services. These settings are essential for accurate environmental data and PV production forecasts.
+- **SE2MQTT_LOCATION\_\_LATITUDE** and **SE2MQTT_LOCATION\_\_LONGITUDE**: Specify your location to enable weather and forecast services. These settings are essential for accurate environmental data and PV production forecasts.
 
 ### Modbus configuration
 
-- **SE2MQTT_MODBUS__HOST**: The IP address of your SolarEdge inverter.
-- **SE2MQTT_MODBUS__PORT**: The port on which your inverter's Modbus is accessible. Default is 1502.
-- **SE2MQTT_MODBUS__TIMEOUT**: The timeout (in seconds) for Modbus connections. A lower value makes the system more responsive but may lead to incomplete data in environments with poor network conditions.
-- **SE2MQTT_MODBUS__UNIT**: The unit address for Modbus communication. Default is 1.
+- **SE2MQTT_MODBUS\_\_HOST**: The IP address of your SolarEdge inverter.
+- **SE2MQTT_MODBUS\_\_PORT**: The port on which your inverter's Modbus is accessible. Default is 1502.
+- **SE2MQTT_MODBUS\_\_TIMEOUT**: The timeout (in seconds) for Modbus connections. A lower value makes the system more responsive but may lead to incomplete data in environments with poor network conditions.
+- **SE2MQTT_MODBUS\_\_UNIT**: The unit address for Modbus communication. Default is 1.
 
 ### MQTT configuration
 
-- **SE2MQTT_MQTT__CLIENT_ID**: Identifier for the MQTT client, defaults to 'solaredge2mqtt'.
-- **SE2MQTT_MQTT__BROKER**: The IP address of your MQTT broker.
-- **SE2MQTT_MQTT__PORT**: The port your MQTT broker listens on. Default is 1883.
-- **SE2MQTT_MQTT__USERNAME** and **SE2MQTT_MQTT__PASSWORD**: Credentials for connecting to your MQTT broker. It's recommended to use secrets for the password if deploying with Docker.
-- **SE2MQTT_MQTT__TOPIC_PREFIX**: The prefix used for MQTT topics. Defaults to 'solaredge'.
+- **SE2MQTT_MQTT\_\_CLIENT_ID**: Identifier for the MQTT client, defaults to 'solaredge2mqtt'.
+- **SE2MQTT_MQTT\_\_BROKER**: The IP address of your MQTT broker.
+- **SE2MQTT_MQTT\_\_PORT**: The port your MQTT broker listens on. Default is 1883.
+- **SE2MQTT_MQTT\_\_USERNAME** and **SE2MQTT_MQTT\_\_PASSWORD**: Credentials for connecting to your MQTT broker. It's recommended to use secrets for the password if deploying with Docker.
+- **SE2MQTT_MQTT\_\_TOPIC_PREFIX**: The prefix used for MQTT topics. Defaults to 'solaredge'.
 
 ### Monitoring
 
 To enable panel energy value retrieval from the SolarEdge monitoring platform, you must configure:
 
-- **SE2MQTT_MONITORING__SITE_ID**: Your site ID as registered on the SolarEdge platform.
-- **SE2MQTT_MONITORING__USERNAME**: Your username for the SolarEdge monitoring platform.
-- **SE2MQTT_MONITORING__PASSWORD**: Your password. Ensure to use Docker secrets or a secure method to protect this information.
+- **SE2MQTT_MONITORING\_\_SITE_ID**: Your site ID as registered on the SolarEdge platform.
+- **SE2MQTT_MONITORING\_\_USERNAME**: Your username for the SolarEdge monitoring platform.
+- **SE2MQTT_MONITORING\_\_PASSWORD**: Your password. Ensure to use Docker secrets or a secure method to protect this information.
 
 ### Wallbox
 
 For monitoring SolarEdge Wallbox, provide:
 
-- **SE2MQTT_WALLBOX__HOST**: The IP address of your Wallbox.
-- **SE2MQTT_WALLBOX__PASSWORD**: The admin password for Wallbox web UI access.
-- **SE2MQTT_WALLBOX__SERIAL**: The serial number of your Wallbox.
+- **SE2MQTT_WALLBOX\_\_HOST**: The IP address of your Wallbox.
+- **SE2MQTT_WALLBOX\_\_PASSWORD**: The admin password for Wallbox web UI access.
+- **SE2MQTT_WALLBOX\_\_SERIAL**: The serial number of your Wallbox.
 
 ### InfluxDB
 
 Configure your InfluxDB settings with these environment variables to store monitoring data effectively:
 
-- **SE2MQTT_INFLUXDB__HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
-- **SE2MQTT_INFLUXDB__PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
-- **SE2MQTT_INFLUXDB__TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
-- **SE2MQTT_INFLUXDB__ORG**: The ID of your organization within InfluxDB. Default is None.
-- **SE2MQTT_INFLUXDB__BUCKET**: The name of the bucket where the data will be saved. Default bucket name is solaredge.
-- **SE2MQTT_INFLUXDB__RETENTION_RAW**: The retention policy for raw data in hours. This setting defines how long the raw power values are stored in InfluxDB. Default is 25 hours.
-- **SE2MQTT_INFLUXDB__RETENTION**: The retention policy for aggregated data in seconds. This sets how long the aggregated data will be stored in InfluxDB, with the default being 2 years (63072000 seconds).
-These configurations allow you to tailor the InfluxDB storage for your SolarEdge monitoring data, ensuring that you have the flexibility to define how long the data should be retained both in raw and aggregated forms.
+- **SE2MQTT_INFLUXDB\_\_HOST**: Specify the host of your InfluxDB instance (e.g., http://localhost). Default is None.
+- **SE2MQTT_INFLUXDB\_\_PORT**: The port number on which your InfluxDB instance is running. The default value is 8086.
+- **SE2MQTT_INFLUXDB\_\_TOKEN**: Your access token for InfluxDB. It is imperative to use this token securely, especially when deploying with Docker. The token requires full access since the service will be managing necessary buckets and tasks. Default is None.
+- **SE2MQTT_INFLUXDB\_\_ORG**: The ID of your organization within InfluxDB. Default is None.
+- **SE2MQTT_INFLUXDB\_\_BUCKET**: The name of the bucket where the data will be saved. Default bucket name is solaredge.
+- **SE2MQTT_INFLUXDB\_\_RETENTION_RAW**: The retention policy for raw data in hours. This setting defines how long the raw power values are stored in InfluxDB. Default is 25 hours.
+- **SE2MQTT_INFLUXDB\_\_RETENTION**: The retention policy for aggregated data in seconds. This sets how long the aggregated data will be stored in InfluxDB, with the default being 2 years (63072000 seconds).
+  These configurations allow you to tailor the InfluxDB storage for your SolarEdge monitoring data, ensuring that you have the flexibility to define how long the data should be retained both in raw and aggregated forms.
 
 ### Price Configuration
+
 To calculate your savings and earnings, you can specify the amount you pay for consumption and the amount you receive for delivery per kilowatt-hour (kWh). Please note, this feature is only operational in conjunction with InfluxDB.
 
-- **SE2MQTT_PRICES__CONSUMPTION**: Set the price you pay per 1 kWh for energy received from the grid.
-- **SE2MQTT_PRICES__DELIVERY**: Set the price you receive per 1 kWh for energy delivered to the grid.
+- **SE2MQTT_PRICES\_\_CONSUMPTION**: Set the price you pay per 1 kWh for energy received from the grid.
+- **SE2MQTT_PRICES\_\_DELIVERY**: Set the price you receive per 1 kWh for energy delivered to the grid.
 
 These additional settings allow for a comprehensive analysis of your energy production and usage, enabling you not just to monitor energy flow but also understand the financial aspects of your energy generation and consumption.
 
 ### Weather
 
 Leverage real-time weather data in your SolarEdge2MQTT service by integrating with OpenWeatherMap. This feature enriches your service with accurate environmental conditions, which can be essential for detailed energy production analysis.
 
-- **SE2MQTT_WEATHER__API_KEY**: Securely set your OpenWeatherMap OneCall API key here. For enhanced security, it's recommended to use this key as a secret within Docker environments.
-- **SE2MQTT_WEATHER__LANGUAGE**: Customize the language for weather data retrieved from the API. The default setting is English (en).
+- **SE2MQTT_WEATHER\_\_API_KEY**: Securely set your OpenWeatherMap OneCall API key here. For enhanced security, it's recommended to use this key as a secret within Docker environments.
+- **SE2MQTT_WEATHER\_\_LANGUAGE**: Customize the language for weather data retrieved from the API. The default setting is English (en).
 
-To access current weather data, ensure you have an OpenWeatherMap account, an API key, and a subscription to the One-Call API. Visit [OpenWeatherMap](https://openweathermap.org/) for more information on obtaining these prerequisites.
+To access current weather data, ensure you have an OpenWeatherMap account, an API key, and a [subscription](https://home.openweathermap.org/subscriptions) to the One-Call API. Visit [OpenWeatherMap](https://openweathermap.org/) for more information on obtaining these prerequisites.
 
 ### Forecast
 
 The SolarEdge2MQTT service features an integrated machine learning component designed to forecast PV production for the current and following day. For optimal functionality, confirm that your settings for [location](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#basic-configuration), [InfluxDB](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#influxdb) and [weather](https://github.com/DerOetzi/solaredge2mqtt/blob/main/README.md#weather) are correctly configured.
 
-- **SE2MQTT_FORECAST__ENABLE**: Activate the machine learning-based forecast feature by setting this to true. The default is false.
-- **SE2MQTT_FORECAST__HYPERPARAMETERTUNING**: Optimize forecast accuracy by enabling hyperparameter tuning. Note that this process is computationally intensive and may not be suitable for devices with limited processing power, such as Raspberry Pi. The default setting is false.
+- **SE2MQTT_FORECAST\_\_ENABLE**: Activate the machine learning-based forecast feature by setting this to true. The default is false.
+- **SE2MQTT_FORECAST\_\_HYPERPARAMETERTUNING**: Optimize forecast accuracy by enabling hyperparameter tuning. Note that this process is computationally intensive and may not be suitable for devices with limited processing power, such as Raspberry Pi. The default setting is false.
+
+**Precondition for Forecasting**: Before a forecast can be made, a minimum of 60 hours of training data must be collected. These data serve as the basis for model training and are crucial for prediction accuracy. Ensure that the service has had sufficient time to collect data before expecting forecast activation.
+
+**Note on Training Data Collection**: If the service goes without recording production data for longer than an hour, it will be unable to save training data. It's essential to ensure consistent data recording to maintain the integrity of the training process and ensure accurate forecasting.
 
-*Your experience and feedback, especially regarding forecast accuracy and performance on low-powered devices, are highly valued. This continuous improvement effort aims to enhance the predictive capabilities of the SolarEdge2MQTT service for all users.*
+_Your experience and feedback, especially regarding forecast accuracy and performance on low-powered devices, are highly valued. This continuous improvement effort aims to enhance the predictive capabilities of the SolarEdge2MQTT service for all users._
 
-## Running the service 
+## Running the service
 
 Each of these methods provides a different level of control and isolation, catering to various use cases from development and testing to full-scale production deployment.
 
 ### In the Console
 
 For users looking to run SolarEdge2MQTT directly within their console, which is ideal for testing or development environments, follow these steps:
```

### Comparing `solaredge2mqtt-1.0.8/solaredge2mqtt.egg-info/SOURCES.txt` & `solaredge2mqtt-1.0.9/solaredge2mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solaredge2mqtt-1.0.8/versioneer.py` & `solaredge2mqtt-1.0.9/versioneer.py`

 * *Files identical despite different names*

