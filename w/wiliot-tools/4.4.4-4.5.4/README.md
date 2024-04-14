# Comparing `tmp/wiliot-tools-4.4.4.tar.gz` & `tmp/wiliot-tools-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-tools-4.4.4.tar", last modified: Mon Jan 29 12:01:09 2024, max compression
+gzip compressed data, was "wiliot-tools-4.5.4.tar", last modified: Sun Apr 14 08:15:22 2024, max compression
```

## Comparing `wiliot-tools-4.4.4.tar` & `wiliot-tools-4.5.4.tar`

### file list

```diff
@@ -1,63 +1,77 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.265474 wiliot-tools-4.4.4/
--rw-rw-rw-   0 root         (0) root         (0)      452 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3486 2024-01-29 12:01:09.265474 wiliot-tools-4.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2982 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7557 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      330 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-29 12:01:09.265474 wiliot-tools-4.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1899 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.261474 wiliot-tools-4.4.4/wiliot_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.261474 wiliot-tools-4.4.4/wiliot_tools/association_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/association_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4786 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/association_tool/association_configs.py
--rw-rw-rw-   0 root         (0) root         (0)    18617 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/association_tool/association_tool.py
--rw-rw-rw-   0 root         (0) root         (0)    17451 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/association_tool/send_association_to_cloud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.261474 wiliot-tools-4.4.4/wiliot_tools/association_tool/sensor_count/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/association_tool/sensor_count/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2367 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/association_tool/sensor_count/sensor_count.ino
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.261474 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/gw_configs.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/local_gateway_gui.bat
--rw-rw-rw-   0 root         (0) root         (0)    79928 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/local_gateway_gui.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.261474 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/.gwCommands.json
--rw-rw-rw-   0 root         (0) root         (0)     4010 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/advanced_gui.ui
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/configs.gif
--rw-rw-rw-   0 root         (0) root         (0)    17562 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/custom_ep.ui
--rw-rw-rw-   0 root         (0) root         (0)    10355 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/custom_plots.ui
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/debug_mode.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/folder.png
--rw-rw-rw-   0 root         (0) root         (0)    28925 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui
--rw-rw-rw-   0 root         (0) root         (0)     5671 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/gw_macros.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.265474 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/owner_change_app.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/owner_change_gui.bat
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/owner_change_gui.sh
--rw-rw-rw-   0 root         (0) root         (0)     5359 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/owner_change_requests_page.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/owner_change_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6807 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/requests_details_page.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.265474 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/resources/
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/resources/columns_width.json
--rw-rw-rw-   0 root         (0) root         (0)     4441 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/resources/wiliot-green
--rw-rw-rw-   0 root         (0) root         (0)    14210 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/resources/wiliot.png
--rw-rw-rw-   0 root         (0) root         (0)     7556 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/send_request_multiple_reels_page.py
--rw-rw-rw-   0 root         (0) root         (0)     5016 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/send_request_one_reel_page.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.265474 wiliot-tools-4.4.4/wiliot_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6186 2024-01-29 12:01:01.000000 wiliot-tools-4.4.4/wiliot_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-29 12:01:09.000000 wiliot-tools-4.4.4/wiliot_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-01-29 12:01:09.261474 wiliot-tools-4.4.4/wiliot_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3486 2024-01-29 12:01:09.000000 wiliot-tools-4.4.4/wiliot_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2137 2024-01-29 12:01:09.000000 wiliot-tools-4.4.4/wiliot_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-29 12:01:09.000000 wiliot-tools-4.4.4/wiliot_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-29 12:01:09.000000 wiliot-tools-4.4.4/wiliot_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-01-29 12:01:09.000000 wiliot-tools-4.4.4/wiliot_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-01-29 12:01:09.000000 wiliot-tools-4.4.4/wiliot_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.017706 wiliot-tools-4.5.4/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2024-04-14 08:15:22.017706 wiliot-tools-4.5.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3315 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7557 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-14 08:15:22.017706 wiliot-tools-4.5.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.009706 wiliot-tools-4.5.4/wiliot_tools/
+-rw-rw-rw-   0 root         (0) root         (0)     4158 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.009706 wiliot-tools-4.5.4/wiliot_tools/association_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/association_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4786 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/association_tool/association_configs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18670 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/association_tool/association_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)    18636 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/association_tool/send_association_to_cloud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.009706 wiliot-tools-4.5.4/wiliot_tools/association_tool/sensor_count/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/association_tool/sensor_count/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/association_tool/sensor_count/sensor_count.ino
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.009706 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/local_gateway_gui.bat
+-rw-rw-rw-   0 root         (0) root         (0)    81167 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/local_gateway_gui.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.009706 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/.gwCommands.json
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3469 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/advanced_gui.ui
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/configs.gif
+-rw-rw-rw-   0 root         (0) root         (0)    17562 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/custom_ep.ui
+-rw-rw-rw-   0 root         (0) root         (0)    10355 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/custom_plots.ui
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/debug_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/folder.png
+-rw-rw-rw-   0 root         (0) root         (0)    29616 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/gw_macros.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.013707 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/owner_change_app.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/owner_change_gui.bat
+-rw-rw-rw-   0 root         (0) root         (0)     6044 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/owner_change_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     7219 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/owner_change_requests_page.py
+-rw-rw-rw-   0 root         (0) root         (0)     2601 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/owner_change_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6777 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/requests_details_page.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.013707 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/resources/columns_width.json
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/resources/wiliot-green
+-rw-rw-rw-   0 root         (0) root         (0)    14210 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/resources/wiliot.png
+-rw-rw-rw-   0 root         (0) root         (0)     7533 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/send_request_multiple_reels_page.py
+-rw-rw-rw-   0 root         (0) root         (0)     5982 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/send_request_one_reel_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.013707 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/requests_details_page.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/requests_df.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.013707 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     1372 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/resources/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4441 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/resources/wiliot-green
+-rw-rw-rw-   0 root         (0) root         (0)    14210 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/resources/wiliot.png
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/send_request_multiple_reels_page.py
+-rw-rw-rw-   0 root         (0) root         (0)     2802 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/send_request_one_reel_page.py
+-rw-rw-rw-   0 root         (0) root         (0)     4586 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/shipment_approval_app.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/shipment_approval_gui.bat
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/shipment_approval_gui.sh
+-rw-rw-rw-   0 root         (0) root         (0)     6361 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/shipment_approval_requests_page.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/shipment_approval_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.013707 wiliot-tools-4.5.4/wiliot_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6186 2024-04-14 08:15:08.000000 wiliot-tools-4.5.4/wiliot_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-14 08:15:21.000000 wiliot-tools-4.5.4/wiliot_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 08:15:22.009706 wiliot-tools-4.5.4/wiliot_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2024-04-14 08:15:21.000000 wiliot-tools-4.5.4/wiliot_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-14 08:15:21.000000 wiliot-tools-4.5.4/wiliot_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-14 08:15:21.000000 wiliot-tools-4.5.4/wiliot_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-14 08:15:21.000000 wiliot-tools-4.5.4/wiliot_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-14 08:15:21.000000 wiliot-tools-4.5.4/wiliot_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-14 08:15:21.000000 wiliot-tools-4.5.4/wiliot_tools.egg-info/top_level.txt
```

### Comparing `wiliot-tools-4.4.4/LICENSE` & `wiliot-tools-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/PKG-INFO` & `wiliot-tools-4.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-tools
-Version: 4.4.4
+Version: 4.5.4
 Summary: A library for interacting with Wiliot's private tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -55,14 +55,25 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.5.4:
+-----------------
+* Gateway GUI:
+  * use the multi-process option when handling the GW if system allow it
+  * print the GW response as well and not only the packets
+  * add more options to the macro
+  * add options to run and config gw separately
+  
+* owner change GUI:
+  * added support to move tags from AWS to GCP
+
 Version 4.4.4:
 -----------------
 * Added association tool to associate between tags and id for GCP and AWS platforms
 
 * local gw gui:
   * add start/stop gw app instead of only reset option
```

### Comparing `wiliot-tools-4.4.4/README.md` & `wiliot-tools-4.5.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,25 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.5.4:
+-----------------
+* Gateway GUI:
+  * use the multi-process option when handling the GW if system allow it
+  * print the GW response as well and not only the packets
+  * add more options to the macro
+  * add options to run and config gw separately
+  
+* owner change GUI:
+  * added support to move tags from AWS to GCP
+
 Version 4.4.4:
 -----------------
 * Added association tool to associate between tags and id for GCP and AWS platforms
 
 * local gw gui:
   * add start/stop gw app instead of only reset option
```

### Comparing `wiliot-tools-4.4.4/bitbucket-pipelines.yml` & `wiliot-tools-4.5.4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/setup.py` & `wiliot-tools-4.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,16 @@
                  packages=setuptools.find_packages(),
                  package_data={"": ["*.*"]},  # add all support files to the installation
                  install_requires=[
                      'setuptools_scm',
                      'pyserial',
                      'pandas',
                      'pygubu==0.16',
-                     'wiliot-api>=4.7.1',
-                     'wiliot-core>=5.4.3',
+                     'wiliot-api>=4.8.2',
+                     'wiliot-core>=5.5.8',
                      'customtkinter>=5.0.3',
                      'pillow>=9.0.1',
                      'CtkMessagebox'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                  include_package_data=True,
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/association_tool/association_configs.py` & `wiliot-tools-4.5.4/wiliot_tools/association_tool/association_configs.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/association_tool/association_tool.py` & `wiliot-tools-4.5.4/wiliot_tools/association_tool/association_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         """
         self.is_stop = is_stop_event
         self.is_new_label = new_label_event
         self.logger = logging.getLogger(logger_name)
         self.associate_q = associate_q
 
         self.scanner = CognexDataMan(log_name=logger_name)
+        # TODO add here config to upload cognex file
         if not self.scanner.connected:
             raise Exception('Could not connect to Cognex. please check connection and other app usage')
 
     def run(self):
         self.logger.info('Starts Scanner Association')
         t_start = time.time()
         need_to_recovery = False
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/association_tool/send_association_to_cloud.py` & `wiliot-tools-4.5.4/wiliot_tools/association_tool/send_association_to_cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,42 +71,43 @@
 OWNER_ID = '185369804174'
 GDC_TYPE = 'hvdc'  # options: outbound-pallet, hvdc
 CATEGORY_ID = '1e55d376-a12f-4f75-9583-ff8bad995d35'
 IS_GCP = False
 
 
 class CloudAssociation(object):
-    def __init__(self, associate_q, stop_event):
+    def __init__(self, associate_q, stop_event, owner_id=OWNER_ID, is_gcp=IS_GCP, category_id=CATEGORY_ID):
         """
         @type associate_q Queue
         @param associate_q each element of the queue is a dict {'wiliot_code': [], 'asset_code': [], 'timestamp': 0}
         """
         self.logger_path, self.logger = set_logger(app_name='CloudAssociation',
                                                    dir_name='cloud_association', file_name='cloud_association_log')
         self.associate_q = associate_q
         self.is_stop_event = stop_event
         self.associate_batch = {}
         try:
-            _, api_key, is_successful = check_user_config_is_ok(env='prod', owner_id=OWNER_ID, client_type='asset')
-            if IS_GCP:
-                self.client = PlatformClient(api_key=api_key, owner_id=OWNER_ID,  env='prod', logger_=self.logger.name,
+            _, api_key, is_successful = check_user_config_is_ok(env='prod', owner_id=owner_id, client_type='asset')
+            if is_gcp:
+                self.client = PlatformClient(api_key=api_key, owner_id=owner_id,  env='prod', logger_=self.logger.name,
                                              cloud='GCP', region='us-central1')
             else:
-                self.client = PlatformClient(api_key=api_key, owner_id=OWNER_ID,  env='prod', logger_=self.logger.name)
+                self.client = PlatformClient(api_key=api_key, owner_id=owner_id,  env='prod', logger_=self.logger.name)
         except Exception as e:
             self.logger.warning(f' Could not create a client due to {e}')
             raise Exception(f' Could not create a client due to {e}')
 
         try:
             self.base_payload = {"scan_source": "gdc",
                                  "pixel_id": [],
                                  "asset_id": None,
                                  "gdc_type": GDC_TYPE,
                                  "timestamp": datetime.datetime.now().timestamp(),
                                  "printer": True}
+            self.category_id = category_id
         except Exception as e:
             self.logger.warning(f'Could not create the base payload due to {e}')
             raise Exception(f'Could not create the base payload due to {e}')
 
         if associate_q:
             self.run()
 
@@ -134,15 +135,17 @@
         time.sleep(1)
         while not self.associate_q.empty():
             data = self.associate_q.get(timeout=1)
             self.add_data_to_batch(data)
 
         if self.associate_batch:
             self.logger.info('sending data to cloud before exiting CloudAssociation')
-            self.send_batch_to_cloud()
+            bad_association = self.send_batch_to_cloud()
+            if len(bad_association):
+                self.logger.warning(f'association was done with the following bad association: {bad_association}')
         self.logger.info('CloudAssociation is Done')
 
     def add_data_to_batch(self, data):
         wiliot_code = data['wiliot_code']  # list
         asset_id = data['asset_code']
         timestamp = data['timestamp']
 
@@ -155,38 +158,54 @@
             self.associate_batch[asset_id]['pixel_id'] += wiliot_code
             self.associate_batch[asset_id]['timestamp'] += timestamp
         else:
             self.associate_batch[asset_id] = {'pixel_id': wiliot_code}
         self.associate_batch[asset_id]['timestamp'] = timestamp
 
     def send_batch_to_cloud(self):
+        bad_association = []
         payload = self.base_payload.copy()
         for asset_id, pixel_dict in self.associate_batch.items():
             payload["asset_id"] = asset_id
             payload["pixel_id"] = list(set(pixel_dict['pixel_id']))
             payload["timestamp"] = int(pixel_dict['timestamp'] * 1000)
             try:
-                message = self.send_to_cloud_debug(payload)  # TODO remove after debug
+                message = self.send_to_cloud_debug(payload)  # for debug
                 if IS_GCP:
                     message = self.send_to_cloud(payload)
                 else:  # AWS
-                    message = self.create_asset_and_label(asset_id=payload["asset_id"], category_id=CATEGORY_ID,
+                    message = self.create_asset_and_label(asset_id=payload["asset_id"], category_id=self.category_id,
                                                           pixels=payload["pixel_id"])
             except Exception as e:
                 message = {'status_code': 999,
                            'data': f'Exception during send_to_cloud {e}'}
 
-            if message['status_code'] == 201:
-                self.logger.info(f'Successful Association for {asset_id}: {message}')
-            elif message['status_code'] == 403:
-                self.logger.warning(f'Failed Association for {asset_id} due '
-                                    f'to Authentication and authorization issues: {message}')
-            else:
-                self.logger.warning(f'Failed Association for {asset_id} due '
-                                    f'to Unexpected error: {message}')
+            bad_association = self.handle_results(message, asset_id, pixel_dict, bad_association)
+
+        for b_ass in bad_association:  # try again bad association
+            self.add_data_to_batch(b_ass)
+
+        return bad_association
+
+    def handle_results(self, message, asset_id, pixel_dict, bad_association):
+        if message['status_code'] == 201:
+            self.logger.info(f'Successful Association for {asset_id}: {message}')
+        else:
+            bad_association.append({'asset_code': asset_id,
+                                    'wiliot_code': pixel_dict['pixel_id'],
+                                    'timestamp': pixel_dict['timestamp']})
+        if message['status_code'] in [404, 409, 504]:
+            pass  # already handled
+        elif message['status_code'] == 403:
+            self.logger.warning(f'Failed Association for {asset_id} due '
+                                f'to Authentication and authorization issues: {message}')
+        else:
+            self.logger.warning(f'Failed Association for {asset_id} due '
+                                f'to Unexpected error: {message}')
+        return bad_association
 
     def send_to_cloud(self, payload):
         self.client._renew_token()
         headers = {'Content-Type': 'Application/json',
                    'Authorization': f'Bearer {self.client.headers["Authorization"]}'}
         response = requests.post(url=URL_PATH, headers=headers,
                                  data=json.dumps({"data": payload}), params=None)
@@ -234,14 +253,18 @@
                         """
 
                         if success:
                             self.logger.info(f"Associated pixel {pixel} to asset {asset_id}")
                         else:
                             raise Exception("Association failed with no cloud exception")
                     except Exception as e:
+                        if e.args[0]['status_code'] == 400 and \
+                                'tagId is already associated with this asset' in e.args[0]['error']:
+                            self.logger.info(f"pixel {pixel} is already associate to asset {asset_id}")
+                            continue
                         res = {"data": f"Association for {asset_id} and {pixel} failed due to {e}",
                                "status_code": 710}
                         bad_res_list.append(res)
                 if bad_res_list:
                     res = {"data": '\n'.join([b_res["data"] for b_res in bad_res_list]),
                            "status_code": 710}
                 else:
@@ -281,15 +304,14 @@
                     if wce.args[0].get('status_code', '') == 404:
                         # Either the pixel or the category do not exist in this account
                         self.logger.warning(f"One or more of the pixels do not exist in the account")
                         self.logger.warning(wce.args[0].get('error'))
                     elif wce.args[0].get('status_code', '') == 504:
                         # If the upstream server timed out - return from here - this will be retried
                         self.logger.error("Upstream server timeout")
-                        try_again = 'timeout'
                     elif wce.args[0].get('status_code', '') == 409:
                         # There are two situations we can get a 409 error:
                         # 1. The tag is already associated with another asset - can happen when an asset ID and pixel
                         # are scanned more than once. In this case - we log and exit because there is nothing
                         # else to do
                         if wce.args[0].get("error", "").lower().find("already associated") != -1:
                             self.logger.error(f"Tag {pixels} already associated with an asset")
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/association_tool/sensor_count/sensor_count.ino` & `wiliot-tools-4.5.4/wiliot_tools/association_tool/sensor_count/sensor_count.ino`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/__init__.py` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/local_gateway_gui.py` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/local_gateway_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,22 +131,23 @@
 EP_DEFAULT = 18  # Energizing pattern
 EPs_DEFAULT = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28,
                50, 51, 52)  # All Energizing pattern
 TP_O_DEFAULT = 5  # timing profile on
 TP_P_DEFAULT = 15  # timing profile period
 PI_DEFAULT = 0  # pace interval
 RC_DEFAULT = 37
-RCs_DEFAULT = (37, 38, 39)
+RCs_DEFAULT = tuple(range(40))
 DATA_TYPES = ('raw', 'processed', 'statistics', 'full_UID_mode', 'decoded_packet')
 CONFIG_SUM = "EP:{EP}\nTP_ON:{TP_ON}\nTP_P:{TP_P}\nRC:{RC}\nPI:{PI}\nF:{F}"
 baud_rates = ["921600"]
 energy_pattern_dict = {18: 'Energizing on channel 39 only',
-                       20: '20% channel 37 , 80% channel 39',
-                       50: 'Energizing in 915Mhz',
+                       17: 'beacons only',
+                       50: 'Energizing on 915Mhz + beacons + beacons',
                        51: 'Energizing on both channel 39 and 915Mhz',
+                       52: 'Energizing on 915Mhz only'
                        }
 
 __version__ = get_version()
 
 
 def prepare_version_attribute_options():
     version_attributes = {}
@@ -328,15 +329,15 @@
 
         self.gwAllCommands = self.gwCommands + self.gwUserCommands
 
         self.ttk.lift()
         self.ttk.attributes("-topmost", True)
         self.ttk.attributes("-topmost", False)
 
-        self.ObjGW = WiliotGateway(logger_name=self.full_run_logger.name)
+        self.ObjGW = WiliotGateway(logger_name=self.full_run_logger.name, is_multi_processes=sys.platform != 'darwin')
         self.config_param = {}
         self.formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
         self.logger_num = 1
 
         # update ui
         if self.decryption_mode:
             self.multi_tag = DecryptedTagCollection()
@@ -449,14 +450,15 @@
             try:
                 port = self.builder.get_object('port_box').get().rsplit(' ', 1)[0]
                 baud = self.builder.get_object('baud_rate_box').get().rsplit(' ', 1)[0]
                 if port == '' or baud == '':
                     return
 
                 if self.ObjGW.open_port(port, baud):  # open and check if succeed
+                    self.ObjGW.start_continuous_listener()
                     self.print_function(str_in="> Port successfully opened")
                     self.portActive = True
                     self.builder.get_object('connect_button').configure(text='Disconnect')
                     # print version:
                     self.print_function(str_in=self.ObjGW.hw_version + '=' + self.ObjGW.sw_version)
                     self.builder.get_object('recv_box').see(END)
                     # config gw to receive packets (and not only manage bridges):
@@ -664,14 +666,21 @@
                             self.print_function(str_in=str_to_print)
 
                     elif data_type == DataType.RAW:
                         str_to_print = self.get_raw_str(data_in)
                         self.print_function(str_in=str_to_print)
 
                     consecutive_exception_counter = 0
+
+                if self.ObjGW is not None and self.ObjGW.continuous_listener_enabled and \
+                        (self.is_gw_running or self.ObjGW.is_data_available()):
+                    gw_rsps = self.ObjGW.get_gw_responses()
+                    for rsp in gw_rsps:
+                        self.print_function(', '.join(['{}: {}'.format(k, v) for k, v in rsp.items()]))
+
             except Exception as e:
                 print(f'got exception during recv_data: {e}, try to recovery')
                 consecutive_exception_counter = consecutive_exception_counter + 1
                 if consecutive_exception_counter > MAX_CONSECUTIVE_EXCEPTION:
                     self.full_run_logger.exception(f"Abort DataHandlerProcess due to {e}")
                     return
 
@@ -719,23 +728,29 @@
             self.print_function(str_in="> Update GW version was failed ")
 
     def on_reset(self):
         self.ObjGW.reset_gw()
         time.sleep(1)
         self.ObjGW.reset_listener()
         self.on_clear()
+        self.is_gw_running = False
+        self.ui_update(state='config')
 
     def start_live_plotting(self):
+        self.builder.get_object('data_type').set('decoded_packet')
+        self.on_data_type_change('decoded_packet')
         if self.dash_plotting_instance is None:
             if not DECRYPTION_MODE:
                 raise Exception('Cannot run WiliotLivePlotting on public version, '
                                 'please make sure you have Wiliot Private package')
-            self.dash_plotting_instance = WiliotLivePlotting(self.get_tag_collection, self.stop_live_plots_event, self.logger)
+            self.dash_plotting_instance = WiliotLivePlotting(live_tag_collection=self.get_tag_collection,
+                                                             stop_event=self.stop_live_plots_event,
+                                                             logger=self.logger)
             self.dash_plotting_instance.init_live_plot()
-        webbrowser.open("http://127.0.0.1:8050/")
+        webbrowser.open(self.dash_plotting_instance.get_live_plot_url())
 
     def get_tag_collection(self):
         return self.multi_tag
 
     def on_enter_write(self, args):
         if args.char == '\r':
             self.on_write()
@@ -770,72 +785,90 @@
             data_handler_listener.start()
         else:
             self.print_function("Please select a valid macro")
 
     def run_macro(self):
         selected_macro = self.builder.get_object('macros_ddl').get()
         macro_commands = macros[selected_macro]
-        for c in macro_commands:
-            command_value = c["command"]
-            time_value = c["wait"]
-            self.print_function("Command: {c},\t Wait: {t}".format(c=command_value, t=time_value))
-            command_start_time = time.time()
-            if command_value == 'user_event':
-                self.on_user_event(user_event_text=c.get('values', 'user_event'))
-            elif command_value == 'save_log':
-                self.on_processed_data(c.get('values', r'~/Downloads/output.csv'))
-            elif command_value == 'update_version':
-                self.on_update_gw_version_helper(c.get('values', r''))
-            else:
-                rsp_val = self.ObjGW.write(command_value, with_ack=True)
-                self.on_user_event(user_event_text=command_value)
-                self.print_function(', '.join(['{}: {}'.format(k, v) for k, v in rsp_val.items()]))
-                # self.start_listening()
-            while time.time() - command_start_time < time_value:
-                time.sleep(1)
-        self.print_function('Macro {selected_macro} Done.'.format(selected_macro=selected_macro))
-
-    def on_config(self):
-        self.on_bridge_support()
+        is_cyclic = any(['cyclic' in c.keys() and c['cyclic'] for c in macro_commands])
+        is_first = True
+        self.print_function(f'Macro {selected_macro} Starts')
+        while is_first or is_cyclic:
+            for c in macro_commands:
+                if "command" not in c.keys():
+                    continue
+                command_value = c["command"]
+                time_value = c["wait"]
+                self.print_function("Command: {c},\t Wait: {t}".format(c=command_value, t=time_value))
+                command_start_time = time.time()
+                if command_value == 'user_event':
+                    self.on_user_event(user_event_text=c.get('values', 'user_event'))
+                elif command_value == 'save_log':
+                    self.on_processed_data(c.get('values', r'~/Downloads/output.csv'))
+                elif command_value == 'update_version':
+                    self.on_update_gw_version_helper(c.get('values', r''))
+                else:
+                    rsp_val = self.ObjGW.write(command_value, with_ack=True)
+                    self.on_user_event(user_event_text=command_value)
+                    self.print_function(', '.join(['{}: {}'.format(k, v) for k, v in rsp_val.items()]))
+                    # self.start_listening()
+                while time.time() - command_start_time < time_value:
+                    time.sleep(1)
+            if not self.is_gw_running:
+                break
+        self.print_function(f'Macro {selected_macro} Done.')
+
+    def on_config_and_run(self):
+        self.on_config()
+        self.on_run()
 
+    def on_run(self):
         if self.is_gw_running:
             is_stopped = self.ObjGW.stop_gw_app()
-            self.print_function(f'Gw transmitting and receiving was {"" if is_stopped else "NOT"} stopped')
+            self.print_function(f'Gw transmitting and receiving was {"" if is_stopped else "NOT "}stopped')
         else:
-            pacer_val = int(self.builder.get_object('pace_inter').get())
-            energ_ptrn_val = int(self.builder.get_object('energizing_pattern').get())
-            time_profile_val = [int(self.builder.get_object('timing_profile_on').get()),
-                                int(self.builder.get_object('timing_profile_period').get())]
-            received_channel_val = int(self.builder.get_object('received_channel').get())
-            self.print_function(str_in="> Setting GW configuration...")
-            if energ_ptrn_val in energy_pattern_dict.keys():
-                self.print_function(str_in='Setting pattern {energ_ptrn_val} -> {pattern_explanation}'.format(
-                    energ_ptrn_val=str(energ_ptrn_val), pattern_explanation=energy_pattern_dict[energ_ptrn_val]))
-
-            config_param_set, gateway_response = self.ObjGW.config_gw(pacer_val=pacer_val,
-                                                                      energy_pattern_val=energ_ptrn_val,
-                                                                      time_profile_val=time_profile_val,
-                                                                      received_channel=received_channel_val,
-                                                                      with_ack=True)
-
-            # update user event
-            for event in gateway_response:
-                user_event_data = f"raw: {event['raw']}, command: {event['command']}"
-                new_row = pd.DataFrame([{'user_event_time': event['time'], 'user_event_data': user_event_data}])
-                self.user_events = pd.concat([self.user_events, new_row], ignore_index=True)
-
-            # update config parameters:
-            for key, value in config_param_set.__dict__.items():
-                self.config_param[key] = str(value)
-
-            self.print_function(str_in="> Configuration is set")
+            self.ObjGW.config_gw(start_gw_app=True)
 
         self.is_gw_running = not self.is_gw_running
         self.ui_update(state='config')
 
+    def on_config(self):
+        self.on_bridge_support()
+
+        pacer_val = int(self.builder.get_object('pace_inter').get())
+        energ_ptrn_val = int(self.builder.get_object('energizing_pattern').get())
+        time_profile_val = [int(self.builder.get_object('timing_profile_on').get()),
+                            int(self.builder.get_object('timing_profile_period').get())]
+        received_channel_val = int(self.builder.get_object('received_channel').get())
+
+        self.print_function(str_in="> Setting GW configuration...")
+        if energ_ptrn_val in energy_pattern_dict.keys():
+            self.print_function(str_in=f'Setting pattern {energ_ptrn_val} -> {energy_pattern_dict[energ_ptrn_val]}')
+
+        config_param_set, gateway_response = self.ObjGW.config_gw(pacer_val=pacer_val,
+                                                                  energy_pattern_val=energ_ptrn_val,
+                                                                  time_profile_val=time_profile_val,
+                                                                  received_channel=received_channel_val,
+                                                                  with_ack=True,
+                                                                  start_gw_app=False)
+
+        # update user event
+        for event in gateway_response:
+            user_event_data = f"raw: {event['raw']}, command: {event['command']}"
+            new_row = pd.DataFrame([{'user_event_time': event['time'], 'user_event_data': user_event_data}])
+            self.user_events = pd.concat([self.user_events, new_row], ignore_index=True)
+            self.print_function(', '.join(['{}: {}'.format(k, v) for k, v in event.items()]))
+
+        # update config parameters:
+        for key, value in config_param_set.__dict__.items():
+            self.config_param[key] = str(value)
+
+        self.print_function(str_in="> Configuration is set")
+        self.ui_update(state='config')
+
     def on_clear(self, restart=True):
         self.builder.get_object('recv_box').delete('1.0', END)
         self.builder.get_object('recv_box').see(END)
         if restart:
             self.multi_tag = DecryptedTagCollection() if DECRYPTION_MODE else TagCollection()
             if self.decryption_mode:
                 self.update_tags_count_label(0)
@@ -899,15 +932,16 @@
 
     def on_bridge_support(self):
         self.is_listen_to_bridge = self.builder.get_variable('bridge_support_state').get()
         self.ObjGW.write(f'!listen_to_tag_only {int(not self.is_listen_to_bridge)}')
 
     def on_data_type_change(self, selected):
         self.on_clear()
-        if selected.widget.get() == 'decoded_packet' or selected.widget.get() == 'full_UID_mode':
+        selected_type = selected if isinstance(selected, str) else selected.widget.get()
+        if selected_type == 'decoded_packet' or selected_type == 'full_UID_mode':
             self.builder.get_object('filter_id')['state'] = 'enabled'
             self.builder.get_object('filter_id').delete(0, 'end')
             self.builder.get_object('filter_id').insert(0, 'filter ids')
             self.get_filter_text()
             if self.decryption_mode:
                 self.builder.get_object('save_to_file')['state'] = 'enabled'
                 self.builder.get_object('plot_log')['state'] = 'enabled'
@@ -934,14 +968,16 @@
     def on_custom_plots(self):
         t = Toplevel(self.ttk)
         CustomPlotGui(plot_config=self.plot_config, print_func=self.print_function, tk_frame=t,
                       logger=self.full_run_logger)
 
     def on_advanced(self):
         t = Toplevel(self.ttk)
+        t.attributes('-topmost', True)
+        t.after(100, lambda: t.attributes('-topmost', False))
         AdvancedGui(gw_obj=self.ObjGW, print_func=self.print_function, tk_frame=t, logger=self.full_run_logger)
 
     def on_user_event(self, user_event_text=None):
         if user_event_text is None:
             user_event_text = self.builder.get_object('user_event_text').get()
         self.print_function(str_in="user_event_time: {}, User event: {}".format(self.ObjGW.get_curr_timestamp_in_sec(),
                                                                                 user_event_text))
@@ -1190,14 +1226,16 @@
                 self.builder.get_object('version_num_cur').delete('1.0', END)
                 self.builder.get_object('version_num_cur').insert(END, 'current:')
                 self.builder.get_object('config_sum').delete(1.0, END)
                 self.builder.get_object('config_sum').insert(END, CONFIG_SUM.format(
                     RC="", EP="", TP_ON="", TP_P="", PI="", F=""))
                 self.builder.get_object('config_sum').see(END)
 
+            self.builder.get_object('config_and_run_button')['state'] = enable_disable_str
+            self.builder.get_object('run_button')['state'] = enable_disable_str
             self.builder.get_object('config_button')['state'] = enable_disable_str
             self.builder.get_object('energizing_pattern')['state'] = enable_disable_str
             self.builder.get_object('timing_profile_on')['state'] = enable_disable_str
             self.builder.get_object('timing_profile_period')['state'] = enable_disable_str
             self.builder.get_object('pace_inter')['state'] = enable_disable_str
             self.builder.get_object('write_button')['state'] = enable_disable_str
             self.builder.get_object('write_box')['state'] = enable_disable_str
@@ -1225,21 +1263,25 @@
                                                                            EP=self.config_param["energy_pattern"],
                                                                            TP_ON=self.config_param["time_profile_on"],
                                                                            TP_P=self.config_param[
                                                                                "time_profile_period"],
                                                                            PI=self.config_param["pacer_val"],
                                                                            F=self.config_param["filter"]))
             self.builder.get_object('config_sum').see(END)
-            self.builder.get_object('config_button')['text'] = 'Stop Gw' if self.is_gw_running else 'Run Config'
+            self.builder.get_object('config_and_run_button')['text'] = 'Stop Gw' \
+                if self.is_gw_running else 'Configure and Run'
             enable_disable_str = 'disabled' if self.is_gw_running else 'enabled'
             self.builder.get_object('energizing_pattern')['state'] = enable_disable_str
             self.builder.get_object('timing_profile_on')['state'] = enable_disable_str
             self.builder.get_object('timing_profile_period')['state'] = enable_disable_str
             self.builder.get_object('received_channel')['state'] = enable_disable_str
             self.builder.get_object('pace_inter')['state'] = enable_disable_str
+            self.builder.get_object('config_button')['state'] = enable_disable_str
+            self.builder.get_object('run_button')['state'] = enable_disable_str
+
             if DECRYPTION_MODE:
                 self.builder.get_object('advanced_gui')['state'] = enable_disable_str
 
     def on_log_browser(self):
         path_loc = filedialog.asksaveasfilename(
             filetypes=[("txt file", ".log")], defaultextension=".log", title='Choose location to save log',
             initialfile='gw_log_{}.log'.format(datetime.datetime.now().strftime("%Y%m%d_%H%M%S")))
@@ -1547,18 +1589,14 @@
         self.advanced_builder.connect_callbacks(self)
         self.advanced_builder.connect_callbacks(self)
         self.ttk_advanced.lift()
         self.ttk_advanced.attributes("-topmost", True)
 
         self.advanced_builder.get_object('mini_rx_operation')['values'] = tuple(MiniRxOperations.__members__)
         self.advanced_builder.get_object('mini_rx_value')['values'] = tuple()
-        self.advanced_builder.get_object('mini_rx_scan_ch')['values'] = tuple(range(40))
-        self.advanced_builder.get_object('mini_rx_scan_ch').set(0)
-        self.advanced_builder.get_object('mini_rx_white_ch')['values'] = tuple(range(40))
-        self.advanced_builder.get_object('mini_rx_white_ch').set(0)
 
         self.advanced_builder.get_variable('mini_rx_sub1g').set(False)
 
         self.ttk_advanced.protocol("WM_DELETE_WINDOW", self.close_window)
         self.ttk_advanced.after_idle(self.periodic_call)
         self.ttk_advanced.mainloop()
 
@@ -1577,49 +1615,40 @@
         elif selected_operation == MiniRxOperations.DEBUG_PACKET.name:
             self.operation_value = DebugPacketValues
             values = tuple(DebugPacketValues.__members__)
         else:
             return
 
         self.advanced_builder.get_object('mini_rx_value')['values'] = values
+        self.advanced_builder.get_object('mini_rx_value').set('')
         self.operation = MiniRxOperations[selected_operation]
 
-    def update_whiten(self, args):
-        self.advanced_builder.get_object('mini_rx_white_ch').set(
-            self.advanced_builder.get_object('mini_rx_scan_ch').get())
-
     def on_run(self):
-        scan_ch = self.advanced_builder.get_object('mini_rx_scan_ch').get()
-        white_ch = self.advanced_builder.get_object('mini_rx_white_ch').get()
-        if scan_ch:
-            cmd = f'!scan_ch {scan_ch}'
-            cmd += f' {white_ch}' if white_ch else ''
-            rsp = self.gw_obj.write(cmd)
-            self.print_func(f'command:{cmd}, time:{rsp["time"]}, rsp:{rsp["raw"]}')
         operation_value = self.advanced_builder.get_object('mini_rx_value').get()
         sub1g_energy = self.advanced_builder.get_variable('mini_rx_sub1g').get()
-        start_gw_app = True
-        self.gw_obj.send_mini_rx(self.operation, self.operation_value[operation_value],
-                                 sub1g_energy=sub1g_energy,
-                                 start_gw_app=start_gw_app)
-        self.print_func(f'running mini with the following parameters: operation: '
-                        f'{self.operation}, value: {operation_value}, sub1g energy: {sub1g_energy}, '
-                        f'start gw app: {start_gw_app}')
-        self.close_requested = True
+
+        try:
+            self.gw_obj.send_mini_rx(self.operation, self.operation_value[operation_value],
+                                     sub1g_energy=sub1g_energy,
+                                     start_gw_app=False)
+            self.print_func(f'running mini with the following parameters: operation: '
+                            f'{self.operation}, value: {operation_value}, sub1g energy: {sub1g_energy}')
+        except Exception as e:
+            self.logger.exception('problem occurred during advanced setting: {}'.format(e))
 
     def periodic_call(self):
         if not self.close_requested:
             self.ttk_advanced.after(500, self.periodic_call)
 
         else:
             print("Destroying Advanced GUI at:", time.time())
             try:
                 self.ttk_advanced.destroy()
             except Exception as e:
-                self.logger.exception('problem occured during exit the gui: {}'.format(e))
+                self.logger.exception('problem occurred during exit the gui: {}'.format(e))
                 exit(1)
 
     def close_window(self):
         self.close_requested = True
         print("User requested close at:", time.time())
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/.gwCommands.json` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/.gwCommands.json`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/__init__.py` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/advanced_gui.ui` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/advanced_gui.ui`

 * *Files 18% similar despite different names*

#### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/advanced_gui.ui` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/advanced_gui.ui`

```diff
@@ -27,15 +27,15 @@
           <property name="propagate">True</property>
           <property name="row">1</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="mini_rx_operation">
-        <bind add="" handler="change_value_type" sequence="&lt;FocusOut&gt;"/>
+        <bind add="" handler="change_value_type" sequence="&lt;FocusIn&gt;"/>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="columnspan">2</property>
           <property name="padx">10</property>
           <property name="propagate">True</property>
           <property name="row">2</property>
         </layout>
@@ -75,57 +75,18 @@
           <property name="row">5</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="mini_rx_run">
         <property cbtype="simple" name="command" type="command">on_run</property>
-        <property name="text" translatable="yes">RUN</property>
+        <property name="text" translatable="yes">Send Configuration</property>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="pady">10</property>
           <property name="propagate">True</property>
           <property name="row">10</property>
         </layout>
       </object>
     </child>
-    <child>
-      <object class="ttk.Label" id="label4">
-        <property name="text" translatable="yes">scan channel</property>
-        <layout manager="grid">
-          <property name="column">0</property>
-          <property name="propagate">True</property>
-          <property name="row">6</property>
-        </layout>
-      </object>
-    </child>
-    <child>
-      <object class="ttk.Combobox" id="mini_rx_scan_ch">
-        <bind add="True" handler="update_whiten" sequence="&lt;FocusOut&gt;"/>
-        <layout manager="grid">
-          <property name="column">0</property>
-          <property name="propagate">True</property>
-          <property name="row">7</property>
-        </layout>
-      </object>
-    </child>
-    <child>
-      <object class="ttk.Label" id="label5">
-        <property name="text" translatable="yes">whitening channel</property>
-        <layout manager="grid">
-          <property name="column">0</property>
-          <property name="propagate">True</property>
-          <property name="row">8</property>
-        </layout>
-      </object>
-    </child>
-    <child>
-      <object class="ttk.Combobox" id="mini_rx_white_ch">
-        <layout manager="grid">
-          <property name="column">0</property>
-          <property name="propagate">True</property>
-          <property name="row">9</property>
-        </layout>
-      </object>
-    </child>
   </object>
 </interface>
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/configs.gif` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/configs.gif`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/custom_ep.ui` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/custom_ep.ui`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/custom_plots.ui` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/custom_plots.ui`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui`

 * *Files 1% similar despite different names*

#### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui`

```diff
@@ -205,20 +205,19 @@
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="config_button">
         <property cbtype="simple" name="command" type="command">on_config</property>
-        <property name="text" translatable="yes">Run Config</property>
+        <property name="text" translatable="yes">Configure Only</property>
         <layout manager="grid">
-          <property name="column">4</property>
-          <property name="columnspan">4</property>
-          <property name="row">0</property>
-          <property name="sticky">ew</property>
+          <property name="column">6</property>
+          <property name="columnspan">2</property>
+          <property name="row">8</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Label" id="label2">
         <property name="text" translatable="yes">Energizing Pattern:</property>
         <layout manager="grid">
@@ -293,15 +292,15 @@
     </child>
     <child>
       <object class="ttk.Combobox" id="received_channel">
         <property name="state">disabled</property>
         <property name="width">4</property>
         <layout manager="grid">
           <property name="column">5</property>
-          <property name="columnspan">2</property>
+          <property name="columnspan">1</property>
           <property name="ipadx">10</property>
           <property name="row">4</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
@@ -683,15 +682,14 @@
       </object>
     </child>
     <child>
       <object class="ttk.Separator" id="separator1">
         <property name="orient">vertical</property>
         <layout manager="grid">
           <property name="column">13</property>
-          <property name="propagate">True</property>
           <property name="row">0</property>
           <property name="rowspan">9</property>
           <property name="sticky">ns</property>
         </layout>
       </object>
     </child>
     <child>
@@ -701,50 +699,70 @@
         <property name="onvalue">1</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">listen to bridge</property>
         <property name="variable">boolean:bridge_support_state</property>
         <layout manager="grid">
           <property name="column">4</property>
           <property name="columnspan">2</property>
-          <property name="propagate">True</property>
           <property name="row">7</property>
           <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="packet_version_list">
         <property name="state">disabled</property>
         <layout manager="grid">
           <property name="column">6</property>
-          <property name="propagate">True</property>
           <property name="row">7</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Label" id="label5">
         <property name="text" translatable="yes">packet
 version</property>
         <layout manager="grid">
           <property name="column">5</property>
-          <property name="propagate">True</property>
           <property name="row">7</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="advanced_gui">
         <property cbtype="simple" name="command" type="command">on_advanced</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">advanced setting</property>
         <layout manager="grid">
           <property name="column">4</property>
           <property name="columnspan">1</property>
-          <property name="propagate">True</property>
           <property name="row">8</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
+    <child>
+      <object class="ttk.Button" id="run_button">
+        <property cbtype="simple" name="command" type="command">on_run</property>
+        <property name="text" translatable="yes">Run only</property>
+        <layout manager="grid">
+          <property name="column">5</property>
+          <property name="columnspan">2</property>
+          <property name="row">8</property>
+        </layout>
+      </object>
+    </child>
+    <child>
+      <object class="ttk.Button" id="config_and_run_button">
+        <property cbtype="simple" name="command" type="command">on_config_and_run</property>
+        <property name="text" translatable="yes">Configure and Run</property>
+        <layout manager="grid">
+          <property name="column">4</property>
+          <property name="columnspan">4</property>
+          <property name="propagate">True</property>
+          <property name="row">0</property>
+          <property name="sticky">ew</property>
+        </layout>
+      </object>
+    </child>
   </object>
 </interface>
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/local_gateway_gui/utils/gw_macros.py` & `wiliot-tools-4.5.4/wiliot_tools/local_gateway_gui/utils/gw_macros.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     ** user_event, it will trigger user event with the specified text under 'values' key
     ** save log, it will save the log at the specified location under 'values' key
     * wait : time to wait in seconds after the command is done
 
 """
 
 macros = {
-    "update_version_macro": [{"command": "update_version", 'values': r'', "wait": 1},],
+    "update_version_macro": [{"command": "update_version", 'values': r'', "wait": 1}],
     "example_macro": [
         {"command": "!version", "wait": 3},
         {"command": "user_event", 'values': 'Set tag in initial location', "wait": 1},
         {"command": "!output_power pos3dBm", "wait": 5},
         {"command": "user_event", 'values': 'Pick up tag', "wait": 1},
         {"command": "!gateway_app 37 15 5 18", "wait": 3},
         {"command": "!cancel", "wait": 1},
@@ -93,9 +93,14 @@
         {"command": "!set_sub_1_ghz_energizing_frequency 915000", "wait": 0},
         {"command": "!beacons_backoff 0", "wait": 0},
         {"command": "user_event", 'values': 'Set new config', "wait": 0},
         {"command": "!gateway_app 37 15 5 50", "wait": 90},  # test for 90 seconds
         {"command": "!cancel", "wait": 1},
         {"command": "user_event", 'values': 'Stop gw app and eneter into brownout', "wait": 300},
         {"command": "save_log", 'values': r'~/Downloads/output.csv', "wait": 0},
+    ],
+    "toggle_rx_channel": [
+        {"cyclic": True},
+        {"command": "!scan_ch 37 37", "wait": 1},
+        {"command": "!scan_ch 0 0", "wait": 1},
     ]
 }
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/owner_change_app.py` & `wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/shipment_approval_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 from tkinter import ttk
 from wiliot_api import ManufacturingClient
-from wiliot_tools.owner_change_gui.owner_change_requests_page import *
-from wiliot_tools.owner_change_gui.requests_details_page import *
-from wiliot_tools.owner_change_gui.send_request_multiple_reels_page import *
-from wiliot_tools.owner_change_gui.send_request_one_reel_page import *
 
+from wiliot_tools.shipment_approval_gui.resources.config import col_width
+from wiliot_tools.shipment_approval_gui.shipment_approval_requests_page import *
+from wiliot_tools.shipment_approval_gui.requests_details_page import *
+from wiliot_tools.shipment_approval_gui.send_request_multiple_reels_page import *
+from wiliot_tools.shipment_approval_gui.send_request_one_reel_page import *
 
-class OwnerChangeApp(ctk.CTk):
-    def __init__(self):
+
+class ShipmentApprovalApp(ctk.CTk):
+    def __init__(self, env="prod"):
         super().__init__()
+        self.env = env
         self.prev_api_key = ""
         style = ttk.Style(self)
         style.configure("Treeview.Heading", background="#39a987", foreground="black")
         self.W = 1200
         self.H = 800
-        self.title("Owner Change")
+        self.title("Shipment Approval")
         self.geometry(f"{self.W}x{self.H}")
         self.resizable(0, 0)
         ctk.set_appearance_mode("light")
         ctk.set_default_color_theme("resources/wiliot-green")
         if not os.path.exists("data"):
             os.makedirs("data")
         self.api_key = ""
         self.setup_config()
         self.client = None
         self.attached_df = None
-        self.requests_df = None
-        self.col_width_dict = col_width()
-        self.selected_cols = ['-', '-', '-', '-', '-']
-        self.cols = ['Ex. ID Prefix', 'First Tag', 'Last Tag', 'To Owner']
-        self.requests_cols = ['Tracking ID', 'From Owner', 'To Owner', 'Status', 'Total Tags', 'Passed', 'Failed', 'Sent At']
-        OwnerChangeRequests(self, self.show_send_request_multiple_reels_page).pack(fill="both", expand=True)
+        self.requests = None
+        self.selected_cols = ['-']
+        self.cols = ['Ex. ID Prefix']
+        ShipmentApprovalRequests(self, self.show_send_request_multiple_reels_page).pack(fill="both", expand=True)
 
     def setup_config(self):
         config = configparser.ConfigParser()
         if not os.path.exists('resources/config.ini'):
             config['API'] = {'key': ''}
             with open('resources/config.ini', 'w') as configfile:
                 config.write(configfile)
         config.read('resources/config.ini')
         self.api_key = config['API']['key']
 
     def get_col_width(self, col, cols, width):
-        return int(self.col_width_dict[col] * width / sum([self.col_width_dict[col] for col in cols]))
+        return int(col_width[col] * width / sum([col_width[col] for col in cols]))
 
     def show_error_popup(self, message, width=400, height=200):
         CTkMessagebox(master=self, title="Error", message=message, icon="cancel", width=width, height=height)
 
     def show_request_details_page(self, request_id, prev_frame):
         prev_frame.destroy()
-        RequestDetails(self, self.show_owner_change_requests_page, request_id=request_id).pack(fill="both", expand=True)
+        RequestDetails(self, self.show_shipment_approval_requests_page, request_id=request_id).pack(fill="both", expand=True)
 
-    def show_owner_change_requests_page(self, prev_frame):
+    def show_shipment_approval_requests_page(self, prev_frame):
         prev_frame.destroy()
-        OwnerChangeRequests(self, self.show_send_request_multiple_reels_page).pack(fill="both", expand=True)
+        ShipmentApprovalRequests(self, self.show_send_request_multiple_reels_page).pack(fill="both", expand=True)
 
     def show_send_request_multiple_reels_page(self, prev_frame):
         prev_frame.destroy()
-        MultiReelRequestPage(self, self.show_owner_change_requests_page).pack(fill="both", expand=True)
+        MultiReelRequestPage(self, self.show_shipment_approval_requests_page).pack(fill="both", expand=True)
 
     def show_send_request_one_reel_page(self, prev_frame):
         prev_frame.destroy()
-        OneReelRequestPage(self, self.show_owner_change_requests_page).pack(fill="both", expand=True)
-
-    def save_data(self):
-        self.requests_df.to_csv("data/requests.csv")
+        OneReelRequestPage(self, self.show_shipment_approval_requests_page).pack(fill="both", expand=True)
 
     def create_tree_view(self, frame, df, equal_width=True, height=23, width=100):
         tree = ttk.Treeview(frame, columns=list(df.columns), show="headings", height=height)
         for col in df.columns:
             tree.heading(col, text=col)
             if equal_width:
                 tree.column(col, width=(self.W - width) // len(df.columns), anchor="center")
@@ -77,34 +75,35 @@
 
         for index, row in df.iterrows():
             tree.insert("", "end", values=list(row))
         return tree
 
     def check_client(self):
         if self.prev_api_key != self.api_key:
-            self.client = ManufacturingClient(api_key=self.api_key)
+            self.client = ManufacturingClient(api_key=self.api_key, env=self.env)
             self.prev_api_key = self.api_key
 
-    def send_request_file(self, from_owner, to_owner, df):
+    def send_request(self, external_id_prefix):
         self.check_client()
-        file_path = "data/tags_tmp.csv"
-        df.to_csv(file_path)
-        request_id = self.client.change_pixel_owner_by_file(from_owner, to_owner, file_path)
+        request_id = self.client.post_shipment_approval_request(external_id_prefix)
         return request_id
 
     def get_request_status(self, request_id):
         self.check_client()
-        json_data = self.client.get_pixel_change_request_status(request_id)
+        json_data = self.client.get_shipment_approval_request_status(request_id)
         return json_data, json_data['status_code']
 
     def get_request_tags_info(self, request_id):
         file_path = "data/tags_tmp.csv"
         with open(file_path, "w") as f:
             self.check_client()
-            self.client.get_pixel_change_request_details(request_id, f)
-        df = pd.read_csv(file_path)
+            self.client.get_shipment_approval_request_details(request_id, f)
+        try:
+            df = pd.read_csv(file_path)
+        except pd.errors.EmptyDataError:
+            df = pd.DataFrame(columns=['external_id', 'reason'])
         return df
 
 
 if __name__ == "__main__":
-    app = OwnerChangeApp()
+    app = ShipmentApprovalApp()
     app.mainloop()
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/owner_change_requests_page.py` & `wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/shipment_approval_requests_page.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import threading
 import customtkinter as ctk
 import pandas as pd
-from wiliot_tools.owner_change_gui.owner_change_utils import show_img
 
+from wiliot_tools.shipment_approval_gui.requests_df import Requests
+from wiliot_tools.shipment_approval_gui.resources.config import DISPLAY_COLS
+from wiliot_tools.shipment_approval_gui.shipment_approval_utils import show_img, open_csv_with_excel
 
-class OwnerChangeRequests(ctk.CTkFrame):
+
+class ShipmentApprovalRequests(ctk.CTkFrame):
     def __init__(self, parent, show_page_callback):
         super().__init__(parent)
         self.parent = parent
         self.show_page_callback = lambda: show_page_callback(self)
-
-        label = ctk.CTkLabel(self, text="Owner Change Requests", font=("Arial", 28, "bold"))
+        # self.full_cols = ['requestId', 'processStatus', 'externalIdPrefix', 'totalTestedTags', 'passedTags',
+        #                   'failedOfflineTags', 'failedPpAndShipmentTags', 'yield', 'failedSerializationQty',
+        #                   'corruptedTagsQty', 'duplicationsQty', 'numOfCommonRunNames', 'commonRunNames',
+        #                   'firstExternalId', 'lastExternalId', 'gapsTagsQty', 'gapsTags', 'uploadedAt']
+        label = ctk.CTkLabel(self, text="Shipment Approval Requests", font=("Arial", 28, "bold"))
         label.pack(pady=50)
-        if self.parent.requests_df is None:
-            try:
-                self.parent.requests_df = pd.read_csv('data/requests.csv', index_col=0, dtype=str)
-            except FileNotFoundError:
-                self.parent.requests_df = pd.DataFrame(columns=self.parent.requests_cols)
+        if self.parent.requests is None:
+            self.parent.requests = Requests()
         # df = self.parent.df
-        self.tree = self.parent.create_tree_view(self, self.parent.requests_df, equal_width=False)
+        self.tree = self.parent.create_tree_view(self, self.parent.requests.get_df(DISPLAY_COLS), equal_width=False)
         self.tree.tag_configure('red', foreground='#d44e2a')
         self.tree.tag_configure('green', foreground='#39a987')
         self.tree.tag_configure('yellow', foreground='#FFBF00')
         self.tree.tag_configure('orange', foreground='orange')
         self.tree.pack(pady=20, padx=20)
         self.color_requests()
 
         btn = ctk.CTkButton(master=self, text="Request Details", command=self.request_details, width=220,
                             font=('Helvetica', 14))
         btn.place(x=self.parent.W / 2 - 110, y=self.parent.H - 150)
 
+        btn = ctk.CTkButton(master=self, text="Open Full Data in Excel", command=lambda : open_csv_with_excel("data/requests.csv"), width=220,
+                            font=('Helvetica', 14))
+        btn.place(x=self.parent.W / 2 - 110, y=self.parent.H - 100)
+
         self.delete_btn = ctk.CTkButton(master=self, text="Delete Selected", command=lambda: self.delete(), width=220,
                                         font=('Helvetica', 14))
         self.delete_btn.place(x=50, y=self.parent.H - 150)
 
         self.delete_btn = ctk.CTkButton(master=self, text="Delete All", command=lambda: self.delete(all=True),
                                         width=220,
                                         font=('Helvetica', 14))
@@ -45,77 +52,81 @@
         btn = ctk.CTkButton(self, text="Create Request (One Reel)",
                             command=lambda: self.parent.show_send_request_one_reel_page(self),
                             width=220)
         btn.place(x=self.parent.W - 270, y=self.parent.H - 150)
         show_img(self)
         self.after(1, self.refresh)
 
+
     def request_details(self):
         items = self.tree.selection()
         if len(items) == 0:
             self.parent.show_error_popup("No Request Was Selected!")
             return
         item = items[0]
-        if self.tree.item(item, "values")[3] != 'processed':
+        if self.tree.item(item, "values")[2] != 'processed':
             self.parent.show_error_popup("The Request has not been Processed Yet!")
             return
         request_id = self.tree.item(item, "values")[0]
         self.parent.show_request_details_page(request_id, self)
 
     def color_requests(self):
         for i, item in enumerate(self.tree.get_children()):
             values = self.tree.item(item, "values")
-            if values[3] in ('not-started', 'processing'):
+            if values[2] in ('not started', 'processing', 'sent for processing'):
                 self.tree.item(item, tags=('yellow',))
-            elif values[3] == 'failed':
+            elif values[2] in ('failed', 'missing commonRunNames'):
                 self.tree.item(item, tags=('red',))
-            elif values[3] == 'processed' and int(values[6]) == int(values[4]):
-                self.tree.item(item, tags=('red',))
-            elif values[3] == 'processed' and int(values[6]) > 0:
-                self.tree.item(item, tags=('orange',))
-            elif values[3] == 'processed':
+            elif values[2] == 'processed' and all([values[i] == 'Passed' for i in range(-1, -6, -1)]):
                 self.tree.item(item, tags=('green',))
+            elif values[2] == 'processed':
+                self.tree.item(item, tags=('red',))
 
-    def sync(self):
-        self.parent.requests_df = pd.DataFrame(
-            [self.tree.item(item, "values") for item in self.tree.get_children()],
-            columns=self.parent.requests_cols
-        )
+
+    # def sync(self):
+    #     self.parent.requests_df = pd.DataFrame(
+    #         [self.tree.item(item, "values") for item in self.tree.get_children()],
+    #         columns=self.parent.requests_cols
+    #     )
+
+    def update_request(self, item, response):
+        request_id = response['requestId']
+        self.parent.requests.delete(request_id)
+        display_values = self.parent.requests.process_response(response)
+        self.tree.item(item, values=display_values)
 
     def update_requests(self):
         for item in self.tree.get_children():
             values = self.tree.item(item, "values")
-            if values[3] in ('not-started', '-', 'processing'):
+            if values[2] in ('not started', '-', 'processing', 'sent for processing'):
                 response, status_code = self.parent.get_request_status(values[0])
                 if status_code == 200:
-                    new_values = list(response.values())[:7] + [values[7]]
-                    new_values = ['-' if str(v) == 'None' else v for v in new_values]
-                    self.update_item(item, new_values)
+                    # new_values = [response.get(col, '-') if col in response else response['summaryData'].get(col, '-')
+                    #               for col in self.full_cols]
+                    self.update_request(item, response)
                 else:
                     values = list(values)
-                    values[3] = 'failed'
-                    self.update_item(item, values)
+                    values[2] = 'failed'
+                    self.update_request(item, values)
                     print(f"API Response {status_code}, Response: {response}")
 
         self.color_requests()
-        self.sync()
-        self.parent.save_data()
+        self.parent.requests.save_data()
 
     def refresh(self):
         print('Refreshing Requests!')
         threading.Thread(target=self.update_requests).start()
         self.after(30000, self.refresh)
 
-    def update_item(self, item_id, new_values):
-        self.tree.item(item_id, values=new_values)
-
     def delete(self, all=False):
         if all:
             items = self.tree.get_children()
         else:
             items = self.tree.selection()
             if len(items) == 0:
                 self.parent.show_error_popup("No Request Was Selected!")
                 return
         for item in items:
+            request_id = self.tree.item(item, "values")[0]
+            self.parent.requests.delete(request_id)
             self.tree.delete(item)
-        self.sync()
+        self.parent.requests.save_data()
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/owner_change_utils.py` & `wiliot-tools-4.5.4/wiliot_tools/shipment_approval_gui/shipment_approval_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from PIL import Image, ImageTk
 import json
 import customtkinter as ctk
 import pandas as pd
-
-
-def col_width():
-    with open("resources/columns_width.json", "r") as json_file:
-        cols_width = json.load(json_file)
-    return cols_width
+import os
+import subprocess
 
 
 def show_img(frame):
     try:
         image = Image.open("resources/wiliot.png")
         image = image.resize((150, 75))
         tk_image = ImageTk.PhotoImage(image)
@@ -36,24 +32,39 @@
         for x in range(int(row['First Tag']), int(row['Last Tag']) + 1):
             rows.append(row['Ex. ID Prefix'] + "T" + str(x).zfill(4))
     rows = set(rows)
     return pd.DataFrame([[row] for row in rows], columns=['tagId']).sort_values('tagId')
 
 
 def verify_file(df):
-    if not all((df['Ex. ID Prefix'].str.len() >= 4)):
+    if not all((df['Ex. ID Prefix'].str.len() >= 3)):
         raise ValueError(f"Not all values for column 'Ex. ID Prefix' are correct\n"
-                         "please verify that all values at least 4 letters")
+                         "please verify that all values at least 3 letters")
 
     if not df['First Tag'].apply(can_be_int).all():
         raise ValueError(f"Not all values for column 'First Tag' are numbers and under 10000")
 
     if not df['Last Tag'].apply(can_be_int).all():
         raise ValueError(f"Not all values for column 'Last Tag' are numbers and under 10000")
 
     if not df['To Owner'].apply(lambda x: x != "").all():
         raise ValueError(f"To Owner column has empty values")
 
     for i, row in df.iterrows():
         if str(row['First Tag']).zfill(4) > str(row['Last Tag']).zfill(4):
             raise ValueError(f"First Tag is bigger than Last Tag\n"
                              f"({row['Ex. ID Prefix']}, {row['First Tag']}, {row['Last Tag']})")
+
+
+def open_csv_with_excel(csv_file_path):
+    if os.path.exists(csv_file_path):
+        try:
+            subprocess.Popen(["excel", csv_file_path])
+        except:
+            try:
+                subprocess.call(["open", "-a", "Microsoft Excel", csv_file_path])
+            except FileNotFoundError:
+                raise Exception("Microsoft Excel is not found. Please make sure Excel is installed on your PC.")
+            except Exception as e:
+                print(f"An error occurred: {e}")
+    else:
+        raise Exception("Something went wrong!")
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/requests_details_page.py` & `wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/requests_details_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import threading
-from wiliot_tools.owner_change_gui.owner_change_utils import *
+from owner_change_utils import *
 
 
 class RequestDetails(ctk.CTkFrame):
 
     def __init__(self, parent, show_page_callback, request_id=None):
         super().__init__(parent)
         self.tags_df = None
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/resources/wiliot-green` & `wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/resources/wiliot-green`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/resources/wiliot.png` & `wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/resources/wiliot.png`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/send_request_multiple_reels_page.py` & `wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/send_request_multiple_reels_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import configparser
 import os
 from tkinter import filedialog
 from CTkMessagebox import CTkMessagebox
-from wiliot_tools.owner_change_gui.owner_change_utils import *
+from owner_change_utils import *
 from datetime import datetime
 
 
 class MultiReelRequestPage(ctk.CTkFrame):
 
     def __init__(self, parent, show_page_callback):
         super().__init__(parent)
@@ -105,15 +105,15 @@
                     self.parent.requests_df = pd.concat([request_df, self.parent.requests_df])
                 except Exception as ex:
                     failed_to_owners.append(to_owner)
                     expections.append(str(ex))
             if len(failed_to_owners) > 0:
                 for failed_to_owner, expection in zip(failed_to_owners, expections):
                     request_df = pd.DataFrame(
-                        [[expection, from_owner, failed_to_owner, 'failed', '-', '-', '-', str(datetime.now())[:16]]],
+                        [[expection, from_owner, failed_to_owner, 'failed', '-', '-', '-', str(datetime.now())[:16], 'AWS']],
                         columns=self.parent.requests_cols)
                     self.parent.requests_df = pd.concat([request_df, self.parent.requests_df])
                     print(f'\n - To Owner: {failed_to_owner} reason: {expection}')
                 message = f"Requests Failed For These Owners:\n {failed_to_owners}"
                 message += "\n\n Please find file failed_owners.csv in the same dirictory as the input file," \
                            "\nplease fix the issues and upload again."
                 df[df['To Owner'].isin(failed_to_owners)].to_csv(
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/owner_change_gui/send_request_one_reel_page.py` & `wiliot-tools-4.5.4/wiliot_tools/owner_change_gui/send_request_one_reel_page.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import configparser
 from datetime import datetime
-from wiliot_tools.owner_change_gui.owner_change_utils import *
+from owner_change_utils import *
 
 
 class OneReelRequestPage(ctk.CTkFrame):
 
     def __init__(self, parent, show_page_callback):
         super().__init__(parent)
         self.parent = parent
         self.show_page_callback = lambda: show_page_callback(self)
         self.tree = None
         self.parent.attached_df = None
         show_img(self)
 
-        start_y = 200
+        start_y = 150
         label_width = 120
         entry_width = 200
         y_spacing = 70
         x_spacing = 50
 
         label = ctk.CTkLabel(self, text="Create Request (One Reel)", font=("Arial", 28, "bold"))
         label.pack(pady=50)
@@ -55,19 +55,35 @@
 
         label = ctk.CTkLabel(self, text="Last Tag:", font=("Arial", 15))
         label.place(x=self.parent.W / 2 - label_width - 10 - x_spacing, y=start_y + 5 * y_spacing)
 
         self.last_tag_entry = ctk.CTkEntry(self, width=entry_width)
         self.last_tag_entry.place(x=self.parent.W / 2 + 10 - x_spacing, y=start_y + 5 * y_spacing)
 
+        label = ctk.CTkLabel(self, text="Cloud Destination:", font=("Arial", 15))
+        label.place(x=self.parent.W / 2 - label_width - 10 - x_spacing, y=start_y + 6 * y_spacing)
+
+        # self.cloud_destination = ctk.CTkEntry(self, width=entry_width)
+        # self.cloud_destination.place(x=self.parent.W / 2 + 10 - x_spacing, y=start_y + 6 * y_spacing)
+        self.cloud_destination = ctk.CTkComboBox(master=self, values=['AWS', 'GCP'], justify='center',width=entry_width)
+        self.cloud_destination.place(x=self.parent.W / 2 + 10 - x_spacing, y=start_y + 6 * y_spacing)
+        self.cloud_destination.set('AWS')
+
+        label = ctk.CTkLabel(self, text="GCP API Key:", font=("Arial", 15))
+        label.place(x=self.parent.W / 2 - label_width - 10 - x_spacing, y=start_y + 7 * y_spacing)
+
+        self.gcp_api_key_entry = ctk.CTkEntry(self, width=entry_width, show="*")
+        self.gcp_api_key_entry.place(x=self.parent.W / 2 + 10 - x_spacing, y=start_y + 7 * y_spacing)
+        self.gcp_api_key_entry.insert(0, self.parent.gcp_api_key)
+
         btn = ctk.CTkButton(self, text="Back", command=self.show_page_callback, width=120)
         btn.place(x=50, y=self.parent.H - 50)
 
         btn = ctk.CTkButton(self, text="Send Request", command=self.send_request, width=200)
-        btn.place(x=self.parent.W / 2 - btn.winfo_reqwidth() / 2, y=start_y + 7 * y_spacing)
+        btn.place(x=self.parent.W / 2 - btn.winfo_reqwidth() / 2, y=start_y + 8 * y_spacing)
 
     def verify_request(self):
         if len(self.ex_id_prefix_entry.get()) < 4:
             raise ValueError(f"Ex. ID Prefix valuue must be at least 4 letters")
 
         if not can_be_int(self.first_tag_entry.get()):
             raise ValueError(f"First Tag must be a number and under 10000")
@@ -77,27 +93,25 @@
 
         if str(self.first_tag_entry.get()).zfill(4) > str(self.last_tag_entry.get()).zfill(4):
             raise ValueError(f"First Tag is bigger than Last Tag")
 
     def send_request(self):
         try:
             self.verify_request()
-            config = configparser.ConfigParser()
-            self.parent.api_key = self.api_key_entry.get()
-            config['API'] = {'key': self.parent.api_key}
-            with open('resources/config.ini', 'w') as configfile:
-                config.write(configfile)
+            self.parent.save_api_keys(self.api_key_entry.get(), self.gcp_api_key_entry.get())
+
             df = pd.DataFrame([[self.ex_id_prefix_entry.get(), self.first_tag_entry.get(), self.last_tag_entry.get()]],
                               columns=self.parent.cols[:-1])
-            tags_df = create_tags_df(df)
+            tags_df = create_tags_df(df, self.parent.seperator)
             from_owner = self.from_owner_entry.get()
             to_owner = self.to_owner_entry.get()
+            cloud_destination = self.cloud_destination.get()
             if from_owner == "" or to_owner == "" or self.parent.api_key == "":
                 raise Exception("Some Fields are Empty!")
-            request_id = self.parent.send_request_file(from_owner, to_owner, tags_df)
+            request_id = self.parent.send_request_file(from_owner, to_owner, tags_df, cloud_destination)
             df.to_csv('data/' + request_id + '.csv')
-            request_df = pd.DataFrame([[request_id, '-', '-', '-', '-', '-', '-', str(datetime.now())[:16]]],
+            request_df = pd.DataFrame([[request_id, '-', '-', '-', '-', '-', '-', str(datetime.now())[:16], cloud_destination]],
                                       columns=self.parent.requests_cols)
             self.parent.requests_df = pd.concat([request_df, self.parent.requests_df])
             self.show_page_callback()
         except Exception as ex:
             self.parent.show_error_popup(str(ex))
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools/utils/get_version.py` & `wiliot-tools-4.5.4/wiliot_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.4.4/wiliot_tools.egg-info/PKG-INFO` & `wiliot-tools-4.5.4/wiliot_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-tools
-Version: 4.4.4
+Version: 4.5.4
 Summary: A library for interacting with Wiliot's private tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -55,14 +55,25 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.5.4:
+-----------------
+* Gateway GUI:
+  * use the multi-process option when handling the GW if system allow it
+  * print the GW response as well and not only the packets
+  * add more options to the macro
+  * add options to run and config gw separately
+  
+* owner change GUI:
+  * added support to move tags from AWS to GCP
+
 Version 4.4.4:
 -----------------
 * Added association tool to associate between tags and id for GCP and AWS platforms
 
 * local gw gui:
   * add start/stop gw app instead of only reset option
```

### Comparing `wiliot-tools-4.4.4/wiliot_tools.egg-info/SOURCES.txt` & `wiliot-tools-4.5.4/wiliot_tools.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 wiliot_tools/association_tool/__init__.py
 wiliot_tools/association_tool/association_configs.py
 wiliot_tools/association_tool/association_tool.py
 wiliot_tools/association_tool/send_association_to_cloud.py
 wiliot_tools/association_tool/sensor_count/__init__.py
 wiliot_tools/association_tool/sensor_count/sensor_count.ino
 wiliot_tools/local_gateway_gui/__init__.py
-wiliot_tools/local_gateway_gui/gw_configs.py
 wiliot_tools/local_gateway_gui/local_gateway_gui.bat
 wiliot_tools/local_gateway_gui/local_gateway_gui.py
 wiliot_tools/local_gateway_gui/utils/.gwCommands.json
 wiliot_tools/local_gateway_gui/utils/__init__.py
 wiliot_tools/local_gateway_gui/utils/advanced_gui.ui
 wiliot_tools/local_gateway_gui/utils/configs.gif
 wiliot_tools/local_gateway_gui/utils/custom_ep.ui
@@ -34,18 +33,31 @@
 wiliot_tools/local_gateway_gui/utils/debug_mode.py
 wiliot_tools/local_gateway_gui/utils/folder.png
 wiliot_tools/local_gateway_gui/utils/gw_debugger.ui
 wiliot_tools/local_gateway_gui/utils/gw_macros.py
 wiliot_tools/owner_change_gui/__init__.py
 wiliot_tools/owner_change_gui/owner_change_app.py
 wiliot_tools/owner_change_gui/owner_change_gui.bat
-wiliot_tools/owner_change_gui/owner_change_gui.sh
+wiliot_tools/owner_change_gui/owner_change_main.py
 wiliot_tools/owner_change_gui/owner_change_requests_page.py
 wiliot_tools/owner_change_gui/owner_change_utils.py
 wiliot_tools/owner_change_gui/requests_details_page.py
 wiliot_tools/owner_change_gui/send_request_multiple_reels_page.py
 wiliot_tools/owner_change_gui/send_request_one_reel_page.py
 wiliot_tools/owner_change_gui/resources/columns_width.json
 wiliot_tools/owner_change_gui/resources/wiliot-green
 wiliot_tools/owner_change_gui/resources/wiliot.png
+wiliot_tools/shipment_approval_gui/__init__.py
+wiliot_tools/shipment_approval_gui/requests_details_page.py
+wiliot_tools/shipment_approval_gui/requests_df.py
+wiliot_tools/shipment_approval_gui/send_request_multiple_reels_page.py
+wiliot_tools/shipment_approval_gui/send_request_one_reel_page.py
+wiliot_tools/shipment_approval_gui/shipment_approval_app.py
+wiliot_tools/shipment_approval_gui/shipment_approval_gui.bat
+wiliot_tools/shipment_approval_gui/shipment_approval_gui.sh
+wiliot_tools/shipment_approval_gui/shipment_approval_requests_page.py
+wiliot_tools/shipment_approval_gui/shipment_approval_utils.py
+wiliot_tools/shipment_approval_gui/resources/config.py
+wiliot_tools/shipment_approval_gui/resources/wiliot-green
+wiliot_tools/shipment_approval_gui/resources/wiliot.png
 wiliot_tools/utils/__init__.py
 wiliot_tools/utils/get_version.py
```

