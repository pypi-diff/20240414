# Comparing `tmp/lakefs-client-1.9.0.tar.gz` & `tmp/lakefs-client-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakefs-client-1.9.0.tar", last modified: Sun Jan 21 12:16:37 2024, max compression
+gzip compressed data, was "lakefs-client-1.9.1.tar", last modified: Mon Jan 22 08:45:38 2024, max compression
```

## Comparing `lakefs-client-1.9.0.tar` & `lakefs-client-1.9.1.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:37.474366 lakefs-client-1.9.0/
--rw-r--r--   0     1001      127    34552 2024-01-21 12:16:37.474366 lakefs-client-1.9.0/PKG-INFO
--rw-r--r--   0     1001      127    27203 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/README.md
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:37.434366 lakefs-client-1.9.0/lakefs_client/
--rw-r--r--   0     1001      127      705 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/__init__.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:37.438366 lakefs-client-1.9.0/lakefs_client/api/
--rw-r--r--   0     1001      127      217 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/__init__.py
--rw-r--r--   0     1001      127    20697 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/api/actions_api.py
--rw-r--r--   0     1001      127   137567 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/api/auth_api.py
--rw-r--r--   0     1001      127    40074 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/api/branches_api.py
--rw-r--r--   0     1001      127    10525 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/api/commits_api.py
--rw-r--r--   0     1001      127     4640 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/api/config_api.py
--rw-r--r--   0     1001      127    32337 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/experimental_api.py
--rw-r--r--   0     1001      127     4339 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/health_check_api.py
--rw-r--r--   0     1001      127    15359 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/import_api.py
--rw-r--r--   0     1001      127   119235 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/internal_api.py
--rw-r--r--   0     1001      127     9809 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/metadata_api.py
--rw-r--r--   0     1001      127    49915 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/objects_api.py
--rw-r--r--   0     1001      127    24986 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/refs_api.py
--rw-r--r--   0     1001      127    63153 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/repositories_api.py
--rw-r--r--   0     1001      127    11547 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/staging_api.py
--rw-r--r--   0     1001      127    19344 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api/tags_api.py
--rw-r--r--   0     1001      127    36807 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/api_client.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:37.438366 lakefs-client-1.9.0/lakefs_client/apis/
--rw-r--r--   0     1001      127     1221 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/apis/__init__.py
--rw-r--r--   0     1001      127     6684 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/client.py
--rw-r--r--   0     1001      127    18527 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/configuration.py
--rw-r--r--   0     1001      127     5035 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/exceptions.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:37.454366 lakefs-client-1.9.0/lakefs_client/model/
--rw-r--r--   0     1001      127      348 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/model/__init__.py
--rw-r--r--   0     1001      127    11219 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/abort_presign_multipart_upload.py
--rw-r--r--   0     1001      127    11898 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/access_key_credentials.py
--rw-r--r--   0     1001      127    11283 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/acl.py
--rw-r--r--   0     1001      127    12568 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/action_run.py
--rw-r--r--   0     1001      127    11638 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/action_run_list.py
--rw-r--r--   0     1001      127    11286 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/auth_capabilities.py
--rw-r--r--   0     1001      127    11470 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/authentication_token.py
--rw-r--r--   0     1001      127    11562 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/branch_creation.py
--rw-r--r--   0     1001      127    11295 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/branch_protection_rule.py
--rw-r--r--   0     1001      127    12020 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/cherry_pick_creation.py
--rw-r--r--   0     1001      127    11892 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/comm_prefs_input.py
--rw-r--r--   0     1001      127    13135 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/commit.py
--rw-r--r--   0     1001      127    12361 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/commit_creation.py
--rw-r--r--   0     1001      127    11607 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/commit_list.py
--rw-r--r--   0     1001      127    14023 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/commit_record_creation.py
--rw-r--r--   0     1001      127    12263 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/complete_presign_multipart_upload.py
--rw-r--r--   0     1001      127    11608 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/config.py
--rw-r--r--   0     1001      127    11471 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/credentials.py
--rw-r--r--   0     1001      127    11657 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/credentials_list.py
--rw-r--r--   0     1001      127    11834 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/credentials_with_secret.py
--rw-r--r--   0     1001      127    11181 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/current_user.py
--rw-r--r--   0     1001      127    12102 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/diff.py
--rw-r--r--   0     1001      127    11587 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/diff_list.py
--rw-r--r--   0     1001      127    11048 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/diff_properties.py
--rw-r--r--   0     1001      127    11124 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/error.py
--rw-r--r--   0     1001      127    11412 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/error_no_acl.py
--rw-r--r--   0     1001      127    12082 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/find_merge_base_result.py
--rw-r--r--   0     1001      127    11249 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/garbage_collection_config.py
--rw-r--r--   0     1001      127    12604 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/garbage_collection_prepare_response.py
--rw-r--r--   0     1001      127    11424 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/garbage_collection_rule.py
--rw-r--r--   0     1001      127    11773 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/garbage_collection_rules.py
--rw-r--r--   0     1001      127    11510 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/group.py
--rw-r--r--   0     1001      127    11023 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/group_creation.py
--rw-r--r--   0     1001      127    11597 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/group_list.py
--rw-r--r--   0     1001      127    12339 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/hook_run.py
--rw-r--r--   0     1001      127    11618 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/hook_run_list.py
--rw-r--r--   0     1001      127    11941 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/import_creation.py
--rw-r--r--   0     1001      127    11108 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/import_creation_response.py
--rw-r--r--   0     1001      127    12471 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/import_location.py
--rw-r--r--   0     1001      127    12522 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/import_status.py
--rw-r--r--   0     1001      127    11161 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/inline_object.py
--rw-r--r--   0     1001      127    11078 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/inline_object1.py
--rw-r--r--   0     1001      127    11617 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/installation_usage_report.py
--rw-r--r--   0     1001      127    13582 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/login_config.py
--rw-r--r--   0     1001      127    11486 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/login_information.py
--rw-r--r--   0     1001      127    12240 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/merge.py
--rw-r--r--   0     1001      127    11094 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/merge_result.py
--rw-r--r--   0     1001      127    11353 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/meta_range_creation.py
--rw-r--r--   0     1001      127    11095 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/meta_range_creation_response.py
--rw-r--r--   0     1001      127    11801 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/object_copy_creation.py
--rw-r--r--   0     1001      127    11721 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/object_error.py
--rw-r--r--   0     1001      127    11271 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/object_error_list.py
--rw-r--r--   0     1001      127    12912 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/object_stage_creation.py
--rw-r--r--   0     1001      127    14337 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/object_stats.py
--rw-r--r--   0     1001      127    11658 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/object_stats_list.py
--rw-r--r--   0     1001      127    10783 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/object_user_metadata.py
--rw-r--r--   0     1001      127    12651 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/otf_diff_entry.py
--rw-r--r--   0     1001      127    11620 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/otf_diff_list.py
--rw-r--r--   0     1001      127    11212 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/otf_diffs.py
--rw-r--r--   0     1001      127    12264 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/pagination.py
--rw-r--r--   0     1001      127    11047 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/path_list.py
--rw-r--r--   0     1001      127    11764 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/policy.py
--rw-r--r--   0     1001      127    11607 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/policy_list.py
--rw-r--r--   0     1001      127    11115 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/prepare_gc_uncommitted_request.py
--rw-r--r--   0     1001      127    11841 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/prepare_gc_uncommitted_response.py
--rw-r--r--   0     1001      127    11683 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/presign_multipart_upload.py
--rw-r--r--   0     1001      127    12236 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/range_metadata.py
--rw-r--r--   0     1001      127    11238 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/ref.py
--rw-r--r--   0     1001      127    11577 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/ref_list.py
--rw-r--r--   0     1001      127    11949 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/refs_dump.py
--rw-r--r--   0     1001      127    12260 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/refs_restore.py
--rw-r--r--   0     1001      127    12526 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/repository.py
--rw-r--r--   0     1001      127    12756 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/repository_creation.py
--rw-r--r--   0     1001      127    12081 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/repository_dump_status.py
--rw-r--r--   0     1001      127    11647 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/repository_list.py
--rw-r--r--   0     1001      127    10783 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/repository_metadata.py
--rw-r--r--   0     1001      127    11078 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/repository_metadata_keys.py
--rw-r--r--   0     1001      127    11143 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/repository_metadata_set.py
--rw-r--r--   0     1001      127    11741 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/repository_restore_status.py
--rw-r--r--   0     1001      127    11731 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/reset_creation.py
--rw-r--r--   0     1001      127    11918 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/revert_creation.py
--rw-r--r--   0     1001      127    11580 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/setup.py
--rw-r--r--   0     1001      127    11859 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/setup_state.py
--rw-r--r--   0     1001      127    12261 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/staging_location.py
--rw-r--r--   0     1001      127    12745 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/staging_metadata.py
--rw-r--r--   0     1001      127    11661 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/statement.py
--rw-r--r--   0     1001      127    11918 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/stats_event.py
--rw-r--r--   0     1001      127    11264 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/stats_events_list.py
--rw-r--r--   0     1001      127    14077 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/storage_config.py
--rw-r--r--   0     1001      127    11080 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/storage_uri.py
--rw-r--r--   0     1001      127    11574 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/tag_creation.py
--rw-r--r--   0     1001      127    11038 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/task_info.py
--rw-r--r--   0     1001      127    11120 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/underlying_object_properties.py
--rw-r--r--   0     1001      127    11138 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/update_token.py
--rw-r--r--   0     1001      127    11303 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/upload_part.py
--rw-r--r--   0     1001      127    11441 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/usage_report.py
--rw-r--r--   0     1001      127    12747 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/user.py
--rw-r--r--   0     1001      127    11304 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/user_creation.py
--rw-r--r--   0     1001      127    11587 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/user_list.py
--rw-r--r--   0     1001      127    11715 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/lakefs_client/model/version_config.py
--rw-r--r--   0     1001      127    81856 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/model_utils.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:37.454366 lakefs-client-1.9.0/lakefs_client/models/
--rw-r--r--   0     1001      127     6693 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/models/__init__.py
--rw-r--r--   0     1001      127    12638 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/lakefs_client/rest.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:37.474366 lakefs-client-1.9.0/lakefs_client.egg-info/
--rw-r--r--   0     1001      127    34552 2024-01-21 12:16:37.000000 lakefs-client-1.9.0/lakefs_client.egg-info/PKG-INFO
--rw-r--r--   0     1001      127     8256 2024-01-21 12:16:37.000000 lakefs-client-1.9.0/lakefs_client.egg-info/SOURCES.txt
--rw-r--r--   0     1001      127        1 2024-01-21 12:16:37.000000 lakefs-client-1.9.0/lakefs_client.egg-info/dependency_links.txt
--rw-r--r--   0     1001      127       32 2024-01-21 12:16:37.000000 lakefs-client-1.9.0/lakefs_client.egg-info/requires.txt
--rw-r--r--   0     1001      127       14 2024-01-21 12:16:37.000000 lakefs-client-1.9.0/lakefs_client.egg-info/top_level.txt
--rw-r--r--   0     1001      127       69 2024-01-21 12:16:37.474366 lakefs-client-1.9.0/setup.cfg
--rw-r--r--   0     1001      127     1398 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/setup.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:37.474366 lakefs-client-1.9.0/test/
--rw-r--r--   0     1001      127      818 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_abort_presign_multipart_upload.py
--rw-r--r--   0     1001      127      768 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_access_key_credentials.py
--rw-r--r--   0     1001      127      647 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_acl.py
--rw-r--r--   0     1001      127      690 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_action_run.py
--rw-r--r--   0     1001      127      898 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_action_run_list.py
--rw-r--r--   0     1001      127     1091 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_actions_api.py
--rw-r--r--   0     1001      127     4947 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_auth_api.py
--rw-r--r--   0     1001      127      739 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_auth_capabilities.py
--rw-r--r--   0     1001      127      760 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_authentication_token.py
--rw-r--r--   0     1001      127      725 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_branch_creation.py
--rw-r--r--   0     1001      127      768 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_branch_protection_rule.py
--rw-r--r--   0     1001      127     1637 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_branches_api.py
--rw-r--r--   0     1001      127      754 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_cherry_pick_creation.py
--rw-r--r--   0     1001      127      726 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_comm_prefs_input.py
--rw-r--r--   0     1001      127      668 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_commit.py
--rw-r--r--   0     1001      127      725 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_commit_creation.py
--rw-r--r--   0     1001      127      863 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_commit_list.py
--rw-r--r--   0     1001      127      768 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_commit_record_creation.py
--rw-r--r--   0     1001      127      781 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_commits_api.py
--rw-r--r--   0     1001      127      931 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_complete_presign_multipart_upload.py
--rw-r--r--   0     1001      127      876 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_config.py
--rw-r--r--   0     1001      127      621 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_config_api.py
--rw-r--r--   0     1001      127      703 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_credentials.py
--rw-r--r--   0     1001      127      918 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_credentials_list.py
--rw-r--r--   0     1001      127      775 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_credentials_with_secret.py
--rw-r--r--   0     1001      127      771 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_current_user.py
--rw-r--r--   0     1001      127      654 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_diff.py
--rw-r--r--   0     1001      127      841 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_diff_list.py
--rw-r--r--   0     1001      127      725 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_diff_properties.py
--rw-r--r--   0     1001      127      661 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_error.py
--rw-r--r--   0     1001      127      698 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_error_no_acl.py
--rw-r--r--   0     1001      127     1579 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_experimental_api.py
--rw-r--r--   0     1001      127      762 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_find_merge_base_result.py
--rw-r--r--   0     1001      127      789 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_garbage_collection_config.py
--rw-r--r--   0     1001      127      853 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_garbage_collection_prepare_response.py
--rw-r--r--   0     1001      127      775 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_garbage_collection_rule.py
--rw-r--r--   0     1001      127      919 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_garbage_collection_rules.py
--rw-r--r--   0     1001      127      661 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_group.py
--rw-r--r--   0     1001      127      718 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_group_creation.py
--rw-r--r--   0     1001      127      852 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_group_list.py
--rw-r--r--   0     1001      127      651 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_health_check_api.py
--rw-r--r--   0     1001      127      676 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_hook_run.py
--rw-r--r--   0     1001      127      876 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_hook_run_list.py
--rw-r--r--   0     1001      127      961 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_import_api.py
--rw-r--r--   0     1001      127      941 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_import_creation.py
--rw-r--r--   0     1001      127      782 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_import_creation_response.py
--rw-r--r--   0     1001      127      725 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_import_location.py
--rw-r--r--   0     1001      127      857 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_import_status.py
--rw-r--r--   0     1001      127      711 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_inline_object.py
--rw-r--r--   0     1001      127      718 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_inline_object1.py
--rw-r--r--   0     1001      127      885 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_installation_usage_report.py
--rw-r--r--   0     1001      127     5081 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_internal_api.py
--rw-r--r--   0     1001      127      704 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_login_config.py
--rw-r--r--   0     1001      127      739 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_login_information.py
--rw-r--r--   0     1001      127      661 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_merge.py
--rw-r--r--   0     1001      127      704 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_merge_result.py
--rw-r--r--   0     1001      127      851 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_meta_range_creation.py
--rw-r--r--   0     1001      127      804 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_meta_range_creation_response.py
--rw-r--r--   0     1001      127      834 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_metadata_api.py
--rw-r--r--   0     1001      127      754 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_object_copy_creation.py
--rw-r--r--   0     1001      127      704 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_object_error.py
--rw-r--r--   0     1001      127      829 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_object_error_list.py
--rw-r--r--   0     1001      127      886 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_object_stage_creation.py
--rw-r--r--   0     1001      127      829 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_object_stats.py
--rw-r--r--   0     1001      127      920 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_object_stats_list.py
--rw-r--r--   0     1001      127      754 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_object_user_metadata.py
--rw-r--r--   0     1001      127     1912 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_objects_api.py
--rw-r--r--   0     1001      127      712 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_otf_diff_entry.py
--rw-r--r--   0     1001      127      806 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_otf_diff_list.py
--rw-r--r--   0     1001      127      791 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_otf_diffs.py
--rw-r--r--   0     1001      127      696 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_pagination.py
--rw-r--r--   0     1001      127      683 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_path_list.py
--rw-r--r--   0     1001      127      755 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_policy.py
--rw-r--r--   0     1001      127      863 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_policy_list.py
--rw-r--r--   0     1001      127      818 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_prepare_gc_uncommitted_request.py
--rw-r--r--   0     1001      127      825 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_prepare_gc_uncommitted_response.py
--rw-r--r--   0     1001      127      782 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_presign_multipart_upload.py
--rw-r--r--   0     1001      127      718 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_range_metadata.py
--rw-r--r--   0     1001      127      647 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_ref.py
--rw-r--r--   0     1001      127      830 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_ref_list.py
--rw-r--r--   0     1001      127     1160 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_refs_api.py
--rw-r--r--   0     1001      127      683 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_refs_dump.py
--rw-r--r--   0     1001      127      704 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_refs_restore.py
--rw-r--r--   0     1001      127     2652 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_repositories_api.py
--rw-r--r--   0     1001      127      696 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_repository.py
--rw-r--r--   0     1001      127      753 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_repository_creation.py
--rw-r--r--   0     1001      127      852 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_repository_dump_status.py
--rw-r--r--   0     1001      127      907 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_repository_list.py
--rw-r--r--   0     1001      127      753 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_repository_metadata.py
--rw-r--r--   0     1001      127      782 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_repository_metadata_keys.py
--rw-r--r--   0     1001      127      775 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_repository_metadata_set.py
--rw-r--r--   0     1001      127      789 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_repository_restore_status.py
--rw-r--r--   0     1001      127      718 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_reset_creation.py
--rw-r--r--   0     1001      127      725 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_revert_creation.py
--rw-r--r--   0     1001      127      794 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_setup.py
--rw-r--r--   0     1001      127      793 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_setup_state.py
--rw-r--r--   0     1001      127      922 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_staging_api.py
--rw-r--r--   0     1001      127      732 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_staging_location.py
--rw-r--r--   0     1001      127      844 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_staging_metadata.py
--rw-r--r--   0     1001      127      689 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_statement.py
--rw-r--r--   0     1001      127      697 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_stats_event.py
--rw-r--r--   0     1001      127      825 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_stats_events_list.py
--rw-r--r--   0     1001      127      718 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_storage_config.py
--rw-r--r--   0     1001      127      697 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_storage_uri.py
--rw-r--r--   0     1001      127      704 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_tag_creation.py
--rw-r--r--   0     1001      127     1013 2024-01-21 12:15:57.000000 lakefs-client-1.9.0/test/test_tags_api.py
--rw-r--r--   0     1001      127      683 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_task_info.py
--rw-r--r--   0     1001      127      810 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_underlying_object_properties.py
--rw-r--r--   0     1001      127      704 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_update_token.py
--rw-r--r--   0     1001      127      697 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_upload_part.py
--rw-r--r--   0     1001      127      704 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_usage_report.py
--rw-r--r--   0     1001      127      654 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_user.py
--rw-r--r--   0     1001      127      711 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_user_creation.py
--rw-r--r--   0     1001      127      841 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_user_list.py
--rw-r--r--   0     1001      127      718 2024-01-21 12:15:56.000000 lakefs-client-1.9.0/test/test_version_config.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:38.176135 lakefs-client-1.9.1/
+-rw-r--r--   0     1001      127    34552 2024-01-22 08:45:38.176135 lakefs-client-1.9.1/PKG-INFO
+-rw-r--r--   0     1001      127    27203 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/README.md
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:38.132135 lakefs-client-1.9.1/lakefs_client/
+-rw-r--r--   0     1001      127      705 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/__init__.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:38.136135 lakefs-client-1.9.1/lakefs_client/api/
+-rw-r--r--   0     1001      127      217 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/__init__.py
+-rw-r--r--   0     1001      127    20697 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/api/actions_api.py
+-rw-r--r--   0     1001      127   137567 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/api/auth_api.py
+-rw-r--r--   0     1001      127    40074 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/api/branches_api.py
+-rw-r--r--   0     1001      127    10525 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/commits_api.py
+-rw-r--r--   0     1001      127     4640 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/config_api.py
+-rw-r--r--   0     1001      127    32337 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/experimental_api.py
+-rw-r--r--   0     1001      127     4339 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/health_check_api.py
+-rw-r--r--   0     1001      127    15359 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/import_api.py
+-rw-r--r--   0     1001      127   119235 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/internal_api.py
+-rw-r--r--   0     1001      127     9809 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/metadata_api.py
+-rw-r--r--   0     1001      127    49915 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/objects_api.py
+-rw-r--r--   0     1001      127    24986 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/refs_api.py
+-rw-r--r--   0     1001      127    63153 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/repositories_api.py
+-rw-r--r--   0     1001      127    11547 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/staging_api.py
+-rw-r--r--   0     1001      127    19344 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api/tags_api.py
+-rw-r--r--   0     1001      127    36807 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/api_client.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:38.136135 lakefs-client-1.9.1/lakefs_client/apis/
+-rw-r--r--   0     1001      127     1221 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/apis/__init__.py
+-rw-r--r--   0     1001      127     6684 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/client.py
+-rw-r--r--   0     1001      127    18527 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/configuration.py
+-rw-r--r--   0     1001      127     5035 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/exceptions.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:38.156135 lakefs-client-1.9.1/lakefs_client/model/
+-rw-r--r--   0     1001      127      348 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/model/__init__.py
+-rw-r--r--   0     1001      127    11219 2024-01-22 08:44:56.000000 lakefs-client-1.9.1/lakefs_client/model/abort_presign_multipart_upload.py
+-rw-r--r--   0     1001      127    11898 2024-01-22 08:44:56.000000 lakefs-client-1.9.1/lakefs_client/model/access_key_credentials.py
+-rw-r--r--   0     1001      127    11283 2024-01-22 08:44:56.000000 lakefs-client-1.9.1/lakefs_client/model/acl.py
+-rw-r--r--   0     1001      127    12568 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/action_run.py
+-rw-r--r--   0     1001      127    11638 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/action_run_list.py
+-rw-r--r--   0     1001      127    11286 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/auth_capabilities.py
+-rw-r--r--   0     1001      127    11470 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/authentication_token.py
+-rw-r--r--   0     1001      127    11562 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/branch_creation.py
+-rw-r--r--   0     1001      127    11295 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/branch_protection_rule.py
+-rw-r--r--   0     1001      127    12020 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/cherry_pick_creation.py
+-rw-r--r--   0     1001      127    11892 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/comm_prefs_input.py
+-rw-r--r--   0     1001      127    13057 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/commit.py
+-rw-r--r--   0     1001      127    12361 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/commit_creation.py
+-rw-r--r--   0     1001      127    11607 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/commit_list.py
+-rw-r--r--   0     1001      127    14023 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/commit_record_creation.py
+-rw-r--r--   0     1001      127    12263 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/complete_presign_multipart_upload.py
+-rw-r--r--   0     1001      127    11608 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/config.py
+-rw-r--r--   0     1001      127    11471 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/credentials.py
+-rw-r--r--   0     1001      127    11657 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/credentials_list.py
+-rw-r--r--   0     1001      127    11834 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/credentials_with_secret.py
+-rw-r--r--   0     1001      127    11181 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/current_user.py
+-rw-r--r--   0     1001      127    12102 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/diff.py
+-rw-r--r--   0     1001      127    11587 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/diff_list.py
+-rw-r--r--   0     1001      127    11048 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/diff_properties.py
+-rw-r--r--   0     1001      127    11124 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/error.py
+-rw-r--r--   0     1001      127    11412 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/error_no_acl.py
+-rw-r--r--   0     1001      127    12082 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/find_merge_base_result.py
+-rw-r--r--   0     1001      127    11249 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/garbage_collection_config.py
+-rw-r--r--   0     1001      127    12604 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/garbage_collection_prepare_response.py
+-rw-r--r--   0     1001      127    11424 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/garbage_collection_rule.py
+-rw-r--r--   0     1001      127    11773 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/garbage_collection_rules.py
+-rw-r--r--   0     1001      127    11510 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/group.py
+-rw-r--r--   0     1001      127    11023 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/group_creation.py
+-rw-r--r--   0     1001      127    11597 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/group_list.py
+-rw-r--r--   0     1001      127    12339 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/hook_run.py
+-rw-r--r--   0     1001      127    11618 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/hook_run_list.py
+-rw-r--r--   0     1001      127    11941 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/import_creation.py
+-rw-r--r--   0     1001      127    11108 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/import_creation_response.py
+-rw-r--r--   0     1001      127    12471 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/import_location.py
+-rw-r--r--   0     1001      127    12522 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/import_status.py
+-rw-r--r--   0     1001      127    11161 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/inline_object.py
+-rw-r--r--   0     1001      127    11078 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/inline_object1.py
+-rw-r--r--   0     1001      127    11617 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/installation_usage_report.py
+-rw-r--r--   0     1001      127    13582 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/login_config.py
+-rw-r--r--   0     1001      127    11486 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/login_information.py
+-rw-r--r--   0     1001      127    12240 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/merge.py
+-rw-r--r--   0     1001      127    11094 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/merge_result.py
+-rw-r--r--   0     1001      127    11353 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/meta_range_creation.py
+-rw-r--r--   0     1001      127    11095 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/meta_range_creation_response.py
+-rw-r--r--   0     1001      127    11801 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/object_copy_creation.py
+-rw-r--r--   0     1001      127    11721 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/object_error.py
+-rw-r--r--   0     1001      127    11271 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/object_error_list.py
+-rw-r--r--   0     1001      127    12912 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/object_stage_creation.py
+-rw-r--r--   0     1001      127    14337 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/object_stats.py
+-rw-r--r--   0     1001      127    11658 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/object_stats_list.py
+-rw-r--r--   0     1001      127    10783 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/object_user_metadata.py
+-rw-r--r--   0     1001      127    12651 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/otf_diff_entry.py
+-rw-r--r--   0     1001      127    11620 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/otf_diff_list.py
+-rw-r--r--   0     1001      127    11212 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/otf_diffs.py
+-rw-r--r--   0     1001      127    12264 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/pagination.py
+-rw-r--r--   0     1001      127    11047 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/path_list.py
+-rw-r--r--   0     1001      127    11764 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/policy.py
+-rw-r--r--   0     1001      127    11607 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/policy_list.py
+-rw-r--r--   0     1001      127    11115 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/prepare_gc_uncommitted_request.py
+-rw-r--r--   0     1001      127    11841 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/prepare_gc_uncommitted_response.py
+-rw-r--r--   0     1001      127    11683 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/presign_multipart_upload.py
+-rw-r--r--   0     1001      127    12236 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/range_metadata.py
+-rw-r--r--   0     1001      127    11238 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/ref.py
+-rw-r--r--   0     1001      127    11577 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/ref_list.py
+-rw-r--r--   0     1001      127    11949 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/refs_dump.py
+-rw-r--r--   0     1001      127    12260 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/refs_restore.py
+-rw-r--r--   0     1001      127    12526 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/repository.py
+-rw-r--r--   0     1001      127    12756 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/repository_creation.py
+-rw-r--r--   0     1001      127    12081 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/repository_dump_status.py
+-rw-r--r--   0     1001      127    11647 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/repository_list.py
+-rw-r--r--   0     1001      127    10783 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/repository_metadata.py
+-rw-r--r--   0     1001      127    11078 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/repository_metadata_keys.py
+-rw-r--r--   0     1001      127    11143 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/repository_metadata_set.py
+-rw-r--r--   0     1001      127    11741 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/repository_restore_status.py
+-rw-r--r--   0     1001      127    11731 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/reset_creation.py
+-rw-r--r--   0     1001      127    11918 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/revert_creation.py
+-rw-r--r--   0     1001      127    11580 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/setup.py
+-rw-r--r--   0     1001      127    11859 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/setup_state.py
+-rw-r--r--   0     1001      127    12261 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/staging_location.py
+-rw-r--r--   0     1001      127    12745 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/staging_metadata.py
+-rw-r--r--   0     1001      127    11661 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/statement.py
+-rw-r--r--   0     1001      127    11918 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/stats_event.py
+-rw-r--r--   0     1001      127    11264 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/stats_events_list.py
+-rw-r--r--   0     1001      127    14077 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/storage_config.py
+-rw-r--r--   0     1001      127    11080 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/storage_uri.py
+-rw-r--r--   0     1001      127    11574 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/tag_creation.py
+-rw-r--r--   0     1001      127    11038 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/task_info.py
+-rw-r--r--   0     1001      127    11120 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/underlying_object_properties.py
+-rw-r--r--   0     1001      127    11138 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/update_token.py
+-rw-r--r--   0     1001      127    11303 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/upload_part.py
+-rw-r--r--   0     1001      127    11441 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/usage_report.py
+-rw-r--r--   0     1001      127    12747 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/user.py
+-rw-r--r--   0     1001      127    11304 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/user_creation.py
+-rw-r--r--   0     1001      127    11587 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/user_list.py
+-rw-r--r--   0     1001      127    11715 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/lakefs_client/model/version_config.py
+-rw-r--r--   0     1001      127    81856 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/model_utils.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:38.156135 lakefs-client-1.9.1/lakefs_client/models/
+-rw-r--r--   0     1001      127     6693 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/models/__init__.py
+-rw-r--r--   0     1001      127    12638 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/lakefs_client/rest.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:38.176135 lakefs-client-1.9.1/lakefs_client.egg-info/
+-rw-r--r--   0     1001      127    34552 2024-01-22 08:45:38.000000 lakefs-client-1.9.1/lakefs_client.egg-info/PKG-INFO
+-rw-r--r--   0     1001      127     8256 2024-01-22 08:45:38.000000 lakefs-client-1.9.1/lakefs_client.egg-info/SOURCES.txt
+-rw-r--r--   0     1001      127        1 2024-01-22 08:45:38.000000 lakefs-client-1.9.1/lakefs_client.egg-info/dependency_links.txt
+-rw-r--r--   0     1001      127       32 2024-01-22 08:45:38.000000 lakefs-client-1.9.1/lakefs_client.egg-info/requires.txt
+-rw-r--r--   0     1001      127       14 2024-01-22 08:45:38.000000 lakefs-client-1.9.1/lakefs_client.egg-info/top_level.txt
+-rw-r--r--   0     1001      127       69 2024-01-22 08:45:38.176135 lakefs-client-1.9.1/setup.cfg
+-rw-r--r--   0     1001      127     1398 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/setup.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:38.176135 lakefs-client-1.9.1/test/
+-rw-r--r--   0     1001      127      818 2024-01-22 08:44:56.000000 lakefs-client-1.9.1/test/test_abort_presign_multipart_upload.py
+-rw-r--r--   0     1001      127      768 2024-01-22 08:44:56.000000 lakefs-client-1.9.1/test/test_access_key_credentials.py
+-rw-r--r--   0     1001      127      647 2024-01-22 08:44:56.000000 lakefs-client-1.9.1/test/test_acl.py
+-rw-r--r--   0     1001      127      690 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_action_run.py
+-rw-r--r--   0     1001      127      898 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_action_run_list.py
+-rw-r--r--   0     1001      127     1091 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_actions_api.py
+-rw-r--r--   0     1001      127     4947 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_auth_api.py
+-rw-r--r--   0     1001      127      739 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_auth_capabilities.py
+-rw-r--r--   0     1001      127      760 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_authentication_token.py
+-rw-r--r--   0     1001      127      725 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_branch_creation.py
+-rw-r--r--   0     1001      127      768 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_branch_protection_rule.py
+-rw-r--r--   0     1001      127     1637 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_branches_api.py
+-rw-r--r--   0     1001      127      754 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_cherry_pick_creation.py
+-rw-r--r--   0     1001      127      726 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_comm_prefs_input.py
+-rw-r--r--   0     1001      127      668 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_commit.py
+-rw-r--r--   0     1001      127      725 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_commit_creation.py
+-rw-r--r--   0     1001      127      863 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_commit_list.py
+-rw-r--r--   0     1001      127      768 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_commit_record_creation.py
+-rw-r--r--   0     1001      127      781 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_commits_api.py
+-rw-r--r--   0     1001      127      931 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_complete_presign_multipart_upload.py
+-rw-r--r--   0     1001      127      876 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_config.py
+-rw-r--r--   0     1001      127      621 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_config_api.py
+-rw-r--r--   0     1001      127      703 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_credentials.py
+-rw-r--r--   0     1001      127      918 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_credentials_list.py
+-rw-r--r--   0     1001      127      775 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_credentials_with_secret.py
+-rw-r--r--   0     1001      127      771 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_current_user.py
+-rw-r--r--   0     1001      127      654 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_diff.py
+-rw-r--r--   0     1001      127      841 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_diff_list.py
+-rw-r--r--   0     1001      127      725 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_diff_properties.py
+-rw-r--r--   0     1001      127      661 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_error.py
+-rw-r--r--   0     1001      127      698 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_error_no_acl.py
+-rw-r--r--   0     1001      127     1579 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_experimental_api.py
+-rw-r--r--   0     1001      127      762 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_find_merge_base_result.py
+-rw-r--r--   0     1001      127      789 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_garbage_collection_config.py
+-rw-r--r--   0     1001      127      853 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_garbage_collection_prepare_response.py
+-rw-r--r--   0     1001      127      775 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_garbage_collection_rule.py
+-rw-r--r--   0     1001      127      919 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_garbage_collection_rules.py
+-rw-r--r--   0     1001      127      661 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_group.py
+-rw-r--r--   0     1001      127      718 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_group_creation.py
+-rw-r--r--   0     1001      127      852 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_group_list.py
+-rw-r--r--   0     1001      127      651 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_health_check_api.py
+-rw-r--r--   0     1001      127      676 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_hook_run.py
+-rw-r--r--   0     1001      127      876 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_hook_run_list.py
+-rw-r--r--   0     1001      127      961 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_import_api.py
+-rw-r--r--   0     1001      127      941 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_import_creation.py
+-rw-r--r--   0     1001      127      782 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_import_creation_response.py
+-rw-r--r--   0     1001      127      725 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_import_location.py
+-rw-r--r--   0     1001      127      857 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_import_status.py
+-rw-r--r--   0     1001      127      711 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_inline_object.py
+-rw-r--r--   0     1001      127      718 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_inline_object1.py
+-rw-r--r--   0     1001      127      885 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_installation_usage_report.py
+-rw-r--r--   0     1001      127     5081 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_internal_api.py
+-rw-r--r--   0     1001      127      704 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_login_config.py
+-rw-r--r--   0     1001      127      739 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_login_information.py
+-rw-r--r--   0     1001      127      661 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_merge.py
+-rw-r--r--   0     1001      127      704 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_merge_result.py
+-rw-r--r--   0     1001      127      851 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_meta_range_creation.py
+-rw-r--r--   0     1001      127      804 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_meta_range_creation_response.py
+-rw-r--r--   0     1001      127      834 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_metadata_api.py
+-rw-r--r--   0     1001      127      754 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_object_copy_creation.py
+-rw-r--r--   0     1001      127      704 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_object_error.py
+-rw-r--r--   0     1001      127      829 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_object_error_list.py
+-rw-r--r--   0     1001      127      886 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_object_stage_creation.py
+-rw-r--r--   0     1001      127      829 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_object_stats.py
+-rw-r--r--   0     1001      127      920 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_object_stats_list.py
+-rw-r--r--   0     1001      127      754 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_object_user_metadata.py
+-rw-r--r--   0     1001      127     1912 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_objects_api.py
+-rw-r--r--   0     1001      127      712 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_otf_diff_entry.py
+-rw-r--r--   0     1001      127      806 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_otf_diff_list.py
+-rw-r--r--   0     1001      127      791 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_otf_diffs.py
+-rw-r--r--   0     1001      127      696 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_pagination.py
+-rw-r--r--   0     1001      127      683 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_path_list.py
+-rw-r--r--   0     1001      127      755 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_policy.py
+-rw-r--r--   0     1001      127      863 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_policy_list.py
+-rw-r--r--   0     1001      127      818 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_prepare_gc_uncommitted_request.py
+-rw-r--r--   0     1001      127      825 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_prepare_gc_uncommitted_response.py
+-rw-r--r--   0     1001      127      782 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_presign_multipart_upload.py
+-rw-r--r--   0     1001      127      718 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_range_metadata.py
+-rw-r--r--   0     1001      127      647 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_ref.py
+-rw-r--r--   0     1001      127      830 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_ref_list.py
+-rw-r--r--   0     1001      127     1160 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_refs_api.py
+-rw-r--r--   0     1001      127      683 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_refs_dump.py
+-rw-r--r--   0     1001      127      704 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_refs_restore.py
+-rw-r--r--   0     1001      127     2652 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_repositories_api.py
+-rw-r--r--   0     1001      127      696 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_repository.py
+-rw-r--r--   0     1001      127      753 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_repository_creation.py
+-rw-r--r--   0     1001      127      852 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_repository_dump_status.py
+-rw-r--r--   0     1001      127      907 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_repository_list.py
+-rw-r--r--   0     1001      127      753 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_repository_metadata.py
+-rw-r--r--   0     1001      127      782 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_repository_metadata_keys.py
+-rw-r--r--   0     1001      127      775 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_repository_metadata_set.py
+-rw-r--r--   0     1001      127      789 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_repository_restore_status.py
+-rw-r--r--   0     1001      127      718 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_reset_creation.py
+-rw-r--r--   0     1001      127      725 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_revert_creation.py
+-rw-r--r--   0     1001      127      794 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_setup.py
+-rw-r--r--   0     1001      127      793 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_setup_state.py
+-rw-r--r--   0     1001      127      922 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_staging_api.py
+-rw-r--r--   0     1001      127      732 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_staging_location.py
+-rw-r--r--   0     1001      127      844 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_staging_metadata.py
+-rw-r--r--   0     1001      127      689 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_statement.py
+-rw-r--r--   0     1001      127      697 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_stats_event.py
+-rw-r--r--   0     1001      127      825 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_stats_events_list.py
+-rw-r--r--   0     1001      127      718 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_storage_config.py
+-rw-r--r--   0     1001      127      697 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_storage_uri.py
+-rw-r--r--   0     1001      127      704 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_tag_creation.py
+-rw-r--r--   0     1001      127     1013 2024-01-22 08:44:58.000000 lakefs-client-1.9.1/test/test_tags_api.py
+-rw-r--r--   0     1001      127      683 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_task_info.py
+-rw-r--r--   0     1001      127      810 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_underlying_object_properties.py
+-rw-r--r--   0     1001      127      704 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_update_token.py
+-rw-r--r--   0     1001      127      697 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_upload_part.py
+-rw-r--r--   0     1001      127      704 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_usage_report.py
+-rw-r--r--   0     1001      127      654 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_user.py
+-rw-r--r--   0     1001      127      711 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_user_creation.py
+-rw-r--r--   0     1001      127      841 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_user_list.py
+-rw-r--r--   0     1001      127      718 2024-01-22 08:44:57.000000 lakefs-client-1.9.1/test/test_version_config.py
```

### Comparing `lakefs-client-1.9.0/PKG-INFO` & `lakefs-client-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-client
-Version: 1.9.0
+Version: 1.9.1
 Summary: lakeFS API
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python-legacy
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API
 Requires-Python: >=3.6
@@ -14,15 +14,15 @@
 
 # lakefs-client
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `lakefs-client-1.9.0/README.md` & `lakefs-client-1.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lakefs-client
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `lakefs-client-1.9.0/lakefs_client/__init__.py` & `lakefs-client-1.9.1/lakefs_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 1.0.0
     Contact: services@treeverse.io
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 # import ApiClient
 from lakefs_client.api_client import ApiClient
 
 # import Configuration
 from lakefs_client.configuration import Configuration
```

### Comparing `lakefs-client-1.9.0/lakefs_client/api/actions_api.py` & `lakefs-client-1.9.1/lakefs_client/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/auth_api.py` & `lakefs-client-1.9.1/lakefs_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/branches_api.py` & `lakefs-client-1.9.1/lakefs_client/api/branches_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/commits_api.py` & `lakefs-client-1.9.1/lakefs_client/api/commits_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/config_api.py` & `lakefs-client-1.9.1/lakefs_client/api/config_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/experimental_api.py` & `lakefs-client-1.9.1/lakefs_client/api/experimental_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/health_check_api.py` & `lakefs-client-1.9.1/lakefs_client/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/import_api.py` & `lakefs-client-1.9.1/lakefs_client/api/import_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/internal_api.py` & `lakefs-client-1.9.1/lakefs_client/api/internal_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/metadata_api.py` & `lakefs-client-1.9.1/lakefs_client/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/objects_api.py` & `lakefs-client-1.9.1/lakefs_client/api/objects_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/refs_api.py` & `lakefs-client-1.9.1/lakefs_client/api/refs_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/repositories_api.py` & `lakefs-client-1.9.1/lakefs_client/api/repositories_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/staging_api.py` & `lakefs-client-1.9.1/lakefs_client/api/staging_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api/tags_api.py` & `lakefs-client-1.9.1/lakefs_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/api_client.py` & `lakefs-client-1.9.1/lakefs_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'lakefs-python-sdk/1.9.0-legacy'
+        self.user_agent = 'lakefs-python-sdk/1.9.1-legacy'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lakefs-client-1.9.0/lakefs_client/apis/__init__.py` & `lakefs-client-1.9.1/lakefs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/client.py` & `lakefs-client-1.9.1/lakefs_client/client.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/configuration.py` & `lakefs-client-1.9.1/lakefs_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.9.0".\
+               "SDK Package Version: 1.9.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lakefs-client-1.9.0/lakefs_client/exceptions.py` & `lakefs-client-1.9.1/lakefs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/abort_presign_multipart_upload.py` & `lakefs-client-1.9.1/lakefs_client/model/abort_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/access_key_credentials.py` & `lakefs-client-1.9.1/lakefs_client/model/access_key_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/acl.py` & `lakefs-client-1.9.1/lakefs_client/model/acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/action_run.py` & `lakefs-client-1.9.1/lakefs_client/model/action_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/action_run_list.py` & `lakefs-client-1.9.1/lakefs_client/model/action_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/auth_capabilities.py` & `lakefs-client-1.9.1/lakefs_client/model/auth_capabilities.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/authentication_token.py` & `lakefs-client-1.9.1/lakefs_client/model/authentication_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/branch_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/branch_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/branch_protection_rule.py` & `lakefs-client-1.9.1/lakefs_client/model/branch_protection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/cherry_pick_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/cherry_pick_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/comm_prefs_input.py` & `lakefs-client-1.9.1/lakefs_client/model/comm_prefs_input.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/commit.py` & `lakefs-client-1.9.1/lakefs_client/model/commit.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,55 +88,53 @@
         return {
             'id': (str,),  # noqa: E501
             'parents': ([str],),  # noqa: E501
             'committer': (str,),  # noqa: E501
             'message': (str,),  # noqa: E501
             'creation_date': (int,),  # noqa: E501
             'meta_range_id': (str,),  # noqa: E501
+            'metadata': ({str: (str,)},),  # noqa: E501
             'generation': (int,),  # noqa: E501
             'version': (int,),  # noqa: E501
-            'metadata': ({str: (str,)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'parents': 'parents',  # noqa: E501
         'committer': 'committer',  # noqa: E501
         'message': 'message',  # noqa: E501
         'creation_date': 'creation_date',  # noqa: E501
         'meta_range_id': 'meta_range_id',  # noqa: E501
+        'metadata': 'metadata',  # noqa: E501
         'generation': 'generation',  # noqa: E501
         'version': 'version',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, parents, committer, message, creation_date, meta_range_id, generation, version, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, parents, committer, message, creation_date, meta_range_id, *args, **kwargs):  # noqa: E501
         """Commit - a model defined in OpenAPI
 
         Args:
             id (str):
             parents ([str]):
             committer (str):
             message (str):
             creation_date (int): Unix Epoch in seconds
             meta_range_id (str):
-            generation (int):
-            version (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -162,14 +160,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             metadata ({str: (str,)}): [optional]  # noqa: E501
+            generation (int): [optional]  # noqa: E501
+            version (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,16 +195,14 @@
 
         self.id = id
         self.parents = parents
         self.committer = committer
         self.message = message
         self.creation_date = creation_date
         self.meta_range_id = meta_range_id
-        self.generation = generation
-        self.version = version
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -217,26 +215,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, parents, committer, message, creation_date, meta_range_id, generation, version, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, parents, committer, message, creation_date, meta_range_id, *args, **kwargs):  # noqa: E501
         """Commit - a model defined in OpenAPI
 
         Args:
             id (str):
             parents ([str]):
             committer (str):
             message (str):
             creation_date (int): Unix Epoch in seconds
             meta_range_id (str):
-            generation (int):
-            version (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -262,14 +258,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             metadata ({str: (str,)}): [optional]  # noqa: E501
+            generation (int): [optional]  # noqa: E501
+            version (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -293,16 +291,14 @@
 
         self.id = id
         self.parents = parents
         self.committer = committer
         self.message = message
         self.creation_date = creation_date
         self.meta_range_id = meta_range_id
-        self.generation = generation
-        self.version = version
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `lakefs-client-1.9.0/lakefs_client/model/commit_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/commit_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/commit_list.py` & `lakefs-client-1.9.1/lakefs_client/model/commit_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/commit_record_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/commit_record_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/complete_presign_multipart_upload.py` & `lakefs-client-1.9.1/lakefs_client/model/complete_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/config.py` & `lakefs-client-1.9.1/lakefs_client/model/config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/credentials.py` & `lakefs-client-1.9.1/lakefs_client/model/credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/credentials_list.py` & `lakefs-client-1.9.1/lakefs_client/model/credentials_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/credentials_with_secret.py` & `lakefs-client-1.9.1/lakefs_client/model/credentials_with_secret.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/current_user.py` & `lakefs-client-1.9.1/lakefs_client/model/current_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/diff.py` & `lakefs-client-1.9.1/lakefs_client/model/diff.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/diff_list.py` & `lakefs-client-1.9.1/lakefs_client/model/diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/diff_properties.py` & `lakefs-client-1.9.1/lakefs_client/model/diff_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/error.py` & `lakefs-client-1.9.1/lakefs_client/model/error.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/error_no_acl.py` & `lakefs-client-1.9.1/lakefs_client/model/error_no_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/find_merge_base_result.py` & `lakefs-client-1.9.1/lakefs_client/model/find_merge_base_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/garbage_collection_config.py` & `lakefs-client-1.9.1/lakefs_client/model/garbage_collection_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/garbage_collection_prepare_response.py` & `lakefs-client-1.9.1/lakefs_client/model/garbage_collection_prepare_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/garbage_collection_rule.py` & `lakefs-client-1.9.1/lakefs_client/model/garbage_collection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/garbage_collection_rules.py` & `lakefs-client-1.9.1/lakefs_client/model/garbage_collection_rules.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/group.py` & `lakefs-client-1.9.1/lakefs_client/model/group.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/group_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/group_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/group_list.py` & `lakefs-client-1.9.1/lakefs_client/model/group_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/hook_run.py` & `lakefs-client-1.9.1/lakefs_client/model/hook_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/hook_run_list.py` & `lakefs-client-1.9.1/lakefs_client/model/hook_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/import_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/import_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/import_creation_response.py` & `lakefs-client-1.9.1/lakefs_client/model/import_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/import_location.py` & `lakefs-client-1.9.1/lakefs_client/model/import_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/import_status.py` & `lakefs-client-1.9.1/lakefs_client/model/import_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/inline_object.py` & `lakefs-client-1.9.1/lakefs_client/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/inline_object1.py` & `lakefs-client-1.9.1/lakefs_client/model/inline_object1.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/installation_usage_report.py` & `lakefs-client-1.9.1/lakefs_client/model/installation_usage_report.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/login_config.py` & `lakefs-client-1.9.1/lakefs_client/model/login_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/login_information.py` & `lakefs-client-1.9.1/lakefs_client/model/login_information.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/merge.py` & `lakefs-client-1.9.1/lakefs_client/model/merge.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/merge_result.py` & `lakefs-client-1.9.1/lakefs_client/model/merge_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/meta_range_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/meta_range_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/meta_range_creation_response.py` & `lakefs-client-1.9.1/lakefs_client/model/meta_range_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/object_copy_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/object_copy_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/object_error.py` & `lakefs-client-1.9.1/lakefs_client/model/object_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/object_error_list.py` & `lakefs-client-1.9.1/lakefs_client/model/object_error_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/object_stage_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/object_stage_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/object_stats.py` & `lakefs-client-1.9.1/lakefs_client/model/object_stats.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/object_stats_list.py` & `lakefs-client-1.9.1/lakefs_client/model/object_stats_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/object_user_metadata.py` & `lakefs-client-1.9.1/lakefs_client/model/object_user_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/otf_diff_entry.py` & `lakefs-client-1.9.1/lakefs_client/model/otf_diff_entry.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/otf_diff_list.py` & `lakefs-client-1.9.1/lakefs_client/model/otf_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/otf_diffs.py` & `lakefs-client-1.9.1/lakefs_client/model/otf_diffs.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/pagination.py` & `lakefs-client-1.9.1/lakefs_client/model/pagination.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/path_list.py` & `lakefs-client-1.9.1/lakefs_client/model/path_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/policy.py` & `lakefs-client-1.9.1/lakefs_client/model/policy.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/policy_list.py` & `lakefs-client-1.9.1/lakefs_client/model/policy_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/prepare_gc_uncommitted_request.py` & `lakefs-client-1.9.1/lakefs_client/model/prepare_gc_uncommitted_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/prepare_gc_uncommitted_response.py` & `lakefs-client-1.9.1/lakefs_client/model/prepare_gc_uncommitted_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/presign_multipart_upload.py` & `lakefs-client-1.9.1/lakefs_client/model/presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/range_metadata.py` & `lakefs-client-1.9.1/lakefs_client/model/range_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/ref.py` & `lakefs-client-1.9.1/lakefs_client/model/ref.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/ref_list.py` & `lakefs-client-1.9.1/lakefs_client/model/ref_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/refs_dump.py` & `lakefs-client-1.9.1/lakefs_client/model/refs_dump.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/refs_restore.py` & `lakefs-client-1.9.1/lakefs_client/model/refs_restore.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/repository.py` & `lakefs-client-1.9.1/lakefs_client/model/repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/repository_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/repository_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/repository_dump_status.py` & `lakefs-client-1.9.1/lakefs_client/model/repository_dump_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/repository_list.py` & `lakefs-client-1.9.1/lakefs_client/model/repository_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/repository_metadata.py` & `lakefs-client-1.9.1/lakefs_client/model/repository_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/repository_metadata_keys.py` & `lakefs-client-1.9.1/lakefs_client/model/repository_metadata_keys.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/repository_metadata_set.py` & `lakefs-client-1.9.1/lakefs_client/model/repository_metadata_set.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/repository_restore_status.py` & `lakefs-client-1.9.1/lakefs_client/model/repository_restore_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/reset_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/reset_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/revert_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/revert_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/setup.py` & `lakefs-client-1.9.1/lakefs_client/model/setup.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/setup_state.py` & `lakefs-client-1.9.1/lakefs_client/model/setup_state.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/staging_location.py` & `lakefs-client-1.9.1/lakefs_client/model/staging_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/staging_metadata.py` & `lakefs-client-1.9.1/lakefs_client/model/staging_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/statement.py` & `lakefs-client-1.9.1/lakefs_client/model/statement.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/stats_event.py` & `lakefs-client-1.9.1/lakefs_client/model/stats_event.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/stats_events_list.py` & `lakefs-client-1.9.1/lakefs_client/model/stats_events_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/storage_config.py` & `lakefs-client-1.9.1/lakefs_client/model/storage_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/storage_uri.py` & `lakefs-client-1.9.1/lakefs_client/model/storage_uri.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/tag_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/tag_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/task_info.py` & `lakefs-client-1.9.1/lakefs_client/model/task_info.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/underlying_object_properties.py` & `lakefs-client-1.9.1/lakefs_client/model/underlying_object_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/update_token.py` & `lakefs-client-1.9.1/lakefs_client/model/update_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/upload_part.py` & `lakefs-client-1.9.1/lakefs_client/model/upload_part.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/usage_report.py` & `lakefs-client-1.9.1/lakefs_client/model/usage_report.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/user.py` & `lakefs-client-1.9.1/lakefs_client/model/user.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/user_creation.py` & `lakefs-client-1.9.1/lakefs_client/model/user_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/user_list.py` & `lakefs-client-1.9.1/lakefs_client/model/user_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model/version_config.py` & `lakefs-client-1.9.1/lakefs_client/model/version_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/model_utils.py` & `lakefs-client-1.9.1/lakefs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/models/__init__.py` & `lakefs-client-1.9.1/lakefs_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client/rest.py` & `lakefs-client-1.9.1/lakefs_client/rest.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/lakefs_client.egg-info/PKG-INFO` & `lakefs-client-1.9.1/lakefs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-client
-Version: 1.9.0
+Version: 1.9.1
 Summary: lakeFS API
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python-legacy
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API
 Requires-Python: >=3.6
@@ -14,15 +14,15 @@
 
 # lakefs-client
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >= 3.6
 
 ## Installation & Usage
```

### Comparing `lakefs-client-1.9.0/lakefs_client.egg-info/SOURCES.txt` & `lakefs-client-1.9.1/lakefs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/setup.py` & `lakefs-client-1.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "lakefs-client"
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `lakefs-client-1.9.0/test/test_abort_presign_multipart_upload.py` & `lakefs-client-1.9.1/test/test_abort_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_access_key_credentials.py` & `lakefs-client-1.9.1/test/test_access_key_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_acl.py` & `lakefs-client-1.9.1/test/test_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_action_run.py` & `lakefs-client-1.9.1/test/test_action_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_action_run_list.py` & `lakefs-client-1.9.1/test/test_action_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_actions_api.py` & `lakefs-client-1.9.1/test/test_actions_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_auth_api.py` & `lakefs-client-1.9.1/test/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_auth_capabilities.py` & `lakefs-client-1.9.1/test/test_auth_capabilities.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_authentication_token.py` & `lakefs-client-1.9.1/test/test_authentication_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_branch_creation.py` & `lakefs-client-1.9.1/test/test_branch_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_branch_protection_rule.py` & `lakefs-client-1.9.1/test/test_branch_protection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_branches_api.py` & `lakefs-client-1.9.1/test/test_branches_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_cherry_pick_creation.py` & `lakefs-client-1.9.1/test/test_cherry_pick_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_comm_prefs_input.py` & `lakefs-client-1.9.1/test/test_comm_prefs_input.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_commit.py` & `lakefs-client-1.9.1/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_commit_creation.py` & `lakefs-client-1.9.1/test/test_commit_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_commit_list.py` & `lakefs-client-1.9.1/test/test_commit_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_commit_record_creation.py` & `lakefs-client-1.9.1/test/test_commit_record_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_commits_api.py` & `lakefs-client-1.9.1/test/test_commits_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_complete_presign_multipart_upload.py` & `lakefs-client-1.9.1/test/test_complete_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_config.py` & `lakefs-client-1.9.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_config_api.py` & `lakefs-client-1.9.1/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_credentials.py` & `lakefs-client-1.9.1/test/test_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_credentials_list.py` & `lakefs-client-1.9.1/test/test_credentials_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_credentials_with_secret.py` & `lakefs-client-1.9.1/test/test_credentials_with_secret.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_current_user.py` & `lakefs-client-1.9.1/test/test_current_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_diff.py` & `lakefs-client-1.9.1/test/test_diff.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_diff_list.py` & `lakefs-client-1.9.1/test/test_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_diff_properties.py` & `lakefs-client-1.9.1/test/test_diff_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_error.py` & `lakefs-client-1.9.1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_error_no_acl.py` & `lakefs-client-1.9.1/test/test_error_no_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_experimental_api.py` & `lakefs-client-1.9.1/test/test_experimental_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_find_merge_base_result.py` & `lakefs-client-1.9.1/test/test_find_merge_base_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_garbage_collection_config.py` & `lakefs-client-1.9.1/test/test_garbage_collection_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_garbage_collection_prepare_response.py` & `lakefs-client-1.9.1/test/test_garbage_collection_prepare_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_garbage_collection_rule.py` & `lakefs-client-1.9.1/test/test_garbage_collection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_garbage_collection_rules.py` & `lakefs-client-1.9.1/test/test_garbage_collection_rules.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_group.py` & `lakefs-client-1.9.1/test/test_group.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_group_creation.py` & `lakefs-client-1.9.1/test/test_group_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_group_list.py` & `lakefs-client-1.9.1/test/test_group_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_health_check_api.py` & `lakefs-client-1.9.1/test/test_health_check_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_hook_run.py` & `lakefs-client-1.9.1/test/test_hook_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_hook_run_list.py` & `lakefs-client-1.9.1/test/test_hook_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_import_api.py` & `lakefs-client-1.9.1/test/test_import_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_import_creation.py` & `lakefs-client-1.9.1/test/test_import_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_import_creation_response.py` & `lakefs-client-1.9.1/test/test_import_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_import_location.py` & `lakefs-client-1.9.1/test/test_import_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_import_status.py` & `lakefs-client-1.9.1/test/test_import_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_inline_object.py` & `lakefs-client-1.9.1/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_inline_object1.py` & `lakefs-client-1.9.1/test/test_inline_object1.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_installation_usage_report.py` & `lakefs-client-1.9.1/test/test_installation_usage_report.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_internal_api.py` & `lakefs-client-1.9.1/test/test_internal_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_login_config.py` & `lakefs-client-1.9.1/test/test_login_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_login_information.py` & `lakefs-client-1.9.1/test/test_login_information.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_merge.py` & `lakefs-client-1.9.1/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_merge_result.py` & `lakefs-client-1.9.1/test/test_merge_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_meta_range_creation.py` & `lakefs-client-1.9.1/test/test_meta_range_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_meta_range_creation_response.py` & `lakefs-client-1.9.1/test/test_meta_range_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_metadata_api.py` & `lakefs-client-1.9.1/test/test_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_object_copy_creation.py` & `lakefs-client-1.9.1/test/test_object_copy_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_object_error.py` & `lakefs-client-1.9.1/test/test_object_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_object_error_list.py` & `lakefs-client-1.9.1/test/test_object_error_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_object_stage_creation.py` & `lakefs-client-1.9.1/test/test_object_stage_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_object_stats.py` & `lakefs-client-1.9.1/test/test_object_stats.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_object_stats_list.py` & `lakefs-client-1.9.1/test/test_object_stats_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_object_user_metadata.py` & `lakefs-client-1.9.1/test/test_object_user_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_objects_api.py` & `lakefs-client-1.9.1/test/test_objects_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_otf_diff_entry.py` & `lakefs-client-1.9.1/test/test_otf_diff_entry.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_otf_diff_list.py` & `lakefs-client-1.9.1/test/test_otf_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_otf_diffs.py` & `lakefs-client-1.9.1/test/test_otf_diffs.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_pagination.py` & `lakefs-client-1.9.1/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_path_list.py` & `lakefs-client-1.9.1/test/test_path_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_policy.py` & `lakefs-client-1.9.1/test/test_policy.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_policy_list.py` & `lakefs-client-1.9.1/test/test_policy_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_prepare_gc_uncommitted_request.py` & `lakefs-client-1.9.1/test/test_prepare_gc_uncommitted_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_prepare_gc_uncommitted_response.py` & `lakefs-client-1.9.1/test/test_prepare_gc_uncommitted_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_presign_multipart_upload.py` & `lakefs-client-1.9.1/test/test_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_range_metadata.py` & `lakefs-client-1.9.1/test/test_range_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_ref.py` & `lakefs-client-1.9.1/test/test_ref.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_ref_list.py` & `lakefs-client-1.9.1/test/test_ref_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_refs_api.py` & `lakefs-client-1.9.1/test/test_refs_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_refs_dump.py` & `lakefs-client-1.9.1/test/test_refs_dump.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_refs_restore.py` & `lakefs-client-1.9.1/test/test_refs_restore.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repositories_api.py` & `lakefs-client-1.9.1/test/test_repositories_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repository.py` & `lakefs-client-1.9.1/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repository_creation.py` & `lakefs-client-1.9.1/test/test_repository_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repository_dump_status.py` & `lakefs-client-1.9.1/test/test_repository_dump_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repository_list.py` & `lakefs-client-1.9.1/test/test_repository_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repository_metadata.py` & `lakefs-client-1.9.1/test/test_repository_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repository_metadata_keys.py` & `lakefs-client-1.9.1/test/test_repository_metadata_keys.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repository_metadata_set.py` & `lakefs-client-1.9.1/test/test_repository_metadata_set.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_repository_restore_status.py` & `lakefs-client-1.9.1/test/test_repository_restore_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_reset_creation.py` & `lakefs-client-1.9.1/test/test_reset_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_revert_creation.py` & `lakefs-client-1.9.1/test/test_revert_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_setup.py` & `lakefs-client-1.9.1/test/test_setup.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_setup_state.py` & `lakefs-client-1.9.1/test/test_setup_state.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_staging_api.py` & `lakefs-client-1.9.1/test/test_staging_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_staging_location.py` & `lakefs-client-1.9.1/test/test_staging_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_staging_metadata.py` & `lakefs-client-1.9.1/test/test_staging_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_statement.py` & `lakefs-client-1.9.1/test/test_statement.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_stats_event.py` & `lakefs-client-1.9.1/test/test_stats_event.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_stats_events_list.py` & `lakefs-client-1.9.1/test/test_stats_events_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_storage_config.py` & `lakefs-client-1.9.1/test/test_storage_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_storage_uri.py` & `lakefs-client-1.9.1/test/test_storage_uri.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_tag_creation.py` & `lakefs-client-1.9.1/test/test_tag_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_tags_api.py` & `lakefs-client-1.9.1/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_task_info.py` & `lakefs-client-1.9.1/test/test_task_info.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_underlying_object_properties.py` & `lakefs-client-1.9.1/test/test_underlying_object_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_update_token.py` & `lakefs-client-1.9.1/test/test_update_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_upload_part.py` & `lakefs-client-1.9.1/test/test_upload_part.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_usage_report.py` & `lakefs-client-1.9.1/test/test_usage_report.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_user.py` & `lakefs-client-1.9.1/test/test_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_user_creation.py` & `lakefs-client-1.9.1/test/test_user_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_user_list.py` & `lakefs-client-1.9.1/test/test_user_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-client-1.9.0/test/test_version_config.py` & `lakefs-client-1.9.1/test/test_version_config.py`

 * *Files identical despite different names*

