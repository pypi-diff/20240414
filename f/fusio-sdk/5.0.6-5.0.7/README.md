# Comparing `tmp/fusio-sdk-5.0.6.tar.gz` & `tmp/fusio_sdk-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusio-sdk-5.0.6.tar", last modified: Wed Apr 10 21:20:59 2024, max compression
+gzip compressed data, was "fusio_sdk-5.0.7.tar", last modified: Sun Apr 14 18:03:38 2024, max compression
```

## Comparing `fusio-sdk-5.0.6.tar` & `fusio_sdk-5.0.7.tar`

### file list

```diff
@@ -1,278 +1,278 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 21:20:56.000000 fusio-sdk-5.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:20:59.732830 fusio-sdk-5.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 21:20:59.000000 fusio-sdk-5.0.6/src/fusio_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:20:59.776830 fusio-sdk-5.0.6/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/authorization_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_account_change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_response_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_execute_response_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_action_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_audit_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_audit_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_audit_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_backup_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_backup_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_backup_import_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_backup_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_category_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_config_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_config_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_config_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_introspection_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_introspection_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_introspection_entity_row.py
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_connection_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_cronjob_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_dashboard_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_event_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_index_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_index_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_provider_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_provider_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_generator_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_index_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_identity_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log_error_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_collection_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_install.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_local_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_remote_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_marketplace_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_throws.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_operation_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_page_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_plan_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_rate_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_role_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_preview_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_schema_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_category_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8124 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_scope_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_sdk_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_sdk_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_sdk_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_sdk_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_statistic_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_statistic_chart_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_statistic_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_statistic_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_tenant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_data_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_trash_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/backend_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_select.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_form_element_text_area.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_message_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/common_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_account_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_app_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_authorize_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_authorize_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_authorize_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_authorize_response_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_event_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_event_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_grant_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_grant_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_identity_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_identity_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_log_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_page_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_checkout_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_checkout_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_portal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_portal_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_plan_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_plan_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_scope_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_scope_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_token_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_transaction_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_email.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_password_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_user_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/consumer_webhook_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/passthru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_about.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_about_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_about_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_connection_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_meta_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_o_auth_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_payment_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_route.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_route_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_route_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_schema_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_schema_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-10 21:20:55.000000 fusio-sdk-5.0.6/src/sdk/system_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:03:38.663508 fusio_sdk-5.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-14 18:03:38.000000 fusio_sdk-5.0.7/src/fusio_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:03:38.715508 fusio_sdk-5.0.7/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/authorization_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_account_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_execute_response_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_action_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_audit_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_audit_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_audit_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_backup_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_backup_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_backup_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_backup_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_category_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_config_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_config_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_config_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_introspection_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_introspection_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_introspection_entity_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_connection_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_cronjob_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_dashboard_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_event_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_index_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_index_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_provider_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_generator_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_index_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_identity_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log_error_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_collection_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_local_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_marketplace_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_throws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_operation_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_page_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_plan_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_rate_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_role_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_preview_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_schema_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_category_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_scope_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_sdk_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_sdk_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_sdk_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_sdk_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_statistic_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_statistic_chart_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_statistic_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18687 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_statistic_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_tenant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_data_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_trash_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/backend_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_form_element_text_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_message_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/common_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14302 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_account_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_app_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_authorize_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_authorize_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_authorize_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_authorize_response_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_event_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_grant_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_grant_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_identity_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_identity_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_log_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_page_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_checkout_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_checkout_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_portal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_portal_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_plan_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_plan_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_scope_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_scope_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_token_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_transaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_password_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_user_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/consumer_webhook_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/passthru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_about_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_about_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_connection_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_meta_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_o_auth_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_payment_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_route_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_route_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_schema_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_schema_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-14 18:03:34.000000 fusio_sdk-5.0.7/src/sdk/system_tag.py
```

### Comparing `fusio-sdk-5.0.6/LICENSE` & `fusio_sdk-5.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.6/pyproject.toml` & `fusio_sdk-5.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fusio-sdk"
-version = "5.0.6"
+version = "5.0.7"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "SDK to talk to the Fusio REST API"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `fusio-sdk-5.0.6/src/fusio_sdk.egg-info/SOURCES.txt` & `fusio_sdk-5.0.7/src/fusio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusio-sdk-5.0.6/src/sdk/authorization_tag.py` & `fusio_sdk-5.0.7/src/sdk/authorization_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 AuthorizationTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_user import BackendUser
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class AuthorizationTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get_whoami(self) -> BackendUser:
         try:
             path_params = {}
 
             query_params = {}
 
@@ -29,25 +28,23 @@
             url = self.parser.url("/authorization/whoami", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendUser.from_json(response.content)
+                return BackendUser.model_validate_json(json_data=response.content)
 
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def revoke(self) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -55,21 +52,19 @@
             url = self.parser.url("/authorization/revoke", path_params)
 
             headers = {}
 
             response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_account_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_account_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,90 +2,85 @@
 BackendAccountTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_account_change_password import BackendAccountChangePassword
 from .backend_user import BackendUser
 from .backend_user_update import BackendUserUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendAccountTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def change_password(self, payload: BackendAccountChangePassword) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/account/change_password", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, payload: BackendUserUpdate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/account", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self) -> BackendUser:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -93,21 +88,19 @@
             url = self.parser.url("/backend/account", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendUser.from_json(response.content)
+                return BackendUser.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_action_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_scope_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,81 @@
 """
-BackendActionTag automatically generated by SDKgen please do not edit this file manually
+BackendScopeTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_action import BackendAction
-from .backend_action_collection import BackendActionCollection
-from .backend_action_create import BackendActionCreate
-from .backend_action_execute_request import BackendActionExecuteRequest
-from .backend_action_execute_response import BackendActionExecuteResponse
-from .backend_action_index import BackendActionIndex
-from .backend_action_update import BackendActionUpdate
-from .common_form_container import CommonFormContainer
+from .backend_scope import BackendScope
+from .backend_scope_categories import BackendScopeCategories
+from .backend_scope_collection import BackendScopeCollection
+from .backend_scope_create import BackendScopeCreate
+from .backend_scope_update import BackendScopeUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
-class BackendActionTag(sdkgen.TagAbstract):
+class BackendScopeTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, action_id: str) -> CommonMessage:
+    def delete(self, scope_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["action_id"] = action_id
+            path_params["scope_id"] = scope_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/action/$action_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/scope/$scope_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
-            if response.status_code == 404:
+            if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
+            if response.status_code == 404:
+                raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, action_id: str, payload: BackendActionUpdate) -> CommonMessage:
+    def update(self, scope_id: str, payload: BackendScopeUpdate) -> CommonMessage:
         try:
             path_params = {}
-            path_params["action_id"] = action_id
+            path_params["scope_id"] = scope_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/action/$action_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/scope/$scope_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -88,192 +84,123 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, action_id: str) -> BackendAction:
+    def get(self, scope_id: str) -> BackendScope:
         try:
             path_params = {}
-            path_params["action_id"] = action_id
+            path_params["scope_id"] = scope_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/action/$action_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/scope/$scope_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendAction.from_json(response.content)
+                return BackendScope.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def execute(self, action_id: str, payload: BackendActionExecuteRequest) -> BackendActionExecuteResponse:
+    def get_categories(self) -> BackendScopeCategories:
         try:
             path_params = {}
-            path_params["action_id"] = action_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/action/execute/:action_id", path_params)
-
-            headers = {}
-            headers["Content-Type"] = "application/json"
-
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
-
-            if response.status_code >= 200 and response.status_code < 300:
-                return BackendActionExecuteResponse.from_json(response.content)
-
-            if response.status_code == 401:
-                raise CommonMessageException(response.content)
-            if response.status_code == 500:
-                raise CommonMessageException(response.content)
-
-            raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
-        except RequestException as e:
-            raise sdkgen.ClientException("An unknown error occurred: " + str(e))
-
-    pass
-
-    def get_form(self, _class: str) -> CommonFormContainer:
-        try:
-            path_params = {}
-
-            query_params = {}
-            query_params["class"] = _class
-
-            query_struct_names = []
-
-            url = self.parser.url("/backend/action/form", path_params)
+            url = self.parser.url("/backend/scope/categories", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonFormContainer.from_json(response.content)
+                return BackendScopeCategories.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_classes(self) -> BackendActionIndex:
+    def create(self, payload: BackendScopeCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/action/list", path_params)
-
-            headers = {}
-
-            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
-
-            if response.status_code >= 200 and response.status_code < 300:
-                return BackendActionIndex.from_json(response.content)
-
-            if response.status_code == 401:
-                raise CommonMessageException(response.content)
-            if response.status_code == 500:
-                raise CommonMessageException(response.content)
-
-            raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
-        except RequestException as e:
-            raise sdkgen.ClientException("An unknown error occurred: " + str(e))
-
-    pass
-
-    def create(self, payload: BackendActionCreate) -> CommonMessage:
-        try:
-            path_params = {}
-
-            query_params = {}
-
-            query_struct_names = []
-
-            url = self.parser.url("/backend/action", path_params)
+            url = self.parser.url("/backend/scope", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendActionCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> BackendScopeCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/action", path_params)
+            url = self.parser.url("/backend/scope", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendActionCollection.from_json(response.content)
+                return BackendScopeCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_app_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_app_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 BackendAppTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_app import BackendApp
 from .backend_app_collection import BackendAppCollection
 from .backend_app_create import BackendAppCreate
 from .backend_app_update import BackendAppUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendAppTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def delete_token(self, app_id: str, token_id: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["app_id"] = app_id
             path_params["token_id"] = token_id
 
@@ -34,31 +33,29 @@
             url = self.parser.url("/backend/app/$app_id<[0-9]+>/token/:token_id", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def delete(self, app_id: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["app_id"] = app_id
 
             query_params = {}
 
@@ -67,49 +64,47 @@
             url = self.parser.url("/backend/app/$app_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, app_id: str, payload: BackendAppUpdate) -> CommonMessage:
         try:
             path_params = {}
             path_params["app_id"] = app_id
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/app/$app_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -118,16 +113,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self, app_id: str) -> BackendApp:
         try:
             path_params = {}
             path_params["app_id"] = app_id
 
             query_params = {}
 
@@ -136,62 +129,58 @@
             url = self.parser.url("/backend/app/$app_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendApp.from_json(response.content)
+                return BackendApp.model_validate_json(json_data=response.content)
 
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def create(self, payload: BackendAppCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/app", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self, start_index: int, count: int, search: str) -> BackendAppCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -202,21 +191,19 @@
             url = self.parser.url("/backend/app", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendAppCollection.from_json(response.content)
+                return BackendAppCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_audit_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_transaction_tag.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,87 @@
 """
-BackendAuditTag automatically generated by SDKgen please do not edit this file manually
+BackendTransactionTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_audit import BackendAudit
-from .backend_audit_collection import BackendAuditCollection
+from .backend_transaction import BackendTransaction
+from .backend_transaction_collection import BackendTransactionCollection
 from .common_message_exception import CommonMessageException
 
-class BackendAuditTag(sdkgen.TagAbstract):
+class BackendTransactionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def get(self, audit_id: str) -> BackendAudit:
+    def get(self, transaction_id: str) -> BackendTransaction:
         try:
             path_params = {}
-            path_params["audit_id"] = audit_id
+            path_params["transaction_id"] = transaction_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/audit/$audit_id<[0-9]+>", path_params)
+            url = self.parser.url("/backend/transaction/$transaction_id<[0-9]+>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendAudit.from_json(response.content)
+                return BackendTransaction.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str, _from: str, to: str, app_id: int, user_id: int, event: str, ip: str, message: str) -> BackendAuditCollection:
+    def get_all(self, start_index: int, count: int, search: str, from_: str, to: str, plan_id: int, user_id: int, app_id: int, status: str, provider: str) -> BackendTransactionCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
-            query_params["appId"] = app_id
+            query_params["planId"] = plan_id
             query_params["userId"] = user_id
-            query_params["event"] = event
-            query_params["ip"] = ip
-            query_params["message"] = message
+            query_params["appId"] = app_id
+            query_params["status"] = status
+            query_params["provider"] = provider
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/audit", path_params)
+            url = self.parser.url("/backend/transaction", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendAuditCollection.from_json(response.content)
+                return BackendTransactionCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_backup_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_page_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 """
-BackendBackupTag automatically generated by SDKgen please do not edit this file manually
+ConsumerPageTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_backup_export import BackendBackupExport
-from .backend_backup_import import BackendBackupImport
-from .backend_backup_import_result import BackendBackupImportResult
 from .common_message_exception import CommonMessageException
+from .consumer_page import ConsumerPage
+from .consumer_page_collection import ConsumerPageCollection
 
-class BackendBackupTag(sdkgen.TagAbstract):
+class ConsumerPageTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def _import(self, payload: BackendBackupImport) -> BackendBackupImportResult:
+    def get(self, page_id: str) -> ConsumerPage:
         try:
             path_params = {}
+            path_params["page_id"] = page_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/backup/import", path_params)
+            url = self.parser.url("/consumer/page/:page_id", path_params)
 
             headers = {}
-            headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendBackupImportResult.from_json(response.content)
+                return ConsumerPage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
+            if response.status_code == 404:
+                raise CommonMessageException(response.content)
+            if response.status_code == 410:
+                raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def export(self) -> BackendBackupExport:
+    def get_all(self, start_index: int, count: int, search: str) -> ConsumerPageCollection:
         try:
             path_params = {}
 
             query_params = {}
+            query_params["startIndex"] = start_index
+            query_params["count"] = count
+            query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/backup/export", path_params)
+            url = self.parser.url("/consumer/page", path_params)
 
             headers = {}
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendBackupExport.from_json(response.content)
+                return ConsumerPageCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_category_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_category_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 BackendCategoryTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_category import BackendCategory
 from .backend_category_collection import BackendCategoryCollection
 from .backend_category_create import BackendCategoryCreate
 from .backend_category_update import BackendCategoryUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendCategoryTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def delete(self, category_id: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["category_id"] = category_id
 
             query_params = {}
@@ -33,49 +32,47 @@
             url = self.parser.url("/backend/category/$category_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, category_id: str, payload: BackendCategoryUpdate) -> CommonMessage:
         try:
             path_params = {}
             path_params["category_id"] = category_id
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/category/$category_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,16 +81,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self, category_id: str) -> BackendCategory:
         try:
             path_params = {}
             path_params["category_id"] = category_id
 
             query_params = {}
 
@@ -102,62 +97,58 @@
             url = self.parser.url("/backend/category/$category_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendCategory.from_json(response.content)
+                return BackendCategory.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def create(self, payload: BackendCategoryCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/category", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self, start_index: int, count: int, search: str) -> BackendCategoryCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -168,21 +159,19 @@
             url = self.parser.url("/backend/category", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendCategoryCollection.from_json(response.content)
+                return BackendCategoryCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_config_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_config_tag.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 BackendConfigTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_config import BackendConfig
 from .backend_config_collection import BackendConfigCollection
 from .backend_config_update import BackendConfigUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendConfigTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def update(self, config_id: str, payload: BackendConfigUpdate) -> CommonMessage:
         try:
             path_params = {}
             path_params["config_id"] = config_id
 
             query_params = {}
@@ -30,18 +29,18 @@
             query_struct_names = []
 
             url = self.parser.url("/backend/config/$config_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -50,16 +49,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self, config_id: str) -> BackendConfig:
         try:
             path_params = {}
             path_params["config_id"] = config_id
 
             query_params = {}
 
@@ -68,31 +65,29 @@
             url = self.parser.url("/backend/config/$config_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendConfig.from_json(response.content)
+                return BackendConfig.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self, start_index: int, count: int, search: str) -> BackendConfigCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -103,21 +98,19 @@
             url = self.parser.url("/backend/config", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendConfigCollection.from_json(response.content)
+                return BackendConfigCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_connection_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_connection_tag.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 BackendConnectionTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_connection import BackendConnection
 from .backend_connection_collection import BackendConnectionCollection
 from .backend_connection_create import BackendConnectionCreate
 from .backend_connection_index import BackendConnectionIndex
 from .backend_connection_introspection_entities import BackendConnectionIntrospectionEntities
 from .backend_connection_introspection_entity import BackendConnectionIntrospectionEntity
@@ -18,16 +19,14 @@
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendConnectionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get_introspection_for_entity(self, connection_id: str, entity: str) -> BackendConnectionIntrospectionEntity:
         try:
             path_params = {}
             path_params["connection_id"] = connection_id
             path_params["entity"] = entity
 
@@ -38,29 +37,27 @@
             url = self.parser.url("/backend/connection/$connection_id<[0-9]+|^~>/introspection/:entity", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendConnectionIntrospectionEntity.from_json(response.content)
+                return BackendConnectionIntrospectionEntity.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_introspection(self, connection_id: str) -> BackendConnectionIntrospectionEntities:
         try:
             path_params = {}
             path_params["connection_id"] = connection_id
 
             query_params = {}
 
@@ -69,29 +66,27 @@
             url = self.parser.url("/backend/connection/$connection_id<[0-9]+|^~>/introspection", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendConnectionIntrospectionEntities.from_json(response.content)
+                return BackendConnectionIntrospectionEntities.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_redirect(self, connection_id: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["connection_id"] = connection_id
 
             query_params = {}
 
@@ -100,27 +95,25 @@
             url = self.parser.url("/backend/connection/$connection_id<[0-9]+|^~>/redirect", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def delete(self, connection_id: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["connection_id"] = connection_id
 
             query_params = {}
 
@@ -129,49 +122,47 @@
             url = self.parser.url("/backend/connection/$connection_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, connection_id: str, payload: BackendConnectionUpdate) -> CommonMessage:
         try:
             path_params = {}
             path_params["connection_id"] = connection_id
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/connection/$connection_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -180,16 +171,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self, connection_id: str) -> BackendConnection:
         try:
             path_params = {}
             path_params["connection_id"] = connection_id
 
             query_params = {}
 
@@ -198,60 +187,56 @@
             url = self.parser.url("/backend/connection/$connection_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendConnection.from_json(response.content)
+                return BackendConnection.model_validate_json(json_data=response.content)
 
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_form(self, _class: str) -> CommonFormContainer:
+    def get_form(self, class_: str) -> CommonFormContainer:
         try:
             path_params = {}
 
             query_params = {}
-            query_params["class"] = _class
+            query_params["class"] = class_
 
             query_struct_names = []
 
             url = self.parser.url("/backend/connection/form", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonFormContainer.from_json(response.content)
+                return CommonFormContainer.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_classes(self) -> BackendConnectionIndex:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -259,58 +244,54 @@
             url = self.parser.url("/backend/connection/list", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendConnectionIndex.from_json(response.content)
+                return BackendConnectionIndex.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def create(self, payload: BackendConnectionCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/connection", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self, start_index: int, count: int, search: str) -> BackendConnectionCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -321,21 +302,19 @@
             url = self.parser.url("/backend/connection", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendConnectionCollection.from_json(response.content)
+                return BackendConnectionCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_cronjob_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_cronjob_tag.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 BackendCronjobTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_cronjob import BackendCronjob
 from .backend_cronjob_collection import BackendCronjobCollection
 from .backend_cronjob_create import BackendCronjobCreate
 from .backend_cronjob_update import BackendCronjobUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendCronjobTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def delete(self, cronjob_id: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["cronjob_id"] = cronjob_id
 
             query_params = {}
@@ -33,49 +32,47 @@
             url = self.parser.url("/backend/cronjob/$cronjob_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, cronjob_id: str, payload: BackendCronjobUpdate) -> CommonMessage:
         try:
             path_params = {}
             path_params["cronjob_id"] = cronjob_id
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/cronjob/$cronjob_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,16 +81,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self, cronjob_id: str) -> BackendCronjob:
         try:
             path_params = {}
             path_params["cronjob_id"] = cronjob_id
 
             query_params = {}
 
@@ -102,62 +97,58 @@
             url = self.parser.url("/backend/cronjob/$cronjob_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendCronjob.from_json(response.content)
+                return BackendCronjob.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def create(self, payload: BackendCronjobCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/cronjob", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self, start_index: int, count: int, search: str) -> BackendCronjobCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -168,21 +159,19 @@
             url = self.parser.url("/backend/cronjob", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendCronjobCollection.from_json(response.content)
+                return BackendCronjobCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_dashboard_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_dashboard_tag.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 BackendDashboardTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_dashboard import BackendDashboard
 from .common_message_exception import CommonMessageException
 
 class BackendDashboardTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get_all(self) -> BackendDashboard:
         try:
             path_params = {}
 
             query_params = {}
 
@@ -28,21 +27,19 @@
             url = self.parser.url("/backend/dashboard", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendDashboard.from_json(response.content)
+                return BackendDashboard.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_event_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_webhook_tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 """
-BackendEventTag automatically generated by SDKgen please do not edit this file manually
+ConsumerWebhookTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_event import BackendEvent
-from .backend_event_collection import BackendEventCollection
-from .backend_event_create import BackendEventCreate
-from .backend_event_update import BackendEventUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
+from .consumer_webhook import ConsumerWebhook
+from .consumer_webhook_collection import ConsumerWebhookCollection
+from .consumer_webhook_create import ConsumerWebhookCreate
+from .consumer_webhook_update import ConsumerWebhookUpdate
 
-class BackendEventTag(sdkgen.TagAbstract):
+class ConsumerWebhookTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, event_id: str) -> CommonMessage:
+    def delete(self, webhook_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["event_id"] = event_id
+            path_params["webhook_id"] = webhook_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/event/$event_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/webhook/$webhook_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, event_id: str, payload: BackendEventUpdate) -> CommonMessage:
+    def update(self, webhook_id: str, payload: ConsumerWebhookUpdate) -> CommonMessage:
         try:
             path_params = {}
-            path_params["event_id"] = event_id
+            path_params["webhook_id"] = webhook_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/event/$event_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/webhook/$webhook_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,105 +81,97 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, event_id: str) -> BackendEvent:
+    def get(self, webhook_id: str) -> ConsumerWebhook:
         try:
             path_params = {}
-            path_params["event_id"] = event_id
+            path_params["webhook_id"] = webhook_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/event/$event_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/webhook/$webhook_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendEvent.from_json(response.content)
+                return ConsumerWebhook.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def create(self, payload: BackendEventCreate) -> CommonMessage:
+    def create(self, payload: ConsumerWebhookCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/event", path_params)
+            url = self.parser.url("/consumer/webhook", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendEventCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> ConsumerWebhookCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/event", path_params)
+            url = self.parser.url("/consumer/webhook", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendEventCollection.from_json(response.content)
+                return ConsumerWebhookCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_generator_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_generator_tag.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 BackendGeneratorTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_generator_index_providers import BackendGeneratorIndexProviders
 from .backend_generator_provider import BackendGeneratorProvider
 from .backend_generator_provider_changelog import BackendGeneratorProviderChangelog
 from .backend_generator_provider_config import BackendGeneratorProviderConfig
 from .common_form_container import CommonFormContainer
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendGeneratorTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get_changelog(self, provider: str, payload: BackendGeneratorProviderConfig) -> BackendGeneratorProviderChangelog:
         try:
             path_params = {}
             path_params["provider"] = provider
 
             query_params = {}
@@ -32,64 +31,60 @@
             query_struct_names = []
 
             url = self.parser.url("/backend/generator/:provider", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendGeneratorProviderChangelog.from_json(response.content)
+                return BackendGeneratorProviderChangelog.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def execute_provider(self, provider: str, payload: BackendGeneratorProvider) -> CommonMessage:
         try:
             path_params = {}
             path_params["provider"] = provider
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/generator/:provider", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_form(self, provider: str) -> CommonFormContainer:
         try:
             path_params = {}
             path_params["provider"] = provider
 
             query_params = {}
 
@@ -98,29 +93,27 @@
             url = self.parser.url("/backend/generator/:provider", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonFormContainer.from_json(response.content)
+                return CommonFormContainer.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_classes(self) -> BackendGeneratorIndexProviders:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -128,21 +121,19 @@
             url = self.parser.url("/backend/generator", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendGeneratorIndexProviders.from_json(response.content)
+                return BackendGeneratorIndexProviders.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_identity_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_identity_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 BackendIdentityTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_identity import BackendIdentity
 from .backend_identity_collection import BackendIdentityCollection
 from .backend_identity_create import BackendIdentityCreate
 from .backend_identity_index import BackendIdentityIndex
 from .backend_identity_update import BackendIdentityUpdate
 from .common_form_container import CommonFormContainer
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendIdentityTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def delete(self, identity_id: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["identity_id"] = identity_id
 
             query_params = {}
@@ -35,49 +34,47 @@
             url = self.parser.url("/backend/identity/$identity_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, identity_id: str, payload: BackendIdentityUpdate) -> CommonMessage:
         try:
             path_params = {}
             path_params["identity_id"] = identity_id
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/identity/$identity_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -86,16 +83,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self, identity_id: str) -> BackendIdentity:
         try:
             path_params = {}
             path_params["identity_id"] = identity_id
 
             query_params = {}
 
@@ -104,60 +99,56 @@
             url = self.parser.url("/backend/identity/$identity_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendIdentity.from_json(response.content)
+                return BackendIdentity.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_form(self, _class: str) -> CommonFormContainer:
+    def get_form(self, class_: str) -> CommonFormContainer:
         try:
             path_params = {}
 
             query_params = {}
-            query_params["class"] = _class
+            query_params["class"] = class_
 
             query_struct_names = []
 
             url = self.parser.url("/backend/identity/form", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonFormContainer.from_json(response.content)
+                return CommonFormContainer.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_classes(self) -> BackendIdentityIndex:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -165,58 +156,54 @@
             url = self.parser.url("/backend/identity/list", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendIdentityIndex.from_json(response.content)
+                return BackendIdentityIndex.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def create(self, payload: BackendIdentityCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/identity", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self, start_index: int, count: int, search: str) -> BackendIdentityCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -227,21 +214,19 @@
             url = self.parser.url("/backend/identity", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendIdentityCollection.from_json(response.content)
+                return BackendIdentityCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_log_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_log_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 BackendLogTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_log import BackendLog
 from .backend_log_collection import BackendLogCollection
 from .backend_log_error import BackendLogError
 from .backend_log_error_collection import BackendLogErrorCollection
 from .common_message_exception import CommonMessageException
 
 class BackendLogTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get(self, log_id: str) -> BackendLog:
         try:
             path_params = {}
             path_params["log_id"] = log_id
 
             query_params = {}
@@ -32,40 +31,38 @@
             url = self.parser.url("/backend/log/$log_id<[0-9]+>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendLog.from_json(response.content)
+                return BackendLog.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str, _from: str, to: str, route_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendLogCollection:
+    def get_all(self, start_index: int, count: int, search: str, from_: str, to: str, route_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendLogCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["routeId"] = route_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -78,27 +75,25 @@
             url = self.parser.url("/backend/log", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendLogCollection.from_json(response.content)
+                return BackendLogCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_error(self, error_id: str) -> BackendLogError:
         try:
             path_params = {}
             path_params["error_id"] = error_id
 
             query_params = {}
 
@@ -107,27 +102,25 @@
             url = self.parser.url("/backend/log/error/$error_id<[0-9]+>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendLogError.from_json(response.content)
+                return BackendLogError.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all_errors(self, start_index: int, count: int, search: str) -> BackendLogErrorCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -138,21 +131,19 @@
             url = self.parser.url("/backend/log/error", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendLogErrorCollection.from_json(response.content)
+                return BackendLogErrorCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_marketplace_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_marketplace_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 BackendMarketplaceTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_marketplace_collection import BackendMarketplaceCollection
 from .backend_marketplace_install import BackendMarketplaceInstall
 from .backend_marketplace_local_app import BackendMarketplaceLocalApp
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendMarketplaceTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def remove(self, app_name: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["app_name"] = app_name
 
             query_params = {}
@@ -32,29 +31,27 @@
             url = self.parser.url("/backend/marketplace/:app_name", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, app_name: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["app_name"] = app_name
 
             query_params = {}
 
@@ -63,15 +60,15 @@
             url = self.parser.url("/backend/marketplace/:app_name", path_params)
 
             headers = {}
 
             response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -80,16 +77,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self, app_name: str) -> BackendMarketplaceLocalApp:
         try:
             path_params = {}
             path_params["app_name"] = app_name
 
             query_params = {}
 
@@ -98,62 +93,58 @@
             url = self.parser.url("/backend/marketplace/:app_name", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendMarketplaceLocalApp.from_json(response.content)
+                return BackendMarketplaceLocalApp.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def install(self, payload: BackendMarketplaceInstall) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/marketplace", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self) -> BackendMarketplaceCollection:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -161,21 +152,19 @@
             url = self.parser.url("/backend/marketplace", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendMarketplaceCollection.from_json(response.content)
+                return BackendMarketplaceCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_operation_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_token_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,79 @@
 """
-BackendOperationTag automatically generated by SDKgen please do not edit this file manually
+ConsumerTokenTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_operation import BackendOperation
-from .backend_operation_collection import BackendOperationCollection
-from .backend_operation_create import BackendOperationCreate
-from .backend_operation_update import BackendOperationUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
+from .consumer_token import ConsumerToken
+from .consumer_token_access_token import ConsumerTokenAccessToken
+from .consumer_token_collection import ConsumerTokenCollection
+from .consumer_token_create import ConsumerTokenCreate
+from .consumer_token_update import ConsumerTokenUpdate
 
-class BackendOperationTag(sdkgen.TagAbstract):
+class ConsumerTokenTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, operation_id: str) -> CommonMessage:
+    def delete(self, token_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["operation_id"] = operation_id
+            path_params["token_id"] = token_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/operation/$operation_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/token/$token_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, operation_id: str, payload: BackendOperationUpdate) -> CommonMessage:
+    def update(self, token_id: str, payload: ConsumerTokenUpdate) -> ConsumerTokenAccessToken:
         try:
             path_params = {}
-            path_params["operation_id"] = operation_id
+            path_params["token_id"] = token_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/operation/$operation_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/token/$token_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return ConsumerTokenAccessToken.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,105 +82,97 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, operation_id: str) -> BackendOperation:
+    def get(self, token_id: str) -> ConsumerToken:
         try:
             path_params = {}
-            path_params["operation_id"] = operation_id
+            path_params["token_id"] = token_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/operation/$operation_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/token/$token_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendOperation.from_json(response.content)
+                return ConsumerToken.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def create(self, payload: BackendOperationCreate) -> CommonMessage:
+    def create(self, payload: ConsumerTokenCreate) -> ConsumerTokenAccessToken:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/operation", path_params)
+            url = self.parser.url("/consumer/token", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return ConsumerTokenAccessToken.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendOperationCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> ConsumerTokenCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/operation", path_params)
+            url = self.parser.url("/consumer/token", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendOperationCollection.from_json(response.content)
+                return ConsumerTokenCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_page_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_webhook_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 """
-BackendPageTag automatically generated by SDKgen please do not edit this file manually
+BackendWebhookTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_page import BackendPage
-from .backend_page_collection import BackendPageCollection
-from .backend_page_create import BackendPageCreate
-from .backend_page_update import BackendPageUpdate
+from .backend_webhook import BackendWebhook
+from .backend_webhook_collection import BackendWebhookCollection
+from .backend_webhook_create import BackendWebhookCreate
+from .backend_webhook_update import BackendWebhookUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
-class BackendPageTag(sdkgen.TagAbstract):
+class BackendWebhookTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, page_id: str) -> CommonMessage:
+    def delete(self, webhook_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["page_id"] = page_id
+            path_params["webhook_id"] = webhook_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/page/$page_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/webhook/$webhook_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, page_id: str, payload: BackendPageUpdate) -> CommonMessage:
+    def update(self, webhook_id: str, payload: BackendWebhookUpdate) -> CommonMessage:
         try:
             path_params = {}
-            path_params["page_id"] = page_id
+            path_params["webhook_id"] = webhook_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/page/$page_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/webhook/$webhook_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,105 +81,95 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, page_id: str) -> BackendPage:
+    def get(self, webhook_id: str) -> BackendWebhook:
         try:
             path_params = {}
-            path_params["page_id"] = page_id
+            path_params["webhook_id"] = webhook_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/page/$page_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/webhook/$webhook_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendPage.from_json(response.content)
+                return BackendWebhook.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
-            if response.status_code == 410:
-                raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def create(self, payload: BackendPageCreate) -> CommonMessage:
+    def create(self, payload: BackendWebhookCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/page", path_params)
+            url = self.parser.url("/backend/webhook", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendPageCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> BackendWebhookCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/page", path_params)
+            url = self.parser.url("/backend/webhook", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendPageCollection.from_json(response.content)
+                return BackendWebhookCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_plan_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_event_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 """
-BackendPlanTag automatically generated by SDKgen please do not edit this file manually
+BackendEventTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_plan import BackendPlan
-from .backend_plan_collection import BackendPlanCollection
-from .backend_plan_create import BackendPlanCreate
-from .backend_plan_update import BackendPlanUpdate
+from .backend_event import BackendEvent
+from .backend_event_collection import BackendEventCollection
+from .backend_event_create import BackendEventCreate
+from .backend_event_update import BackendEventUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
-class BackendPlanTag(sdkgen.TagAbstract):
+class BackendEventTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, plan_id: str) -> CommonMessage:
+    def delete(self, event_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["plan_id"] = plan_id
+            path_params["event_id"] = event_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/plan/$plan_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/event/$event_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, plan_id: str, payload: BackendPlanUpdate) -> CommonMessage:
+    def update(self, event_id: str, payload: BackendEventUpdate) -> CommonMessage:
         try:
             path_params = {}
-            path_params["plan_id"] = plan_id
+            path_params["event_id"] = event_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/plan/$plan_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/event/$event_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,105 +81,97 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, plan_id: str) -> BackendPlan:
+    def get(self, event_id: str) -> BackendEvent:
         try:
             path_params = {}
-            path_params["plan_id"] = plan_id
+            path_params["event_id"] = event_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/plan/$plan_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/event/$event_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendPlan.from_json(response.content)
+                return BackendEvent.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def create(self, payload: BackendPlanCreate) -> CommonMessage:
+    def create(self, payload: BackendEventCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/plan", path_params)
+            url = self.parser.url("/backend/event", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendPlanCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> BackendEventCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/plan", path_params)
+            url = self.parser.url("/backend/event", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendPlanCollection.from_json(response.content)
+                return BackendEventCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_rate_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_app_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 """
-BackendRateTag automatically generated by SDKgen please do not edit this file manually
+ConsumerAppTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_rate import BackendRate
-from .backend_rate_collection import BackendRateCollection
-from .backend_rate_create import BackendRateCreate
-from .backend_rate_update import BackendRateUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
+from .consumer_app import ConsumerApp
+from .consumer_app_collection import ConsumerAppCollection
+from .consumer_app_create import ConsumerAppCreate
+from .consumer_app_update import ConsumerAppUpdate
 
-class BackendRateTag(sdkgen.TagAbstract):
+class ConsumerAppTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, rate_id: str) -> CommonMessage:
+    def delete(self, app_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["rate_id"] = rate_id
+            path_params["app_id"] = app_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/rate/$rate_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/app/$app_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, rate_id: str, payload: BackendRateUpdate) -> CommonMessage:
+    def update(self, app_id: str, payload: ConsumerAppUpdate) -> CommonMessage:
         try:
             path_params = {}
-            path_params["rate_id"] = rate_id
+            path_params["app_id"] = app_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/rate/$rate_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/app/$app_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,105 +81,97 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, rate_id: str) -> BackendRate:
+    def get(self, app_id: str) -> ConsumerApp:
         try:
             path_params = {}
-            path_params["rate_id"] = rate_id
+            path_params["app_id"] = app_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/rate/$rate_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/consumer/app/$app_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendRate.from_json(response.content)
+                return ConsumerApp.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def create(self, payload: BackendRateCreate) -> CommonMessage:
+    def create(self, payload: ConsumerAppCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/rate", path_params)
+            url = self.parser.url("/consumer/app", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendRateCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> ConsumerAppCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/rate", path_params)
+            url = self.parser.url("/consumer/app", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendRateCollection.from_json(response.content)
+                return ConsumerAppCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_role_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_user_tag.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 """
-BackendRoleTag automatically generated by SDKgen please do not edit this file manually
+BackendUserTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_role import BackendRole
-from .backend_role_collection import BackendRoleCollection
-from .backend_role_create import BackendRoleCreate
-from .backend_role_update import BackendRoleUpdate
+from .backend_user import BackendUser
+from .backend_user_collection import BackendUserCollection
+from .backend_user_create import BackendUserCreate
+from .backend_user_update import BackendUserUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
-class BackendRoleTag(sdkgen.TagAbstract):
+class BackendUserTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, role_id: str) -> CommonMessage:
+    def delete(self, user_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["role_id"] = role_id
+            path_params["user_id"] = user_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/role/$role_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/user/$user_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, role_id: str, payload: BackendRoleUpdate) -> CommonMessage:
+    def update(self, user_id: str, payload: BackendUserUpdate) -> CommonMessage:
         try:
             path_params = {}
-            path_params["role_id"] = role_id
+            path_params["user_id"] = user_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/role/$role_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/user/$user_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,105 +81,97 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, role_id: str) -> BackendRole:
+    def get(self, user_id: str) -> BackendUser:
         try:
             path_params = {}
-            path_params["role_id"] = role_id
+            path_params["user_id"] = user_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/role/$role_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/user/$user_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendRole.from_json(response.content)
+                return BackendUser.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def create(self, payload: BackendRoleCreate) -> CommonMessage:
+    def create(self, payload: BackendUserCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/role", path_params)
+            url = self.parser.url("/backend/user", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendRoleCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> BackendUserCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/role", path_params)
+            url = self.parser.url("/backend/user", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendRoleCollection.from_json(response.content)
+                return BackendUserCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_schema_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_schema_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,29 @@
 BackendSchemaTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_schema import BackendSchema
 from .backend_schema_collection import BackendSchemaCollection
 from .backend_schema_create import BackendSchemaCreate
 from .backend_schema_form import BackendSchemaForm
 from .backend_schema_preview_response import BackendSchemaPreviewResponse
 from .backend_schema_update import BackendSchemaUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendSchemaTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def delete(self, schema_id: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["schema_id"] = schema_id
 
             query_params = {}
@@ -35,49 +34,47 @@
             url = self.parser.url("/backend/schema/$schema_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, schema_id: str, payload: BackendSchemaUpdate) -> CommonMessage:
         try:
             path_params = {}
             path_params["schema_id"] = schema_id
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/schema/$schema_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -86,16 +83,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self, schema_id: str) -> BackendSchema:
         try:
             path_params = {}
             path_params["schema_id"] = schema_id
 
             query_params = {}
 
@@ -104,49 +99,47 @@
             url = self.parser.url("/backend/schema/$schema_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendSchema.from_json(response.content)
+                return BackendSchema.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update_form(self, schema_id: str, payload: BackendSchemaForm) -> CommonMessage:
         try:
             path_params = {}
             path_params["schema_id"] = schema_id
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/schema/form/$schema_id<[0-9]+>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -155,16 +148,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_preview(self, schema_id: str) -> BackendSchemaPreviewResponse:
         try:
             path_params = {}
             path_params["schema_id"] = schema_id
 
             query_params = {}
 
@@ -173,58 +164,54 @@
             url = self.parser.url("/backend/schema/preview/:schema_id", path_params)
 
             headers = {}
 
             response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendSchemaPreviewResponse.from_json(response.content)
+                return BackendSchemaPreviewResponse.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def create(self, payload: BackendSchemaCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/schema", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self, start_index: int, count: int, search: str) -> BackendSchemaCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -235,21 +222,19 @@
             url = self.parser.url("/backend/schema", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendSchemaCollection.from_json(response.content)
+                return BackendSchemaCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_scope_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_rate_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,78 @@
 """
-BackendScopeTag automatically generated by SDKgen please do not edit this file manually
+BackendRateTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_scope import BackendScope
-from .backend_scope_categories import BackendScopeCategories
-from .backend_scope_collection import BackendScopeCollection
-from .backend_scope_create import BackendScopeCreate
-from .backend_scope_update import BackendScopeUpdate
+from .backend_rate import BackendRate
+from .backend_rate_collection import BackendRateCollection
+from .backend_rate_create import BackendRateCreate
+from .backend_rate_update import BackendRateUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
-class BackendScopeTag(sdkgen.TagAbstract):
+class BackendRateTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, scope_id: str) -> CommonMessage:
+    def delete(self, rate_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["scope_id"] = scope_id
+            path_params["rate_id"] = rate_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/scope/$scope_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/rate/$rate_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
-            if response.status_code == 400:
-                raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, scope_id: str, payload: BackendScopeUpdate) -> CommonMessage:
+    def update(self, rate_id: str, payload: BackendRateUpdate) -> CommonMessage:
         try:
             path_params = {}
-            path_params["scope_id"] = scope_id
+            path_params["rate_id"] = rate_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/scope/$scope_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/rate/$rate_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -87,133 +81,97 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, scope_id: str) -> BackendScope:
+    def get(self, rate_id: str) -> BackendRate:
         try:
             path_params = {}
-            path_params["scope_id"] = scope_id
+            path_params["rate_id"] = rate_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/scope/$scope_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/rate/$rate_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendScope.from_json(response.content)
+                return BackendRate.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_categories(self) -> BackendScopeCategories:
-        try:
-            path_params = {}
-
-            query_params = {}
-
-            query_struct_names = []
-
-            url = self.parser.url("/backend/scope/categories", path_params)
-
-            headers = {}
-
-            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
-
-            if response.status_code >= 200 and response.status_code < 300:
-                return BackendScopeCategories.from_json(response.content)
-
-            if response.status_code == 401:
-                raise CommonMessageException(response.content)
-            if response.status_code == 500:
-                raise CommonMessageException(response.content)
-
-            raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
-        except RequestException as e:
-            raise sdkgen.ClientException("An unknown error occurred: " + str(e))
-
-    pass
-
-    def create(self, payload: BackendScopeCreate) -> CommonMessage:
+    def create(self, payload: BackendRateCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/scope", path_params)
+            url = self.parser.url("/backend/rate", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendScopeCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> BackendRateCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/scope", path_params)
+            url = self.parser.url("/backend/rate", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendScopeCollection.from_json(response.content)
+                return BackendRateCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_sdk_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_sdk_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,56 +2,53 @@
 BackendSdkTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_sdk_generate import BackendSdkGenerate
 from .backend_sdk_response import BackendSdkResponse
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendSdkTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def generate(self, payload: BackendSdkGenerate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/backend/sdk", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self) -> BackendSdkResponse:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -59,21 +56,19 @@
             url = self.parser.url("/backend/sdk", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendSdkResponse.from_json(response.content)
+                return BackendSdkResponse.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_statistic_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_statistic_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,34 @@
 BackendStatisticTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_statistic_chart import BackendStatisticChart
 from .backend_statistic_count import BackendStatisticCount
 from .common_message_exception import CommonMessageException
 
 class BackendStatisticTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def get_used_points(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_used_points(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -43,36 +42,34 @@
             url = self.parser.url("/backend/statistic/used_points", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_time_per_operation(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_time_per_operation(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -85,36 +82,34 @@
             url = self.parser.url("/backend/statistic/time_per_operation", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_time_average(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_time_average(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -127,36 +122,34 @@
             url = self.parser.url("/backend/statistic/time_average", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_most_used_operations(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_most_used_operations(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -169,36 +162,34 @@
             url = self.parser.url("/backend/statistic/most_used_operations", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_most_used_apps(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_most_used_apps(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -211,36 +202,34 @@
             url = self.parser.url("/backend/statistic/most_used_apps", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_issued_tokens(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_issued_tokens(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -253,36 +242,34 @@
             url = self.parser.url("/backend/statistic/issued_tokens", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_incoming_transactions(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_incoming_transactions(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -295,36 +282,34 @@
             url = self.parser.url("/backend/statistic/incoming_transactions", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_incoming_requests(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_incoming_requests(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -337,36 +322,34 @@
             url = self.parser.url("/backend/statistic/incoming_requests", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_errors_per_operation(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
+    def get_errors_per_operation(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticChart:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -379,36 +362,34 @@
             url = self.parser.url("/backend/statistic/errors_per_operation", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticChart.from_json(response.content)
+                return BackendStatisticChart.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_count_requests(self, start_index: int, count: int, search: str, _from: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticCount:
+    def get_count_requests(self, start_index: int, count: int, search: str, from_: str, to: str, operation_id: int, app_id: int, user_id: int, ip: str, user_agent: str, method: str, path: str, header: str, body: str) -> BackendStatisticCount:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["operationId"] = operation_id
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["ip"] = ip
             query_params["userAgent"] = user_agent
             query_params["method"] = method
@@ -421,21 +402,19 @@
             url = self.parser.url("/backend/statistic/count_requests", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendStatisticCount.from_json(response.content)
+                return BackendStatisticCount.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_tenant_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_grant_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,80 @@
 """
-BackendTenantTag automatically generated by SDKgen please do not edit this file manually
+ConsumerGrantTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
+from .consumer_grant_collection import ConsumerGrantCollection
 
-class BackendTenantTag(sdkgen.TagAbstract):
+class ConsumerGrantTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def remove(self, tenant_id: str) -> CommonMessage:
+    def delete(self, grant_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["tenant_id"] = tenant_id
+            path_params["grant_id"] = grant_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/tenant/:tenant_id", path_params)
+            url = self.parser.url("/consumer/grant/$grant_id<[0-9]+>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def setup(self, tenant_id: str) -> CommonMessage:
+    def get_all(self, start_index: int, count: int, search: str) -> ConsumerGrantCollection:
         try:
             path_params = {}
-            path_params["tenant_id"] = tenant_id
 
             query_params = {}
+            query_params["startIndex"] = start_index
+            query_params["count"] = count
+            query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/tenant/:tenant_id", path_params)
+            url = self.parser.url("/consumer/grant", path_params)
 
             headers = {}
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return ConsumerGrantCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
-            if response.status_code == 404:
-                raise CommonMessageException(response.content)
-            if response.status_code == 410:
-                raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_token_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_token_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 BackendTokenTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_token import BackendToken
 from .backend_token_collection import BackendTokenCollection
 from .common_message_exception import CommonMessageException
 
 class BackendTokenTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get(self, token_id: str) -> BackendToken:
         try:
             path_params = {}
             path_params["token_id"] = token_id
 
             query_params = {}
@@ -30,38 +29,36 @@
             url = self.parser.url("/backend/token/$token_id<[0-9]+>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendToken.from_json(response.content)
+                return BackendToken.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str, _from: str, to: str, app_id: int, user_id: int, status: int, scope: str, ip: str) -> BackendTokenCollection:
+    def get_all(self, start_index: int, count: int, search: str, from_: str, to: str, app_id: int, user_id: int, status: int, scope: str, ip: str) -> BackendTokenCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
+            query_params["from"] = from_
             query_params["to"] = to
             query_params["appId"] = app_id
             query_params["userId"] = user_id
             query_params["status"] = status
             query_params["scope"] = scope
             query_params["ip"] = ip
 
@@ -70,21 +67,19 @@
             url = self.parser.url("/backend/token", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendTokenCollection.from_json(response.content)
+                return BackendTokenCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_transaction_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_transaction_tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,80 @@
 """
-BackendTransactionTag automatically generated by SDKgen please do not edit this file manually
+ConsumerTransactionTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_transaction import BackendTransaction
-from .backend_transaction_collection import BackendTransactionCollection
 from .common_message_exception import CommonMessageException
+from .consumer_transaction import ConsumerTransaction
+from .consumer_transaction_collection import ConsumerTransactionCollection
 
-class BackendTransactionTag(sdkgen.TagAbstract):
+class ConsumerTransactionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def get(self, transaction_id: str) -> BackendTransaction:
+    def get(self, transaction_id: str) -> ConsumerTransaction:
         try:
             path_params = {}
             path_params["transaction_id"] = transaction_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/transaction/$transaction_id<[0-9]+>", path_params)
+            url = self.parser.url("/consumer/transaction/$transaction_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendTransaction.from_json(response.content)
+                return ConsumerTransaction.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str, _from: str, to: str, plan_id: int, user_id: int, app_id: int, status: str, provider: str) -> BackendTransactionCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> ConsumerTransactionCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
-            query_params["from"] = _from
-            query_params["to"] = to
-            query_params["planId"] = plan_id
-            query_params["userId"] = user_id
-            query_params["appId"] = app_id
-            query_params["status"] = status
-            query_params["provider"] = provider
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/transaction", path_params)
+            url = self.parser.url("/consumer/transaction", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendTransactionCollection.from_json(response.content)
+                return ConsumerTransactionCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_trash_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_trash_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 BackendTrashTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_trash_data_collection import BackendTrashDataCollection
 from .backend_trash_restore import BackendTrashRestore
 from .backend_trash_types import BackendTrashTypes
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class BackendTrashTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def restore(self, type: str, payload: BackendTrashRestore) -> CommonMessage:
         try:
             path_params = {}
             path_params["type"] = type
 
             query_params = {}
@@ -30,32 +29,30 @@
             query_struct_names = []
 
             url = self.parser.url("/backend/trash/:type", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all_by_type(self, type: str, start_index: int, count: int, search: str) -> BackendTrashDataCollection:
         try:
             path_params = {}
             path_params["type"] = type
 
             query_params = {}
             query_params["startIndex"] = start_index
@@ -67,27 +64,25 @@
             url = self.parser.url("/backend/trash/:type", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendTrashDataCollection.from_json(response.content)
+                return BackendTrashDataCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_types(self) -> BackendTrashTypes:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -95,21 +90,19 @@
             url = self.parser.url("/backend/trash", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendTrashTypes.from_json(response.content)
+                return BackendTrashTypes.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/backend_user_tag.py` & `fusio_sdk-5.0.7/src/sdk/system_meta_tag.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,188 +1,164 @@
 """
-BackendUserTag automatically generated by SDKgen please do not edit this file manually
+SystemMetaTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
-from .backend_user import BackendUser
-from .backend_user_collection import BackendUserCollection
-from .backend_user_create import BackendUserCreate
-from .backend_user_update import BackendUserUpdate
-from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
+from .passthru import Passthru
+from .system_about import SystemAbout
+from .system_health_check import SystemHealthCheck
+from .system_o_auth_configuration import SystemOAuthConfiguration
+from .system_route import SystemRoute
+from .system_schema import SystemSchema
 
-class BackendUserTag(sdkgen.TagAbstract):
+class SystemMetaTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, user_id: str) -> CommonMessage:
+    def get_schema(self, name: str) -> SystemSchema:
         try:
             path_params = {}
-            path_params["user_id"] = user_id
+            path_params["name"] = name
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/user/$user_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/system/schema/:name", path_params)
 
             headers = {}
 
-            response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return SystemSchema.model_validate_json(json_data=response.content)
 
-            if response.status_code == 401:
-                raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, user_id: str, payload: BackendUserUpdate) -> CommonMessage:
+    def get_routes(self) -> SystemRoute:
         try:
             path_params = {}
-            path_params["user_id"] = user_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/user/$user_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/system/route", path_params)
 
             headers = {}
-            headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return SystemRoute.model_validate_json(json_data=response.content)
 
-            if response.status_code == 400:
-                raise CommonMessageException(response.content)
-            if response.status_code == 401:
-                raise CommonMessageException(response.content)
-            if response.status_code == 404:
-                raise CommonMessageException(response.content)
-            if response.status_code == 410:
-                raise CommonMessageException(response.content)
-            if response.status_code == 500:
-                raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, user_id: str) -> BackendUser:
+    def get_o_auth_configuration(self) -> SystemOAuthConfiguration:
         try:
             path_params = {}
-            path_params["user_id"] = user_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/user/$user_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/system/oauth-authorization-server", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendUser.from_json(response.content)
+                return SystemOAuthConfiguration.model_validate_json(json_data=response.content)
 
-            if response.status_code == 401:
-                raise CommonMessageException(response.content)
-            if response.status_code == 404:
-                raise CommonMessageException(response.content)
-            if response.status_code == 410:
-                raise CommonMessageException(response.content)
-            if response.status_code == 500:
-                raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
+    def get_health(self) -> SystemHealthCheck:
+        try:
+            path_params = {}
 
-    def create(self, payload: BackendUserCreate) -> CommonMessage:
+            query_params = {}
+
+            query_struct_names = []
+
+            url = self.parser.url("/system/health", path_params)
+
+            headers = {}
+
+            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+
+            if response.status_code >= 200 and response.status_code < 300:
+                return SystemHealthCheck.model_validate_json(json_data=response.content)
+
+
+            raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
+        except RequestException as e:
+            raise sdkgen.ClientException("An unknown error occurred: " + str(e))
+
+    def get_debug(self, payload: Passthru) -> Passthru:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/user", path_params)
+            url = self.parser.url("/system/debug", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return Passthru.model_validate_json(json_data=response.content)
 
-            if response.status_code == 400:
-                raise CommonMessageException(response.content)
-            if response.status_code == 401:
-                raise CommonMessageException(response.content)
-            if response.status_code == 500:
-                raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> BackendUserCollection:
+    def get_about(self) -> SystemAbout:
         try:
             path_params = {}
 
             query_params = {}
-            query_params["startIndex"] = start_index
-            query_params["count"] = count
-            query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/backend/user", path_params)
+            url = self.parser.url("/system/about", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return BackendUserCollection.from_json(response.content)
+                return SystemAbout.model_validate_json(json_data=response.content)
 
-            if response.status_code == 401:
-                raise CommonMessageException(response.content)
-            if response.status_code == 500:
-                raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/client.py` & `fusio_sdk-5.0.7/src/sdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,58 +2,48 @@
 Client automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .authorization_tag import AuthorizationTag
 from .system_tag import SystemTag
 from .consumer_tag import ConsumerTag
 from .backend_tag import BackendTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
-    pass
-
     def authorization(self) -> AuthorizationTag:
         return AuthorizationTag(
             self.http_client,
             self.parser
         )
 
-    pass
-
     def system(self) -> SystemTag:
         return SystemTag(
             self.http_client,
             self.parser
         )
 
-    pass
-
     def consumer(self) -> ConsumerTag:
         return ConsumerTag(
             self.http_client,
             self.parser
         )
 
-    pass
-
     def backend(self) -> BackendTag:
         return BackendTag(
             self.http_client,
             self.parser
         )
 
-    pass
-
 
 
     @staticmethod
     def build(clientId: str, clientSecret: str, tokenStore: sdkgen.TokenStoreInterface, scopes: List[str]):
         return Client("https://api.typehub.cloud/", sdkgen.OAuth2(clientId, clientSecret, "https://api.typehub.cloud/authorization/token", "", tokenStore, scopes))
 
-    pass
```

### Comparing `fusio-sdk-5.0.6/src/sdk/common_form_element_select.py` & `fusio_sdk-5.0.7/src/sdk/common_form_element_select.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 common_form_element_select automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
-from dataclasses import dataclass, field
-from dataclasses_json import dataclass_json, config
-from typing import List
+from pydantic import BaseModel, Field, GetCoreSchemaHandler
+from pydantic_core import CoreSchema, core_schema
+from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 from .common_form_element import CommonFormElement
 from .common_form_element_select_option import CommonFormElementSelectOption
-@dataclass_json
-@dataclass
 class CommonFormElementSelect(CommonFormElement):
-    options: List[CommonFormElementSelectOption] = field(default=None, metadata=config(field_name="options"))
+    options: Optional[List[CommonFormElementSelectOption]] = Field(default=None, alias="options")
+    pass
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_account_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_account_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ConsumerAccountTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .backend_account_change_password import BackendAccountChangePassword
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 from .consumer_authorize_meta import ConsumerAuthorizeMeta
 from .consumer_authorize_request import ConsumerAuthorizeRequest
 from .consumer_authorize_response import ConsumerAuthorizeResponse
@@ -22,199 +23,185 @@
 from .consumer_user_refresh import ConsumerUserRefresh
 from .consumer_user_register import ConsumerUserRegister
 
 class ConsumerAccountTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def execute_password_reset(self, payload: ConsumerUserPasswordReset) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/password_reset", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def request_password_reset(self, payload: ConsumerUserEmail) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/password_reset", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def register(self, payload: ConsumerUserRegister) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/register", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def refresh(self, payload: ConsumerUserRefresh) -> ConsumerUserJWT:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/login", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerUserJWT.from_json(response.content)
+                return ConsumerUserJWT.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def login(self, payload: ConsumerUserLogin) -> ConsumerUserJWT:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/login", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerUserJWT.from_json(response.content)
+                return ConsumerUserJWT.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def authorize(self, payload: ConsumerAuthorizeRequest) -> ConsumerAuthorizeResponse:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/authorize", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerAuthorizeResponse.from_json(response.content)
+                return ConsumerAuthorizeResponse.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_app(self) -> ConsumerAuthorizeMeta:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -222,106 +209,100 @@
             url = self.parser.url("/consumer/authorize", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerAuthorizeMeta.from_json(response.content)
+                return ConsumerAuthorizeMeta.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def activate(self, payload: ConsumerUserActivate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/activate", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def change_password(self, payload: BackendAccountChangePassword) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/account/change_password", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def update(self, payload: ConsumerUserAccount) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/account", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -330,16 +311,14 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get(self) -> ConsumerUserAccount:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
@@ -347,25 +326,23 @@
             url = self.parser.url("/consumer/account", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerUserAccount.from_json(response.content)
+                return ConsumerUserAccount.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_app_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_plan_tag.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 """
-ConsumerAppTag automatically generated by SDKgen please do not edit this file manually
+BackendPlanTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
+from .backend_plan import BackendPlan
+from .backend_plan_collection import BackendPlanCollection
+from .backend_plan_create import BackendPlanCreate
+from .backend_plan_update import BackendPlanUpdate
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
-from .consumer_app import ConsumerApp
-from .consumer_app_collection import ConsumerAppCollection
-from .consumer_app_create import ConsumerAppCreate
-from .consumer_app_update import ConsumerAppUpdate
 
-class ConsumerAppTag(sdkgen.TagAbstract):
+class BackendPlanTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, app_id: str) -> CommonMessage:
+    def delete(self, plan_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["app_id"] = app_id
+            path_params["plan_id"] = plan_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/app/$app_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/plan/$plan_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def update(self, app_id: str, payload: ConsumerAppUpdate) -> CommonMessage:
+    def update(self, plan_id: str, payload: BackendPlanUpdate) -> CommonMessage:
         try:
             path_params = {}
-            path_params["app_id"] = app_id
+            path_params["plan_id"] = plan_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/app/$app_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/plan/$plan_id<[0-9]+|^~>", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
@@ -84,105 +81,97 @@
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get(self, app_id: str) -> ConsumerApp:
+    def get(self, plan_id: str) -> BackendPlan:
         try:
             path_params = {}
-            path_params["app_id"] = app_id
+            path_params["plan_id"] = plan_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/app/$app_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/plan/$plan_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerApp.from_json(response.content)
+                return BackendPlan.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def create(self, payload: ConsumerAppCreate) -> CommonMessage:
+    def create(self, payload: BackendPlanCreate) -> CommonMessage:
         try:
             path_params = {}
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/app", path_params)
+            url = self.parser.url("/backend/plan", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> ConsumerAppCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> BackendPlanCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/app", path_params)
+            url = self.parser.url("/backend/plan", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerAppCollection.from_json(response.content)
+                return BackendPlanCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_event_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_event_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 ConsumerEventTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message_exception import CommonMessageException
 from .consumer_event_collection import ConsumerEventCollection
 
 class ConsumerEventTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get_all(self, start_index: int, count: int, search: str) -> ConsumerEventCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
@@ -31,21 +30,19 @@
             url = self.parser.url("/consumer/event", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerEventCollection.from_json(response.content)
+                return ConsumerEventCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_grant_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_tenant_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,81 @@
 """
-ConsumerGrantTag automatically generated by SDKgen please do not edit this file manually
+BackendTenantTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
-from .consumer_grant_collection import ConsumerGrantCollection
 
-class ConsumerGrantTag(sdkgen.TagAbstract):
+class BackendTenantTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def delete(self, grant_id: str) -> CommonMessage:
+    def remove(self, tenant_id: str) -> CommonMessage:
         try:
             path_params = {}
-            path_params["grant_id"] = grant_id
+            path_params["tenant_id"] = tenant_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/grant/$grant_id<[0-9]+>", path_params)
+            url = self.parser.url("/backend/tenant/:tenant_id", path_params)
 
             headers = {}
 
             response = self.http_client.delete(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> ConsumerGrantCollection:
+    def setup(self, tenant_id: str) -> CommonMessage:
         try:
             path_params = {}
+            path_params["tenant_id"] = tenant_id
 
             query_params = {}
-            query_params["startIndex"] = start_index
-            query_params["count"] = count
-            query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/grant", path_params)
+            url = self.parser.url("/backend/tenant/:tenant_id", path_params)
 
             headers = {}
 
-            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+            response = self.http_client.put(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerGrantCollection.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
+            if response.status_code == 404:
+                raise CommonMessageException(response.content)
+            if response.status_code == 410:
+                raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_identity_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_identity_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 ConsumerIdentityTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message_exception import CommonMessageException
 from .consumer_identity_collection import ConsumerIdentityCollection
 from .passthru import Passthru
 
 class ConsumerIdentityTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def redirect(self, identity: str) -> Passthru:
         try:
             path_params = {}
             path_params["identity"] = identity
 
             query_params = {}
@@ -30,27 +29,25 @@
             url = self.parser.url("/consumer/identity/:identity/redirect", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return Passthru.from_json(response.content)
+                return Passthru.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def exchange(self, identity: str) -> Passthru:
         try:
             path_params = {}
             path_params["identity"] = identity
 
             query_params = {}
 
@@ -59,50 +56,47 @@
             url = self.parser.url("/consumer/identity/:identity/exchange", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return Passthru.from_json(response.content)
+                return Passthru.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, app_id: int) -> ConsumerIdentityCollection:
+    def get_all(self, app_id: int, app_key: str) -> ConsumerIdentityCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["appId"] = app_id
+            query_params["appKey"] = app_key
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/identity", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerIdentityCollection.from_json(response.content)
+                return ConsumerIdentityCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 400:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_log_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_log_tag.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 ConsumerLogTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message_exception import CommonMessageException
 from .consumer_log import ConsumerLog
 from .consumer_log_collection import ConsumerLogCollection
 
 class ConsumerLogTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get(self, log_id: str) -> ConsumerLog:
         try:
             path_params = {}
             path_params["log_id"] = log_id
 
             query_params = {}
@@ -30,31 +29,29 @@
             url = self.parser.url("/consumer/log/$log_id<[0-9]+>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerLog.from_json(response.content)
+                return ConsumerLog.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def get_all(self, start_index: int, count: int, search: str) -> ConsumerLogCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
@@ -65,21 +62,19 @@
             url = self.parser.url("/consumer/log", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerLogCollection.from_json(response.content)
+                return ConsumerLogCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_page_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_plan_tag.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,80 @@
 """
-ConsumerPageTag automatically generated by SDKgen please do not edit this file manually
+ConsumerPlanTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message_exception import CommonMessageException
-from .consumer_page import ConsumerPage
-from .consumer_page_collection import ConsumerPageCollection
+from .consumer_plan import ConsumerPlan
+from .consumer_plan_collection import ConsumerPlanCollection
 
-class ConsumerPageTag(sdkgen.TagAbstract):
+class ConsumerPlanTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def get(self, page_id: str) -> ConsumerPage:
+    def get(self, plan_id: str) -> ConsumerPlan:
         try:
             path_params = {}
-            path_params["page_id"] = page_id
+            path_params["plan_id"] = plan_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/page/:page_id", path_params)
+            url = self.parser.url("/consumer/plan/$plan_id<[0-9]+|^~>", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerPage.from_json(response.content)
+                return ConsumerPlan.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 404:
                 raise CommonMessageException(response.content)
             if response.status_code == 410:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> ConsumerPageCollection:
+    def get_all(self, start_index: int, count: int, search: str) -> ConsumerPlanCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
             query_params["count"] = count
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/page", path_params)
+            url = self.parser.url("/consumer/plan", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerPageCollection.from_json(response.content)
+                return ConsumerPlanCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_payment_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_payment_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 ConsumerPaymentTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message_exception import CommonMessageException
 from .consumer_payment_checkout_request import ConsumerPaymentCheckoutRequest
 from .consumer_payment_checkout_response import ConsumerPaymentCheckoutResponse
 from .consumer_payment_portal_request import ConsumerPaymentPortalRequest
 from .consumer_payment_portal_response import ConsumerPaymentPortalResponse
 
 class ConsumerPaymentTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def checkout(self, provider: str, payload: ConsumerPaymentCheckoutRequest) -> ConsumerPaymentCheckoutResponse:
         try:
             path_params = {}
             path_params["provider"] = provider
 
             query_params = {}
@@ -30,54 +29,50 @@
             query_struct_names = []
 
             url = self.parser.url("/consumer/payment/:provider/checkout", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerPaymentCheckoutResponse.from_json(response.content)
+                return ConsumerPaymentCheckoutResponse.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
     def portal(self, provider: str, payload: ConsumerPaymentPortalRequest) -> ConsumerPaymentPortalResponse:
         try:
             path_params = {}
             path_params["provider"] = provider
 
             query_params = {}
 
             query_struct_names = []
 
             url = self.parser.url("/consumer/payment/:provider/portal", path_params)
 
             headers = {}
             headers["Content-Type"] = "application/json"
 
-            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), data=payload.to_json())
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerPaymentPortalResponse.from_json(response.content)
+                return ConsumerPaymentPortalResponse.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_plan_tag.py` & `fusio_sdk-5.0.7/src/sdk/backend_backup_tag.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,74 @@
 """
-ConsumerPlanTag automatically generated by SDKgen please do not edit this file manually
+BackendBackupTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
+from .backend_backup_export import BackendBackupExport
+from .backend_backup_import import BackendBackupImport
+from .backend_backup_import_result import BackendBackupImportResult
 from .common_message_exception import CommonMessageException
-from .consumer_plan import ConsumerPlan
-from .consumer_plan_collection import ConsumerPlanCollection
 
-class ConsumerPlanTag(sdkgen.TagAbstract):
+class BackendBackupTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
 
-
-    def get(self, plan_id: str) -> ConsumerPlan:
+    def import_(self, payload: BackendBackupImport) -> BackendBackupImportResult:
         try:
             path_params = {}
-            path_params["plan_id"] = plan_id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/plan/$plan_id<[0-9]+|^~>", path_params)
+            url = self.parser.url("/backend/backup/import", path_params)
 
             headers = {}
+            headers["Content-Type"] = "application/json"
 
-            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names), json=payload.model_dump(by_alias=True))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerPlan.from_json(response.content)
+                return BackendBackupImportResult.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
-            if response.status_code == 404:
-                raise CommonMessageException(response.content)
-            if response.status_code == 410:
-                raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
-    def get_all(self, start_index: int, count: int, search: str) -> ConsumerPlanCollection:
+    def export(self) -> BackendBackupExport:
         try:
             path_params = {}
 
             query_params = {}
-            query_params["startIndex"] = start_index
-            query_params["count"] = count
-            query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/consumer/plan", path_params)
+            url = self.parser.url("/backend/backup/export", path_params)
 
             headers = {}
 
-            response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
+            response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerPlanCollection.from_json(response.content)
+                return BackendBackupExport.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_scope_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_scope_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 ConsumerScopeTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message_exception import CommonMessageException
 from .consumer_scope_collection import ConsumerScopeCollection
 
 class ConsumerScopeTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def get_all(self, start_index: int, count: int, search: str) -> ConsumerScopeCollection:
         try:
             path_params = {}
 
             query_params = {}
             query_params["startIndex"] = start_index
@@ -31,21 +30,19 @@
             url = self.parser.url("/consumer/scope", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return ConsumerScopeCollection.from_json(response.content)
+                return ConsumerScopeCollection.model_validate_json(json_data=response.content)
 
             if response.status_code == 401:
                 raise CommonMessageException(response.content)
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/consumer_tag.py` & `fusio_sdk-5.0.7/src/sdk/consumer_tag.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ConsumerTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .consumer_account_tag import ConsumerAccountTag
 from .consumer_app_tag import ConsumerAppTag
 from .consumer_event_tag import ConsumerEventTag
 from .consumer_grant_tag import ConsumerGrantTag
 from .consumer_identity_tag import ConsumerIdentityTag
 from .consumer_log_tag import ConsumerLogTag
@@ -21,114 +22,86 @@
 from .consumer_transaction_tag import ConsumerTransactionTag
 from .consumer_webhook_tag import ConsumerWebhookTag
 
 class ConsumerTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
     def identity(self) -> ConsumerIdentityTag:
         return ConsumerIdentityTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def account(self) -> ConsumerAccountTag:
         return ConsumerAccountTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def transaction(self) -> ConsumerTransactionTag:
         return ConsumerTransactionTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def webhook(self) -> ConsumerWebhookTag:
         return ConsumerWebhookTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def token(self) -> ConsumerTokenTag:
         return ConsumerTokenTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def scope(self) -> ConsumerScopeTag:
         return ConsumerScopeTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def plan(self) -> ConsumerPlanTag:
         return ConsumerPlanTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def payment(self) -> ConsumerPaymentTag:
         return ConsumerPaymentTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def page(self) -> ConsumerPageTag:
         return ConsumerPageTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def log(self) -> ConsumerLogTag:
         return ConsumerLogTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def grant(self) -> ConsumerGrantTag:
         return ConsumerGrantTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def event(self) -> ConsumerEventTag:
         return ConsumerEventTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
     def app(self) -> ConsumerAppTag:
         return ConsumerAppTag(
-            this.http_client,
-            this.parser
+            self.http_client,
+            self.parser
         )
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/system_connection_tag.py` & `fusio_sdk-5.0.7/src/sdk/system_connection_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 SystemConnectionTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message import CommonMessage
 
 class SystemConnectionTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def callback(self, name: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["name"] = name
 
             query_params = {}
@@ -28,17 +27,15 @@
             url = self.parser.url("/system/connection/:name/callback", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

### Comparing `fusio-sdk-5.0.6/src/sdk/system_payment_tag.py` & `fusio_sdk-5.0.7/src/sdk/system_payment_tag.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 SystemPaymentTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
+from typing import List
 
 from .common_message import CommonMessage
 from .common_message_exception import CommonMessageException
 
 class SystemPaymentTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
-    pass
-
 
     def webhook(self, provider: str) -> CommonMessage:
         try:
             path_params = {}
             path_params["provider"] = provider
 
             query_params = {}
@@ -29,19 +28,17 @@
             url = self.parser.url("/system/payment/:provider/webhook", path_params)
 
             headers = {}
 
             response = self.http_client.post(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return CommonMessage.from_json(response.content)
+                return CommonMessage.model_validate_json(json_data=response.content)
 
             if response.status_code == 500:
                 raise CommonMessageException(response.content)
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    pass
-
```

