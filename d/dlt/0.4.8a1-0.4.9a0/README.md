# Comparing `tmp/dlt-0.4.8a1.tar.gz` & `tmp/dlt-0.4.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.4.8a1.tar", max compression
+gzip compressed data, was "dlt-0.4.9a0.tar", max compression
```

## Comparing `dlt-0.4.8a1.tar` & `dlt-0.4.9a0.tar`

### file list

```diff
@@ -1,341 +1,347 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.4.8a1/LICENSE.txt
--rw-r--r--   0        0        0     5296 2024-03-22 07:07:43.963916 dlt-0.4.8a1/README.md
--rw-r--r--   0        0        0     2229 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/__init__.py
--rw-r--r--   0        0        0       69 2024-03-08 19:36:32.659855 dlt-0.4.8a1/dlt/__main__.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.8a1/dlt/cli/__init__.py
--rw-r--r--   0        0        0    21507 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     4178 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    18229 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    16912 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1944 2024-01-25 20:07:33.363195 dlt-0.4.8a1/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-11-18 17:38:04.257189 dlt-0.4.8a1/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    21105 2024-01-25 20:07:33.363195 dlt-0.4.8a1/dlt/cli/init_command.py
--rw-r--r--   0        0        0    14152 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0    10152 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     2524 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/requirements.py
--rw-r--r--   0        0        0     4895 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1912 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     2086 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/utils.py
--rw-r--r--   0        0        0      292 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/__init__.py
--rw-r--r--   0        0        0     1311 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      808 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5144 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     7410 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     8457 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0    11848 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1777 2024-01-25 20:07:33.363195 dlt-0.4.8a1/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      682 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      805 2024-03-05 18:21:35.930419 dlt-0.4.8a1/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1129 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1346 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1995 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     5161 2024-02-27 21:03:24.127544 dlt-0.4.8a1/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1319 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    13407 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    20983 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1742 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1836 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     5263 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0     2643 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/specs/azure_credentials.py
--rw-r--r--   0        0        0    18147 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     6498 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3456 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     2339 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2667 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    13313 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      874 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2856 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6680 2024-02-29 18:05:14.217554 dlt-0.4.8a1/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      220 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6859 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      269 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      537 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     9917 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     4936 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0     1021 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0    12252 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      423 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     3967 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0     5108 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/destination/exceptions.py
--rw-r--r--   0        0        0    24950 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6274 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/exceptions.py
--rw-r--r--   0        0        0     5149 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/git.py
--rw-r--r--   0        0        0     7195 2024-02-27 21:03:24.127544 dlt-0.4.8a1/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1814 2024-02-16 18:38:47.332466 dlt-0.4.8a1/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2948 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1562 2023-11-18 17:38:04.257189 dlt-0.4.8a1/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.8a1/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0      181 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/common/libs/numpy.py
--rw-r--r--   0        0        0      436 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/libs/pandas.py
--rw-r--r--   0        0        0      217 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/libs/pandas_sql.py
--rw-r--r--   0        0        0    14420 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0    15624 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/common/libs/pydantic.py
--rw-r--r--   0        0        0    15486 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/common/libs/sql_alchemy.py
--rw-r--r--   0        0        0     3652 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/logger.py
--rw-r--r--   0        0        0      854 2024-03-01 09:52:05.856761 dlt-0.4.8a1/dlt/common/managed_thread_pool.py
--rw-r--r--   0        0        0      384 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1408 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      510 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1905 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    14418 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0      123 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      810 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0      798 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      830 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     4570 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     2967 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      359 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     3426 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      461 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/common/pendulum.py
--rw-r--r--   0        0        0    31088 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.267189 dlt-0.4.8a1/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      375 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     6119 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5103 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      329 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      665 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     3640 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4132 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3162 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-11-18 17:38:04.267189 dlt-0.4.8a1/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5583 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       71 2023-11-18 17:38:04.267189 dlt-0.4.8a1/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    14599 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     5461 2024-01-25 20:07:33.363195 dlt-0.4.8a1/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0     1067 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     6616 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runtime/json_logging.py
--rw-r--r--   0        0        0     2074 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     6753 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2784 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     1938 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      582 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0     2960 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      579 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runtime/typing.py
--rw-r--r--   0        0        0      805 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     2419 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     5245 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0     5269 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/common/schema/migrations.py
--rw-r--r--   0        0        0    42525 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     5209 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    28381 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1672 2024-02-10 23:59:00.181729 dlt-0.4.8a1/dlt/common/source.py
--rw-r--r--   0        0        0     1182 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     4869 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     4833 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     4289 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    14242 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0    11056 2024-02-26 22:08:47.270507 dlt-0.4.8a1/dlt/common/storages/fsspec_filesystem.py
--rw-r--r--   0        0        0        0 2024-02-26 22:08:47.270507 dlt-0.4.8a1/dlt/common/storages/fsspecs/__init__.py
--rw-r--r--   0        0        0    20474 2024-02-26 22:08:47.270507 dlt-0.4.8a1/dlt/common/storages/fsspecs/google_drive.py
--rw-r--r--   0        0        0     3513 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    25742 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/storages/load_package.py
--rw-r--r--   0        0        0     9624 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     3197 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     9524 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9065 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2867 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     7578 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/common/time.py
--rw-r--r--   0        0        0     8854 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/common/typing.py
--rw-r--r--   0        0        0    19563 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/common/utils.py
--rw-r--r--   0        0        0     7978 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/common/validation.py
--rw-r--r--   0        0        0     1658 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/common/versioned_state.py
--rw-r--r--   0        0        0     5528 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/warnings.py
--rw-r--r--   0        0        0     1219 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/wei.py
--rw-r--r--   0        0        0     1147 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      404 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/adapters.py
--rw-r--r--   0        0        0     4855 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/decorators.py
--rw-r--r--   0        0        0     4918 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/destinations/impl/__init__.py
--rw-r--r--   0        0        0     1311 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/destinations/impl/athena/__init__.py
--rw-r--r--   0        0        0    18448 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/impl/athena/athena.py
--rw-r--r--   0        0        0     1054 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/athena/configuration.py
--rw-r--r--   0        0        0     2169 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/destinations/impl/athena/factory.py
--rw-r--r--   0        0        0      439 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/impl/bigquery/README.md
--rw-r--r--   0        0        0     1118 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/destinations/impl/bigquery/__init__.py
--rw-r--r--   0        0        0    18083 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/bigquery/bigquery.py
--rw-r--r--   0        0        0     7453 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/destinations/impl/bigquery/bigquery_adapter.py
--rw-r--r--   0        0        0     1714 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/bigquery/configuration.py
--rw-r--r--   0        0        0     1309 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/bigquery/factory.py
--rw-r--r--   0        0        0    10708 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/bigquery/sql_client.py
--rw-r--r--   0        0        0     1430 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/databricks/__init__.py
--rw-r--r--   0        0        0     2043 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/databricks/configuration.py
--rw-r--r--   0        0        0    13411 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/databricks/databricks.py
--rw-r--r--   0        0        0     1741 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/databricks/factory.py
--rw-r--r--   0        0        0     6136 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/databricks/sql_client.py
--rw-r--r--   0        0        0      706 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/impl/destination/__init__.py
--rw-r--r--   0        0        0     1046 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/destination/configuration.py
--rw-r--r--   0        0        0     7654 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/impl/destination/destination.py
--rw-r--r--   0        0        0     5631 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/impl/destination/factory.py
--rw-r--r--   0        0        0     1236 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/duckdb/__init__.py
--rw-r--r--   0        0        0     9013 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/duckdb/configuration.py
--rw-r--r--   0        0        0     6803 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/duckdb/duck.py
--rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/duckdb/factory.py
--rw-r--r--   0        0        0     6828 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/duckdb/sql_client.py
--rw-r--r--   0        0        0     1459 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/dummy/__init__.py
--rw-r--r--   0        0        0     1027 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/dummy/configuration.py
--rw-r--r--   0        0        0     6704 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/impl/dummy/dummy.py
--rw-r--r--   0        0        0     1111 2024-02-23 11:16:27.641941 dlt-0.4.8a1/dlt/destinations/impl/dummy/factory.py
--rw-r--r--   0        0        0      194 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/filesystem/__init__.py
--rw-r--r--   0        0        0      889 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/filesystem/configuration.py
--rw-r--r--   0        0        0     2411 2024-03-24 19:55:58.511453 dlt-0.4.8a1/dlt/destinations/impl/filesystem/factory.py
--rw-r--r--   0        0        0     9542 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/impl/filesystem/filesystem.py
--rw-r--r--   0        0        0     1134 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/motherduck/__init__.py
--rw-r--r--   0        0        0     3243 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/motherduck/configuration.py
--rw-r--r--   0        0        0     1966 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/motherduck/factory.py
--rw-r--r--   0        0        0      911 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/motherduck/motherduck.py
--rw-r--r--   0        0        0     1515 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/motherduck/sql_client.py
--rw-r--r--   0        0        0      253 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/mssql/README.md
--rw-r--r--   0        0        0     1385 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/mssql/__init__.py
--rw-r--r--   0        0        0     3971 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/mssql/configuration.py
--rw-r--r--   0        0        0     1764 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/mssql/factory.py
--rw-r--r--   0        0        0     7267 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/mssql/mssql.py
--rw-r--r--   0        0        0     6282 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/mssql/sql_client.py
--rw-r--r--   0        0        0      251 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/postgres/README.md
--rw-r--r--   0        0        0     1349 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/postgres/__init__.py
--rw-r--r--   0        0        0     1794 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/postgres/configuration.py
--rw-r--r--   0        0        0     1840 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/postgres/factory.py
--rw-r--r--   0        0        0     5320 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/postgres/postgres.py
--rw-r--r--   0        0        0     5678 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/postgres/sql_client.py
--rw-r--r--   0        0        0      677 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/qdrant/__init__.py
--rw-r--r--   0        0        0     3044 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/qdrant/configuration.py
--rw-r--r--   0        0        0     1146 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/qdrant/factory.py
--rw-r--r--   0        0        0     1831 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/qdrant/qdrant_adapter.py
--rw-r--r--   0        0        0    17902 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/impl/qdrant/qdrant_client.py
--rw-r--r--   0        0        0     1159 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/redshift/README.md
--rw-r--r--   0        0        0     1181 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/redshift/__init__.py
--rw-r--r--   0        0        0     1005 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/redshift/configuration.py
--rw-r--r--   0        0        0     2006 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/redshift/factory.py
--rw-r--r--   0        0        0    10603 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/redshift/redshift.py
--rw-r--r--   0        0        0     1218 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/snowflake/__init__.py
--rw-r--r--   0        0        0     5449 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/snowflake/configuration.py
--rw-r--r--   0        0        0     2008 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/snowflake/factory.py
--rw-r--r--   0        0        0    11443 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/snowflake/snowflake.py
--rw-r--r--   0        0        0     6885 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/snowflake/sql_client.py
--rw-r--r--   0        0        0     2355 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/synapse/__init__.py
--rw-r--r--   0        0        0     2746 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/synapse/configuration.py
--rw-r--r--   0        0        0     2640 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/synapse/factory.py
--rw-r--r--   0        0        0     1179 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/synapse/sql_client.py
--rw-r--r--   0        0        0    13083 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/impl/synapse/synapse.py
--rw-r--r--   0        0        0     2231 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/destinations/impl/synapse/synapse_adapter.py
--rw-r--r--   0        0        0      526 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/weaviate/README.md
--rw-r--r--   0        0        0      752 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/weaviate/__init__.py
--rw-r--r--   0        0        0      280 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/weaviate/ci_naming.py
--rw-r--r--   0        0        0     2009 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/weaviate/configuration.py
--rw-r--r--   0        0        0      666 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/impl/weaviate/exceptions.py
--rw-r--r--   0        0        0     1935 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/weaviate/factory.py
--rw-r--r--   0        0        0     3259 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/weaviate/naming.py
--rw-r--r--   0        0        0     3914 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/weaviate/weaviate_adapter.py
--rw-r--r--   0        0        0    26322 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/impl/weaviate/weaviate_client.py
--rw-r--r--   0        0        0     6532 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    23883 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     2086 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     3049 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/path_utils.py
--rw-r--r--   0        0        0     9310 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    21311 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/sql_jobs.py
--rw-r--r--   0        0        0     4895 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/type_mapping.py
--rw-r--r--   0        0        0     1877 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/typing.py
--rw-r--r--   0        0        0      506 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/utils.py
--rw-r--r--   0        0        0      639 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/extract/__init__.py
--rw-r--r--   0        0        0     8539 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/extract/concurrency.py
--rw-r--r--   0        0        0    35614 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/extract/decorators.py
--rw-r--r--   0        0        0    16480 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/extract/exceptions.py
--rw-r--r--   0        0        0    17152 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/extract/extract.py
--rw-r--r--   0        0        0    14914 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/extract/extractors.py
--rw-r--r--   0        0        0    18640 2024-03-24 08:57:37.871597 dlt-0.4.8a1/dlt/extract/hints.py
--rw-r--r--   0        0        0    29556 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/extract/incremental/__init__.py
--rw-r--r--   0        0        0     1142 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/extract/incremental/exceptions.py
--rw-r--r--   0        0        0    14942 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/extract/incremental/transform.py
--rw-r--r--   0        0        0      322 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/extract/incremental/typing.py
--rw-r--r--   0        0        0     6786 2024-03-24 08:57:37.871597 dlt-0.4.8a1/dlt/extract/items.py
--rw-r--r--   0        0        0    16368 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/extract/pipe.py
--rw-r--r--   0        0        0    16344 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/extract/pipe_iterator.py
--rw-r--r--   0        0        0    26683 2024-03-24 08:57:37.871597 dlt-0.4.8a1/dlt/extract/resource.py
--rw-r--r--   0        0        0    19990 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/extract/source.py
--rw-r--r--   0        0        0     5293 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/extract/storage.py
--rw-r--r--   0        0        0     9254 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/extract/utils.py
--rw-r--r--   0        0        0     3500 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/extract/validation.py
--rw-r--r--   0        0        0      832 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/extract/wrappers.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.4.8a1/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    23495 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3701 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1241 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6821 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      772 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     7163 2024-02-07 18:59:43.286965 dlt-0.4.8a1/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    15742 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     4881 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/helpers/dbt_cloud/__init__.py
--rw-r--r--   0        0        0     4926 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/helpers/dbt_cloud/client.py
--rw-r--r--   0        0        0      623 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/helpers/dbt_cloud/configuration.py
--rw-r--r--   0        0        0      349 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/__init__.py
--rw-r--r--   0        0        0     1230 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/load_info.py
--rw-r--r--   0        0        0      483 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/menu.py
--rw-r--r--   0        0        0     2451 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/query.py
--rw-r--r--   0        0        0      928 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/resource_state.py
--rw-r--r--   0        0        0      618 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/show_data.py
--rw-r--r--   0        0        0     2842 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/table_hints.py
--rw-r--r--   0        0        0      150 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/index.py
--rw-r--r--   0        0        0        0 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/__init__.py
--rw-r--r--   0        0        0     1668 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/dashboard.py
--rw-r--r--   0        0        0     4446 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/load_info.py
--rw-r--r--   0        0        0      757 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/theme.py
--rw-r--r--   0        0        0     2361 2024-03-24 08:57:37.871597 dlt-0.4.8a1/dlt/helpers/streamlit_app/utils.py
--rw-r--r--   0        0        0      386 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/__init__.py
--rw-r--r--   0        0        0      901 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/color_mode_selector.py
--rw-r--r--   0        0        0     1004 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/logo.py
--rw-r--r--   0        0        0      613 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/schema.py
--rw-r--r--   0        0        0     1542 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/stats.py
--rw-r--r--   0        0        0      805 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/summary.py
--rw-r--r--   0        0        0     1189 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/tags.py
--rw-r--r--   0        0        0       51 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/load/__init__.py
--rw-r--r--   0        0        0      807 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/load/configuration.py
--rw-r--r--   0        0        0     2061 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/load/exceptions.py
--rw-r--r--   0        0        0    24626 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/load/load.py
--rw-r--r--   0        0        0     8096 2024-03-20 22:31:16.351558 dlt-0.4.8a1/dlt/load/utils.py
--rw-r--r--   0        0        0       58 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1525 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/normalize/configuration.py
--rw-r--r--   0        0        0      529 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    15226 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/normalize/items_normalizers.py
--rw-r--r--   0        0        0    20321 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    14454 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     2098 2024-03-25 16:17:38.059826 dlt-0.4.8a1/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      709 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4950 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     4599 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     9792 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      212 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    73879 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0     3858 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/pipeline/platform.py
--rw-r--r--   0        0        0     1007 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     5539 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0    13256 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     5579 2024-02-27 21:03:24.147544 dlt-0.4.8a1/dlt/pipeline/track.py
--rw-r--r--   0        0        0       92 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/typing.py
--rw-r--r--   0        0        0      796 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/warnings.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.4.8a1/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      565 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/reflection/names.py
--rw-r--r--   0        0        0     5818 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6278 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      417 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/__init__.py
--rw-r--r--   0        0        0      110 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/config.py
--rw-r--r--   0        0        0      790 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/credentials.py
--rw-r--r--   0        0        0      200 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/filesystem.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0     1291 2024-03-27 11:19:53.626208 dlt-0.4.8a1/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0    10965 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      234 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/sources/helpers/requests/typing.py
--rw-r--r--   0        0        0     1210 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/__init__.py
--rw-r--r--   0        0        0     7202 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/auth.py
--rw-r--r--   0        0        0     9317 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/client.py
--rw-r--r--   0        0        0     4502 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/detector.py
--rw-r--r--   0        0        0      103 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/exceptions.py
--rw-r--r--   0        0        0     5510 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/paginators.py
--rw-r--r--   0        0        0      446 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/typing.py
--rw-r--r--   0        0        0      406 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/utils.py
--rw-r--r--   0        0        0      682 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-11-28 14:04:28.308006 dlt-0.4.8a1/dlt/version.py
--rw-r--r--   0        0        0     6929 2024-03-27 12:18:58.750863 dlt-0.4.8a1/pyproject.toml
--rw-r--r--   0        0        0     9890 1970-01-01 00:00:00.000000 dlt-0.4.8a1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.4.9a0/LICENSE.txt
+-rw-r--r--   0        0        0     5298 2024-04-14 11:41:16.421673 dlt-0.4.9a0/README.md
+-rw-r--r--   0        0        0     2229 2024-04-07 14:59:43.705656 dlt-0.4.9a0/dlt/__init__.py
+-rw-r--r--   0        0        0       69 2024-03-08 19:36:32.659855 dlt-0.4.9a0/dlt/__main__.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    21512 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     4187 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    18229 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    16912 2024-04-13 11:38:43.050742 dlt-0.4.9a0/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1944 2024-01-25 20:07:33.363195 dlt-0.4.9a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-11-18 17:38:04.257189 dlt-0.4.9a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    21105 2024-04-13 11:38:33.320742 dlt-0.4.9a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    14157 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0    10152 2024-04-13 11:38:50.650742 dlt-0.4.9a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     2524 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/cli/requirements.py
+-rw-r--r--   0        0        0     4895 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1912 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     1999 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      292 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1311 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      808 2024-04-07 14:59:43.705656 dlt-0.4.9a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5144 2024-01-24 17:23:08.476518 dlt-0.4.9a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     7410 2024-04-07 14:59:43.705656 dlt-0.4.9a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     8457 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0    11848 2024-04-13 11:29:48.720735 dlt-0.4.9a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1777 2024-01-25 20:07:33.363195 dlt-0.4.9a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      682 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      805 2024-03-05 18:21:35.930419 dlt-0.4.9a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1129 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1346 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1995 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     5141 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1319 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    13416 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    20983 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1742 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1836 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     5263 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0     2591 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/specs/azure_credentials.py
+-rw-r--r--   0        0        0    18147 2024-04-11 11:44:50.568746 dlt-0.4.9a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     6498 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3456 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     2339 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2667 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    13349 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      874 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2856 2024-04-09 13:29:46.170457 dlt-0.4.9a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6650 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      220 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6832 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      269 2024-01-24 17:23:08.486518 dlt-0.4.9a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      592 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0    10821 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     5665 2024-04-14 11:41:16.421673 dlt-0.4.9a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0     1757 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0    23095 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      423 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     3651 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0     5132 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/destination/exceptions.py
+-rw-r--r--   0        0        0    25485 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6274 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     5149 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/git.py
+-rw-r--r--   0        0        0     7099 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1814 2024-02-16 18:38:47.332466 dlt-0.4.9a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2948 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1562 2023-11-18 17:38:04.257189 dlt-0.4.9a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.9a0/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/libs/numpy.py
+-rw-r--r--   0        0        0      436 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/libs/pandas.py
+-rw-r--r--   0        0        0      217 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/libs/pandas_sql.py
+-rw-r--r--   0        0        0    14934 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0    15624 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/common/libs/pydantic.py
+-rw-r--r--   0        0        0    15486 2024-03-08 19:36:32.669855 dlt-0.4.9a0/dlt/common/libs/sql_alchemy.py
+-rw-r--r--   0        0        0     3652 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/logger.py
+-rw-r--r--   0        0        0      854 2024-03-01 09:52:05.856761 dlt-0.4.9a0/dlt/common/managed_thread_pool.py
+-rw-r--r--   0        0        0      384 2024-03-18 14:01:48.098768 dlt-0.4.9a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1408 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      510 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1905 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    16970 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0      123 2024-03-18 14:01:48.098768 dlt-0.4.9a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      810 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0      798 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      830 2024-03-18 14:01:48.098768 dlt-0.4.9a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     4570 2024-03-18 14:01:48.098768 dlt-0.4.9a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     2967 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      359 2024-03-18 14:01:48.108768 dlt-0.4.9a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     3426 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      461 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    31127 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.267189 dlt-0.4.9a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      375 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     6119 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5103 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      329 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      665 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     3678 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4132 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3162 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-11-18 17:38:04.267189 dlt-0.4.9a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5583 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       71 2023-11-18 17:38:04.267189 dlt-0.4.9a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    14599 2024-04-13 11:30:10.760740 dlt-0.4.9a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     5461 2024-01-25 20:07:33.363195 dlt-0.4.9a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0     1067 2024-04-13 11:30:15.860741 dlt-0.4.9a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     6616 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runtime/json_logging.py
+-rw-r--r--   0        0        0     2044 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     6702 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2784 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     1938 2024-04-13 11:30:29.100742 dlt-0.4.9a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      613 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2960 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      579 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/runtime/typing.py
+-rw-r--r--   0        0        0      805 2024-01-24 17:23:08.496518 dlt-0.4.9a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     2454 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     5308 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0     5269 2024-03-18 14:01:48.108768 dlt-0.4.9a0/dlt/common/schema/migrations.py
+-rw-r--r--   0        0        0    42497 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     5865 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    28875 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1672 2024-02-10 23:59:00.181729 dlt-0.4.9a0/dlt/common/source.py
+-rw-r--r--   0        0        0     1224 2024-04-14 11:41:16.431673 dlt-0.4.9a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     4869 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     4230 2024-04-13 11:30:55.040743 dlt-0.4.9a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     4184 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    14242 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0    11065 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/fsspec_filesystem.py
+-rw-r--r--   0        0        0        0 2024-02-26 22:08:47.270507 dlt-0.4.9a0/dlt/common/storages/fsspecs/__init__.py
+-rw-r--r--   0        0        0    20479 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/fsspecs/google_drive.py
+-rw-r--r--   0        0        0     3513 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    26784 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/load_package.py
+-rw-r--r--   0        0        0    10771 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     3197 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     9551 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9065 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2867 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     7604 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/time.py
+-rw-r--r--   0        0        0     8878 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    19596 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     7978 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     2369 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/common/versioned_state.py
+-rw-r--r--   0        0        0     5528 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/warnings.py
+-rw-r--r--   0        0        0     1219 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/common/wei.py
+-rw-r--r--   0        0        0     1217 2024-04-11 11:44:50.568746 dlt-0.4.9a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      404 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/destinations/adapters.py
+-rw-r--r--   0        0        0     4856 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/destinations/decorators.py
+-rw-r--r--   0        0        0     4918 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/destinations/impl/__init__.py
+-rw-r--r--   0        0        0     1311 2024-03-18 14:01:48.108768 dlt-0.4.9a0/dlt/destinations/impl/athena/__init__.py
+-rw-r--r--   0        0        0    18693 2024-04-13 11:31:25.760744 dlt-0.4.9a0/dlt/destinations/impl/athena/athena.py
+-rw-r--r--   0        0        0     1054 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/athena/configuration.py
+-rw-r--r--   0        0        0     2169 2024-01-24 17:23:08.506518 dlt-0.4.9a0/dlt/destinations/impl/athena/factory.py
+-rw-r--r--   0        0        0      439 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/destinations/impl/bigquery/README.md
+-rw-r--r--   0        0        0     1118 2024-03-18 14:01:48.108768 dlt-0.4.9a0/dlt/destinations/impl/bigquery/__init__.py
+-rw-r--r--   0        0        0    21073 2024-04-14 11:41:16.441673 dlt-0.4.9a0/dlt/destinations/impl/bigquery/bigquery.py
+-rw-r--r--   0        0        0     8397 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/bigquery/bigquery_adapter.py
+-rw-r--r--   0        0        0     1740 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/bigquery/configuration.py
+-rw-r--r--   0        0        0     1309 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/bigquery/factory.py
+-rw-r--r--   0        0        0    10772 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1430 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/databricks/__init__.py
+-rw-r--r--   0        0        0     2043 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/databricks/configuration.py
+-rw-r--r--   0        0        0    13640 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/databricks/databricks.py
+-rw-r--r--   0        0        0     1741 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/databricks/factory.py
+-rw-r--r--   0        0        0     6074 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/databricks/sql_client.py
+-rw-r--r--   0        0        0      673 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/destination/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/destination/configuration.py
+-rw-r--r--   0        0        0     3675 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/destination/destination.py
+-rw-r--r--   0        0        0     5626 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/destination/factory.py
+-rw-r--r--   0        0        0     1243 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/__init__.py
+-rw-r--r--   0        0        0     1617 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/configuration.py
+-rw-r--r--   0        0        0     8692 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/dremio.py
+-rw-r--r--   0        0        0     1787 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/factory.py
+-rw-r--r--   0        0        0     9314 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dremio/pydremio.py
+-rw-r--r--   0        0        0     5934 2024-04-13 11:31:52.880745 dlt-0.4.9a0/dlt/destinations/impl/dremio/sql_client.py
+-rw-r--r--   0        0        0     1236 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/duckdb/__init__.py
+-rw-r--r--   0        0        0     9013 2024-04-13 11:31:56.870745 dlt-0.4.9a0/dlt/destinations/impl/duckdb/configuration.py
+-rw-r--r--   0        0        0     7022 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/duckdb/duck.py
+-rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/duckdb/factory.py
+-rw-r--r--   0        0        0     6828 2024-04-05 22:42:00.549456 dlt-0.4.9a0/dlt/destinations/impl/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1485 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/dummy/__init__.py
+-rw-r--r--   0        0        0     1027 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/dummy/configuration.py
+-rw-r--r--   0        0        0     6713 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/dummy/dummy.py
+-rw-r--r--   0        0        0     1111 2024-02-23 11:16:27.641941 dlt-0.4.9a0/dlt/destinations/impl/dummy/factory.py
+-rw-r--r--   0        0        0      194 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/filesystem/__init__.py
+-rw-r--r--   0        0        0      889 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/filesystem/configuration.py
+-rw-r--r--   0        0        0     2411 2024-03-24 19:55:58.511453 dlt-0.4.9a0/dlt/destinations/impl/filesystem/factory.py
+-rw-r--r--   0        0        0     9542 2024-04-13 11:32:01.360745 dlt-0.4.9a0/dlt/destinations/impl/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1134 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/motherduck/__init__.py
+-rw-r--r--   0        0        0     3111 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/motherduck/configuration.py
+-rw-r--r--   0        0        0     1966 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/motherduck/factory.py
+-rw-r--r--   0        0        0      911 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1515 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/motherduck/sql_client.py
+-rw-r--r--   0        0        0      253 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/mssql/README.md
+-rw-r--r--   0        0        0     1385 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/mssql/__init__.py
+-rw-r--r--   0        0        0     3971 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/mssql/configuration.py
+-rw-r--r--   0        0        0     1764 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/mssql/factory.py
+-rw-r--r--   0        0        0     7537 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/mssql/mssql.py
+-rw-r--r--   0        0        0     6629 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/mssql/sql_client.py
+-rw-r--r--   0        0        0      251 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/postgres/README.md
+-rw-r--r--   0        0        0     1356 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/postgres/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/postgres/configuration.py
+-rw-r--r--   0        0        0     1840 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/postgres/factory.py
+-rw-r--r--   0        0        0     6940 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/postgres/postgres.py
+-rw-r--r--   0        0        0     5678 2024-03-31 18:13:49.090176 dlt-0.4.9a0/dlt/destinations/impl/postgres/sql_client.py
+-rw-r--r--   0        0        0      677 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/qdrant/__init__.py
+-rw-r--r--   0        0        0     3044 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/qdrant/configuration.py
+-rw-r--r--   0        0        0     1146 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/qdrant/factory.py
+-rw-r--r--   0        0        0     1831 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/qdrant/qdrant_adapter.py
+-rw-r--r--   0        0        0    17960 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/qdrant/qdrant_client.py
+-rw-r--r--   0        0        0     1159 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/redshift/README.md
+-rw-r--r--   0        0        0     1181 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/redshift/__init__.py
+-rw-r--r--   0        0        0     1005 2024-04-09 13:29:46.180457 dlt-0.4.9a0/dlt/destinations/impl/redshift/configuration.py
+-rw-r--r--   0        0        0     2006 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/redshift/factory.py
+-rw-r--r--   0        0        0    10832 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/redshift/redshift.py
+-rw-r--r--   0        0        0     1218 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/snowflake/__init__.py
+-rw-r--r--   0        0        0     5449 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/snowflake/configuration.py
+-rw-r--r--   0        0        0     2008 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/snowflake/factory.py
+-rw-r--r--   0        0        0    11468 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/snowflake/snowflake.py
+-rw-r--r--   0        0        0     6885 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/snowflake/sql_client.py
+-rw-r--r--   0        0        0     2851 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/synapse/__init__.py
+-rw-r--r--   0        0        0     2746 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/synapse/configuration.py
+-rw-r--r--   0        0        0     2640 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/synapse/factory.py
+-rw-r--r--   0        0        0     1179 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/synapse/sql_client.py
+-rw-r--r--   0        0        0    13201 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/impl/synapse/synapse.py
+-rw-r--r--   0        0        0     2231 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/destinations/impl/synapse/synapse_adapter.py
+-rw-r--r--   0        0        0      526 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/weaviate/README.md
+-rw-r--r--   0        0        0      752 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/destinations/impl/weaviate/__init__.py
+-rw-r--r--   0        0        0      280 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/weaviate/ci_naming.py
+-rw-r--r--   0        0        0     2009 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/weaviate/configuration.py
+-rw-r--r--   0        0        0      666 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/destinations/impl/weaviate/exceptions.py
+-rw-r--r--   0        0        0     1935 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/weaviate/factory.py
+-rw-r--r--   0        0        0     3259 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/impl/weaviate/naming.py
+-rw-r--r--   0        0        0     3914 2024-02-07 18:59:43.276965 dlt-0.4.9a0/dlt/destinations/impl/weaviate/weaviate_adapter.py
+-rw-r--r--   0        0        0    26468 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/impl/weaviate/weaviate_client.py
+-rw-r--r--   0        0        0     6149 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    23940 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     6300 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     3075 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/path_utils.py
+-rw-r--r--   0        0        0     9279 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    26428 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/destinations/sql_jobs.py
+-rw-r--r--   0        0        0     4895 2024-02-27 21:03:24.137544 dlt-0.4.9a0/dlt/destinations/type_mapping.py
+-rw-r--r--   0        0        0     1877 2024-01-24 17:23:08.516518 dlt-0.4.9a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0      506 2024-04-11 11:44:50.568746 dlt-0.4.9a0/dlt/destinations/utils.py
+-rw-r--r--   0        0        0      639 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0     8539 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/extract/concurrency.py
+-rw-r--r--   0        0        0    35950 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    16480 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0    17697 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    15690 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/extract/extractors.py
+-rw-r--r--   0        0        0    21382 2024-04-14 11:41:16.451673 dlt-0.4.9a0/dlt/extract/hints.py
+-rw-r--r--   0        0        0    29587 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/extract/incremental/__init__.py
+-rw-r--r--   0        0        0     1142 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/extract/incremental/exceptions.py
+-rw-r--r--   0        0        0    14951 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/extract/incremental/transform.py
+-rw-r--r--   0        0        0      322 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/extract/incremental/typing.py
+-rw-r--r--   0        0        0     6786 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/extract/items.py
+-rw-r--r--   0        0        0    16368 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0    16344 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/extract/pipe_iterator.py
+-rw-r--r--   0        0        0    26683 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/extract/resource.py
+-rw-r--r--   0        0        0    19990 2024-03-18 14:01:48.118769 dlt-0.4.9a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4650 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/extract/storage.py
+-rw-r--r--   0        0        0    10122 2024-04-09 20:42:07.310460 dlt-0.4.9a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0     3500 2024-03-08 19:36:32.679855 dlt-0.4.9a0/dlt/extract/validation.py
+-rw-r--r--   0        0        0      832 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/extract/wrappers.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.4.9a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    23547 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3701 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6848 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      772 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     7163 2024-02-07 18:59:43.286965 dlt-0.4.9a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    15742 2024-04-13 11:33:15.710743 dlt-0.4.9a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     4881 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/helpers/dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     4926 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/helpers/dbt_cloud/client.py
+-rw-r--r--   0        0        0      623 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/helpers/dbt_cloud/configuration.py
+-rw-r--r--   0        0        0      349 2024-04-14 11:41:16.461673 dlt-0.4.9a0/dlt/helpers/streamlit_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/load_info.py
+-rw-r--r--   0        0        0      483 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/menu.py
+-rw-r--r--   0        0        0     2451 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/query.py
+-rw-r--r--   0        0        0     1139 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/resource_state.py
+-rw-r--r--   0        0        0      618 2024-04-07 14:59:43.715656 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/show_data.py
+-rw-r--r--   0        0        0     2842 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/table_hints.py
+-rw-r--r--   0        0        0      150 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/index.py
+-rw-r--r--   0        0        0        0 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/__init__.py
+-rw-r--r--   0        0        0     1668 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/dashboard.py
+-rw-r--r--   0        0        0     4446 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/load_info.py
+-rw-r--r--   0        0        0      757 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/theme.py
+-rw-r--r--   0        0        0     2361 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/helpers/streamlit_app/utils.py
+-rw-r--r--   0        0        0      386 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/color_mode_selector.py
+-rw-r--r--   0        0        0     1004 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/logo.py
+-rw-r--r--   0        0        0      613 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/schema.py
+-rw-r--r--   0        0        0     1542 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/stats.py
+-rw-r--r--   0        0        0      805 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/summary.py
+-rw-r--r--   0        0        0     1189 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/tags.py
+-rw-r--r--   0        0        0       51 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0      807 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     2061 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    25029 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/load/load.py
+-rw-r--r--   0        0        0     8096 2024-04-13 11:33:36.000744 dlt-0.4.9a0/dlt/load/utils.py
+-rw-r--r--   0        0        0       58 2024-01-24 17:23:08.526518 dlt-0.4.9a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1525 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0      644 2024-04-09 20:42:07.320460 dlt-0.4.9a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    18280 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/normalize/items_normalizers.py
+-rw-r--r--   0        0        0    22419 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    15006 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2097 2024-04-09 20:42:07.320460 dlt-0.4.9a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      709 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4950 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     4599 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     9785 2024-04-09 20:42:07.320460 dlt-0.4.9a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      212 2024-04-07 14:59:43.725656 dlt-0.4.9a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    74019 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3864 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/platform.py
+-rw-r--r--   0        0        0     1007 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4856 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0    13259 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     5610 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       92 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0      796 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/pipeline/warnings.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.4.9a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      565 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5818 2024-04-13 11:34:58.380741 dlt-0.4.9a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6278 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      417 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      110 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/config.py
+-rw-r--r--   0        0        0      790 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0      200 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/filesystem.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-09 20:42:07.320460 dlt-0.4.9a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10965 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.536518 dlt-0.4.9a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-11-18 17:38:04.277189 dlt-0.4.9a0/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0     1210 2024-04-13 11:26:19.690742 dlt-0.4.9a0/dlt/sources/helpers/rest_client/__init__.py
+-rw-r--r--   0        0        0     7190 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/sources/helpers/rest_client/auth.py
+-rw-r--r--   0        0        0     9181 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/sources/helpers/rest_client/client.py
+-rw-r--r--   0        0        0     4456 2024-04-13 22:20:19.334997 dlt-0.4.9a0/dlt/sources/helpers/rest_client/detector.py
+-rw-r--r--   0        0        0      103 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/sources/helpers/rest_client/exceptions.py
+-rw-r--r--   0        0        0     6001 2024-04-13 22:20:19.334997 dlt-0.4.9a0/dlt/sources/helpers/rest_client/paginators.py
+-rw-r--r--   0        0        0      426 2024-04-13 22:20:19.334997 dlt-0.4.9a0/dlt/sources/helpers/rest_client/typing.py
+-rw-r--r--   0        0        0      406 2024-04-09 13:29:46.190457 dlt-0.4.9a0/dlt/sources/helpers/rest_client/utils.py
+-rw-r--r--   0        0        0     4860 2024-04-14 11:41:16.471673 dlt-0.4.9a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1130 2024-04-14 11:41:16.481673 dlt-0.4.9a0/dlt/version.py
+-rw-r--r--   0        0        0     6985 2024-04-14 11:41:36.261674 dlt-0.4.9a0/pyproject.toml
+-rw-r--r--   0        0        0     9936 1970-01-01 00:00:00.000000 dlt-0.4.9a0/PKG-INFO
```

### Comparing `dlt-0.4.8a1/LICENSE.txt` & `dlt-0.4.9a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/README.md` & `dlt-0.4.9a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -109,8 +109,8 @@
 - **Track progress of our work and our plans**: Please check out our [public Github project](https://github.com/orgs/dlt-hub/projects/9)
 - **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.
 - **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.
 - **Improve documentation**: Help us enhance the dlt documentation.
 
 ## License
 
-DLT is released under the [Apache 2.0 License](LICENSE.txt).
+`dlt` is released under the [Apache 2.0 License](LICENSE.txt).
```

### Comparing `dlt-0.4.8a1/dlt/__init__.py` & `dlt-0.4.9a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/_dlt.py` & `dlt-0.4.9a0/dlt/cli/_dlt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Sequence, Optional
 import yaml
 import os
 import argparse
 import click
 
 from dlt.version import __version__
-from dlt.common import json
+from dlt.common.json import json
 from dlt.common.schema import Schema
 from dlt.common.typing import DictStrAny
 from dlt.common.runners import Venv
 
 import dlt.cli.echo as fmt
 from dlt.cli import utils
 from dlt.pipeline.exceptions import CannotRestorePipelineException
```

### Comparing `dlt-0.4.8a1/dlt/cli/config_toml_writer.py` & `dlt-0.4.9a0/dlt/cli/config_toml_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, NamedTuple, Tuple, Iterable
 import tomlkit
 from tomlkit.items import Table as TOMLTable
 from tomlkit.container import Container as TOMLContainer
 from collections.abc import Sequence as C_Sequence
 
-from dlt.common import pendulum
+from dlt.common.pendulum import pendulum
 from dlt.common.configuration.specs import (
     BaseConfiguration,
     is_base_configuration_inner_hint,
     extract_inner_hint,
 )
 from dlt.common.data_types import py_type_to_sc_type
 from dlt.common.typing import AnyType, is_final_type, is_optional_type
```

### Comparing `dlt-0.4.8a1/dlt/cli/deploy_command.py` & `dlt-0.4.9a0/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/deploy_command_helpers.py` & `dlt-0.4.9a0/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/echo.py` & `dlt-0.4.9a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/init_command.py` & `dlt-0.4.9a0/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/pipeline_command.py` & `dlt-0.4.9a0/dlt/cli/pipeline_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import yaml
 from typing import Any, Optional, Sequence, Tuple
 import dlt
 from dlt.cli.exceptions import CliCommandException
 
-from dlt.common import json
+from dlt.common.json import json
 from dlt.common.pipeline import resource_state, get_dlt_pipelines_dir, TSourceState
 from dlt.common.destination.reference import TDestinationReferenceArg
 from dlt.common.runners import Venv
 from dlt.common.runners.stdout import iter_stdout
 from dlt.common.schema.utils import group_tables_by_resource, remove_defaults
 from dlt.common.storages import FileStorage, PackageStorage
 from dlt.pipeline.helpers import DropCommand
```

### Comparing `dlt-0.4.8a1/dlt/cli/pipeline_files.py` & `dlt-0.4.9a0/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/requirements.py` & `dlt-0.4.9a0/dlt/cli/requirements.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/source_detection.py` & `dlt-0.4.9a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/telemetry_command.py` & `dlt-0.4.9a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/cli/utils.py` & `dlt-0.4.9a0/dlt/cli/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import ast
 import os
-import tempfile
 from typing import Callable
 
-from dlt.common import git
 from dlt.common.reflection.utils import set_ast_parents
-from dlt.common.storages import FileStorage
 from dlt.common.typing import TFun
 from dlt.common.configuration import resolve_configuration
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.runtime.telemetry import with_telemetry
 
 from dlt.reflection.script_visitor import PipelineScriptVisitor
```

### Comparing `dlt-0.4.8a1/dlt/common/arithmetics.py` & `dlt-0.4.9a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/__init__.py` & `dlt-0.4.9a0/dlt/common/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/accessors.py` & `dlt-0.4.9a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/container.py` & `dlt-0.4.9a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/exceptions.py` & `dlt-0.4.9a0/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/inject.py` & `dlt-0.4.9a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/paths.py` & `dlt-0.4.9a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/providers/__init__.py` & `dlt-0.4.9a0/dlt/common/configuration/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/providers/airflow.py` & `dlt-0.4.9a0/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/providers/context.py` & `dlt-0.4.9a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/providers/dictionary.py` & `dlt-0.4.9a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/providers/environ.py` & `dlt-0.4.9a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.4.9a0/dlt/common/configuration/providers/google_secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import base64
 import string
 import re
-from typing import Tuple
 
-from dlt.common import json
+from dlt.common.json import json
 from dlt.common.configuration.specs import GcpServiceAccountCredentials
 from dlt.common.exceptions import MissingDependencyException
 from .toml import VaultTomlProvider
 from .provider import get_key_name
 
 # Create a translation table to replace punctuation with ""
 # since google secrets allow "-"" and "_" we need to exclude them
```

### Comparing `dlt-0.4.8a1/dlt/common/configuration/providers/provider.py` & `dlt-0.4.9a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/providers/toml.py` & `dlt-0.4.9a0/dlt/common/configuration/providers/toml.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import abc
 import tomlkit
 import contextlib
 from tomlkit.items import Item as TOMLItem
 from tomlkit.container import Container as TOMLContainer
 from typing import Any, Dict, Optional, Tuple, Type, Union
 
-from dlt.common import pendulum
+from dlt.common.pendulum import pendulum
 from dlt.common.configuration.paths import get_dlt_settings_dir, get_dlt_data_dir
 from dlt.common.configuration.utils import auto_cast
 from dlt.common.configuration.specs import known_sections
 from dlt.common.configuration.specs.base_configuration import is_secret_hint
 from dlt.common.utils import update_dict_nested
 
 from dlt.common.typing import AnyType
```

### Comparing `dlt-0.4.8a1/dlt/common/configuration/resolve.py` & `dlt-0.4.9a0/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/__init__.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/azure_credentials.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/azure_credentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Optional, Dict, Any
 
-from dlt.common import pendulum
-from dlt.common.exceptions import MissingDependencyException
+from dlt.common.pendulum import pendulum
 from dlt.common.typing import TSecretStrValue
 from dlt.common.configuration.specs import (
     CredentialsConfiguration,
     CredentialsWithDefault,
     configspec,
 )
 from dlt.common.configuration.specs.exceptions import InvalidBoto3Session
```

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/exceptions.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 import sys
 from typing import Any, ClassVar, Final, List, Tuple, Union, Dict
 
-from dlt.common import json, pendulum
+from dlt.common.json import json
+from dlt.common.pendulum import pendulum
 from dlt.common.configuration.specs.api_credentials import OAuth2Credentials
 from dlt.common.configuration.specs.exceptions import (
     InvalidGoogleNativeCredentialsType,
     InvalidGoogleOauth2Json,
     InvalidGoogleServicesJson,
     NativeValueError,
     OAuth2ScopesRequired,
```

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/known_sections.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.4.9a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/configuration/utils.py` & `dlt-0.4.9a0/dlt/common/configuration/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import ast
 import contextlib
 import tomlkit
 from typing import Any, Dict, Mapping, NamedTuple, Optional, Tuple, Type, Sequence
 from collections.abc import Mapping as C_Mapping
 
-from dlt.common import json
+from dlt.common.json import json
 from dlt.common.typing import AnyType, TAny
 from dlt.common.data_types import coerce_value, py_type_to_sc_type
 from dlt.common.configuration.providers import EnvironProvider
 from dlt.common.configuration.exceptions import ConfigValueCannotBeCoercedException, LookupTrace
 from dlt.common.configuration.specs.base_configuration import (
     BaseConfiguration,
     is_base_configuration_inner_hint,
@@ -118,16 +118,14 @@
     config: Optional[BaseConfiguration],
     key: str,
     hint: Type[Any],
     value: Any,
     default_value: Any,
     traces: Sequence[LookupTrace],
 ) -> None:
-    from dlt.common import logger
-
     # if logger.is_logging() and logger.log_level() == "DEBUG" and config:
     #     logger.debug(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
     # print(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
     # for tr in traces:
     #     # print(str(tr))
     #     logger.debug(str(tr))
     # store all traces with resolved values
```

### Comparing `dlt-0.4.8a1/dlt/common/data_types/type_helpers.py` & `dlt-0.4.9a0/dlt/common/data_types/type_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import binascii
 import base64
 import dataclasses
 import datetime  # noqa: I251
 from collections.abc import Mapping as C_Mapping, Sequence as C_Sequence
-from typing import Any, Type, Literal, Union, cast
+from typing import Any, Type, Union
 from enum import Enum
 
-from dlt.common import pendulum, json, Decimal, Wei
 from dlt.common.json import custom_pua_remove, json
 from dlt.common.json._simplejson import custom_encode as json_custom_encode
-from dlt.common.arithmetics import InvalidOperation
+from dlt.common.wei import Wei
+from dlt.common.arithmetics import InvalidOperation, Decimal
 from dlt.common.data_types.typing import TDataType
 from dlt.common.time import (
     ensure_pendulum_datetime,
     ensure_pendulum_date,
     ensure_pendulum_time,
 )
 from dlt.common.utils import map_nested_in_place, str2bool
```

### Comparing `dlt-0.4.8a1/dlt/common/data_writers/__init__.py` & `dlt-0.4.9a0/dlt/common/data_writers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from dlt.common.data_writers.writers import DataWriter, DataWriterMetrics, TLoaderFileFormat
+from dlt.common.data_writers.writers import (
+    DataWriter,
+    DataWriterMetrics,
+    TDataItemFormat,
+    FileWriterSpec,
+)
 from dlt.common.data_writers.buffered import BufferedDataWriter, new_file_id
 from dlt.common.data_writers.escape import (
     escape_redshift_literal,
     escape_redshift_identifier,
     escape_bigquery_identifier,
 )
 
 __all__ = [
     "DataWriter",
+    "FileWriterSpec",
     "DataWriterMetrics",
-    "TLoaderFileFormat",
+    "TDataItemFormat",
     "BufferedDataWriter",
     "new_file_id",
     "escape_redshift_literal",
     "escape_redshift_identifier",
     "escape_bigquery_identifier",
 ]
```

### Comparing `dlt-0.4.8a1/dlt/common/data_writers/buffered.py` & `dlt-0.4.9a0/dlt/common/data_writers/buffered.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import gzip
 import time
-from typing import ClassVar, List, IO, Any, Optional, Type, TypeVar, Generic
+from typing import ClassVar, List, IO, Any, Optional, Type, Generic
 
 from dlt.common.typing import TDataItem, TDataItems
-from dlt.common.data_writers import TLoaderFileFormat
 from dlt.common.data_writers.exceptions import (
     BufferedDataWriterClosed,
     DestinationCapabilitiesRequired,
     InvalidFileNameTemplateException,
 )
-from dlt.common.data_writers.writers import DataWriter, DataWriterMetrics
+from dlt.common.data_writers.writers import TWriter, DataWriter, DataWriterMetrics, FileWriterSpec
 from dlt.common.schema.typing import TTableSchemaColumns
 from dlt.common.configuration import with_config, known_sections, configspec
 from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.utils import uniq_id
 
-TWriter = TypeVar("TWriter", bound=DataWriter)
-
 
 def new_file_id() -> str:
     """Creates new file id which is globally unique within table_name scope"""
     return uniq_id(5)
 
 
 class BufferedDataWriter(Generic[TWriter]):
@@ -34,40 +31,41 @@
         _caps: Optional[DestinationCapabilitiesContext] = None
 
         __section__: ClassVar[str] = known_sections.DATA_WRITER
 
     @with_config(spec=BufferedDataWriterConfiguration)
     def __init__(
         self,
-        file_format: TLoaderFileFormat,
+        writer_spec: FileWriterSpec,
         file_name_template: str,
         *,
         buffer_max_items: int = 5000,
         file_max_items: int = None,
         file_max_bytes: int = None,
         disable_compression: bool = False,
         _caps: DestinationCapabilitiesContext = None
     ):
-        self.file_format = file_format
-        self._file_format_spec = DataWriter.data_format_from_file_format(self.file_format)
-        if self._file_format_spec.requires_destination_capabilities and not _caps:
-            raise DestinationCapabilitiesRequired(file_format)
+        self.writer_spec = writer_spec
+        if self.writer_spec.requires_destination_capabilities and not _caps:
+            raise DestinationCapabilitiesRequired(self.writer_spec.file_format)
+        self.writer_cls = DataWriter.class_factory(
+            writer_spec.file_format, writer_spec.data_item_format
+        )
+        self._supports_schema_changes = self.writer_spec.supports_schema_changes
         self._caps = _caps
         # validate if template has correct placeholders
         self.file_name_template = file_name_template
         self.closed_files: List[DataWriterMetrics] = []  # all fully processed files
         # buffered items must be less than max items in file
         self.buffer_max_items = min(buffer_max_items, file_max_items or buffer_max_items)
         self.file_max_bytes = file_max_bytes
         self.file_max_items = file_max_items
         # the open function is either gzip.open or open
         self.open = (
-            gzip.open
-            if self._file_format_spec.supports_compression and not disable_compression
-            else open
+            gzip.open if self.writer_spec.supports_compression and not disable_compression else open
         )
 
         self._current_columns: TTableSchemaColumns = None
         self._file_name: str = None
         self._buffered_items: List[TDataItem] = []
         self._buffered_items_count: int = 0
         self._writer: TWriter = None
@@ -83,16 +81,17 @@
     def write_data_item(self, item: TDataItems, columns: TTableSchemaColumns) -> int:
         if self._closed:
             self._rotate_file()
             self._closed = False
         # rotate file if columns changed and writer does not allow for that
         # as the only allowed change is to add new column (no updates/deletes), we detect the change by comparing lengths
         if (
-            self._writer
-            and not self._writer.data_format().supports_schema_changes
+            self._current_columns is not None
+            and (self._writer or self._supports_schema_changes == "False")
+            and self._supports_schema_changes != "True"
             and len(columns) != len(self._current_columns)
         ):
             assert len(columns) > len(self._current_columns)
             self._rotate_file()
         # until the first chunk is written we can change the columns schema freely
         if columns is not None:
             self._current_columns = dict(columns)
@@ -161,64 +160,83 @@
         self._file_name = None
         self._last_modified = None
         self._created = None
         # get ready for a next one
         self._rotate_file()
         return metrics
 
-    def close(self) -> None:
-        self._ensure_open()
-        self._flush_and_close_file()
-        self._closed = True
+    def close(self, skip_flush: bool = False) -> None:
+        """Flushes the data, writes footer (skip_flush is True), collects metrics and closes the underlying file."""
+        # like regular files, we do not except on double close
+        if not self._closed:
+            self._flush_and_close_file(skip_flush=skip_flush)
+            self._closed = True
 
     @property
     def closed(self) -> bool:
         return self._closed
 
     def __enter__(self) -> "BufferedDataWriter[TWriter]":
         return self
 
     def __exit__(self, exc_type: Type[BaseException], exc_val: BaseException, exc_tb: Any) -> None:
-        self.close()
+        # skip flush if we had exception
+        in_exception = exc_val is not None
+        try:
+            self.close(skip_flush=in_exception)
+        except Exception:
+            if not in_exception:
+                # close again but without flush
+                self.close(skip_flush=True)
+            # raise the on close exception if we are not handling another exception
+            if not in_exception:
+                raise
 
     def _rotate_file(self, allow_empty_file: bool = False) -> DataWriterMetrics:
         metrics = self._flush_and_close_file(allow_empty_file)
         self._file_name = (
-            self.file_name_template % new_file_id() + "." + self._file_format_spec.file_extension
+            self.file_name_template % new_file_id() + "." + self.writer_spec.file_extension
         )
         self._created = time.time()
         return metrics
 
     def _flush_items(self, allow_empty_file: bool = False) -> None:
-        if self._buffered_items_count > 0 or allow_empty_file:
+        if self._buffered_items or allow_empty_file:
             # we only open a writer when there are any items in the buffer and first flush is requested
             if not self._writer:
                 # create new writer and write header
-                if self._file_format_spec.is_binary_format:
+                if self.writer_spec.is_binary_format:
                     self._file = self.open(self._file_name, "wb")  # type: ignore
                 else:
-                    self._file = self.open(self._file_name, "wt", encoding="utf-8")  # type: ignore
-                self._writer = DataWriter.from_file_format(self.file_format, self._file, caps=self._caps)  # type: ignore[assignment]
+                    self._file = self.open(self._file_name, "wt", encoding="utf-8", newline="")  # type: ignore
+                self._writer = self.writer_cls(self._file, caps=self._caps)  # type: ignore[assignment]
                 self._writer.write_header(self._current_columns)
             # write buffer
             if self._buffered_items:
                 self._writer.write_data(self._buffered_items)
             # reset buffer and counter
             self._buffered_items.clear()
             self._buffered_items_count = 0
 
-    def _flush_and_close_file(self, allow_empty_file: bool = False) -> DataWriterMetrics:
-        # if any buffered items exist, flush them
-        self._flush_items(allow_empty_file)
-        # if writer exists then close it
-        if not self._writer:
-            return None
-        # write the footer of a file
-        self._writer.write_footer()
-        self._file.flush()
+    def _flush_and_close_file(
+        self, allow_empty_file: bool = False, skip_flush: bool = False
+    ) -> DataWriterMetrics:
+        if not skip_flush:
+            # if any buffered items exist, flush them
+            self._flush_items(allow_empty_file)
+            # if writer exists then close it
+            if not self._writer:
+                return None
+            # write the footer of a file
+            self._writer.write_footer()
+            self._file.flush()
+        else:
+            if not self._writer:
+                return None
+        self._writer.close()
         # add file written to the list so we can commit all the files later
         metrics = DataWriterMetrics(
             self._file_name,
             self._writer.items_count,
             self._file.tell(),
             self._created,
             self._last_modified,
```

### Comparing `dlt-0.4.8a1/dlt/common/data_writers/escape.py` & `dlt-0.4.9a0/dlt/common/data_writers/escape.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 import base64
 from typing import Any, Dict
 from datetime import date, datetime, time  # noqa: I251
 
 from dlt.common.json import json
+from dlt.common.pendulum import pendulum
+from dlt.common.time import reduce_pendulum_datetime_precision
 
 # use regex to escape characters in single pass
 SQL_ESCAPE_DICT = {"'": "''", "\\": "\\\\", "\n": "\\n", "\r": "\\r"}
 
 
 def _make_sql_escape_re(escape_dict: Dict[str, str]) -> re.Pattern:  # type: ignore[type-arg]
     return re.compile(
@@ -115,14 +117,15 @@
 
 def escape_redshift_identifier(v: str) -> str:
     return '"' + v.replace('"', '""').replace("\\", "\\\\") + '"'
 
 
 escape_postgres_identifier = escape_redshift_identifier
 escape_athena_identifier = escape_postgres_identifier
+escape_dremio_identifier = escape_postgres_identifier
 
 
 def escape_bigquery_identifier(v: str) -> str:
     # https://cloud.google.com/bigquery/docs/reference/standard-sql/lexical
     return "`" + v.replace("\\", "\\\\").replace("`", "\\`") + "`"
 
 
@@ -147,7 +150,21 @@
         return _escape_extended(json.dumps(v), prefix="'", escape_dict=DATABRICKS_ESCAPE_DICT)
     if isinstance(v, bytes):
         return f"X'{v.hex()}'"
     if v is None:
         return "NULL"
 
     return str(v)
+
+
+def format_datetime_literal(v: pendulum.DateTime, precision: int = 6, no_tz: bool = False) -> str:
+    """Converts `v` to ISO string, optionally without timezone spec (in UTC) and with given `precision`"""
+    if no_tz:
+        v = v.in_timezone(tz="UTC").replace(tzinfo=None)
+    v = reduce_pendulum_datetime_precision(v, precision)
+    # yet another precision translation
+    timespec: str = "microseconds"
+    if precision < 6:
+        timespec = "milliseconds"
+    elif precision < 3:
+        timespec = "seconds"
+    return v.isoformat(sep=" ", timespec=timespec)
```

### Comparing `dlt-0.4.8a1/dlt/common/data_writers/exceptions.py` & `dlt-0.4.9a0/dlt/common/data_writers/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,7 +23,26 @@
 
 class DestinationCapabilitiesRequired(DataWriterException, ValueError):
     def __init__(self, file_format: TLoaderFileFormat):
         self.file_format = file_format
         super().__init__(
             f"Writer for {file_format} requires destination capabilities which were not provided."
         )
+
+
+class DataWriterNotFound(DataWriterException):
+    def __init__(self, file_format: TLoaderFileFormat, data_item_format: str):
+        self.file_format = file_format
+        self.data_item_format = data_item_format
+        super().__init__(
+            f"Can't find a file writer for file format {file_format} and item format"
+            f" {data_item_format}"
+        )
+
+
+class InvalidDataItem(DataWriterException):
+    def __init__(self, file_format: TLoaderFileFormat, data_item_format: str, details: str):
+        self.file_format = file_format
+        self.data_item_format = data_item_format
+        super().__init__(
+            f"A data item of type {data_item_format} cannot be written as {file_format}: {details}"
+        )
```

### Comparing `dlt-0.4.8a1/dlt/common/destination/capabilities.py` & `dlt-0.4.9a0/dlt/common/destination/capabilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,32 +2,23 @@
 
 from dlt.common.configuration.utils import serialize_value
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import ContainerInjectableContext
 from dlt.common.utils import identity
 
 from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
-
 from dlt.common.wei import EVM_DECIMAL_PRECISION
 
 # known loader file formats
 # jsonl - new line separated json documents
-# puae-jsonl - internal extract -> normalize format bases on jsonl
+# typed-jsonl - internal extract -> normalize format bases on jsonl
 # insert_values - insert SQL statements
 # sql - any sql statement
-TLoaderFileFormat = Literal[
-    "jsonl", "puae-jsonl", "insert_values", "sql", "parquet", "reference", "arrow"
-]
+TLoaderFileFormat = Literal["jsonl", "typed-jsonl", "insert_values", "parquet", "csv"]
 ALL_SUPPORTED_FILE_FORMATS: Set[TLoaderFileFormat] = set(get_args(TLoaderFileFormat))
-# file formats used internally by dlt
-INTERNAL_LOADER_FILE_FORMATS: Set[TLoaderFileFormat] = {"sql", "reference", "arrow"}
-# file formats that may be chosen by the user
-EXTERNAL_LOADER_FILE_FORMATS: Set[TLoaderFileFormat] = (
-    set(get_args(TLoaderFileFormat)) - INTERNAL_LOADER_FILE_FORMATS
-)
 
 
 @configspec
 class DestinationCapabilitiesContext(ContainerInjectableContext):
     """Injectable destination capabilities required for many Pipeline stages ie. normalize"""
 
     preferred_loader_file_format: TLoaderFileFormat = None
@@ -63,15 +54,15 @@
 
     @staticmethod
     def generic_capabilities(
         preferred_loader_file_format: TLoaderFileFormat = None,
     ) -> "DestinationCapabilitiesContext":
         caps = DestinationCapabilitiesContext()
         caps.preferred_loader_file_format = preferred_loader_file_format
-        caps.supported_loader_file_formats = ["jsonl", "insert_values", "parquet"]
+        caps.supported_loader_file_formats = ["jsonl", "insert_values", "parquet", "csv"]
         caps.preferred_staging_file_format = None
         caps.supported_staging_file_formats = []
         caps.escape_identifier = identity
         caps.escape_literal = serialize_value
         caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
         caps.wei_precision = (EVM_DECIMAL_PRECISION, 0)
         caps.max_identifier_length = 65536
```

### Comparing `dlt-0.4.8a1/dlt/common/destination/exceptions.py` & `dlt-0.4.9a0/dlt/common/destination/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,17 @@
                 msg = (
                     f"Unsupported file format {file_format} for destination {destination} in"
                     f" combination with staging destination {staging}. Supported formats:"
                     f" {supported_formats_str}"
                 )
         else:
             msg = (
-                f"Unsupported file format {file_format} destination {destination}. Supported"
-                f" formats: {supported_formats_str}. Check the staging option in the dlt.pipeline"
-                " for additional formats."
+                f"Unsupported file format {file_format} in destination {destination}. Supported"
+                f" formats: {supported_formats_str}. If {destination} supports loading data via"
+                " staging bucket, more formats may be available."
             )
         super().__init__(msg)
 
 
 class IdentifierTooLongException(DestinationTerminalException):
     def __init__(
         self,
```

### Comparing `dlt-0.4.8a1/dlt/common/destination/reference.py` & `dlt-0.4.9a0/dlt/common/destination/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 )
 import datetime  # noqa: 251
 from copy import deepcopy
 import inspect
 
 from dlt.common import logger
 from dlt.common.schema import Schema, TTableSchema, TSchemaTables
+from dlt.common.schema.typing import MERGE_STRATEGIES
 from dlt.common.schema.exceptions import SchemaException
 from dlt.common.schema.utils import (
     get_write_disposition,
     get_table_format,
     get_columns_names_with_prop,
     has_column_with_prop,
     get_first_column_name_with_prop,
@@ -340,14 +341,20 @@
             if len(table_name) > self.capabilities.max_identifier_length:
                 raise IdentifierTooLongException(
                     self.config.destination_type,
                     "table",
                     table_name,
                     self.capabilities.max_identifier_length,
                 )
+            if table.get("write_disposition") == "merge":
+                if "x-merge-strategy" in table and table["x-merge-strategy"] not in MERGE_STRATEGIES:  # type: ignore[typeddict-item]
+                    raise SchemaException(
+                        f'"{table["x-merge-strategy"]}" is not a valid merge strategy. '  # type: ignore[typeddict-item]
+                        f"""Allowed values: {', '.join(['"' + s + '"' for s in MERGE_STRATEGIES])}."""
+                    )
             if has_column_with_prop(table, "hard_delete"):
                 if len(get_columns_names_with_prop(table, "hard_delete")) > 1:
                     raise SchemaException(
                         f'Found multiple "hard_delete" column hints for table "{table_name}" in'
                         f' schema "{self.schema.name}" while only one is allowed:'
                         f' {", ".join(get_columns_names_with_prop(table, "hard_delete"))}.'
                     )
```

### Comparing `dlt-0.4.8a1/dlt/common/exceptions.py` & `dlt-0.4.9a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/git.py` & `dlt-0.4.9a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/json/__init__.py` & `dlt-0.4.9a0/dlt/common/json/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from enum import Enum
 
 try:
     from pydantic import BaseModel as PydanticBaseModel
 except ImportError:
     PydanticBaseModel = None  # type: ignore[misc]
 
-from dlt.common import pendulum
+from dlt.common.pendulum import pendulum
 from dlt.common.arithmetics import Decimal
 from dlt.common.wei import Wei
 from dlt.common.utils import map_nested_in_place
 
 
 class SupportsJson(Protocol):
     """Minimum adapter for different json parser implementations"""
@@ -95,27 +95,27 @@
 
 
 def _datetime_decoder(obj: str) -> datetime:
     if obj.endswith("Z"):
         # Backwards compatibility for data encoded with previous dlt version
         # fromisoformat does not support Z suffix (until py3.11)
         obj = obj[:-1] + "+00:00"
-    return pendulum.DateTime.fromisoformat(obj)  # type: ignore[attr-defined, no-any-return]
+    return pendulum.DateTime.fromisoformat(obj)
 
 
 # define decoder for each prefix
 DECODERS: List[Callable[[Any], Any]] = [
     Decimal,
     _datetime_decoder,
-    pendulum.Date.fromisoformat,  # type: ignore[attr-defined]
+    pendulum.Date.fromisoformat,
     UUID,
     HexBytes,
     base64.b64decode,
     Wei,
-    pendulum.Time.fromisoformat,  # type: ignore[attr-defined]
+    pendulum.Time.fromisoformat,
 ]
 # how many decoders?
 PUA_CHARACTER_MAX = len(DECODERS)
 
 
 def custom_pua_encode(obj: Any) -> str:
     # wei is subclass of decimal and must be checked first
```

### Comparing `dlt-0.4.8a1/dlt/common/json/_orjson.py` & `dlt-0.4.9a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/json/_simplejson.py` & `dlt-0.4.9a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/jsonpath.py` & `dlt-0.4.9a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/libs/pyarrow.py` & `dlt-0.4.9a0/dlt/common/libs/pyarrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 from datetime import datetime, date  # noqa: I251
 from pendulum.tz import UTC
-from typing import Any, Tuple, Optional, Union, Callable, Iterable, Iterator, Sequence, Tuple
+from typing import (
+    Any,
+    Dict,
+    Mapping,
+    Tuple,
+    Optional,
+    Union,
+    Callable,
+    Iterable,
+    Iterator,
+    Sequence,
+    Tuple,
+)
 
 from dlt import version
-from dlt.common import pendulum
+from dlt.common.pendulum import pendulum
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.schema.typing import DLT_NAME_PREFIX, TTableSchemaColumns
 
 from dlt.common.destination.capabilities import DestinationCapabilitiesContext
 from dlt.common.schema.typing import TColumnType
 from dlt.common.typing import StrStr, TFileOrPath
 from dlt.common.normalizers.naming import NamingConvention
@@ -19,20 +31,21 @@
 except ModuleNotFoundError:
     raise MissingDependencyException(
         "dlt pyarrow helpers",
         [f"{version.DLT_PKG_NAME}[parquet]"],
         "Install pyarrow to be allow to load arrow tables, panda frames and to use parquet files.",
     )
 
-
 TAnyArrowItem = Union[pyarrow.Table, pyarrow.RecordBatch]
 
 
 def get_py_arrow_datatype(
-    column: TColumnType, caps: DestinationCapabilitiesContext, tz: str
+    column: TColumnType,
+    caps: DestinationCapabilitiesContext,
+    tz: str,
 ) -> Any:
     column_type = column["data_type"]
     if column_type == "text":
         return pyarrow.string()
     elif column_type == "double":
         return pyarrow.float64()
     elif column_type == "bool":
@@ -61,14 +74,15 @@
     elif column_type == "time":
         return get_py_arrow_time(column.get("precision") or caps.timestamp_precision)
     else:
         raise ValueError(column_type)
 
 
 def get_py_arrow_timestamp(precision: int, tz: str) -> Any:
+    tz = tz if tz else None
     if precision == 0:
         return pyarrow.timestamp("s", tz=tz)
     if precision <= 3:
         return pyarrow.timestamp("ms", tz=tz)
     if precision <= 6:
         return pyarrow.timestamp("us", tz=tz)
     return pyarrow.timestamp("ns", tz=tz)
@@ -101,15 +115,15 @@
     elif precision <= 16:
         return pyarrow.int16()
     elif precision <= 32:
         return pyarrow.int32()
     return pyarrow.int64()
 
 
-def _get_column_type_from_py_arrow(dtype: pyarrow.DataType) -> TColumnType:
+def get_column_type_from_py_arrow(dtype: pyarrow.DataType) -> TColumnType:
     """Returns (data_type, precision, scale) tuple from pyarrow.DataType"""
     if pyarrow.types.is_string(dtype) or pyarrow.types.is_large_string(dtype):
         return dict(data_type="text")
     elif pyarrow.types.is_floating(dtype):
         return dict(data_type="double")
     elif pyarrow.types.is_boolean(dtype):
         return dict(data_type="bool")
@@ -201,45 +215,57 @@
             field.with_name(new_name) for new_name, field in zip(new_column_names, item.schema)
         ]
         return pyarrow.RecordBatch.from_arrays(item.columns, schema=pyarrow.schema(new_fields))
     else:
         raise TypeError(f"Unsupported data item type {type(item)}")
 
 
-def normalize_py_arrow_schema(
-    item: TAnyArrowItem,
+def should_normalize_arrow_schema(
+    schema: pyarrow.Schema,
     columns: TTableSchemaColumns,
     naming: NamingConvention,
-    caps: DestinationCapabilitiesContext,
-) -> TAnyArrowItem:
-    """Normalize arrow `item` schema according to the `columns`.
-
-    1. arrow schema field names will be normalized according to `naming`
-    2. arrows columns will be reordered according to `columns`
-    3. empty columns will be inserted if they are missing, types will be generated using `caps`
-    """
-    rename_mapping = get_normalized_arrow_fields_mapping(item, naming)
+) -> Tuple[bool, Mapping[str, str], Dict[str, str], TTableSchemaColumns]:
+    rename_mapping = get_normalized_arrow_fields_mapping(schema, naming)
     rev_mapping = {v: k for k, v in rename_mapping.items()}
-    dlt_table_prefix = naming.normalize_table_identifier(DLT_NAME_PREFIX)
+    dlt_tables = list(map(naming.normalize_table_identifier, ("_dlt_id", "_dlt_load_id")))
 
     # remove all columns that are dlt columns but are not present in arrow schema. we do not want to add such columns
     # that should happen in the normalizer
     columns = {
         name: column
         for name, column in columns.items()
-        if not name.startswith(dlt_table_prefix) or name in rev_mapping
+        if name not in dlt_tables or name in rev_mapping
     }
 
     # check if nothing to rename
-    if list(rename_mapping.keys()) == list(rename_mapping.values()):
-        # check if nothing to reorder
-        if list(rename_mapping.keys())[: len(columns)] == list(columns.keys()):
-            return item
+    skip_normalize = (
+        list(rename_mapping.keys()) == list(rename_mapping.values()) == list(columns.keys())
+    )
+    return not skip_normalize, rename_mapping, rev_mapping, columns
+
 
+def normalize_py_arrow_item(
+    item: TAnyArrowItem,
+    columns: TTableSchemaColumns,
+    naming: NamingConvention,
+    caps: DestinationCapabilitiesContext,
+) -> TAnyArrowItem:
+    """Normalize arrow `item` schema according to the `columns`.
+
+    1. arrow schema field names will be normalized according to `naming`
+    2. arrows columns will be reordered according to `columns`
+    3. empty columns will be inserted if they are missing, types will be generated using `caps`
+    """
     schema = item.schema
+    should_normalize, rename_mapping, rev_mapping, columns = should_normalize_arrow_schema(
+        schema, columns, naming
+    )
+    if not should_normalize:
+        return item
+
     new_fields = []
     new_columns = []
 
     for column_name, column in columns.items():
         # get original field name
         field_name = rev_mapping.pop(column_name, column_name)
         if field_name in rename_mapping:
@@ -264,18 +290,18 @@
         new_fields.append(schema.field(idx).with_name(column_name))
         new_columns.append(item.column(idx))
 
     # create desired type
     return item.__class__.from_arrays(new_columns, schema=pyarrow.schema(new_fields))
 
 
-def get_normalized_arrow_fields_mapping(item: TAnyArrowItem, naming: NamingConvention) -> StrStr:
+def get_normalized_arrow_fields_mapping(schema: pyarrow.Schema, naming: NamingConvention) -> StrStr:
     """Normalizes schema field names and returns mapping from original to normalized name. Raises on name clashes"""
     norm_f = naming.normalize_identifier
-    name_mapping = {n.name: norm_f(n.name) for n in item.schema}
+    name_mapping = {n.name: norm_f(n.name) for n in schema}
     # verify if names uniquely normalize
     normalized_names = set(name_mapping.values())
     if len(name_mapping) != len(normalized_names):
         raise NameNormalizationClash(
             f"Arrow schema fields normalized from {list(name_mapping.keys())} to"
             f" {list(normalized_names)}"
         )
@@ -292,30 +318,30 @@
         TTableSchemaColumns: table schema columns
     """
     result: TTableSchemaColumns = {}
     for field in schema:
         result[field.name] = {
             "name": field.name,
             "nullable": field.nullable,
-            **_get_column_type_from_py_arrow(field.type),
+            **get_column_type_from_py_arrow(field.type),
         }
     return result
 
 
-def get_row_count(parquet_file: TFileOrPath) -> int:
-    """Get the number of rows in a parquet file.
+def get_parquet_metadata(parquet_file: TFileOrPath) -> Tuple[int, pyarrow.Schema]:
+    """Gets parquet file metadata (including row count and schema)
 
     Args:
         parquet_file (str): path to parquet file
 
     Returns:
-        int: number of rows
+        FileMetaData: file metadata
     """
     with pyarrow.parquet.ParquetFile(parquet_file) as reader:
-        return reader.metadata.num_rows  # type: ignore[no-any-return]
+        return reader.metadata.num_rows, reader.schema_arrow
 
 
 def is_arrow_item(item: Any) -> bool:
     return isinstance(item, (pyarrow.Table, pyarrow.RecordBatch))
 
 
 def to_arrow_scalar(value: Any, arrow_type: pyarrow.DataType) -> Any:
```

### Comparing `dlt-0.4.8a1/dlt/common/libs/pydantic.py` & `dlt-0.4.9a0/dlt/common/libs/pydantic.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/libs/sql_alchemy.py` & `dlt-0.4.9a0/dlt/common/libs/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/logger.py` & `dlt-0.4.9a0/dlt/common/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/managed_thread_pool.py` & `dlt-0.4.9a0/dlt/common/managed_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/configuration.py` & `dlt-0.4.9a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/json/__init__.py` & `dlt-0.4.9a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/json/relational.py` & `dlt-0.4.9a0/dlt/common/normalizers/json/relational.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+from functools import lru_cache
 from typing import Dict, List, Mapping, Optional, Sequence, Tuple, cast, TypedDict, Any
-from dlt.common.data_types.typing import TDataType
+from dlt.common.json import json
 from dlt.common.normalizers.exceptions import InvalidJsonNormalizer
 from dlt.common.normalizers.typing import TJSONNormalizer
 from dlt.common.normalizers.utils import generate_dlt_id, DLT_ID_LENGTH_BYTES
 
 from dlt.common.typing import DictStrAny, DictStrStr, TDataItem, StrAny
 from dlt.common.schema import Schema
-from dlt.common.schema.typing import TColumnSchema, TColumnName, TSimpleRegex
-from dlt.common.schema.utils import column_name_validator
+from dlt.common.schema.typing import (
+    TTableSchema,
+    TColumnSchema,
+    TColumnName,
+    TSimpleRegex,
+    DLT_NAME_PREFIX,
+)
+from dlt.common.schema.utils import column_name_validator, get_validity_column_names
+from dlt.common.schema.exceptions import ColumnNameConflictException
 from dlt.common.utils import digest128, update_dict_nested
 from dlt.common.normalizers.json import (
     TNormalizedRowIterator,
     wrap_in_dict,
     DataItemNormalizer as DataItemNormalizerBase,
 )
 from dlt.common.validation import validate_dict
@@ -124,14 +132,26 @@
 
                 out_rec_row[child_name] = v
 
         norm_row_dicts(dict_row, _r_lvl)
         return cast(TDataItemRow, out_rec_row), out_rec_list
 
     @staticmethod
+    def get_row_hash(row: Dict[str, Any]) -> str:
+        """Returns hash of row.
+
+        Hash includes column names and values and is ordered by column name.
+        Excludes dlt system columns.
+        Can be used as deterministic row identifier.
+        """
+        row_filtered = {k: v for k, v in row.items() if not k.startswith(DLT_NAME_PREFIX)}
+        row_str = json.dumps(row_filtered, sort_keys=True)
+        return digest128(row_str, DLT_ID_LENGTH_BYTES)
+
+    @staticmethod
     def _get_child_row_hash(parent_row_id: str, child_table: str, list_idx: int) -> str:
         # create deterministic unique id of the child row taking into account that all lists are ordered
         # and all child tables must be lists
         return digest128(f"{parent_row_id}_{child_table}_{list_idx}", DLT_ID_LENGTH_BYTES)
 
     @staticmethod
     def _link_row(row: TDataItemRowChild, parent_row_id: str, list_idx: int) -> TDataItemRowChild:
@@ -216,18 +236,22 @@
         dict_row: TDataItemRow,
         extend: DictStrAny,
         ident_path: Tuple[str, ...],
         parent_path: Tuple[str, ...] = (),
         parent_row_id: Optional[str] = None,
         pos: Optional[int] = None,
         _r_lvl: int = 0,
+        row_hash: bool = False,
     ) -> TNormalizedRowIterator:
         schema = self.schema
         table = schema.naming.shorten_fragments(*parent_path, *ident_path)
-
+        # compute row hash and set as row id
+        if row_hash:
+            row_id = self.get_row_hash(dict_row)  # type: ignore[arg-type]
+            dict_row["_dlt_id"] = row_id
         # flatten current row and extract all lists to recur into
         flattened_row, lists = self._flatten(table, dict_row, _r_lvl)
         # always extend row
         DataItemNormalizer._extend_row(extend, flattened_row)
         # infer record hash or leave existing primary key if present
         row_id = flattened_row.get("_dlt_id", None)
         if not row_id:
@@ -292,18 +316,26 @@
         # wrap items that are not dictionaries in dictionary, otherwise they cannot be processed by the JSON normalizer
         if not isinstance(item, dict):
             item = wrap_in_dict(item)
         # we will extend event with all the fields necessary to load it as root row
         row = cast(TDataItemRowRoot, item)
         # identify load id if loaded data must be processed after loading incrementally
         row["_dlt_load_id"] = load_id
+        # determine if row hash should be used as dlt id
+        row_hash = False
+        if self._is_scd2_table(self.schema, table_name):
+            row_hash = self._dlt_id_is_row_hash(self.schema, table_name)
+            self._validate_validity_column_names(
+                self._get_validity_column_names(self.schema, table_name), item
+            )
         yield from self._normalize_row(
             cast(TDataItemRowChild, row),
             {},
             (self.schema.naming.normalize_table_identifier(table_name),),
+            row_hash=row_hash,
         )
 
     @classmethod
     def ensure_this_normalizer(cls, norm_config: TJSONNormalizer) -> None:
         # make sure schema has right normalizer
         present_normalizer = norm_config["module"]
         if present_normalizer != __name__:
@@ -329,7 +361,37 @@
     def _validate_normalizer_config(schema: Schema, config: RelationalNormalizerConfig) -> None:
         validate_dict(
             RelationalNormalizerConfig,
             config,
             "./normalizers/json/config",
             validator_f=column_name_validator(schema.naming),
         )
+
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def _is_scd2_table(schema: Schema, table_name: str) -> bool:
+        if table_name in schema.data_table_names():
+            if schema.get_table(table_name).get("x-merge-strategy") == "scd2":
+                return True
+        return False
+
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def _get_validity_column_names(schema: Schema, table_name: str) -> List[Optional[str]]:
+        return get_validity_column_names(schema.get_table(table_name))
+
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def _dlt_id_is_row_hash(schema: Schema, table_name: str) -> bool:
+        return schema.get_table(table_name)["columns"].get("_dlt_id", dict()).get("x-row-version", False)  # type: ignore[return-value]
+
+    @staticmethod
+    def _validate_validity_column_names(
+        validity_column_names: List[Optional[str]], item: TDataItem
+    ) -> None:
+        """Raises exception if configured validity column name appears in data item."""
+        for validity_column_name in validity_column_names:
+            if validity_column_name in item.keys():
+                raise ColumnNameConflictException(
+                    "Found column in data item with same name as validity column"
+                    f' "{validity_column_name}".'
+                )
```

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/naming/direct.py` & `dlt-0.4.9a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.4.9a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.4.9a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/naming/naming.py` & `dlt-0.4.9a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.4.9a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/normalizers/utils.py` & `dlt-0.4.9a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/pipeline.py` & `dlt-0.4.9a0/dlt/common/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,20 @@
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.configuration.paths import get_dlt_data_dir
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.destination import TDestinationReferenceArg, TDestination
 from dlt.common.destination.exceptions import DestinationHasFailedJobs
 from dlt.common.exceptions import PipelineStateNotAvailable, SourceSectionNotAvailable
 from dlt.common.schema import Schema
-from dlt.common.schema.typing import TColumnNames, TColumnSchema, TWriteDisposition, TSchemaContract
+from dlt.common.schema.typing import (
+    TColumnNames,
+    TColumnSchema,
+    TWriteDispositionConfig,
+    TSchemaContract,
+)
 from dlt.common.source import get_current_pipe_name
 from dlt.common.storages.load_storage import LoadPackageInfo
 from dlt.common.time import ensure_pendulum_datetime, precise_time
 from dlt.common.typing import DictStrAny, REPattern, StrAny, SupportsHumanize
 from dlt.common.jsonpath import delete_matches, TAnyJsonPath
 from dlt.common.data_writers.writers import DataWriterMetrics, TLoaderFileFormat
 from dlt.common.utils import RowCounts, merge_row_counts
@@ -517,15 +522,15 @@
         self,
         data: Any = None,
         *,
         destination: TDestinationReferenceArg = None,
         dataset_name: str = None,
         credentials: Any = None,
         table_name: str = None,
-        write_disposition: TWriteDisposition = None,
+        write_disposition: TWriteDispositionConfig = None,
         columns: Sequence[TColumnSchema] = None,
         primary_key: TColumnNames = None,
         schema: Schema = None,
         loader_file_format: TLoaderFileFormat = None,
         schema_contract: TSchemaContract = None,
     ) -> LoadInfo: ...
 
@@ -540,15 +545,15 @@
     def __call__(
         self,
         *,
         destination: TDestinationReferenceArg = None,
         dataset_name: str = None,
         credentials: Any = None,
         table_name: str = None,
-        write_disposition: TWriteDisposition = None,
+        write_disposition: TWriteDispositionConfig = None,
         columns: Sequence[TColumnSchema] = None,
         schema: Schema = None,
         loader_file_format: TLoaderFileFormat = None,
         schema_contract: TSchemaContract = None,
     ) -> LoadInfo: ...
```

### Comparing `dlt-0.4.8a1/dlt/common/reflection/spec.py` & `dlt-0.4.9a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/reflection/utils.py` & `dlt-0.4.9a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runners/configuration.py` & `dlt-0.4.9a0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runners/pool_runner.py` & `dlt-0.4.9a0/dlt/common/runners/pool_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 import multiprocessing
 from typing import Callable, Union, cast, TypeVar
 from concurrent.futures import Executor, ProcessPoolExecutor, ThreadPoolExecutor, Future
 from typing_extensions import ParamSpec
 
-from dlt.common import logger, sleep
+from dlt.common import logger
 from dlt.common.configuration.container import Container
 from dlt.common.runtime import init
 from dlt.common.runners.runnable import Runnable, TExecutor
 from dlt.common.runners.configuration import PoolRunnerConfiguration
 from dlt.common.runners.typing import TRunMetrics
 from dlt.common.runtime import signals
+from dlt.common.runtime.signals import sleep
 from dlt.common.exceptions import SignalReceivedException
 
 
 T = TypeVar("T")
 P = ParamSpec("P")
```

### Comparing `dlt-0.4.8a1/dlt/common/runners/runnable.py` & `dlt-0.4.9a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runners/stdout.py` & `dlt-0.4.9a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runners/synth_pickle.py` & `dlt-0.4.9a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runners/venv.py` & `dlt-0.4.9a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runtime/collector.py` & `dlt-0.4.9a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runtime/exec_info.py` & `dlt-0.4.9a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runtime/init.py` & `dlt-0.4.9a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runtime/json_logging.py` & `dlt-0.4.9a0/dlt/common/runtime/json_logging.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runtime/prometheus.py` & `dlt-0.4.9a0/dlt/common/runtime/prometheus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Iterable
 from prometheus_client import Gauge
 from prometheus_client.metrics import MetricWrapperBase
 
 from dlt.common.configuration.specs import RunConfiguration
-from dlt.common import logger
 from dlt.common.runtime.exec_info import dlt_version_info
 from dlt.common.typing import DictStrAny, StrAny
 
 
 # def init_prometheus(config: RunConfiguration) -> None:
 #         from prometheus_client import start_http_server, Info
```

### Comparing `dlt-0.4.8a1/dlt/common/runtime/segment.py` & `dlt-0.4.9a0/dlt/common/runtime/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 # several code fragments come from https://github.com/RasaHQ/rasa/blob/main/rasa/telemetry.py
 import os
 
 import atexit
 import base64
 import requests
-from concurrent.futures import ThreadPoolExecutor
 from typing import Literal, Optional
 from dlt.common.configuration.paths import get_dlt_data_dir
 
 from dlt.common import logger
 from dlt.common.managed_thread_pool import ManagedThreadPool
-
 from dlt.common.configuration.specs import RunConfiguration
 from dlt.common.runtime.exec_info import get_execution_context, TExecutionContext
 from dlt.common.typing import DictStrAny, StrAny
 from dlt.common.utils import uniq_id
 from dlt.version import __version__
 
 TEventCategory = Literal["pipeline", "command", "helper"]
```

### Comparing `dlt-0.4.8a1/dlt/common/runtime/sentry.py` & `dlt-0.4.9a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runtime/signals.py` & `dlt-0.4.9a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runtime/slack.py` & `dlt-0.4.9a0/dlt/common/runtime/slack.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 
 
 def send_slack_message(incoming_hook: str, message: str, is_markdown: bool = True) -> None:
-    from dlt.common import json, logger
+    from dlt.common import logger
+    from dlt.common.json import json
 
     """Sends a `message` to  Slack `incoming_hook`, by default formatted as markdown."""
     r = requests.post(
         incoming_hook,
         data=json.dumps({"text": message, "mrkdwn": is_markdown}).encode("utf-8"),
         headers={"Content-Type": "application/json;charset=utf-8"},
     )
```

### Comparing `dlt-0.4.8a1/dlt/common/runtime/telemetry.py` & `dlt-0.4.9a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/runtime/typing.py` & `dlt-0.4.9a0/dlt/common/runtime/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/schema/__init__.py` & `dlt-0.4.9a0/dlt/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/schema/detections.py` & `dlt-0.4.9a0/dlt/common/schema/detections.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime  # noqa: 251
 from typing import Any, Optional, Type
 
 from hexbytes import HexBytes
 
-from dlt.common import pendulum, Wei
+from dlt.common.pendulum import pendulum
+from dlt.common.wei import Wei
 from dlt.common.data_types import TDataType
 from dlt.common.time import parse_iso_like_datetime
 
 
 _NOW_TS: float = pendulum.now().timestamp()
 _FLOAT_TS_RANGE = 5 * 31536000.0  # seconds in year
```

### Comparing `dlt-0.4.8a1/dlt/common/schema/exceptions.py` & `dlt-0.4.9a0/dlt/common/schema/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,7 +148,11 @@
         self.data_item = data_item
 
 
 class UnknownTableException(SchemaException):
     def __init__(self, table_name: str) -> None:
         self.table_name = table_name
         super().__init__(f"Trying to access unknown table {table_name}.")
+
+
+class ColumnNameConflictException(SchemaException):
+    pass
```

### Comparing `dlt-0.4.8a1/dlt/common/schema/migrations.py` & `dlt-0.4.9a0/dlt/common/schema/migrations.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/schema/schema.py` & `dlt-0.4.9a0/dlt/common/schema/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from copy import copy, deepcopy
 from typing import ClassVar, Dict, List, Mapping, Optional, Sequence, Tuple, Any, cast, Literal
-from dlt.common import json
 from dlt.common.schema.migrations import migrate_schema
 
 from dlt.common.utils import extend_list_deduplicated
 from dlt.common.typing import (
     DictStrAny,
     StrAny,
     REPattern,
```

### Comparing `dlt-0.4.8a1/dlt/common/schema/typing.py` & `dlt-0.4.9a0/dlt/common/schema/typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
     Callable,
     Dict,
     List,
     Literal,
     Optional,
     Sequence,
     Set,
-    Tuple,
     Type,
     TypedDict,
     NewType,
     Union,
     get_args,
 )
 from typing_extensions import Never
@@ -30,14 +29,16 @@
 SCHEMA_ENGINE_VERSION = 9
 
 # dlt tables
 VERSION_TABLE_NAME = "_dlt_version"
 LOADS_TABLE_NAME = "_dlt_loads"
 STATE_TABLE_NAME = "_dlt_pipeline_state"
 DLT_NAME_PREFIX = "_dlt"
+DEFAULT_VALIDITY_COLUMN_NAMES = ["_dlt_valid_from", "_dlt_valid_to"]
+"""Default values for validity column names used in `scd2` merge strategy."""
 
 TColumnProp = Literal[
     "name",
     "data_type",
     "nullable",
     "partition",
     "cluster",
@@ -60,15 +61,14 @@
     "sort",
     "unique",
     "root_key",
     "merge_key",
     "dedup_sort",
 ]
 """Known hints of a column used to declare hint regexes."""
-TWriteDisposition = Literal["skip", "append", "replace", "merge"]
 TTableFormat = Literal["iceberg", "parquet", "jsonl"]
 TTypeDetections = Literal[
     "timestamp", "iso_timestamp", "iso_date", "large_integer", "hexbytes_to_text", "wei_to_double"
 ]
 TTypeDetectionFunc = Callable[[Type[Any], Any], Optional[TDataType]]
 TColumnNames = Union[str, Sequence[str]]
 """A string representing a column name or a list of"""
@@ -82,15 +82,14 @@
         "foreign_key",
         "sort",
         "unique",
         "merge_key",
         "root_key",
     ]
 )
-WRITE_DISPOSITIONS: Set[TWriteDisposition] = set(get_args(TWriteDisposition))
 
 
 class TColumnType(TypedDict, total=False):
     data_type: Optional[TDataType]
     precision: Optional[int]
     scale: Optional[int]
 
@@ -151,14 +150,35 @@
     includes: Optional[List[TSimpleRegex]]
 
 
 class NormalizerInfo(TypedDict, total=True):
     new_table: bool
 
 
+TWriteDisposition = Literal["skip", "append", "replace", "merge"]
+TLoaderMergeStrategy = Literal["delete-insert", "scd2"]
+
+
+WRITE_DISPOSITIONS: Set[TWriteDisposition] = set(get_args(TWriteDisposition))
+MERGE_STRATEGIES: Set[TLoaderMergeStrategy] = set(get_args(TLoaderMergeStrategy))
+
+
+class TWriteDispositionDict(TypedDict):
+    disposition: TWriteDisposition
+
+
+class TMergeDispositionDict(TWriteDispositionDict, total=False):
+    strategy: Optional[TLoaderMergeStrategy]
+    validity_column_names: Optional[List[str]]
+    row_version_column_name: Optional[str]
+
+
+TWriteDispositionConfig = Union[TWriteDisposition, TWriteDispositionDict, TMergeDispositionDict]
+
+
 # TypedDict that defines properties of a table
 
 
 class TTableSchema(TypedDict, total=False):
     """TypedDict that defines properties of a table"""
 
     name: Optional[str]
```

### Comparing `dlt-0.4.8a1/dlt/common/schema/utils.py` & `dlt-0.4.9a0/dlt/common/schema/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import base64
 import hashlib
 import yaml
 from copy import deepcopy, copy
 from typing import Dict, List, Sequence, Tuple, Type, Any, cast, Iterable, Optional, Union
 
-from dlt.common import json
+from dlt.common.json import json
 from dlt.common.data_types import TDataType
 from dlt.common.exceptions import DictValidationException
 from dlt.common.normalizers.naming import NamingConvention
 from dlt.common.normalizers.naming.snake_case import NamingConvention as SnakeCase
 from dlt.common.typing import DictStrAny, REPattern
 from dlt.common.validation import TCustomValidator, validate_dict_ignoring_xkeys
 from dlt.common.schema import detections
@@ -30,27 +30,29 @@
     TColumnSchema,
     TColumnProp,
     TTableFormat,
     TColumnHint,
     TTypeDetectionFunc,
     TTypeDetections,
     TWriteDisposition,
+    TLoaderMergeStrategy,
     TSchemaContract,
     TSortOrder,
 )
 from dlt.common.schema.exceptions import (
     CannotCoerceColumnException,
     ParentTableNotFoundException,
     TablePropertiesConflictException,
     InvalidSchemaName,
 )
 
 
 RE_NON_ALPHANUMERIC_UNDERSCORE = re.compile(r"[^a-zA-Z\d_]")
 DEFAULT_WRITE_DISPOSITION: TWriteDisposition = "append"
+DEFAULT_MERGE_STRATEGY: TLoaderMergeStrategy = "delete-insert"
 
 
 def is_valid_schema_name(name: str) -> bool:
     """Schema name must be a valid python identifier and have max len of 64"""
     return (
         name is not None
         and name.isidentifier()
@@ -512,14 +514,21 @@
     dedup_sort_col = get_first_column_name_with_prop(table, "dedup_sort", include_incomplete)
     if dedup_sort_col is None:
         return None
     dedup_sort_order = table["columns"][dedup_sort_col]["dedup_sort"]
     return (dedup_sort_col, dedup_sort_order)
 
 
+def get_validity_column_names(table: TTableSchema) -> List[Optional[str]]:
+    return [
+        get_first_column_name_with_prop(table, "x-valid-from"),
+        get_first_column_name_with_prop(table, "x-valid-to"),
+    ]
+
+
 def merge_schema_updates(schema_updates: Sequence[TSchemaUpdate]) -> TSchemaTables:
     aggregated_update: TSchemaTables = {}
     for schema_update in schema_updates:
         for table_name, table_updates in schema_update.items():
             for partial_table in table_updates:
                 # aggregate schema updates
                 aggregated_table = aggregated_update.setdefault(table_name, partial_table)
@@ -709,19 +718,25 @@
     return table
 
 
 def new_column(
     column_name: str,
     data_type: TDataType = None,
     nullable: bool = True,
+    precision: int = None,
+    scale: int = None,
     validate_schema: bool = False,
 ) -> TColumnSchema:
     column: TColumnSchema = {"name": column_name, "nullable": nullable}
     if data_type:
         column["data_type"] = data_type
+    if precision is not None:
+        column["precision"] = precision
+    if scale is not None:
+        column["scale"] = scale
     if validate_schema:
         validate_dict_ignoring_xkeys(
             spec=TColumnSchema,
             doc=column,
             path=f"new_column/{column_name}",
         )
```

### Comparing `dlt-0.4.8a1/dlt/common/source.py` & `dlt-0.4.9a0/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/storages/__init__.py` & `dlt-0.4.9a0/dlt/common/storages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .normalize_storage import NormalizeStorage
 from .load_package import (
     ParsedLoadJobFileName,
     LoadJobInfo,
     LoadPackageInfo,
     PackageStorage,
     TJobState,
+    create_load_id,
 )
 from .data_item_storage import DataItemStorage
 from .load_storage import LoadStorage
 from .configuration import (
     LoadStorageConfiguration,
     NormalizeStorageConfiguration,
     SchemaStorageConfiguration,
@@ -36,10 +37,11 @@
     "TSchemaFileFormat",
     "FilesystemConfiguration",
     "ParsedLoadJobFileName",
     "LoadJobInfo",
     "LoadPackageInfo",
     "PackageStorage",
     "TJobState",
+    "create_load_id",
     "fsspec_from_config",
     "fsspec_filesystem",
 ]
```

### Comparing `dlt-0.4.8a1/dlt/common/storages/configuration.py` & `dlt-0.4.9a0/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/storages/data_item_storage.py` & `dlt-0.4.9a0/dlt/common/storages/data_item_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from pathlib import Path
 from typing import Dict, Any, List, Sequence
 from abc import ABC, abstractmethod
 
 from dlt.common import logger
-from dlt.common.destination import TLoaderFileFormat
 from dlt.common.schema import TTableSchemaColumns
 from dlt.common.typing import StrAny, TDataItems
-from dlt.common.data_writers import BufferedDataWriter, DataWriter, DataWriterMetrics
+from dlt.common.data_writers import (
+    BufferedDataWriter,
+    DataWriter,
+    DataWriterMetrics,
+    FileWriterSpec,
+)
 
 
 class DataItemStorage(ABC):
-    def __init__(self, load_file_type: TLoaderFileFormat, *args: Any) -> None:
-        self.loader_file_format = load_file_type
+    def __init__(self, writer_spec: FileWriterSpec, *args: Any) -> None:
+        self.writer_spec = writer_spec
+        self.writer_cls = DataWriter.class_factory(
+            writer_spec.file_format, writer_spec.data_item_format
+        )
         self.buffered_writers: Dict[str, BufferedDataWriter[DataWriter]] = {}
         super().__init__(*args)
 
     def _get_writer(
         self, load_id: str, schema_name: str, table_name: str
     ) -> BufferedDataWriter[DataWriter]:
         # unique writer id
         writer_id = f"{load_id}.{schema_name}.{table_name}"
         writer = self.buffered_writers.get(writer_id, None)
         if not writer:
             # assign a writer for each table
             path = self._get_data_item_path_template(load_id, schema_name, table_name)
-            writer = BufferedDataWriter(self.loader_file_format, path)
+            writer = BufferedDataWriter(self.writer_spec, path)
             self.buffered_writers[writer_id] = writer
         return writer
 
     def write_data_item(
         self,
         load_id: str,
         schema_name: str,
@@ -61,23 +68,25 @@
 
         The preferred import method is a hard link to avoid copying the data. If current filesystem does not
         support it, a regular copy is used.
         """
         writer = self._get_writer(load_id, schema_name, table_name)
         return writer.import_file(file_path, metrics)
 
-    def close_writers(self, load_id: str) -> None:
-        # flush and close all files
+    def close_writers(self, load_id: str, skip_flush: bool = False) -> None:
+        """Flush, write footers (skip_flush), write metrics and close files in all
+        writers belonging to `load_id` package
+        """
         for name, writer in self.buffered_writers.items():
             if name.startswith(load_id) and not writer.closed:
                 logger.debug(
                     f"Closing writer for {name} with file {writer._file} and actual name"
                     f" {writer._file_name}"
                 )
-                writer.close()
+                writer.close(skip_flush=skip_flush)
 
     def closed_files(self, load_id: str) -> List[DataWriterMetrics]:
         """Return metrics for all fully processed (closed) files"""
         files: List[DataWriterMetrics] = []
         for name, writer in self.buffered_writers.items():
             if name.startswith(load_id):
                 files.extend(writer.closed_files)
@@ -86,32 +95,11 @@
 
     def remove_closed_files(self, load_id: str) -> None:
         """Remove metrics for closed files in a given `load_id`"""
         for name, writer in self.buffered_writers.items():
             if name.startswith(load_id):
                 writer.closed_files.clear()
 
-    def _write_temp_job_file(
-        self,
-        load_id: str,
-        table_name: str,
-        table: TTableSchemaColumns,
-        file_id: str,
-        rows: Sequence[StrAny],
-    ) -> str:
-        """Writes new file into new packages "new_jobs". Intended for testing"""
-        file_name = (
-            self._get_data_item_path_template(load_id, None, table_name) % file_id
-            + "."
-            + self.loader_file_format
-        )
-        format_spec = DataWriter.data_format_from_file_format(self.loader_file_format)
-        mode = "wb" if format_spec.is_binary_format else "w"
-        with self.storage.open_file(file_name, mode=mode) as f:  # type: ignore[attr-defined]
-            writer = DataWriter.from_file_format(self.loader_file_format, f)
-            writer.write_all(table, rows)
-        return Path(file_name).name
-
     @abstractmethod
     def _get_data_item_path_template(self, load_id: str, schema_name: str, table_name: str) -> str:
         """Returns a file template for item writer. note: use %s for file id to create required template format"""
         pass
```

### Comparing `dlt-0.4.8a1/dlt/common/storages/exceptions.py` & `dlt-0.4.9a0/dlt/common/storages/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import semver
 from typing import Iterable
 
 from dlt.common.exceptions import DltException, TerminalValueError
-from dlt.common.destination import TLoaderFileFormat
 
 
 class StorageException(DltException):
     def __init__(self, msg: str) -> None:
         super().__init__(msg)
 
 
@@ -59,24 +58,22 @@
         )
 
 
 class LoadStorageException(StorageException):
     pass
 
 
-class JobWithUnsupportedWriterException(LoadStorageException, TerminalValueError):
-    def __init__(
-        self, load_id: str, expected_file_formats: Iterable[TLoaderFileFormat], wrong_job: str
-    ) -> None:
+class JobFileFormatUnsupported(LoadStorageException, TerminalValueError):
+    def __init__(self, load_id: str, supported_formats: Iterable[str], wrong_job: str) -> None:
         self.load_id = load_id
-        self.expected_file_formats = expected_file_formats
+        self.expected_file_formats = supported_formats
         self.wrong_job = wrong_job
         super().__init__(
-            f"Job {wrong_job} for load id {load_id} requires loader file format that is not one of"
-            f" {expected_file_formats}"
+            f"Job {wrong_job} for load id {load_id} requires job file format that is not one of"
+            f" {supported_formats}"
         )
 
 
 class LoadPackageNotFound(LoadStorageException, FileNotFoundError):
     def __init__(self, load_id: str) -> None:
         self.load_id = load_id
         super().__init__(f"Package with load id {load_id} could not be found")
```

### Comparing `dlt-0.4.8a1/dlt/common/storages/file_storage.py` & `dlt-0.4.9a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/storages/fsspec_filesystem.py` & `dlt-0.4.9a0/dlt/common/storages/fsspec_filesystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 from urllib.parse import urlparse
 
 from fsspec import AbstractFileSystem, register_implementation
 from fsspec.core import url_to_fs
 
 from dlt import version
-from dlt.common import pendulum
+from dlt.common.pendulum import pendulum
 from dlt.common.configuration.specs import (
     GcpCredentials,
     AwsCredentials,
     AzureCredentials,
 )
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.storages.configuration import FileSystemCredentials, FilesystemConfiguration
```

### Comparing `dlt-0.4.8a1/dlt/common/storages/fsspecs/google_drive.py` & `dlt-0.4.9a0/dlt/common/storages/fsspecs/google_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import posixpath
 from typing import Any, Dict, List, Literal, Optional, Tuple
 
-from dlt.common import json
+from dlt.common.json import json
 from dlt.common.configuration.specs import GcpCredentials, GcpOAuthCredentials
 from dlt.common.exceptions import MissingDependencyException
 
 from fsspec.spec import AbstractFileSystem, AbstractBufferedFile
 
 try:
     from googleapiclient.discovery import build
```

### Comparing `dlt-0.4.8a1/dlt/common/storages/live_schema_storage.py` & `dlt-0.4.9a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/storages/load_package.py` & `dlt-0.4.9a0/dlt/common/storages/load_package.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,61 +17,65 @@
     Optional,
     Sequence,
     Set,
     get_args,
     cast,
     Any,
     Tuple,
-    TYPE_CHECKING,
     TypedDict,
 )
+from typing_extensions import NotRequired
 
-from dlt.common import pendulum, json
-
+from dlt.common.pendulum import pendulum
+from dlt.common.json import json
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import ContainerInjectableContext
 from dlt.common.configuration.exceptions import ContextDefaultCannotBeCreated
 from dlt.common.configuration.container import Container
-
 from dlt.common.data_writers import DataWriter, new_file_id
 from dlt.common.destination import TLoaderFileFormat
 from dlt.common.exceptions import TerminalValueError
 from dlt.common.schema import Schema, TSchemaTables
 from dlt.common.schema.typing import TStoredSchema, TTableSchemaColumns
 from dlt.common.storages import FileStorage
 from dlt.common.storages.exceptions import LoadPackageNotFound, CurrentLoadPackageStateNotAvailable
 from dlt.common.typing import DictStrAny, SupportsHumanize
 from dlt.common.utils import flatten_list_or_items
 from dlt.common.versioned_state import (
     generate_state_version_hash,
     bump_state_version_if_modified,
     TVersionedState,
     default_versioned_state,
+    json_decode_state,
+    json_encode_state,
 )
-from typing_extensions import NotRequired
+from dlt.common.time import precise_time
+
+TJobFileFormat = Literal["sql", "reference", TLoaderFileFormat]
+"""Loader file formats with internal job types"""
 
 
 class TLoadPackageState(TVersionedState, total=False):
-    created_at: str
-    """Timestamp when the loadpackage was created"""
+    created_at: DateTime
+    """Timestamp when the load package was created"""
 
     """A section of state that does not participate in change merging and version control"""
     destination_state: NotRequired[Dict[str, Any]]
     """private space for destinations to store state relevant only to the load package"""
 
 
 class TLoadPackage(TypedDict, total=False):
     load_id: str
     """Load id"""
     state: TLoadPackageState
     """State of the load package"""
 
 
 # allows to upgrade state when restored with a new version of state logic/schema
-LOADPACKAGE_STATE_ENGINE_VERSION = 1
+LOAD_PACKAGE_STATE_ENGINE_VERSION = 1
 
 
 def generate_loadpackage_state_version_hash(state: TLoadPackageState) -> str:
     return generate_state_version_hash(state)
 
 
 def bump_loadpackage_state_version_if_modified(state: TLoadPackageState) -> Tuple[int, str, str]:
@@ -93,18 +97,28 @@
     state["_state_engine_version"] = from_engine
     return cast(TLoadPackageState, state)
 
 
 def default_load_package_state() -> TLoadPackageState:
     return {
         **default_versioned_state(),
-        "_state_engine_version": LOADPACKAGE_STATE_ENGINE_VERSION,
+        "_state_engine_version": LOAD_PACKAGE_STATE_ENGINE_VERSION,
     }
 
 
+def create_load_id() -> str:
+    """Creates new package load id which is the current unix timestamp converted to string.
+    Load ids must have the following properties:
+    - They must maintain increase order over time for a particular dlt schema loaded to particular destination and dataset
+    `dlt` executes packages in order of load ids
+    `dlt` considers a state with the highest load id to be the most up to date when restoring state from destination
+    """
+    return str(precise_time())
+
+
 # folders to manage load jobs in a single load package
 TJobState = Literal["new_jobs", "failed_jobs", "started_jobs", "completed_jobs"]
 WORKING_FOLDERS: Set[TJobState] = set(get_args(TJobState))
 TLoadPackageStatus = Literal["new", "extracted", "normalized", "loaded", "aborted"]
 
 
 class ParsedLoadJobFileName(NamedTuple):
@@ -112,15 +126,15 @@
     and a 5 bytes random string to make job file name unique.
     The job id does not contain retry count and is immutable during loading of the data
     """
 
     table_name: str
     file_id: str
     retry_count: int
-    file_format: TLoaderFileFormat
+    file_format: TJobFileFormat
 
     def job_id(self) -> str:
         """Unique identifier of the job"""
         return f"{self.table_name}.{self.file_id}.{self.file_format}"
 
     def file_name(self) -> str:
         """A name of the file with the data to be loaded"""
@@ -134,15 +148,15 @@
     def parse(file_name: str) -> "ParsedLoadJobFileName":
         p = Path(file_name)
         parts = p.name.split(".")
         if len(parts) != 4:
             raise TerminalValueError(parts)
 
         return ParsedLoadJobFileName(
-            parts[0], parts[1], int(parts[2]), cast(TLoaderFileFormat, parts[3])
+            parts[0], parts[1], int(parts[2]), cast(TJobFileFormat, parts[3])
         )
 
     @staticmethod
     def new_file_id() -> str:
         return new_file_id()
 
     def __str__(self) -> str:
@@ -397,34 +411,40 @@
             file_name,
         )
 
     #
     # Create and drop entities
     #
 
-    def create_package(self, load_id: str) -> None:
+    def create_package(self, load_id: str, initial_state: TLoadPackageState = None) -> None:
         self.storage.create_folder(load_id)
         # create processing directories
         self.storage.create_folder(os.path.join(load_id, PackageStorage.NEW_JOBS_FOLDER))
         self.storage.create_folder(os.path.join(load_id, PackageStorage.COMPLETED_JOBS_FOLDER))
         self.storage.create_folder(os.path.join(load_id, PackageStorage.FAILED_JOBS_FOLDER))
         self.storage.create_folder(os.path.join(load_id, PackageStorage.STARTED_JOBS_FOLDER))
-        # ensure created timestamp is set in state when load package is created
-        state = self.get_load_package_state(load_id)
+        # use initial state or create a new by loading non existing state
+        state = self.get_load_package_state(load_id) if initial_state is None else initial_state
         if not state.get("created_at"):
-            state["created_at"] = pendulum.now().to_iso8601_string()
-            self.save_load_package_state(load_id, state)
+            # try to parse load_id as unix timestamp
+            try:
+                created_at = float(load_id)
+            except Exception:
+                created_at = precise_time()
+            state["created_at"] = pendulum.from_timestamp(created_at)
+        self.save_load_package_state(load_id, state)
 
     def complete_loading_package(self, load_id: str, load_state: TLoadPackageStatus) -> str:
         """Completes loading the package by writing marker file with`package_state. Returns path to the completed package"""
         load_path = self.get_package_path(load_id)
         # save marker file
         self.storage.save(
             os.path.join(load_path, PackageStorage.PACKAGE_COMPLETED_FILE_NAME), load_state
         )
+        # TODO: also modify state
         return load_path
 
     def remove_completed_jobs(self, load_id: str) -> None:
         """Deletes completed jobs. If package has failed jobs, nothing gets deleted."""
         has_failed_jobs = len(self.list_failed_jobs(load_id)) > 0
         # delete completed jobs
         if not has_failed_jobs:
@@ -465,29 +485,29 @@
     #
     def get_load_package_state(self, load_id: str) -> TLoadPackageState:
         package_path = self.get_package_path(load_id)
         if not self.storage.has_folder(package_path):
             raise LoadPackageNotFound(load_id)
         try:
             state_dump = self.storage.load(self.get_load_package_state_path(load_id))
-            state = json.loads(state_dump)
+            state = json_decode_state(state_dump)
             return migrate_load_package_state(
-                state, state["_state_engine_version"], LOADPACKAGE_STATE_ENGINE_VERSION
+                state, state["_state_engine_version"], LOAD_PACKAGE_STATE_ENGINE_VERSION
             )
         except FileNotFoundError:
             return default_load_package_state()
 
     def save_load_package_state(self, load_id: str, state: TLoadPackageState) -> None:
         package_path = self.get_package_path(load_id)
         if not self.storage.has_folder(package_path):
             raise LoadPackageNotFound(load_id)
         bump_loadpackage_state_version_if_modified(state)
         self.storage.save(
             self.get_load_package_state_path(load_id),
-            json.dumps(state),
+            json_encode_state(state),
         )
 
     def get_load_package_state_path(self, load_id: str) -> str:
         package_path = self.get_package_path(load_id)
         return os.path.join(package_path, PackageStorage.LOAD_PACKAGE_STATE_FILE_NAME)
 
     #
@@ -590,15 +610,15 @@
         validate_components: bool = True,
         loader_file_format: TLoaderFileFormat = None,
     ) -> str:
         if validate_components:
             FileStorage.validate_file_name_component(table_name)
         fn = f"{table_name}.{file_id}.{int(retry_count)}"
         if loader_file_format:
-            format_spec = DataWriter.data_format_from_file_format(loader_file_format)
+            format_spec = DataWriter.writer_spec_from_file_format(loader_file_format, "object")
             return fn + f".{format_spec.file_extension}"
         return fn
 
     @staticmethod
     def is_package_partially_loaded(package_info: LoadPackageInfo) -> bool:
         """Checks if package is partially loaded - has jobs that are not new."""
         if package_info.state == "normalized":
```

### Comparing `dlt-0.4.8a1/dlt/common/storages/load_storage.py` & `dlt-0.4.9a0/dlt/common/storages/load_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 from os.path import join
-from typing import Iterable, Optional, Sequence
+from typing import Iterable, List, Optional, Sequence
 
-from dlt.common.typing import DictStrAny
-from dlt.common import json
+from dlt.common.data_writers.exceptions import DataWriterNotFound
+from dlt.common.json import json
 from dlt.common.configuration import known_sections
 from dlt.common.configuration.inject import with_config
 from dlt.common.destination import ALL_SUPPORTED_FILE_FORMATS, TLoaderFileFormat
 from dlt.common.configuration.accessors import config
-from dlt.common.exceptions import TerminalValueError
 from dlt.common.schema import TSchemaTables
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.storages.configuration import LoadStorageConfiguration
 from dlt.common.storages.versioned_storage import VersionedStorage
 from dlt.common.storages.data_item_storage import DataItemStorage
 from dlt.common.storages.load_package import (
     LoadJobInfo,
     LoadPackageInfo,
     PackageStorage,
     ParsedLoadJobFileName,
     TJobState,
     TLoadPackageState,
+    TJobFileFormat,
 )
-from dlt.common.storages.exceptions import JobWithUnsupportedWriterException, LoadPackageNotFound
+from dlt.common.data_writers import DataWriter, FileWriterSpec, TDataItemFormat
+from dlt.common.storages.exceptions import JobFileFormatUnsupported, LoadPackageNotFound
 
 
-class LoadStorage(DataItemStorage, VersionedStorage):
+class LoadItemStorage(DataItemStorage):
+    def __init__(self, package_storage: PackageStorage, writer_spec: FileWriterSpec) -> None:
+        """Data item storage using `storage` to manage load packages"""
+        super().__init__(writer_spec)
+        self.package_storage = package_storage
+
+    def _get_data_item_path_template(self, load_id: str, _: str, table_name: str) -> str:
+        # implements DataItemStorage._get_data_item_path_template
+        file_name = PackageStorage.build_job_file_name(table_name, "%s")
+        file_path = self.package_storage.get_job_file_path(
+            load_id, PackageStorage.NEW_JOBS_FOLDER, file_name
+        )
+        return self.package_storage.storage.make_full_path(file_path)
+
+
+class LoadStorage(VersionedStorage):
     STORAGE_VERSION = "1.0.0"
     NORMALIZED_FOLDER = "normalized"  # folder within the volume where load packages are stored
     LOADED_FOLDER = "loaded"  # folder to keep the loads that were completely processed
     NEW_PACKAGES_FOLDER = "new"  # folder where new packages are created
 
     ALL_SUPPORTED_FILE_FORMATS = ALL_SUPPORTED_FILE_FORMATS
 
     @with_config(spec=LoadStorageConfiguration, sections=(known_sections.LOAD,))
     def __init__(
         self,
         is_owner: bool,
-        preferred_file_format: TLoaderFileFormat,
         supported_file_formats: Iterable[TLoaderFileFormat],
         config: LoadStorageConfiguration = config.value,
     ) -> None:
-        # puae-jsonl jobs have the extension .jsonl, so cater for this here
-        if supported_file_formats and "puae-jsonl" in supported_file_formats:
-            supported_file_formats = list(supported_file_formats)
-            supported_file_formats.append("jsonl")
-
-        if not LoadStorage.ALL_SUPPORTED_FILE_FORMATS.issuperset(supported_file_formats):
-            raise TerminalValueError(supported_file_formats)
-        if preferred_file_format and preferred_file_format not in supported_file_formats:
-            raise TerminalValueError(preferred_file_format)
-        self.supported_file_formats = supported_file_formats
+        self.supported_loader_file_formats = supported_file_formats
+        # store job file formats to add internal job formats as needed
+        self.supported_job_file_formats: List[TJobFileFormat] = list(supported_file_formats)
         self.config = config
         super().__init__(
-            preferred_file_format,
             LoadStorage.STORAGE_VERSION,
             is_owner,
             FileStorage(config.load_volume_path, "t", makedirs=is_owner),
         )
         if is_owner:
             self.initialize_storage()
         # create package storages
@@ -71,36 +78,59 @@
         )
 
     def initialize_storage(self) -> None:
         self.storage.create_folder(LoadStorage.NEW_PACKAGES_FOLDER, exists_ok=True)
         self.storage.create_folder(LoadStorage.NORMALIZED_FOLDER, exists_ok=True)
         self.storage.create_folder(LoadStorage.LOADED_FOLDER, exists_ok=True)
 
-    def _get_data_item_path_template(self, load_id: str, _: str, table_name: str) -> str:
-        # implements DataItemStorage._get_data_item_path_template
-        file_name = PackageStorage.build_job_file_name(table_name, "%s")
-        file_path = self.new_packages.get_job_file_path(
-            load_id, PackageStorage.NEW_JOBS_FOLDER, file_name
+    def create_item_storage(
+        self, preferred_format: TLoaderFileFormat, item_format: TDataItemFormat
+    ) -> DataItemStorage:
+        """Creates item storage for preferred_format + item_format combination. If not found, it
+        tries the remaining file formats in supported formats.
+        """
+        try:
+            return LoadItemStorage(
+                self.new_packages,
+                DataWriter.writer_spec_from_file_format(preferred_format, item_format),
+            )
+        except DataWriterNotFound:
+            for supported_format in self.supported_loader_file_formats:
+                if supported_format != preferred_format:
+                    try:
+                        return LoadItemStorage(
+                            self.new_packages,
+                            DataWriter.writer_spec_from_file_format(supported_format, item_format),
+                        )
+                    except DataWriterNotFound:
+                        pass
+            raise
+
+    def import_extracted_package(
+        self, load_id: str, extract_package_storage: PackageStorage
+    ) -> None:
+        # pass the original state
+        self.new_packages.create_package(
+            load_id, extract_package_storage.get_load_package_state(load_id)
         )
-        return self.new_packages.storage.make_full_path(file_path)
 
     def list_new_jobs(self, load_id: str) -> Sequence[str]:
         """Lists all jobs in new jobs folder of normalized package storage and checks if file formats are supported"""
         new_jobs = self.normalized_packages.list_new_jobs(load_id)
         # make sure all jobs have supported writers
         wrong_job = next(
             (
                 j
                 for j in new_jobs
-                if ParsedLoadJobFileName.parse(j).file_format not in self.supported_file_formats
+                if ParsedLoadJobFileName.parse(j).file_format not in self.supported_job_file_formats
             ),
             None,
         )
         if wrong_job is not None:
-            raise JobWithUnsupportedWriterException(load_id, self.supported_file_formats, wrong_job)
+            raise JobFileFormatUnsupported(load_id, self.supported_job_file_formats, wrong_job)
         return new_jobs
 
     def commit_new_load_package(self, load_id: str) -> None:
         self.storage.rename_tree(
             self.get_new_package_path(load_id), self.get_normalized_package_path(load_id)
         )
```

### Comparing `dlt-0.4.8a1/dlt/common/storages/normalize_storage.py` & `dlt-0.4.9a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/storages/schema_storage.py` & `dlt-0.4.9a0/dlt/common/storages/schema_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import yaml
 from typing import Iterator, List, Mapping, Tuple, cast
 
-from dlt.common import json, logger
+from dlt.common import logger
+from dlt.common.json import json
 from dlt.common.configuration import with_config
 from dlt.common.configuration.accessors import config
 from dlt.common.schema.utils import to_pretty_json, to_pretty_yaml
 from dlt.common.storages.configuration import (
     SchemaStorageConfiguration,
     TSchemaFileFormat,
     SchemaFileExtensions,
```

### Comparing `dlt-0.4.8a1/dlt/common/storages/transactional_file.py` & `dlt-0.4.9a0/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/storages/versioned_storage.py` & `dlt-0.4.9a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/time.py` & `dlt-0.4.9a0/dlt/common/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,16 @@
 
 def to_seconds(td: Optional[TimedeltaSeconds]) -> Optional[float]:
     if isinstance(td, timedelta):
         return td.total_seconds()
     return td
 
 
-T = TypeVar("T", bound=Union[pendulum.DateTime, pendulum.Time])
+TTimeWithPrecision = TypeVar("TTimeWithPrecision", bound=Union[pendulum.DateTime, pendulum.Time])
 
 
-def reduce_pendulum_datetime_precision(value: T, microsecond_precision: int) -> T:
-    if microsecond_precision >= 6:
+def reduce_pendulum_datetime_precision(
+    value: TTimeWithPrecision, precision: int
+) -> TTimeWithPrecision:
+    if precision >= 6:
         return value
-    return value.replace(microsecond=value.microsecond // 10 ** (6 - microsecond_precision) * 10 ** (6 - microsecond_precision))  # type: ignore
+    return value.replace(microsecond=value.microsecond // 10 ** (6 - precision) * 10 ** (6 - precision))  # type: ignore
```

### Comparing `dlt-0.4.8a1/dlt/common/typing.py` & `dlt-0.4.9a0/dlt/common/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
 
 def get_all_types_of_class_in_union(hint: Type[Any], cls: Type[TAny]) -> List[Type[TAny]]:
     # hint is an Union that contains classes, return all classes that are a subclass or superclass of cls
     return [
         t
         for t in get_args(hint)
-        if inspect.isclass(t) and (issubclass(t, cls) or issubclass(cls, t))
+        if not is_typeddict(t) and inspect.isclass(t) and (issubclass(t, cls) or issubclass(cls, t))
     ]
 
 
 def get_generic_type_argument_from_instance(
     instance: Any, sample_value: Optional[Any]
 ) -> Type[Any]:
     """Infers type argument of a Generic class from an `instance` of that class using optional `sample_value` of the argument type
```

### Comparing `dlt-0.4.8a1/dlt/common/utils.py` & `dlt-0.4.9a0/dlt/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         both_counter = isinstance(a, Counter) and isinstance(b, Counter)
         return both_mapping and not both_counter
 
     for key in src:
         if key in dst:
             if _is_recursive_merge(dst[key], src[key]):
                 # If the key for both `dst` and `src` are both Mapping types (e.g. dict), then recurse.
-                update_dict_nested(dst[key], src[key])
+                update_dict_nested(dst[key], src[key], keep_dst_values=keep_dst_values)
             elif dst[key] is src[key]:
                 # If a key exists in both objects and the values are `same`, the value from the `dst` object will be used.
                 pass
             else:
                 if not keep_dst_values:
                     # if not keep then overwrite
                     dst[key] = src[key]
```

### Comparing `dlt-0.4.8a1/dlt/common/validation.py` & `dlt-0.4.9a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/versioned_state.py` & `dlt-0.4.9a0/dlt/common/versioned_state.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import base64
 import hashlib
+import binascii
 from copy import copy
+from typing import TypedDict, List, Tuple, Mapping
 
-import datetime  # noqa: 251
-from dlt.common import json
-from typing import TypedDict, Dict, Any, List, Tuple, cast
+from dlt.common.json import json
+from dlt.common.typing import DictStrAny
+from dlt.common.utils import compressed_b64decode, compressed_b64encode
 
 
 class TVersionedState(TypedDict, total=False):
     _state_version: int
     _version_hash: str
     _state_engine_version: int
 
@@ -16,15 +18,15 @@
 def generate_state_version_hash(state: TVersionedState, exclude_attrs: List[str] = None) -> str:
     # generates hash out of stored schema content, excluding hash itself, version and local state
     state_copy = copy(state)
     exclude_attrs = exclude_attrs or []
     exclude_attrs.extend(["_state_version", "_state_engine_version", "_version_hash"])
     for attr in exclude_attrs:
         state_copy.pop(attr, None)  # type: ignore
-    content = json.typed_dumpb(state_copy, sort_keys=True)  # type: ignore
+    content = json.typed_dumpb(state_copy, sort_keys=True)
     h = hashlib.sha3_256(content)
     return base64.b64encode(h.digest()).decode("ascii")
 
 
 def bump_state_version_if_modified(
     state: TVersionedState, exclude_attrs: List[str] = None
 ) -> Tuple[int, str, str]:
@@ -39,7 +41,28 @@
 
     state["_version_hash"] = hash_
     return state["_state_version"], hash_, previous_hash
 
 
 def default_versioned_state() -> TVersionedState:
     return {"_state_version": 0, "_state_engine_version": 1}
+
+
+def json_encode_state(state: TVersionedState) -> str:
+    return json.typed_dumps(state)
+
+
+def json_decode_state(state_str: str) -> DictStrAny:
+    return json.typed_loads(state_str)  # type: ignore[no-any-return]
+
+
+def compress_state(state: TVersionedState) -> str:
+    return compressed_b64encode(json.typed_dumpb(state))
+
+
+def decompress_state(state_str: str) -> DictStrAny:
+    try:
+        state_bytes = compressed_b64decode(state_str)
+    except binascii.Error:
+        return json.typed_loads(state_str)  # type: ignore[no-any-return]
+    else:
+        return json.typed_loadb(state_bytes)  # type: ignore[no-any-return]
```

### Comparing `dlt-0.4.8a1/dlt/common/warnings.py` & `dlt-0.4.9a0/dlt/common/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/common/wei.py` & `dlt-0.4.9a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/__init__.py` & `dlt-0.4.9a0/dlt/destinations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from dlt.destinations.impl.redshift.factory import redshift
 from dlt.destinations.impl.qdrant.factory import qdrant
 from dlt.destinations.impl.motherduck.factory import motherduck
 from dlt.destinations.impl.weaviate.factory import weaviate
 from dlt.destinations.impl.destination.factory import destination
 from dlt.destinations.impl.synapse.factory import synapse
 from dlt.destinations.impl.databricks.factory import databricks
+from dlt.destinations.impl.dremio.factory import dremio
 
 
 __all__ = [
     "postgres",
     "snowflake",
     "filesystem",
     "duckdb",
@@ -26,9 +27,10 @@
     "athena",
     "redshift",
     "qdrant",
     "motherduck",
     "weaviate",
     "synapse",
     "databricks",
+    "dremio",
     "destination",
 ]
```

### Comparing `dlt-0.4.8a1/dlt/destinations/decorators.py` & `dlt-0.4.9a0/dlt/destinations/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 from typing import Any, Type, Optional, Callable, Union
 from typing_extensions import Concatenate
 from dlt.common.typing import AnyFun
 
 from functools import wraps
 
 from dlt.common import logger
+from dlt.common.destination import TLoaderFileFormat
+from dlt.common.typing import TDataItems
+from dlt.common.schema import TTableSchema
+
 from dlt.destinations.impl.destination.factory import destination as _destination
 from dlt.destinations.impl.destination.configuration import (
     TDestinationCallableParams,
     CustomDestinationClientConfiguration,
 )
-from dlt.common.destination import TLoaderFileFormat
-from dlt.common.typing import TDataItems
-from dlt.common.schema import TTableSchema
 
 
 def destination(
     func: Optional[AnyFun] = None,
     /,
     loader_file_format: TLoaderFileFormat = None,
     batch_size: int = 10,
```

### Comparing `dlt-0.4.8a1/dlt/destinations/exceptions.py` & `dlt-0.4.9a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/athena/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/athena/athena.py` & `dlt-0.4.9a0/dlt/destinations/impl/athena/athena.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     DefaultParameterFormatter,
     _DEFAULT_FORMATTERS,
     Formatter,
     _format_date,
 )
 
 from dlt.common import logger
+from dlt.common.exceptions import TerminalValueError
 from dlt.common.utils import without_none
 from dlt.common.data_types import TDataType
 from dlt.common.schema import TColumnSchema, Schema, TSchemaTables, TTableSchema
 from dlt.common.schema.typing import TTableSchema, TColumnType, TWriteDisposition, TTableFormat
 from dlt.common.schema.utils import table_schema_has_type, get_table_format
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import LoadJob, DoNothingFollowupJob, DoNothingJob
@@ -104,15 +105,19 @@
             return "bigint"
         if precision <= 8:
             return "int" if table_format == "iceberg" else "tinyint"
         elif precision <= 16:
             return "int" if table_format == "iceberg" else "smallint"
         elif precision <= 32:
             return "int"
-        return "bigint"
+        elif precision <= 64:
+            return "bigint"
+        raise TerminalValueError(
+            f"bigint with {precision} bits precision cannot be mapped into athena integer type"
+        )
 
     def from_db_type(
         self, db_type: str, precision: Optional[int], scale: Optional[int]
     ) -> TColumnType:
         for key, val in self.dbt_to_sct.items():
             if db_type.startswith(key):
                 return without_none(dict(data_type=val, precision=precision, scale=scale))  # type: ignore[return-value]
@@ -232,15 +237,15 @@
     @staticmethod
     def _make_database_exception(ex: Exception) -> Exception:
         if isinstance(ex, OperationalError):
             if "TABLE_NOT_FOUND" in str(ex):
                 return DatabaseUndefinedRelation(ex)
             elif "SCHEMA_NOT_FOUND" in str(ex):
                 return DatabaseUndefinedRelation(ex)
-            elif "Table not found" in str(ex):
+            elif "Table" in str(ex) and " not found" in str(ex):
                 return DatabaseUndefinedRelation(ex)
             elif "Database does not exist" in str(ex):
                 return DatabaseUndefinedRelation(ex)
             return DatabaseTerminalException(ex)
         elif isinstance(ex, (ProgrammingError, IntegrityError)):
             return DatabaseTerminalException(ex)
         if isinstance(ex, DatabaseError):
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/athena/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/athena/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/athena/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/athena/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/bigquery/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/bigquery/bigquery.py` & `dlt-0.4.9a0/dlt/destinations/impl/bigquery/bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import functools
 import os
 from pathlib import Path
-from typing import ClassVar, Optional, Sequence, Tuple, List, cast, Dict
+from typing import Any, ClassVar, Dict, List, Optional, Sequence, Tuple, Type, cast
 
 import google.cloud.bigquery as bigquery  # noqa: I250
 from google.api_core import exceptions as api_core_exceptions
 from google.cloud import exceptions as gcp_exceptions
+from google.api_core import retry
+from google.cloud.bigquery.retry import _RETRYABLE_REASONS
 
-from dlt.common import json, logger
+from dlt.common import logger
+from dlt.common.json import json
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import (
     FollowupJob,
     NewLoadJob,
     TLoadJobState,
     LoadJob,
     SupportsStagingDestination,
@@ -18,16 +22,19 @@
 from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns
 from dlt.common.schema.exceptions import UnknownTableException
 from dlt.common.schema.typing import TTableSchema, TColumnType, TTableFormat
 from dlt.common.schema.utils import get_inherited_table_hint
 from dlt.common.schema.utils import table_schema_has_type
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.typing import DictStrAny
+from dlt.destinations.job_impl import DestinationJsonlLoadJob, DestinationParquetLoadJob
+from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.exceptions import (
     DestinationSchemaWillNotUpdate,
+    DestinationTerminalException,
     DestinationTransientException,
     LoadJobNotExistsException,
     LoadJobTerminalException,
 )
 from dlt.destinations.impl.bigquery import capabilities
 from dlt.destinations.impl.bigquery.bigquery_adapter import (
     PARTITION_HINT,
@@ -39,14 +46,15 @@
 )
 from dlt.destinations.impl.bigquery.configuration import BigQueryClientConfiguration
 from dlt.destinations.impl.bigquery.sql_client import BigQuerySqlClient, BQ_TERMINAL_REASONS
 from dlt.destinations.job_client_impl import SqlJobClientWithStaging
 from dlt.destinations.job_impl import NewReferenceJob
 from dlt.destinations.sql_jobs import SqlMergeJob
 from dlt.destinations.type_mapping import TypeMapper
+from dlt.pipeline.current import destination_state
 
 
 class BigQueryTypeMapper(TypeMapper):
     sct_to_unbound_dbt = {
         "complex": "JSON",
         "text": "STRING",
         "double": "FLOAT64",
@@ -216,21 +224,48 @@
                     raise DestinationTransientException(gace) from gace
         return job
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
 
         if not job:
+            insert_api = table.get("x-insert-api", "default")
             try:
-                job = BigQueryLoadJob(
-                    FileStorage.get_file_name_from_file_path(file_path),
-                    self._create_load_job(table, file_path),
-                    self.config.http_timeout,
-                    self.config.retry_deadline,
-                )
+                if insert_api == "streaming":
+                    if table["write_disposition"] != "append":
+                        raise DestinationTerminalException(
+                            "BigQuery streaming insert can only be used with `append`"
+                            " write_disposition, while the given resource has"
+                            f" `{table['write_disposition']}`."
+                        )
+                    if file_path.endswith(".jsonl"):
+                        job_cls = DestinationJsonlLoadJob
+                    elif file_path.endswith(".parquet"):
+                        job_cls = DestinationParquetLoadJob  # type: ignore
+                    else:
+                        raise ValueError(
+                            f"Unsupported file type for BigQuery streaming inserts: {file_path}"
+                        )
+
+                    job = job_cls(
+                        table,
+                        file_path,
+                        self.config,  # type: ignore
+                        self.schema,
+                        destination_state(),
+                        functools.partial(_streaming_load, self.sql_client),
+                        [],
+                    )
+                else:
+                    job = BigQueryLoadJob(
+                        FileStorage.get_file_name_from_file_path(file_path),
+                        self._create_load_job(table, file_path),
+                        self.config.http_timeout,
+                        self.config.retry_deadline,
+                    )
             except api_core_exceptions.GoogleAPICallError as gace:
                 reason = BigQuerySqlClient._get_reason_from_errors(gace)
                 if reason == "notFound":
                     # google.api_core.exceptions.NotFound: 404 – table not found
                     raise UnknownTableException(table["name"]) from gace
                 elif (
                     reason == "duplicate"
@@ -239,14 +274,15 @@
                 elif reason in BQ_TERMINAL_REASONS:
                     # google.api_core.exceptions.BadRequest - will not be processed ie bad job name
                     raise LoadJobTerminalException(
                         file_path, f"The server reason was: {reason}"
                     ) from gace
                 else:
                     raise DestinationTransientException(gace) from gace
+
         return job
 
     def _get_table_update_sql(
         self, table_name: str, new_columns: Sequence[TColumnSchema], generate_alter: bool
     ) -> List[str]:
         table: Optional[TTableSchema] = self.prepare_load_table(table_name)
         sql = super()._get_table_update_sql(table_name, new_columns, generate_alter)
@@ -421,7 +457,45 @@
         job_id = BigQueryLoadJob.get_job_id_from_file_path(file_path)
         return cast(bigquery.LoadJob, self.sql_client.native_connection.get_job(job_id))
 
     def _from_db_type(
         self, bq_t: str, precision: Optional[int], scale: Optional[int]
     ) -> TColumnType:
         return self.type_mapper.from_db_type(bq_t, precision, scale)
+
+
+def _streaming_load(
+    sql_client: SqlClientBase[BigQueryClient], items: List[Dict[Any, Any]], table: Dict[str, Any]
+) -> None:
+    """
+    Upload the given items into BigQuery table, using streaming API.
+    Streaming API is used for small amounts of data, with optimal
+    batch size equal to 500 rows.
+
+    Args:
+        sql_client (dlt.destinations.impl.bigquery.bigquery.BigQueryClient):
+            BigQuery client.
+        items (List[Dict[Any, Any]]): List of rows to upload.
+        table (Dict[Any, Any]): Table schema.
+    """
+
+    def _should_retry(exc: api_core_exceptions.GoogleAPICallError) -> bool:
+        """Predicate to decide if we need to retry the exception.
+
+        Args:
+            exc (google.api_core.exceptions.GoogleAPICallError):
+                Exception raised by the client.
+
+        Returns:
+            bool: True if the exception is retryable, False otherwise.
+        """
+        reason = exc.errors[0]["reason"]
+        return reason in _RETRYABLE_REASONS
+
+    full_name = sql_client.make_qualified_table_name(table["name"], escape=False)
+
+    bq_client = sql_client._client
+    bq_client.insert_rows_json(
+        full_name,
+        items,
+        retry=retry.Retry(predicate=_should_retry, deadline=600),  # with 10 mins deadline
+    )
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/bigquery/bigquery_adapter.py` & `dlt-0.4.9a0/dlt/destinations/impl/bigquery/bigquery_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     data: Any,
     partition: TColumnNames = None,
     cluster: TColumnNames = None,
     round_half_away_from_zero: TColumnNames = None,
     round_half_even: TColumnNames = None,
     table_description: Optional[str] = None,
     table_expiration_datetime: Optional[str] = None,
+    insert_api: Optional[Literal["streaming", "default"]] = None,
 ) -> DltResource:
     """
     Prepares data for loading into BigQuery.
 
     This function takes data, which can be raw or already wrapped in a DltResource object,
     and prepares it for BigQuery by optionally specifying partitioning, clustering, table description and
     table expiration settings.
@@ -52,14 +53,19 @@
         round_half_even (TColumnNames, optional): Determines how values in the column are rounded when written to the table.
             This mode rounds halfway cases towards the nearest even digit.
             The columns specified must be mutually exclusive from `round_half_away_from_zero`.
             See https://cloud.google.com/bigquery/docs/schemas#rounding_mode for more information.
         table_description (str, optional): A description for the BigQuery table.
         table_expiration_datetime (str, optional): String representing the datetime when the BigQuery table expires.
             This is always interpreted as UTC, BigQuery's default.
+        insert_api (Optional[Literal["streaming", "default"]]): The API to use for inserting data into BigQuery.
+            If "default" is chosen, the original SQL query mechanism is used.
+            If "streaming" is chosen, the streaming API (https://cloud.google.com/bigquery/docs/streaming-data-into-bigquery)
+            is used.
+            NOTE: due to BigQuery features, streaming insert is only available for `append` write_disposition.
 
     Returns:
         A `DltResource` object that is ready to be loaded into BigQuery.
 
     Raises:
         ValueError: If any hint is invalid or none are specified.
 
@@ -130,24 +136,32 @@
             )
         additional_table_hints |= {TABLE_DESCRIPTION_HINT: table_description}  # type: ignore[operator]
 
     if table_expiration_datetime:
         if not isinstance(table_expiration_datetime, str):
             raise ValueError(
                 "`table_expiration_datetime` must be string representing the datetime when the"
-                " BigQuery table."
+                " BigQuery table will be deleted."
             )
         try:
             parsed_table_expiration_datetime = parser.parse(table_expiration_datetime).replace(
                 tzinfo=timezone.utc
             )
             additional_table_hints |= {TABLE_EXPIRATION_HINT: parsed_table_expiration_datetime}  # type: ignore[operator]
         except ValueError as e:
             raise ValueError(f"{table_expiration_datetime} could not be parsed!") from e
 
+    if insert_api is not None:
+        if insert_api == "streaming" and data.write_disposition != "append":
+            raise ValueError(
+                "BigQuery streaming insert can only be used with `append` write_disposition, while "
+                f"the given resource has `{data.write_disposition}`."
+            )
+        additional_table_hints |= {"x-insert-api": insert_api}  # type: ignore[operator]
+
     if column_hints or additional_table_hints:
         resource.apply_hints(columns=column_hints, additional_table_hints=additional_table_hints)
     else:
         raise ValueError(
             "AT LEAST one of `partition`, `cluster`, `round_half_away_from_zero`,"
             " `round_half_even`, `table_description` or `table_expiration_datetime` must be"
             " specified."
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/bigquery/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/bigquery/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     location: str = "US"
 
     http_timeout: float = 15.0  # connection timeout for http request to BigQuery api
     file_upload_timeout: float = 30 * 60.0  # a timeout for file upload when loading local files
     retry_deadline: float = (
         60.0  # how long to retry the operation in case of error, the backoff 60 s.
     )
+    batch_size: int = 500
 
     __config_gen_annotations__: ClassVar[List[str]] = ["location"]
 
     def get_location(self) -> str:
         if self.location != "US":
             return self.location
         # default was changed in credentials, emit deprecation message
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/bigquery/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/bigquery/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/bigquery/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/bigquery/sql_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     """Use native BigQuery data frame support if available"""
 
     native_cursor: BQDbApiCursor  # type: ignore
 
     def df(self, chunk_size: int = None, **kwargs: Any) -> DataFrame:
         if chunk_size is not None:
             return super().df(chunk_size=chunk_size)
-        query_job: bigquery.QueryJob = self.native_cursor._query_job
+        query_job: bigquery.QueryJob = getattr(
+            self.native_cursor, "_query_job", self.native_cursor.query_job
+        )
 
         try:
             return query_job.to_dataframe(**kwargs)
         except ValueError:
             # no pyarrow/db-types, fallback to our implementation
             return super().df()
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/databricks/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/databricks/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/databricks/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/databricks/databricks.py` & `dlt-0.4.9a0/dlt/destinations/impl/databricks/databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from dlt.common.configuration.specs import (
     AwsCredentialsWithoutDefaults,
     AzureCredentials,
     AzureCredentialsWithoutDefaults,
 )
 from dlt.common.data_types import TDataType
+from dlt.common.exceptions import TerminalValueError
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns
 from dlt.common.schema.typing import TTableSchema, TColumnType, TSchemaTables, TTableFormat
 from dlt.common.schema.utils import table_schema_has_type
 
 
 from dlt.destinations.insert_job_client import InsertValuesJobClient
@@ -77,15 +78,19 @@
             return "BIGINT"
         if precision <= 8:
             return "TINYINT"
         if precision <= 16:
             return "SMALLINT"
         if precision <= 32:
             return "INT"
-        return "BIGINT"
+        if precision <= 64:
+            return "BIGINT"
+        raise TerminalValueError(
+            f"bigint with {precision} bits precision cannot be mapped into databricks integer type"
+        )
 
     def from_db_type(
         self, db_type: str, precision: Optional[int] = None, scale: Optional[int] = None
     ) -> TColumnType:
         # precision and scale arguments here are meaningless as they're not included separately in information schema
         # We use full_data_type from databricks which is either in form "typename" or "typename(precision, scale)"
         type_parts = db_type.split("(")
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/databricks/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/databricks/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/databricks/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/databricks/sql_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from databricks import sql as databricks_lib
 from databricks.sql.client import (
     Connection as DatabricksSqlConnection,
     Cursor as DatabricksSqlCursor,
 )
 from databricks.sql.exc import Error as DatabricksSqlError
 
-from dlt.common import pendulum
-from dlt.common import logger
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.destinations.exceptions import (
     DatabaseTerminalException,
     DatabaseTransientException,
     DatabaseUndefinedRelation,
 )
 from dlt.destinations.sql_client import (
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/destination/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/destination/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import Optional
-from dlt.common.destination import DestinationCapabilitiesContext
-from dlt.common.data_writers import TLoaderFileFormat
+from dlt.common.destination import DestinationCapabilitiesContext, TLoaderFileFormat
 
 
 def capabilities(
-    preferred_loader_file_format: TLoaderFileFormat = "puae-jsonl",
+    preferred_loader_file_format: TLoaderFileFormat = "typed-jsonl",
     naming_convention: str = "direct",
     max_table_nesting: Optional[int] = 0,
 ) -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext.generic_capabilities(preferred_loader_file_format)
-    caps.supported_loader_file_formats = ["puae-jsonl", "parquet"]
+    caps.supported_loader_file_formats = ["typed-jsonl", "parquet"]
     caps.supports_ddl_transactions = False
     caps.supports_transactions = False
     caps.naming_convention = naming_convention
     caps.max_table_nesting = max_table_nesting
     return caps
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/destination/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/destination/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 TDestinationCallableParams = ParamSpec("TDestinationCallableParams")
 
 
 @configspec
 class CustomDestinationClientConfiguration(DestinationClientConfiguration):
     destination_type: Final[str] = dataclasses.field(default="destination", init=False, repr=False, compare=False)  # type: ignore
     destination_callable: Optional[Union[str, TDestinationCallable]] = None  # noqa: A003
-    loader_file_format: TLoaderFileFormat = "puae-jsonl"
+    loader_file_format: TLoaderFileFormat = "typed-jsonl"
     batch_size: int = 10
     skip_dlt_columns_and_tables: bool = True
     max_table_nesting: int = 0
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/destination/destination.py` & `dlt-0.4.9a0/dlt/destinations/impl/dremio/dremio.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,212 +1,241 @@
-from abc import ABC, abstractmethod
-from types import TracebackType
-from typing import ClassVar, Dict, Optional, Type, Iterable, Iterable, cast, Dict, List
-from copy import deepcopy
+from typing import ClassVar, Optional, Sequence, Tuple, List, Any
+from urllib.parse import urlparse
 
-from dlt.common.destination.reference import LoadJob
-from dlt.destinations.job_impl import EmptyLoadJob
-from dlt.common.typing import TDataItems, AnyFun
-from dlt.common import json
-from dlt.pipeline.current import (
-    destination_state,
-    commit_load_package_state,
-)
-from dlt.common.configuration import create_resolved_partial
-
-from dlt.common.schema import Schema, TTableSchema, TSchemaTables
-from dlt.common.schema.typing import TTableSchema
-from dlt.common.storages import FileStorage
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import (
+    FollowupJob,
     TLoadJobState,
     LoadJob,
-    DoNothingJob,
-    JobClientBase,
-)
-
-from dlt.destinations.impl.destination import capabilities
-from dlt.destinations.impl.destination.configuration import (
-    CustomDestinationClientConfiguration,
-    TDestinationCallable,
+    SupportsStagingDestination,
+    NewLoadJob,
 )
+from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns
+from dlt.common.schema.typing import TTableSchema, TColumnType, TTableFormat, TColumnSchemaBase
+from dlt.common.storages.file_storage import FileStorage
+from dlt.common.utils import uniq_id
+from dlt.destinations.exceptions import LoadJobTerminalException
+from dlt.destinations.impl.dremio import capabilities
+from dlt.destinations.impl.dremio.configuration import DremioClientConfiguration
+from dlt.destinations.impl.dremio.sql_client import DremioSqlClient
+from dlt.destinations.job_client_impl import SqlJobClientWithStaging
+from dlt.destinations.job_impl import EmptyLoadJob
+from dlt.destinations.job_impl import NewReferenceJob
+from dlt.destinations.sql_jobs import SqlMergeJob
+from dlt.destinations.type_mapping import TypeMapper
+from dlt.destinations.sql_client import SqlClientBase
+
+
+class DremioTypeMapper(TypeMapper):
+    BIGINT_PRECISION = 19
+    sct_to_unbound_dbt = {
+        "complex": "VARCHAR",
+        "text": "VARCHAR",
+        "double": "DOUBLE",
+        "bool": "BOOLEAN",
+        "date": "DATE",
+        "timestamp": "TIMESTAMP",
+        "bigint": "BIGINT",
+        "binary": "VARBINARY",
+        "time": "TIME",
+    }
+
+    sct_to_dbt = {
+        "decimal": "DECIMAL(%i,%i)",
+        "wei": "DECIMAL(%i,%i)",
+    }
+
+    dbt_to_sct = {
+        "VARCHAR": "text",
+        "DOUBLE": "double",
+        "FLOAT": "double",
+        "BOOLEAN": "bool",
+        "DATE": "date",
+        "TIMESTAMP": "timestamp",
+        "VARBINARY": "binary",
+        "BINARY": "binary",
+        "BINARY VARYING": "binary",
+        "VARIANT": "complex",
+        "TIME": "time",
+        "BIGINT": "bigint",
+        "DECIMAL": "decimal",
+    }
+
+    def from_db_type(
+        self, db_type: str, precision: Optional[int] = None, scale: Optional[int] = None
+    ) -> TColumnType:
+        if db_type == "DECIMAL":
+            if (precision, scale) == self.capabilities.wei_precision:
+                return dict(data_type="wei")
+            return dict(data_type="decimal", precision=precision, scale=scale)
+        return super().from_db_type(db_type, precision, scale)
+
+
+class DremioMergeJob(SqlMergeJob):
+    @classmethod
+    def _new_temp_table_name(cls, name_prefix: str, sql_client: SqlClientBase[Any]) -> str:
+        return sql_client.make_qualified_table_name(f"_temp_{name_prefix}_{uniq_id()}")
+
+    @classmethod
+    def _to_temp_table(cls, select_sql: str, temp_table_name: str) -> str:
+        return f"CREATE TABLE {temp_table_name} AS {select_sql};"
+
+    @classmethod
+    def default_order_by(cls) -> str:
+        return "NULL"
 
 
-class DestinationLoadJob(LoadJob, ABC):
+class DremioLoadJob(LoadJob, FollowupJob):
     def __init__(
         self,
-        table: TTableSchema,
         file_path: str,
-        config: CustomDestinationClientConfiguration,
-        schema: Schema,
-        destination_state: Dict[str, int],
-        destination_callable: TDestinationCallable,
-        skipped_columns: List[str],
+        table_name: str,
+        client: DremioSqlClient,
+        stage_name: Optional[str] = None,
     ) -> None:
-        super().__init__(FileStorage.get_file_name_from_file_path(file_path))
-        self._file_path = file_path
-        self._config = config
-        self._table = table
-        self._schema = schema
-        # we create pre_resolved callable here
-        self._callable = destination_callable
-        self._state: TLoadJobState = "running"
-        self._storage_id = f"{self._parsed_file_name.table_name}.{self._parsed_file_name.file_id}"
-        self.skipped_columns = skipped_columns
-        try:
-            if self._config.batch_size == 0:
-                # on batch size zero we only call the callable with the filename
-                self.call_callable_with_items(self._file_path)
-            else:
-                current_index = destination_state.get(self._storage_id, 0)
-                for batch in self.run(current_index):
-                    self.call_callable_with_items(batch)
-                    current_index += len(batch)
-                    destination_state[self._storage_id] = current_index
-
-            self._state = "completed"
-        except Exception as e:
-            self._state = "retry"
-            raise e
-        finally:
-            # save progress
-            commit_load_package_state()
-
-    @abstractmethod
-    def run(self, start_index: int) -> Iterable[TDataItems]:
-        pass
-
-    def call_callable_with_items(self, items: TDataItems) -> None:
-        if not items:
-            return
-        # call callable
-        self._callable(items, self._table)
+        file_name = FileStorage.get_file_name_from_file_path(file_path)
+        super().__init__(file_name)
 
-    def state(self) -> TLoadJobState:
-        return self._state
+        qualified_table_name = client.make_qualified_table_name(table_name)
 
-    def exception(self) -> str:
-        raise NotImplementedError()
+        # extract and prepare some vars
+        bucket_path = (
+            NewReferenceJob.resolve_reference(file_path)
+            if NewReferenceJob.is_reference_job(file_path)
+            else ""
+        )
 
+        if not bucket_path:
+            raise RuntimeError("Could not resolve bucket path.")
 
-class DestinationParquetLoadJob(DestinationLoadJob):
-    def run(self, start_index: int) -> Iterable[TDataItems]:
-        # stream items
-        from dlt.common.libs.pyarrow import pyarrow
-
-        # guard against changed batch size after restart of loadjob
-        assert (
-            start_index % self._config.batch_size
-        ) == 0, "Batch size was changed during processing of one load package"
-
-        # on record batches we cannot drop columns, we need to
-        # select the ones we want to keep
-        keep_columns = list(self._table["columns"].keys())
-        start_batch = start_index / self._config.batch_size
-        with pyarrow.parquet.ParquetFile(self._file_path) as reader:
-            for record_batch in reader.iter_batches(
-                batch_size=self._config.batch_size, columns=keep_columns
-            ):
-                if start_batch > 0:
-                    start_batch -= 1
-                    continue
-                yield record_batch
-
-
-class DestinationJsonlLoadJob(DestinationLoadJob):
-    def run(self, start_index: int) -> Iterable[TDataItems]:
-        current_batch: TDataItems = []
-
-        # stream items
-        with FileStorage.open_zipsafe_ro(self._file_path) as f:
-            encoded_json = json.typed_loads(f.read())
-
-            for item in encoded_json:
-                # find correct start position
-                if start_index > 0:
-                    start_index -= 1
-                    continue
-                # skip internal columns
-                for column in self.skipped_columns:
-                    item.pop(column, None)
-                current_batch.append(item)
-                if len(current_batch) == self._config.batch_size:
-                    yield current_batch
-                    current_batch = []
-            yield current_batch
+        file_name = (
+            FileStorage.get_file_name_from_file_path(bucket_path) if bucket_path else file_name
+        )
 
+        bucket_url = urlparse(bucket_path)
+        bucket_scheme = bucket_url.scheme
+        if bucket_scheme == "s3" and stage_name:
+            from_clause = (
+                f"FROM '@{stage_name}/{bucket_url.hostname}/{bucket_url.path.lstrip('/')}'"
+            )
+        else:
+            raise LoadJobTerminalException(
+                file_path, "Only s3 staging currently supported in Dremio destination"
+            )
 
-class DestinationClient(JobClientBase):
-    """Sink Client"""
+        source_format = file_name.split(".")[-1]
 
-    capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
+        client.execute_sql(f"""COPY INTO {qualified_table_name}
+            {from_clause}
+            FILE_FORMAT '{source_format}'
+            """)
 
-    def __init__(self, schema: Schema, config: CustomDestinationClientConfiguration) -> None:
-        super().__init__(schema, config)
-        self.config: CustomDestinationClientConfiguration = config
-        # create pre-resolved callable to avoid multiple config resolutions during execution of the jobs
-        self.destination_callable = create_resolved_partial(
-            cast(AnyFun, self.config.destination_callable), self.config
-        )
+    def state(self) -> TLoadJobState:
+        return "completed"
 
-    def initialize_storage(self, truncate_tables: Iterable[str] = None) -> None:
-        pass
+    def exception(self) -> str:
+        raise NotImplementedError()
 
-    def is_storage_initialized(self) -> bool:
-        return True
 
-    def drop_storage(self) -> None:
-        pass
+class DremioClient(SqlJobClientWithStaging, SupportsStagingDestination):
+    capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
-    def update_stored_schema(
-        self, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None
-    ) -> Optional[TSchemaTables]:
-        return super().update_stored_schema(only_tables, expected_update)
+    def __init__(self, schema: Schema, config: DremioClientConfiguration) -> None:
+        sql_client = DremioSqlClient(config.normalize_dataset_name(schema), config.credentials)
+        super().__init__(schema, config, sql_client)
+        self.config: DremioClientConfiguration = config
+        self.sql_client: DremioSqlClient = sql_client  # type: ignore
+        self.type_mapper = DremioTypeMapper(self.capabilities)
 
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
-        # skip internal tables and remove columns from schema if so configured
-        skipped_columns: List[str] = []
-        if self.config.skip_dlt_columns_and_tables:
-            if table["name"].startswith(self.schema._dlt_tables_prefix):
-                return DoNothingJob(file_path)
-            table = deepcopy(table)
-            for column in list(table["columns"].keys()):
-                if column.startswith(self.schema._dlt_tables_prefix):
-                    table["columns"].pop(column)
-                    skipped_columns.append(column)
-
-        # save our state in destination name scope
-        load_state = destination_state()
-        if file_path.endswith("parquet"):
-            return DestinationParquetLoadJob(
-                table,
-                file_path,
-                self.config,
-                self.schema,
-                load_state,
-                self.destination_callable,
-                skipped_columns,
-            )
-        if file_path.endswith("jsonl"):
-            return DestinationJsonlLoadJob(
-                table,
-                file_path,
-                self.config,
-                self.schema,
-                load_state,
-                self.destination_callable,
-                skipped_columns,
+        job = super().start_file_load(table, file_path, load_id)
+
+        if not job:
+            job = DremioLoadJob(
+                file_path=file_path,
+                table_name=table["name"],
+                client=self.sql_client,
+                stage_name=self.config.staging_data_source,
             )
-        return None
+        return job
 
     def restore_file_load(self, file_path: str) -> LoadJob:
         return EmptyLoadJob.from_file_path(file_path, "completed")
 
-    def complete_load(self, load_id: str) -> None: ...
-
-    def __enter__(self) -> "DestinationClient":
-        return self
+    def _get_table_update_sql(
+        self,
+        table_name: str,
+        new_columns: Sequence[TColumnSchema],
+        generate_alter: bool,
+        separate_alters: bool = False,
+    ) -> List[str]:
+        sql = super()._get_table_update_sql(table_name, new_columns, generate_alter)
+
+        if not generate_alter:
+            partition_list = [
+                self.capabilities.escape_identifier(c["name"])
+                for c in new_columns
+                if c.get("partition")
+            ]
+            if partition_list:
+                sql[0] += "\nPARTITION BY (" + ",".join(partition_list) + ")"
+
+            sort_list = [
+                self.capabilities.escape_identifier(c["name"]) for c in new_columns if c.get("sort")
+            ]
+            if sort_list:
+                sql[0] += "\nLOCALSORT BY (" + ",".join(sort_list) + ")"
+
+        return sql
+
+    def _from_db_type(
+        self, bq_t: str, precision: Optional[int], scale: Optional[int]
+    ) -> TColumnType:
+        return self.type_mapper.from_db_type(bq_t, precision, scale)
+
+    def _get_column_def_sql(self, c: TColumnSchema, table_format: TTableFormat = None) -> str:
+        name = self.capabilities.escape_identifier(c["name"])
+        return (
+            f"{name} {self.type_mapper.to_db_type(c)} {self._gen_not_null(c.get('nullable', True))}"
+        )
 
-    def __exit__(
-        self, exc_type: Type[BaseException], exc_val: BaseException, exc_tb: TracebackType
-    ) -> None:
-        pass
+    def get_storage_table(self, table_name: str) -> Tuple[bool, TTableSchemaColumns]:
+        def _null_to_bool(v: str) -> bool:
+            if v == "NO":
+                return False
+            elif v == "YES":
+                return True
+            raise ValueError(v)
+
+        fields = self._get_storage_table_query_columns()
+        table_schema = self.sql_client.fully_qualified_dataset_name(escape=False)
+        db_params = (table_schema, table_name)
+        query = f"""
+SELECT {",".join(fields)}
+    FROM INFORMATION_SCHEMA.COLUMNS
+WHERE
+    table_catalog = 'DREMIO' AND table_schema = %s AND table_name = %s ORDER BY ordinal_position;
+"""
+        rows = self.sql_client.execute_sql(query, *db_params)
+
+        # if no rows we assume that table does not exist
+        schema_table: TTableSchemaColumns = {}
+        if len(rows) == 0:
+            return False, schema_table
+        for c in rows:
+            numeric_precision = c[3]
+            numeric_scale = c[4]
+            schema_c: TColumnSchemaBase = {
+                "name": c[0],
+                "nullable": _null_to_bool(c[2]),
+                **self._from_db_type(c[1], numeric_precision, numeric_scale),
+            }
+            schema_table[c[0]] = schema_c  # type: ignore
+        return True, schema_table
+
+    def _create_merge_followup_jobs(self, table_chain: Sequence[TTableSchema]) -> List[NewLoadJob]:
+        return [DremioMergeJob.from_table_chain(table_chain, self.sql_client)]
+
+    def _make_add_column_sql(
+        self, new_columns: Sequence[TColumnSchema], table_format: TTableFormat = None
+    ) -> List[str]:
+        return ["ADD COLUMNS (" + ", ".join(self._get_column_def_sql(c) for c in new_columns) + ")"]
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/destination/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/destination/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import typing as t
 import inspect
 from importlib import import_module
-
 from types import ModuleType
-from dlt.common.typing import AnyFun
 
-from dlt.common.destination import Destination, DestinationCapabilitiesContext
-from dlt.destinations.exceptions import DestinationTransientException
+from dlt.common import logger
+from dlt.common.typing import AnyFun
+from dlt.common.destination import Destination, DestinationCapabilitiesContext, TLoaderFileFormat
 from dlt.common.configuration import known_sections, with_config, get_fun_spec
 from dlt.common.configuration.exceptions import ConfigurationValueError
-from dlt.common import logger
+from dlt.common.utils import get_callable_name, is_inner_callable
 
+from dlt.destinations.exceptions import DestinationTransientException
 from dlt.destinations.impl.destination.configuration import (
     CustomDestinationClientConfiguration,
     TDestinationCallable,
 )
 from dlt.destinations.impl.destination import capabilities
-from dlt.common.data_writers import TLoaderFileFormat
-from dlt.common.utils import get_callable_name, is_inner_callable
 
 if t.TYPE_CHECKING:
     from dlt.destinations.impl.destination.destination import DestinationClient
 
 
 class DestinationInfo(t.NamedTuple):
     """Runtime information on a discovered destination"""
@@ -34,15 +32,17 @@
 _DESTINATIONS: t.Dict[str, DestinationInfo] = {}
 """A registry of all the decorated destinations"""
 
 
 class destination(Destination[CustomDestinationClientConfiguration, "DestinationClient"]):
     def capabilities(self) -> DestinationCapabilitiesContext:
         return capabilities(
-            preferred_loader_file_format=self.config_params.get("loader_file_format", "puae-jsonl"),
+            preferred_loader_file_format=self.config_params.get(
+                "loader_file_format", "typed-jsonl"
+            ),
             naming_convention=self.config_params.get("naming_convention", "direct"),
             max_table_nesting=self.config_params.get("max_table_nesting", None),
         )
 
     @property
     def spec(self) -> t.Type[CustomDestinationClientConfiguration]:
         """A spec of destination configuration resolved from the sink function signature"""
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/duckdb/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/duckdb/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/duckdb/duck.py` & `dlt-0.4.9a0/dlt/destinations/impl/duckdb/duck.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,29 +77,34 @@
             return "TINYINT"
         elif precision <= 16:
             return "SMALLINT"
         elif precision <= 32:
             return "INTEGER"
         elif precision <= 64:
             return "BIGINT"
-        return "HUGEINT"
+        elif precision <= 128:
+            return "HUGEINT"
+        raise TerminalValueError(
+            f"bigint with {precision} bits precision cannot be mapped into duckdb integer type"
+        )
 
     def to_db_datetime_type(
         self, precision: Optional[int], table_format: TTableFormat = None
     ) -> str:
         if precision is None or precision == 6:
             return super().to_db_datetime_type(precision, table_format)
         if precision == 0:
             return "TIMESTAMP_S"
         if precision == 3:
             return "TIMESTAMP_MS"
         if precision == 9:
             return "TIMESTAMP_NS"
         raise TerminalValueError(
-            f"timestamp {precision} cannot be mapped into duckdb TIMESTAMP typ"
+            f"timestamp with {precision} decimals after seconds cannot be mapped into duckdb"
+            " TIMESTAMP type"
         )
 
     def from_db_type(
         self, db_type: str, precision: Optional[int], scale: Optional[int]
     ) -> TColumnType:
         # duckdb provides the types with scale and precision
         db_type = db_type.split("(")[0].upper()
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/duckdb/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/duckdb/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/duckdb/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/dummy/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/dummy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def _configure(config: DummyClientConfiguration = config.value) -> DummyClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     config = _configure()
     additional_formats: List[TLoaderFileFormat] = (
-        ["reference"] if config.create_followup_jobs else []
+        ["reference"] if config.create_followup_jobs else []  # type:ignore[list-item]
     )
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = config.loader_file_format
     caps.supported_loader_file_formats = additional_formats + [config.loader_file_format]
     caps.preferred_staging_file_format = None
     caps.supported_staging_file_formats = additional_formats + [config.loader_file_format]
     caps.max_identifier_length = 127
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/dummy/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/dummy/dummy.py` & `dlt-0.4.9a0/dlt/destinations/impl/dummy/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Optional,
     Sequence,
     Type,
     Iterable,
     List,
 )
 
-from dlt.common import pendulum
+from dlt.common.pendulum import pendulum
 from dlt.common.schema import Schema, TTableSchema, TSchemaTables
 from dlt.common.storages import FileStorage
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.exceptions import (
     DestinationTerminalException,
     DestinationTransientException,
 )
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/dummy/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/dummy/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/filesystem/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/filesystem/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/filesystem/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/filesystem/filesystem.py` & `dlt-0.4.9a0/dlt/destinations/impl/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/motherduck/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/motherduck/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/motherduck/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/motherduck/configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 MOTHERDUCK_DRIVERNAME = "md"
 
 
 @configspec(init=False)
 class MotherDuckCredentials(DuckDbBaseCredentials):
     drivername: Final[str] = dataclasses.field(default="md", init=False, repr=False, compare=False)  # type: ignore
     username: str = "motherduck"
+    password: TSecretValue = None
+    database: str = "my_db"
 
     read_only: bool = False  # open database read/write
 
     __config_gen_annotations__: ClassVar[List[str]] = ["password", "database"]
 
     def _conn_str(self) -> str:
         return f"{MOTHERDUCK_DRIVERNAME}:{self.database}?token={self.password}"
@@ -43,21 +45,19 @@
 
             raise
 
     def parse_native_representation(self, native_value: Any) -> None:
         super().parse_native_representation(native_value)
         self._token_to_password()
 
-    def on_resolved(self) -> None:
+    def on_partial(self) -> None:
+        """Takes a token from query string and reuses it as a password"""
         self._token_to_password()
-        if self.drivername == MOTHERDUCK_DRIVERNAME and not self.password:
-            raise ConfigurationValueError(
-                "Motherduck schema 'md' was specified without corresponding token or password. The"
-                " required format of connection string is: md:///<database_name>?token=<token>"
-            )
+        if not self.is_partial():
+            self.resolve()
 
 
 @configspec
 class MotherDuckClientConfiguration(DestinationClientDwhWithStagingConfiguration):
     destination_type: Final[str] = dataclasses.field(default="motherduck", init=False, repr=False, compare=False)  # type: ignore
     credentials: MotherDuckCredentials = None
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/motherduck/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/motherduck/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/motherduck/motherduck.py` & `dlt-0.4.9a0/dlt/destinations/impl/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/motherduck/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/mssql/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/mssql/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/mssql/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/mssql/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/mssql/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/mssql/mssql.py` & `dlt-0.4.9a0/dlt/destinations/impl/mssql/mssql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import ClassVar, Dict, Optional, Sequence, List, Any, Tuple
 
+from dlt.common.exceptions import TerminalValueError
 from dlt.common.wei import EVM_DECIMAL_PRECISION
 from dlt.common.destination.reference import NewLoadJob
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.data_types import TDataType
 from dlt.common.schema import TColumnSchema, TColumnHint, Schema
 from dlt.common.schema.typing import TTableSchema, TColumnType, TTableFormat
 from dlt.common.utils import uniq_id
@@ -69,15 +70,19 @@
             return "bigint"
         if precision <= 8:
             return "tinyint"
         if precision <= 16:
             return "smallint"
         if precision <= 32:
             return "int"
-        return "bigint"
+        elif precision <= 64:
+            return "bigint"
+        raise TerminalValueError(
+            f"bigint with {precision} bits precision cannot be mapped into mssql integer type"
+        )
 
     def from_db_type(
         self, db_type: str, precision: Optional[int], scale: Optional[int]
     ) -> TColumnType:
         if db_type == "decimal":
             if (precision, scale) == self.capabilities.wei_precision:
                 return dict(data_type="wei")
@@ -131,16 +136,16 @@
         )
 
     @classmethod
     def _to_temp_table(cls, select_sql: str, temp_table_name: str) -> str:
         return f"SELECT * INTO {temp_table_name} FROM ({select_sql}) as t;"
 
     @classmethod
-    def _new_temp_table_name(cls, name_prefix: str) -> str:
-        name = SqlMergeJob._new_temp_table_name(name_prefix)
+    def _new_temp_table_name(cls, name_prefix: str, sql_client: SqlClientBase[Any]) -> str:
+        name = SqlMergeJob._new_temp_table_name(name_prefix, sql_client)
         return "#" + name
 
 
 class MsSqlClient(InsertValuesJobClient):
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
     def __init__(self, schema: Schema, config: MsSqlClientConfiguration) -> None:
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/mssql/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/mssql/sql_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,16 +79,25 @@
     @raise_database_error
     def commit_transaction(self) -> None:
         self._conn.commit()
         self._conn.autocommit = True
 
     @raise_database_error
     def rollback_transaction(self) -> None:
-        self._conn.rollback()
-        self._conn.autocommit = True
+        try:
+            self._conn.rollback()
+        except pyodbc.ProgrammingError as ex:
+            if (
+                ex.args[0] == "42000" and "(111214)" in ex.args[1]
+            ):  # "no corresponding transaction found"
+                pass  # there was nothing to rollback, we silently ignore the error
+            else:
+                raise
+        finally:
+            self._conn.autocommit = True
 
     @property
     def native_connection(self) -> pyodbc.Connection:
         return self._conn
 
     def drop_dataset(self) -> None:
         # MS Sql doesn't support DROP ... CASCADE, drop tables in the schema first
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/postgres/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/postgres/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dlt.common.wei import EVM_DECIMAL_PRECISION
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     # https://www.postgresql.org/docs/current/limits.html
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "insert_values"
-    caps.supported_loader_file_formats = ["insert_values"]
+    caps.supported_loader_file_formats = ["insert_values", "csv"]
     caps.preferred_staging_file_format = None
     caps.supported_staging_file_formats = []
     caps.escape_identifier = escape_postgres_identifier
     caps.escape_literal = escape_postgres_literal
     caps.decimal_precision = (DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE)
     caps.wei_precision = (2 * EVM_DECIMAL_PRECISION, EVM_DECIMAL_PRECISION)
     caps.max_identifier_length = 63
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/postgres/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/postgres/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/postgres/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/postgres/postgres.py` & `dlt-0.4.9a0/dlt/destinations/impl/postgres/postgres.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from typing import ClassVar, Dict, Optional, Sequence, List, Any
 
-from dlt.common.wei import EVM_DECIMAL_PRECISION
-from dlt.common.destination.reference import NewLoadJob
+from dlt.common.destination.reference import FollowupJob, LoadJob, NewLoadJob, TLoadJobState
 from dlt.common.destination import DestinationCapabilitiesContext
-from dlt.common.data_types import TDataType
+from dlt.common.exceptions import TerminalValueError
 from dlt.common.schema import TColumnSchema, TColumnHint, Schema
 from dlt.common.schema.typing import TTableSchema, TColumnType, TTableFormat
+from dlt.common.storages.file_storage import FileStorage
 
 from dlt.destinations.sql_jobs import SqlStagingCopyJob, SqlJobParams
-
 from dlt.destinations.insert_job_client import InsertValuesJobClient
-
 from dlt.destinations.impl.postgres import capabilities
 from dlt.destinations.impl.postgres.sql_client import Psycopg2SqlClient
 from dlt.destinations.impl.postgres.configuration import PostgresClientConfiguration
 from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.type_mapping import TypeMapper
 
-
 HINT_TO_POSTGRES_ATTR: Dict[TColumnHint, str] = {"unique": "UNIQUE"}
 
 
 class PostgresTypeMapper(TypeMapper):
     sct_to_unbound_dbt = {
         "complex": "jsonb",
         "text": "varchar",
@@ -64,15 +61,19 @@
         if precision is None:
             return "bigint"
         # Precision is number of bits
         if precision <= 16:
             return "smallint"
         elif precision <= 32:
             return "integer"
-        return "bigint"
+        elif precision <= 64:
+            return "bigint"
+        raise TerminalValueError(
+            f"bigint with {precision} bits precision cannot be mapped into postgres integer type"
+        )
 
     def from_db_type(
         self, db_type: str, precision: Optional[int] = None, scale: Optional[int] = None
     ) -> TColumnType:
         if db_type == "numeric":
             if (precision, scale) == self.capabilities.wei_precision:
                 return dict(data_type="wei")
@@ -100,25 +101,58 @@
                 f" {sql_client.fully_qualified_dataset_name()};"
             )
             # recreate staging table
             sql.append(f"CREATE TABLE {staging_table_name} (like {table_name} including all);")
         return sql
 
 
+class PostgresCsvCopyJob(LoadJob, FollowupJob):
+    def __init__(self, table_name: str, file_path: str, sql_client: Psycopg2SqlClient) -> None:
+        super().__init__(FileStorage.get_file_name_from_file_path(file_path))
+
+        with FileStorage.open_zipsafe_ro(file_path, "rb") as f:
+            # all headers in first line
+            headers = f.readline().decode("utf-8").strip()
+            qualified_table_name = sql_client.make_qualified_table_name(table_name)
+            copy_sql = (
+                "COPY %s (%s) FROM STDIN WITH (FORMAT CSV, DELIMITER ',', NULL '', FORCE_NULL(%s))"
+                % (
+                    qualified_table_name,
+                    headers,
+                    headers,
+                )
+            )
+            with sql_client.begin_transaction():
+                with sql_client.native_connection.cursor() as cursor:
+                    cursor.copy_expert(copy_sql, f, size=8192)
+
+    def state(self) -> TLoadJobState:
+        return "completed"
+
+    def exception(self) -> str:
+        raise NotImplementedError()
+
+
 class PostgresClient(InsertValuesJobClient):
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
     def __init__(self, schema: Schema, config: PostgresClientConfiguration) -> None:
         sql_client = Psycopg2SqlClient(config.normalize_dataset_name(schema), config.credentials)
         super().__init__(schema, config, sql_client)
         self.config: PostgresClientConfiguration = config
-        self.sql_client = sql_client
+        self.sql_client: Psycopg2SqlClient = sql_client
         self.active_hints = HINT_TO_POSTGRES_ATTR if self.config.create_indexes else {}
         self.type_mapper = PostgresTypeMapper(self.capabilities)
 
+    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
+        job = super().start_file_load(table, file_path, load_id)
+        if not job and file_path.endswith("csv"):
+            job = PostgresCsvCopyJob(table["name"], file_path, self.sql_client)
+        return job
+
     def _get_column_def_sql(self, c: TColumnSchema, table_format: TTableFormat = None) -> str:
         hints_str = " ".join(
             self.active_hints.get(h, "")
             for h in self.active_hints.keys()
             if c.get(h, False) is True
         )
         column_name = self.capabilities.escape_identifier(c["name"])
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/postgres/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/qdrant/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/qdrant/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/qdrant/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/qdrant/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/qdrant/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/qdrant/qdrant_adapter.py` & `dlt-0.4.9a0/dlt/destinations/impl/qdrant/qdrant_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/qdrant/qdrant_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/qdrant/qdrant_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from types import TracebackType
 from typing import ClassVar, Optional, Sequence, List, Dict, Type, Iterable, Any, IO
 
-from dlt.common import json, pendulum, logger
+from dlt.common import logger
+from dlt.common.json import json
+from dlt.common.pendulum import pendulum
 from dlt.common.schema import Schema, TTableSchema, TSchemaTables
 from dlt.common.schema.utils import get_columns_names_with_prop
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import TLoadJobState, LoadJob, JobClientBase, WithStateSync
 from dlt.common.storages import FileStorage
 
 from dlt.destinations.job_impl import EmptyLoadJob
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/redshift/README.md` & `dlt-0.4.9a0/dlt/destinations/impl/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/redshift/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/redshift/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/redshift/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/redshift/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/redshift/redshift.py` & `dlt-0.4.9a0/dlt/destinations/impl/redshift/redshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import platform
 import os
 
+from dlt.common.exceptions import TerminalValueError
 from dlt.destinations.impl.postgres.sql_client import Psycopg2SqlClient
 
 from dlt.common.schema.utils import table_schema_has_type, table_schema_has_type_with_precision
 
 if platform.python_implementation() == "PyPy":
     import psycopg2cffi as psycopg2
 
@@ -88,15 +89,19 @@
     ) -> str:
         if precision is None:
             return "bigint"
         if precision <= 16:
             return "smallint"
         elif precision <= 32:
             return "integer"
-        return "bigint"
+        elif precision <= 64:
+            return "bigint"
+        raise TerminalValueError(
+            f"bigint with {precision} bits precision cannot be mapped into postgres integer type"
+        )
 
     def from_db_type(
         self, db_type: str, precision: Optional[int], scale: Optional[int]
     ) -> TColumnType:
         if db_type == "numeric":
             if (precision, scale) == self.capabilities.wei_precision:
                 return dict(data_type="wei")
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/snowflake/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/snowflake/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/snowflake/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/snowflake/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/snowflake/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/snowflake/snowflake.py` & `dlt-0.4.9a0/dlt/destinations/impl/snowflake/snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 stage_name = client.make_qualified_table_name("%" + table_name)
             stage_file_path = f'@{stage_name}/"{load_id}"/{file_name}'
             from_clause = f"FROM {stage_file_path}"
 
         # decide on source format, stage_file_path will either be a local file or a bucket path
         source_format = "( TYPE = 'JSON', BINARY_FORMAT = 'BASE64' )"
         if file_name.endswith("parquet"):
-            source_format = "(TYPE = 'PARQUET', BINARY_AS_TEXT = FALSE)"
+            source_format = "(TYPE = 'PARQUET', BINARY_AS_TEXT = FALSE, USE_LOGICAL_TYPE = TRUE)"
 
         with client.begin_transaction():
             # PUT and COPY in one tx if local file, otherwise only copy
             if not bucket_path:
                 client.execute_sql(
                     f'PUT file://{file_path} @{stage_name}/"{load_id}" OVERWRITE = TRUE,'
                     " AUTO_COMPRESS = FALSE"
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/snowflake/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/snowflake/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/synapse/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/synapse/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -37,12 +37,18 @@
     caps.max_text_data_type_length = 2 * 1024 * 1024 * 1024
     caps.is_max_text_data_type_length_in_bytes = True
 
     # https://learn.microsoft.com/en-us/azure/synapse-analytics/sql-data-warehouse/sql-data-warehouse-develop-transactions
     caps.supports_transactions = True
     caps.supports_ddl_transactions = False
 
+    # Synapse throws "Some part of your SQL statement is nested too deeply. Rewrite the query or break it up into smaller queries."
+    # if number of records exceeds a certain number. Which exact number that is seems not deterministic:
+    # in tests, I've seen a query with 12230 records run succesfully on one run, but fail on a subsequent run, while the query remained exactly the same.
+    # 10.000 records is a "safe" amount that always seems to work.
+    caps.max_rows_per_insert = 10000
+
     # datetimeoffset can store 7 digits for fractional seconds
     # https://learn.microsoft.com/en-us/sql/t-sql/data-types/datetimeoffset-transact-sql?view=sql-server-ver16
     caps.timestamp_precision = 7
 
     return caps
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/synapse/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/synapse/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/synapse/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/synapse/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/synapse/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/synapse/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/synapse/synapse.py` & `dlt-0.4.9a0/dlt/destinations/impl/synapse/synapse.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 
 from dlt import current
 
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import (
     SupportsStagingDestination,
     NewLoadJob,
-    CredentialsConfiguration,
 )
 
 from dlt.common.schema import TTableSchema, TColumnSchema, Schema, TColumnHint
-from dlt.common.schema.utils import table_schema_has_type, get_inherited_table_hint
-from dlt.common.schema.typing import TTableSchemaColumns
+from dlt.common.schema.utils import (
+    table_schema_has_type,
+    get_inherited_table_hint,
+    is_complete_column,
+)
 
 from dlt.common.configuration.specs import AzureCredentialsWithoutDefaults
 
 from dlt.destinations.job_impl import NewReferenceJob
 from dlt.destinations.sql_jobs import SqlStagingCopyJob, SqlJobParams
 from dlt.destinations.sql_client import SqlClientBase
-from dlt.destinations.insert_job_client import InsertValuesJobClient
 from dlt.destinations.job_client_impl import SqlJobClientBase, LoadJob, CopyRemoteFileLoadJob
 from dlt.destinations.exceptions import LoadJobTerminalException
 
 from dlt.destinations.impl.mssql.mssql import (
     MsSqlTypeMapper,
     MsSqlClient,
     VARCHAR_MAX_N,
@@ -123,15 +124,27 @@
             return {**c, **{"precision": VARBINARY_MAX_N}}
         return c
 
     def _create_replace_followup_jobs(
         self, table_chain: Sequence[TTableSchema]
     ) -> List[NewLoadJob]:
         if self.config.replace_strategy == "staging-optimized":
-            return [SynapseStagingCopyJob.from_table_chain(table_chain, self.sql_client)]
+            # we must recreate staging table after SCHEMA TRANSFER
+            job_params: SqlJobParams = {"table_chain_create_table_statements": {}}
+            create_statements = job_params["table_chain_create_table_statements"]
+            with self.with_staging_dataset():
+                for table in table_chain:
+                    columns = [c for c in self.schema.get_table_columns(table["name"]).values()]
+                    # generate CREATE TABLE statement
+                    create_statements[table["name"]] = self._get_table_update_sql(
+                        table["name"], columns, generate_alter=False
+                    )
+            return [
+                SynapseStagingCopyJob.from_table_chain(table_chain, self.sql_client, job_params)
+            ]
         return super()._create_replace_followup_jobs(table_chain)
 
     def prepare_load_table(self, table_name: str, staging: bool = False) -> TTableSchema:
         table = super().prepare_load_table(table_name, staging)
         if staging and self.config.replace_strategy == "insert-from-staging":
             # Staging tables should always be heap tables, because "when you are
             # temporarily landing data in dedicated SQL pool, you may find that
@@ -190,23 +203,15 @@
             sql.append(f"DROP TABLE {table_name};")
             # moving staging table to destination schema
             sql.append(
                 f"ALTER SCHEMA {sql_client.fully_qualified_dataset_name()} TRANSFER"
                 f" {staging_table_name};"
             )
             # recreate staging table
-            job_client = current.pipeline().destination_client()  # type: ignore[operator]
-            with job_client.with_staging_dataset():
-                # get table columns from schema
-                columns = [c for c in job_client.schema.get_table_columns(table["name"]).values()]
-                # generate CREATE TABLE statement
-                create_table_stmt = job_client._get_table_update_sql(
-                    table["name"], columns, generate_alter=False
-                )
-            sql.extend(create_table_stmt)
+            sql.extend(params["table_chain_create_table_statements"][table["name"]])
 
         return sql
 
 
 class SynapseCopyFileLoadJob(CopyRemoteFileLoadJob):
     def __init__(
         self,
```

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/synapse/synapse_adapter.py` & `dlt-0.4.9a0/dlt/destinations/impl/synapse/synapse_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/weaviate/README.md` & `dlt-0.4.9a0/dlt/destinations/impl/weaviate/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/weaviate/__init__.py` & `dlt-0.4.9a0/dlt/destinations/impl/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/weaviate/configuration.py` & `dlt-0.4.9a0/dlt/destinations/impl/weaviate/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/weaviate/exceptions.py` & `dlt-0.4.9a0/dlt/destinations/impl/weaviate/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/weaviate/factory.py` & `dlt-0.4.9a0/dlt/destinations/impl/weaviate/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/weaviate/naming.py` & `dlt-0.4.9a0/dlt/destinations/impl/weaviate/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/weaviate/weaviate_adapter.py` & `dlt-0.4.9a0/dlt/destinations/impl/weaviate/weaviate_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/impl/weaviate/weaviate_client.py` & `dlt-0.4.9a0/dlt/destinations/impl/weaviate/weaviate_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,17 @@
     DestinationTerminalException,
 )
 
 import weaviate
 from weaviate.gql.get import GetBuilder
 from weaviate.util import generate_uuid5
 
-from dlt.common import json, pendulum, logger
+from dlt.common import logger
+from dlt.common.json import json
+from dlt.common.pendulum import pendulum
 from dlt.common.typing import StrAny, TFun
 from dlt.common.time import ensure_pendulum_datetime
 from dlt.common.schema import Schema, TTableSchema, TSchemaTables, TTableSchemaColumns
 from dlt.common.schema.typing import TColumnSchema, TColumnType
 from dlt.common.schema.utils import get_columns_names_with_prop
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import TLoadJobState, LoadJob, JobClientBase, WithStateSync
@@ -487,15 +489,16 @@
         # we need to find a stored state that matches a load id that was completed
         # we retrieve the state in blocks of 10 for this
         stepsize = 10
         offset = 0
         while True:
             state_records = self.get_records(
                 self.schema.state_table_name,
-                sort={"path": ["created_at"], "order": "desc"},
+                # search by package load id which is guaranteed to increase over time
+                sort={"path": ["_dlt_load_id"], "order": "desc"},
                 where={
                     "path": ["pipeline_name"],
                     "operator": "Equal",
                     "valueString": pipeline_name,
                 },
                 limit=stepsize,
                 offset=offset,
```

### Comparing `dlt-0.4.8a1/dlt/destinations/insert_job_client.py` & `dlt-0.4.9a0/dlt/destinations/insert_job_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,18 +32,22 @@
         raise NotImplementedError()
 
     def _insert(self, qualified_table_name: str, file_path: str) -> Iterator[List[str]]:
         # WARNING: maximum redshift statement is 16MB https://docs.aws.amazon.com/redshift/latest/dg/c_redshift-sql.html
         # the procedure below will split the inserts into max_query_length // 2 packs
         with FileStorage.open_zipsafe_ro(file_path, "r", encoding="utf-8") as f:
             header = f.readline()
-            if self._sql_client.capabilities.insert_values_writer_type == "default":
+            writer_type = self._sql_client.capabilities.insert_values_writer_type
+            if writer_type == "default":
+                sep = ","
                 # properly formatted file has a values marker at the beginning
                 values_mark = f.readline()
                 assert values_mark == "VALUES\n"
+            elif writer_type == "select_union":
+                sep = " UNION ALL"
 
             max_rows = self._sql_client.capabilities.max_rows_per_insert
 
             insert_sql = []
             while content := f.read(self._sql_client.capabilities.max_query_length // 2):
                 # read one more line in order to
                 # 1. complete the content which ends at "random" position, not an end line
@@ -53,45 +57,40 @@
                 # TODO: write test for this case (content ends with ",")
                 if until_nl == "\n":
                     until_nl = f.readline()
                 until_nl = until_nl.strip("\n")
                 # if there was anything left, until_nl contains the last line
                 is_eof = len(until_nl) == 0 or until_nl[-1] == ";"
                 if not is_eof:
-                    # print(f'replace the "," with " {until_nl} {len(insert_sql)}')
-                    until_nl = until_nl[:-1] + ";"
-
+                    until_nl = until_nl[: -len(sep)] + ";"  # replace the separator with ";"
                 if max_rows is not None:
                     # mssql has a limit of 1000 rows per INSERT, so we need to split into separate statements
                     values_rows = content.splitlines(keepends=True)
                     len_rows = len(values_rows)
                     processed = 0
                     # Chunk by max_rows - 1 for simplicity because one more row may be added
                     for chunk in chunks(values_rows, max_rows - 1):
                         processed += len(chunk)
                         insert_sql.append(header.format(qualified_table_name))
-                        if self._sql_client.capabilities.insert_values_writer_type == "default":
+                        if writer_type == "default":
                             insert_sql.append(values_mark)
                         if processed == len_rows:
                             # On the last chunk we need to add the extra row read
                             insert_sql.append("".join(chunk) + until_nl)
                         else:
                             # Replace the , with ;
-                            insert_sql.append("".join(chunk).strip()[:-1] + ";\n")
+                            insert_sql.append("".join(chunk).strip()[: -len(sep)] + ";\n")
                 else:
                     # otherwise write all content in a single INSERT INTO
-                    if self._sql_client.capabilities.insert_values_writer_type == "default":
+                    if writer_type == "default":
                         insert_sql.extend(
-                            [header.format(qualified_table_name), values_mark, content]
+                            [header.format(qualified_table_name), values_mark, content + until_nl]
                         )
-                    elif self._sql_client.capabilities.insert_values_writer_type == "select_union":
-                        insert_sql.extend([header.format(qualified_table_name), content])
-
-                    if until_nl:
-                        insert_sql.append(until_nl)
+                    elif writer_type == "select_union":
+                        insert_sql.extend([header.format(qualified_table_name), content + until_nl])
 
                 # actually this may be empty if we were able to read a full file into content
                 if not is_eof:
                     # execute chunk of insert
                     yield insert_sql
                     insert_sql = []
 
@@ -120,16 +119,7 @@
     def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
         job = super().start_file_load(table, file_path, load_id)
         if not job:
             # this is using sql_client internally and will raise a right exception
             if file_path.endswith("insert_values"):
                 job = InsertValuesLoadJob(table["name"], file_path, self.sql_client)
         return job
-
-    # # TODO: implement indexes and primary keys for postgres
-    # def _get_in_table_constraints_sql(self, t: TTableSchema) -> str:
-    #     # get primary key
-    #     pass
-
-    # def _get_out_table_constrains_sql(self, t: TTableSchema) -> str:
-    #     # set non unique indexes
-    #     pass
```

### Comparing `dlt-0.4.8a1/dlt/destinations/job_client_impl.py` & `dlt-0.4.9a0/dlt/destinations/job_client_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     Iterator,
     ContextManager,
     cast,
 )
 import zlib
 import re
 
-from dlt.common import json, pendulum, logger
+from dlt.common import logger
+from dlt.common.json import json
+from dlt.common.pendulum import pendulum
 from dlt.common.data_types import TDataType
 from dlt.common.schema.typing import (
     COLUMN_HINTS,
     TColumnType,
     TColumnSchemaBase,
     TTableSchema,
     TWriteDisposition,
@@ -359,15 +361,15 @@
 
     def get_stored_state(self, pipeline_name: str) -> StateInfo:
         state_table = self.sql_client.make_qualified_table_name(self.schema.state_table_name)
         loads_table = self.sql_client.make_qualified_table_name(self.schema.loads_table_name)
         query = (
             f"SELECT {self.state_table_columns} FROM {state_table} AS s JOIN {loads_table} AS l ON"
             " l.load_id = s._dlt_load_id WHERE pipeline_name = %s AND l.status = 0 ORDER BY"
-            " created_at DESC"
+            " l.load_id DESC"
         )
         with self.sql_client.execute_query(query, pipeline_name) as cur:
             row = cur.fetchone()
         if not row:
             return None
         return StateInfo(row[0], row[1], row[2], row[3], pendulum.instance(row[4]))
```

### Comparing `dlt-0.4.8a1/dlt/destinations/path_utils.py` & `dlt-0.4.9a0/dlt/destinations/path_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # this can probably go some other place, but it is shared by destinations, so for now it is here
 from typing import List, Sequence, Tuple
 
-import pendulum
 import re
 
+from dlt.common.pendulum import pendulum
+
 from dlt.destinations.exceptions import InvalidFilesystemLayout, CantExtractTablePrefix
 
 # TODO: ensure layout only has supported placeholders
 SUPPORTED_PLACEHOLDERS = {"schema_name", "table_name", "load_id", "file_id", "ext", "curr_date"}
 
 SUPPORTED_TABLE_NAME_PREFIX_PLACEHOLDERS = ("schema_name",)
```

### Comparing `dlt-0.4.8a1/dlt/destinations/sql_client.py` & `dlt-0.4.9a0/dlt/destinations/sql_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from dlt.common.typing import TFun
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.utils import concat_strings_with_limit
 
 from dlt.destinations.exceptions import (
     DestinationConnectionError,
     LoadClientNotConnected,
-    DatabaseTerminalException,
 )
 from dlt.destinations.typing import DBApi, TNativeConn, DBApiCursor, DataFrame, DBTransaction
 
 
 class SqlClientBase(ABC, Generic[TNativeConn]):
     dbapi: ClassVar[DBApi] = None
     capabilities: ClassVar[DestinationCapabilitiesContext] = None
```

### Comparing `dlt-0.4.8a1/dlt/destinations/sql_jobs.py` & `dlt-0.4.9a0/dlt/destinations/sql_jobs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,41 @@
-from typing import Any, Callable, List, Sequence, Tuple, cast, TypedDict, Optional
+from typing import Any, Dict, List, Sequence, Tuple, cast, TypedDict, Optional
 
 import yaml
+from dlt.common.data_writers.escape import format_datetime_literal
 from dlt.common.logger import pretty_format_exception
 
-from dlt.common.schema.typing import TTableSchema, TSortOrder
+from dlt.common.pendulum import pendulum
+from dlt.common.schema.typing import (
+    TTableSchema,
+    TSortOrder,
+)
 from dlt.common.schema.utils import (
     get_columns_names_with_prop,
     get_first_column_name_with_prop,
     get_dedup_sort_tuple,
+    get_validity_column_names,
+    DEFAULT_MERGE_STRATEGY,
 )
 from dlt.common.storages.load_storage import ParsedLoadJobFileName
 from dlt.common.utils import uniq_id
 from dlt.common.destination.capabilities import DestinationCapabilitiesContext
 from dlt.destinations.exceptions import MergeDispositionException
 from dlt.destinations.job_impl import NewLoadJobImpl
 from dlt.destinations.sql_client import SqlClientBase
+from dlt.pipeline.current import load_package as current_load_package
+
 
+HIGH_TS = pendulum.datetime(9999, 12, 31)
+"""High timestamp used to indicate active records in `scd2` merge strategy."""
 
-class SqlJobParams(TypedDict):
+
+class SqlJobParams(TypedDict, total=False):
     replace: Optional[bool]
+    table_chain_create_table_statements: Dict[str, Sequence[str]]
 
 
 DEFAULTS: SqlJobParams = {"replace": False}
 
 
 class SqlBaseJob(NewLoadJobImpl):
     """Sql base job for jobs that rely on the whole tablechain"""
@@ -36,15 +49,15 @@
         sql_client: SqlClientBase[Any],
         params: Optional[SqlJobParams] = None,
     ) -> NewLoadJobImpl:
         """Generates a list of sql statements, that will be executed by the sql client when the job is executed in the loader.
 
         The `table_chain` contains a list schemas of a tables with parent-child relationship, ordered by the ancestry (the root of the tree is first on the list).
         """
-        params = cast(SqlJobParams, {**DEFAULTS, **(params or {})})  # type: ignore
+        params = cast(SqlJobParams, {**DEFAULTS, **(params or {})})
         top_table = table_chain[0]
         file_info = ParsedLoadJobFileName(
             top_table["name"], ParsedLoadJobFileName.new_file_id(), 0, "sql"
         )
         try:
             # Remove line breaks from multiline statements and write one SQL statement per line in output file
             # to support clients that need to execute one statement at a time (i.e. snowflake)
@@ -134,33 +147,25 @@
 
 class SqlMergeJob(SqlBaseJob):
     """Generates a list of sql statements that merge the data from staging dataset into destination dataset."""
 
     failed_text: str = "Tried to generate a merge sql job for the following tables:"
 
     @classmethod
-    def generate_sql(
+    def generate_sql(  # type: ignore[return]
         cls,
         table_chain: Sequence[TTableSchema],
         sql_client: SqlClientBase[Any],
         params: Optional[SqlJobParams] = None,
     ) -> List[str]:
-        """Generates a list of sql statements that merge the data in staging dataset with the data in destination dataset.
-
-        The `table_chain` contains a list schemas of a tables with parent-child relationship, ordered by the ancestry (the root of the tree is first on the list).
-        The root table is merged using primary_key and merge_key hints which can be compound and be both specified. In that case the OR clause is generated.
-        The child tables are merged based on propagated `root_key` which is a type of foreign key but always leading to a root table.
-
-        First we store the root_keys of root table elements to be deleted in the temp table. Then we use the temp table to delete records from root and all child tables in the destination dataset.
-        At the end we copy the data from the staging dataset into destination dataset.
-
-        If a hard_delete column is specified, records flagged as deleted will be excluded from the copy into the destination dataset.
-        If a dedup_sort column is specified in conjunction with a primary key, records will be sorted before deduplication, so the "latest" record remains.
-        """
-        return cls.gen_merge_sql(table_chain, sql_client)
+        merge_strategy = table_chain[0].get("x-merge-strategy", DEFAULT_MERGE_STRATEGY)
+        if merge_strategy == "delete-insert":
+            return cls.gen_merge_sql(table_chain, sql_client)
+        elif merge_strategy == "scd2":
+            return cls.gen_scd2_sql(table_chain, sql_client)
 
     @classmethod
     def _gen_key_table_clauses(
         cls, primary_keys: Sequence[str], merge_keys: Sequence[str]
     ) -> List[str]:
         """Generate sql clauses to select rows to delete via merge and primary key. Return select all clause if no keys defined."""
         clauses: List[str] = []
@@ -190,22 +195,22 @@
         return [
             f"FROM {root_table_name} as d WHERE EXISTS (SELECT 1 FROM {staging_root_table_name} as"
             f" s WHERE {' OR '.join([c.format(d='d',s='s') for c in key_clauses])})"
         ]
 
     @classmethod
     def gen_delete_temp_table_sql(
-        cls, unique_column: str, key_table_clauses: Sequence[str]
+        cls, unique_column: str, key_table_clauses: Sequence[str], sql_client: SqlClientBase[Any]
     ) -> Tuple[List[str], str]:
         """Generate sql that creates delete temp table and inserts `unique_column` from root table for all records to delete. May return several statements.
 
         Returns temp table name for cases where special names are required like SQLServer.
         """
         sql: List[str] = []
-        temp_table_name = cls._new_temp_table_name("delete")
+        temp_table_name = cls._new_temp_table_name("delete", sql_client)
         select_statement = f"SELECT d.{unique_column} {key_table_clauses[0]}"
         sql.append(cls._to_temp_table(select_statement, temp_table_name))
         for clause in key_table_clauses[1:]:
             sql.append(f"INSERT INTO {temp_table_name} SELECT {unique_column} {clause};")
         return sql, temp_table_name
 
     @classmethod
@@ -250,15 +255,15 @@
             A string representing a SELECT FROM SQL statement where the FROM
             clause represents a deduplicated version of the `table_name` table.
 
             The returned value is used in two ways:
             1) To select the values for an INSERT INTO statement.
             2) To select the values for a temporary table used for inserts.
         """
-        order_by = "(SELECT NULL)"
+        order_by = cls.default_order_by()
         if dedup_sort is not None:
             order_by = f"{dedup_sort[0]} {dedup_sort[1].upper()}"
         if condition is None:
             condition = "1 = 1"
         col_str = ", ".join(columns)
         inner_col_str = col_str
         if condition_columns is not None:
@@ -268,24 +273,29 @@
                 FROM (
                     SELECT ROW_NUMBER() OVER (partition BY {", ".join(primary_keys)} ORDER BY {order_by}) AS _dlt_dedup_rn, {inner_col_str}
                     FROM {table_name}
                 ) AS _dlt_dedup_numbered WHERE _dlt_dedup_rn = 1 AND ({condition})
         """
 
     @classmethod
+    def default_order_by(cls) -> str:
+        return "(SELECT NULL)"
+
+    @classmethod
     def gen_insert_temp_table_sql(
         cls,
         staging_root_table_name: str,
+        sql_client: SqlClientBase[Any],
         primary_keys: Sequence[str],
         unique_column: str,
         dedup_sort: Tuple[str, TSortOrder] = None,
         condition: str = None,
         condition_columns: Sequence[str] = None,
     ) -> Tuple[List[str], str]:
-        temp_table_name = cls._new_temp_table_name("insert")
+        temp_table_name = cls._new_temp_table_name("insert", sql_client)
         if len(primary_keys) > 0:
             # deduplicate
             select_sql = cls.gen_select_from_dedup_sql(
                 staging_root_table_name,
                 primary_keys,
                 [unique_column],
                 dedup_sort,
@@ -309,15 +319,15 @@
         return f"""DELETE FROM {table_name}
             WHERE {unique_column} IN (
                 SELECT * FROM {delete_temp_table_name}
             );
         """
 
     @classmethod
-    def _new_temp_table_name(cls, name_prefix: str) -> str:
+    def _new_temp_table_name(cls, name_prefix: str, sql_client: SqlClientBase[Any]) -> str:
         return f"{name_prefix}_{uniq_id()}"
 
     @classmethod
     def _to_temp_table(cls, select_sql: str, temp_table_name: str) -> str:
         """Generate sql that creates temp table from select statement. May return several statements.
 
         Args:
@@ -329,28 +339,41 @@
         """
         return f"CREATE TEMP TABLE {temp_table_name} AS {select_sql};"
 
     @classmethod
     def gen_merge_sql(
         cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]
     ) -> List[str]:
+        """Generates a list of sql statements that merge the data in staging dataset with the data in destination dataset.
+
+        The `table_chain` contains a list schemas of a tables with parent-child relationship, ordered by the ancestry (the root of the tree is first on the list).
+        The root table is merged using primary_key and merge_key hints which can be compound and be both specified. In that case the OR clause is generated.
+        The child tables are merged based on propagated `root_key` which is a type of foreign key but always leading to a root table.
+
+        First we store the root_keys of root table elements to be deleted in the temp table. Then we use the temp table to delete records from root and all child tables in the destination dataset.
+        At the end we copy the data from the staging dataset into destination dataset.
+
+        If a hard_delete column is specified, records flagged as deleted will be excluded from the copy into the destination dataset.
+        If a dedup_sort column is specified in conjunction with a primary key, records will be sorted before deduplication, so the "latest" record remains.
+        """
         sql: List[str] = []
         root_table = table_chain[0]
 
         escape_id = sql_client.capabilities.escape_identifier
         escape_lit = sql_client.capabilities.escape_literal
         if escape_id is None:
             escape_id = DestinationCapabilitiesContext.generic_capabilities().escape_identifier
         if escape_lit is None:
             escape_lit = DestinationCapabilitiesContext.generic_capabilities().escape_literal
 
         # get top level table full identifiers
         root_table_name = sql_client.make_qualified_table_name(root_table["name"])
         with sql_client.with_staging_dataset(staging=True):
             staging_root_table_name = sql_client.make_qualified_table_name(root_table["name"])
+
         # get merge and primary keys from top level
         primary_keys = list(
             map(
                 escape_id,
                 get_columns_names_with_prop(root_table, "primary_key"),
             )
         )
@@ -386,15 +409,15 @@
                     f"There is no unique column (ie _dlt_id) in top table {root_table['name']} so"
                     " it is not possible to link child tables to it.",
                 )
             # get first unique column
             unique_column = escape_id(unique_columns[0])
             # create temp table with unique identifier
             create_delete_temp_table_sql, delete_temp_table_name = cls.gen_delete_temp_table_sql(
-                unique_column, key_table_clauses
+                unique_column, key_table_clauses, sql_client
             )
             sql.extend(create_delete_temp_table_sql)
 
             # delete from child tables first. This is important for databricks which does not support temporary tables,
             # but uses temporary views instead
             for table in table_chain[1:]:
                 table_name = sql_client.make_qualified_table_name(table["name"])
@@ -440,14 +463,15 @@
             if len(primary_keys) > 0 or hard_delete_col is not None:
                 condition_columns = [hard_delete_col] if not_deleted_cond is not None else None
                 (
                     create_insert_temp_table_sql,
                     insert_temp_table_name,
                 ) = cls.gen_insert_temp_table_sql(
                     staging_root_table_name,
+                    sql_client,
                     primary_keys,
                     unique_column,
                     dedup_sort,
                     not_deleted_cond,
                     condition_columns,
                 )
                 sql.extend(create_insert_temp_table_sql)
@@ -474,7 +498,91 @@
                 # without child tables we deduplicate inside the query instead of using a temp table
                 select_sql = cls.gen_select_from_dedup_sql(
                     staging_table_name, primary_keys, columns, dedup_sort, insert_cond
                 )
 
             sql.append(f"INSERT INTO {table_name}({col_str}) {select_sql};")
         return sql
+
+    @classmethod
+    def gen_scd2_sql(
+        cls, table_chain: Sequence[TTableSchema], sql_client: SqlClientBase[Any]
+    ) -> List[str]:
+        """Generates SQL statements for the `scd2` merge strategy.
+
+        The root table can be inserted into and updated.
+        Updates only take place when a record retires (because there is a new version
+        or it is deleted) and only affect the "valid to" column.
+        Child tables are insert-only.
+        """
+        sql: List[str] = []
+        root_table = table_chain[0]
+        root_table_name = sql_client.make_qualified_table_name(root_table["name"])
+        with sql_client.with_staging_dataset(staging=True):
+            staging_root_table_name = sql_client.make_qualified_table_name(root_table["name"])
+
+        # get column names
+        escape_id = sql_client.capabilities.escape_identifier
+        from_, to = list(map(escape_id, get_validity_column_names(root_table)))  # validity columns
+        hash_ = escape_id(
+            get_first_column_name_with_prop(root_table, "x-row-version")
+        )  # row hash column
+
+        # define values for validity columns
+        boundary_ts = format_datetime_literal(
+            current_load_package()["state"]["created_at"],
+            sql_client.capabilities.timestamp_precision,
+        )
+        active_record_ts = format_datetime_literal(
+            HIGH_TS, sql_client.capabilities.timestamp_precision
+        )
+
+        # retire updated and deleted records
+        sql.append(f"""
+            UPDATE {root_table_name} SET {to} = '{boundary_ts}'
+            WHERE NOT EXISTS (
+                SELECT s.{hash_} FROM {staging_root_table_name} AS s
+                WHERE {root_table_name}.{hash_} = s.{hash_}
+            ) AND {to} = '{active_record_ts}';
+        """)
+
+        # insert new active records in root table
+        columns = map(escape_id, list(root_table["columns"].keys()))
+        col_str = ", ".join([c for c in columns if c not in (from_, to)])
+        sql.append(f"""
+            INSERT INTO {root_table_name} ({col_str}, {from_}, {to})
+            SELECT {col_str}, '{boundary_ts}' AS {from_}, '{active_record_ts}' AS {to}
+            FROM {staging_root_table_name} AS s
+            WHERE NOT EXISTS (SELECT s.{hash_} FROM {root_table_name} AS f WHERE f.{hash_} = s.{hash_});
+        """)
+
+        # insert list elements for new active records in child tables
+        child_tables = table_chain[1:]
+        if child_tables:
+            unique_column: str = None
+            # use unique hint to create temp table with all identifiers to delete
+            unique_columns = get_columns_names_with_prop(root_table, "unique")
+            if not unique_columns:
+                raise MergeDispositionException(
+                    sql_client.fully_qualified_dataset_name(),
+                    staging_root_table_name,
+                    [t["name"] for t in table_chain],
+                    f"There is no unique column (ie _dlt_id) in top table {root_table['name']} so"
+                    " it is not possible to link child tables to it.",
+                )
+            # get first unique column
+            unique_column = escape_id(unique_columns[0])
+            # TODO: - based on deterministic child hashes (OK)
+            # - if row hash changes all is right
+            # - if it does not we only capture new records, while we should replace existing with those in stage
+            # - this write disposition is way more similar to regular merge (how root tables are handled is different, other tables handled same)
+            for table in child_tables:
+                table_name = sql_client.make_qualified_table_name(table["name"])
+                with sql_client.with_staging_dataset(staging=True):
+                    staging_table_name = sql_client.make_qualified_table_name(table["name"])
+                sql.append(f"""
+                    INSERT INTO {table_name}
+                    SELECT *
+                    FROM {staging_table_name} AS s
+                    WHERE NOT EXISTS (SELECT 1 FROM {table_name} AS f WHERE f.{unique_column} = s.{unique_column});
+                """)
+        return sql
```

### Comparing `dlt-0.4.8a1/dlt/destinations/type_mapping.py` & `dlt-0.4.9a0/dlt/destinations/type_mapping.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/destinations/typing.py` & `dlt-0.4.9a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/__init__.py` & `dlt-0.4.9a0/dlt/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/concurrency.py` & `dlt-0.4.9a0/dlt/extract/concurrency.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/decorators.py` & `dlt-0.4.9a0/dlt/extract/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 from dlt.common.exceptions import ArgumentsOverloadException
 from dlt.common.pipeline import PipelineContext
 from dlt.common.schema.utils import DEFAULT_WRITE_DISPOSITION
 from dlt.common.source import _SOURCES, SourceInfo
 from dlt.common.schema.schema import Schema
 from dlt.common.schema.typing import (
     TColumnNames,
-    TTableSchemaColumns,
     TWriteDisposition,
+    TWriteDispositionConfig,
     TAnySchemaColumns,
     TSchemaContract,
     TTableFormat,
 )
 from dlt.extract.hints import make_hints
 from dlt.extract.utils import (
     simulate_func_call,
@@ -282,15 +282,15 @@
 
 @overload
 def resource(
     data: Callable[TResourceFunParams, Any],
     /,
     name: str = None,
     table_name: TTableHintTemplate[str] = None,
-    write_disposition: TTableHintTemplate[TWriteDisposition] = None,
+    write_disposition: TTableHintTemplate[TWriteDispositionConfig] = None,
     columns: TTableHintTemplate[TAnySchemaColumns] = None,
     primary_key: TTableHintTemplate[TColumnNames] = None,
     merge_key: TTableHintTemplate[TColumnNames] = None,
     schema_contract: TTableHintTemplate[TSchemaContract] = None,
     table_format: TTableHintTemplate[TTableFormat] = None,
     selected: bool = True,
     spec: Type[BaseConfiguration] = None,
@@ -300,15 +300,15 @@
 
 @overload
 def resource(
     data: None = ...,
     /,
     name: str = None,
     table_name: TTableHintTemplate[str] = None,
-    write_disposition: TTableHintTemplate[TWriteDisposition] = None,
+    write_disposition: TTableHintTemplate[TWriteDispositionConfig] = None,
     columns: TTableHintTemplate[TAnySchemaColumns] = None,
     primary_key: TTableHintTemplate[TColumnNames] = None,
     merge_key: TTableHintTemplate[TColumnNames] = None,
     schema_contract: TTableHintTemplate[TSchemaContract] = None,
     table_format: TTableHintTemplate[TTableFormat] = None,
     selected: bool = True,
     spec: Type[BaseConfiguration] = None,
@@ -318,15 +318,15 @@
 
 @overload
 def resource(
     data: None = ...,
     /,
     name: TTableHintTemplate[str] = None,
     table_name: TTableHintTemplate[str] = None,
-    write_disposition: TTableHintTemplate[TWriteDisposition] = None,
+    write_disposition: TTableHintTemplate[TWriteDispositionConfig] = None,
     columns: TTableHintTemplate[TAnySchemaColumns] = None,
     primary_key: TTableHintTemplate[TColumnNames] = None,
     merge_key: TTableHintTemplate[TColumnNames] = None,
     schema_contract: TTableHintTemplate[TSchemaContract] = None,
     table_format: TTableHintTemplate[TTableFormat] = None,
     selected: bool = True,
     spec: Type[BaseConfiguration] = None,
@@ -337,15 +337,15 @@
 
 @overload
 def resource(
     data: Union[List[Any], Tuple[Any], Iterator[Any]],
     /,
     name: str = None,
     table_name: TTableHintTemplate[str] = None,
-    write_disposition: TTableHintTemplate[TWriteDisposition] = None,
+    write_disposition: TTableHintTemplate[TWriteDispositionConfig] = None,
     columns: TTableHintTemplate[TAnySchemaColumns] = None,
     primary_key: TTableHintTemplate[TColumnNames] = None,
     merge_key: TTableHintTemplate[TColumnNames] = None,
     schema_contract: TTableHintTemplate[TSchemaContract] = None,
     table_format: TTableHintTemplate[TTableFormat] = None,
     selected: bool = True,
     spec: Type[BaseConfiguration] = None,
@@ -354,15 +354,15 @@
 
 
 def resource(
     data: Optional[Any] = None,
     /,
     name: TTableHintTemplate[str] = None,
     table_name: TTableHintTemplate[str] = None,
-    write_disposition: TTableHintTemplate[TWriteDisposition] = None,
+    write_disposition: TTableHintTemplate[TWriteDispositionConfig] = None,
     columns: TTableHintTemplate[TAnySchemaColumns] = None,
     primary_key: TTableHintTemplate[TColumnNames] = None,
     merge_key: TTableHintTemplate[TColumnNames] = None,
     schema_contract: TTableHintTemplate[TSchemaContract] = None,
     table_format: TTableHintTemplate[TTableFormat] = None,
     selected: bool = True,
     spec: Type[BaseConfiguration] = None,
@@ -396,15 +396,17 @@
 
         name (str, optional): A name of the resource that by default also becomes the name of the table to which the data is loaded.
         If not present, the name of the decorated function will be used.
 
         table_name (TTableHintTemplate[str], optional): An table name, if different from `name`.
         This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
 
-        write_disposition (Literal["skip", "append", "replace", "merge"], optional): Controls how to write data to a table. `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
+        write_disposition (TTableHintTemplate[TWriteDispositionConfig], optional): Controls how to write data to a table. Accepts a shorthand string literal or configuration dictionary.
+        Allowed shorthand string literals: `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
+        Write behaviour can be further customized through a configuration dictionary. For example, to obtain an SCD2 table provide `write_disposition={"disposition": "merge", "strategy": "scd2"}`.
         This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
 
         columns (Sequence[TAnySchemaColumns], optional): A list, dict or pydantic model of column schemas.
             Typed dictionary describing column names, data types, write disposition and performance hints that gives you full control over the created table schema.
             This argument also accepts a callable that is used to dynamically create tables for stream-like resources yielding many datatypes.
             When the argument is a pydantic model, the model will be used to validate the data yielded by the resource as well.
```

### Comparing `dlt-0.4.8a1/dlt/extract/exceptions.py` & `dlt-0.4.9a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/extract.py` & `dlt-0.4.9a0/dlt/extract/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import contextlib
 from collections.abc import Sequence as C_Sequence
 from copy import copy
 import itertools
-from typing import List, Set, Dict, Optional, Set, Any
+from typing import Iterator, List, Dict, Any
 import yaml
 
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.resolve import inject_section
 from dlt.common.configuration.specs import ConfigSectionContext, known_sections
-from dlt.common.data_writers import TLoaderFileFormat
-from dlt.common.data_writers.writers import EMPTY_DATA_WRITER_METRICS
+from dlt.common.data_writers.writers import EMPTY_DATA_WRITER_METRICS, TDataItemFormat
 from dlt.common.pipeline import (
     ExtractDataInfo,
     ExtractInfo,
     ExtractMetrics,
     SupportsPipeline,
     WithStepInfo,
     reset_resource_state,
@@ -21,37 +20,38 @@
 from dlt.common.runtime import signals
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.schema import Schema, utils
 from dlt.common.schema.typing import (
     TAnySchemaColumns,
     TColumnNames,
     TSchemaContract,
-    TWriteDisposition,
+    TWriteDispositionConfig,
 )
 from dlt.common.storages import NormalizeStorageConfiguration, LoadPackageInfo, SchemaStorage
 from dlt.common.storages.load_package import ParsedLoadJobFileName
 from dlt.common.utils import get_callable_name, get_full_class_name
 
 from dlt.extract.decorators import SourceInjectableContext, SourceSchemaInjectableContext
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints
 from dlt.extract.incremental import IncrementalResourceWrapper
 from dlt.extract.pipe_iterator import PipeIterator
 from dlt.extract.source import DltSource
 from dlt.extract.resource import DltResource
 from dlt.extract.storage import ExtractStorage
-from dlt.extract.extractors import JsonLExtractor, ArrowExtractor, Extractor
+from dlt.extract.extractors import ObjectExtractor, ArrowExtractor, Extractor
+from dlt.extract.utils import get_data_item_format
 
 
 def data_to_sources(
     data: Any,
     pipeline: SupportsPipeline,
     schema: Schema = None,
     table_name: str = None,
     parent_table_name: str = None,
-    write_disposition: TWriteDisposition = None,
+    write_disposition: TWriteDispositionConfig = None,
     columns: TAnySchemaColumns = None,
     primary_key: TColumnNames = None,
     schema_contract: TSchemaContract = None,
 ) -> List[DltSource]:
     """Creates a list of sources for data items present in `data` and applies specified hints to all resources.
 
     `data` may be a DltSource, DltResource, a list of those or any other data type accepted by pipeline.run
@@ -240,18 +240,18 @@
             "table_metrics": table_metrics,
             "resource_metrics": resource_metrics,
             "dag": source.resources.selected_dag,
             "hints": clean_hints,
         }
 
     def _write_empty_files(
-        self, source: DltSource, extractors: Dict[TLoaderFileFormat, Extractor]
+        self, source: DltSource, extractors: Dict[TDataItemFormat, Extractor]
     ) -> None:
         schema = source.schema
-        json_extractor = extractors["puae-jsonl"]
+        json_extractor = extractors["object"]
         resources_with_items = set().union(*[e.resources_with_items for e in extractors.values()])
         # find REPLACE resources that did not yield any pipe items and create empty jobs for them
         # NOTE: do not include tables that have never seen data
         data_tables = {t["name"]: t for t in schema.data_tables(seen_data_only=True)}
         tables_by_resources = utils.group_tables_by_resource(data_tables)
         for resource in source.resources.selected.values():
             if resource.write_disposition != "replace" or resource.name in resources_with_items:
@@ -292,62 +292,74 @@
         *,
         max_parallel_items: int = None,
         workers: int = None,
         futures_poll_interval: float = None,
     ) -> None:
         schema = source.schema
         collector = self.collector
-        extractors: Dict[TLoaderFileFormat, Extractor] = {
-            "puae-jsonl": JsonLExtractor(
-                load_id, self.extract_storage, schema, collector=collector
+        extractors: Dict[TDataItemFormat, Extractor] = {
+            "object": ObjectExtractor(
+                load_id, self.extract_storage.item_storages["object"], schema, collector=collector
+            ),
+            "arrow": ArrowExtractor(
+                load_id, self.extract_storage.item_storages["arrow"], schema, collector=collector
             ),
-            "arrow": ArrowExtractor(load_id, self.extract_storage, schema, collector=collector),
         }
-        last_item_format: Optional[TLoaderFileFormat] = None
-
+        # make sure we close storage on exception
         with collector(f"Extract {source.name}"):
-            self._step_info_start_load_id(load_id)
-            # yield from all selected pipes
-            with PipeIterator.from_pipes(
-                source.resources.selected_pipes,
-                max_parallel_items=max_parallel_items,
-                workers=workers,
-                futures_poll_interval=futures_poll_interval,
-            ) as pipes:
-                left_gens = total_gens = len(pipes._sources)
-                collector.update("Resources", 0, total_gens)
-                for pipe_item in pipes:
-                    curr_gens = len(pipes._sources)
-                    if left_gens > curr_gens:
-                        delta = left_gens - curr_gens
-                        left_gens -= delta
-                        collector.update("Resources", delta)
-
-                    signals.raise_if_signalled()
-
-                    resource = source.resources[pipe_item.pipe.name]
-                    # Fallback to last item's format or default (puae-jsonl) if the current item is an empty list
-                    item_format = (
-                        Extractor.item_format(pipe_item.item) or last_item_format or "puae-jsonl"
-                    )
-                    extractors[item_format].write_items(resource, pipe_item.item, pipe_item.meta)
-                    last_item_format = item_format
-
-                self._write_empty_files(source, extractors)
-                if left_gens > 0:
-                    # go to 100%
-                    collector.update("Resources", left_gens)
+            with self.manage_writers(load_id, source):
+                # yield from all selected pipes
+                with PipeIterator.from_pipes(
+                    source.resources.selected_pipes,
+                    max_parallel_items=max_parallel_items,
+                    workers=workers,
+                    futures_poll_interval=futures_poll_interval,
+                ) as pipes:
+                    left_gens = total_gens = len(pipes._sources)
+                    collector.update("Resources", 0, total_gens)
+                    for pipe_item in pipes:
+                        curr_gens = len(pipes._sources)
+                        if left_gens > curr_gens:
+                            delta = left_gens - curr_gens
+                            left_gens -= delta
+                            collector.update("Resources", delta)
+                        signals.raise_if_signalled()
+                        resource = source.resources[pipe_item.pipe.name]
+                        item_format = get_data_item_format(pipe_item.item)
+                        extractors[item_format].write_items(
+                            resource, pipe_item.item, pipe_item.meta
+                        )
 
-            # flush all buffered writers
+                    self._write_empty_files(source, extractors)
+                    if left_gens > 0:
+                        # go to 100%
+                        collector.update("Resources", left_gens)
+
+    @contextlib.contextmanager
+    def manage_writers(self, load_id: str, source: DltSource) -> Iterator[ExtractStorage]:
+        self._step_info_start_load_id(load_id)
+        # self.current_source = source
+        try:
+            yield self.extract_storage
+        except Exception:
+            # kill writers without flushing the content
+            self.extract_storage.close_writers(load_id, skip_flush=True)
+            raise
+        else:
             self.extract_storage.close_writers(load_id)
-            # gather metrics
-            self._step_info_complete_load_id(load_id, self._compute_metrics(load_id, source))
-            # remove the metrics of files processed in this extract run
-            # NOTE: there may be more than one extract run per load id: ie. the resource and then dlt state
-            self.extract_storage.remove_closed_files(load_id)
+        finally:
+            # gather metrics when storage is closed
+            self.gather_metrics(load_id, source)
+
+    def gather_metrics(self, load_id: str, source: DltSource) -> None:
+        # gather metrics
+        self._step_info_complete_load_id(load_id, self._compute_metrics(load_id, source))
+        # remove the metrics of files processed in this extract run
+        # NOTE: there may be more than one extract run per load id: ie. the resource and then dlt state
+        self.extract_storage.remove_closed_files(load_id)
 
     def extract(
         self,
         source: DltSource,
         max_parallel_items: int,
         workers: int,
     ) -> str:
```

### Comparing `dlt-0.4.8a1/dlt/extract/extractors.py` & `dlt-0.4.9a0/dlt/extract/extractors.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from copy import copy
 from typing import Set, Dict, Any, Optional, List
 
 from dlt.common import logger
 from dlt.common.configuration.inject import with_config
 from dlt.common.configuration.specs import BaseConfiguration, configspec
 from dlt.common.destination.capabilities import DestinationCapabilitiesContext
-from dlt.common.data_writers import TLoaderFileFormat
 from dlt.common.exceptions import MissingDependencyException
 
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.utils import update_dict_nested
 from dlt.common.typing import TDataItems, TDataItem
 from dlt.common.schema import Schema, utils
 from dlt.common.schema.typing import (
@@ -18,15 +17,15 @@
     TTableSchema,
     TTableSchemaColumns,
     TPartialTableSchema,
 )
 from dlt.extract.hints import HintsMeta
 from dlt.extract.resource import DltResource
 from dlt.extract.items import TableNameMeta
-from dlt.extract.storage import ExtractStorage, ExtractorItemStorage
+from dlt.extract.storage import ExtractorItemStorage
 
 try:
     from dlt.common.libs import pyarrow
     from dlt.common.libs.pyarrow import pyarrow as pa, TAnyArrowItem
 except MissingDependencyException:
     pyarrow = None
     pa = None
@@ -45,65 +44,42 @@
 
 def materialize_schema_item() -> MaterializedEmptyList:
     """Yield this to materialize schema in the destination, even if there's no data."""
     return MaterializedEmptyList()
 
 
 class Extractor:
-    file_format: TLoaderFileFormat
-
     @configspec
     class ExtractorConfiguration(BaseConfiguration):
         _caps: Optional[DestinationCapabilitiesContext] = None
 
     @with_config(spec=ExtractorConfiguration)
     def __init__(
         self,
         load_id: str,
-        storage: ExtractStorage,
+        item_storage: ExtractorItemStorage,
         schema: Schema,
         collector: Collector = NULL_COLLECTOR,
         *,
         _caps: DestinationCapabilitiesContext = None,
     ) -> None:
         self.schema = schema
         self.naming = schema.naming
         self.collector = collector
         self.resources_with_items: Set[str] = set()
         """Tracks resources that received items"""
         self.resources_with_empty: Set[str] = set()
         """Track resources that received empty materialized list"""
         self.load_id = load_id
+        self.item_storage = item_storage
         self._table_contracts: Dict[str, TSchemaContractDict] = {}
         self._filtered_tables: Set[str] = set()
         self._filtered_columns: Dict[str, Dict[str, TSchemaEvolutionMode]] = {}
-        self._storage = storage
         self._caps = _caps or DestinationCapabilitiesContext.generic_capabilities()
 
-    @property
-    def storage(self) -> ExtractorItemStorage:
-        return self._storage.get_storage(self.file_format)
-
-    @staticmethod
-    def item_format(items: TDataItems) -> Optional[TLoaderFileFormat]:
-        """Detect the loader file format of the data items based on type.
-        Currently this is either 'arrow' or 'puae-jsonl'
-
-        Returns:
-            The loader file format or `None` if if can't be detected.
-        """
-        for item in items if isinstance(items, list) else [items]:
-            # Assume all items in list are the same type
-            if (pyarrow and pyarrow.is_arrow_item(item)) or (
-                pandas and isinstance(item, pandas.DataFrame)
-            ):
-                return "arrow"
-            return "puae-jsonl"
-        return None  # Empty list is unknown format
-
     def write_items(self, resource: DltResource, items: TDataItems, meta: Any) -> None:
         """Write `items` to `resource` optionally computing table schemas and revalidating/filtering data"""
         if isinstance(meta, HintsMeta):
             # update the resource with new hints, remove all caches so schema is recomputed
             # and contracts re-applied
             resource.merge_hints(meta.hints, meta.create_table_variant)
             # convert to table meta if created table variant so item is assigned to this table
@@ -117,15 +93,15 @@
             self._write_to_static_table(resource, table_name, items, meta)
         else:
             # table has name or other hints depending on data items
             self._write_to_dynamic_table(resource, items)
 
     def write_empty_items_file(self, table_name: str) -> None:
         table_name = self.naming.normalize_table_identifier(table_name)
-        self.storage.write_empty_items_file(self.load_id, self.schema.name, table_name, None)
+        self.item_storage.write_empty_items_file(self.load_id, self.schema.name, table_name, None)
 
     def _get_static_table_name(self, resource: DltResource, meta: Any) -> Optional[str]:
         if resource._table_name_hint_fun:
             return None
         if isinstance(meta, TableNameMeta):
             table_name = meta.table_name
         else:
@@ -138,19 +114,20 @@
     def _write_item(
         self,
         table_name: str,
         resource_name: str,
         items: TDataItems,
         columns: TTableSchemaColumns = None,
     ) -> None:
-        new_rows_count = self.storage.write_data_item(
+        new_rows_count = self.item_storage.write_data_item(
             self.load_id, self.schema.name, table_name, items, columns
         )
         self.collector.update(table_name, inc=new_rows_count)
-        if new_rows_count > 0:
+        # if there were rows or item was empty arrow table
+        if new_rows_count > 0 or self.__class__ is ArrowExtractor:
             self.resources_with_items.add(resource_name)
         else:
             if isinstance(items, MaterializedEmptyList):
                 self.resources_with_empty.add(resource_name)
 
     def _write_to_dynamic_table(self, resource: DltResource, items: TDataItems) -> None:
         if not isinstance(items, list):
@@ -225,20 +202,29 @@
     def _reset_contracts_cache(self) -> None:
         """Removes all cached contracts, filtered columns and tables"""
         self._table_contracts.clear()
         self._filtered_tables.clear()
         self._filtered_columns.clear()
 
 
-class JsonLExtractor(Extractor):
-    file_format = "puae-jsonl"
+class ObjectExtractor(Extractor):
+    """Extracts Python object data items into typed jsonl"""
+
+    pass
 
 
 class ArrowExtractor(Extractor):
-    file_format = "arrow"
+    """Extracts arrow data items into parquet. Normalizes arrow items column names.
+    Compares the arrow schema to actual dlt table schema to reorder the columns and to
+    insert missing columns (without data).
+
+    We do things that normalizer should do here so we do not need to load and save parquet
+    files again later.
+
+    """
 
     def write_items(self, resource: DltResource, items: TDataItems, meta: Any) -> None:
         static_table_name = self._get_static_table_name(resource, meta)
         items = [
             # 3. remove columns and rows in data contract filters
             # 2. Remove null-type columns from the table(s) as they can't be loaded
             self._apply_contract_filters(
@@ -252,20 +238,27 @@
                     else item
                 )
                 for item in (items if isinstance(items, list) else [items])
             )
         ]
         super().write_items(resource, items, meta)
 
+    def _write_to_static_table(
+        self, resource: DltResource, table_name: str, items: TDataItems, meta: Any
+    ) -> None:
+        # contract cache not supported for arrow tables
+        self._reset_contracts_cache()
+        super()._write_to_static_table(resource, table_name, items, meta)
+
     def _apply_contract_filters(
         self, item: "TAnyArrowItem", resource: DltResource, static_table_name: Optional[str]
     ) -> "TAnyArrowItem":
         """Removes the columns (discard value) or rows (discard rows) as indicated by contract filters."""
         # convert arrow schema names into normalized names
-        rename_mapping = pyarrow.get_normalized_arrow_fields_mapping(item, self.naming)
+        rename_mapping = pyarrow.get_normalized_arrow_fields_mapping(item.schema, self.naming)
         # find matching columns and delete by original name
         table_name = static_table_name or self._get_dynamic_table_name(resource, item)
         filtered_columns = self._filtered_columns.get(table_name)
         if filtered_columns:
             # remove rows where columns have non null values
             # create a mask where rows will be False if any of the specified columns are non-null
             mask = None
@@ -294,50 +287,64 @@
     def _write_item(
         self,
         table_name: str,
         resource_name: str,
         items: TDataItems,
         columns: TTableSchemaColumns = None,
     ) -> None:
-        columns = columns or self.schema.tables[table_name]["columns"]
+        columns = columns or self.schema.get_table_columns(table_name)
         # Note: `items` is always a list here due to the conversion in `write_table`
         items = [
-            pyarrow.normalize_py_arrow_schema(item, columns, self.naming, self._caps)
+            pyarrow.normalize_py_arrow_item(item, columns, self.naming, self._caps)
             for item in items
         ]
+        # write items one by one
         super()._write_item(table_name, resource_name, items, columns)
 
     def _compute_table(
         self, resource: DltResource, items: TDataItems, meta: Any
     ) -> TPartialTableSchema:
-        items = items[0]
-        computed_table = super()._compute_table(resource, items, Any)
+        arrow_table: TTableSchema = None
 
-        # Merge the columns to include primary_key and other hints that may be set on the resource
-        arrow_table = copy(computed_table)
-        arrow_table["columns"] = pyarrow.py_arrow_to_table_schema_columns(items.schema)
-        # normalize arrow table before merging
-        arrow_table = self.schema.normalize_table_identifiers(arrow_table)
-        # issue warnings when overriding computed with arrow
-        for col_name, column in arrow_table["columns"].items():
-            if src_column := computed_table["columns"].get(col_name):
-                for hint_name, hint in column.items():
-                    if (src_hint := src_column.get(hint_name)) is not None:
-                        if src_hint != hint:
-                            logger.warning(
-                                f"In resource: {resource.name}, when merging arrow schema on column"
-                                f" {col_name}. The hint {hint_name} value {src_hint} defined in"
-                                f" resource is overwritten from arrow with value {hint}."
-                            )
-
-        # we must override the columns to preserve the order in arrow table
-        arrow_table["columns"] = update_dict_nested(
-            arrow_table["columns"], computed_table["columns"], keep_dst_values=True
-        )
+        # several arrow tables will update the pipeline schema and we want that earlier
+        # arrow tables override the latter so the resultant schema is the same as if
+        # they are sent separately
+        for item in reversed(items):
+            computed_table = super()._compute_table(resource, item, Any)
+            # Merge the columns to include primary_key and other hints that may be set on the resource
+            if arrow_table:
+                utils.merge_table(computed_table, arrow_table)
+            else:
+                arrow_table = copy(computed_table)
+            arrow_table["columns"] = pyarrow.py_arrow_to_table_schema_columns(item.schema)
+            # normalize arrow table before merging
+            arrow_table = self.schema.normalize_table_identifiers(arrow_table)
+            # issue warnings when overriding computed with arrow
+            override_warn: bool = False
+            for col_name, column in arrow_table["columns"].items():
+                if src_column := computed_table["columns"].get(col_name):
+                    for hint_name, hint in column.items():
+                        if (src_hint := src_column.get(hint_name)) is not None:
+                            if src_hint != hint:
+                                override_warn = True
+                                logger.info(
+                                    f"In resource: {resource.name}, when merging arrow schema on"
+                                    f" column {col_name}. The hint {hint_name} value"
+                                    f" {src_hint} defined in resource will overwrite arrow hint"
+                                    f" with value {hint}."
+                                )
+            if override_warn:
+                logger.warning(
+                    f"In resource: {resource.name}, when merging arrow schema with dlt schema,"
+                    " several column hints were different. dlt schema hints were kept and arrow"
+                    " schema and data were unmodified. It is up to destination to coerce the"
+                    " differences when loading. Change log level to INFO for more details."
+                )
 
+            update_dict_nested(arrow_table["columns"], computed_table["columns"])
         return arrow_table
 
     def _compute_and_update_table(
         self, resource: DltResource, table_name: str, items: TDataItems, meta: Any
     ) -> TDataItems:
         items = super()._compute_and_update_table(resource, table_name, items, meta)
         # filter data item as filters could be updated in compute table
```

### Comparing `dlt-0.4.8a1/dlt/extract/hints.py` & `dlt-0.4.9a0/dlt/extract/hints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from copy import copy, deepcopy
 from typing import TypedDict, cast, Any, Optional, Dict
 
+from dlt.common import logger
 from dlt.common.schema.typing import (
     TColumnNames,
     TColumnProp,
     TPartialTableSchema,
     TTableSchema,
     TTableSchemaColumns,
-    TWriteDisposition,
+    TWriteDispositionConfig,
+    TMergeDispositionDict,
     TAnySchemaColumns,
     TTableFormat,
     TSchemaContract,
+    DEFAULT_VALIDITY_COLUMN_NAMES,
 )
-from dlt.common import logger
-from dlt.common.schema.utils import DEFAULT_WRITE_DISPOSITION, merge_column, new_column, new_table
-from dlt.common.typing import TDataItem, DictStrAny, DictStrStr
+from dlt.common.schema.utils import (
+    DEFAULT_WRITE_DISPOSITION,
+    DEFAULT_MERGE_STRATEGY,
+    merge_column,
+    new_column,
+    new_table,
+)
+from dlt.common.typing import TDataItem
 from dlt.common.utils import update_dict_nested
 from dlt.common.validation import validate_dict_ignoring_xkeys
 from dlt.extract.exceptions import (
     DataItemRequiredForDynamicTableHints,
     InconsistentTableTemplate,
 )
 from dlt.extract.incremental import Incremental
@@ -26,15 +34,15 @@
 from dlt.extract.utils import ensure_table_schema_columns, ensure_table_schema_columns_hint
 from dlt.extract.validation import create_item_validator
 
 
 class TResourceHints(TypedDict, total=False):
     name: TTableHintTemplate[str]
     # description: TTableHintTemplate[str]
-    write_disposition: TTableHintTemplate[TWriteDisposition]
+    write_disposition: TTableHintTemplate[TWriteDispositionConfig]
     # table_sealed: Optional[bool]
     parent: TTableHintTemplate[str]
     columns: TTableHintTemplate[TTableSchemaColumns]
     primary_key: TTableHintTemplate[TColumnNames]
     merge_key: TTableHintTemplate[TColumnNames]
     incremental: Incremental[Any]
     schema_contract: TTableHintTemplate[TSchemaContract]
@@ -53,15 +61,15 @@
 
 NATURAL_CALLABLES = ["incremental", "validator", "original_columns"]
 
 
 def make_hints(
     table_name: TTableHintTemplate[str] = None,
     parent_table_name: TTableHintTemplate[str] = None,
-    write_disposition: TTableHintTemplate[TWriteDisposition] = None,
+    write_disposition: TTableHintTemplate[TWriteDispositionConfig] = None,
     columns: TTableHintTemplate[TAnySchemaColumns] = None,
     primary_key: TTableHintTemplate[TColumnNames] = None,
     merge_key: TTableHintTemplate[TColumnNames] = None,
     schema_contract: TTableHintTemplate[TSchemaContract] = None,
     table_format: TTableHintTemplate[TTableFormat] = None,
 ) -> TResourceHints:
     """A convenience function to create resource hints. Accepts both static and dynamic hints based on data.
@@ -127,21 +135,21 @@
         return self._hints.get("name") or self.name if self._hints else self.name
 
     @table_name.setter
     def table_name(self, value: TTableHintTemplate[str]) -> None:
         self.apply_hints(table_name=value)
 
     @property
-    def write_disposition(self) -> TTableHintTemplate[TWriteDisposition]:
+    def write_disposition(self) -> TTableHintTemplate[TWriteDispositionConfig]:
         if self._hints is None or self._hints.get("write_disposition") is None:
             return DEFAULT_WRITE_DISPOSITION
         return self._hints.get("write_disposition")
 
     @write_disposition.setter
-    def write_disposition(self, value: TTableHintTemplate[TWriteDisposition]) -> None:
+    def write_disposition(self, value: TTableHintTemplate[TWriteDispositionConfig]) -> None:
         self.apply_hints(write_disposition=value)
 
     @property
     def columns(self) -> TTableHintTemplate[TTableSchemaColumns]:
         """Gets columns' schema that can be modified in place"""
         return None if self._hints is None else self._hints.get("columns")
 
@@ -172,28 +180,27 @@
             raise DataItemRequiredForDynamicTableHints(self.name)
         # resolve
         resolved_template: TResourceHints = {
             k: self._resolve_hint(item, v)
             for k, v in table_template.items()
             if k not in NATURAL_CALLABLES
         }  # type: ignore
-        table_schema = self._merge_keys(resolved_template)
-        table_schema["resource"] = self.name
+        table_schema = self._create_table_schema(resolved_template, self.name)
         validate_dict_ignoring_xkeys(
             spec=TTableSchema,
             doc=table_schema,
             path=f"new_table/{self.name}",
         )
         return table_schema
 
     def apply_hints(
         self,
         table_name: TTableHintTemplate[str] = None,
         parent_table_name: TTableHintTemplate[str] = None,
-        write_disposition: TTableHintTemplate[TWriteDisposition] = None,
+        write_disposition: TTableHintTemplate[TWriteDispositionConfig] = None,
         columns: TTableHintTemplate[TAnySchemaColumns] = None,
         primary_key: TTableHintTemplate[TColumnNames] = None,
         merge_key: TTableHintTemplate[TColumnNames] = None,
         incremental: Incremental[Any] = None,
         schema_contract: TTableHintTemplate[TSchemaContract] = None,
         additional_table_hints: Optional[Dict[str, TTableHintTemplate[Any]]] = None,
         table_format: TTableHintTemplate[TTableFormat] = None,
@@ -387,25 +394,84 @@
             if key in partial["columns"]:
                 merge_column(partial["columns"][key], {hint: True})  # type: ignore
             else:
                 partial["columns"][key] = new_column(key, nullable=False)
                 partial["columns"][key][hint] = True
 
     @staticmethod
-    def _merge_keys(t_: TResourceHints) -> TPartialTableSchema:
-        """Merges resolved keys into columns"""
-        partial = cast(TPartialTableSchema, t_)
-        # assert not callable(t_["merge_key"])
-        # assert not callable(t_["primary_key"])
-        if "primary_key" in t_:
-            DltResourceHints._merge_key("primary_key", t_.pop("primary_key"), partial)  # type: ignore
-        if "merge_key" in t_:
-            DltResourceHints._merge_key("merge_key", t_.pop("merge_key"), partial)  # type: ignore
+    def _merge_keys(dict_: Dict[str, Any]) -> None:
+        """Merges primary and merge keys into columns in place."""
+
+        if "primary_key" in dict_:
+            DltResourceHints._merge_key("primary_key", dict_.pop("primary_key"), dict_)  # type: ignore
+        if "merge_key" in dict_:
+            DltResourceHints._merge_key("merge_key", dict_.pop("merge_key"), dict_)  # type: ignore
+
+    @staticmethod
+    def _merge_write_disposition_dict(dict_: Dict[str, Any]) -> None:
+        """Merges write disposition dictionary into write disposition shorthand and x-hints in place."""
+
+        if dict_["write_disposition"]["disposition"] == "merge":
+            DltResourceHints._merge_merge_disposition_dict(dict_)
+        # reduce merge disposition from dict to shorthand
+        dict_["write_disposition"] = dict_["write_disposition"]["disposition"]
+
+    @staticmethod
+    def _merge_merge_disposition_dict(dict_: Dict[str, Any]) -> None:
+        """Merges merge disposition dict into x-hints on in place."""
+
+        mddict: TMergeDispositionDict = deepcopy(dict_["write_disposition"])
+        if mddict is not None:
+            dict_["x-merge-strategy"] = (
+                mddict["strategy"] if "strategy" in mddict else DEFAULT_MERGE_STRATEGY
+            )
+            # add columns for `scd2` merge strategy
+            if dict_.get("x-merge-strategy") == "scd2":
+                if mddict.get("validity_column_names") is None:
+                    from_, to = DEFAULT_VALIDITY_COLUMN_NAMES
+                else:
+                    from_, to = mddict["validity_column_names"]
+                dict_["columns"][from_] = {
+                    "name": from_,
+                    "data_type": "timestamp",
+                    "nullable": (
+                        True
+                    ),  # validity columns are empty when first loaded into staging table
+                    "x-valid-from": True,
+                }
+                dict_["columns"][to] = {
+                    "name": to,
+                    "data_type": "timestamp",
+                    "nullable": True,
+                    "x-valid-to": True,
+                }
+                if mddict.get("row_version_column_name") is None:
+                    hash_ = "_dlt_id"
+                else:
+                    hash_ = mddict["row_version_column_name"]
+                dict_["columns"][hash_] = {
+                    "name": hash_,
+                    "nullable": False,
+                    "x-row-version": True,
+                }
+
+    @staticmethod
+    def _create_table_schema(resource_hints: TResourceHints, resource_name: str) -> TTableSchema:
+        """Creates table schema from resource hints and resource name."""
 
-        return partial
+        dict_ = cast(Dict[str, Any], resource_hints)
+        DltResourceHints._merge_keys(dict_)
+        dict_["resource"] = resource_name
+        if "write_disposition" in dict_:
+            if isinstance(dict_["write_disposition"], str):
+                dict_["write_disposition"] = {
+                    "disposition": dict_["write_disposition"]
+                }  # wrap in dict
+            DltResourceHints._merge_write_disposition_dict(dict_)
+        return cast(TTableSchema, dict_)
 
     @staticmethod
     def validate_dynamic_hints(template: TResourceHints) -> None:
         table_name = template.get("name")
         # if any of the hints is a function, then name must be as well.
         if any(
             callable(v) for k, v in template.items() if k not in ["name", *NATURAL_CALLABLES]
```

### Comparing `dlt-0.4.8a1/dlt/extract/incremental/__init__.py` & `dlt-0.4.9a0/dlt/extract/incremental/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from typing_extensions import get_origin, get_args
 
 import inspect
 from functools import wraps
 
 
 import dlt
+from dlt.common import logger
 from dlt.common.exceptions import MissingDependencyException
-from dlt.common import pendulum, logger
+from dlt.common.pendulum import pendulum
 from dlt.common.jsonpath import compile_path
 from dlt.common.typing import (
     TDataItem,
     TDataItems,
     TFun,
     TSortOrder,
     extract_inner_type,
```

### Comparing `dlt-0.4.8a1/dlt/extract/incremental/exceptions.py` & `dlt-0.4.9a0/dlt/extract/incremental/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/incremental/transform.py` & `dlt-0.4.9a0/dlt/extract/incremental/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime, date  # noqa: I251
 from typing import Any, Optional, Set, Tuple, List
 
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.utils import digest128
 from dlt.common.json import json
-from dlt.common import pendulum
+from dlt.common.pendulum import pendulum
 from dlt.common.typing import TDataItem
 from dlt.common.jsonpath import find_values, JSONPathFields, compile_path
 from dlt.extract.incremental.exceptions import (
     IncrementalCursorPathMissing,
     IncrementalPrimaryKeyMissing,
 )
 from dlt.extract.incremental.typing import TCursorValue, LastValueFunc
```

### Comparing `dlt-0.4.8a1/dlt/extract/items.py` & `dlt-0.4.9a0/dlt/extract/items.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/pipe.py` & `dlt-0.4.9a0/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/pipe_iterator.py` & `dlt-0.4.9a0/dlt/extract/pipe_iterator.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/resource.py` & `dlt-0.4.9a0/dlt/extract/resource.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/source.py` & `dlt-0.4.9a0/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/storage.py` & `dlt-0.4.9a0/dlt/extract/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,58 @@
 import os
 from typing import Dict, List
 
-from dlt.common.data_writers import TLoaderFileFormat
-from dlt.common.data_writers.writers import DataWriterMetrics
+from dlt.common.data_writers import TDataItemFormat, DataWriterMetrics, DataWriter, FileWriterSpec
 from dlt.common.schema import Schema
-from dlt.common.schema.typing import TTableSchemaColumns
 from dlt.common.storages import (
     NormalizeStorageConfiguration,
     NormalizeStorage,
     DataItemStorage,
     FileStorage,
     PackageStorage,
     LoadPackageInfo,
+    create_load_id,
 )
 from dlt.common.storages.exceptions import LoadPackageNotFound
-from dlt.common.typing import TDataItems
-from dlt.common.time import precise_time
 from dlt.common.utils import uniq_id
 
 
 class ExtractorItemStorage(DataItemStorage):
-    load_file_type: TLoaderFileFormat
-
-    def __init__(self, package_storage: PackageStorage) -> None:
+    def __init__(self, package_storage: PackageStorage, writer_spec: FileWriterSpec) -> None:
         """Data item storage using `storage` to manage load packages"""
-        super().__init__(self.load_file_type)
+        super().__init__(writer_spec)
         self.package_storage = package_storage
 
     def _get_data_item_path_template(self, load_id: str, _: str, table_name: str) -> str:
         file_name = PackageStorage.build_job_file_name(table_name, "%s")
         file_path = self.package_storage.get_job_file_path(
             load_id, PackageStorage.NEW_JOBS_FOLDER, file_name
         )
         return self.package_storage.storage.make_full_path(file_path)
 
 
-class JsonLExtractorStorage(ExtractorItemStorage):
-    load_file_type: TLoaderFileFormat = "puae-jsonl"
-
-
-class ArrowExtractorStorage(ExtractorItemStorage):
-    load_file_type: TLoaderFileFormat = "arrow"
-
-
 class ExtractStorage(NormalizeStorage):
     """Wrapper around multiple extractor storages with different file formats"""
 
     def __init__(self, config: NormalizeStorageConfiguration) -> None:
         super().__init__(True, config)
         # always create new packages in an unique folder for each instance so
         # extracts are isolated ie. if they fail
         self.new_packages_folder = uniq_id(8)
         self.storage.create_folder(self.new_packages_folder, exists_ok=True)
         self.new_packages = PackageStorage(
             FileStorage(os.path.join(self.storage.storage_path, self.new_packages_folder)), "new"
         )
-        self._item_storages: Dict[TLoaderFileFormat, ExtractorItemStorage] = {
-            "puae-jsonl": JsonLExtractorStorage(self.new_packages),
-            "arrow": ArrowExtractorStorage(self.new_packages),
+        self.item_storages: Dict[TDataItemFormat, ExtractorItemStorage] = {
+            "object": ExtractorItemStorage(
+                self.new_packages, DataWriter.writer_spec_from_file_format("typed-jsonl", "object")
+            ),
+            "arrow": ExtractorItemStorage(
+                self.new_packages, DataWriter.writer_spec_from_file_format("parquet", "arrow")
+            ),
         }
 
     def create_load_package(self, schema: Schema, reuse_exiting_package: bool = True) -> str:
         """Creates a new load package for given `schema` or returns if such package already exists.
 
         You can prevent reuse of the existing package by setting `reuse_exiting_package` to False
         """
@@ -71,35 +62,32 @@
             # TODO: we may cache this mapping but fallback to files is required if pipeline restarts
             load_ids = self.new_packages.list_packages()
             for load_id in load_ids:
                 if self.new_packages.schema_name(load_id) == schema.name:
                     break
                 load_id = None
         if not load_id:
-            load_id = str(precise_time())
+            load_id = create_load_id()
             self.new_packages.create_package(load_id)
         # always save schema
         self.new_packages.save_schema(load_id, schema)
         return load_id
 
-    def get_storage(self, loader_file_format: TLoaderFileFormat) -> ExtractorItemStorage:
-        return self._item_storages[loader_file_format]
-
-    def close_writers(self, load_id: str) -> None:
-        for storage in self._item_storages.values():
-            storage.close_writers(load_id)
+    def close_writers(self, load_id: str, skip_flush: bool = False) -> None:
+        for storage in self.item_storages.values():
+            storage.close_writers(load_id, skip_flush=skip_flush)
 
     def closed_files(self, load_id: str) -> List[DataWriterMetrics]:
         files = []
-        for storage in self._item_storages.values():
+        for storage in self.item_storages.values():
             files.extend(storage.closed_files(load_id))
         return files
 
     def remove_closed_files(self, load_id: str) -> None:
-        for storage in self._item_storages.values():
+        for storage in self.item_storages.values():
             storage.remove_closed_files(load_id)
 
     def commit_new_load_package(self, load_id: str, schema: Schema) -> None:
         self.new_packages.save_schema(load_id, schema)
         self.storage.rename_tree(
             os.path.join(self.new_packages_folder, self.new_packages.get_package_path(load_id)),
             os.path.join(
@@ -113,20 +101,7 @@
 
     def get_load_package_info(self, load_id: str) -> LoadPackageInfo:
         """Returns information on temp and extracted packages"""
         try:
             return self.new_packages.get_load_package_info(load_id)
         except LoadPackageNotFound:
             return self.extracted_packages.get_load_package_info(load_id)
-
-    def write_data_item(
-        self,
-        file_format: TLoaderFileFormat,
-        load_id: str,
-        schema_name: str,
-        table_name: str,
-        item: TDataItems,
-        columns: TTableSchemaColumns,
-    ) -> None:
-        self.get_storage(file_format).write_data_item(
-            load_id, schema_name, table_name, item, columns
-        )
```

### Comparing `dlt-0.4.8a1/dlt/extract/utils.py` & `dlt-0.4.9a0/dlt/extract/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Awaitable,
     Generator,
     Iterator,
 )
 from collections.abc import Mapping as C_Mapping
 from functools import wraps, partial
 
+from dlt.common.data_writers import TDataItemFormat
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.pipeline import reset_resource_state
 from dlt.common.schema.typing import TColumnNames, TAnySchemaColumns, TTableSchemaColumns
 from dlt.common.typing import AnyFun, DictStrAny, TDataItem, TDataItems, TAnyFunOrGenerator
 from dlt.common.utils import get_callable_name
 
 from dlt.extract.exceptions import (
@@ -38,14 +39,49 @@
 
 try:
     from dlt.common.libs import pydantic
 except MissingDependencyException:
     pydantic = None
 
 
+try:
+    from dlt.common.libs import pyarrow
+except MissingDependencyException:
+    pyarrow = None
+
+try:
+    from dlt.common.libs.pandas import pandas
+except MissingDependencyException:
+    pandas = None
+
+
+def get_data_item_format(items: TDataItems) -> TDataItemFormat:
+    """Detect the format of the data item from `items`.
+
+    Reverts to `object` for empty lists
+
+    Returns:
+        The data file format.
+    """
+    if not pyarrow and not pandas:
+        return "object"
+
+    # Assume all items in list are the same type
+    try:
+        if isinstance(items, list):
+            items = items[0]
+        if (pyarrow and pyarrow.is_arrow_item(items)) or (
+            pandas and isinstance(items, pandas.DataFrame)
+        ):
+            return "arrow"
+    except IndexError:
+        pass
+    return "object"
+
+
 def resolve_column_value(
     column_hint: TTableHintTemplate[TColumnNames], item: TDataItem
 ) -> Union[Any, List[Any]]:
     """Extract values from the data item given a column hint.
     Returns either a single value or list of values when hint is a composite.
     """
     columns = column_hint(item) if callable(column_hint) else column_hint
```

### Comparing `dlt-0.4.8a1/dlt/extract/validation.py` & `dlt-0.4.9a0/dlt/extract/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/extract/wrappers.py` & `dlt-0.4.9a0/dlt/extract/wrappers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/airflow_helper.py` & `dlt-0.4.9a0/dlt/helpers/airflow_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,21 @@
     from airflow.operators.dummy import DummyOperator  # type: ignore
     from airflow.operators.python import PythonOperator, get_current_context
 except ModuleNotFoundError:
     raise MissingDependencyException("Airflow", ["apache-airflow>=2.5"])
 
 
 import dlt
-from dlt.common import pendulum
 from dlt.common import logger
+from dlt.common.pendulum import pendulum
 from dlt.common.runtime.telemetry import with_telemetry
-from dlt.common.data_writers import TLoaderFileFormat
-from dlt.common.schema.typing import TWriteDisposition, TSchemaContract
+
+from dlt.common.destination import TLoaderFileFormat
+from dlt.common.schema.typing import TWriteDispositionConfig, TSchemaContract
+
 from dlt.common.utils import uniq_id
 from dlt.common.normalizers.naming.snake_case import NamingConvention as SnakeCaseNamingConvention
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.specs.config_providers_context import ConfigProvidersContext
 from dlt.common.runtime.collector import NULL_COLLECTOR
 
 from dlt.extract import DltSource
@@ -161,30 +163,30 @@
         return task_name
 
     def run(
         self,
         pipeline: Pipeline,
         data: Any,
         table_name: str = None,
-        write_disposition: TWriteDisposition = None,
+        write_disposition: TWriteDispositionConfig = None,
         loader_file_format: TLoaderFileFormat = None,
         schema_contract: TSchemaContract = None,
         pipeline_name: str = None,
         **kwargs: Any,
     ) -> PythonOperator:
         """
         Create a task to run the given pipeline with the
         given data in Airflow.
 
         Args:
             pipeline (Pipeline): The pipeline to run
             data (Any): The data to run the pipeline with
             table_name (str, optional): The name of the table to
                 which the data should be loaded within the `dataset`.
-            write_disposition (TWriteDisposition, optional): Same as
+            write_disposition (TWriteDispositionConfig, optional): Same as
                 in `run` command.
             loader_file_format (TLoaderFileFormat, optional):
                 The file format the loader will use to create the
                 load package.
             schema_contract (TSchemaContract, optional): On override
                 for the schema contract settings, this will replace
                 the schema contract settings for all tables in the schema.
@@ -206,28 +208,28 @@
         return PythonOperator(task_id=self._task_name(pipeline, data), python_callable=f, **kwargs)
 
     def _run(
         self,
         pipeline: Pipeline,
         data: Any,
         table_name: str = None,
-        write_disposition: TWriteDisposition = None,
+        write_disposition: TWriteDispositionConfig = None,
         loader_file_format: TLoaderFileFormat = None,
         schema_contract: TSchemaContract = None,
         pipeline_name: str = None,
     ) -> None:
         """Run the given pipeline with the given data.
 
         Args:
             pipeline (Pipeline): The pipeline to run
             data (Any): The data to run the pipeline with
             table_name (str, optional): The name of the
                 table to which the data should be loaded
                 within the `dataset`.
-            write_disposition (TWriteDisposition, optional):
+            write_disposition (TWriteDispositionConfig, optional):
                 Same as in `run` command.
             loader_file_format (TLoaderFileFormat, optional):
                 The file format the loader will use to create
                 the load package.
             schema_contract (TSchemaContract, optional): On
                 override for the schema contract settings,
                 this will replace the schema contract settings
@@ -316,15 +318,15 @@
     def add_run(
         self,
         pipeline: Pipeline,
         data: Any,
         *,
         decompose: Literal["none", "serialize", "parallel", "parallel-isolated"] = "none",
         table_name: str = None,
-        write_disposition: TWriteDisposition = None,
+        write_disposition: TWriteDispositionConfig = None,
         loader_file_format: TLoaderFileFormat = None,
         schema_contract: TSchemaContract = None,
         **kwargs: Any,
     ) -> List[PythonOperator]:
         """Creates a task or a group of tasks to run `data` with `pipeline`
 
         Creates an Airflow task that extracts, normalizes and loads `data` with the passed pipeline instance `pipeline`. If `data` is a source
@@ -354,15 +356,15 @@
                 NOTE: In case the SequentialExecutor is used by Airflow, the tasks
                       will remain sequential despite 'parallel' or 'parallel-isolated' mode.
                       Use another executor (e.g. CeleryExecutor) to make tasks parallel!
 
                 Parallel tasks are executed in different pipelines, all derived from the original
                 one, but with the state isolated from each other.
             table_name: (str): The name of the table to which the data should be loaded within the `dataset`
-            write_disposition (TWriteDisposition, optional): Same as in `run` command. Defaults to None.
+            write_disposition (TWriteDispositionConfig, optional): Same as in `run` command. Defaults to None.
             loader_file_format (Literal["jsonl", "insert_values", "parquet"], optional): The file format the loader will use to create the load package.
                 Not all file_formats are compatible with all destinations. Defaults to the preferred file format of the selected destination.
             schema_contract (TSchemaContract, optional): On override for the schema contract settings,
                 this will replace the schema contract settings for all tables in the schema. Defaults to None.
 
         Returns:
             Any: Airflow tasks created in order of creation.
```

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt/__init__.py` & `dlt-0.4.9a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt/configuration.py` & `dlt-0.4.9a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.4.9a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import logging
 from typing import Any, Sequence, Optional, Union
 import warnings
 
-from dlt.common import json, logger
+from dlt.common import logger
+from dlt.common.json import json
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.typing import StrAny
 
 from dlt.helpers.dbt.exceptions import (
     DBTProcessingError,
     DBTNodeResult,
     IncrementalSchemaOutOfSyncError,
```

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt/exceptions.py` & `dlt-0.4.9a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt/profiles.yml` & `dlt-0.4.9a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt/runner.py` & `dlt-0.4.9a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt_cloud/__init__.py` & `dlt-0.4.9a0/dlt/helpers/dbt_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt_cloud/client.py` & `dlt-0.4.9a0/dlt/helpers/dbt_cloud/client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/dbt_cloud/configuration.py` & `dlt-0.4.9a0/dlt/helpers/dbt_cloud/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/load_info.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/load_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import dlt
 import humanize
 import streamlit as st
 
-from dlt.common import pendulum
+from dlt.common.pendulum import pendulum
 from dlt.helpers.streamlit_app.utils import query_data_live
 from dlt.helpers.streamlit_app.widgets import stat
 
 
 def last_load_info(pipeline: dlt.Pipeline) -> None:
     loads_df = query_data_live(
         pipeline,
```

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/query.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,17 @@
                             st.bar_chart(df)
                         if df.dtypes.shape[0] == 2 and show_charts:
                             # try to import altair charts
                             try:
                                 import altair as alt
                             except ModuleNotFoundError:
                                 raise MissingDependencyException(
-                                    "DLT Streamlit Helpers",
+                                    "dlt Streamlit Helpers",
                                     ["altair"],
-                                    "DLT Helpers for Streamlit should be run within a streamlit"
+                                    "dlt Helpers for Streamlit should be run within a streamlit"
                                     " app.",
                                 )
 
                             # try altair
                             bar_chart = (
                                 alt.Chart(df)
                                 .mark_bar()
```

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/resource_state.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/resource_state.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-import dlt
+from typing import Union
 import streamlit as st
 import yaml
 
-from dlt.common import json
-from dlt.common.libs.pandas import pandas as pd
-from dlt.common.pipeline import resource_state, TSourceState
-from dlt.common.schema.utils import group_tables_by_resource
-from dlt.helpers.streamlit_app.widgets.tags import tag
+import dlt
+from dlt.common.pendulum import pendulum
+
+
+def date_to_iso(
+    dumper: yaml.SafeDumper, data: Union[pendulum.Date, pendulum.DateTime]
+) -> yaml.ScalarNode:
+    return dumper.represent_datetime(data)  # type: ignore[arg-type]
+
+
+yaml.representer.SafeRepresenter.add_representer(pendulum.Date, date_to_iso)  # type: ignore[arg-type]
+yaml.representer.SafeRepresenter.add_representer(pendulum.DateTime, date_to_iso)  # type: ignore[arg-type]
 
 
 def resource_state_info(
     pipeline: dlt.Pipeline,
     schema_name: str,
     resource_name: str,
 ) -> None:
     sources_state = pipeline.state.get("sources") or {}
     schema = sources_state.get(schema_name)
     if not schema:
         st.error(f"Schema with name: {schema_name} is not found")
         return
 
     resource = schema["resources"].get(resource_name)
+
     with st.expander("Resource state", expanded=(resource is None)):
         if not resource:
             st.info(f"{resource_name} is missing resource state")
         else:
             spec = yaml.safe_dump(resource)
             st.code(spec, language="yaml")
```

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/show_data.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/show_data.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/table_hints.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/blocks/table_hints.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/dashboard.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/load_info.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/pages/load_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/theme.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/theme.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/utils.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/color_mode_selector.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/color_mode_selector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/logo.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/logo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/schema.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/stats.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/stats.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/summary.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/summary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/tags.py` & `dlt-0.4.9a0/dlt/helpers/streamlit_app/widgets/tags.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/load/configuration.py` & `dlt-0.4.9a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/load/exceptions.py` & `dlt-0.4.9a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/load/load.py` & `dlt-0.4.9a0/dlt/load/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import contextlib
 from functools import reduce
 import datetime  # noqa: 251
 from typing import Dict, List, Optional, Tuple, Set, Iterator, Iterable
 from concurrent.futures import Executor
 import os
 
-from dlt.common import sleep, logger
+from dlt.common import logger
+from dlt.common.runtime.signals import sleep
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.resolve import inject_section
 from dlt.common.configuration.accessors import config
 from dlt.common.pipeline import (
     LoadInfo,
     LoadMetrics,
     SupportsPipeline,
@@ -82,24 +83,26 @@
         super().__init__()
 
     def create_storage(self, is_storage_owner: bool) -> LoadStorage:
         supported_file_formats = self.capabilities.supported_loader_file_formats
         if self.staging_destination:
             supported_file_formats = (
                 self.staging_destination.capabilities().supported_loader_file_formats
-                + ["reference"]
             )
-        if isinstance(self.get_destination_client(Schema("test")), WithStagingDataset):
-            supported_file_formats += ["sql"]
         load_storage = LoadStorage(
             is_storage_owner,
-            self.capabilities.preferred_loader_file_format,
             supported_file_formats,
             config=self.config._load_storage_config,
         )
+        # add internal job formats
+        if issubclass(self.destination.client_class, WithStagingDataset):
+            load_storage.supported_job_file_formats += ["sql"]
+        if self.staging_destination:
+            load_storage.supported_job_file_formats += ["reference"]
+
         return load_storage
 
     def get_destination_client(self, schema: Schema) -> JobClientBase:
         return self.destination.client(schema, self.initial_client_config)
 
     def get_staging_destination_client(self, schema: Schema) -> JobClientBase:
         return self.staging_destination.client(schema, self.initial_staging_client_config)
@@ -135,15 +138,15 @@
             # if we have a staging destination and the file is not a reference, send to staging
             with (
                 self.get_staging_destination_client(schema)
                 if is_staging_destination_job
                 else job_client
             ) as client:
                 job_info = ParsedLoadJobFileName.parse(file_path)
-                if job_info.file_format not in self.load_storage.supported_file_formats:
+                if job_info.file_format not in self.load_storage.supported_job_file_formats:
                     raise LoadClientUnsupportedFileFormats(
                         job_info.file_format,
                         self.capabilities.supported_loader_file_formats,
                         file_path,
                     )
                 logger.info(f"Will load file {file_path} with table name {job_info.table_name}")
                 table = client.prepare_load_table(job_info.table_name)
@@ -173,14 +176,20 @@
             # if job irreversibly cannot be started, mark it as failed
             logger.exception(f"Terminal problem when adding job {file_path}")
             job = EmptyLoadJob.from_file_path(file_path, "failed", pretty_format_exception())
         except (DestinationTransientException, Exception):
             # return no job so file stays in new jobs (root) folder
             logger.exception(f"Temporary problem when adding job {file_path}")
             job = EmptyLoadJob.from_file_path(file_path, "retry", pretty_format_exception())
+        if job is None:
+            raise DestinationTerminalException(
+                f"Destination could not create a job for file {file_path}. Typically the file"
+                " extension could not be associated with job type and that indicates an error in"
+                " the code."
+            )
         self.load_storage.normalized_packages.start_job(load_id, job.file_name())
         return job
 
     def spool_new_jobs(self, load_id: str, schema: Schema) -> Tuple[int, List[LoadJob]]:
         # use thread based pool as jobs processing is mostly I/O and we do not want to pickle jobs
         load_files = self.load_storage.list_new_jobs(load_id)[: self.config.workers]
         file_count = len(load_files)
```

### Comparing `dlt-0.4.8a1/dlt/load/utils.py` & `dlt-0.4.9a0/dlt/load/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/normalize/configuration.py` & `dlt-0.4.9a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/normalize/items_normalizers.py` & `dlt-0.4.9a0/dlt/normalize/items_normalizers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from typing import List, Dict, Set, Any
 from abc import abstractmethod
 
-from dlt.common import json, logger
+from dlt.common import logger
+from dlt.common.json import json
 from dlt.common.data_writers import DataWriterMetrics
+from dlt.common.data_writers.writers import ArrowToObjectAdapter
 from dlt.common.json import custom_pua_decode, may_have_pua
 from dlt.common.runtime import signals
 from dlt.common.schema.typing import TSchemaEvolutionMode, TTableSchemaColumns, TSchemaContractDict
 from dlt.common.schema.utils import has_table_seen_data
 from dlt.common.storages import (
     NormalizeStorage,
     LoadStorage,
 )
+from dlt.common.storages.data_item_storage import DataItemStorage
 from dlt.common.storages.load_package import ParsedLoadJobFileName
 from dlt.common.typing import DictStrAny, TDataItem
 from dlt.common.schema import TSchemaUpdate, Schema
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.normalizers.utils import generate_dlt_ids
 
 from dlt.normalize.configuration import NormalizeConfiguration
@@ -26,40 +29,40 @@
     pyarrow = None
     pa = None
 
 
 class ItemsNormalizer:
     def __init__(
         self,
-        load_storage: LoadStorage,
+        item_storage: DataItemStorage,
         normalize_storage: NormalizeStorage,
         schema: Schema,
         load_id: str,
         config: NormalizeConfiguration,
     ) -> None:
-        self.load_storage = load_storage
+        self.item_storage = item_storage
         self.normalize_storage = normalize_storage
         self.schema = schema
         self.load_id = load_id
         self.config = config
 
     @abstractmethod
     def __call__(self, extracted_items_file: str, root_table_name: str) -> List[TSchemaUpdate]: ...
 
 
 class JsonLItemsNormalizer(ItemsNormalizer):
     def __init__(
         self,
-        load_storage: LoadStorage,
+        item_storage: DataItemStorage,
         normalize_storage: NormalizeStorage,
         schema: Schema,
         load_id: str,
         config: NormalizeConfiguration,
     ) -> None:
-        super().__init__(load_storage, normalize_storage, schema, load_id, config)
+        super().__init__(item_storage, normalize_storage, schema, load_id, config)
         self._table_contracts: Dict[str, TSchemaContractDict] = {}
         self._filtered_tables: Set[str] = set()
         self._filtered_tables_columns: Dict[str, Dict[str, TSchemaEvolutionMode]] = {}
         # quick access to column schema for writers below
         self._column_schemas: Dict[str, TTableSchemaColumns] = {}
 
     def _filter_columns(
@@ -170,15 +173,15 @@
                         columns = schema.get_table_columns(table_name)
                         column_schemas[table_name] = columns
                     # store row
                     # TODO: store all rows for particular items all together after item is fully completed
                     #   will be useful if we implement bad data sending to a table
                     # we skip write when discovering schema for empty file
                     if not skip_write:
-                        self.load_storage.write_data_item(
+                        self.item_storage.write_data_item(
                             self.load_id, schema_name, table_name, row, columns
                         )
             except StopIteration:
                 pass
             signals.raise_if_signalled()
         return schema_update
 
@@ -207,28 +210,28 @@
                 root_table = self.schema.tables[root_table_name]
                 if not has_table_seen_data(root_table):
                     # if this is a new table, add normalizer columns
                     partial_update = self._normalize_chunk(
                         root_table_name, [{}], False, skip_write=True
                     )
                     schema_updates.append(partial_update)
-                self.load_storage.write_empty_items_file(
+                self.item_storage.write_empty_items_file(
                     self.load_id,
                     self.schema.name,
                     root_table_name,
                     self.schema.get_table_columns(root_table_name),
                 )
                 logger.debug(
                     f"No lines in file {extracted_items_file}, written empty load job file"
                 )
 
         return schema_updates
 
 
-class ParquetItemsNormalizer(ItemsNormalizer):
+class ArrowItemsNormalizer(ItemsNormalizer):
     REWRITE_ROW_GROUPS = 1
 
     def _write_with_dlt_columns(
         self, extracted_items_file: str, root_table_name: str, add_load_id: bool, add_dlt_id: bool
     ) -> List[TSchemaUpdate]:
         new_columns: List[Any] = []
         schema = self.schema
@@ -275,81 +278,129 @@
                     -1,
                     pa.field("_dlt_id", pyarrow.pyarrow.string(), nullable=False),
                     lambda batch: pa.array(generate_dlt_ids(batch.num_rows)),
                 )
             )
 
         items_count = 0
-        as_py = self.load_storage.loader_file_format != "arrow"
+        columns_schema = schema.get_table_columns(root_table_name)
+        # if we use adapter to convert arrow to dicts, then normalization is not necessary
+        is_native_arrow_writer = not issubclass(self.item_storage.writer_cls, ArrowToObjectAdapter)
+        should_normalize: bool = None
         with self.normalize_storage.extracted_packages.storage.open_file(
             extracted_items_file, "rb"
         ) as f:
             for batch in pyarrow.pq_stream_with_new_columns(
                 f, new_columns, row_groups_per_read=self.REWRITE_ROW_GROUPS
             ):
                 items_count += batch.num_rows
-                if as_py:
-                    # Write python rows to jsonl, insert-values, etc... storage
-                    batch = batch.to_pylist()
-                self.load_storage.write_data_item(
+                # we may need to normalize
+                if is_native_arrow_writer and should_normalize is None:
+                    should_normalize, _, _, _ = pyarrow.should_normalize_arrow_schema(
+                        batch.schema, columns_schema, schema.naming
+                    )
+                    if should_normalize:
+                        logger.info(
+                            f"When writing arrow table to {root_table_name} the schema requires"
+                            " normalization because its shape does not match the actual schema of"
+                            " destination table. Arrow table columns will be reordered and missing"
+                            " columns will be added if needed."
+                        )
+                if should_normalize:
+                    batch = pyarrow.normalize_py_arrow_item(
+                        batch, columns_schema, schema.naming, self.config.destination_capabilities
+                    )
+                self.item_storage.write_data_item(
                     load_id,
                     schema.name,
                     root_table_name,
                     batch,
-                    schema.get_table_columns(root_table_name),
+                    columns_schema,
                 )
-        if items_count == 0:
-            self.load_storage.write_empty_items_file(
+        # TODO: better to check if anything is in the buffer and skip writing file
+        if items_count == 0 and not is_native_arrow_writer:
+            self.item_storage.write_empty_items_file(
                 load_id,
                 schema.name,
                 root_table_name,
-                self.schema.get_table_columns(root_table_name),
+                columns_schema,
             )
 
         return [schema_update]
 
-    def _fix_schema_precisions(self, root_table_name: str) -> List[TSchemaUpdate]:
-        """Reduce precision of timestamp columns if needed, according to destination caps"""
+    def _fix_schema_precisions(
+        self, root_table_name: str, arrow_schema: Any
+    ) -> List[TSchemaUpdate]:
+        """Update precision of timestamp columns to the precision of parquet being normalized.
+        Reduce the precision if it is out of range of destination timestamp precision.
+        """
         schema = self.schema
         table = schema.tables[root_table_name]
         max_precision = self.config.destination_capabilities.timestamp_precision
 
         new_cols: TTableSchemaColumns = {}
         for key, column in table["columns"].items():
             if column.get("data_type") in ("timestamp", "time"):
-                if (prec := column.get("precision")) and prec > max_precision:
-                    new_cols[key] = dict(column, precision=max_precision)  # type: ignore[assignment]
-
+                if prec := column.get("precision"):
+                    # apply the arrow schema precision to dlt column schema
+                    data_type = pyarrow.get_column_type_from_py_arrow(arrow_schema.field(key).type)
+                    if data_type["data_type"] in ("timestamp", "time"):
+                        prec = data_type["precision"]
+                    # limit with destination precision
+                    if prec > max_precision:
+                        prec = max_precision
+                    new_cols[key] = dict(column, precision=prec)  # type: ignore[assignment]
         if not new_cols:
             return []
         return [
             {root_table_name: [schema.update_table({"name": root_table_name, "columns": new_cols})]}
         ]
 
     def __call__(self, extracted_items_file: str, root_table_name: str) -> List[TSchemaUpdate]:
-        base_schema_update = self._fix_schema_precisions(root_table_name)
+        # read schema and counts from file metadata
+        from dlt.common.libs.pyarrow import get_parquet_metadata
+
+        with self.normalize_storage.extracted_packages.storage.open_file(
+            extracted_items_file, "rb"
+        ) as f:
+            num_rows, arrow_schema = get_parquet_metadata(f)
+            file_metrics = DataWriterMetrics(extracted_items_file, num_rows, f.tell(), 0, 0)
+        # when parquet files is saved, timestamps will be truncated and coerced. take the updated values
+        # and apply them to dlt schema
+        base_schema_update = self._fix_schema_precisions(root_table_name, arrow_schema)
 
         add_dlt_id = self.config.parquet_normalizer.add_dlt_id
         add_dlt_load_id = self.config.parquet_normalizer.add_dlt_load_id
-
-        if add_dlt_id or add_dlt_load_id or self.load_storage.loader_file_format != "arrow":
+        # if we need to add any columns or the file format is not parquet, we can't just import files
+        must_rewrite = (
+            add_dlt_id or add_dlt_load_id or self.item_storage.writer_spec.file_format != "parquet"
+        )
+        if not must_rewrite:
+            # in rare cases normalization may be needed
+            must_rewrite, _, _, _ = pyarrow.should_normalize_arrow_schema(
+                arrow_schema, self.schema.get_table_columns(root_table_name), self.schema.naming
+            )
+        if must_rewrite:
+            logger.info(
+                f"Table {root_table_name} parquet file {extracted_items_file} must be rewritten:"
+                f" add_dlt_id: {add_dlt_id} add_dlt_load_id: {add_dlt_load_id} destination file"
+                f" format: {self.item_storage.writer_spec.file_format} or due to required"
+                " normalization "
+            )
             schema_update = self._write_with_dlt_columns(
                 extracted_items_file, root_table_name, add_dlt_load_id, add_dlt_id
             )
             return base_schema_update + schema_update
 
-        from dlt.common.libs.pyarrow import get_row_count
-
-        with self.normalize_storage.extracted_packages.storage.open_file(
-            extracted_items_file, "rb"
-        ) as f:
-            file_metrics = DataWriterMetrics(extracted_items_file, get_row_count(f), f.tell(), 0, 0)
-
+        logger.info(
+            f"Table {root_table_name} parquet file {extracted_items_file} will be directly imported"
+            " without normalization"
+        )
         parts = ParsedLoadJobFileName.parse(extracted_items_file)
-        self.load_storage.import_items_file(
+        self.item_storage.import_items_file(
             self.load_id,
             self.schema.name,
             parts.table_name,
             self.normalize_storage.extracted_packages.storage.make_full_path(extracted_items_file),
             file_metrics,
         )
```

### Comparing `dlt-0.4.8a1/dlt/normalize/normalize.py` & `dlt-0.4.9a0/dlt/normalize/normalize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
-import datetime  # noqa: 251
 import itertools
 from typing import Callable, List, Dict, NamedTuple, Sequence, Tuple, Set, Optional
 from concurrent.futures import Future, Executor
 
-from dlt.common import logger, sleep
+from dlt.common import logger
+from dlt.common.runtime.signals import sleep
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
 from dlt.common.configuration.container import Container
-from dlt.common.data_writers import DataWriterMetrics
+from dlt.common.data_writers import DataWriter, DataWriterMetrics, TDataItemFormat
 from dlt.common.data_writers.writers import EMPTY_DATA_WRITER_METRICS
-from dlt.common.destination import TLoaderFileFormat
 from dlt.common.runners import TRunMetrics, Runnable, NullExecutor
 from dlt.common.runtime import signals
 from dlt.common.runtime.collector import Collector, NULL_COLLECTOR
 from dlt.common.schema.typing import TStoredSchema
 from dlt.common.schema.utils import merge_schema_updates
 from dlt.common.storages import (
     NormalizeStorage,
@@ -35,15 +34,15 @@
 from dlt.common.storages.exceptions import LoadPackageNotFound
 from dlt.common.storages.load_package import LoadPackageInfo
 from dlt.common.utils import chunks
 
 from dlt.normalize.configuration import NormalizeConfiguration
 from dlt.normalize.exceptions import NormalizeJobFailed
 from dlt.normalize.items_normalizers import (
-    ParquetItemsNormalizer,
+    ArrowItemsNormalizer,
     JsonLItemsNormalizer,
     ItemsNormalizer,
 )
 
 
 class TWorkerRV(NamedTuple):
     schema_updates: List[TSchemaUpdate]
@@ -85,15 +84,14 @@
         # pass initial normalize storage config embedded in normalize config
         self.normalize_storage = NormalizeStorage(
             True, config=self.config._normalize_storage_config
         )
         # normalize saves in preferred format but can read all supported formats
         self.load_storage = LoadStorage(
             True,
-            self.config.destination_capabilities.preferred_loader_file_format,
             LoadStorage.ALL_SUPPORTED_FILE_FORMATS,
             config=self.config._load_storage_config,
         )
 
     @staticmethod
     def w_normalize_files(
         config: NormalizeConfiguration,
@@ -101,85 +99,115 @@
         loader_storage_config: LoadStorageConfiguration,
         stored_schema: TStoredSchema,
         load_id: str,
         extracted_items_files: Sequence[str],
     ) -> TWorkerRV:
         destination_caps = config.destination_capabilities
         schema_updates: List[TSchemaUpdate] = []
-        item_normalizers: Dict[TLoaderFileFormat, ItemsNormalizer] = {}
-
-        def _create_load_storage(file_format: TLoaderFileFormat) -> LoadStorage:
-            """Creates a load storage for particular file_format"""
-            # TODO: capabilities.supported_*_formats can be None, it should have defaults
-            supported_formats = destination_caps.supported_loader_file_formats or []
-            if file_format == "parquet":
-                if file_format in supported_formats:
-                    supported_formats.append(
-                        "arrow"
-                    )  # TODO: Hack to make load storage use the correct writer
-                    file_format = "arrow"
-                else:
-                    # Use default storage if parquet is not supported to make normalizer fallback to read rows from the file
-                    file_format = (
-                        destination_caps.preferred_loader_file_format
-                        or destination_caps.preferred_staging_file_format
-                    )
-            else:
-                file_format = (
-                    destination_caps.preferred_loader_file_format
-                    or destination_caps.preferred_staging_file_format
-                )
-            return LoadStorage(False, file_format, supported_formats, loader_storage_config)
+        item_normalizers: Dict[TDataItemFormat, ItemsNormalizer] = {}
+        # Use default storage if parquet is not supported to make normalizer fallback to read rows from the file
+        preferred_file_format = (
+            destination_caps.preferred_loader_file_format
+            or destination_caps.preferred_staging_file_format
+        )
+        # TODO: capabilities.supported_*_formats can be None, it should have defaults
+        supported_formats = destination_caps.supported_loader_file_formats or []
 
         # process all files with data items and write to buffered item storage
         with Container().injectable_context(destination_caps):
             schema = Schema.from_stored_schema(stored_schema)
             normalize_storage = NormalizeStorage(False, normalize_storage_config)
+            load_storage = LoadStorage(False, supported_formats, loader_storage_config)
 
-            def _get_items_normalizer(file_format: TLoaderFileFormat) -> ItemsNormalizer:
-                if file_format in item_normalizers:
-                    return item_normalizers[file_format]
-                klass = ParquetItemsNormalizer if file_format == "parquet" else JsonLItemsNormalizer
-                norm = item_normalizers[file_format] = klass(
-                    _create_load_storage(file_format), normalize_storage, schema, load_id, config
+            def _get_items_normalizer(item_format: TDataItemFormat) -> ItemsNormalizer:
+                if item_format in item_normalizers:
+                    return item_normalizers[item_format]
+                item_storage = load_storage.create_item_storage(preferred_file_format, item_format)
+                if item_storage.writer_spec.file_format != preferred_file_format:
+                    logger.warning(
+                        f"For data items yielded as {item_format} job files in format"
+                        f" {preferred_file_format} cannot be created."
+                        f" {item_storage.writer_spec.file_format} jobs will be used instead."
+                    )
+                cls = ArrowItemsNormalizer if item_format == "arrow" else JsonLItemsNormalizer
+                logger.info(
+                    f"Created items normalizer {cls.__name__} with writer"
+                    f" {item_storage.writer_cls.__name__} for item format {item_format} and file"
+                    f" format {item_storage.writer_spec.file_format}"
+                )
+                norm = item_normalizers[item_format] = cls(
+                    item_storage,
+                    normalize_storage,
+                    schema,
+                    load_id,
+                    config,
                 )
                 return norm
 
+            def _gather_metrics_and_close(
+                parsed_fn: ParsedLoadJobFileName, in_exception: bool
+            ) -> List[DataWriterMetrics]:
+                writer_metrics: List[DataWriterMetrics] = []
+                try:
+                    try:
+                        for normalizer in item_normalizers.values():
+                            normalizer.item_storage.close_writers(load_id, skip_flush=in_exception)
+                    except Exception:
+                        # if we had exception during flushing the writers, close them without flushing
+                        if not in_exception:
+                            for normalizer in item_normalizers.values():
+                                normalizer.item_storage.close_writers(load_id, skip_flush=True)
+                        raise
+                    finally:
+                        # always gather metrics
+                        for normalizer in item_normalizers.values():
+                            norm_metrics = normalizer.item_storage.closed_files(load_id)
+                            writer_metrics.extend(norm_metrics)
+                        for normalizer in item_normalizers.values():
+                            normalizer.item_storage.remove_closed_files(load_id)
+                except Exception as exc:
+                    if in_exception:
+                        # swallow exception if we already handle exceptions
+                        return writer_metrics
+                    else:
+                        # enclose the exception during the closing in job failed exception
+                        job_id = parsed_fn.job_id() if parsed_fn else ""
+                        raise NormalizeJobFailed(load_id, job_id, str(exc), writer_metrics)
+                return writer_metrics
+
             parsed_file_name: ParsedLoadJobFileName = None
             try:
                 root_tables: Set[str] = set()
                 for extracted_items_file in extracted_items_files:
                     parsed_file_name = ParsedLoadJobFileName.parse(extracted_items_file)
                     # normalize table name in case the normalization changed
                     # NOTE: this is the best we can do, until a full lineage information is in the schema
                     root_table_name = schema.naming.normalize_table_identifier(
                         parsed_file_name.table_name
                     )
                     root_tables.add(root_table_name)
-                    normalizer = _get_items_normalizer(parsed_file_name.file_format)
+                    normalizer = _get_items_normalizer(
+                        DataWriter.item_format_from_file_extension(parsed_file_name.file_format)
+                    )
                     logger.debug(
                         f"Processing extracted items in {extracted_items_file} in load_id"
                         f" {load_id} with table name {root_table_name} and schema {schema.name}"
                     )
                     partial_updates = normalizer(extracted_items_file, root_table_name)
                     schema_updates.extend(partial_updates)
                     logger.debug(f"Processed file {extracted_items_file}")
             except Exception as exc:
                 job_id = parsed_file_name.job_id() if parsed_file_name else ""
-                raise NormalizeJobFailed(load_id, job_id, str(exc)) from exc
-            finally:
-                for normalizer in item_normalizers.values():
-                    normalizer.load_storage.close_writers(load_id)
-
-        writer_metrics: List[DataWriterMetrics] = []
-        for normalizer in item_normalizers.values():
-            norm_metrics = normalizer.load_storage.closed_files(load_id)
-            writer_metrics.extend(norm_metrics)
-        logger.info(f"Processed all items in {len(extracted_items_files)} files")
-        return TWorkerRV(schema_updates, writer_metrics)
+                writer_metrics = _gather_metrics_and_close(parsed_file_name, in_exception=True)
+                raise NormalizeJobFailed(load_id, job_id, str(exc), writer_metrics) from exc
+            else:
+                writer_metrics = _gather_metrics_and_close(parsed_file_name, in_exception=False)
+
+            logger.info(f"Processed all items in {len(extracted_items_files)} files")
+            return TWorkerRV(schema_updates, writer_metrics)
 
     def update_table(self, schema: Schema, schema_updates: List[TSchemaUpdate]) -> None:
         for schema_update in schema_updates:
             for table_name, table_updates in schema_update.items():
                 logger.info(
                     f"Updating schema for table {table_name} with {len(table_updates)} deltas"
                 )
@@ -229,17 +257,19 @@
 
         while len(tasks) > 0:
             sleep(0.3)
             # operate on copy of the list
             for task in list(tasks):
                 pending, params = task
                 if pending.done():
-                    result: TWorkerRV = (
-                        pending.result()
-                    )  # Exception in task (if any) is raised here
+                    # collect metrics from the exception (if any)
+                    if isinstance(pending.exception(), NormalizeJobFailed):
+                        summary.file_metrics.extend(pending.exception().writer_metrics)  # type: ignore[attr-defined]
+                    # Exception in task (if any) is raised here
+                    result: TWorkerRV = pending.result()
                     try:
                         # gather schema from all manifests, validate consistency and combine
                         self.update_table(schema, result[0])
                         summary.schema_updates.extend(result.schema_updates)
                         summary.file_metrics.extend(result.file_metrics)
                         # update metrics
                         self.collector.update("Files", len(result.file_metrics))
@@ -344,29 +374,33 @@
             },
         )
 
     def spool_schema_files(self, load_id: str, schema: Schema, files: Sequence[str]) -> str:
         # delete existing folder for the case that this is a retry
         self.load_storage.new_packages.delete_package(load_id, not_exists_ok=True)
         # normalized files will go here before being atomically renamed
-        self.load_storage.new_packages.create_package(load_id)
+        self.load_storage.import_extracted_package(
+            load_id, self.normalize_storage.extracted_packages
+        )
         logger.info(f"Created new load package {load_id} on loading volume")
         try:
             # process parallel
             self.spool_files(
                 load_id, schema.clone(update_normalizers=True), self.map_parallel, files
             )
         except CannotCoerceColumnException as exc:
             # schema conflicts resulting from parallel executing
             logger.warning(
                 f"Parallel schema update conflict, switching to single thread ({str(exc)}"
             )
             # start from scratch
             self.load_storage.new_packages.delete_package(load_id)
-            self.load_storage.new_packages.create_package(load_id)
+            self.load_storage.import_extracted_package(
+                load_id, self.normalize_storage.extracted_packages
+            )
             self.spool_files(load_id, schema.clone(update_normalizers=True), self.map_single, files)
 
         return load_id
 
     def run(self, pool: Optional[Executor]) -> TRunMetrics:
         # keep the pool in class instance
         self.pool = pool or NullExecutor()
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/__init__.py` & `dlt-0.4.9a0/dlt/pipeline/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,43 @@
-from typing import Sequence, cast, overload
+from typing import Sequence, Type, cast, overload
+from typing_extensions import TypeVar
 
 from dlt.common.schema import Schema
-from dlt.common.schema.typing import TColumnSchema, TWriteDisposition, TSchemaContract
+from dlt.common.schema.typing import TColumnSchema, TWriteDispositionConfig, TSchemaContract
 
 from dlt.common.typing import TSecretValue, Any
 from dlt.common.configuration import with_config
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.inject import get_orig_args, last_config
 from dlt.common.destination import TLoaderFileFormat, Destination, TDestinationReferenceArg
 from dlt.common.pipeline import LoadInfo, PipelineContext, get_dlt_pipelines_dir
 
 from dlt.pipeline.configuration import PipelineConfiguration, ensure_correct_pipeline_kwargs
 from dlt.pipeline.pipeline import Pipeline
 from dlt.pipeline.progress import _from_name as collector_from_name, TCollectorArg, _NULL_COLLECTOR
 from dlt.pipeline.warnings import credentials_argument_deprecated
 
+TPipeline = TypeVar("TPipeline", bound=Pipeline, default=Pipeline)
+
 
 @overload
 def pipeline(
     pipeline_name: str = None,
     pipelines_dir: str = None,
     pipeline_salt: TSecretValue = None,
     destination: TDestinationReferenceArg = None,
     staging: TDestinationReferenceArg = None,
     dataset_name: str = None,
     import_schema_path: str = None,
     export_schema_path: str = None,
     full_refresh: bool = False,
     credentials: Any = None,
     progress: TCollectorArg = _NULL_COLLECTOR,
-) -> Pipeline:
+    _impl_cls: Type[TPipeline] = Pipeline,  # type: ignore[assignment]
+) -> TPipeline:
     """Creates a new instance of `dlt` pipeline, which moves the data from the source ie. a REST API to a destination ie. database or a data lake.
 
     #### Note:
     The `pipeline` functions allows you to pass the destination name to which the data should be loaded, the name of the dataset and several other options that govern loading of the data.
     The created `Pipeline` object lets you load the data from any source with `run` method or to have more granular control over the loading process with `extract`, `normalize` and `load` methods.
 
     Please refer to the following doc pages
@@ -93,29 +97,30 @@
     staging: TDestinationReferenceArg = None,
     dataset_name: str = None,
     import_schema_path: str = None,
     export_schema_path: str = None,
     full_refresh: bool = False,
     credentials: Any = None,
     progress: TCollectorArg = _NULL_COLLECTOR,
+    _impl_cls: Type[TPipeline] = Pipeline,  # type: ignore[assignment]
     **kwargs: Any,
-) -> Pipeline:
+) -> TPipeline:
     ensure_correct_pipeline_kwargs(pipeline, **kwargs)
     # call without arguments returns current pipeline
     orig_args = get_orig_args(**kwargs)  # original (*args, **kwargs)
     # is any of the arguments different from defaults
     has_arguments = bool(orig_args[0]) or any(orig_args[1].values())
 
     credentials_argument_deprecated("pipeline", credentials, destination)
 
     if not has_arguments:
         context = Container()[PipelineContext]
         # if pipeline instance is already active then return it, otherwise create a new one
         if context.is_active():
-            return cast(Pipeline, context.pipeline())
+            return cast(TPipeline, context.pipeline())
         else:
             pass
 
     # if working_dir not provided use temp folder
     if not pipelines_dir:
         pipelines_dir = get_dlt_pipelines_dir()
 
@@ -125,15 +130,15 @@
     staging = Destination.from_reference(
         staging or kwargs.get("staging_type", None),
         destination_name=kwargs.get("staging_name", None),
     )
 
     progress = collector_from_name(progress)
     # create new pipeline instance
-    p = Pipeline(
+    p = _impl_cls(
         pipeline_name,
         pipelines_dir,
         pipeline_salt,
         destination,
         staging,
         dataset_name,
         credentials,
@@ -192,15 +197,15 @@
     data: Any,
     *,
     destination: TDestinationReferenceArg = None,
     staging: TDestinationReferenceArg = None,
     dataset_name: str = None,
     credentials: Any = None,
     table_name: str = None,
-    write_disposition: TWriteDisposition = None,
+    write_disposition: TWriteDispositionConfig = None,
     columns: Sequence[TColumnSchema] = None,
     schema: Schema = None,
     loader_file_format: TLoaderFileFormat = None,
     schema_contract: TSchemaContract = None,
 ) -> LoadInfo:
     """Loads the data in `data` argument into the destination specified in `destination` and dataset specified in `dataset_name`.
 
@@ -234,15 +239,17 @@
 
         table_name (str, optional): The name of the table to which the data should be loaded within the `dataset`. This argument is required for a `data` that is a list/Iterable or Iterator without `__name__` attribute.
         The behavior of this argument depends on the type of the `data`:
         * generator functions: the function name is used as table name, `table_name` overrides this default
         * `@dlt.resource`: resource contains the full table schema and that includes the table name. `table_name` will override this property. Use with care!
         * `@dlt.source`: source contains several resources each with a table schema. `table_name` will override all table names within the source and load the data into single table.
 
-        write_disposition (Literal["skip", "append", "replace", "merge"], optional): Controls how to write data to a table. `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
+        write_disposition (TWriteDispositionConfig, optional): Controls how to write data to a table. Accepts a shorthand string literal or configuration dictionary.
+        Allowed shorthand string literals: `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
+        Write behaviour can be further customized through a configuration dictionary. For example, to obtain an SCD2 table provide `write_disposition={"disposition": "merge", "strategy": "scd2"}`.
         Please note that in case of `dlt.resource` the table schema value will be overwritten and in case of `dlt.source`, the values in all resources will be overwritten.
 
         columns (Sequence[TColumnSchema], optional): A list of column schemas. Typed dictionary describing column names, data types, write disposition and performance hints that gives you full control over the created table schema.
 
         schema (Schema, optional): An explicit `Schema` object in which all table schemas will be grouped. By default `dlt` takes the schema from the source (if passed in `data` argument) or creates a default one itself.
 
     Raises:
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/configuration.py` & `dlt-0.4.9a0/dlt/pipeline/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Optional
 
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import RunConfiguration, BaseConfiguration
 from dlt.common.typing import AnyFun, TSecretValue
 from dlt.common.utils import digest256
-from dlt.common.data_writers import TLoaderFileFormat
+from dlt.common.destination import TLoaderFileFormat
 
 
 @configspec
 class PipelineConfiguration(BaseConfiguration):
     pipeline_name: Optional[str] = None
     pipelines_dir: Optional[str] = None
     destination_type: Optional[str] = None
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/current.py` & `dlt-0.4.9a0/dlt/pipeline/current.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/pipeline/dbt.py` & `dlt-0.4.9a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/pipeline/exceptions.py` & `dlt-0.4.9a0/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/pipeline/helpers.py` & `dlt-0.4.9a0/dlt/pipeline/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import contextlib
-from typing import Callable, Sequence, Iterable, Optional, Any, List, Dict, Tuple, Union, TypedDict
+from typing import Callable, Sequence, Iterable, Optional, Any, List, Dict, Union, TypedDict
 from itertools import chain
 
 from dlt.common.jsonpath import resolve_paths, TAnyJsonPath, compile_paths
 from dlt.common.exceptions import TerminalException
 from dlt.common.schema.utils import (
     group_tables_by_resource,
     compile_simple_regexes,
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/pipeline.py` & `dlt-0.4.9a0/dlt/pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     Type,
     cast,
     get_type_hints,
     ContextManager,
 )
 
 from dlt import version
-from dlt.common import json, logger, pendulum
+from dlt.common import logger
+from dlt.common.json import json
+from dlt.common.pendulum import pendulum
 from dlt.common.configuration import inject_section, known_sections
 from dlt.common.configuration.specs import RunConfiguration, CredentialsConfiguration
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import (
     ConfigFieldMissingException,
     ContextDefaultCannotBeCreated,
 )
@@ -38,48 +40,52 @@
 )
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.normalizers import explicit_normalizers, import_normalizers
 from dlt.common.runtime import signals, initialize_runtime
 from dlt.common.schema.typing import (
     TColumnNames,
     TSchemaTables,
-    TWriteDisposition,
+    TWriteDispositionConfig,
     TAnySchemaColumns,
     TSchemaContract,
 )
 from dlt.common.schema.utils import normalize_schema_name
 from dlt.common.storages.exceptions import LoadPackageNotFound
-from dlt.common.typing import DictStrAny, TFun, TSecretValue, is_optional_type
+from dlt.common.typing import TFun, TSecretValue, is_optional_type
 from dlt.common.runners import pool_runner as runner
 from dlt.common.storages import (
     LiveSchemaStorage,
     NormalizeStorage,
     LoadStorage,
     SchemaStorage,
     FileStorage,
     NormalizeStorageConfiguration,
     SchemaStorageConfiguration,
     LoadStorageConfiguration,
     PackageStorage,
     LoadJobInfo,
     LoadPackageInfo,
 )
-from dlt.common.destination import DestinationCapabilitiesContext, TDestination
+from dlt.common.destination import (
+    DestinationCapabilitiesContext,
+    TDestination,
+    ALL_SUPPORTED_FILE_FORMATS,
+    TLoaderFileFormat,
+)
 from dlt.common.destination.reference import (
     DestinationClientDwhConfiguration,
     WithStateSync,
     Destination,
     JobClientBase,
     DestinationClientConfiguration,
     TDestinationReferenceArg,
     DestinationClientStagingConfiguration,
     DestinationClientStagingConfiguration,
     DestinationClientDwhWithStagingConfiguration,
 )
-from dlt.common.destination.capabilities import INTERNAL_LOADER_FILE_FORMATS
 from dlt.common.pipeline import (
     ExtractInfo,
     LoadInfo,
     NormalizeInfo,
     PipelineContext,
     StepInfo,
     TStepInfo,
@@ -88,16 +94,16 @@
     TPipelineState,
     StateInjectableContext,
     TStepMetrics,
     WithStepInfo,
 )
 from dlt.common.schema import Schema
 from dlt.common.utils import is_interactive
-from dlt.common.data_writers import TLoaderFileFormat
 from dlt.common.warnings import deprecated, Dlt04DeprecationWarning
+from dlt.common.versioned_state import json_encode_state, json_decode_state
 
 from dlt.extract import DltSource
 from dlt.extract.exceptions import SourceExhausted
 from dlt.extract.extract import Extract, data_to_sources
 from dlt.normalize import Normalize
 from dlt.normalize.configuration import NormalizeConfiguration
 from dlt.destinations.sql_client import SqlClientBase
@@ -129,16 +135,14 @@
 from dlt.pipeline.state_sync import (
     PIPELINE_STATE_ENGINE_VERSION,
     bump_pipeline_state_version_if_modified,
     load_pipeline_state_from_destination,
     mark_state_extracted,
     migrate_pipeline_state,
     state_resource,
-    json_encode_state,
-    json_decode_state,
     default_pipeline_state,
 )
 from dlt.pipeline.warnings import credentials_argument_deprecated
 from dlt.common.storages.load_package import TLoadPackageState
 
 
 def with_state_sync(may_extract_state: bool = False) -> Callable[[TFun], TFun]:
@@ -386,15 +390,15 @@
     @with_config_section((known_sections.EXTRACT,))
     def extract(
         self,
         data: Any,
         *,
         table_name: str = None,
         parent_table_name: str = None,
-        write_disposition: TWriteDisposition = None,
+        write_disposition: TWriteDispositionConfig = None,
         columns: TAnySchemaColumns = None,
         primary_key: TColumnNames = None,
         schema: Schema = None,
         max_parallel_items: int = None,
         workers: int = None,
         schema_contract: TSchemaContract = None,
     ) -> ExtractInfo:
@@ -429,35 +433,37 @@
                     self._bump_version_and_extract_state(
                         self._container[StateInjectableContext].state, True, extract_step
                     )
                 # commit load packages
                 extract_step.commit_packages()
                 return self._get_step_info(extract_step)
         except Exception as exc:
+            # emit step info
             step_info = self._get_step_info(extract_step)
+            current_load_id = step_info.loads_ids[-1] if len(step_info.loads_ids) > 0 else None
             raise PipelineStepFailed(
                 self,
                 "extract",
-                extract_step.current_load_id,
+                current_load_id,
                 exc,
                 step_info,
             ) from exc
 
     @with_runtime_trace()
     @with_schemas_sync
     @with_config_section((known_sections.NORMALIZE,))
     def normalize(
         self, workers: int = 1, loader_file_format: TLoaderFileFormat = None
     ) -> NormalizeInfo:
         """Normalizes the data prepared with `extract` method, infers the schema and creates load packages for the `load` method. Requires `destination` to be known."""
         if is_interactive():
             workers = 1
 
-        if loader_file_format and loader_file_format in INTERNAL_LOADER_FILE_FORMATS:
-            raise ValueError(f"{loader_file_format} is one of internal dlt file formats.")
+        if loader_file_format and loader_file_format not in ALL_SUPPORTED_FILE_FORMATS:
+            raise ValueError(f"{loader_file_format} is unknown.")
         # check if any schema is present, if not then no data was extracted
         if not self.default_schema_name:
             return None
 
         # make sure destination capabilities are available
         self._get_destination_capabilities()
 
@@ -552,15 +558,15 @@
         data: Any = None,
         *,
         destination: TDestinationReferenceArg = None,
         staging: TDestinationReferenceArg = None,
         dataset_name: str = None,
         credentials: Any = None,
         table_name: str = None,
-        write_disposition: TWriteDisposition = None,
+        write_disposition: TWriteDispositionConfig = None,
         columns: TAnySchemaColumns = None,
         primary_key: TColumnNames = None,
         schema: Schema = None,
         loader_file_format: TLoaderFileFormat = None,
         schema_contract: TSchemaContract = None,
     ) -> LoadInfo:
         """Loads the data from `data` argument into the destination specified in `destination` and dataset specified in `dataset_name`.
@@ -596,15 +602,17 @@
 
             table_name (str, optional): The name of the table to which the data should be loaded within the `dataset`. This argument is required for a `data` that is a list/Iterable or Iterator without `__name__` attribute.
             The behavior of this argument depends on the type of the `data`:
             * generator functions: the function name is used as table name, `table_name` overrides this default
             * `@dlt.resource`: resource contains the full table schema and that includes the table name. `table_name` will override this property. Use with care!
             * `@dlt.source`: source contains several resources each with a table schema. `table_name` will override all table names within the source and load the data into single table.
 
-            write_disposition (Literal["skip", "append", "replace", "merge"], optional): Controls how to write data to a table. `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
+            write_disposition (TWriteDispositionConfig, optional): Controls how to write data to a table. Accepts a shorthand string literal or configuration dictionary.
+            Allowed shorthand string literals: `append` will always add new data at the end of the table. `replace` will replace existing data with new data. `skip` will prevent data from loading. "merge" will deduplicate and merge data based on "primary_key" and "merge_key" hints. Defaults to "append".
+            Write behaviour can be further customized through a configuration dictionary. For example, to obtain an SCD2 table provide `write_disposition={"disposition": "merge", "strategy": "scd2"}`.
             Please note that in case of `dlt.resource` the table schema value will be overwritten and in case of `dlt.source`, the values in all resources will be overwritten.
 
             columns (Sequence[TColumnSchema], optional): A list of column schemas. Typed dictionary describing column names, data types, write disposition and performance hints that gives you full control over the created table schema.
 
             primary_key (str | Sequence[str]): A column name or a list of column names that comprise a private key. Typically used with "merge" write disposition to deduplicate loaded data.
 
             schema (Schema, optional): An explicit `Schema` object in which all table schemas will be grouped. By default `dlt` takes the schema from the source (if passed in `data` argument) or creates a default one itself.
@@ -889,16 +897,15 @@
                 "default_schema_name",
                 "load",
                 "Pipeline contains no schemas. Please extract any data with `extract` or `run`"
                 " methods.",
             )
 
         schema = self.schemas[schema_name] if schema_name else self.default_schema
-        client_config = self._get_destination_client_initial_config(credentials)
-        with self._get_destination_clients(schema, client_config)[0] as client:
+        with self._get_destination_clients(schema)[0] as client:
             client.initialize_storage()
             return client.update_stored_schema()
 
     def set_local_state_val(self, key: str, value: Any) -> None:
         """Sets value in local state. Local state is not synchronized with destination."""
         try:
             # get managed state that is read/write
@@ -946,16 +953,15 @@
         >>> with pipeline.destination_client() as client:
         >>>     client.drop_storage()  # removes storage which typically wipes all data in it
 
         The client is authenticated. You can provide alternative `schema_name` which will be used to normalize dataset name and alternative `credentials`.
         If no schema name is provided and no default schema is present in the pipeline, and ad hoc schema will be created and discarded after use.
         """
         schema = self._get_schema_or_create(schema_name)
-        client_config = self._get_destination_client_initial_config(credentials)
-        return self._get_destination_clients(schema, client_config)[0]
+        return self._get_destination_clients(schema)[0]
 
     def _get_schema_or_create(self, schema_name: str = None) -> Schema:
         if schema_name:
             return self.schemas[schema_name]
         if self.default_schema_name:
             return self.default_schema
         with self._maybe_destination_capabilities():
@@ -972,15 +978,14 @@
     def _get_normalize_storage(self) -> NormalizeStorage:
         return NormalizeStorage(True, self._normalize_storage_config())
 
     def _get_load_storage(self) -> LoadStorage:
         caps = self._get_destination_capabilities()
         return LoadStorage(
             True,
-            caps.preferred_loader_file_format,
             caps.supported_loader_file_formats,
             self._load_storage_config(),
         )
 
     def _normalize_storage_config(self) -> NormalizeStorageConfiguration:
         return NormalizeStorageConfiguration(
             normalize_volume_path=os.path.join(self.working_dir, "normalize")
@@ -1316,15 +1321,15 @@
             else:
                 file_format = possible_file_formats[0] if len(possible_file_formats) > 0 else None
         if file_format not in possible_file_formats:
             raise DestinationIncompatibleLoaderFileFormatException(
                 destination,
                 staging,
                 file_format,
-                set(possible_file_formats) - INTERNAL_LOADER_FILE_FORMATS,
+                set(possible_file_formats),
             )
         return file_format
 
     def _set_default_normalizers(self) -> None:
         _, self._default_naming, _ = import_normalizers(explicit_normalizers())
 
     def _set_dataset_name(self, new_dataset_name: str) -> None:
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/platform.py` & `dlt-0.4.9a0/dlt/pipeline/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Implements SupportsTracking"""
 from typing import Any, cast, TypedDict, List
 import requests
-from dlt.common.managed_thread_pool import ManagedThreadPool
 from urllib.parse import urljoin
 
-from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace, TPipelineStep, SupportsPipeline
-from dlt.common import json
 from dlt.common import logger
+from dlt.common.json import json
 from dlt.common.pipeline import LoadInfo
+from dlt.common.managed_thread_pool import ManagedThreadPool
 from dlt.common.schema.typing import TStoredSchema
 
+from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace, TPipelineStep, SupportsPipeline
+
 _THREAD_POOL: ManagedThreadPool = ManagedThreadPool(1)
 TRACE_URL_SUFFIX = "/trace"
 STATE_URL_SUFFIX = "/state"
 
 
 class TPipelineSyncPayload(TypedDict):
     pipeline_name: str
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/progress.py` & `dlt-0.4.9a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/pipeline/state_sync.py` & `dlt-0.4.9a0/dlt/pipeline/state_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import binascii
 from copy import copy
-from typing import Tuple, cast, List
-import pendulum
+from typing import Tuple, cast
 
 import dlt
-from dlt.common import json
+from dlt.common.pendulum import pendulum
 from dlt.common.typing import DictStrAny
 from dlt.common.schema.typing import STATE_TABLE_NAME, TTableSchemaColumns
 from dlt.common.destination.reference import WithStateSync, Destination
-from dlt.common.utils import compressed_b64decode, compressed_b64encode
 from dlt.common.versioned_state import (
     generate_state_version_hash,
     bump_state_version_if_modified,
     default_versioned_state,
+    compress_state,
+    decompress_state,
 )
 from dlt.common.pipeline import TPipelineState
 
 from dlt.extract import DltResource
 
 from dlt.pipeline.exceptions import (
     PipelineStateEngineNoUpgradePathException,
@@ -35,35 +34,14 @@
         "name": "version_hash",
         "data_type": "text",
         "nullable": True,
     },  # set to nullable so we can migrate existing tables
 }
 
 
-def json_encode_state(state: TPipelineState) -> str:
-    return json.typed_dumps(state)
-
-
-def json_decode_state(state_str: str) -> DictStrAny:
-    return json.typed_loads(state_str)  # type: ignore[no-any-return]
-
-
-def compress_state(state: TPipelineState) -> str:
-    return compressed_b64encode(json.typed_dumpb(state))
-
-
-def decompress_state(state_str: str) -> DictStrAny:
-    try:
-        state_bytes = compressed_b64decode(state_str)
-    except binascii.Error:
-        return json.typed_loads(state_str)  # type: ignore[no-any-return]
-    else:
-        return json.typed_loadb(state_bytes)  # type: ignore[no-any-return]
-
-
 def generate_pipeline_state_version_hash(state: TPipelineState) -> str:
     return generate_state_version_hash(state, exclude_attrs=["_local"])
 
 
 def bump_pipeline_state_version_if_modified(state: TPipelineState) -> Tuple[int, str, str]:
     return bump_state_version_if_modified(state, exclude_attrs=["_local"])
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/trace.py` & `dlt-0.4.9a0/dlt/pipeline/trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import pickle
 import datetime  # noqa: 251
 import dataclasses
 from typing import Any, List, NamedTuple, Optional, Protocol, Sequence
 import humanize
 
-from dlt.common import pendulum, json
+from dlt.common.pendulum import pendulum
 from dlt.common.configuration import is_secret_hint
 from dlt.common.configuration.exceptions import ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.configuration.utils import _RESOLVED_TRACES
 from dlt.common.configuration.container import Container
 from dlt.common.exceptions import ExceptionTrace, ResourceNameNotAvailable
 from dlt.common.logger import suppress_and_warn
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/track.py` & `dlt-0.4.9a0/dlt/pipeline/track.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implements SupportsTracking"""
 import contextlib
 from typing import Any
 import humanize
 
-from dlt.common import pendulum, logger
+from dlt.common import logger
+from dlt.common.pendulum import pendulum
 from dlt.common.utils import digest128
 from dlt.common.runtime.exec_info import github_info
 from dlt.common.runtime.segment import track as dlthub_telemetry_track
 from dlt.common.runtime.slack import send_slack_message
 from dlt.common.pipeline import LoadInfo, ExtractInfo, SupportsPipeline
 
 from dlt.pipeline.typing import TPipelineStep
```

### Comparing `dlt-0.4.8a1/dlt/pipeline/warnings.py` & `dlt-0.4.9a0/dlt/pipeline/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/reflection/names.py` & `dlt-0.4.9a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/reflection/script_inspector.py` & `dlt-0.4.9a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/reflection/script_visitor.py` & `dlt-0.4.9a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/sources/credentials.py` & `dlt-0.4.9a0/dlt/sources/credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/sources/helpers/requests/__init__.py` & `dlt-0.4.9a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/sources/helpers/requests/retry.py` & `dlt-0.4.9a0/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/sources/helpers/requests/session.py` & `dlt-0.4.9a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/sources/helpers/rest_client/__init__.py` & `dlt-0.4.9a0/dlt/sources/helpers/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a1/dlt/sources/helpers/rest_client/auth.py` & `dlt-0.4.9a0/dlt/sources/helpers/rest_client/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,33 @@
     Optional,
     Union,
     Any,
     cast,
     Iterable,
     TYPE_CHECKING,
 )
-from dlt.sources.helpers import requests
 from requests.auth import AuthBase
 from requests import PreparedRequest  # noqa: I251
-import pendulum
-
-from dlt.common.exceptions import MissingDependencyException
 
 from dlt.common import logger
+from dlt.common.exceptions import MissingDependencyException
 from dlt.common.configuration.specs.base_configuration import configspec
 from dlt.common.configuration.specs import CredentialsConfiguration
 from dlt.common.configuration.specs.exceptions import NativeValueError
+from dlt.common.pendulum import pendulum
 from dlt.common.typing import TSecretStrValue
 
+from dlt.sources.helpers import requests
+
 if TYPE_CHECKING:
     from cryptography.hazmat.primitives.asymmetric.types import PrivateKeyTypes
 else:
     PrivateKeyTypes = Any
 
-TApiKeyLocation = Literal[
-    "header", "cookie", "query", "param"
-]  # Alias for scheme "in" field
+TApiKeyLocation = Literal["header", "cookie", "query", "param"]  # Alias for scheme "in" field
 
 
 class AuthConfigBase(AuthBase, CredentialsConfiguration):
     """Authenticator base which is both `requests` friendly AuthBase and dlt SPEC
     configurable via env variables or toml files
     """
 
@@ -98,15 +96,16 @@
             value = list(value)
             if len(value) == 2:
                 self.username, self.password = value
                 return
         raise NativeValueError(
             type(self),
             value,
-            f"HttpBasicAuth username and password must be a tuple of two strings, got {type(value)}",
+            "HttpBasicAuth username and password must be a tuple of two strings, got"
+            f" {type(value)}",
         )
 
     def __call__(self, request: PreparedRequest) -> PreparedRequest:
         encoded = b64encode(f"{self.username}:{self.password}".encode()).decode()
         request.headers["Authorization"] = f"Basic {encoded}"
         return request
 
@@ -143,17 +142,15 @@
     auth_endpoint: str = None
     scopes: Optional[Union[str, List[str]]] = None
     headers: Optional[Dict[str, str]] = None
     private_key_passphrase: Optional[TSecretStrValue] = None
     default_token_expiration: int = 3600
 
     def __post_init__(self) -> None:
-        self.scopes = (
-            self.scopes if isinstance(self.scopes, str) else " ".join(self.scopes)
-        )
+        self.scopes = self.scopes if isinstance(self.scopes, str) else " ".join(self.scopes)
         self.token = None
         self.token_expiry: Optional[pendulum.DateTime] = None
 
     def __call__(self, r: PreparedRequest) -> PreparedRequest:
         if self.token is None or self.is_token_expired():
             self.obtain_token()
         r.headers["Authorization"] = f"Bearer {self.token}"
@@ -167,17 +164,15 @@
             import jwt
         except ModuleNotFoundError:
             raise MissingDependencyException("dlt OAuth helpers", ["PyJWT"])
 
         payload = self.create_jwt_payload()
         data = {
             "grant_type": "urn:ietf:params:oauth:grant-type:jwt-bearer",
-            "assertion": jwt.encode(
-                payload, self.load_private_key(), algorithm="RS256"
-            ),
+            "assertion": jwt.encode(payload, self.load_private_key(), algorithm="RS256"),
         }
 
         logger.debug(f"Obtaining token from {self.auth_endpoint}")
 
         response = requests.post(self.auth_endpoint, headers=self.headers, data=data)
         response.raise_for_status()
 
@@ -204,12 +199,12 @@
             from cryptography.hazmat.primitives import serialization
         except ModuleNotFoundError:
             raise MissingDependencyException("dlt OAuth helpers", ["cryptography"])
 
         private_key_bytes = self.private_key.encode("utf-8")
         return serialization.load_pem_private_key(
             private_key_bytes,
-            password=self.private_key_passphrase.encode("utf-8")
-            if self.private_key_passphrase
-            else None,
+            password=(
+                self.private_key_passphrase.encode("utf-8") if self.private_key_passphrase else None
+            ),
             backend=default_backend(),
         )
```

### Comparing `dlt-0.4.8a1/dlt/sources/helpers/rest_client/client.py` & `dlt-0.4.9a0/dlt/sources/helpers/rest_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     Any,
     TypeVar,
     Iterable,
     cast,
 )
 import copy
 from urllib.parse import urlparse
-
 from requests import Session as BaseSession  # noqa: I251
+from requests import Response, Request
 
-from dlt.common import logger
 from dlt.common import jsonpath
+from dlt.common import logger
+
 from dlt.sources.helpers.requests.retry import Client
-from dlt.sources.helpers.requests import Response, Request
 
 from .typing import HTTPMethodBasic, HTTPMethod, Hooks
 from .paginators import BasePaginator
 from .auth import AuthConfigBase
 from .detector import PaginatorFactory, find_records
 from .exceptions import IgnoreResponseException
 
@@ -131,32 +131,26 @@
             f" with params={request.params}, json={request.json}"
         )
 
         prepared_request = self.session.prepare_request(request)
 
         return self.session.send(prepared_request)
 
-    def request(
-        self, path: str = "", method: HTTPMethod = "GET", **kwargs: Any
-    ) -> Response:
+    def request(self, path: str = "", method: HTTPMethod = "GET", **kwargs: Any) -> Response:
         prepared_request = self._create_request(
             path=path,
             method=method,
             **kwargs,
         )
         return self._send_request(prepared_request)
 
-    def get(
-        self, path: str, params: Optional[Dict[str, Any]] = None, **kwargs: Any
-    ) -> Response:
+    def get(self, path: str, params: Optional[Dict[str, Any]] = None, **kwargs: Any) -> Response:
         return self.request(path, method="GET", params=params, **kwargs)
 
-    def post(
-        self, path: str, json: Optional[Dict[str, Any]] = None, **kwargs: Any
-    ) -> Response:
+    def post(self, path: str, json: Optional[Dict[str, Any]] = None, **kwargs: Any) -> Response:
         return self.request(path, method="POST", json=json, **kwargs)
 
     def paginate(
         self,
         path: str = "",
         method: HTTPMethodBasic = "GET",
         params: Optional[Dict[str, Any]] = None,
@@ -220,24 +214,20 @@
                 paginator = self.detect_paginator(response)
 
             data = self.extract_response(response, data_selector)
             paginator.update_state(response)
             paginator.update_request(request)
 
             # yield data with context
-            yield PageData(
-                data, request=request, response=response, paginator=paginator, auth=auth
-            )
+            yield PageData(data, request=request, response=response, paginator=paginator, auth=auth)
 
             if not paginator.has_next_page:
                 break
 
-    def extract_response(
-        self, response: Response, data_selector: jsonpath.TJsonPath
-    ) -> List[Any]:
+    def extract_response(self, response: Response, data_selector: jsonpath.TJsonPath) -> List[Any]:
         if data_selector:
             # we should compile data_selector
             data: Any = jsonpath.find_values(data_selector, response.json())
             # extract if single item selected
             data = data[0] if isinstance(data, list) and len(data) == 1 else data
         else:
             data = find_records(response.json())
@@ -253,12 +243,10 @@
             response (Response): The response to detect the paginator for.
 
         Returns:
             BasePaginator: The paginator instance that was detected.
         """
         paginator = self.pagination_factory.create_paginator(response)
         if paginator is None:
-            raise ValueError(
-                f"No suitable paginator found for the response at {response.url}"
-            )
+            raise ValueError(f"No suitable paginator found for the response at {response.url}")
         logger.info(f"Detected paginator: {paginator.__class__.__name__}")
         return paginator
```

### Comparing `dlt-0.4.8a1/dlt/sources/helpers/rest_client/detector.py` & `dlt-0.4.9a0/dlt/sources/helpers/rest_client/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List, Dict, Any, Tuple, Union, Optional, Callable, Iterable
 
-from dlt.sources.helpers.requests import Response
+from requests import Response
 
 from .paginators import (
     BasePaginator,
     HeaderLinkPaginator,
     JSONResponsePaginator,
     SinglePagePaginator,
 )
@@ -76,16 +76,15 @@
         # could not detect anything
         return response
     # we are ordered by nesting level, find the most suitable list
     try:
         return next(
             list_info[2]
             for list_info in lists
-            if list_info[1] in RECORD_KEY_PATTERNS
-            and list_info[1] not in NON_RECORD_KEY_PATTERNS
+            if list_info[1] in RECORD_KEY_PATTERNS and list_info[1] not in NON_RECORD_KEY_PATTERNS
         )
     except StopIteration:
         # return the least nested element
         return lists[0][2]
 
 
 def matches_any_pattern(key: str, patterns: Iterable[str]) -> bool:
@@ -138,17 +137,15 @@
 
 def single_page_detector(response: Response) -> Optional[SinglePagePaginator]:
     """This is our fallback paginator, also for results that are single entities"""
     return SinglePagePaginator()
 
 
 class PaginatorFactory:
-    def __init__(
-        self, detectors: List[Callable[[Response], Optional[BasePaginator]]] = None
-    ):
+    def __init__(self, detectors: List[Callable[[Response], Optional[BasePaginator]]] = None):
         if detectors is None:
             detectors = [
                 header_links_detector,
                 json_links_detector,
                 single_page_detector,
             ]
         self.detectors = detectors
```

### Comparing `dlt-0.4.8a1/dlt/sources/helpers/rest_client/paginators.py` & `dlt-0.4.9a0/dlt/sources/helpers/rest_client/paginators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Optional
+from urllib.parse import urlparse, urljoin
 
-from dlt.sources.helpers.requests import Response, Request
+from requests import Response, Request
 from dlt.common import jsonpath
 
 
 class BasePaginator(ABC):
     def __init__(self) -> None:
         self._has_next_page = True
         self._next_reference: Optional[str] = None
@@ -79,16 +80,22 @@
         self.limit = initial_limit
 
     def update_state(self, response: Response) -> None:
         values = jsonpath.find_values(self.total_path, response.json())
         total = values[0] if values else None
 
         if total is None:
+            raise ValueError(f"Total count not found in response for {self.__class__.__name__}")
+
+        try:
+            total = int(total)
+        except ValueError:
             raise ValueError(
-                f"Total count not found in response for {self.__class__.__name__}"
+                f"Total count is not an integer in response for {self.__class__.__name__}. "
+                f"Expected an integer, got {total}"
             )
 
         self.offset += self.limit
 
         if self.offset >= total:
             self._has_next_page = False
 
@@ -98,14 +105,20 @@
 
         request.params[self.offset_param] = self.offset
         request.params[self.limit_param] = self.limit
 
 
 class BaseNextUrlPaginator(BasePaginator):
     def update_request(self, request: Request) -> None:
+        # Handle relative URLs
+        if self.next_reference:
+            parsed_url = urlparse(self.next_reference)
+            if not parsed_url.scheme:
+                self.next_reference = urljoin(request.url, self.next_reference)
+
         request.url = self.next_reference
 
 
 class HeaderLinkPaginator(BaseNextUrlPaginator):
     """A paginator that uses the 'Link' header in HTTP responses
     for pagination.
```

### Comparing `dlt-0.4.8a1/dlt/version.py` & `dlt-0.4.9a0/dlt/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def get_installed_requirement_string(package: str = DLT_PKG_NAME) -> str:
     """Gets the requirement string of currently installed dlt version"""
     dist = pkg_distribution(package)
     # PEP 610 https://packaging.python.org/en/latest/specifications/direct-url/#specification
     direct_url = dist.read_text("direct_url.json")
     if direct_url is not None:
-        from dlt.common import json
+        from dlt.common.json import json
 
         # `url` contain the location of the distribution
         url = urlparse(json.loads(direct_url)["url"])
         # we are interested only in file urls
         if url.scheme == "file":
             return url2pathname(url.path)
```

### Comparing `dlt-0.4.8a1/pyproject.toml` & `dlt-0.4.9a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.4.8a1"
+version = "0.4.9a0"
 description = "dlt is an open-source python-first scalable data loading library that does not require any backend to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -99,14 +99,15 @@
 cli = ["pipdeptree", "cron-descriptor"]
 athena = ["pyathena", "pyarrow", "s3fs", "botocore"]
 weaviate = ["weaviate-client"]
 mssql = ["pyodbc"]
 synapse = ["pyodbc", "adlfs", "pyarrow"]
 qdrant = ["qdrant-client"]
 databricks = ["databricks-sql-connector"]
+dremio = ["pyarrow"]
 
 [tool.poetry.scripts]
 dlt = "dlt.cli._dlt:_main"
 
 [tool.poetry.group.dev.dependencies]
 cffi = "^1.16"
 greenlet = "^3.0.3"
@@ -140,14 +141,15 @@
 types-tqdm = "^4.66.0.2"
 types-psutil = "^5.9.5.16"
 types-psycopg2 = "^2.9.21.14"
 cryptography = "^41.0.7"
 google-api-python-client = ">=1.7.11"
 pytest-asyncio = "^0.23.5"
 types-sqlalchemy = "^1.4.53.38"
+types-pytz = ">=2024.1.0.20240203"
 ruff = "^0.3.2"
 pyjwt = "^2.8.0"
 
 [tool.poetry.group.pipeline]
 optional=true
 
 [tool.poetry.group.pipeline.dependencies]
```

### Comparing `dlt-0.4.8a1/PKG-INFO` & `dlt-0.4.9a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.4.8a1
+Version: 0.4.9a0
 Summary: dlt is an open-source python-first scalable data loading library that does not require any backend to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -24,14 +24,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: athena
 Provides-Extra: az
 Provides-Extra: bigquery
 Provides-Extra: cli
 Provides-Extra: databricks
 Provides-Extra: dbt
+Provides-Extra: dremio
 Provides-Extra: duckdb
 Provides-Extra: filesystem
 Provides-Extra: gcp
 Provides-Extra: gs
 Provides-Extra: motherduck
 Provides-Extra: mssql
 Provides-Extra: parquet
@@ -71,15 +72,15 @@
 Requires-Dist: orjson (>=3.6.7,<=3.9.10) ; platform_python_implementation != "PyPy"
 Requires-Dist: packaging (>=21.1)
 Requires-Dist: pathvalidate (>=2.5.2)
 Requires-Dist: pendulum (>=2.1.2)
 Requires-Dist: pipdeptree (>=2.9.0,<2.10) ; extra == "cli"
 Requires-Dist: psycopg2-binary (>=2.9.1) ; extra == "postgres" or extra == "redshift"
 Requires-Dist: psycopg2cffi (>=2.9.0) ; (platform_python_implementation == "PyPy") and (extra == "postgres" or extra == "redshift")
-Requires-Dist: pyarrow (>=12.0.0) ; extra == "bigquery" or extra == "parquet" or extra == "motherduck" or extra == "athena" or extra == "synapse"
+Requires-Dist: pyarrow (>=12.0.0) ; extra == "bigquery" or extra == "parquet" or extra == "motherduck" or extra == "athena" or extra == "synapse" or extra == "dremio"
 Requires-Dist: pyathena (>=2.9.6) ; extra == "athena"
 Requires-Dist: pyodbc (>=4.0.39,<5.0.0) ; extra == "mssql" or extra == "synapse"
 Requires-Dist: pytz (>=2022.6)
 Requires-Dist: qdrant-client[fastembed] (>=1.6.4,<2.0.0) ; extra == "qdrant"
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: requirements-parser (>=0.5.0)
 Requires-Dist: s3fs (>=2022.4.0) ; extra == "filesystem" or extra == "s3" or extra == "athena"
@@ -207,9 +208,9 @@
 - **Track progress of our work and our plans**: Please check out our [public Github project](https://github.com/orgs/dlt-hub/projects/9)
 - **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.
 - **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.
 - **Improve documentation**: Help us enhance the dlt documentation.
 
 ## License
 
-DLT is released under the [Apache 2.0 License](LICENSE.txt).
+`dlt` is released under the [Apache 2.0 License](LICENSE.txt).
```

