# Comparing `tmp/scs-core-3.9.4.tar.gz` & `tmp/scs-core-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-core-3.9.4.tar", last modified: Tue Feb  6 15:51:39 2024, max compression
+gzip compressed data, was "scs-core-3.9.5.tar", last modified: Tue Feb 20 11:09:43 2024, max compression
```

## Comparing `scs-core-3.9.4.tar` & `scs-core-3.9.5.tar`

### file list

```diff
@@ -1,517 +1,517 @@
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.018481 scs-core-3.9.4/
--rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:38.000000 scs-core-3.9.4/LICENSE
--rw-r--r--   0 bruno      (502) admin       (80)       77 2023-11-22 14:02:56.000000 scs-core-3.9.4/MANIFEST.in
--rw-r--r--   0 bruno      (502) admin       (80)     2303 2024-02-06 15:51:39.018294 scs-core-3.9.4/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)     1404 2023-09-11 10:21:38.000000 scs-core-3.9.4/README.md
--rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:38.000000 scs-core-3.9.4/README.rst
--rw-r--r--   0 bruno      (502) admin       (80)      124 2023-09-11 10:21:38.000000 scs-core-3.9.4/requirements.txt
--rw-r--r--   0 bruno      (502) admin       (80)       38 2024-02-06 15:51:39.018517 scs-core-3.9.4/setup.cfg
--rwxr-xr-x   0 bruno      (502) admin       (80)     2258 2024-01-31 08:47:30.000000 scs-core-3.9.4/setup.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.949126 scs-core-3.9.4/src/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.955450 scs-core-3.9.4/src/scs_core/
--rw-r--r--   0 bruno      (502) admin       (80)      183 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.956134 scs-core-3.9.4/src/scs_core/aqcsv/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.956438 scs-core-3.9.4/src/scs_core/aqcsv/conf/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/conf/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2617 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/conf/airnow_site_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     1034 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.957003 scs-core-3.9.4/src/scs_core/aqcsv/connector/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/connector/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)    10215 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/connector/airnow_mapping_task.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.957203 scs-core-3.9.4/src/scs_core/aqcsv/connector/archive/
--rw-r--r--   0 bruno      (502) admin       (80)      448 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/connector/archive/source_mappings.csv
--rw-r--r--   0 bruno      (502) admin       (80)     6657 2024-01-08 13:20:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/connector/datum_mapping.py
--rw-r--r--   0 bruno      (502) admin       (80)     5042 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/connector/source_mapping.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.957697 scs-core-3.9.4/src/scs_core/aqcsv/data/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/data/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3764 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/data/aqcsv_datetime.py
--rw-r--r--   0 bruno      (502) admin       (80)    13736 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/data/aqcsv_record.py
--rw-r--r--   0 bruno      (502) admin       (80)     3046 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/data/aqcsv_site.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.959101 scs-core-3.9.4/src/scs_core/aqcsv/specification/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2837 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/agency.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.961475 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/
--rw-r--r--   0 bruno      (502) admin       (80)    10261 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/agencies.csv
--rw-r--r--   0 bruno      (502) admin       (80)     4728 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/countries.csv
--rw-r--r--   0 bruno      (502) admin       (80)  1079325 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/methods.csv
--rw-r--r--   0 bruno      (502) admin       (80)      768 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/mpcs.csv
--rw-r--r--   0 bruno      (502) admin       (80)    28901 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/parameters.csv
--rw-r--r--   0 bruno      (502) admin       (80)      149 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/qcs.csv
--rw-r--r--   0 bruno      (502) admin       (80)     5420 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/qualifiers.csv
--rw-r--r--   0 bruno      (502) admin       (80)     2484 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/units.csv
--rw-r--r--   0 bruno      (502) admin       (80)     2742 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/country.py
--rw-r--r--   0 bruno      (502) admin       (80)     1163 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/country_iso.py
--rw-r--r--   0 bruno      (502) admin       (80)     1175 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/country_numeric.py
--rw-r--r--   0 bruno      (502) admin       (80)     9813 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/method.py
--rw-r--r--   0 bruno      (502) admin       (80)     3778 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/mpc.py
--rw-r--r--   0 bruno      (502) admin       (80)     3466 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/parameter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2868 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/qc.py
--rw-r--r--   0 bruno      (502) admin       (80)     3745 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/qualifier.py
--rw-r--r--   0 bruno      (502) admin       (80)     2892 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aqcsv/specification/unit.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.961613 scs-core-3.9.4/src/scs_core/aws/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.963545 scs-core-3.9.4/src/scs_core/aws/client/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3585 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client/access_key.py
--rw-r--r--   0 bruno      (502) admin       (80)     2332 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client/api_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     2960 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/client/api_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     1576 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/client/api_intercourse.py
--rw-r--r--   0 bruno      (502) admin       (80)     1217 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client/client.py
--rw-r--r--   0 bruno      (502) admin       (80)     5103 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client/client_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     1264 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client/device_control_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3294 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client/email_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3361 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client/monitor_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     7544 2023-11-09 16:14:47.000000 scs-core-3.9.4/src/scs_core/aws/client/mqtt_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     4002 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/client/rest_client.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.964070 scs-core-3.9.4/src/scs_core/aws/client_traffic/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/client_traffic/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     6793 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/client_traffic/client_traffic.py
--rw-r--r--   0 bruno      (502) admin       (80)     1475 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/client_traffic/client_traffic_finder.py
--rw-r--r--   0 bruno      (502) admin       (80)     4636 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/client_traffic/client_traffic_intercourse.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.964424 scs-core-3.9.4/src/scs_core/aws/config/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/config/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)      744 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/config/aws.py
--rw-r--r--   0 bruno      (502) admin       (80)     4471 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/config/project.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.965203 scs-core-3.9.4/src/scs_core/aws/data/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/data/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4998 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/data/dataset.py
--rw-r--r--   0 bruno      (502) admin       (80)     3550 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/data/deployment.py
--rw-r--r--   0 bruno      (502) admin       (80)     2956 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/data/http_response.py
--rw-r--r--   0 bruno      (502) admin       (80)     3175 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/data/message.py
--rw-r--r--   0 bruno      (502) admin       (80)     2884 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/data/upload_interval.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.966080 scs-core-3.9.4/src/scs_core/aws/greengrass/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1998 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/aws_deployer.py
--rw-r--r--   0 bruno      (502) admin       (80)     3017 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/aws_deployment_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     9610 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/aws_group.py
--rw-r--r--   0 bruno      (502) admin       (80)    16808 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/aws_group_configuration.py
--rw-r--r--   0 bruno      (502) admin       (80)    11557 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/aws_identity.py
--rw-r--r--   0 bruno      (502) admin       (80)      440 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/gg_errors.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.966214 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.966465 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/g0/
--rw-r--r--   0 bruno      (502) admin       (80)     2259 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/g0/gg_functions.json
--rw-r--r--   0 bruno      (502) admin       (80)     1736 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/g0/gg_resources.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.966962 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/m0/
--rw-r--r--   0 bruno      (502) admin       (80)     1245 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/m0/gg_functions.json
--rw-r--r--   0 bruno      (502) admin       (80)      216 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/m0/gg_logger.json
--rw-r--r--   0 bruno      (502) admin       (80)      485 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/m0/gg_resources.json
--rw-r--r--   0 bruno      (502) admin       (80)     1450 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/m0/gg_subscriptions.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.967208 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oE.1/
--rw-r--r--   0 bruno      (502) admin       (80)     3781 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oE.1/gg_functions.json
--rw-r--r--   0 bruno      (502) admin       (80)     2607 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oE.1/gg_resources.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.967453 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oP.2/
--rw-r--r--   0 bruno      (502) admin       (80)     2259 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oP.2/gg_functions.json
--rw-r--r--   0 bruno      (502) admin       (80)     1607 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oP.2/gg_resources.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.967699 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oPG.2/
--rw-r--r--   0 bruno      (502) admin       (80)     3781 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oPG.2/gg_functions.json
--rw-r--r--   0 bruno      (502) admin       (80)     2478 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oPG.2/gg_resources.json
--rw-r--r--   0 bruno      (502) admin       (80)      108 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/read.me
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.967947 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/uE.1/
--rw-r--r--   0 bruno      (502) admin       (80)     4256 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/uE.1/gg_functions.json
--rw-r--r--   0 bruno      (502) admin       (80)     3954 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/uE.1/gg_resources.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.968241 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/vB.1/
--rw-r--r--   0 bruno      (502) admin       (80)     3781 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/vB.1/gg_functions.json
--rw-r--r--   0 bruno      (502) admin       (80)     2652 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/greengrass/templates/vB.1/gg_resources.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.969184 scs-core-3.9.4/src/scs_core/aws/manager/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/manager/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.970324 scs-core-3.9.4/src/scs_core/aws/manager/byline/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/byline/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     9906 2023-12-13 16:10:25.000000 scs-core-3.9.4/src/scs_core/aws/manager/byline/byline.py
--rw-r--r--   0 bruno      (502) admin       (80)     3872 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/byline/byline_finder.py
--rw-r--r--   0 bruno      (502) admin       (80)     2784 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/byline/byline_intercourse.py
--rw-r--r--   0 bruno      (502) admin       (80)     1792 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/byline/byline_list.py
--rw-r--r--   0 bruno      (502) admin       (80)     3726 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/byline/byline_manager.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.971382 scs-core-3.9.4/src/scs_core/aws/manager/configuration/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/configuration/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1351 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_check_finder.py
--rw-r--r--   0 bruno      (502) admin       (80)     6032 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_check_intercourse.py
--rw-r--r--   0 bruno      (502) admin       (80)     1251 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_check_requester.py
--rw-r--r--   0 bruno      (502) admin       (80)     2082 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_check_requester_intercourse.py
--rw-r--r--   0 bruno      (502) admin       (80)     1289 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_finder.py
--rw-r--r--   0 bruno      (502) admin       (80)     8803 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_intercourse.py
--rw-r--r--   0 bruno      (502) admin       (80)    10200 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/dynamo_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     3527 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/manager/ec2_message_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)    16782 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/aws/manager/lambda_message_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)    18063 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/aws/manager/s3_manager.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.971765 scs-core-3.9.4/src/scs_core/aws/manager/sagemaker/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/sagemaker/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4295 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/sagemaker/sagemaker_model_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     7802 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/sagemaker/sagemaker_trial_manager.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.972151 scs-core-3.9.4/src/scs_core/aws/manager/topic_history/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/topic_history/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)    13260 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/aws/manager/topic_history/topic_history_intercourse.py
--rw-r--r--   0 bruno      (502) admin       (80)     2352 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/manager/topic_history/topic_history_manager.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.972290 scs-core-3.9.4/src/scs_core/aws/monitor/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.973173 scs-core-3.9.4/src/scs_core/aws/monitor/alert/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/alert/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)    18013 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert.py
--rw-r--r--   0 bruno      (502) admin       (80)     5632 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert_specification_intercourse.py
--rw-r--r--   0 bruno      (502) admin       (80)     2682 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert_specification_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     5830 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert_status_intercourse.py
--rw-r--r--   0 bruno      (502) admin       (80)     1425 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert_status_manager.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.974769 scs-core-3.9.4/src/scs_core/aws/monitor/device/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     5348 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_email_list.py
--rw-r--r--   0 bruno      (502) admin       (80)    18902 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_report.py
--rw-r--r--   0 bruno      (502) admin       (80)     8821 2023-11-22 11:44:01.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_specification.py
--rw-r--r--   0 bruno      (502) admin       (80)     2610 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_specification_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     1207 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_status_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     1776 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/power_list.py
--rw-r--r--   0 bruno      (502) admin       (80)     1795 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/status_list.py
--rw-r--r--   0 bruno      (502) admin       (80)     1792 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/monitor/device/uptime_list.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.978566 scs-core-3.9.4/src/scs_core/aws/security/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/security/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1157 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/security/access_key_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     9194 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_authentication.py
--rw-r--r--   0 bruno      (502) admin       (80)     5244 2023-11-21 12:16:13.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_client_credentials.py
--rw-r--r--   0 bruno      (502) admin       (80)     7852 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_device.py
--rw-r--r--   0 bruno      (502) admin       (80)     1507 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_device_creator.py
--rw-r--r--   0 bruno      (502) admin       (80)     2597 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_device_finder.py
--rw-r--r--   0 bruno      (502) admin       (80)     2111 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_device_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     1506 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_login_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     2600 2023-09-13 10:24:58.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_membership.py
--rw-r--r--   0 bruno      (502) admin       (80)     2280 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_password_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)    11923 2023-09-13 10:24:58.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_user.py
--rw-r--r--   0 bruno      (502) admin       (80)     2714 2023-09-25 13:43:59.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_user_finder.py
--rw-r--r--   0 bruno      (502) admin       (80)     3134 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/security/cognito_user_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     2936 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/security/device_whitelist_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     1947 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/security/opr_membership.py
--rw-r--r--   0 bruno      (502) admin       (80)    23762 2023-12-13 16:10:25.000000 scs-core-3.9.4/src/scs_core/aws/security/organisation.py
--rw-r--r--   0 bruno      (502) admin       (80)    11204 2023-09-25 13:43:59.000000 scs-core-3.9.4/src/scs_core/aws/security/organisation_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     2397 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/aws/security/organisation_membership.py
--rw-r--r--   0 bruno      (502) admin       (80)     1752 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/aws/security/path_filter.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.979712 scs-core-3.9.4/src/scs_core/client/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/client/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4378 2023-11-09 16:14:47.000000 scs-core-3.9.4/src/scs_core/client/http_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     7578 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/client/http_exception.py
--rw-r--r--   0 bruno      (502) admin       (80)      497 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/client/http_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     2831 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/client/network.py
--rw-r--r--   0 bruno      (502) admin       (80)     1415 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/client/resource_unavailable_exception.py
--rw-r--r--   0 bruno      (502) admin       (80)     2638 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/client/sftp_client_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.981048 scs-core-3.9.4/src/scs_core/climate/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1407 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/absolute_humidity.py
--rw-r--r--   0 bruno      (502) admin       (80)     1418 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/icp10101_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3081 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/mpl115a2_calib.py
--rw-r--r--   0 bruno      (502) admin       (80)     2911 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/mpl115a2_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     2290 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/pressure_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     2188 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/pressure_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3156 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/sht_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     1844 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/climate/sht_datum.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.981914 scs-core-3.9.4/src/scs_core/comms/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/comms/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3125 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/comms/mqtt_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     2395 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/comms/uds_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     1552 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/comms/uds_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)     2350 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/comms/uds_server.py
--rw-r--r--   0 bruno      (502) admin       (80)     1614 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/comms/uds_writer.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.982614 scs-core-3.9.4/src/scs_core/control/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/control/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4918 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/control/command.py
--rw-r--r--   0 bruno      (502) admin       (80)     4897 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/control/control_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3792 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/control/control_handler.py
--rw-r--r--   0 bruno      (502) admin       (80)     4738 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/control/control_receipt.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.984408 scs-core-3.9.4/src/scs_core/csv/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/csv/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1979 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/csv/csv_archive.py
--rw-r--r--   0 bruno      (502) admin       (80)     6044 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/csv/csv_data_log.py
--rw-r--r--   0 bruno      (502) admin       (80)     7484 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/csv/csv_dict.py
--rw-r--r--   0 bruno      (502) admin       (80)     7017 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/csv/csv_log.py
--rw-r--r--   0 bruno      (502) admin       (80)     8640 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/csv/csv_log_cursor_queue.py
--rw-r--r--   0 bruno      (502) admin       (80)     9032 2023-11-27 12:34:26.000000 scs-core-3.9.4/src/scs_core/csv/csv_log_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)     8361 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/csv/csv_logger.py
--rw-r--r--   0 bruno      (502) admin       (80)     4396 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/csv/csv_logger_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     5273 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/csv/csv_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)     4498 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/csv/csv_writer.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.989539 scs-core-3.9.4/src/scs_core/data/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4903 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/data/aggregate.py
--rw-r--r--   0 bruno      (502) admin       (80)     2050 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/array_dict.py
--rw-r--r--   0 bruno      (502) admin       (80)     2415 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/average.py
--rw-r--r--   0 bruno      (502) admin       (80)     2158 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/categorical_regression.py
--rw-r--r--   0 bruno      (502) admin       (80)     8948 2023-11-21 12:16:13.000000 scs-core-3.9.4/src/scs_core/data/checkpoint_generator.py
--rw-r--r--   0 bruno      (502) admin       (80)     1008 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/crc.py
--rw-r--r--   0 bruno      (502) admin       (80)     2092 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/crypt.py
--rw-r--r--   0 bruno      (502) admin       (80)    20317 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/data/datetime.py
--rw-r--r--   0 bruno      (502) admin       (80)     6537 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/data/datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     1510 2023-11-21 12:16:13.000000 scs-core-3.9.4/src/scs_core/data/differential.py
--rw-r--r--   0 bruno      (502) admin       (80)     6560 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/diurnal_period.py
--rw-r--r--   0 bruno      (502) admin       (80)     2634 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/duplicates.py
--rw-r--r--   0 bruno      (502) admin       (80)     3809 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/histogram.py
--rw-r--r--   0 bruno      (502) admin       (80)     1747 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/interval.py
--rw-r--r--   0 bruno      (502) admin       (80)     5951 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/join.py
--rw-r--r--   0 bruno      (502) admin       (80)    14228 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/data/json.py
--rw-r--r--   0 bruno      (502) admin       (80)     3274 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/lin_regress.py
--rw-r--r--   0 bruno      (502) admin       (80)     5617 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/data/linear_regression.py
--rw-r--r--   0 bruno      (502) admin       (80)     1372 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/low_pass_filter.py
--rw-r--r--   0 bruno      (502) admin       (80)     1628 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/median_filter.py
--rw-r--r--   0 bruno      (502) admin       (80)     1892 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/min_list.py
--rw-r--r--   0 bruno      (502) admin       (80)     5682 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/model_delta.py
--rw-r--r--   0 bruno      (502) admin       (80)     8334 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/path_dict.py
--rw-r--r--   0 bruno      (502) admin       (80)     1904 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/period.py
--rw-r--r--   0 bruno      (502) admin       (80)     1291 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/precision.py
--rw-r--r--   0 bruno      (502) admin       (80)     3466 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/publication.py
--rw-r--r--   0 bruno      (502) admin       (80)     4181 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/queue_report.py
--rw-r--r--   0 bruno      (502) admin       (80)    10343 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/recurring_period.py
--rw-r--r--   0 bruno      (502) admin       (80)     1265 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/regression.py
--rw-r--r--   0 bruno      (502) admin       (80)     4348 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/rtc_datetime.py
--rw-r--r--   0 bruno      (502) admin       (80)     2249 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/sample_delta.py
--rw-r--r--   0 bruno      (502) admin       (80)    10713 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/stats.py
--rw-r--r--   0 bruno      (502) admin       (80)     1280 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/str.py
--rw-r--r--   0 bruno      (502) admin       (80)     8129 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/data/timedelta.py
--rw-r--r--   0 bruno      (502) admin       (80)     2272 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/data/tokens.py
--rw-r--r--   0 bruno      (502) admin       (80)     7456 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/data/topic_path.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.989762 scs-core-3.9.4/src/scs_core/display/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/display/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3786 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/display/display_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.990309 scs-core-3.9.4/src/scs_core/email/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/email/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2717 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/email/email.py
--rw-r--r--   0 bruno      (502) admin       (80)     2132 2023-10-13 10:36:59.000000 scs-core-3.9.4/src/scs_core/email/email_queue.py
--rw-r--r--   0 bruno      (502) admin       (80)     2633 2023-11-21 12:16:13.000000 scs-core-3.9.4/src/scs_core/email/email_queue_manager.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.992186 scs-core-3.9.4/src/scs_core/estate/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/estate/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     5502 2023-11-21 12:16:13.000000 scs-core-3.9.4/src/scs_core/estate/baseline_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)    30187 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/estate/configuration.py
--rw-r--r--   0 bruno      (502) admin       (80)     4521 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/estate/configuration_check.py
--rw-r--r--   0 bruno      (502) admin       (80)     5221 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/estate/git_pull.py
--rw-r--r--   0 bruno      (502) admin       (80)     3621 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/estate/git_pull_check.py
--rw-r--r--   0 bruno      (502) admin       (80)     6685 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/estate/mqtt_device_poller.py
--rw-r--r--   0 bruno      (502) admin       (80)     2445 2023-12-01 15:40:33.000000 scs-core-3.9.4/src/scs_core/estate/mqtt_peer.py
--rw-r--r--   0 bruno      (502) admin       (80)     6718 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/estate/package_version.py
--rw-r--r--   0 bruno      (502) admin       (80)     2717 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/estate/software_version.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.992297 scs-core-3.9.4/src/scs_core/exegesis/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/exegesis/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.992635 scs-core-3.9.4/src/scs_core/exegesis/gas/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/exegesis/gas/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)      693 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/exegesis/gas/exegete_catalogue.py
--rw-r--r--   0 bruno      (502) admin       (80)     1345 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/exegesis/gas/exegete_collection.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.993121 scs-core-3.9.4/src/scs_core/exegesis/particulate/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/exegesis/particulate/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)      701 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/exegesis/particulate/exegete_catalogue.py
--rw-r--r--   0 bruno      (502) admin       (80)     1353 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/exegesis/particulate/exegete_collection.py
--rw-r--r--   0 bruno      (502) admin       (80)     2248 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/exegesis/particulate/text.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.994390 scs-core-3.9.4/src/scs_core/gas/
--rw-r--r--   0 bruno      (502) admin       (80)      292 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.995756 scs-core-3.9.4/src/scs_core/gas/a4/
--rw-r--r--   0 bruno      (502) admin       (80)      410 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3700 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4.py
--rw-r--r--   0 bruno      (502) admin       (80)    10274 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4_calib.py
--rw-r--r--   0 bruno      (502) admin       (80)     5667 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     4131 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
--rw-r--r--   0 bruno      (502) admin       (80)     3932 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
--rw-r--r--   0 bruno      (502) admin       (80)     5191 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
--rw-r--r--   0 bruno      (502) admin       (80)     5557 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
--rw-r--r--   0 bruno      (502) admin       (80)     4662 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     6990 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/a4/a4_temp_comp.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.996317 scs-core-3.9.4/src/scs_core/gas/afe/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/afe/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1542 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/afe/afe_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3242 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/afe/pt1000_calib.py
--rw-r--r--   0 bruno      (502) admin       (80)     2445 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/afe/pt1000_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3600 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/afe_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)    11550 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/afe_calib.py
--rw-r--r--   0 bruno      (502) admin       (80)     6742 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/afe_id.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.996590 scs-core-3.9.4/src/scs_core/gas/d4/
--rw-r--r--   0 bruno      (502) admin       (80)      130 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/d4/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3710 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/d4/d4_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3106 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/dsi_calib.py
--rw-r--r--   0 bruno      (502) admin       (80)     4352 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/gas/gas.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.996840 scs-core-3.9.4/src/scs_core/gas/isi/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/isi/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1373 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/isi/isi_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     7370 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/gas/minimum.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.997574 scs-core-3.9.4/src/scs_core/gas/ndir/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/ndir/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1777 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/ndir/ndir.py
--rw-r--r--   0 bruno      (502) admin       (80)     2723 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/ndir/ndir_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     3363 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/gas/ndir/ndir_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3649 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/ndir/ndir_version.py
--rw-r--r--   0 bruno      (502) admin       (80)     3078 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/gas/ndir/ndir_voltages.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.998573 scs-core-3.9.4/src/scs_core/gas/pid/
--rw-r--r--   0 bruno      (502) admin       (80)      378 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/pid/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4498 2024-01-08 13:20:30.000000 scs-core-3.9.4/src/scs_core/gas/pid/pid.py
--rw-r--r--   0 bruno      (502) admin       (80)     7136 2024-01-08 13:20:30.000000 scs-core-3.9.4/src/scs_core/gas/pid/pid_calib.py
--rw-r--r--   0 bruno      (502) admin       (80)     4028 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/pid/pid_calibrated_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3837 2024-01-08 13:20:30.000000 scs-core-3.9.4/src/scs_core/gas/pid/pid_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3694 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/pid/pid_temp_comp.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.999044 scs-core-3.9.4/src/scs_core/gas/scd30/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/scd30/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2538 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/scd30/scd30_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     2804 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/scd30/scd30_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     2866 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/scd30/scd30_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3556 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/sensor.py
--rw-r--r--   0 bruno      (502) admin       (80)     6167 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/gas/sensor_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     3043 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gas/sensor_calib.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.999251 scs-core-3.9.4/src/scs_core/gps/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gps/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4077 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/gps/gps_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.999461 scs-core-3.9.4/src/scs_core/interface/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/interface/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2271 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/interface/interface_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:38.999782 scs-core-3.9.4/src/scs_core/led/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/led/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)      870 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/led/led.py
--rw-r--r--   0 bruno      (502) admin       (80)     2356 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/led/led_state.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.000203 scs-core-3.9.4/src/scs_core/location/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/location/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2992 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/location/timezone.py
--rw-r--r--   0 bruno      (502) admin       (80)     3708 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/location/timezone_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     2379 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/location/timezone_offset.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.000522 scs-core-3.9.4/src/scs_core/model/
--rw-r--r--   0 bruno      (502) admin       (80)      276 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.001279 scs-core-3.9.4/src/scs_core/model/catalogue/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.002319 scs-core-3.9.4/src/scs_core/model/catalogue/archive/
--rw-r--r--   0 bruno      (502) admin       (80)     2027 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/archive/O3-vE-Urban-20H1.json
--rw-r--r--   0 bruno      (502) admin       (80)     1659 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-0p2ppm.json
--rw-r--r--   0 bruno      (502) admin       (80)     1660 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-0p5ppm.json
--rw-r--r--   0 bruno      (502) admin       (80)     1658 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-1ppm.json
--rw-r--r--   0 bruno      (502) admin       (80)     1651 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-50ppb.json
--rw-r--r--   0 bruno      (502) admin       (80)     1651 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3.json
--rw-r--r--   0 bruno      (502) admin       (80)      188 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/archive/uE-1.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.003090 scs-core-3.9.4/src/scs_core/model/catalogue/compendia/
--rw-r--r--   0 bruno      (502) admin       (80)     1663 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/compendia/NO-vE-Urban-20H1.json
--rw-r--r--   0 bruno      (502) admin       (80)     1640 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/compendia/NO2-vE-OPCube-21H1.json
--rw-r--r--   0 bruno      (502) admin       (80)     1643 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/compendia/NO2-vE-OPCube-21HA.json
--rw-r--r--   0 bruno      (502) admin       (80)     1662 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/compendia/NO2-vE-Urban-20HB.json
--rw-r--r--   0 bruno      (502) admin       (80)     2029 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/compendia/O3-vE-Urban-20H1.json
--rw-r--r--   0 bruno      (502) admin       (80)     1643 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/compendia/SO2-vE-Urban-22Q1.json
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.003480 scs-core-3.9.4/src/scs_core/model/catalogue/groups/
--rw-r--r--   0 bruno      (502) admin       (80)       85 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/groups/oE-1.json
--rw-r--r--   0 bruno      (502) admin       (80)      107 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/groups/read.me
--rw-r--r--   0 bruno      (502) admin       (80)      154 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/groups/uE-1.json
--rw-r--r--   0 bruno      (502) admin       (80)    11042 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/model_compendium.py
--rw-r--r--   0 bruno      (502) admin       (80)     4779 2023-11-21 12:16:13.000000 scs-core-3.9.4/src/scs_core/model/catalogue/model_compendium_group.py
--rw-r--r--   0 bruno      (502) admin       (80)     5220 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/term.py
--rw-r--r--   0 bruno      (502) admin       (80)     2038 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/catalogue/training_period.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.004193 scs-core-3.9.4/src/scs_core/model/gas/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3368 2023-11-21 12:16:13.000000 scs-core-3.9.4/src/scs_core/model/gas/baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     1354 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/gas_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     1545 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/gas_inference_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     2873 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/gas/gas_model_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.004558 scs-core-3.9.4/src/scs_core/model/gas/s1/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/s1/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2704 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/s1/gas_request.py
--rw-r--r--   0 bruno      (502) admin       (80)     3289 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/model/gas/s1/s1_gas_inference_client.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.004917 scs-core-3.9.4/src/scs_core/model/gas/vB/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/vB/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2702 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/vB/gas_request.py
--rw-r--r--   0 bruno      (502) admin       (80)     3065 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/model/gas/vB/vb_gas_inference_client.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.005256 scs-core-3.9.4/src/scs_core/model/gas/vE/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/vE/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3535 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/vE/gas_request.py
--rw-r--r--   0 bruno      (502) admin       (80)     4507 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/model/gas/vE/ve_gas_inference_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     1218 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/gas/vcal_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     4812 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/model_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     2503 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/model_map.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.005692 scs-core-3.9.4/src/scs_core/model/pmx/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/pmx/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.006006 scs-core-3.9.4/src/scs_core/model/pmx/o2/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/pmx/o2/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4334 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/model/pmx/o2/o2_pmx_inference_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3778 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/pmx/o2/pmx_request.py
--rw-r--r--   0 bruno      (502) admin       (80)     1548 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/model/pmx/pmx_inference_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     1922 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/pmx/pmx_model_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)      602 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/pmx/pmx_request.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.006302 scs-core-3.9.4/src/scs_core/model/pmx/s1/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/model/pmx/s1/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2333 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/model/pmx/s1/pmx_request.py
--rw-r--r--   0 bruno      (502) admin       (80)     2348 2024-02-06 15:51:32.000000 scs-core-3.9.4/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.006774 scs-core-3.9.4/src/scs_core/monitor/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/monitor/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1558 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/monitor/monitor_error.py
--rw-r--r--   0 bruno      (502) admin       (80)     1557 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/monitor/monitor_request.py
--rw-r--r--   0 bruno      (502) admin       (80)     1395 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/monitor/monitor_response.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.008073 scs-core-3.9.4/src/scs_core/particulate/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/particulate/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     5054 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/particulate/opc_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     5142 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/particulate/opc_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3006 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/particulate/opc_error_log.py
--rw-r--r--   0 bruno      (502) admin       (80)     2610 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/particulate/opc_version.py
--rw-r--r--   0 bruno      (502) admin       (80)     2103 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/particulate/pmx_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     6405 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/particulate/sps_datum.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.008457 scs-core-3.9.4/src/scs_core/position/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4062 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/gps_datum.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.010151 scs-core-3.9.4/src/scs_core/position/nmea/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1578 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/gpdatetime.py
--rw-r--r--   0 bruno      (502) admin       (80)     4215 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/gpgga.py
--rw-r--r--   0 bruno      (502) admin       (80)     2685 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/gpgll.py
--rw-r--r--   0 bruno      (502) admin       (80)     3423 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/position/nmea/gpgsa.py
--rw-r--r--   0 bruno      (502) admin       (80)     3850 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/gpgsv.py
--rw-r--r--   0 bruno      (502) admin       (80)     2500 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/gploc.py
--rw-r--r--   0 bruno      (502) admin       (80)     4056 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/gprmc.py
--rw-r--r--   0 bruno      (502) admin       (80)     1318 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/gptime.py
--rw-r--r--   0 bruno      (502) admin       (80)     2685 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/gpvtg.py
--rw-r--r--   0 bruno      (502) admin       (80)     2535 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/nmea_report.py
--rw-r--r--   0 bruno      (502) admin       (80)      782 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/nmea/nmea_sentence.py
--rw-r--r--   0 bruno      (502) admin       (80)     3884 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/position/position.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.011137 scs-core-3.9.4/src/scs_core/psu/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/psu/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2320 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/psu/psu.py
--rw-r--r--   0 bruno      (502) admin       (80)     4543 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/psu/psu_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     1177 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/psu/psu_event_log.py
--rw-r--r--   0 bruno      (502) admin       (80)     1733 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/psu/psu_report.py
--rw-r--r--   0 bruno      (502) admin       (80)     1728 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/psu/psu_uptime.py
--rw-r--r--   0 bruno      (502) admin       (80)     5663 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/psu/psu_version.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.012403 scs-core-3.9.4/src/scs_core/sample/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sample/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     3421 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sample/climate_sample.py
--rw-r--r--   0 bruno      (502) admin       (80)    12016 2023-10-09 13:33:07.000000 scs-core-3.9.4/src/scs_core/sample/configuration_sample.py
--rw-r--r--   0 bruno      (502) admin       (80)     5262 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sample/gases_sample.py
--rw-r--r--   0 bruno      (502) admin       (80)     3724 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sample/particulates_sample.py
--rw-r--r--   0 bruno      (502) admin       (80)     2872 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sample/pressure_sample.py
--rw-r--r--   0 bruno      (502) admin       (80)     4034 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sample/sample.py
--rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-02 13:45:08.000000 scs-core-3.9.4/src/scs_core/sample/status_sample.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.012758 scs-core-3.9.4/src/scs_core/sampler/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sampler/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1263 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sampler/sampler.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.013606 scs-core-3.9.4/src/scs_core/sync/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sync/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2168 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sync/interval_timer.py
--rw-r--r--   0 bruno      (502) admin       (80)     1681 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sync/line_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)      606 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sync/runner.py
--rw-r--r--   0 bruno      (502) admin       (80)     6819 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sync/schedule.py
--rw-r--r--   0 bruno      (502) admin       (80)     1812 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/sync/synchronised_process.py
--rw-r--r--   0 bruno      (502) admin       (80)     1724 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sync/timed_runner.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.017863 scs-core-3.9.4/src/scs_core/sys/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     5061 2024-01-08 13:20:30.000000 scs-core-3.9.4/src/scs_core/sys/command.py
--rw-r--r--   0 bruno      (502) admin       (80)     4443 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/disk_usage.py
--rw-r--r--   0 bruno      (502) admin       (80)     5191 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/disk_volume.py
--rw-r--r--   0 bruno      (502) admin       (80)     2412 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/sys/eeprom_image.py
--rw-r--r--   0 bruno      (502) admin       (80)     2623 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/sys/exception_report.py
--rw-r--r--   0 bruno      (502) admin       (80)     6991 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/filesystem.py
--rw-r--r--   0 bruno      (502) admin       (80)     2371 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/sys/hostname.py
--rw-r--r--   0 bruno      (502) admin       (80)     1994 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/ipv4_address.py
--rw-r--r--   0 bruno      (502) admin       (80)     2733 2023-11-21 12:16:13.000000 scs-core-3.9.4/src/scs_core/sys/logging.py
--rw-r--r--   0 bruno      (502) admin       (80)     1297 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/memory.py
--rw-r--r--   0 bruno      (502) admin       (80)    17137 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/sys/modem.py
--rw-r--r--   0 bruno      (502) admin       (80)     5754 2023-10-17 10:39:03.000000 scs-core-3.9.4/src/scs_core/sys/network.py
--rw-r--r--   0 bruno      (502) admin       (80)     6984 2023-12-01 15:40:33.000000 scs-core-3.9.4/src/scs_core/sys/node.py
--rw-r--r--   0 bruno      (502) admin       (80)     3925 2024-01-31 08:47:30.000000 scs-core-3.9.4/src/scs_core/sys/persistence_manager.py
--rw-r--r--   0 bruno      (502) admin       (80)     1997 2024-01-15 12:16:33.000000 scs-core-3.9.4/src/scs_core/sys/platform.py
--rw-r--r--   0 bruno      (502) admin       (80)      834 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/process_comms.py
--rw-r--r--   0 bruno      (502) admin       (80)     4919 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/ps_datum.py
--rw-r--r--   0 bruno      (502) admin       (80)     3284 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/serial.py
--rw-r--r--   0 bruno      (502) admin       (80)     2405 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/shared_secret.py
--rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-11-23 09:21:51.000000 scs-core-3.9.4/src/scs_core/sys/signalled_exit.py
--rw-r--r--   0 bruno      (502) admin       (80)     2244 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/subprocess.py
--rw-r--r--   0 bruno      (502) admin       (80)     5882 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/system_id.py
--rw-r--r--   0 bruno      (502) admin       (80)     2013 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/system_temp.py
--rw-r--r--   0 bruno      (502) admin       (80)     6610 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/tail.py
--rw-r--r--   0 bruno      (502) admin       (80)     1409 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/timeout.py
--rw-r--r--   0 bruno      (502) admin       (80)     1192 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/timer.py
--rw-r--r--   0 bruno      (502) admin       (80)     1784 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/trace_entry.py
--rw-r--r--   0 bruno      (502) admin       (80)     5602 2023-09-11 10:21:38.000000 scs-core-3.9.4/src/scs_core/sys/uptime_datum.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-06 15:51:39.018039 scs-core-3.9.4/src/scs_core.egg-info/
--rw-r--r--   0 bruno      (502) admin       (80)     2303 2024-02-06 15:51:38.000000 scs-core-3.9.4/src/scs_core.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)    17620 2024-02-06 15:51:38.000000 scs-core-3.9.4/src/scs_core.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (502) admin       (80)        1 2024-02-06 15:51:38.000000 scs-core-3.9.4/src/scs_core.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (502) admin       (80)      124 2024-02-06 15:51:38.000000 scs-core-3.9.4/src/scs_core.egg-info/requires.txt
--rw-r--r--   0 bruno      (502) admin       (80)        9 2024-02-06 15:51:38.000000 scs-core-3.9.4/src/scs_core.egg-info/top_level.txt
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.774266 scs-core-3.9.5/
+-rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:38.000000 scs-core-3.9.5/LICENSE
+-rw-r--r--   0 bruno      (502) admin       (80)       77 2023-11-22 14:02:56.000000 scs-core-3.9.5/MANIFEST.in
+-rw-r--r--   0 bruno      (502) admin       (80)     2303 2024-02-20 11:09:43.774078 scs-core-3.9.5/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)     1404 2023-09-11 10:21:38.000000 scs-core-3.9.5/README.md
+-rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:38.000000 scs-core-3.9.5/README.rst
+-rw-r--r--   0 bruno      (502) admin       (80)      124 2023-09-11 10:21:38.000000 scs-core-3.9.5/requirements.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       38 2024-02-20 11:09:43.774301 scs-core-3.9.5/setup.cfg
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2258 2024-01-31 08:47:30.000000 scs-core-3.9.5/setup.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.702969 scs-core-3.9.5/src/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.709141 scs-core-3.9.5/src/scs_core/
+-rw-r--r--   0 bruno      (502) admin       (80)      183 2024-02-20 11:09:35.000000 scs-core-3.9.5/src/scs_core/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.710051 scs-core-3.9.5/src/scs_core/aqcsv/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.710435 scs-core-3.9.5/src/scs_core/aqcsv/conf/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/conf/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2617 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/conf/airnow_site_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1034 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.711434 scs-core-3.9.5/src/scs_core/aqcsv/connector/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/connector/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)    10215 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/connector/airnow_mapping_task.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.711594 scs-core-3.9.5/src/scs_core/aqcsv/connector/archive/
+-rw-r--r--   0 bruno      (502) admin       (80)      448 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/connector/archive/source_mappings.csv
+-rw-r--r--   0 bruno      (502) admin       (80)     6657 2024-01-08 13:20:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/connector/datum_mapping.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5042 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/connector/source_mapping.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.712296 scs-core-3.9.5/src/scs_core/aqcsv/data/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/data/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3764 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/data/aqcsv_datetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)    13736 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/data/aqcsv_record.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3046 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/data/aqcsv_site.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.714228 scs-core-3.9.5/src/scs_core/aqcsv/specification/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2837 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/agency.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.716490 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/
+-rw-r--r--   0 bruno      (502) admin       (80)    10261 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/agencies.csv
+-rw-r--r--   0 bruno      (502) admin       (80)     4728 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/countries.csv
+-rw-r--r--   0 bruno      (502) admin       (80)  1079325 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/methods.csv
+-rw-r--r--   0 bruno      (502) admin       (80)      768 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/mpcs.csv
+-rw-r--r--   0 bruno      (502) admin       (80)    28901 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/parameters.csv
+-rw-r--r--   0 bruno      (502) admin       (80)      149 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/qcs.csv
+-rw-r--r--   0 bruno      (502) admin       (80)     5420 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/qualifiers.csv
+-rw-r--r--   0 bruno      (502) admin       (80)     2484 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/units.csv
+-rw-r--r--   0 bruno      (502) admin       (80)     2742 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/country.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1163 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/country_iso.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1175 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/country_numeric.py
+-rw-r--r--   0 bruno      (502) admin       (80)     9813 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/method.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3778 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/mpc.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3466 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/parameter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2868 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/qc.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3745 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/qualifier.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2892 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aqcsv/specification/unit.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.716611 scs-core-3.9.5/src/scs_core/aws/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.718285 scs-core-3.9.5/src/scs_core/aws/client/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3585 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client/access_key.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2332 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client/api_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2960 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/client/api_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1576 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/client/api_intercourse.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1217 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client/client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5103 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client/client_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1264 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client/device_control_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3294 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client/email_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3361 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client/monitor_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7544 2023-11-09 16:14:47.000000 scs-core-3.9.5/src/scs_core/aws/client/mqtt_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4002 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/client/rest_client.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.718824 scs-core-3.9.5/src/scs_core/aws/client_traffic/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/client_traffic/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6793 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/client_traffic/client_traffic.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1475 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/client_traffic/client_traffic_finder.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4636 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/client_traffic/client_traffic_intercourse.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.719190 scs-core-3.9.5/src/scs_core/aws/config/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/config/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)      744 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/config/aws.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4471 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/config/project.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.719994 scs-core-3.9.5/src/scs_core/aws/data/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/data/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4998 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/data/dataset.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3550 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/data/deployment.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2956 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/data/http_response.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3175 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/data/message.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2884 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/data/upload_interval.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.720981 scs-core-3.9.5/src/scs_core/aws/greengrass/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1998 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/aws_deployer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3017 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/aws_deployment_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     9610 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/aws_group.py
+-rw-r--r--   0 bruno      (502) admin       (80)    16808 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/aws_group_configuration.py
+-rw-r--r--   0 bruno      (502) admin       (80)    11557 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/aws_identity.py
+-rw-r--r--   0 bruno      (502) admin       (80)      440 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/gg_errors.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.721113 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.721408 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/g0/
+-rw-r--r--   0 bruno      (502) admin       (80)     2259 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/g0/gg_functions.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1736 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/g0/gg_resources.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.722021 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/m0/
+-rw-r--r--   0 bruno      (502) admin       (80)     1245 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/m0/gg_functions.json
+-rw-r--r--   0 bruno      (502) admin       (80)      216 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/m0/gg_logger.json
+-rw-r--r--   0 bruno      (502) admin       (80)      485 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/m0/gg_resources.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1450 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/m0/gg_subscriptions.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.722319 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oE.1/
+-rw-r--r--   0 bruno      (502) admin       (80)     3781 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oE.1/gg_functions.json
+-rw-r--r--   0 bruno      (502) admin       (80)     2607 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oE.1/gg_resources.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.722651 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oP.2/
+-rw-r--r--   0 bruno      (502) admin       (80)     2259 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oP.2/gg_functions.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1607 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oP.2/gg_resources.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.722947 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oPG.2/
+-rw-r--r--   0 bruno      (502) admin       (80)     3781 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oPG.2/gg_functions.json
+-rw-r--r--   0 bruno      (502) admin       (80)     2478 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oPG.2/gg_resources.json
+-rw-r--r--   0 bruno      (502) admin       (80)      108 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/read.me
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.723250 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/uE.1/
+-rw-r--r--   0 bruno      (502) admin       (80)     4256 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/uE.1/gg_functions.json
+-rw-r--r--   0 bruno      (502) admin       (80)     3954 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/uE.1/gg_resources.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.723542 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/vB.1/
+-rw-r--r--   0 bruno      (502) admin       (80)     3781 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/vB.1/gg_functions.json
+-rw-r--r--   0 bruno      (502) admin       (80)     2652 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/greengrass/templates/vB.1/gg_resources.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.724568 scs-core-3.9.5/src/scs_core/aws/manager/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/manager/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.725678 scs-core-3.9.5/src/scs_core/aws/manager/byline/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/byline/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     9906 2023-12-13 16:10:25.000000 scs-core-3.9.5/src/scs_core/aws/manager/byline/byline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3872 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/byline/byline_finder.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2784 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/byline/byline_intercourse.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1792 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/byline/byline_list.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3726 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/byline/byline_manager.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.726665 scs-core-3.9.5/src/scs_core/aws/manager/configuration/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/configuration/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1351 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_check_finder.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6032 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_check_intercourse.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1251 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_check_requester.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2082 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_check_requester_intercourse.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1289 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_finder.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8803 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_intercourse.py
+-rw-r--r--   0 bruno      (502) admin       (80)    10200 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/dynamo_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3527 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/manager/ec2_message_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)    16782 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/aws/manager/lambda_message_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)    18063 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/aws/manager/s3_manager.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.727028 scs-core-3.9.5/src/scs_core/aws/manager/sagemaker/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/sagemaker/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4295 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/sagemaker/sagemaker_model_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7802 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/sagemaker/sagemaker_trial_manager.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.727390 scs-core-3.9.5/src/scs_core/aws/manager/topic_history/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/topic_history/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)    13260 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/aws/manager/topic_history/topic_history_intercourse.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2352 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/manager/topic_history/topic_history_manager.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.727508 scs-core-3.9.5/src/scs_core/aws/monitor/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.728270 scs-core-3.9.5/src/scs_core/aws/monitor/alert/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/alert/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)    18013 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5632 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert_specification_intercourse.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2682 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert_specification_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5830 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert_status_intercourse.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1425 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert_status_manager.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.729908 scs-core-3.9.5/src/scs_core/aws/monitor/device/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5348 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_email_list.py
+-rw-r--r--   0 bruno      (502) admin       (80)    18902 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8821 2023-11-22 11:44:01.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_specification.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2610 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_specification_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1207 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_status_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1776 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/power_list.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1795 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/status_list.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1792 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/monitor/device/uptime_list.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.733393 scs-core-3.9.5/src/scs_core/aws/security/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/security/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1157 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/security/access_key_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     9194 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_authentication.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5244 2023-11-21 12:16:13.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_client_credentials.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7852 2024-02-06 15:51:32.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_device.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1507 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_device_creator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2597 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_device_finder.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2111 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_device_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1506 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_login_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2600 2023-09-13 10:24:58.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_membership.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2280 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_password_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)    11923 2023-09-13 10:24:58.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_user.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2714 2023-09-25 13:43:59.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_user_finder.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3134 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/security/cognito_user_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2936 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/security/device_whitelist_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1947 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/security/opr_membership.py
+-rw-r--r--   0 bruno      (502) admin       (80)    23762 2023-12-13 16:10:25.000000 scs-core-3.9.5/src/scs_core/aws/security/organisation.py
+-rw-r--r--   0 bruno      (502) admin       (80)    11548 2024-02-20 11:09:35.000000 scs-core-3.9.5/src/scs_core/aws/security/organisation_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2397 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/aws/security/organisation_membership.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1752 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/aws/security/path_filter.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.734508 scs-core-3.9.5/src/scs_core/client/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/client/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4378 2023-11-09 16:14:47.000000 scs-core-3.9.5/src/scs_core/client/http_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7578 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/client/http_exception.py
+-rw-r--r--   0 bruno      (502) admin       (80)      497 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/client/http_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2831 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/client/network.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1415 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/client/resource_unavailable_exception.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2638 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/client/sftp_client_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.735625 scs-core-3.9.5/src/scs_core/climate/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1407 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/absolute_humidity.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1418 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/icp10101_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3081 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/mpl115a2_calib.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2911 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/mpl115a2_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2290 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/pressure_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2188 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/pressure_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3156 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/sht_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1844 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/climate/sht_datum.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.736345 scs-core-3.9.5/src/scs_core/comms/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/comms/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3125 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/comms/mqtt_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2395 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/comms/uds_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1552 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/comms/uds_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2350 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/comms/uds_server.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1614 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/comms/uds_writer.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.736966 scs-core-3.9.5/src/scs_core/control/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/control/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4918 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/control/command.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4897 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/control/control_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3792 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/control/control_handler.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4738 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/control/control_receipt.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.738814 scs-core-3.9.5/src/scs_core/csv/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/csv/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1979 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/csv/csv_archive.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6044 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/csv/csv_data_log.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7484 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/csv/csv_dict.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7017 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/csv/csv_log.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8640 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/csv/csv_log_cursor_queue.py
+-rw-r--r--   0 bruno      (502) admin       (80)     9032 2023-11-27 12:34:26.000000 scs-core-3.9.5/src/scs_core/csv/csv_log_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8361 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/csv/csv_logger.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4396 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/csv/csv_logger_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5273 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/csv/csv_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4498 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/csv/csv_writer.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.744233 scs-core-3.9.5/src/scs_core/data/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4903 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/data/aggregate.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2050 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/array_dict.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2415 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/average.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2158 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/categorical_regression.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8948 2023-11-21 12:16:13.000000 scs-core-3.9.5/src/scs_core/data/checkpoint_generator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1008 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/crc.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2092 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/crypt.py
+-rw-r--r--   0 bruno      (502) admin       (80)    20317 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/data/datetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6537 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/data/datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1510 2023-11-21 12:16:13.000000 scs-core-3.9.5/src/scs_core/data/differential.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6560 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/diurnal_period.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2634 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/duplicates.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3809 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/histogram.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1747 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/interval.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5951 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/join.py
+-rw-r--r--   0 bruno      (502) admin       (80)    14228 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/data/json.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3274 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/lin_regress.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5618 2024-02-20 11:09:35.000000 scs-core-3.9.5/src/scs_core/data/linear_regression.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1372 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/low_pass_filter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1628 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/median_filter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1892 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/min_list.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5682 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/model_delta.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8334 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/path_dict.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1904 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/period.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1291 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/precision.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3466 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/publication.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4181 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/queue_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)    10343 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/recurring_period.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1265 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/regression.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4348 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/rtc_datetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2249 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/sample_delta.py
+-rw-r--r--   0 bruno      (502) admin       (80)    10713 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/stats.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1280 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/str.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8129 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/data/timedelta.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2272 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/data/tokens.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7456 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/data/topic_path.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.744480 scs-core-3.9.5/src/scs_core/display/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/display/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3786 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/display/display_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.745072 scs-core-3.9.5/src/scs_core/email/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/email/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2717 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/email/email.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2132 2023-10-13 10:36:59.000000 scs-core-3.9.5/src/scs_core/email/email_queue.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2633 2023-11-21 12:16:13.000000 scs-core-3.9.5/src/scs_core/email/email_queue_manager.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.747178 scs-core-3.9.5/src/scs_core/estate/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/estate/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5502 2023-11-21 12:16:13.000000 scs-core-3.9.5/src/scs_core/estate/baseline_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)    30187 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/estate/configuration.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4521 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/estate/configuration_check.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5221 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/estate/git_pull.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3621 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/estate/git_pull_check.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6685 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/estate/mqtt_device_poller.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2445 2023-12-01 15:40:33.000000 scs-core-3.9.5/src/scs_core/estate/mqtt_peer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6718 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/estate/package_version.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2717 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/estate/software_version.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.747449 scs-core-3.9.5/src/scs_core/exegesis/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/exegesis/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.747807 scs-core-3.9.5/src/scs_core/exegesis/gas/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/exegesis/gas/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)      693 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/exegesis/gas/exegete_catalogue.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1345 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/exegesis/gas/exegete_collection.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.748376 scs-core-3.9.5/src/scs_core/exegesis/particulate/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/exegesis/particulate/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)      701 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/exegesis/particulate/exegete_catalogue.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1353 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/exegesis/particulate/exegete_collection.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2248 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/exegesis/particulate/text.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.749771 scs-core-3.9.5/src/scs_core/gas/
+-rw-r--r--   0 bruno      (502) admin       (80)      292 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.751045 scs-core-3.9.5/src/scs_core/gas/a4/
+-rw-r--r--   0 bruno      (502) admin       (80)      410 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3700 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4.py
+-rw-r--r--   0 bruno      (502) admin       (80)    10274 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4_calib.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5667 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4131 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3932 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5191 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5557 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4662 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6990 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/a4/a4_temp_comp.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.751529 scs-core-3.9.5/src/scs_core/gas/afe/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/afe/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1542 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/afe/afe_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3242 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/afe/pt1000_calib.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2445 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/afe/pt1000_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3600 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/afe_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)    11550 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/afe_calib.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6742 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/afe_id.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.751812 scs-core-3.9.5/src/scs_core/gas/d4/
+-rw-r--r--   0 bruno      (502) admin       (80)      130 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/d4/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3710 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/d4/d4_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3106 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/dsi_calib.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4352 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/gas/gas.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.752035 scs-core-3.9.5/src/scs_core/gas/isi/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/isi/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1373 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/isi/isi_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7370 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/gas/minimum.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.752766 scs-core-3.9.5/src/scs_core/gas/ndir/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/ndir/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1777 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/ndir/ndir.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2723 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/ndir/ndir_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3363 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/gas/ndir/ndir_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3649 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/ndir/ndir_version.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3078 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/gas/ndir/ndir_voltages.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.753791 scs-core-3.9.5/src/scs_core/gas/pid/
+-rw-r--r--   0 bruno      (502) admin       (80)      378 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/pid/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4498 2024-01-08 13:20:30.000000 scs-core-3.9.5/src/scs_core/gas/pid/pid.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7136 2024-01-08 13:20:30.000000 scs-core-3.9.5/src/scs_core/gas/pid/pid_calib.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4028 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/pid/pid_calibrated_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3837 2024-01-08 13:20:30.000000 scs-core-3.9.5/src/scs_core/gas/pid/pid_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3694 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/pid/pid_temp_comp.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.754402 scs-core-3.9.5/src/scs_core/gas/scd30/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/scd30/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2538 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/scd30/scd30_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2804 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/scd30/scd30_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2866 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/scd30/scd30_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3556 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/sensor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6167 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/gas/sensor_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3043 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gas/sensor_calib.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.754654 scs-core-3.9.5/src/scs_core/gps/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gps/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4077 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/gps/gps_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.754905 scs-core-3.9.5/src/scs_core/interface/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/interface/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2271 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/interface/interface_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.755289 scs-core-3.9.5/src/scs_core/led/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/led/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)      870 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/led/led.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2356 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/led/led_state.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.755830 scs-core-3.9.5/src/scs_core/location/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/location/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2992 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/location/timezone.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3708 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/location/timezone_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2379 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/location/timezone_offset.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.756250 scs-core-3.9.5/src/scs_core/model/
+-rw-r--r--   0 bruno      (502) admin       (80)      276 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.757156 scs-core-3.9.5/src/scs_core/model/catalogue/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.758110 scs-core-3.9.5/src/scs_core/model/catalogue/archive/
+-rw-r--r--   0 bruno      (502) admin       (80)     2027 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/archive/O3-vE-Urban-20H1.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1659 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-0p2ppm.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1660 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-0p5ppm.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1658 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-1ppm.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1651 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-50ppb.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1651 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3.json
+-rw-r--r--   0 bruno      (502) admin       (80)      188 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/archive/uE-1.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.758870 scs-core-3.9.5/src/scs_core/model/catalogue/compendia/
+-rw-r--r--   0 bruno      (502) admin       (80)     1663 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/compendia/NO-vE-Urban-20H1.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1640 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/compendia/NO2-vE-OPCube-21H1.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1643 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/compendia/NO2-vE-OPCube-21HA.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1662 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/compendia/NO2-vE-Urban-20HB.json
+-rw-r--r--   0 bruno      (502) admin       (80)     2029 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/compendia/O3-vE-Urban-20H1.json
+-rw-r--r--   0 bruno      (502) admin       (80)     1643 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/compendia/SO2-vE-Urban-22Q1.json
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.759278 scs-core-3.9.5/src/scs_core/model/catalogue/groups/
+-rw-r--r--   0 bruno      (502) admin       (80)       85 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/groups/oE-1.json
+-rw-r--r--   0 bruno      (502) admin       (80)      107 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/groups/read.me
+-rw-r--r--   0 bruno      (502) admin       (80)      154 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/groups/uE-1.json
+-rw-r--r--   0 bruno      (502) admin       (80)    11042 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/model_compendium.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4779 2023-11-21 12:16:13.000000 scs-core-3.9.5/src/scs_core/model/catalogue/model_compendium_group.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5220 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/term.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2038 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/catalogue/training_period.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.760161 scs-core-3.9.5/src/scs_core/model/gas/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3368 2023-11-21 12:16:13.000000 scs-core-3.9.5/src/scs_core/model/gas/baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1354 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/gas_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1545 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/gas_inference_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2873 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/gas/gas_model_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.760695 scs-core-3.9.5/src/scs_core/model/gas/s1/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/s1/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2704 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/s1/gas_request.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3289 2024-02-06 15:51:32.000000 scs-core-3.9.5/src/scs_core/model/gas/s1/s1_gas_inference_client.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.761012 scs-core-3.9.5/src/scs_core/model/gas/vB/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/vB/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2702 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/vB/gas_request.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3065 2024-02-06 15:51:32.000000 scs-core-3.9.5/src/scs_core/model/gas/vB/vb_gas_inference_client.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.761326 scs-core-3.9.5/src/scs_core/model/gas/vE/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/vE/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3535 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/vE/gas_request.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4507 2024-02-06 15:51:32.000000 scs-core-3.9.5/src/scs_core/model/gas/vE/ve_gas_inference_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1218 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/gas/vcal_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4812 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/model_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2503 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/model_map.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.761846 scs-core-3.9.5/src/scs_core/model/pmx/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/pmx/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.762257 scs-core-3.9.5/src/scs_core/model/pmx/o2/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/pmx/o2/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4334 2024-02-06 15:51:32.000000 scs-core-3.9.5/src/scs_core/model/pmx/o2/o2_pmx_inference_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3778 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/pmx/o2/pmx_request.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1548 2024-02-06 15:51:32.000000 scs-core-3.9.5/src/scs_core/model/pmx/pmx_inference_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1922 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/pmx/pmx_model_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)      602 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/pmx/pmx_request.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.762635 scs-core-3.9.5/src/scs_core/model/pmx/s1/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/model/pmx/s1/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2333 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/model/pmx/s1/pmx_request.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2348 2024-02-06 15:51:32.000000 scs-core-3.9.5/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.763128 scs-core-3.9.5/src/scs_core/monitor/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/monitor/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1558 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/monitor/monitor_error.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1557 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/monitor/monitor_request.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1395 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/monitor/monitor_response.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.764251 scs-core-3.9.5/src/scs_core/particulate/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/particulate/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5054 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/particulate/opc_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5142 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/particulate/opc_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3006 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/particulate/opc_error_log.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2610 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/particulate/opc_version.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2103 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/particulate/pmx_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6405 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/particulate/sps_datum.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.764634 scs-core-3.9.5/src/scs_core/position/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4062 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/gps_datum.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.766373 scs-core-3.9.5/src/scs_core/position/nmea/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1578 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/gpdatetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4215 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/gpgga.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2685 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/gpgll.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3423 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/position/nmea/gpgsa.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3850 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/gpgsv.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2500 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/gploc.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4056 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/gprmc.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1318 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/gptime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2685 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/gpvtg.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2535 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/nmea_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)      782 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/nmea/nmea_sentence.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3884 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/position/position.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.767350 scs-core-3.9.5/src/scs_core/psu/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/psu/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2320 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/psu/psu.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4543 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/psu/psu_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1177 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/psu/psu_event_log.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1733 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/psu/psu_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1728 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/psu/psu_uptime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5663 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/psu/psu_version.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.768580 scs-core-3.9.5/src/scs_core/sample/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sample/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3421 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sample/climate_sample.py
+-rw-r--r--   0 bruno      (502) admin       (80)    12016 2023-10-09 13:33:07.000000 scs-core-3.9.5/src/scs_core/sample/configuration_sample.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5262 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sample/gases_sample.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3724 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sample/particulates_sample.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2872 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sample/pressure_sample.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4034 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sample/sample.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-02 13:45:08.000000 scs-core-3.9.5/src/scs_core/sample/status_sample.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.768933 scs-core-3.9.5/src/scs_core/sampler/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sampler/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1263 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sampler/sampler.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.769745 scs-core-3.9.5/src/scs_core/sync/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sync/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2168 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sync/interval_timer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1681 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sync/line_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)      606 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sync/runner.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6819 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sync/schedule.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1812 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/sync/synchronised_process.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1724 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sync/timed_runner.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.773691 scs-core-3.9.5/src/scs_core/sys/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5061 2024-01-08 13:20:30.000000 scs-core-3.9.5/src/scs_core/sys/command.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4443 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/disk_usage.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5191 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/disk_volume.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2412 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/sys/eeprom_image.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2623 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/sys/exception_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6991 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/filesystem.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2371 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/sys/hostname.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1994 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/ipv4_address.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2733 2023-11-21 12:16:13.000000 scs-core-3.9.5/src/scs_core/sys/logging.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1297 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/memory.py
+-rw-r--r--   0 bruno      (502) admin       (80)    17137 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/sys/modem.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5754 2023-10-17 10:39:03.000000 scs-core-3.9.5/src/scs_core/sys/network.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6984 2023-12-01 15:40:33.000000 scs-core-3.9.5/src/scs_core/sys/node.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3925 2024-01-31 08:47:30.000000 scs-core-3.9.5/src/scs_core/sys/persistence_manager.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1997 2024-01-15 12:16:33.000000 scs-core-3.9.5/src/scs_core/sys/platform.py
+-rw-r--r--   0 bruno      (502) admin       (80)      834 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/process_comms.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4919 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/ps_datum.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3284 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/serial.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2405 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/shared_secret.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-11-23 09:21:51.000000 scs-core-3.9.5/src/scs_core/sys/signalled_exit.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2244 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/subprocess.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5882 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/system_id.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2013 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/system_temp.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6610 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/tail.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1409 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/timeout.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1192 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/timer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1784 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/trace_entry.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5602 2023-09-11 10:21:38.000000 scs-core-3.9.5/src/scs_core/sys/uptime_datum.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-02-20 11:09:43.773855 scs-core-3.9.5/src/scs_core.egg-info/
+-rw-r--r--   0 bruno      (502) admin       (80)     2303 2024-02-20 11:09:43.000000 scs-core-3.9.5/src/scs_core.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)    17620 2024-02-20 11:09:43.000000 scs-core-3.9.5/src/scs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2024-02-20 11:09:43.000000 scs-core-3.9.5/src/scs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (502) admin       (80)      124 2024-02-20 11:09:43.000000 scs-core-3.9.5/src/scs_core.egg-info/requires.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        9 2024-02-20 11:09:43.000000 scs-core-3.9.5/src/scs_core.egg-info/top_level.txt
```

### Comparing `scs-core-3.9.4/LICENSE` & `scs-core-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/PKG-INFO` & `scs-core-3.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-core
-Version: 3.9.4
+Version: 3.9.5
 Summary: The root of all South Coast Science environmental monitoring applications.
 Home-page: https://github.com/south-coast-science/scs_core
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-core-3.9.4/README.md` & `scs-core-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/setup.py` & `scs-core-3.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/conf/airnow_site_conf.py` & `scs-core-3.9.5/src/scs_core/aqcsv/conf/airnow_site_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/conf/airnow_uploader_conf.py` & `scs-core-3.9.5/src/scs_core/aqcsv/conf/airnow_uploader_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/connector/airnow_mapping_task.py` & `scs-core-3.9.5/src/scs_core/aqcsv/connector/airnow_mapping_task.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/connector/datum_mapping.py` & `scs-core-3.9.5/src/scs_core/aqcsv/connector/datum_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/connector/source_mapping.py` & `scs-core-3.9.5/src/scs_core/aqcsv/connector/source_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/data/aqcsv_datetime.py` & `scs-core-3.9.5/src/scs_core/aqcsv/data/aqcsv_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/data/aqcsv_record.py` & `scs-core-3.9.5/src/scs_core/aqcsv/data/aqcsv_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/data/aqcsv_site.py` & `scs-core-3.9.5/src/scs_core/aqcsv/data/aqcsv_site.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/agency.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/agency.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/agencies.csv` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/agencies.csv`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/countries.csv` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/countries.csv`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/methods.csv` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/methods.csv`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/mpcs.csv` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/mpcs.csv`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/parameters.csv` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/parameters.csv`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/qualifiers.csv` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/qualifiers.csv`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/archive/units.csv` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/archive/units.csv`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/country.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/country.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/country_iso.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/country_iso.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/country_numeric.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/country_numeric.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/method.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/method.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/mpc.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/mpc.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/parameter.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/parameter.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/qc.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/qc.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/qualifier.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/qualifier.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aqcsv/specification/unit.py` & `scs-core-3.9.5/src/scs_core/aqcsv/specification/unit.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/access_key.py` & `scs-core-3.9.5/src/scs_core/aws/client/access_key.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/api_auth.py` & `scs-core-3.9.5/src/scs_core/aws/client/api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/api_client.py` & `scs-core-3.9.5/src/scs_core/aws/client/api_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/api_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/client/api_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/client.py` & `scs-core-3.9.5/src/scs_core/aws/client/client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/client_auth.py` & `scs-core-3.9.5/src/scs_core/aws/client/client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/device_control_client.py` & `scs-core-3.9.5/src/scs_core/aws/client/device_control_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/email_client.py` & `scs-core-3.9.5/src/scs_core/aws/client/email_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/monitor_auth.py` & `scs-core-3.9.5/src/scs_core/aws/client/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/mqtt_client.py` & `scs-core-3.9.5/src/scs_core/aws/client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client/rest_client.py` & `scs-core-3.9.5/src/scs_core/aws/client/rest_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client_traffic/client_traffic.py` & `scs-core-3.9.5/src/scs_core/aws/client_traffic/client_traffic.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client_traffic/client_traffic_finder.py` & `scs-core-3.9.5/src/scs_core/aws/client_traffic/client_traffic_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/client_traffic/client_traffic_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/client_traffic/client_traffic_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/config/aws.py` & `scs-core-3.9.5/src/scs_core/aws/config/aws.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/config/project.py` & `scs-core-3.9.5/src/scs_core/aws/config/project.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/data/dataset.py` & `scs-core-3.9.5/src/scs_core/aws/data/dataset.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/data/deployment.py` & `scs-core-3.9.5/src/scs_core/aws/data/deployment.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/data/http_response.py` & `scs-core-3.9.5/src/scs_core/aws/data/http_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/data/message.py` & `scs-core-3.9.5/src/scs_core/aws/data/message.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/data/upload_interval.py` & `scs-core-3.9.5/src/scs_core/aws/data/upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/aws_deployer.py` & `scs-core-3.9.5/src/scs_core/aws/greengrass/aws_deployer.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/aws_deployment_reporter.py` & `scs-core-3.9.5/src/scs_core/aws/greengrass/aws_deployment_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/aws_group.py` & `scs-core-3.9.5/src/scs_core/aws/greengrass/aws_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/aws_group_configuration.py` & `scs-core-3.9.5/src/scs_core/aws/greengrass/aws_group_configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/aws_identity.py` & `scs-core-3.9.5/src/scs_core/aws/greengrass/aws_identity.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/g0/gg_functions.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/g0/gg_functions.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/g0/gg_resources.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/g0/gg_resources.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/m0/gg_functions.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/m0/gg_functions.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/m0/gg_subscriptions.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/m0/gg_subscriptions.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oE.1/gg_functions.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oE.1/gg_functions.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oE.1/gg_resources.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oE.1/gg_resources.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oP.2/gg_functions.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oP.2/gg_functions.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oP.2/gg_resources.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oP.2/gg_resources.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oPG.2/gg_functions.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oPG.2/gg_functions.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/oPG.2/gg_resources.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/oPG.2/gg_resources.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/uE.1/gg_functions.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/uE.1/gg_functions.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/uE.1/gg_resources.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/uE.1/gg_resources.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/vB.1/gg_functions.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/vB.1/gg_functions.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/greengrass/templates/vB.1/gg_resources.json` & `scs-core-3.9.5/src/scs_core/aws/greengrass/templates/vB.1/gg_resources.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/byline/byline.py` & `scs-core-3.9.5/src/scs_core/aws/manager/byline/byline.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/byline/byline_finder.py` & `scs-core-3.9.5/src/scs_core/aws/manager/byline/byline_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/byline/byline_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/manager/byline/byline_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/byline/byline_list.py` & `scs-core-3.9.5/src/scs_core/aws/manager/byline/byline_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/byline/byline_manager.py` & `scs-core-3.9.5/src/scs_core/aws/manager/byline/byline_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_check_finder.py` & `scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_check_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_check_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_check_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_check_requester.py` & `scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_check_requester.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_check_requester_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_check_requester_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_finder.py` & `scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/configuration/configuration_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/manager/configuration/configuration_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/dynamo_manager.py` & `scs-core-3.9.5/src/scs_core/aws/manager/dynamo_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/ec2_message_manager.py` & `scs-core-3.9.5/src/scs_core/aws/manager/ec2_message_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/lambda_message_manager.py` & `scs-core-3.9.5/src/scs_core/aws/manager/lambda_message_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/s3_manager.py` & `scs-core-3.9.5/src/scs_core/aws/manager/s3_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/sagemaker/sagemaker_model_manager.py` & `scs-core-3.9.5/src/scs_core/aws/manager/sagemaker/sagemaker_model_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/sagemaker/sagemaker_trial_manager.py` & `scs-core-3.9.5/src/scs_core/aws/manager/sagemaker/sagemaker_trial_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/topic_history/topic_history_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/manager/topic_history/topic_history_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/manager/topic_history/topic_history_manager.py` & `scs-core-3.9.5/src/scs_core/aws/manager/topic_history/topic_history_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert_specification_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert_specification_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert_specification_manager.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert_specification_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert_status_intercourse.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert_status_intercourse.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/alert/alert_status_manager.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/alert/alert_status_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_email_list.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_email_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_report.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_specification.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_specification.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_specification_manager.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_specification_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/device/device_monitor_status_manager.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/device/device_monitor_status_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/device/power_list.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/device/power_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/device/status_list.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/device/status_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/monitor/device/uptime_list.py` & `scs-core-3.9.5/src/scs_core/aws/monitor/device/uptime_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/access_key_manager.py` & `scs-core-3.9.5/src/scs_core/aws/security/access_key_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_authentication.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_authentication.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_client_credentials.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_client_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_device.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_device.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_device_creator.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_device_creator.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_device_finder.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_device_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_device_manager.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_device_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_login_manager.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_login_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_membership.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_password_manager.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_password_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_user.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_user.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_user_finder.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_user_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/cognito_user_manager.py` & `scs-core-3.9.5/src/scs_core/aws/security/cognito_user_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/device_whitelist_manager.py` & `scs-core-3.9.5/src/scs_core/aws/security/device_whitelist_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/opr_membership.py` & `scs-core-3.9.5/src/scs_core/aws/security/opr_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/organisation.py` & `scs-core-3.9.5/src/scs_core/aws/security/organisation.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/organisation_manager.py` & `scs-core-3.9.5/src/scs_core/aws/security/organisation_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,24 @@
 
         response = requests.get(url, headers=self._token_headers(token), data=payload)
         self._check_response(response)
 
         return tuple(Organisation.construct_from_jdict(jdict) for jdict in response.json())
 
 
+    def get_organisation(self, token, id):
+        url = '/'.join((self.__MANAGER_URL, 'organisation'))
+        payload = JSONify.dumps({"ID": id})
+
+        response = requests.get(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
+
+        return Organisation.construct_from_jdict(response.json())
+
+
     def get_organisation_by_label(self, token, label):
         url = '/'.join((self.__MANAGER_URL, 'organisation'))
         payload = JSONify.dumps({"Label": label})
 
         response = requests.get(url, headers=self._token_headers(token), data=payload)
         self._check_response(response)
```

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/organisation_membership.py` & `scs-core-3.9.5/src/scs_core/aws/security/organisation_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/aws/security/path_filter.py` & `scs-core-3.9.5/src/scs_core/aws/security/path_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/client/http_client.py` & `scs-core-3.9.5/src/scs_core/client/http_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/client/http_exception.py` & `scs-core-3.9.5/src/scs_core/client/http_exception.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/client/network.py` & `scs-core-3.9.5/src/scs_core/client/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/client/resource_unavailable_exception.py` & `scs-core-3.9.5/src/scs_core/client/resource_unavailable_exception.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/client/sftp_client_conf.py` & `scs-core-3.9.5/src/scs_core/client/sftp_client_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/climate/absolute_humidity.py` & `scs-core-3.9.5/src/scs_core/climate/absolute_humidity.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/climate/icp10101_datum.py` & `scs-core-3.9.5/src/scs_core/climate/icp10101_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/climate/mpl115a2_calib.py` & `scs-core-3.9.5/src/scs_core/climate/mpl115a2_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/climate/mpl115a2_datum.py` & `scs-core-3.9.5/src/scs_core/climate/mpl115a2_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/climate/pressure_conf.py` & `scs-core-3.9.5/src/scs_core/climate/pressure_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/climate/pressure_datum.py` & `scs-core-3.9.5/src/scs_core/climate/pressure_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/climate/sht_conf.py` & `scs-core-3.9.5/src/scs_core/climate/sht_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/climate/sht_datum.py` & `scs-core-3.9.5/src/scs_core/climate/sht_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/comms/mqtt_conf.py` & `scs-core-3.9.5/src/scs_core/comms/mqtt_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/comms/uds_client.py` & `scs-core-3.9.5/src/scs_core/comms/uds_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/comms/uds_reader.py` & `scs-core-3.9.5/src/scs_core/comms/uds_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/comms/uds_server.py` & `scs-core-3.9.5/src/scs_core/comms/uds_server.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/comms/uds_writer.py` & `scs-core-3.9.5/src/scs_core/comms/uds_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/control/command.py` & `scs-core-3.9.5/src/scs_core/control/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/control/control_datum.py` & `scs-core-3.9.5/src/scs_core/control/control_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/control/control_handler.py` & `scs-core-3.9.5/src/scs_core/control/control_handler.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/control/control_receipt.py` & `scs-core-3.9.5/src/scs_core/control/control_receipt.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_archive.py` & `scs-core-3.9.5/src/scs_core/csv/csv_archive.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_data_log.py` & `scs-core-3.9.5/src/scs_core/csv/csv_data_log.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_dict.py` & `scs-core-3.9.5/src/scs_core/csv/csv_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_log.py` & `scs-core-3.9.5/src/scs_core/csv/csv_log.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_log_cursor_queue.py` & `scs-core-3.9.5/src/scs_core/csv/csv_log_cursor_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_log_reader.py` & `scs-core-3.9.5/src/scs_core/csv/csv_log_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_logger.py` & `scs-core-3.9.5/src/scs_core/csv/csv_logger.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_logger_conf.py` & `scs-core-3.9.5/src/scs_core/csv/csv_logger_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_reader.py` & `scs-core-3.9.5/src/scs_core/csv/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/csv/csv_writer.py` & `scs-core-3.9.5/src/scs_core/csv/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/aggregate.py` & `scs-core-3.9.5/src/scs_core/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/array_dict.py` & `scs-core-3.9.5/src/scs_core/data/array_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/average.py` & `scs-core-3.9.5/src/scs_core/data/average.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/categorical_regression.py` & `scs-core-3.9.5/src/scs_core/data/categorical_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/checkpoint_generator.py` & `scs-core-3.9.5/src/scs_core/data/checkpoint_generator.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/crc.py` & `scs-core-3.9.5/src/scs_core/data/crc.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/crypt.py` & `scs-core-3.9.5/src/scs_core/data/crypt.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/datetime.py` & `scs-core-3.9.5/src/scs_core/data/datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/datum.py` & `scs-core-3.9.5/src/scs_core/data/datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/differential.py` & `scs-core-3.9.5/src/scs_core/data/differential.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/diurnal_period.py` & `scs-core-3.9.5/src/scs_core/data/diurnal_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/duplicates.py` & `scs-core-3.9.5/src/scs_core/data/duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/histogram.py` & `scs-core-3.9.5/src/scs_core/data/histogram.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/interval.py` & `scs-core-3.9.5/src/scs_core/data/interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/join.py` & `scs-core-3.9.5/src/scs_core/data/join.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/json.py` & `scs-core-3.9.5/src/scs_core/data/json.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/lin_regress.py` & `scs-core-3.9.5/src/scs_core/data/lin_regress.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/linear_regression.py` & `scs-core-3.9.5/src/scs_core/data/linear_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         try:
             value = float(min([y for _, y in self.__data]))
             return value if ndigits is None else round(value, ndigits)
 
         except TypeError:
             return None
 
+
     def mid(self, ndigits=None):
         # validation...
         if not self.has_midpoint():
             return None
 
         try:
             # single value...
```

### Comparing `scs-core-3.9.4/src/scs_core/data/low_pass_filter.py` & `scs-core-3.9.5/src/scs_core/data/low_pass_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/median_filter.py` & `scs-core-3.9.5/src/scs_core/data/median_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/min_list.py` & `scs-core-3.9.5/src/scs_core/data/min_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/model_delta.py` & `scs-core-3.9.5/src/scs_core/data/model_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/path_dict.py` & `scs-core-3.9.5/src/scs_core/data/path_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/period.py` & `scs-core-3.9.5/src/scs_core/data/period.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/precision.py` & `scs-core-3.9.5/src/scs_core/data/precision.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/publication.py` & `scs-core-3.9.5/src/scs_core/data/publication.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/queue_report.py` & `scs-core-3.9.5/src/scs_core/data/queue_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/recurring_period.py` & `scs-core-3.9.5/src/scs_core/data/recurring_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/regression.py` & `scs-core-3.9.5/src/scs_core/data/regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/rtc_datetime.py` & `scs-core-3.9.5/src/scs_core/data/rtc_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/sample_delta.py` & `scs-core-3.9.5/src/scs_core/data/sample_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/stats.py` & `scs-core-3.9.5/src/scs_core/data/stats.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/str.py` & `scs-core-3.9.5/src/scs_core/data/str.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/timedelta.py` & `scs-core-3.9.5/src/scs_core/data/timedelta.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/tokens.py` & `scs-core-3.9.5/src/scs_core/data/tokens.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/data/topic_path.py` & `scs-core-3.9.5/src/scs_core/data/topic_path.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/display/display_conf.py` & `scs-core-3.9.5/src/scs_core/display/display_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/email/email.py` & `scs-core-3.9.5/src/scs_core/email/email.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/email/email_queue.py` & `scs-core-3.9.5/src/scs_core/email/email_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/email/email_queue_manager.py` & `scs-core-3.9.5/src/scs_core/email/email_queue_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/baseline_conf.py` & `scs-core-3.9.5/src/scs_core/estate/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/configuration.py` & `scs-core-3.9.5/src/scs_core/estate/configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/configuration_check.py` & `scs-core-3.9.5/src/scs_core/estate/configuration_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/git_pull.py` & `scs-core-3.9.5/src/scs_core/estate/git_pull.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/git_pull_check.py` & `scs-core-3.9.5/src/scs_core/estate/git_pull_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/mqtt_device_poller.py` & `scs-core-3.9.5/src/scs_core/estate/mqtt_device_poller.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/mqtt_peer.py` & `scs-core-3.9.5/src/scs_core/estate/mqtt_peer.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/package_version.py` & `scs-core-3.9.5/src/scs_core/estate/package_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/estate/software_version.py` & `scs-core-3.9.5/src/scs_core/estate/software_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/exegesis/gas/exegete_catalogue.py` & `scs-core-3.9.5/src/scs_core/exegesis/gas/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/exegesis/gas/exegete_collection.py` & `scs-core-3.9.5/src/scs_core/exegesis/gas/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/exegesis/particulate/exegete_catalogue.py` & `scs-core-3.9.5/src/scs_core/exegesis/particulate/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/exegesis/particulate/exegete_collection.py` & `scs-core-3.9.5/src/scs_core/exegesis/particulate/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/exegesis/particulate/text.py` & `scs-core-3.9.5/src/scs_core/exegesis/particulate/text.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4_calib.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum_v1.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum_v1.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum_vA.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum_vA.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum_vB.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum_vB.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4_calibrated_datum_vC.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4_calibrated_datum_vC.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4_datum.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/a4/a4_temp_comp.py` & `scs-core-3.9.5/src/scs_core/gas/a4/a4_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/afe/afe_datum.py` & `scs-core-3.9.5/src/scs_core/gas/afe/afe_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/afe/pt1000_calib.py` & `scs-core-3.9.5/src/scs_core/gas/afe/pt1000_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/afe/pt1000_datum.py` & `scs-core-3.9.5/src/scs_core/gas/afe/pt1000_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/afe_baseline.py` & `scs-core-3.9.5/src/scs_core/gas/afe_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/afe_calib.py` & `scs-core-3.9.5/src/scs_core/gas/afe_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/afe_id.py` & `scs-core-3.9.5/src/scs_core/gas/afe_id.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/d4/d4_datum.py` & `scs-core-3.9.5/src/scs_core/gas/d4/d4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/dsi_calib.py` & `scs-core-3.9.5/src/scs_core/gas/dsi_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/gas.py` & `scs-core-3.9.5/src/scs_core/gas/gas.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/isi/isi_datum.py` & `scs-core-3.9.5/src/scs_core/gas/isi/isi_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/minimum.py` & `scs-core-3.9.5/src/scs_core/gas/minimum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/ndir/ndir.py` & `scs-core-3.9.5/src/scs_core/gas/ndir/ndir.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/ndir/ndir_conf.py` & `scs-core-3.9.5/src/scs_core/gas/ndir/ndir_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/ndir/ndir_datum.py` & `scs-core-3.9.5/src/scs_core/gas/ndir/ndir_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/ndir/ndir_version.py` & `scs-core-3.9.5/src/scs_core/gas/ndir/ndir_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/ndir/ndir_voltages.py` & `scs-core-3.9.5/src/scs_core/gas/ndir/ndir_voltages.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/pid/pid.py` & `scs-core-3.9.5/src/scs_core/gas/pid/pid.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/pid/pid_calib.py` & `scs-core-3.9.5/src/scs_core/gas/pid/pid_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/pid/pid_calibrated_datum.py` & `scs-core-3.9.5/src/scs_core/gas/pid/pid_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/pid/pid_datum.py` & `scs-core-3.9.5/src/scs_core/gas/pid/pid_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/pid/pid_temp_comp.py` & `scs-core-3.9.5/src/scs_core/gas/pid/pid_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/scd30/scd30_baseline.py` & `scs-core-3.9.5/src/scs_core/gas/scd30/scd30_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/scd30/scd30_conf.py` & `scs-core-3.9.5/src/scs_core/gas/scd30/scd30_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/scd30/scd30_datum.py` & `scs-core-3.9.5/src/scs_core/gas/scd30/scd30_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/sensor.py` & `scs-core-3.9.5/src/scs_core/gas/sensor.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/sensor_baseline.py` & `scs-core-3.9.5/src/scs_core/gas/sensor_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gas/sensor_calib.py` & `scs-core-3.9.5/src/scs_core/gas/sensor_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/gps/gps_conf.py` & `scs-core-3.9.5/src/scs_core/gps/gps_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/interface/interface_conf.py` & `scs-core-3.9.5/src/scs_core/interface/interface_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/led/led.py` & `scs-core-3.9.5/src/scs_core/led/led.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/led/led_state.py` & `scs-core-3.9.5/src/scs_core/led/led_state.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/location/timezone.py` & `scs-core-3.9.5/src/scs_core/location/timezone.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/location/timezone_conf.py` & `scs-core-3.9.5/src/scs_core/location/timezone_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/location/timezone_offset.py` & `scs-core-3.9.5/src/scs_core/location/timezone_offset.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/archive/O3-vE-Urban-20H1.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/archive/O3-vE-Urban-20H1.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-0p2ppm.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-0p2ppm.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-0p5ppm.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-0p5ppm.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-1ppm.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-1ppm.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-50ppb.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3-50ppb.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/archive/SO2-vE-Urban-21Q3.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/compendia/NO-vE-Urban-20H1.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/compendia/NO-vE-Urban-20H1.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/compendia/NO2-vE-OPCube-21H1.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/compendia/NO2-vE-OPCube-21H1.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/compendia/NO2-vE-OPCube-21HA.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/compendia/NO2-vE-OPCube-21HA.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/compendia/NO2-vE-Urban-20HB.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/compendia/NO2-vE-Urban-20HB.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/compendia/O3-vE-Urban-20H1.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/compendia/O3-vE-Urban-20H1.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/compendia/SO2-vE-Urban-22Q1.json` & `scs-core-3.9.5/src/scs_core/model/catalogue/compendia/SO2-vE-Urban-22Q1.json`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/model_compendium.py` & `scs-core-3.9.5/src/scs_core/model/catalogue/model_compendium.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/model_compendium_group.py` & `scs-core-3.9.5/src/scs_core/model/catalogue/model_compendium_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/term.py` & `scs-core-3.9.5/src/scs_core/model/catalogue/term.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/catalogue/training_period.py` & `scs-core-3.9.5/src/scs_core/model/catalogue/training_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/baseline.py` & `scs-core-3.9.5/src/scs_core/model/gas/baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/gas_baseline.py` & `scs-core-3.9.5/src/scs_core/model/gas/gas_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/gas_inference_client.py` & `scs-core-3.9.5/src/scs_core/model/gas/gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/gas_model_conf.py` & `scs-core-3.9.5/src/scs_core/model/gas/gas_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/s1/gas_request.py` & `scs-core-3.9.5/src/scs_core/model/gas/s1/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/s1/s1_gas_inference_client.py` & `scs-core-3.9.5/src/scs_core/model/gas/s1/s1_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/vB/gas_request.py` & `scs-core-3.9.5/src/scs_core/model/gas/vB/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/vB/vb_gas_inference_client.py` & `scs-core-3.9.5/src/scs_core/model/gas/vB/vb_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/vE/gas_request.py` & `scs-core-3.9.5/src/scs_core/model/gas/vE/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/vE/ve_gas_inference_client.py` & `scs-core-3.9.5/src/scs_core/model/gas/vE/ve_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/gas/vcal_baseline.py` & `scs-core-3.9.5/src/scs_core/model/gas/vcal_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/model_conf.py` & `scs-core-3.9.5/src/scs_core/model/model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/model_map.py` & `scs-core-3.9.5/src/scs_core/model/model_map.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/pmx/o2/o2_pmx_inference_client.py` & `scs-core-3.9.5/src/scs_core/model/pmx/o2/o2_pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/pmx/o2/pmx_request.py` & `scs-core-3.9.5/src/scs_core/model/pmx/o2/pmx_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/pmx/pmx_inference_client.py` & `scs-core-3.9.5/src/scs_core/model/pmx/pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/pmx/pmx_model_conf.py` & `scs-core-3.9.5/src/scs_core/model/pmx/pmx_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/pmx/pmx_request.py` & `scs-core-3.9.5/src/scs_core/model/pmx/pmx_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/pmx/s1/pmx_request.py` & `scs-core-3.9.5/src/scs_core/model/pmx/s1/pmx_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py` & `scs-core-3.9.5/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/monitor/monitor_error.py` & `scs-core-3.9.5/src/scs_core/monitor/monitor_error.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/monitor/monitor_request.py` & `scs-core-3.9.5/src/scs_core/monitor/monitor_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/monitor/monitor_response.py` & `scs-core-3.9.5/src/scs_core/monitor/monitor_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/particulate/opc_conf.py` & `scs-core-3.9.5/src/scs_core/particulate/opc_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/particulate/opc_datum.py` & `scs-core-3.9.5/src/scs_core/particulate/opc_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/particulate/opc_error_log.py` & `scs-core-3.9.5/src/scs_core/particulate/opc_error_log.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/particulate/opc_version.py` & `scs-core-3.9.5/src/scs_core/particulate/opc_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/particulate/pmx_datum.py` & `scs-core-3.9.5/src/scs_core/particulate/pmx_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/particulate/sps_datum.py` & `scs-core-3.9.5/src/scs_core/particulate/sps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/gps_datum.py` & `scs-core-3.9.5/src/scs_core/position/gps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gpdatetime.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gpdatetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gpgga.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gpgga.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gpgll.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gpgll.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gpgsa.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gpgsa.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gpgsv.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gpgsv.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gploc.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gploc.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gprmc.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gprmc.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gptime.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gptime.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/gpvtg.py` & `scs-core-3.9.5/src/scs_core/position/nmea/gpvtg.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/nmea_report.py` & `scs-core-3.9.5/src/scs_core/position/nmea/nmea_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/nmea/nmea_sentence.py` & `scs-core-3.9.5/src/scs_core/position/nmea/nmea_sentence.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/position/position.py` & `scs-core-3.9.5/src/scs_core/position/position.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/psu/psu.py` & `scs-core-3.9.5/src/scs_core/psu/psu.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/psu/psu_conf.py` & `scs-core-3.9.5/src/scs_core/psu/psu_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/psu/psu_event_log.py` & `scs-core-3.9.5/src/scs_core/psu/psu_event_log.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/psu/psu_report.py` & `scs-core-3.9.5/src/scs_core/psu/psu_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/psu/psu_uptime.py` & `scs-core-3.9.5/src/scs_core/psu/psu_uptime.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/psu/psu_version.py` & `scs-core-3.9.5/src/scs_core/psu/psu_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sample/climate_sample.py` & `scs-core-3.9.5/src/scs_core/sample/climate_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sample/configuration_sample.py` & `scs-core-3.9.5/src/scs_core/sample/configuration_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sample/gases_sample.py` & `scs-core-3.9.5/src/scs_core/sample/gases_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sample/particulates_sample.py` & `scs-core-3.9.5/src/scs_core/sample/particulates_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sample/pressure_sample.py` & `scs-core-3.9.5/src/scs_core/sample/pressure_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sample/sample.py` & `scs-core-3.9.5/src/scs_core/sample/sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sample/status_sample.py` & `scs-core-3.9.5/src/scs_core/sample/status_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sampler/sampler.py` & `scs-core-3.9.5/src/scs_core/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sync/interval_timer.py` & `scs-core-3.9.5/src/scs_core/sync/interval_timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sync/line_reader.py` & `scs-core-3.9.5/src/scs_core/sync/line_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sync/runner.py` & `scs-core-3.9.5/src/scs_core/sync/runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sync/schedule.py` & `scs-core-3.9.5/src/scs_core/sync/schedule.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sync/synchronised_process.py` & `scs-core-3.9.5/src/scs_core/sync/synchronised_process.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sync/timed_runner.py` & `scs-core-3.9.5/src/scs_core/sync/timed_runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/command.py` & `scs-core-3.9.5/src/scs_core/sys/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/disk_usage.py` & `scs-core-3.9.5/src/scs_core/sys/disk_usage.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/disk_volume.py` & `scs-core-3.9.5/src/scs_core/sys/disk_volume.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/eeprom_image.py` & `scs-core-3.9.5/src/scs_core/sys/eeprom_image.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/exception_report.py` & `scs-core-3.9.5/src/scs_core/sys/exception_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/filesystem.py` & `scs-core-3.9.5/src/scs_core/sys/filesystem.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/hostname.py` & `scs-core-3.9.5/src/scs_core/sys/hostname.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/ipv4_address.py` & `scs-core-3.9.5/src/scs_core/sys/ipv4_address.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/logging.py` & `scs-core-3.9.5/src/scs_core/sys/logging.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/memory.py` & `scs-core-3.9.5/src/scs_core/sys/memory.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/modem.py` & `scs-core-3.9.5/src/scs_core/sys/modem.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/network.py` & `scs-core-3.9.5/src/scs_core/sys/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/node.py` & `scs-core-3.9.5/src/scs_core/sys/node.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/persistence_manager.py` & `scs-core-3.9.5/src/scs_core/sys/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/platform.py` & `scs-core-3.9.5/src/scs_core/sys/platform.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/process_comms.py` & `scs-core-3.9.5/src/scs_core/sys/process_comms.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/ps_datum.py` & `scs-core-3.9.5/src/scs_core/sys/ps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/serial.py` & `scs-core-3.9.5/src/scs_core/sys/serial.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/shared_secret.py` & `scs-core-3.9.5/src/scs_core/sys/shared_secret.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/signalled_exit.py` & `scs-core-3.9.5/src/scs_core/sys/signalled_exit.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/subprocess.py` & `scs-core-3.9.5/src/scs_core/sys/subprocess.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/system_id.py` & `scs-core-3.9.5/src/scs_core/sys/system_id.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/system_temp.py` & `scs-core-3.9.5/src/scs_core/sys/system_temp.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/tail.py` & `scs-core-3.9.5/src/scs_core/sys/tail.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/timeout.py` & `scs-core-3.9.5/src/scs_core/sys/timeout.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/timer.py` & `scs-core-3.9.5/src/scs_core/sys/timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/trace_entry.py` & `scs-core-3.9.5/src/scs_core/sys/trace_entry.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core/sys/uptime_datum.py` & `scs-core-3.9.5/src/scs_core/sys/uptime_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-3.9.4/src/scs_core.egg-info/PKG-INFO` & `scs-core-3.9.5/src/scs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-core
-Version: 3.9.4
+Version: 3.9.5
 Summary: The root of all South Coast Science environmental monitoring applications.
 Home-page: https://github.com/south-coast-science/scs_core
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-core-3.9.4/src/scs_core.egg-info/SOURCES.txt` & `scs-core-3.9.5/src/scs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

