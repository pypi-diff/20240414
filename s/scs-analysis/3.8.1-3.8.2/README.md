# Comparing `tmp/scs-analysis-3.8.1.tar.gz` & `tmp/scs_analysis-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-analysis-3.8.1.tar", last modified: Tue Apr  9 15:18:16 2024, max compression
+gzip compressed data, was "scs_analysis-3.8.2.tar", last modified: Sun Apr 14 07:50:20 2024, max compression
```

## Comparing `scs-analysis-3.8.1.tar` & `scs_analysis-3.8.2.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:18:16.105733 scs-analysis-3.8.1/
--rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/LICENSE
--rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs-analysis-3.8.1/MANIFEST.in
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-09 15:18:16.105548 scs-analysis-3.8.1/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/README.md
--rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/README.rst
--rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-09 15:14:30.000000 scs-analysis-3.8.1/requirements.txt
--rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-09 15:18:16.105769 scs-analysis-3.8.1/setup.cfg
--rwxr-xr-x   0 bruno      (502) admin       (80)     5581 2024-04-09 15:18:11.000000 scs-analysis-3.8.1/setup.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:18:16.077936 scs-analysis-3.8.1/src/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:18:16.091975 scs-analysis-3.8.1/src/scs_analysis/
--rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-04-09 15:18:11.000000 scs-analysis-3.8.1/src/scs_analysis/__init__.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs-analysis-3.8.1/src/scs_analysis/alert.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs-analysis-3.8.1/src/scs_analysis/alert_status.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6000 2024-04-09 15:14:30.000000 scs-analysis-3.8.1/src/scs_analysis/aws_byline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs-analysis-3.8.1/src/scs_analysis/aws_client_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/aws_mqtt_client.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7094 2024-04-09 15:14:30.000000 scs-analysis-3.8.1/src/scs_analysis/aws_topic_history.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3339 2024-04-09 15:14:30.000000 scs-analysis-3.8.1/src/scs_analysis/aws_topic_origin.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/aws_topic_publisher.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/aws_upload_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)    14774 2024-04-09 15:14:30.000000 scs-analysis-3.8.1/src/scs_analysis/baseline.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs-analysis-3.8.1/src/scs_analysis/baseline_conf.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:18:16.093433 scs-analysis-3.8.1/src/scs_analysis/chart/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/chart/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/chart/chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/chart/histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/chart/multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/chart/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6514 2024-03-13 09:22:10.000000 scs-analysis-3.8.1/src/scs_analysis/client_traffic.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:18:16.103744 scs-analysis-3.8.1/src/scs_analysis/cmd/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_alert.py
--rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_alert_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-r--r--   0 bruno      (502) admin       (80)     2478 2024-04-09 15:14:30.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_topic_origin.py
--rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_baseline.py
--rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-r--r--   0 bruno      (502) admin       (80)     4868 2024-03-13 09:22:10.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_client_traffic.py
--rw-r--r--   0 bruno      (502) admin       (80)     4739 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_email.py
--rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-r--r--   0 bruno      (502) admin       (80)     4798 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     4518 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-r--r--   0 bruno      (502) admin       (80)     2372 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_configuration_report.py
--rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_join.py
--rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-r--r--   0 bruno      (502) admin       (80)     3987 2023-11-21 12:15:43.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_device_controller.py
--rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_device_monitor.py
--rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_device_monitor_status.py
--rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3123 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_node.py
--rw-r--r--   0 bruno      (502) admin       (80)     5422 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-r--r--   0 bruno      (502) admin       (80)     4597 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-r--r--   0 bruno      (502) admin       (80)     4703 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-r--r--   0 bruno      (502) admin       (80)     6207 2024-02-20 11:09:07.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisations.py
--rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_error.py
--rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
--rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_gas_density.py
--rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_localize.py
--rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_median.py
--rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_record.py
--rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_single_chart.py
--rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_uds.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5450 2024-04-03 10:23:16.000000 scs-analysis-3.8.1/src/scs_analysis/cognito_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6576 2023-12-05 08:54:35.000000 scs-analysis-3.8.1/src/scs_analysis/cognito_email.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs-analysis-3.8.1/src/scs_analysis/cognito_user_credentials.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8085 2024-01-08 13:19:59.000000 scs-analysis-3.8.1/src/scs_analysis/cognito_user_identity.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8359 2023-12-05 08:54:35.000000 scs-analysis-3.8.1/src/scs_analysis/cognito_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7663 2023-12-05 08:54:35.000000 scs-analysis-3.8.1/src/scs_analysis/configuration_csv.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3558 2023-12-05 08:54:35.000000 scs-analysis-3.8.1/src/scs_analysis/configuration_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3947 2023-12-05 08:54:35.000000 scs-analysis-3.8.1/src/scs_analysis/configuration_monitor_check.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4001 2023-12-01 15:39:55.000000 scs-analysis-3.8.1/src/scs_analysis/configuration_report.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/csv_collation_summary.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/csv_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/csv_join.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/csv_reader.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/csv_segmentor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs-analysis-3.8.1/src/scs_analysis/csv_writer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7380 2024-04-08 08:21:13.000000 scs-analysis-3.8.1/src/scs_analysis/device_controller.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5337 2023-12-13 16:09:42.000000 scs-analysis-3.8.1/src/scs_analysis/device_monitor.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs-analysis-3.8.1/src/scs_analysis/device_monitor_status.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:18:16.105047 scs-analysis-3.8.1/src/scs_analysis/handler/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/batch_download_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/configuration_csv_generator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5557 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/csv_collator.py
--rw-r--r--   0 bruno      (502) admin       (80)     5893 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/csv_segmentor.py
--rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/mqtt_reporter.py
--rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/sample_midpoint.py
--rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/handler/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/histo_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2127 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/localised_datetime.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/monitor_auth.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/multi_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs-analysis-3.8.1/src/scs_analysis/node.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6041 2024-01-08 13:19:59.000000 scs-analysis-3.8.1/src/scs_analysis/organisation_devices.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4778 2024-01-08 13:19:59.000000 scs-analysis-3.8.1/src/scs_analysis/organisation_path_roots.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4982 2024-01-08 13:19:59.000000 scs-analysis-3.8.1/src/scs_analysis/organisation_user_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5871 2024-01-08 13:19:59.000000 scs-analysis-3.8.1/src/scs_analysis/organisation_users.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7389 2024-02-20 11:09:07.000000 scs-analysis-3.8.1/src/scs_analysis/organisations.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs-analysis-3.8.1/src/scs_analysis/sample_aggregate.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_average.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_collator.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_distance.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_duplicates.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_error.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_gas_concentration.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3561 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_gas_density.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/sample_interval.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs-analysis-3.8.1/src/scs_analysis/sample_iso_8601.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_localize.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_low_pass.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_max.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_median.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_midpoint.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_min.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/sample_noise.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_nullify.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/sample_paths.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_regression.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs-analysis-3.8.1/src/scs_analysis/sample_slope.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_sort.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_stats.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs-analysis-3.8.1/src/scs_analysis/sample_subset.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/sample_time_shift.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/single_chart.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs-analysis-3.8.1/src/scs_analysis/socket_receiver.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs-analysis-3.8.1/src/scs_analysis/timer.py
--rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs-analysis-3.8.1/src/scs_analysis/uds_receiver.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-09 15:18:16.105225 scs-analysis-3.8.1/src/scs_analysis.egg-info/
--rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-09 15:18:16.000000 scs-analysis-3.8.1/src/scs_analysis.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-04-09 15:18:16.000000 scs-analysis-3.8.1/src/scs_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-09 15:18:16.000000 scs-analysis-3.8.1/src/scs_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (502) admin       (80)      252 2024-04-09 15:18:16.000000 scs-analysis-3.8.1/src/scs_analysis.egg-info/requires.txt
--rw-r--r--   0 bruno      (502) admin       (80)       13 2024-04-09 15:18:16.000000 scs-analysis-3.8.1/src/scs_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:50:20.750470 scs_analysis-3.8.2/
+-rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/LICENSE
+-rw-r--r--   0 bruno      (502) admin       (80)       82 2023-11-22 14:04:33.000000 scs_analysis-3.8.2/MANIFEST.in
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-14 07:50:20.750250 scs_analysis-3.8.2/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)      766 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/README.md
+-rw-r--r--   0 bruno      (502) admin       (80)       41 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/README.rst
+-rw-r--r--   0 bruno      (502) admin       (80)      237 2024-04-09 15:14:30.000000 scs_analysis-3.8.2/requirements.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-14 07:50:20.750506 scs_analysis-3.8.2/setup.cfg
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5581 2024-04-09 15:18:11.000000 scs_analysis-3.8.2/setup.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:50:20.720121 scs_analysis-3.8.2/src/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:50:20.735172 scs_analysis-3.8.2/src/scs_analysis/
+-rwxr-xr-x   0 bruno      (502) admin       (80)      241 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/__init__.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    11522 2024-03-11 10:08:11.000000 scs_analysis-3.8.2/src/scs_analysis/alert.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4218 2024-03-26 13:54:32.000000 scs_analysis-3.8.2/src/scs_analysis/alert_status.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5981 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/aws_byline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2635 2023-10-09 13:33:35.000000 scs_analysis-3.8.2/src/scs_analysis/aws_client_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7224 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/aws_mqtt_client.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7103 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/aws_topic_history.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4190 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/aws_topic_origin.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2218 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/aws_topic_publisher.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2918 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/aws_upload_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)    14779 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/baseline.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6848 2023-11-21 12:15:43.000000 scs_analysis-3.8.2/src/scs_analysis/baseline_conf.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:50:20.736699 scs_analysis-3.8.2/src/scs_analysis/chart/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/chart/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1630 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/chart/chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4546 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/chart/histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4249 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/chart/multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4317 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/chart/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6514 2024-03-13 09:22:10.000000 scs_analysis-3.8.2/src/scs_analysis/client_traffic.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:50:20.747176 scs_analysis-3.8.2/src/scs_analysis/cmd/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)    12610 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_alert.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5235 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6289 2024-03-26 13:54:32.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3185 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     8443 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3875 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_topic_origin.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1755 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7397 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_baseline.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6485 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4868 2024-03-13 09:22:10.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_client_traffic.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4739 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3103 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_email.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3656 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3256 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-r--r--   0 bruno      (502) admin       (80)     7099 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5470 2023-10-09 13:33:35.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4798 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4518 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2372 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_configuration_report.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3328 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2856 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3494 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2813 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2808 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3399 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3987 2023-11-21 12:15:43.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6626 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_device_monitor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3340 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_device_monitor_status.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4078 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3123 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2089 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5637 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3409 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3500 2024-01-15 12:16:08.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_node.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5422 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4597 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4703 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6495 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-r--r--   0 bruno      (502) admin       (80)     6207 2024-02-20 11:09:07.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisations.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3661 2024-01-16 11:21:37.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3584 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2847 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2313 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3035 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1940 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2688 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_gas_concentration.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1952 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_gas_density.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1951 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5239 2023-09-26 10:57:10.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2536 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_localize.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2645 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2422 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2844 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1472 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1609 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3899 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1610 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3109 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5210 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2370 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2673 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3729 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1770 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1570 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_uds.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5450 2024-04-03 10:23:16.000000 scs_analysis-3.8.2/src/scs_analysis/cognito_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6576 2023-12-05 08:54:35.000000 scs_analysis-3.8.2/src/scs_analysis/cognito_email.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5373 2024-01-31 08:47:01.000000 scs_analysis-3.8.2/src/scs_analysis/cognito_user_credentials.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8085 2024-01-08 13:19:59.000000 scs_analysis-3.8.2/src/scs_analysis/cognito_user_identity.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8359 2023-12-05 08:54:35.000000 scs_analysis-3.8.2/src/scs_analysis/cognito_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7628 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/configuration_csv.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3546 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/configuration_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3947 2023-12-05 08:54:35.000000 scs_analysis-3.8.2/src/scs_analysis/configuration_monitor_check.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4001 2023-12-01 15:39:55.000000 scs_analysis-3.8.2/src/scs_analysis/configuration_report.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6401 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/csv_collation_summary.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3967 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/csv_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6835 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/csv_join.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5065 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/csv_reader.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4697 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/csv_segmentor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3863 2023-11-27 12:33:51.000000 scs_analysis-3.8.2/src/scs_analysis/csv_writer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7380 2024-04-08 08:21:13.000000 scs_analysis-3.8.2/src/scs_analysis/device_controller.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5337 2023-12-13 16:09:42.000000 scs_analysis-3.8.2/src/scs_analysis/device_monitor.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4521 2023-12-05 08:54:35.000000 scs_analysis-3.8.2/src/scs_analysis/device_monitor_status.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:50:20.748410 scs_analysis-3.8.2/src/scs_analysis/handler/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4051 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2329 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2360 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/handler/batch_download_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1436 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5557 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/csv_collator.py
+-rw-r--r--   0 bruno      (502) admin       (80)     5893 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/csv_segmentor.py
+-rw-r--r--   0 bruno      (502) admin       (80)     1184 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/mqtt_reporter.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2007 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/sample_midpoint.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2151 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/handler/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4308 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/histo_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2127 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/localised_datetime.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2544 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/monitor_auth.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4367 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/multi_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5962 2024-01-31 08:47:01.000000 scs_analysis-3.8.2/src/scs_analysis/node.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6041 2024-01-08 13:19:59.000000 scs_analysis-3.8.2/src/scs_analysis/organisation_devices.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4778 2024-01-08 13:19:59.000000 scs_analysis-3.8.2/src/scs_analysis/organisation_path_roots.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4982 2024-01-08 13:19:59.000000 scs_analysis-3.8.2/src/scs_analysis/organisation_user_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5871 2024-01-08 13:19:59.000000 scs_analysis-3.8.2/src/scs_analysis/organisation_users.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7389 2024-02-20 11:09:07.000000 scs_analysis-3.8.2/src/scs_analysis/organisations.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     7807 2024-01-17 09:58:13.000000 scs_analysis-3.8.2/src/scs_analysis/sample_aggregate.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4821 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_average.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5162 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_collator.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3970 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_distance.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3765 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_duplicates.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4685 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_error.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5606 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_gas_concentration.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3522 2024-04-14 07:50:13.000000 scs_analysis-3.8.2/src/scs_analysis/sample_gas_density.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3181 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/sample_interval.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     8224 2023-09-26 10:57:10.000000 scs_analysis-3.8.2/src/scs_analysis/sample_iso_8601.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4792 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_localize.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3802 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_low_pass.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3571 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_max.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3776 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_median.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3529 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_midpoint.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3570 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_min.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5151 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/sample_noise.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4017 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_nullify.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1746 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/sample_paths.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     3320 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_regression.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5661 2024-02-06 15:51:04.000000 scs_analysis-3.8.2/src/scs_analysis/sample_slope.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2502 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_sort.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     5928 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_stats.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     6155 2024-01-08 13:19:59.000000 scs_analysis-3.8.2/src/scs_analysis/sample_subset.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2965 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/sample_time_shift.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     4463 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/single_chart.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2530 2023-11-09 16:15:38.000000 scs_analysis-3.8.2/src/scs_analysis/socket_receiver.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1942 2023-10-09 13:33:35.000000 scs_analysis-3.8.2/src/scs_analysis/timer.py
+-rwxr-xr-x   0 bruno      (502) admin       (80)     1849 2023-09-11 10:21:50.000000 scs_analysis-3.8.2/src/scs_analysis/uds_receiver.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-14 07:50:20.748597 scs_analysis-3.8.2/src/scs_analysis.egg-info/
+-rw-r--r--   0 bruno      (502) admin       (80)     1960 2024-04-14 07:50:20.000000 scs_analysis-3.8.2/src/scs_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)     6234 2024-04-14 07:50:20.000000 scs_analysis-3.8.2/src/scs_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-14 07:50:20.000000 scs_analysis-3.8.2/src/scs_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (502) admin       (80)      252 2024-04-14 07:50:20.000000 scs_analysis-3.8.2/src/scs_analysis.egg-info/requires.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       13 2024-04-14 07:50:20.000000 scs_analysis-3.8.2/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs-analysis-3.8.1/LICENSE` & `scs_analysis-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/PKG-INFO` & `scs_analysis-3.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.8.1
+Version: 3.8.2
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-3.8.1/README.md` & `scs_analysis-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/setup.py` & `scs_analysis-3.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/alert.py` & `scs_analysis-3.8.2/src/scs_analysis/alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/alert_status.py` & `scs_analysis-3.8.2/src/scs_analysis/alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/aws_byline.py` & `scs_analysis-3.8.2/src/scs_analysis/aws_byline.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,15 @@
             logger.error("login: %s." % auth.authentication_status.description)
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        reporter = BatchDownloadReporter()
-        finder = BylineFinder(reporter=reporter)
+        finder = BylineFinder(reporter=BatchDownloadReporter('bylines'))
 
         manager = BylineManager()
 
 
         # ------------------------------------------------------------------------------------------------------------
         # check...
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/aws_client_auth.py` & `scs_analysis-3.8.2/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/aws_mqtt_client.py` & `scs_analysis-3.8.2/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/aws_topic_history.py` & `scs_analysis-3.8.2/src/scs_analysis/aws_topic_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         # BylineFinder...
         byline_finder = BylineFinder()
 
         # MessageManager...
-        reporter = BatchDownloadReporter()
+        reporter = BatchDownloadReporter('history')
         finder = TopicHistoryFinder(reporter=reporter)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # check...
 
         if not Network.is_available():
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/aws_topic_origin.py` & `scs_analysis-3.8.2/src/scs_analysis/aws_topic_origin.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,36 +4,41 @@
 Created on 9 Apr 2024
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The aws_topic_origin utility is used to discover the datetime of the earliest recorded publication on the given topic.
+The aws_topic_origin utility is used to discover the datetime of the earliest recorded publication on the given
+topic(s), for a device, or for all topics known to aws_byline.
 
 SYNOPSIS
-aws_topic_origin.py [-c CREDENTIALS] [-i INDENT] [-v] TOPIC
+aws_topic_origin.py [-c CREDENTIALS] [-i INDENT] [-v] { -a | -d DEVICE | -t TOPIC_1 [...TOPIC_N] }
 
 EXAMPLES
-aws_topic_origin.py -v -c super south-coast-science-dev/development/loc/1/climate
+aws_topic_origin.py -vi4 -c super -d scs-be2-806
+aws_topic_origin.py -v -c super -a | node.py -s | csv_writer.py -v origins-2024-04-10.csv
 
-DOCUMENT EXAMPLE - OUTPUT
-{"topic": "south-coast-science-dev/development/loc/1/climate", "device": "scs-be2-3", "rec": "2023-03-14T00:00:03Z"}
+DOCUMENT EXAMPLE
+{"topic": "ricardo/gatwick/loc/1/gases", "device": "scs-bgx-507", "rec": "2019-05-10T09:17:39Z",
+"expiry": "2019-05-17T09:17:46Z"}
 
 SEE ALSO
 scs_analysis/aws_byline
 scs_analysis/aws_topic_history
 
 scs_lambda/aws_message_delete
 """
 
 import sys
 
 from scs_analysis.cmd.cmd_aws_topic_origin import CmdAWSTopicOrigin
+from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
+from scs_core.aws.manager.byline.byline_finder import BylineFinder
 from scs_core.aws.manager.topic_origin.topic_origin_finder import TopicOriginFinder
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
 from scs_core.client.http_exception import HTTPException
 from scs_core.client.network import Network
@@ -41,14 +46,15 @@
 from scs_core.data.json import JSONify
 
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
+# TODO: optionally exclude control topics - they are not in DynamoDB (or shouldn't be!)
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     # ----------------------------------------------------------------------------------------------------------------
     # cmd...
 
@@ -79,32 +85,42 @@
             logger.error("login: %s." % auth.authentication_status.description)
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        finder = TopicOriginFinder()
+        byline_finder = BylineFinder(reporter=BatchDownloadReporter('bylines'))
+        origin_finder = TopicOriginFinder(reporter=BatchDownloadReporter('origins'))
 
 
         # ------------------------------------------------------------------------------------------------------------
         # check...
 
         if not Network.is_available():
             logger.info("waiting for network")
             Network.wait()
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
-        origin = finder.find(auth.id_token, cmd.topic)
+        # topics...
+        if cmd.all:
+            topics = byline_finder.find_topics(auth.id_token)
+        elif cmd.device:
+            topics = byline_finder.find_topics_for_device(auth.id_token, cmd.device)
+        else:
+            topics = cmd.requested_topics
 
-        if origin:
-            print(JSONify.dumps(origin, indent=cmd.indent))
+        # origins...
+        origins = origin_finder.find_for_topics(auth.id_token, topics)
+
+        print(JSONify.dumps(origins, indent=cmd.indent))
+        logger.info("found: %s" % len(origins))
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/aws_topic_publisher.py` & `scs_analysis-3.8.2/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/aws_upload_interval.py` & `scs_analysis-3.8.2/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/baseline.py` & `scs_analysis-3.8.2/src/scs_analysis/baseline.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,19 +139,18 @@
             exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         # BylineFinder...
-        reporter = BatchDownloadReporter()
-        byline_finder = BylineFinder(reporter=reporter)
+        byline_finder = BylineFinder(reporter=BatchDownloadReporter('bylines'))
 
         # MessageManager...
-        history_finder = TopicHistoryFinder(reporter=reporter)
+        history_finder = TopicHistoryFinder(reporter=BatchDownloadReporter('history'))
 
         # DeviceControlClient...
         client = DeviceControlClient()
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/baseline_conf.py` & `scs_analysis-3.8.2/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/chart/chart.py` & `scs_analysis-3.8.2/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/chart/histo_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/chart/multi_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/chart/single_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/client_traffic.py` & `scs_analysis-3.8.2/src/scs_analysis/client_traffic.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_alert.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_alert_status.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_topic_origin.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_gas_concentration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 """
-Created on 9 Apr 2024
+Created on 15 Feb 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 from scs_analysis import version
+from scs_core.gas.gas import Gas
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdAWSTopicOrigin(object):
+class CmdSampleGasConcentration(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-i INDENT] [-v] TOPIC", version=version())
+        self.__parser = optparse.OptionParser(usage="%prog [-v] GAS DENSITY_PATH T_PATH [{P_PATH | -p PRESSURE}]",
+                                              version=version())
 
-        # identity...
-        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
-                                 help="the stored credentials to be presented")
-
-        # filters...
-        self.__parser.add_option("--indent", "-i", action="store", dest="indent", type=int,
-                                 help="pretty-print the output with INDENT")
+        # mode...
+        self.__parser.add_option("--pressure", "-p", type="float", action="store", dest="pressure",
+                                 default=Gas.STP_PRESSURE, help="assume constant atmospheric pressure in kPA "
+                                                                "(default %s)" % Gas.STP_PRESSURE)
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if not self.__args or len(self.__args) != 1:
+        if len(self.__args) < 3:
+            return False
+
+        if self.pressure is not None and self.p_path is not None:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
-    # properties: identity...
 
     @property
-    def credentials_name(self):
-        return self.__opts.credentials_name
+    def pressure(self):
+        return self.__opts.pressure
 
 
     @property
-    def topic(self):
-        return None if self.__args is None else self.__args[0]
+    def verbose(self):
+        return self.__opts.verbose
 
 
-    # ----------------------------------------------------------------------------------------------------------------
-    # properties: output...
+    @property
+    def gas(self):
+        return self.__args[0] if len(self.__args) > 0 else None
+
 
     @property
-    def indent(self):
-        return self.__opts.indent
+    def density_path(self):
+        return self.__args[1] if len(self.__args) > 1 else None
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def t_path(self):
+        return self.__args[2] if len(self.__args) > 2 else None
+
+
+    @property
+    def p_path(self):
+        return self.__args[3] if len(self.__args) > 3 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAWSTopicOrigin:{credentials_name:%s, indent:%s, verbose:%s, topic:%s}" % \
-               (self.credentials_name, self.indent, self.verbose, self.topic)
+        return "CmdSampleGasConcentration:{pressure:%s, verbose:%s, gas:%s, density_path:%s, t_path:%s, p_path:%s}" % \
+               (self.pressure, self.verbose, self.gas, self.density_path, self.t_path, self.p_path)
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_baseline.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_client_traffic.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_client_traffic.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_email.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_configuration_report.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_configuration_report.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_join.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_device_controller.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_device_monitor.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_device_monitor_status.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_node.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_organisations.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_error.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_gas_concentration.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,92 @@
 """
-Created on 15 Feb 2019
+Created on 16 Mar 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 from scs_analysis import version
-from scs_core.gas.gas import Gas
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleGasConcentration(object):
-    """unix command line handler"""
+class CmdLowPass(object):
+    """
+    unix command line handler
+    """
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] GAS DENSITY_PATH T_PATH [{P_PATH | -p PRESSURE}]",
+        self.__parser = optparse.OptionParser(usage="%prog -d DELTA_T -c CUT_OFF [-p PRECISION] [-v] [PATH]",
                                               version=version())
 
-        # mode...
-        self.__parser.add_option("--pressure", "-p", type="float", action="store", dest="pressure",
-                                 default=Gas.STP_PRESSURE, help="assume constant atmospheric pressure in kPA "
-                                                                "(default %s)" % Gas.STP_PRESSURE)
+        # compulsory...
+        self.__parser.add_option("--delta", "-d", type="float", action="store", dest="delta",
+                                 help="sampling time interval")
+
+        self.__parser.add_option("--cut-off", "-c", type="float", action="store", dest="cut_off",
+                                 help="cut-off frequency")
 
         # output...
+        self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
+                                 help="precision (default 0 decimal places)")
+
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if len(self.__args) < 3:
+        if self.delta is None or self.cut_off is None:
             return False
 
-        if self.pressure is not None and self.p_path is not None:
+        if self.__args and len(self.__args) != 1:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def pressure(self):
-        return self.__opts.pressure
+    def delta(self):
+        return self.__opts.delta
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def cut_off(self):
+        return self.__opts.cut_off
 
 
     @property
-    def gas(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+    def precision(self):
+        return self.__opts.precision
 
 
     @property
-    def density_path(self):
-        return self.__args[1] if len(self.__args) > 1 else None
-
-
-    @property
-    def t_path(self):
-        return self.__args[2] if len(self.__args) > 2 else None
+    def verbose(self):
+        return self.__opts.verbose
 
 
     @property
-    def p_path(self):
-        return self.__args[3] if len(self.__args) > 3 else None
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleGasConcentration:{pressure:%s, verbose:%s, gas:%s, density_path:%s, t_path:%s, p_path:%s}" % \
-               (self.pressure, self.verbose, self.gas, self.density_path, self.t_path, self.p_path)
+        return "CmdLowPassFilter:{delta:%s, cut_off:%s, precision:%s, verbose:%s, path:%s}" % \
+               (self.delta, self.cut_off, self.precision, self.verbose, self.path)
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_gas_density.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_gas_density.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_localize.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,65 @@
 """
-Created on 16 Mar 2017
+Created on 20 Mar 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 from scs_analysis import version
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdLowPass(object):
+class CmdSampleMedian(object):
     """
     unix command line handler
     """
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -d DELTA_T -c CUT_OFF [-p PRECISION] [-v] [PATH]",
+        self.__parser = optparse.OptionParser(usage="%prog [-w SIZE] [-p PRECISION] [-v] [PATH]",
                                               version=version())
 
-        # compulsory...
-        self.__parser.add_option("--delta", "-d", type="float", action="store", dest="delta",
-                                 help="sampling time interval")
-
-        self.__parser.add_option("--cut-off", "-c", type="float", action="store", dest="cut_off",
-                                 help="cut-off frequency")
+        # optional...
+        self.__parser.add_option("--window", "-w", type="int", action="store", dest="window", default=3,
+                                 help="window size (must be an odd number, default 3)")
 
         # output...
         self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
                                  help="precision (default 0 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.delta is None or self.cut_off is None:
+        if self.window is not None and self.window % 2 == 0:
             return False
 
         if self.__args and len(self.__args) != 1:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def delta(self):
-        return self.__opts.delta
-
-
-    @property
-    def cut_off(self):
-        return self.__opts.cut_off
+    def window(self):
+        return self.__opts.window
 
 
     @property
     def precision(self):
         return self.__opts.precision
 
 
@@ -84,9 +76,9 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdLowPassFilter:{delta:%s, cut_off:%s, precision:%s, verbose:%s, path:%s}" % \
-               (self.delta, self.cut_off, self.precision, self.verbose, self.path)
+        return "CmdSampleMedian:{window:%s, verbose:%s, precision:%s, path:%s}" % \
+               (self.window, self.verbose, self.precision, self.path)
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_median.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,50 @@
 """
-Created on 20 Mar 2018
+Created on 11 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 from scs_analysis import version
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleMedian(object):
-    """
-    unix command line handler
-    """
+class CmdSampleRecord(object):
+    """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-w SIZE] [-p PRECISION] [-v] [PATH]",
-                                              version=version())
-
-        # optional...
-        self.__parser.add_option("--window", "-w", type="int", action="store", dest="window", default=3,
-                                 help="window size (must be an odd number, default 3)")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] [PATH]", version=version())
 
         # output...
-        self.__parser.add_option("--prec", "-p", type="int", action="store", default=None, dest="precision",
-                                 help="precision (default 0 decimal places)")
-
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.window is not None and self.window % 2 == 0:
-            return False
-
-        if self.__args and len(self.__args) != 1:
+        if self.path is None:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def window(self):
-        return self.__opts.window
-
-
-    @property
-    def precision(self):
-        return self.__opts.precision
-
-
-    @property
     def verbose(self):
         return self.__opts.verbose
 
 
     @property
     def path(self):
         return self.__args[0] if len(self.__args) > 0 else None
@@ -76,9 +53,8 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleMedian:{window:%s, verbose:%s, precision:%s, path:%s}" % \
-               (self.window, self.verbose, self.precision, self.path)
+        return "CmdSampleRecord:{verbose:%s, path:%s}" % (self.verbose, self.path)
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_record.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_uds.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
-Created on 11 Jul 2016
+Created on 25 Apr 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 from scs_analysis import version
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleRecord(object):
+class CmdUDS(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] [PATH]", version=version())
+        self.__parser = optparse.OptionParser(usage="%prog [-v] UDS_SUB", version=version())
 
         # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
@@ -37,24 +37,24 @@
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+    def verbose(self):
+        return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleRecord:{verbose:%s, path:%s}" % (self.verbose, self.path)
+        return "CmdUDS:{verbose:%s}" % self.verbose
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_single_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_socket_receiver.py` & `scs_analysis-3.8.2/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cmd/cmd_uds.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,45 @@
 """
-Created on 25 Apr 2017
+Created on 6 Jul 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
-import optparse
+import sys
 
-from scs_analysis import version
+from scs_core.data.datetime import LocalizedDatetime
 
 
 # --------------------------------------------------------------------------------------------------------------------
+# reporter...
 
-class CmdUDS(object):
-    """unix command line handler"""
+class MQTTReporter(object):
+    """
+    classdocs
+    """
 
-    def __init__(self):
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __init__(self, verbose):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] UDS_SUB", version=version())
-
-        # output...
-        self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
-                                 help="report narrative to stderr")
-
-        self.__opts, self.__args = self.__parser.parse_args()
+        self.__verbose = verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def is_valid(self):
-        if self.path is None:
-            return False
-
-        return True
+    def print(self, status):
+        if not self.__verbose:
+            return
+
+        now = LocalizedDatetime.now().utc()
+        print("%s:         mqtt: %s" % (now.as_time(), status), file=sys.stderr)
+        sys.stderr.flush()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
-
-
-    @property
-    def verbose(self):
-        return self.__opts.verbose
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def print_help(self, file):
-        self.__parser.print_help(file)
-
-
     def __str__(self, *args, **kwargs):
-        return "CmdUDS:{verbose:%s}" % self.verbose
+        return "MQTTReporter:{verbose:%s}" % self.__verbose
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cognito_devices.py` & `scs_analysis-3.8.2/src/scs_analysis/cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cognito_email.py` & `scs_analysis-3.8.2/src/scs_analysis/cognito_email.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cognito_user_credentials.py` & `scs_analysis-3.8.2/src/scs_analysis/cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cognito_user_identity.py` & `scs_analysis-3.8.2/src/scs_analysis/cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/cognito_users.py` & `scs_analysis-3.8.2/src/scs_analysis/cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/configuration_csv.py` & `scs_analysis-3.8.2/src/scs_analysis/configuration_csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,19 +132,16 @@
         # resources...
 
         # nodes...
         if cmd.node_names:
             print(node_names, file=sys.stderr)
             exit(0)
 
-        # reporter...
-        reporter = BatchDownloadReporter()
-
         # ConfigurationFinder...
-        configuration_finder = ConfigurationFinder(reporter=reporter)
+        configuration_finder = ConfigurationFinder(reporter=BatchDownloadReporter('configurations'))
         check_finder = ConfigurationCheckFinder()
 
         # ConfigurationCSVGenerator...
         csv_generator = ConfigurationCSVGenerator(cmd.verbose)
 
 
         # ------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/configuration_monitor.py` & `scs_analysis-3.8.2/src/scs_analysis/configuration_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,15 @@
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         # ConfigurationFinder...
-        reporter = BatchDownloadReporter()
-        finder = ConfigurationFinder(reporter=reporter)
+        finder = ConfigurationFinder(reporter=BatchDownloadReporter('configurations'))
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         response = finder.find(auth.id_token, cmd.tag_filter, cmd.exact_match, cmd.response_mode())
         items = list(response)
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/configuration_monitor_check.py` & `scs_analysis-3.8.2/src/scs_analysis/configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/configuration_report.py` & `scs_analysis-3.8.2/src/scs_analysis/configuration_report.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/csv_collation_summary.py` & `scs_analysis-3.8.2/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/csv_collator.py` & `scs_analysis-3.8.2/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/csv_join.py` & `scs_analysis-3.8.2/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/csv_reader.py` & `scs_analysis-3.8.2/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/csv_segmentor.py` & `scs_analysis-3.8.2/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/csv_writer.py` & `scs_analysis-3.8.2/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/device_controller.py` & `scs_analysis-3.8.2/src/scs_analysis/device_controller.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/device_monitor.py` & `scs_analysis-3.8.2/src/scs_analysis/device_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/device_monitor_status.py` & `scs_analysis-3.8.2/src/scs_analysis/device_monitor_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/handler/batch_download_reporter.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 class BatchDownloadReporter(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self):
+    def __init__(self, name):
         """
         Constructor
         """
+        self.__name = name
+
         self.__block_count = 0
         self.__document_count = 0
         self.__start_time = time.time()
 
         self.__logger = Logging.getLogger()
 
 
@@ -48,24 +50,31 @@
         self.__block_count += 1
         self.__document_count += block_length
         elapsed_time = int(round(time.time() - self.__start_time))
         elapsed_delta = Timedelta(seconds=elapsed_time)
         elapsed = elapsed_delta.as_json()
 
         if block_start is None:
-            self.__logger.info("docs:%d elapsed:%s" % (self.__document_count, elapsed))
+            self.__logger.info("%s: docs:%d elapsed:%s" %
+                               (self.name, self.__document_count, elapsed))
         else:
-            self.__logger.info("block start:%s docs:%d elapsed:%s" % (block_start, self.__document_count, elapsed))
+            self.__logger.info("%s: block start:%s docs:%d elapsed:%s" %
+                               (self.name, block_start, self.__document_count, elapsed))
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
+    def name(self):
+        return self.__name
+
+
+    @property
     def block_count(self):
         return self.__block_count
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "BatchDownloadReporter:{block_count:%d, document_count:%d, start_time:%d}" % \
-               (self.block_count, self.__document_count, self.__start_time)
+        return "BatchDownloadReporter:{name:%d, block_count:%d, document_count:%d, start_time:%d}" % \
+               (self.name, self.block_count, self.__document_count, self.__start_time)
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/handler/configuration_csv_generator.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/handler/csv_collator.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/handler/csv_segmentor.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/handler/sample_midpoint.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/handler/sample_regression.py` & `scs_analysis-3.8.2/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/histo_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/localised_datetime.py` & `scs_analysis-3.8.2/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/monitor_auth.py` & `scs_analysis-3.8.2/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/multi_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/node.py` & `scs_analysis-3.8.2/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/organisation_devices.py` & `scs_analysis-3.8.2/src/scs_analysis/organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/organisation_path_roots.py` & `scs_analysis-3.8.2/src/scs_analysis/organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/organisation_user_paths.py` & `scs_analysis-3.8.2/src/scs_analysis/organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/organisation_users.py` & `scs_analysis-3.8.2/src/scs_analysis/organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/organisations.py` & `scs_analysis-3.8.2/src/scs_analysis/organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_aggregate.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_average.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_collator.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_distance.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_duplicates.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_error.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_gas_concentration.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_gas_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_gas_density.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_gas_density.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,25 +39,25 @@
 from scs_core.sys.logging import Logging
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 def gas_name(path):
     pieces = path.split('.')
-    return pieces[len(pieces) - 2]
+    return pieces[-2]
 
 
 def is_concentration(path):
     pieces = path.split('.')
-    return pieces[len(pieces) - 1] == 'cnc'
+    return pieces[-1] == 'cnc'
 
 
 def density_path(path):
     pieces = path.split('.')
-    pieces[len(pieces) - 1] = 'dns'
+    pieces[-1] = 'dns'
 
     return '.'.join(pieces)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_interval.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_iso_8601.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_localize.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_localize.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_low_pass.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_max.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_median.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_midpoint.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_min.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_noise.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_nullify.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_paths.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_regression.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_slope.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_sort.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_stats.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_subset.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/sample_time_shift.py` & `scs_analysis-3.8.2/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/single_chart.py` & `scs_analysis-3.8.2/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/socket_receiver.py` & `scs_analysis-3.8.2/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/timer.py` & `scs_analysis-3.8.2/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis/uds_receiver.py` & `scs_analysis-3.8.2/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-3.8.1/src/scs_analysis.egg-info/PKG-INFO` & `scs_analysis-3.8.2/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 3.8.1
+Version: 3.8.2
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-3.8.1/src/scs_analysis.egg-info/SOURCES.txt` & `scs_analysis-3.8.2/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

