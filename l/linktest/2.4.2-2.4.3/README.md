# Comparing `tmp/linktest-2.4.2.tar.gz` & `tmp/linktest-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.4.2.tar", last modified: Fri Apr 12 14:38:50 2024, max compression
+gzip compressed data, was "linktest-2.4.3.tar", last modified: Sun Apr 14 16:24:48 2024, max compression
```

## Comparing `linktest-2.4.2.tar` & `linktest-2.4.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-12 14:38:50.549996 linktest-2.4.2/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-12 14:38:50.549702 linktest-2.4.2/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-12 14:38:50.545276 linktest-2.4.2/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-12 14:34:03.000000 linktest-2.4.2/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-12 14:31:48.000000 linktest-2.4.2/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15915 2024-04-12 14:31:42.000000 linktest-2.4.2/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3825 2024-04-12 13:57:12.000000 linktest-2.4.2/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    37292 2024-04-12 14:18:40.000000 linktest-2.4.2/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10265 2024-04-09 02:55:29.000000 linktest-2.4.2/linktest/logged_requests copy.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   104608 2024-04-12 14:31:34.000000 linktest-2.4.2/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7937 2024-04-12 10:48:42.000000 linktest-2.4.2/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-12 14:34:03.000000 linktest-2.4.2/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-12 14:31:12.000000 linktest-2.4.2/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11563 2024-04-12 02:12:43.000000 linktest-2.4.2/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-11 08:19:05.000000 linktest-2.4.2/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-12 14:38:50.549418 linktest-2.4.2/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1304 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-12 14:38:50.000000 linktest-2.4.2/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-12 14:38:50.550092 linktest-2.4.2/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-12 14:38:44.000000 linktest-2.4.2/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-14 16:24:48.519912 linktest-2.4.3/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-14 16:24:48.519662 linktest-2.4.3/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-14 16:24:48.510177 linktest-2.4.3/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-14 16:23:39.000000 linktest-2.4.3/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15915 2024-04-12 11:05:25.000000 linktest-2.4.3/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4308 2024-04-14 16:16:30.000000 linktest-2.4.3/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    37292 2024-04-12 14:18:40.000000 linktest-2.4.3/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10265 2024-04-09 02:55:29.000000 linktest-2.4.3/linktest/logged_requests copy.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   104608 2024-04-12 14:06:49.000000 linktest-2.4.3/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7937 2024-04-12 10:48:42.000000 linktest-2.4.3/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-14 16:23:49.000000 linktest-2.4.3/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11013 2024-04-14 15:04:52.000000 linktest-2.4.3/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-14 16:24:48.519264 linktest-2.4.3/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1304 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-14 16:24:48.519958 linktest-2.4.3/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-14 16:24:42.000000 linktest-2.4.3/setup.py
```

### Comparing `linktest-2.4.2/linktest/appium_utils.py` & `linktest-2.4.3/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/auto_generate_testcase_list.py` & `linktest-2.4.3/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.4.3/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/base_testcase.py` & `linktest-2.4.3/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/clean_data.py` & `linktest-2.4.3/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/conver_xml_into_db.py` & `linktest-2.4.3/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/database_helper.py` & `linktest-2.4.3/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/date_utilities.py` & `linktest-2.4.3/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/doctor.py` & `linktest-2.4.3/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/framework_log.py` & `linktest-2.4.3/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/generate_html_log.py` & `linktest-2.4.3/linktest/generate_html_log.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 
 import re
-import html
 
 
 def starts_with_date(input_string):
     # 正则表达式匹配 YYYY-MM-DD 格式的日期
     pattern = r'^\d{4}-\d{2}-\d{2}'
 
     # 使用 re.match 检查字符串开头是否匹配该模式
@@ -69,34 +68,40 @@
     """ % executing_testcase.logger.name
 
     lines = ""
     single_line_flag = False
 
     # 将日志行转换为HTML元素
     for line in execution_log:
-        line = html.escape(line)
         class_name = "log-entry"
         if "ERROR" in line:
             class_name += " error"
         elif "INFO" in line:
             class_name += " info"
 
-        if line.__contains__("WebDriver Action:"):
-            line = line.replace("WebDriver Action:", "<span style='color:blue'>WebDriver Action:</span>")
+        if "WebDriver Action:" in line:
+            action_name = line.split("'")[1]
+            line = line.replace("WebDriver Action:", "<span style='color:#0066CC'>WebDriver Action:</span>")
+            line = line.replace(f"'{action_name}'", f"<b style='color:#006600'>'{action_name}'</b>")
+            if "args" in line:
+                line = line.replace("args", "<b style='color:#333333'>args</b>")
+
+        if "WebElement Action:" in line:
+            action_name = line.split("'")[1]
+            line = line.replace("WebElement Action:", "<span style='color:#0066CC'>WebElement Action:</span>")
+            line = line.replace(f"'{action_name}'", f"<b style='color:#006600'>'{action_name}'</b>")
+            if "args" in line:
+                line = line.replace("args", "<b style='color:#333333'>args</b>")
 
-        if line.__contains__("WebElement Action:"):
-            line = line.replace("WebElement Action:", "<span style='color:blue'>WebElement Action:</span>")
-
-        if line.__contains__("logged_requests.py"):
+        if "logged_requests.py" in line:
             line = line.replace("logged_requests.py", "<span style='color:green'>logged_requests.py</span>")
 
-        if line.__contains__("linktest_screenshot_filename:"):
-            line = line.replace("linktest_screenshot_filename:",
-                                "<img src='" + line.split("linktest_screenshot_filename:")[
-                                    1].strip() + "' width='100%'>")
+        if "WebDriver Action:</span> <b style='color:#006600'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:" in line:
+            line += "<img src='" + line.split("WebDriver Action:</span> <b style='color:#006600'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:")[1].strip() + "' width='100%'>"
+
 
         if line == "\n":
             continue
 
         if starts_with_date(line):
             if single_line_flag:
                 html_content += f'<div class="{class_name}"><p>{lines}</p></div>'
```

### Comparing `linktest-2.4.2/linktest/get_adb_devices.py` & `linktest-2.4.3/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/get_ios_devices_list.py` & `linktest-2.4.3/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/get_platform_info.py` & `linktest-2.4.3/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/get_project_info.py` & `linktest-2.4.3/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/html_report.py` & `linktest-2.4.3/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/logged_requests copy.py` & `linktest-2.4.3/linktest/logged_requests copy.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/logged_requests.py` & `linktest-2.4.3/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/main.py` & `linktest-2.4.3/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/memory_usage.py` & `linktest-2.4.3/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/re_func.py` & `linktest-2.4.3/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/run.py` & `linktest-2.4.3/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/run_testcase_thread.py` & `linktest-2.4.3/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/scp_report_to_specified_path.py` & `linktest-2.4.3/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/selenium_helper.py` & `linktest-2.4.3/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/timeout_thread.py` & `linktest-2.4.3/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/ui_testcase.py` & `linktest-2.4.3/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/update_config.py` & `linktest-2.4.3/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest/webdriver_wrapper.py` & `linktest-2.4.3/linktest/webdriver_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -63,39 +63,42 @@
 
 class WebElementWrapper:
     def __init__(self, element, logger):
         self.element = element
         self.logger = logger
 
     def _log_action(self, action, *args):
-        msg = f"- WebElement Action: '{action}' with args: {', '.join(map(str, args))}"
+        if args:
+            msg = f"- WebElement Action: '{action}' with args: {', '.join(map(str, args))}"
+        else:
+            msg = f"- WebElement Action: '{action}'"
         self.logger.info(msg)
 
     def send_keys(self, *value):
         self._log_action("send_keys", *value)
         self.element.send_keys(*value)
 
     def click(self):
-        self.logger.info(f"- WebElementWrapper Action: 'click'")
+        self._log_action("click")
         self.element.click()
 
     def clear(self):
-        self.logger.info(f"- WebElementWrapper Action: 'clear'")
+        self._log_action("clear")
         self.element.clear()
 
     def tag_name(self) -> str:
-        self.logger.info(f"- WebElementWrapper Action: 'tag_name'")
+        self._log_action("tag_name")
         return self.element.tag_name
 
     def submit(self):
-        self.logger.info(f"- WebElementWrapper Action: 'submit'")
+        self._log_action("submit")
         self.element.submit()
 
     def text(self) -> str:
-        self.logger.info(f"- WebElementWrapper Action: 'text'")
+        self._log_action("text")
         return self.element.text
 
     def get_property(self, name) -> Union[str, bool, WebElement, dict]:
         self._log_action("get_property", name)
         return self.element.get_property(name)
 
     def get_dom_attribute(self, name) -> str:
@@ -103,43 +106,43 @@
         return self.element.get_attribute(name)
 
     def get_attribute(self, name) -> Union[str, None]:
         self._log_action("get_attribute", name)
         return self.element.get_attribute(name)
 
     def is_selected(self) -> bool:
-        self.logger.info(f"- WebElementWrapper Action: 'is_selected'")
+        self._log_action("is_selected")
         return self.element.is_selected()
 
     def is_enabled(self) -> bool:
-        self.logger.info(f"- WebElementWrapper Action: 'is_enabled'")
+        self._log_action("is_enabled")
         return self.element.is_enabled()
 
     def is_displayed(self) -> bool:
-        self.logger.info(f"- WebElementWrapper Action: 'is_displayed'")
+        self._log_action("is_displayed")
         return self.element.is_displayed()
 
     def location_once_scrolled_into_view(self) -> dict:
         self._log_action("location_once_scrolled_into_view")
         return self.element.location_once_scrolled_into_view
 
     def size(self) -> dict:
-        self.logger.info(f"- WebElementWrapper Action: 'size'")
+        self._log_action("size")
         return self.element.size
 
     def value_of_css_property(self, property_name) -> str:
         self._log_action("value_of_css_property", property_name)
         return self.element.value_of_css_property(property_name)
 
     def location(self) -> dict:
-        self.logger.info(f"- WebElementWrapper Action: 'location'")
+        self._log_action("location")
         return self.element.location
 
     def rect(self) -> dict:
-        self.logger.info(f"- WebElementWrapper Action: 'rect'")
+        self._log_action("rect")
         return self.element.rect
 
     def screenshot_as_base64(self) -> str:
         self._log_action("screenshot_as_base64")
         return self.element.screenshot_as_base64
 
     def screenshot_as_png(self) -> bytes:
@@ -147,19 +150,19 @@
         return self.element.screenshot_as_png
 
     def screenshot(self, filename) -> bool:
         self._log_action("screenshot", filename)
         return self.element.screenshot(filename)
 
     def parent(self):
-        self.logger.info(f"- WebElementWrapper Action: 'parent'")
+        self._log_action("parent")
         return self.element.parent
 
     def id(self) -> str:
-        self.logger.info(f"- WebElementWrapper Action: 'id'")
+        self._log_action("id")
         return self.element.id
 
     def find_element(self, by=By.ID, value=None) -> WebElement:
         self._log_action("find_element", by, value)
         return self.element.find_element(by, value)
 
     def find_elements(self, by=By.ID, value=None) -> List[WebElement]:
@@ -176,15 +179,18 @@
 class WebDriverWrapper(Chrome):
     def __init__(self, ui_testcase, *args, **kwargs):
         self.logger = ui_testcase.logger
         self.ui_testcase = ui_testcase
         super().__init__(*args, **kwargs)
 
     def _log_action(self, action, *args):
-        msg = f"- WebDriver Action: '{action}' with args: {', '.join(map(str, args))}"
+        if args:
+            msg = f"- WebDriver Action: '{action}' with args: {', '.join(map(str, args))}"
+        else:
+            msg = f"- WebDriver Action: '{action}'"
         self.logger.info(msg)
 
     def get(self, url):
         self._log_action("get", url)
         super().get(url)
 
     def find_element(self, by=By.ID, value=None):
@@ -205,95 +211,95 @@
     #     return super().execute(driver_command, params)
 
     def execute_async_script(self, script: str, *args):
         self._log_action("execute_async_script", script, *args)
         return super().execute_async_script(script, *args)
 
     def title(self) -> str:
-        self.logger.info(f"- WebDriver Action: 'title'")
+        self._log_action("title")
         return super().title
 
     # def create_web_element(self, element_id: str) -> WebElement:
     #     self._log_action("create_web_element", element_id)
     #     return super().create_web_element(element_id)
 
     def start_session(self, capabilities: dict) -> None:
         self._log_action("start_session", capabilities)
         super().start_session(capabilities)
 
     def current_url(self) -> str:
-        self.logger.info(f"- WebDriver Action: 'current_url'")
+        self._log_action("current_url")
         return super().current_url
 
     def page_source(self) -> str:
-        self.logger.info(f"- WebDriver Action: 'page_source'")
+        self._log_action("page_source")
         return super().page_source
 
     def close(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'close'")
+        self._log_action("close")
         super().close()
 
     def quit(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'quit'")
+        self._log_action("quit")
         super().quit()
 
     def current_window_handle(self) -> str:
-        self.logger.info(f"- WebDriver Action: 'current_window_handle'")
+        self._log_action("current_window_handle")
         return super().current_window_handle
 
     def window_handles(self) -> List[str]:
         self._log_action("window_handles")
         return super().window_handles
 
     def maximize_window(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'maximize_window'")
+        self._log_action("maximize_window")
         super().maximize_window()
 
     def fullscreen_window(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'fullscreen_window'")
+        self._log_action("fullscreen_window")
         super().fullscreen_window()
 
     def minimize_window(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'minimize_window'")
+        self._log_action("minimize_window")
         super().minimize_window()
 
     def get_cookie(self, name) -> typing.Optional[typing.Dict]:
         self._log_action("get_cookie", name)
         return super().get_cookie(name)
 
     def refresh(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'refresh'")
+        self._log_action("refresh")
         super().refresh()
 
     def forward(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'forward'")
+        self._log_action("forward")
         super().forward()
 
     def back(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'back'")
+        self._log_action("back")
         super().back()
 
     def print_page(self, print_options: Optional[PrintOptions] = None) -> str:
         self._log_action("print_page", print_options)
         return super().print_page(print_options)
 
     def get_cookies(self) -> List[dict]:
-        self.logger.info(f"- WebDriver Action: 'get_cookies'")
+        self._log_action("get_cookies")
         return super().get_cookies()
 
     def add_cookie(self, cookie_dict) -> None:
         self._log_action("add_cookie", cookie_dict)
         super().add_cookie(cookie_dict)
 
     def delete_cookie(self, name) -> None:
         self._log_action("delete_cookie", name)
         super().delete_cookie(name)
 
     def delete_all_cookies(self) -> None:
-        self.logger.info(f"- WebDriver Action: 'delete_all_cookies'")
+        self._log_action("delete_all_cookies")
         super().delete_all_cookies()
 
     def implicitly_wait(self, time_to_wait: float) -> None:
         self._log_action("implicitly_wait", time_to_wait)
         super().implicitly_wait(time_to_wait)
 
     def set_script_timeout(self, time_to_wait: float) -> None:
@@ -308,12 +314,12 @@
         if filename is None:
             if not getattr(self.ui_testcase, 'linktest_screenshot_index', False):
                 setattr(self.ui_testcase, 'linktest_screenshot_index', 1)
             else:
                 self.ui_testcase.linktest_screenshot_index += 1
 
             filename = self.ui_testcase.full_tc_folder + os.sep + self.logger.name + "_" + str(self.ui_testcase.linktest_screenshot_index) + "_screenshot.png"
-            self.logger.info("linktest_screenshot_filename: " + filename)
-        # self._log_action("save_screenshot", filename)
+            # self.logger.info("linktest_screenshot_filename: " + filename)
+        self._log_action("save_screenshot", filename)
         return super().save_screenshot(filename)
 
     # todo 可以继续在此处添加其他 WebDriver 方法的日志记录功能
```

### Comparing `linktest-2.4.2/linktest/xml_report.py` & `linktest-2.4.3/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.2/linktest.egg-info/SOURCES.txt` & `linktest-2.4.3/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

