# Comparing `tmp/elgas-24.1.0b1.tar.gz` & `tmp/elgas-24.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elgas-24.1.0b1.tar", last modified: Sun Feb 25 14:11:53 2024, max compression
+gzip compressed data, was "elgas-24.1.0b2.tar", last modified: Sun Apr 14 11:41:27 2024, max compression
```

## Comparing `elgas-24.1.0b1.tar` & `elgas-24.1.0b2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-02-25 14:11:53.881974 elgas-24.1.0b1/
--rw-r--r--   0 henrik     (501) staff       (20)     5243 2024-02-25 12:45:21.000000 elgas-24.1.0b1/LICENSE
--rw-r--r--   0 henrik     (501) staff       (20)     2608 2024-02-25 14:11:53.881805 elgas-24.1.0b1/PKG-INFO
--rw-r--r--   0 henrik     (501) staff       (20)      685 2024-02-16 14:03:48.000000 elgas-24.1.0b1/README.md
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-02-25 14:11:53.875367 elgas-24.1.0b1/elgas/
--rw-r--r--   0 henrik     (501) staff       (20)        0 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/__init__.py
--rw-r--r--   0 henrik     (501) staff       (20)    11929 2024-02-25 12:45:21.000000 elgas-24.1.0b1/elgas/application.py
--rw-r--r--   0 henrik     (501) staff       (20)     4809 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/client.py
--rw-r--r--   0 henrik     (501) staff       (20)     6889 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/connection.py
--rw-r--r--   0 henrik     (501) staff       (20)      749 2024-02-25 12:45:21.000000 elgas-24.1.0b1/elgas/constants.py
--rw-r--r--   0 henrik     (501) staff       (20)      878 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/exceptions.py
--rw-r--r--   0 henrik     (501) staff       (20)     7133 2024-02-25 12:45:21.000000 elgas-24.1.0b1/elgas/frames.py
--rw-r--r--   0 henrik     (501) staff       (20)     1023 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/integration.py
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-02-25 14:11:53.880122 elgas-24.1.0b1/elgas/parameters/
--rw-r--r--   0 henrik     (501) staff       (20)        0 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/__init__.py
--rw-r--r--   0 henrik     (501) staff       (20)     6219 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/analog_quantity.py
--rw-r--r--   0 henrik     (501) staff       (20)     4376 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/binary.py
--rw-r--r--   0 henrik     (501) staff       (20)     4341 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/compressibility.py
--rw-r--r--   0 henrik     (501) staff       (20)     5043 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/conversion_coefficient.py
--rw-r--r--   0 henrik     (501) staff       (20)     6144 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     3718 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/device_error.py
--rw-r--r--   0 henrik     (501) staff       (20)     4778 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/diagnostics.py
--rw-r--r--   0 henrik     (501) staff       (20)     4782 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/difference_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     4896 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/energy.py
--rw-r--r--   0 henrik     (501) staff       (20)     1391 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/enumerations.py
--rw-r--r--   0 henrik     (501) staff       (20)     5100 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/error_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     4177 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/error_standard_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     7558 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/factory.py
--rw-r--r--   0 henrik     (501) staff       (20)     8143 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/flow_rate.py
--rw-r--r--   0 henrik     (501) staff       (20)     3792 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/gas_composition.py
--rw-r--r--   0 henrik     (501) staff       (20)     5027 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/modem.py
--rw-r--r--   0 henrik     (501) staff       (20)     3949 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/setpoint.py
--rw-r--r--   0 henrik     (501) staff       (20)     4495 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/standard_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     9441 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/statistics.py
--rw-r--r--   0 henrik     (501) staff       (20)     3716 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/sum_of_alarms.py
--rw-r--r--   0 henrik     (501) staff       (20)    15165 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/system_parameters.py
--rw-r--r--   0 henrik     (501) staff       (20)     9128 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/tariff_counter.py
--rw-r--r--   0 henrik     (501) staff       (20)     3630 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/time_window.py
--rw-r--r--   0 henrik     (501) staff       (20)     3159 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parameters/timer.py
--rw-r--r--   0 henrik     (501) staff       (20)     1144 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/parser.py
--rw-r--r--   0 henrik     (501) staff       (20)     3375 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/security.py
--rw-r--r--   0 henrik     (501) staff       (20)     3003 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/state.py
--rw-r--r--   0 henrik     (501) staff       (20)     8412 2024-02-16 14:03:48.000000 elgas-24.1.0b1/elgas/transport.py
--rw-r--r--   0 henrik     (501) staff       (20)     7307 2024-02-25 10:06:46.000000 elgas-24.1.0b1/elgas/utils.py
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-02-25 14:11:53.876300 elgas-24.1.0b1/elgas.egg-info/
--rw-r--r--   0 henrik     (501) staff       (20)     2608 2024-02-25 14:11:53.000000 elgas-24.1.0b1/elgas.egg-info/PKG-INFO
--rw-r--r--   0 henrik     (501) staff       (20)     1457 2024-02-25 14:11:53.000000 elgas-24.1.0b1/elgas.egg-info/SOURCES.txt
--rw-r--r--   0 henrik     (501) staff       (20)        1 2024-02-25 14:11:53.000000 elgas-24.1.0b1/elgas.egg-info/dependency_links.txt
--rw-r--r--   0 henrik     (501) staff       (20)        1 2024-02-16 14:09:11.000000 elgas-24.1.0b1/elgas.egg-info/not-zip-safe
--rw-r--r--   0 henrik     (501) staff       (20)      127 2024-02-25 14:11:53.000000 elgas-24.1.0b1/elgas.egg-info/requires.txt
--rw-r--r--   0 henrik     (501) staff       (20)        6 2024-02-25 14:11:53.000000 elgas-24.1.0b1/elgas.egg-info/top_level.txt
--rw-r--r--   0 henrik     (501) staff       (20)      324 2024-02-16 14:03:48.000000 elgas-24.1.0b1/pyproject.toml
--rw-r--r--   0 henrik     (501) staff       (20)       38 2024-02-25 14:11:53.882016 elgas-24.1.0b1/setup.cfg
--rw-r--r--   0 henrik     (501) staff       (20)     3324 2024-02-25 12:48:24.000000 elgas-24.1.0b1/setup.py
-drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-02-25 14:11:53.881582 elgas-24.1.0b1/tests/
--rw-r--r--   0 henrik     (501) staff       (20)     9040 2024-02-16 14:03:48.000000 elgas-24.1.0b1/tests/test_application.py
--rw-r--r--   0 henrik     (501) staff       (20)     5428 2024-02-25 12:45:21.000000 elgas-24.1.0b1/tests/test_call_to_dispatch.py
--rw-r--r--   0 henrik     (501) staff       (20)     2849 2024-02-16 14:03:48.000000 elgas-24.1.0b1/tests/test_frames.py
--rw-r--r--   0 henrik     (501) staff       (20)    12259 2024-02-16 14:03:48.000000 elgas-24.1.0b1/tests/test_parameters.py
--rw-r--r--   0 henrik     (501) staff       (20)    13302 2024-02-16 14:03:48.000000 elgas-24.1.0b1/tests/test_parser.py
--rw-r--r--   0 henrik     (501) staff       (20)    24777 2024-02-16 14:03:48.000000 elgas-24.1.0b1/tests/test_schema.py
--rw-r--r--   0 henrik     (501) staff       (20)     3659 2024-02-25 12:49:03.000000 elgas-24.1.0b1/tests/test_security.py
--rw-r--r--   0 henrik     (501) staff       (20)     4436 2024-02-16 14:03:48.000000 elgas-24.1.0b1/tests/test_utils.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.124174 elgas-24.1.0b2/
+-rw-r--r--   0 henrik     (501) staff       (20)     5243 2024-02-25 12:45:21.000000 elgas-24.1.0b2/LICENSE
+-rw-r--r--   0 henrik     (501) staff       (20)     2691 2024-04-14 11:41:27.124035 elgas-24.1.0b2/PKG-INFO
+-rw-r--r--   0 henrik     (501) staff       (20)      685 2024-02-16 14:03:48.000000 elgas-24.1.0b2/README.md
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.118196 elgas-24.1.0b2/elgas/
+-rw-r--r--   0 henrik     (501) staff       (20)        0 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/__init__.py
+-rw-r--r--   0 henrik     (501) staff       (20)    12129 2024-04-14 11:33:30.000000 elgas-24.1.0b2/elgas/application.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4809 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/client.py
+-rw-r--r--   0 henrik     (501) staff       (20)     6889 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/connection.py
+-rw-r--r--   0 henrik     (501) staff       (20)      749 2024-02-25 12:45:21.000000 elgas-24.1.0b2/elgas/constants.py
+-rw-r--r--   0 henrik     (501) staff       (20)      878 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/exceptions.py
+-rw-r--r--   0 henrik     (501) staff       (20)     7133 2024-02-25 12:45:21.000000 elgas-24.1.0b2/elgas/frames.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1023 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/integration.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.122397 elgas-24.1.0b2/elgas/parameters/
+-rw-r--r--   0 henrik     (501) staff       (20)        0 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/__init__.py
+-rw-r--r--   0 henrik     (501) staff       (20)     6219 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/analog_quantity.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4376 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/binary.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4341 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/compressibility.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5043 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/conversion_coefficient.py
+-rw-r--r--   0 henrik     (501) staff       (20)     6144 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3718 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/device_error.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4778 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/diagnostics.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4782 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/difference_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4896 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/energy.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1391 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/enumerations.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5100 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/error_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4177 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/error_standard_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     7558 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/factory.py
+-rw-r--r--   0 henrik     (501) staff       (20)     8143 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/flow_rate.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3792 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/gas_composition.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5027 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/modem.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3949 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/setpoint.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4495 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/standard_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     9441 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/statistics.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3716 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/sum_of_alarms.py
+-rw-r--r--   0 henrik     (501) staff       (20)    15165 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/system_parameters.py
+-rw-r--r--   0 henrik     (501) staff       (20)     9128 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/tariff_counter.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3630 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/time_window.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3159 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parameters/timer.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1144 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/parser.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3375 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/security.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3003 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/state.py
+-rw-r--r--   0 henrik     (501) staff       (20)     8412 2024-02-16 14:03:48.000000 elgas-24.1.0b2/elgas/transport.py
+-rw-r--r--   0 henrik     (501) staff       (20)     7307 2024-02-25 10:06:46.000000 elgas-24.1.0b2/elgas/utils.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.119044 elgas-24.1.0b2/elgas.egg-info/
+-rw-r--r--   0 henrik     (501) staff       (20)     2691 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/PKG-INFO
+-rw-r--r--   0 henrik     (501) staff       (20)     1457 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/SOURCES.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/dependency_links.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2024-02-16 14:09:11.000000 elgas-24.1.0b2/elgas.egg-info/not-zip-safe
+-rw-r--r--   0 henrik     (501) staff       (20)      127 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/requires.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        6 2024-04-14 11:41:27.000000 elgas-24.1.0b2/elgas.egg-info/top_level.txt
+-rw-r--r--   0 henrik     (501) staff       (20)      324 2024-02-16 14:03:48.000000 elgas-24.1.0b2/pyproject.toml
+-rw-r--r--   0 henrik     (501) staff       (20)       38 2024-04-14 11:41:27.124217 elgas-24.1.0b2/setup.cfg
+-rw-r--r--   0 henrik     (501) staff       (20)     3324 2024-04-14 11:40:40.000000 elgas-24.1.0b2/setup.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-14 11:41:27.123803 elgas-24.1.0b2/tests/
+-rw-r--r--   0 henrik     (501) staff       (20)     9252 2024-04-14 11:38:33.000000 elgas-24.1.0b2/tests/test_application.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5428 2024-02-25 12:45:21.000000 elgas-24.1.0b2/tests/test_call_to_dispatch.py
+-rw-r--r--   0 henrik     (501) staff       (20)     2849 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_frames.py
+-rw-r--r--   0 henrik     (501) staff       (20)    12259 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_parameters.py
+-rw-r--r--   0 henrik     (501) staff       (20)    13302 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_parser.py
+-rw-r--r--   0 henrik     (501) staff       (20)    24777 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_schema.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3659 2024-02-25 12:49:03.000000 elgas-24.1.0b2/tests/test_security.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4436 2024-02-16 14:03:48.000000 elgas-24.1.0b2/tests/test_utils.py
```

### Comparing `elgas-24.1.0b1/LICENSE` & `elgas-24.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/PKG-INFO` & `elgas-24.1.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgas
-Version: 24.1.0b1
+Version: 24.1.0b2
 Summary: A Python library for the ELGAS protocol
 Home-page: https://github.com/u9n/elgas
 Author: Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB
 Author-email: henrik.wahlgren@utilitarian.io
 Maintainer: Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB
 Maintainer-email: henrik.wahlgren@utilitarian.io
 Project-URL: Bug Tracker, https://github.com/u9n/elgas/issues
@@ -65,14 +65,20 @@
 
 ### Removed
 
 ### Fixed
 
 ### Security
 
+## [24.1.0] - 2024-04-14
+
+### Added
+
+Cryout bit in Service x71 (WriteTimeRequest)
+
 ## [22.2.1] - 2022-05-04
 
 ### Fixed
 
 * correct padding of password
 
 ## [22.2.0] - 2022-05-03
```

### Comparing `elgas-24.1.0b1/README.md` & `elgas-24.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/application.py` & `elgas-24.1.0b2/elgas/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,20 +133,24 @@
 
     service: ClassVar[
         constants.ServiceNumber
     ] = constants.ServiceNumber.WRITE_DEVICE_TIME
 
     password: str
     device_time: datetime
+    cryout: bool = attr.ib(default=False)
 
     def to_bytes(self) -> bytes:
         out = bytearray()
         out.extend(utils.pad_password(self.password).encode("latin-1"))
         out.extend(utils.datetime_to_bytes(self.device_time))
-        out.append(0b00000100)  # Flag to only sync time.
+        flags = 0b00000100  # Flag set to only sync time.
+        #if self.cryout:
+        #    flags = flags | 0b00000001  # Set the cryout bit
+        out.append(flags & 0xff)  # force to one byte just to be safe.
 
         return bytes(out)
 
 
 @attr.s(auto_attribs=True)
 class WriteTimeResponse:
     """
```

### Comparing `elgas-24.1.0b1/elgas/client.py` & `elgas-24.1.0b2/elgas/client.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/connection.py` & `elgas-24.1.0b2/elgas/connection.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/constants.py` & `elgas-24.1.0b2/elgas/constants.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/exceptions.py` & `elgas-24.1.0b2/elgas/exceptions.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/frames.py` & `elgas-24.1.0b2/elgas/frames.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/integration.py` & `elgas-24.1.0b2/elgas/integration.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/analog_quantity.py` & `elgas-24.1.0b2/elgas/parameters/analog_quantity.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/binary.py` & `elgas-24.1.0b2/elgas/parameters/binary.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/compressibility.py` & `elgas-24.1.0b2/elgas/parameters/compressibility.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/conversion_coefficient.py` & `elgas-24.1.0b2/elgas/parameters/conversion_coefficient.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/counter.py` & `elgas-24.1.0b2/elgas/parameters/counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/device_error.py` & `elgas-24.1.0b2/elgas/parameters/device_error.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/diagnostics.py` & `elgas-24.1.0b2/elgas/parameters/diagnostics.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/difference_counter.py` & `elgas-24.1.0b2/elgas/parameters/difference_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/energy.py` & `elgas-24.1.0b2/elgas/parameters/energy.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/enumerations.py` & `elgas-24.1.0b2/elgas/parameters/enumerations.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/error_counter.py` & `elgas-24.1.0b2/elgas/parameters/error_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/error_standard_counter.py` & `elgas-24.1.0b2/elgas/parameters/error_standard_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/factory.py` & `elgas-24.1.0b2/elgas/parameters/factory.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/flow_rate.py` & `elgas-24.1.0b2/elgas/parameters/flow_rate.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/gas_composition.py` & `elgas-24.1.0b2/elgas/parameters/gas_composition.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/modem.py` & `elgas-24.1.0b2/elgas/parameters/modem.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/setpoint.py` & `elgas-24.1.0b2/elgas/parameters/setpoint.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/standard_counter.py` & `elgas-24.1.0b2/elgas/parameters/standard_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/statistics.py` & `elgas-24.1.0b2/elgas/parameters/statistics.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/sum_of_alarms.py` & `elgas-24.1.0b2/elgas/parameters/sum_of_alarms.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/system_parameters.py` & `elgas-24.1.0b2/elgas/parameters/system_parameters.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/tariff_counter.py` & `elgas-24.1.0b2/elgas/parameters/tariff_counter.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/time_window.py` & `elgas-24.1.0b2/elgas/parameters/time_window.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parameters/timer.py` & `elgas-24.1.0b2/elgas/parameters/timer.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/parser.py` & `elgas-24.1.0b2/elgas/parser.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/security.py` & `elgas-24.1.0b2/elgas/security.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/state.py` & `elgas-24.1.0b2/elgas/state.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/transport.py` & `elgas-24.1.0b2/elgas/transport.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas/utils.py` & `elgas-24.1.0b2/elgas/utils.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/elgas.egg-info/PKG-INFO` & `elgas-24.1.0b2/elgas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgas
-Version: 24.1.0b1
+Version: 24.1.0b2
 Summary: A Python library for the ELGAS protocol
 Home-page: https://github.com/u9n/elgas
 Author: Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB
 Author-email: henrik.wahlgren@utilitarian.io
 Maintainer: Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB
 Maintainer-email: henrik.wahlgren@utilitarian.io
 Project-URL: Bug Tracker, https://github.com/u9n/elgas/issues
@@ -65,14 +65,20 @@
 
 ### Removed
 
 ### Fixed
 
 ### Security
 
+## [24.1.0] - 2024-04-14
+
+### Added
+
+Cryout bit in Service x71 (WriteTimeRequest)
+
 ## [22.2.1] - 2022-05-04
 
 ### Fixed
 
 * correct padding of password
 
 ## [22.2.0] - 2022-05-03
```

### Comparing `elgas-24.1.0b1/elgas.egg-info/SOURCES.txt` & `elgas-24.1.0b2/elgas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/setup.py` & `elgas-24.1.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 PROJECT_URLS = {
     "Bug Tracker": "https://github.com/u9n/elgas/issues",
     "Source Code": "https://github.com/u9n/elgas",
 }
 EMAIL = "henrik.wahlgren@utilitarian.io"
 AUTHOR = "Henrik Palmlund Wahlgren @ Palmlund Wahlgren Innovative Technology AB"
 REQUIRES_PYTHON = "~=3.7"
-VERSION = "24.1.0b1"
+VERSION = "24.1.0b2"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "attrs>=21.4.0",
     "cryptography==42.0.5",
     "marshmallow>=3.14.1",
     "structlog>=21.5.0",
```

### Comparing `elgas-24.1.0b1/tests/test_application.py` & `elgas-24.1.0b2/tests/test_application.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,21 +78,24 @@
 
     pdu = application.ReadArchiveByTimeResponse.from_bytes(response.data)
     print(pdu)
     assert response
 
 
 def test_write_time():
-    time = datetime.datetime.now()
+    time = datetime.datetime.fromisoformat("2024-04-14T13:34:36")
+    print(time)
     req = application.WriteTimeRequest(password="123456", device_time=time)
     print(req)
     print(req.to_bytes().hex())
     frame = frames.Request(
         service=req.service,
         destination_address_2=0,
         destination_address_1=0,
         source_address_2=0,
         source_address_1=0,
         data=req.to_bytes(),
     )
     print(frame)
     print(frame.to_bytes().hex())
+    # cant check as password is padded with random bytes.
+    #assert frame.to_bytes().hex() == "02fe84712000000000000000313233343536210359733634131404240405f5030d"
```

### Comparing `elgas-24.1.0b1/tests/test_call_to_dispatch.py` & `elgas-24.1.0b2/tests/test_call_to_dispatch.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/tests/test_frames.py` & `elgas-24.1.0b2/tests/test_frames.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/tests/test_parameters.py` & `elgas-24.1.0b2/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/tests/test_parser.py` & `elgas-24.1.0b2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/tests/test_schema.py` & `elgas-24.1.0b2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/tests/test_security.py` & `elgas-24.1.0b2/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `elgas-24.1.0b1/tests/test_utils.py` & `elgas-24.1.0b2/tests/test_utils.py`

 * *Files identical despite different names*

