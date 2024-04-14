# Comparing `tmp/lakefs-sdk-1.9.0.tar.gz` & `tmp/lakefs-sdk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakefs-sdk-1.9.0.tar", last modified: Sun Jan 21 12:16:32 2024, max compression
+gzip compressed data, was "lakefs-sdk-1.9.1.tar", last modified: Mon Jan 22 08:45:28 2024, max compression
```

## Comparing `lakefs-sdk-1.9.0.tar` & `lakefs-sdk-1.9.1.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:32.701829 lakefs-sdk-1.9.0/
--rw-r--r--   0     1001      127    34711 2024-01-21 12:16:32.701829 lakefs-sdk-1.9.0/PKG-INFO
--rw-r--r--   0     1001      127    26513 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/README.md
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:32.661828 lakefs-sdk-1.9.0/lakefs_sdk/
--rw-r--r--   0     1001      127     7568 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/__init__.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:32.665829 lakefs-sdk-1.9.0/lakefs_sdk/api/
--rw-r--r--   0     1001      127      811 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/__init__.py
--rw-r--r--   0     1001      127    28887 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/actions_api.py
--rw-r--r--   0     1001      127   198763 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/auth_api.py
--rw-r--r--   0     1001      127    56966 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/branches_api.py
--rw-r--r--   0     1001      127    15033 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/commits_api.py
--rw-r--r--   0     1001      127     6477 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/config_api.py
--rw-r--r--   0     1001      127    46444 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/experimental_api.py
--rw-r--r--   0     1001      127     6140 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/health_check_api.py
--rw-r--r--   0     1001      127    21428 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/import_api.py
--rw-r--r--   0     1001      127   173939 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/internal_api.py
--rw-r--r--   0     1001      127    13452 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/metadata_api.py
--rw-r--r--   0     1001      127    72798 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/objects_api.py
--rw-r--r--   0     1001      127    38427 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/refs_api.py
--rw-r--r--   0     1001      127    91068 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/repositories_api.py
--rw-r--r--   0     1001      127    16467 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/staging_api.py
--rw-r--r--   0     1001      127    27469 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api/tags_api.py
--rw-r--r--   0     1001      127    29962 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api_client.py
--rw-r--r--   0     1001      127      844 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/api_response.py
--rw-r--r--   0     1001      127     4300 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/client.py
--rw-r--r--   0     1001      127    16791 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/configuration.py
--rw-r--r--   0     1001      127     5292 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/exceptions.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:32.681829 lakefs-sdk-1.9.0/lakefs_sdk/models/
--rw-r--r--   0     1001      127     6297 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/__init__.py
--rw-r--r--   0     1001      127     1975 2024-01-21 12:16:09.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/abort_presign_multipart_upload.py
--rw-r--r--   0     1001      127     2240 2024-01-21 12:16:09.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/access_key_credentials.py
--rw-r--r--   0     1001      127     1875 2024-01-21 12:16:09.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/acl.py
--rw-r--r--   0     1001      127     2682 2024-01-21 12:16:09.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/action_run.py
--rw-r--r--   0     1001      127     2700 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/action_run_list.py
--rw-r--r--   0     1001      127     2020 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/auth_capabilities.py
--rw-r--r--   0     1001      127     2150 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/authentication_token.py
--rw-r--r--   0     1001      127     2079 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/branch_creation.py
--rw-r--r--   0     1001      127     1985 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/branch_protection_rule.py
--rw-r--r--   0     1001      127     2409 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/cherry_pick_creation.py
--rw-r--r--   0     1001      127     2323 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/comm_prefs_input.py
--rw-r--r--   0     1001      127     2693 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/commit.py
--rw-r--r--   0     1001      127     2558 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/commit_creation.py
--rw-r--r--   0     1001      127     2663 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/commit_list.py
--rw-r--r--   0     1001      127     3337 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/commit_record_creation.py
--rw-r--r--   0     1001      127     2939 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/complete_presign_multipart_upload.py
--rw-r--r--   0     1001      127     2598 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/config.py
--rw-r--r--   0     1001      127     1997 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/credentials.py
--rw-r--r--   0     1001      127     2723 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/credentials_list.py
--rw-r--r--   0     1001      127     2207 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/credentials_with_secret.py
--rw-r--r--   0     1001      127     2033 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/current_user.py
--rw-r--r--   0     1001      127     2745 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/diff.py
--rw-r--r--   0     1001      127     2639 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/diff_list.py
--rw-r--r--   0     1001      127     1823 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/diff_properties.py
--rw-r--r--   0     1001      127     1813 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/error.py
--rw-r--r--   0     1001      127     2045 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/error_no_acl.py
--rw-r--r--   0     1001      127     2325 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/find_merge_base_result.py
--rw-r--r--   0     1001      127     2067 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/garbage_collection_config.py
--rw-r--r--   0     1001      127     2749 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/garbage_collection_prepare_response.py
--rw-r--r--   0     1001      127     2028 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/garbage_collection_rule.py
--rw-r--r--   0     1001      127     2590 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/garbage_collection_rules.py
--rw-r--r--   0     1001      127     2014 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/group.py
--rw-r--r--   0     1001      127     1807 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/group_creation.py
--rw-r--r--   0     1001      127     2651 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/group_list.py
--rw-r--r--   0     1001      127     2576 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/hook_run.py
--rw-r--r--   0     1001      127     2676 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/hook_run_list.py
--rw-r--r--   0     1001      127     2844 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/import_creation.py
--rw-r--r--   0     1001      127     1923 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/import_creation_response.py
--rw-r--r--   0     1001      127     2749 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/import_location.py
--rw-r--r--   0     1001      127     3006 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/import_status.py
--rw-r--r--   0     1001      127     2520 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/installation_usage_report.py
--rw-r--r--   0     1001      127     2051 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/internal_delete_branch_protection_rule_request.py
--rw-r--r--   0     1001      127     3496 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/login_config.py
--rw-r--r--   0     1001      127     2005 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/login_information.py
--rw-r--r--   0     1001      127     2430 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/merge.py
--rw-r--r--   0     1001      127     1819 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/merge_result.py
--rw-r--r--   0     1001      127     2351 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/meta_range_creation.py
--rw-r--r--   0     1001      127     1988 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/meta_range_creation_response.py
--rw-r--r--   0     1001      127     2272 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/object_copy_creation.py
--rw-r--r--   0     1001      127     2190 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/object_error.py
--rw-r--r--   0     1001      127     2314 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/object_error_list.py
--rw-r--r--   0     1001      127     2687 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/object_stage_creation.py
--rw-r--r--   0     1001      127     3602 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/object_stats.py
--rw-r--r--   0     1001      127     2724 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/object_stats_list.py
--rw-r--r--   0     1001      127     2698 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/otf_diff_entry.py
--rw-r--r--   0     1001      127     2762 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/otf_diff_list.py
--rw-r--r--   0     1001      127     2268 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/otf_diffs.py
--rw-r--r--   0     1001      127     2359 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/pagination.py
--rw-r--r--   0     1001      127     1820 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/path_list.py
--rw-r--r--   0     1001      127     2537 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/policy.py
--rw-r--r--   0     1001      127     2663 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/policy_list.py
--rw-r--r--   0     1001      127     2007 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/prepare_gc_uncommitted_request.py
--rw-r--r--   0     1001      127     2318 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/prepare_gc_uncommitted_response.py
--rw-r--r--   0     1001      127     2206 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/presign_multipart_upload.py
--rw-r--r--   0     1001      127     2406 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/range_metadata.py
--rw-r--r--   0     1001      127     1825 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/ref.py
--rw-r--r--   0     1001      127     2627 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/ref_list.py
--rw-r--r--   0     1001      127     2127 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/refs_dump.py
--rw-r--r--   0     1001      127     2321 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/refs_restore.py
--rw-r--r--   0     1001      127     2541 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/repository.py
--rw-r--r--   0     1001      127     3270 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/repository_creation.py
--rw-r--r--   0     1001      127     2575 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/repository_dump_status.py
--rw-r--r--   0     1001      127     2711 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/repository_list.py
--rw-r--r--   0     1001      127     1928 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/repository_metadata_keys.py
--rw-r--r--   0     1001      127     1929 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/repository_metadata_set.py
--rw-r--r--   0     1001      127     2255 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/repository_restore_status.py
--rw-r--r--   0     1001      127     2402 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/reset_creation.py
--rw-r--r--   0     1001      127     2289 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/revert_creation.py
--rw-r--r--   0     1001      127     2236 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/setup.py
--rw-r--r--   0     1001      127     2800 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/setup_state.py
--rw-r--r--   0     1001      127     2828 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/staging_location.py
--rw-r--r--   0     1001      127     2917 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/staging_metadata.py
--rw-r--r--   0     1001      127     2278 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/statement.py
--rw-r--r--   0     1001      127     2269 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/stats_event.py
--rw-r--r--   0     1001      127     2310 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/stats_events_list.py
--rw-r--r--   0     1001      127     3176 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/storage_config.py
--rw-r--r--   0     1001      127     1871 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/storage_uri.py
--rw-r--r--   0     1001      127     2122 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/tag_creation.py
--rw-r--r--   0     1001      127     1797 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/task_info.py
--rw-r--r--   0     1001      127     2210 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/underlying_object_properties.py
--rw-r--r--   0     1001      127     1835 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/update_token.py
--rw-r--r--   0     1001      127     1908 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/upload_part.py
--rw-r--r--   0     1001      127     1963 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/usage_report.py
--rw-r--r--   0     1001      127     2691 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/user.py
--rw-r--r--   0     1001      127     1998 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/user_creation.py
--rw-r--r--   0     1001      127     2639 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/user_list.py
--rw-r--r--   0     1001      127     2238 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/models/version_config.py
--rw-r--r--   0     1001      127        0 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/py.typed
--rw-r--r--   0     1001      127    12858 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/lakefs_sdk/rest.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:32.701829 lakefs-sdk-1.9.0/lakefs_sdk.egg-info/
--rw-r--r--   0     1001      127    34711 2024-01-21 12:16:32.000000 lakefs-sdk-1.9.0/lakefs_sdk.egg-info/PKG-INFO
--rw-r--r--   0     1001      127     7794 2024-01-21 12:16:32.000000 lakefs-sdk-1.9.0/lakefs_sdk.egg-info/SOURCES.txt
--rw-r--r--   0     1001      127        1 2024-01-21 12:16:32.000000 lakefs-sdk-1.9.0/lakefs_sdk.egg-info/dependency_links.txt
--rw-r--r--   0     1001      127       65 2024-01-21 12:16:32.000000 lakefs-sdk-1.9.0/lakefs_sdk.egg-info/requires.txt
--rw-r--r--   0     1001      127       11 2024-01-21 12:16:32.000000 lakefs-sdk-1.9.0/lakefs_sdk.egg-info/top_level.txt
--rw-r--r--   0     1001      127      692 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/pyproject.toml
--rw-r--r--   0     1001      127       69 2024-01-21 12:16:32.701829 lakefs-sdk-1.9.0/setup.cfg
--rw-r--r--   0     1001      127     1516 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/setup.py
-drwxr-xr-x   0     1001      127        0 2024-01-21 12:16:32.701829 lakefs-sdk-1.9.0/test/
--rw-r--r--   0     1001      127     1654 2024-01-21 12:16:09.000000 lakefs-sdk-1.9.0/test/test_abort_presign_multipart_upload.py
--rw-r--r--   0     1001      127     1763 2024-01-21 12:16:09.000000 lakefs-sdk-1.9.0/test/test_access_key_credentials.py
--rw-r--r--   0     1001      127     1348 2024-01-21 12:16:09.000000 lakefs-sdk-1.9.0/test/test_acl.py
--rw-r--r--   0     1001      127     1997 2024-01-21 12:16:09.000000 lakefs-sdk-1.9.0/test/test_action_run.py
--rw-r--r--   0     1001      127     2941 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_action_run_list.py
--rw-r--r--   0     1001      127     1226 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_actions_api.py
--rw-r--r--   0     1001      127     5079 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_auth_api.py
--rw-r--r--   0     1001      127     1517 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_auth_capabilities.py
--rw-r--r--   0     1001      127     1572 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_authentication_token.py
--rw-r--r--   0     1001      127     1560 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_branch_creation.py
--rw-r--r--   0     1001      127     1566 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_branch_protection_rule.py
--rw-r--r--   0     1001      127     1773 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_branches_api.py
--rw-r--r--   0     1001      127     1586 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_cherry_pick_creation.py
--rw-r--r--   0     1001      127     1610 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_comm_prefs_input.py
--rw-r--r--   0     1001      127     1999 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_commit.py
--rw-r--r--   0     1001      127     1660 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_commit_creation.py
--rw-r--r--   0     1001      127     3005 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_commit_list.py
--rw-r--r--   0     1001      127     2214 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_commit_record_creation.py
--rw-r--r--   0     1001      127      916 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_commits_api.py
--rw-r--r--   0     1001      127     2198 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_complete_presign_multipart_upload.py
--rw-r--r--   0     1001      127     2107 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_config.py
--rw-r--r--   0     1001      127      755 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_config_api.py
--rw-r--r--   0     1001      127     1523 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_credentials.py
--rw-r--r--   0     1001      127     2283 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_credentials_list.py
--rw-r--r--   0     1001      127     1728 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_credentials_with_secret.py
--rw-r--r--   0     1001      127     1778 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_current_user.py
--rw-r--r--   0     1001      127     1538 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_diff.py
--rw-r--r--   0     1001      127     2337 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_diff_list.py
--rw-r--r--   0     1001      127     1470 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_diff_properties.py
--rw-r--r--   0     1001      127     1366 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_error.py
--rw-r--r--   0     1001      127     1462 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_error_no_acl.py
--rw-r--r--   0     1001      127     1719 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_experimental_api.py
--rw-r--r--   0     1001      127     1722 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_find_merge_base_result.py
--rw-r--r--   0     1001      127     1561 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_garbage_collection_config.py
--rw-r--r--   0     1001      127     2196 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_garbage_collection_prepare_response.py
--rw-r--r--   0     1001      127     1641 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_garbage_collection_rule.py
--rw-r--r--   0     1001      127     2055 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_garbage_collection_rules.py
--rw-r--r--   0     1001      127     1457 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_group.py
--rw-r--r--   0     1001      127     1454 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_group_creation.py
--rw-r--r--   0     1001      127     2237 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_group_list.py
--rw-r--r--   0     1001      127      791 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_health_check_api.py
--rw-r--r--   0     1001      127     1912 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_hook_run.py
--rw-r--r--   0     1001      127     2831 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_hook_run_list.py
--rw-r--r--   0     1001      127     1095 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_import_api.py
--rw-r--r--   0     1001      127     2676 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_import_creation.py
--rw-r--r--   0     1001      127     1564 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_import_creation_response.py
--rw-r--r--   0     1001      127     1720 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_import_location.py
--rw-r--r--   0     1001      127     2346 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_import_status.py
--rw-r--r--   0     1001      127     2055 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_installation_usage_report.py
--rw-r--r--   0     1001      127     5217 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_internal_api.py
--rw-r--r--   0     1001      127     1808 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_internal_delete_branch_protection_rule_request.py
--rw-r--r--   0     1001      127     1850 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_login_config.py
--rw-r--r--   0     1001      127     1593 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_login_information.py
--rw-r--r--   0     1001      127     1483 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_merge.py
--rw-r--r--   0     1001      127     1444 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_merge_result.py
--rw-r--r--   0     1001      127     2384 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_meta_range_creation.py
--rw-r--r--   0     1001      127     1577 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_meta_range_creation_response.py
--rw-r--r--   0     1001      127      970 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_metadata_api.py
--rw-r--r--   0     1001      127     1590 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_object_copy_creation.py
--rw-r--r--   0     1001      127     1537 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_object_error.py
--rw-r--r--   0     1001      127     1896 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_object_error_list.py
--rw-r--r--   0     1001      127     1866 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_object_stage_creation.py
--rw-r--r--   0     1001      127     1925 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_object_stats.py
--rw-r--r--   0     1001      127     3035 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_object_stats_list.py
--rw-r--r--   0     1001      127     2047 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_objects_api.py
--rw-r--r--   0     1001      127     1746 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_otf_diff_entry.py
--rw-r--r--   0     1001      127     2200 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_otf_diff_list.py
--rw-r--r--   0     1001      127     1500 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_otf_diffs.py
--rw-r--r--   0     1001      127     1629 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_pagination.py
--rw-r--r--   0     1001      127     1488 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_path_list.py
--rw-r--r--   0     1001      127     1994 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_policy.py
--rw-r--r--   0     1001      127     2899 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_policy_list.py
--rw-r--r--   0     1001      127     1617 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_prepare_gc_uncommitted_request.py
--rw-r--r--   0     1001      127     1781 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_prepare_gc_uncommitted_response.py
--rw-r--r--   0     1001      127     1739 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_presign_multipart_upload.py
--rw-r--r--   0     1001      127     2010 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_range_metadata.py
--rw-r--r--   0     1001      127     1397 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_ref.py
--rw-r--r--   0     1001      127     2125 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_ref_list.py
--rw-r--r--   0     1001      127     1292 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_refs_api.py
--rw-r--r--   0     1001      127     1606 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_refs_dump.py
--rw-r--r--   0     1001      127     1673 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_refs_restore.py
--rw-r--r--   0     1001      127     2792 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_repositories_api.py
--rw-r--r--   0     1001      127     1680 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_repository.py
--rw-r--r--   0     1001      127     1791 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_repository_creation.py
--rw-r--r--   0     1001      127     2054 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_repository_dump_status.py
--rw-r--r--   0     1001      127     2521 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_repository_list.py
--rw-r--r--   0     1001      127     1656 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_repository_metadata_keys.py
--rw-r--r--   0     1001      127     1668 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_repository_metadata_set.py
--rw-r--r--   0     1001      127     1881 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_repository_restore_status.py
--rw-r--r--   0     1001      127     1529 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_reset_creation.py
--rw-r--r--   0     1001      127     1572 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_revert_creation.py
--rw-r--r--   0     1001      127     1602 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_setup.py
--rw-r--r--   0     1001      127     1886 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_setup_state.py
--rw-r--r--   0     1001      127     1057 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_staging_api.py
--rw-r--r--   0     1001      127     1548 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_staging_location.py
--rw-r--r--   0     1001      127     2140 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_staging_metadata.py
--rw-r--r--   0     1001      127     1632 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_statement.py
--rw-r--r--   0     1001      127     1544 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_stats_event.py
--rw-r--r--   0     1001      127     1876 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_stats_events_list.py
--rw-r--r--   0     1001      127     2139 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_storage_config.py
--rw-r--r--   0     1001      127     1430 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_storage_uri.py
--rw-r--r--   0     1001      127     1514 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_tag_creation.py
--rw-r--r--   0     1001      127     1145 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_tags_api.py
--rw-r--r--   0     1001      127     1394 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_task_info.py
--rw-r--r--   0     1001      127     1598 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_underlying_object_properties.py
--rw-r--r--   0     1001      127     1452 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_update_token.py
--rw-r--r--   0     1001      127     1491 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_upload_part.py
--rw-r--r--   0     1001      127     1548 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_usage_report.py
--rw-r--r--   0     1001      127     1483 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_user.py
--rw-r--r--   0     1001      127     1479 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_user_creation.py
--rw-r--r--   0     1001      127     2313 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_user_list.py
--rw-r--r--   0     1001      127     1552 2024-01-21 12:16:10.000000 lakefs-sdk-1.9.0/test/test_version_config.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:28.212427 lakefs-sdk-1.9.1/
+-rw-r--r--   0     1001      127    34711 2024-01-22 08:45:28.212427 lakefs-sdk-1.9.1/PKG-INFO
+-rw-r--r--   0     1001      127    26513 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/README.md
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:28.172427 lakefs-sdk-1.9.1/lakefs_sdk/
+-rw-r--r--   0     1001      127     7568 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/__init__.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:28.176427 lakefs-sdk-1.9.1/lakefs_sdk/api/
+-rw-r--r--   0     1001      127      811 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/__init__.py
+-rw-r--r--   0     1001      127    28887 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/actions_api.py
+-rw-r--r--   0     1001      127   198763 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/auth_api.py
+-rw-r--r--   0     1001      127    56966 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/branches_api.py
+-rw-r--r--   0     1001      127    15033 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/commits_api.py
+-rw-r--r--   0     1001      127     6477 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/config_api.py
+-rw-r--r--   0     1001      127    46444 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/experimental_api.py
+-rw-r--r--   0     1001      127     6140 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/health_check_api.py
+-rw-r--r--   0     1001      127    21428 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/import_api.py
+-rw-r--r--   0     1001      127   173939 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/internal_api.py
+-rw-r--r--   0     1001      127    13452 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/metadata_api.py
+-rw-r--r--   0     1001      127    72798 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/objects_api.py
+-rw-r--r--   0     1001      127    38427 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/refs_api.py
+-rw-r--r--   0     1001      127    91068 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/repositories_api.py
+-rw-r--r--   0     1001      127    16467 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/staging_api.py
+-rw-r--r--   0     1001      127    27469 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api/tags_api.py
+-rw-r--r--   0     1001      127    29962 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api_client.py
+-rw-r--r--   0     1001      127      844 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/api_response.py
+-rw-r--r--   0     1001      127     4300 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/client.py
+-rw-r--r--   0     1001      127    16791 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/configuration.py
+-rw-r--r--   0     1001      127     5292 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/exceptions.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:28.192427 lakefs-sdk-1.9.1/lakefs_sdk/models/
+-rw-r--r--   0     1001      127     6297 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/__init__.py
+-rw-r--r--   0     1001      127     1975 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/abort_presign_multipart_upload.py
+-rw-r--r--   0     1001      127     2240 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/access_key_credentials.py
+-rw-r--r--   0     1001      127     1875 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/acl.py
+-rw-r--r--   0     1001      127     2682 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/action_run.py
+-rw-r--r--   0     1001      127     2700 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/action_run_list.py
+-rw-r--r--   0     1001      127     2020 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/auth_capabilities.py
+-rw-r--r--   0     1001      127     2150 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/authentication_token.py
+-rw-r--r--   0     1001      127     2079 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/branch_creation.py
+-rw-r--r--   0     1001      127     1985 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/branch_protection_rule.py
+-rw-r--r--   0     1001      127     2409 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/cherry_pick_creation.py
+-rw-r--r--   0     1001      127     2323 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/comm_prefs_input.py
+-rw-r--r--   0     1001      127     2701 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/commit.py
+-rw-r--r--   0     1001      127     2558 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/commit_creation.py
+-rw-r--r--   0     1001      127     2663 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/commit_list.py
+-rw-r--r--   0     1001      127     3337 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/commit_record_creation.py
+-rw-r--r--   0     1001      127     2939 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/complete_presign_multipart_upload.py
+-rw-r--r--   0     1001      127     2598 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/config.py
+-rw-r--r--   0     1001      127     1997 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/credentials.py
+-rw-r--r--   0     1001      127     2723 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/credentials_list.py
+-rw-r--r--   0     1001      127     2207 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/credentials_with_secret.py
+-rw-r--r--   0     1001      127     2033 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/current_user.py
+-rw-r--r--   0     1001      127     2745 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/diff.py
+-rw-r--r--   0     1001      127     2639 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/diff_list.py
+-rw-r--r--   0     1001      127     1823 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/diff_properties.py
+-rw-r--r--   0     1001      127     1813 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/error.py
+-rw-r--r--   0     1001      127     2045 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/error_no_acl.py
+-rw-r--r--   0     1001      127     2325 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/find_merge_base_result.py
+-rw-r--r--   0     1001      127     2067 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/garbage_collection_config.py
+-rw-r--r--   0     1001      127     2749 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/garbage_collection_prepare_response.py
+-rw-r--r--   0     1001      127     2028 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/garbage_collection_rule.py
+-rw-r--r--   0     1001      127     2590 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/garbage_collection_rules.py
+-rw-r--r--   0     1001      127     2014 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/group.py
+-rw-r--r--   0     1001      127     1807 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/group_creation.py
+-rw-r--r--   0     1001      127     2651 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/group_list.py
+-rw-r--r--   0     1001      127     2576 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/hook_run.py
+-rw-r--r--   0     1001      127     2676 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/hook_run_list.py
+-rw-r--r--   0     1001      127     2844 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/import_creation.py
+-rw-r--r--   0     1001      127     1923 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/import_creation_response.py
+-rw-r--r--   0     1001      127     2749 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/import_location.py
+-rw-r--r--   0     1001      127     3006 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/import_status.py
+-rw-r--r--   0     1001      127     2520 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/installation_usage_report.py
+-rw-r--r--   0     1001      127     2051 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/internal_delete_branch_protection_rule_request.py
+-rw-r--r--   0     1001      127     3496 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/login_config.py
+-rw-r--r--   0     1001      127     2005 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/login_information.py
+-rw-r--r--   0     1001      127     2430 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/merge.py
+-rw-r--r--   0     1001      127     1819 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/merge_result.py
+-rw-r--r--   0     1001      127     2351 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/meta_range_creation.py
+-rw-r--r--   0     1001      127     1988 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/meta_range_creation_response.py
+-rw-r--r--   0     1001      127     2272 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/object_copy_creation.py
+-rw-r--r--   0     1001      127     2190 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/object_error.py
+-rw-r--r--   0     1001      127     2314 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/object_error_list.py
+-rw-r--r--   0     1001      127     2687 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/object_stage_creation.py
+-rw-r--r--   0     1001      127     3602 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/object_stats.py
+-rw-r--r--   0     1001      127     2724 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/object_stats_list.py
+-rw-r--r--   0     1001      127     2698 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/otf_diff_entry.py
+-rw-r--r--   0     1001      127     2762 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/otf_diff_list.py
+-rw-r--r--   0     1001      127     2268 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/otf_diffs.py
+-rw-r--r--   0     1001      127     2359 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/pagination.py
+-rw-r--r--   0     1001      127     1820 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/path_list.py
+-rw-r--r--   0     1001      127     2537 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/policy.py
+-rw-r--r--   0     1001      127     2663 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/policy_list.py
+-rw-r--r--   0     1001      127     2007 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/prepare_gc_uncommitted_request.py
+-rw-r--r--   0     1001      127     2318 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/prepare_gc_uncommitted_response.py
+-rw-r--r--   0     1001      127     2206 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/presign_multipart_upload.py
+-rw-r--r--   0     1001      127     2406 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/range_metadata.py
+-rw-r--r--   0     1001      127     1825 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/ref.py
+-rw-r--r--   0     1001      127     2627 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/ref_list.py
+-rw-r--r--   0     1001      127     2127 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/refs_dump.py
+-rw-r--r--   0     1001      127     2321 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/refs_restore.py
+-rw-r--r--   0     1001      127     2541 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/repository.py
+-rw-r--r--   0     1001      127     3270 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/repository_creation.py
+-rw-r--r--   0     1001      127     2575 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/repository_dump_status.py
+-rw-r--r--   0     1001      127     2711 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/repository_list.py
+-rw-r--r--   0     1001      127     1928 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/repository_metadata_keys.py
+-rw-r--r--   0     1001      127     1929 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/repository_metadata_set.py
+-rw-r--r--   0     1001      127     2255 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/repository_restore_status.py
+-rw-r--r--   0     1001      127     2402 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/reset_creation.py
+-rw-r--r--   0     1001      127     2289 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/revert_creation.py
+-rw-r--r--   0     1001      127     2236 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/setup.py
+-rw-r--r--   0     1001      127     2800 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/setup_state.py
+-rw-r--r--   0     1001      127     2828 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/staging_location.py
+-rw-r--r--   0     1001      127     2917 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/staging_metadata.py
+-rw-r--r--   0     1001      127     2278 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/statement.py
+-rw-r--r--   0     1001      127     2269 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/stats_event.py
+-rw-r--r--   0     1001      127     2310 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/stats_events_list.py
+-rw-r--r--   0     1001      127     3176 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/storage_config.py
+-rw-r--r--   0     1001      127     1871 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/storage_uri.py
+-rw-r--r--   0     1001      127     2122 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/tag_creation.py
+-rw-r--r--   0     1001      127     1797 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/task_info.py
+-rw-r--r--   0     1001      127     2210 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/underlying_object_properties.py
+-rw-r--r--   0     1001      127     1835 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/update_token.py
+-rw-r--r--   0     1001      127     1908 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/upload_part.py
+-rw-r--r--   0     1001      127     1963 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/usage_report.py
+-rw-r--r--   0     1001      127     2691 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/user.py
+-rw-r--r--   0     1001      127     1998 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/user_creation.py
+-rw-r--r--   0     1001      127     2639 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/user_list.py
+-rw-r--r--   0     1001      127     2238 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/lakefs_sdk/models/version_config.py
+-rw-r--r--   0     1001      127        0 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/py.typed
+-rw-r--r--   0     1001      127    12858 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/lakefs_sdk/rest.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:28.212427 lakefs-sdk-1.9.1/lakefs_sdk.egg-info/
+-rw-r--r--   0     1001      127    34711 2024-01-22 08:45:28.000000 lakefs-sdk-1.9.1/lakefs_sdk.egg-info/PKG-INFO
+-rw-r--r--   0     1001      127     7794 2024-01-22 08:45:28.000000 lakefs-sdk-1.9.1/lakefs_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0     1001      127        1 2024-01-22 08:45:28.000000 lakefs-sdk-1.9.1/lakefs_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0     1001      127       65 2024-01-22 08:45:28.000000 lakefs-sdk-1.9.1/lakefs_sdk.egg-info/requires.txt
+-rw-r--r--   0     1001      127       11 2024-01-22 08:45:28.000000 lakefs-sdk-1.9.1/lakefs_sdk.egg-info/top_level.txt
+-rw-r--r--   0     1001      127      692 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/pyproject.toml
+-rw-r--r--   0     1001      127       69 2024-01-22 08:45:28.212427 lakefs-sdk-1.9.1/setup.cfg
+-rw-r--r--   0     1001      127     1516 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/setup.py
+drwxr-xr-x   0     1001      127        0 2024-01-22 08:45:28.212427 lakefs-sdk-1.9.1/test/
+-rw-r--r--   0     1001      127     1654 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_abort_presign_multipart_upload.py
+-rw-r--r--   0     1001      127     1763 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_access_key_credentials.py
+-rw-r--r--   0     1001      127     1348 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_acl.py
+-rw-r--r--   0     1001      127     1997 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_action_run.py
+-rw-r--r--   0     1001      127     2941 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_action_run_list.py
+-rw-r--r--   0     1001      127     1226 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_actions_api.py
+-rw-r--r--   0     1001      127     5079 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_auth_api.py
+-rw-r--r--   0     1001      127     1517 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_auth_capabilities.py
+-rw-r--r--   0     1001      127     1572 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_authentication_token.py
+-rw-r--r--   0     1001      127     1560 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_branch_creation.py
+-rw-r--r--   0     1001      127     1566 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_branch_protection_rule.py
+-rw-r--r--   0     1001      127     1773 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_branches_api.py
+-rw-r--r--   0     1001      127     1586 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_cherry_pick_creation.py
+-rw-r--r--   0     1001      127     1610 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_comm_prefs_input.py
+-rw-r--r--   0     1001      127     1937 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_commit.py
+-rw-r--r--   0     1001      127     1660 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_commit_creation.py
+-rw-r--r--   0     1001      127     3005 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_commit_list.py
+-rw-r--r--   0     1001      127     2214 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_commit_record_creation.py
+-rw-r--r--   0     1001      127      916 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_commits_api.py
+-rw-r--r--   0     1001      127     2198 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_complete_presign_multipart_upload.py
+-rw-r--r--   0     1001      127     2107 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_config.py
+-rw-r--r--   0     1001      127      755 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_config_api.py
+-rw-r--r--   0     1001      127     1523 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_credentials.py
+-rw-r--r--   0     1001      127     2283 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_credentials_list.py
+-rw-r--r--   0     1001      127     1728 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_credentials_with_secret.py
+-rw-r--r--   0     1001      127     1778 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_current_user.py
+-rw-r--r--   0     1001      127     1538 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_diff.py
+-rw-r--r--   0     1001      127     2337 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_diff_list.py
+-rw-r--r--   0     1001      127     1470 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_diff_properties.py
+-rw-r--r--   0     1001      127     1366 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_error.py
+-rw-r--r--   0     1001      127     1462 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_error_no_acl.py
+-rw-r--r--   0     1001      127     1719 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_experimental_api.py
+-rw-r--r--   0     1001      127     1722 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_find_merge_base_result.py
+-rw-r--r--   0     1001      127     1561 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_garbage_collection_config.py
+-rw-r--r--   0     1001      127     2196 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_garbage_collection_prepare_response.py
+-rw-r--r--   0     1001      127     1641 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_garbage_collection_rule.py
+-rw-r--r--   0     1001      127     2055 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_garbage_collection_rules.py
+-rw-r--r--   0     1001      127     1457 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_group.py
+-rw-r--r--   0     1001      127     1454 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_group_creation.py
+-rw-r--r--   0     1001      127     2237 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_group_list.py
+-rw-r--r--   0     1001      127      791 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_health_check_api.py
+-rw-r--r--   0     1001      127     1912 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_hook_run.py
+-rw-r--r--   0     1001      127     2831 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_hook_run_list.py
+-rw-r--r--   0     1001      127     1095 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_import_api.py
+-rw-r--r--   0     1001      127     2676 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_import_creation.py
+-rw-r--r--   0     1001      127     1564 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_import_creation_response.py
+-rw-r--r--   0     1001      127     1720 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_import_location.py
+-rw-r--r--   0     1001      127     2346 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_import_status.py
+-rw-r--r--   0     1001      127     2055 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_installation_usage_report.py
+-rw-r--r--   0     1001      127     5217 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_internal_api.py
+-rw-r--r--   0     1001      127     1808 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_internal_delete_branch_protection_rule_request.py
+-rw-r--r--   0     1001      127     1850 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_login_config.py
+-rw-r--r--   0     1001      127     1593 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_login_information.py
+-rw-r--r--   0     1001      127     1483 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_merge.py
+-rw-r--r--   0     1001      127     1444 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_merge_result.py
+-rw-r--r--   0     1001      127     2384 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_meta_range_creation.py
+-rw-r--r--   0     1001      127     1577 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_meta_range_creation_response.py
+-rw-r--r--   0     1001      127      970 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_metadata_api.py
+-rw-r--r--   0     1001      127     1590 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_object_copy_creation.py
+-rw-r--r--   0     1001      127     1537 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_object_error.py
+-rw-r--r--   0     1001      127     1896 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_object_error_list.py
+-rw-r--r--   0     1001      127     1866 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_object_stage_creation.py
+-rw-r--r--   0     1001      127     1925 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_object_stats.py
+-rw-r--r--   0     1001      127     3035 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_object_stats_list.py
+-rw-r--r--   0     1001      127     2047 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_objects_api.py
+-rw-r--r--   0     1001      127     1746 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_otf_diff_entry.py
+-rw-r--r--   0     1001      127     2200 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_otf_diff_list.py
+-rw-r--r--   0     1001      127     1500 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_otf_diffs.py
+-rw-r--r--   0     1001      127     1629 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_pagination.py
+-rw-r--r--   0     1001      127     1488 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_path_list.py
+-rw-r--r--   0     1001      127     1994 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_policy.py
+-rw-r--r--   0     1001      127     2899 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_policy_list.py
+-rw-r--r--   0     1001      127     1617 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_prepare_gc_uncommitted_request.py
+-rw-r--r--   0     1001      127     1781 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_prepare_gc_uncommitted_response.py
+-rw-r--r--   0     1001      127     1739 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_presign_multipart_upload.py
+-rw-r--r--   0     1001      127     2010 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_range_metadata.py
+-rw-r--r--   0     1001      127     1397 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_ref.py
+-rw-r--r--   0     1001      127     2125 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_ref_list.py
+-rw-r--r--   0     1001      127     1292 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_refs_api.py
+-rw-r--r--   0     1001      127     1606 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_refs_dump.py
+-rw-r--r--   0     1001      127     1673 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_refs_restore.py
+-rw-r--r--   0     1001      127     2792 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_repositories_api.py
+-rw-r--r--   0     1001      127     1680 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_repository.py
+-rw-r--r--   0     1001      127     1791 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_repository_creation.py
+-rw-r--r--   0     1001      127     2054 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_repository_dump_status.py
+-rw-r--r--   0     1001      127     2521 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_repository_list.py
+-rw-r--r--   0     1001      127     1656 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_repository_metadata_keys.py
+-rw-r--r--   0     1001      127     1668 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_repository_metadata_set.py
+-rw-r--r--   0     1001      127     1881 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_repository_restore_status.py
+-rw-r--r--   0     1001      127     1529 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_reset_creation.py
+-rw-r--r--   0     1001      127     1572 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_revert_creation.py
+-rw-r--r--   0     1001      127     1602 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_setup.py
+-rw-r--r--   0     1001      127     1886 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_setup_state.py
+-rw-r--r--   0     1001      127     1057 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_staging_api.py
+-rw-r--r--   0     1001      127     1548 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_staging_location.py
+-rw-r--r--   0     1001      127     2140 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_staging_metadata.py
+-rw-r--r--   0     1001      127     1632 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_statement.py
+-rw-r--r--   0     1001      127     1544 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_stats_event.py
+-rw-r--r--   0     1001      127     1876 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_stats_events_list.py
+-rw-r--r--   0     1001      127     2139 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_storage_config.py
+-rw-r--r--   0     1001      127     1430 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_storage_uri.py
+-rw-r--r--   0     1001      127     1514 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_tag_creation.py
+-rw-r--r--   0     1001      127     1145 2024-01-22 08:45:07.000000 lakefs-sdk-1.9.1/test/test_tags_api.py
+-rw-r--r--   0     1001      127     1394 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_task_info.py
+-rw-r--r--   0     1001      127     1598 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_underlying_object_properties.py
+-rw-r--r--   0     1001      127     1452 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_update_token.py
+-rw-r--r--   0     1001      127     1491 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_upload_part.py
+-rw-r--r--   0     1001      127     1548 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_usage_report.py
+-rw-r--r--   0     1001      127     1483 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_user.py
+-rw-r--r--   0     1001      127     1479 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_user_creation.py
+-rw-r--r--   0     1001      127     2313 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_user_list.py
+-rw-r--r--   0     1001      127     1552 2024-01-22 08:45:06.000000 lakefs-sdk-1.9.1/test/test_version_config.py
```

### Comparing `lakefs-sdk-1.9.0/PKG-INFO` & `lakefs-sdk-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: lakeFS API
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API
 Requires-Python: >=3.6
@@ -16,15 +16,15 @@
 
 # lakefs-sdk
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `lakefs-sdk-1.9.0/README.md` & `lakefs-sdk-1.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lakefs-sdk
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/__init__.py` & `lakefs-sdk-1.9.1/lakefs_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: services@treeverse.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 # import apis into sdk package
 from lakefs_sdk.api.actions_api import ActionsApi
 from lakefs_sdk.api.auth_api import AuthApi
 from lakefs_sdk.api.branches_api import BranchesApi
 from lakefs_sdk.api.commits_api import CommitsApi
 from lakefs_sdk.api.config_api import ConfigApi
```

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/__init__.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/actions_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/auth_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/branches_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/branches_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/commits_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/commits_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/config_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/config_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/experimental_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/experimental_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/health_check_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/import_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/import_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/internal_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/internal_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/metadata_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/objects_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/objects_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/refs_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/refs_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/repositories_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/repositories_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/staging_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/staging_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api/tags_api.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api_client.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'lakefs-python-sdk/1.9.0'
+        self.user_agent = 'lakefs-python-sdk/1.9.1'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/api_response.py` & `lakefs-sdk-1.9.1/lakefs_sdk/api_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/client.py` & `lakefs-sdk-1.9.1/lakefs_sdk/client.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/configuration.py` & `lakefs-sdk-1.9.1/lakefs_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,15 +443,15 @@
 
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

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/exceptions.py` & `lakefs-sdk-1.9.1/lakefs_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/__init__.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/abort_presign_multipart_upload.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/abort_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/access_key_credentials.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/access_key_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/acl.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/action_run.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/action_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/action_run_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/action_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/auth_capabilities.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/auth_capabilities.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/authentication_token.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/authentication_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/branch_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/branch_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/branch_protection_rule.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/branch_protection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/cherry_pick_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/cherry_pick_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/comm_prefs_input.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/comm_prefs_input.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/commit.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/commit.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     id: StrictStr = Field(...)
     parents: conlist(StrictStr) = Field(...)
     committer: StrictStr = Field(...)
     message: StrictStr = Field(...)
     creation_date: StrictInt = Field(..., description="Unix Epoch in seconds")
     meta_range_id: StrictStr = Field(...)
     metadata: Optional[Dict[str, StrictStr]] = None
-    generation: StrictInt = Field(...)
-    version: conint(strict=True, le=1, ge=0) = Field(...)
+    generation: Optional[StrictInt] = None
+    version: Optional[conint(strict=True, le=1, ge=0)] = None
     __properties = ["id", "parents", "committer", "message", "creation_date", "meta_range_id", "metadata", "generation", "version"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/commit_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/commit_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/commit_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/commit_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/commit_record_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/commit_record_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/complete_presign_multipart_upload.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/complete_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/config.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/credentials.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/credentials_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/credentials_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/credentials_with_secret.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/credentials_with_secret.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/current_user.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/current_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/diff.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/diff.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/diff_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/diff_properties.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/diff_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/error.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/error.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/error_no_acl.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/error_no_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/find_merge_base_result.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/find_merge_base_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/garbage_collection_config.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/garbage_collection_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/garbage_collection_prepare_response.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/garbage_collection_prepare_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/garbage_collection_rule.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/garbage_collection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/garbage_collection_rules.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/garbage_collection_rules.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/group.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/group.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/group_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/group_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/group_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/group_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/hook_run.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/hook_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/hook_run_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/hook_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/import_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/import_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/import_creation_response.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/import_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/import_location.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/import_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/import_status.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/import_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/installation_usage_report.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/installation_usage_report.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/internal_delete_branch_protection_rule_request.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/internal_delete_branch_protection_rule_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/login_config.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/login_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/login_information.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/login_information.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/merge.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/merge.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/merge_result.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/merge_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/meta_range_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/meta_range_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/meta_range_creation_response.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/meta_range_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/object_copy_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/object_copy_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/object_error.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/object_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/object_error_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/object_error_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/object_stage_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/object_stage_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/object_stats.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/object_stats.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/object_stats_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/object_stats_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/otf_diff_entry.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/otf_diff_entry.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/otf_diff_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/otf_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/otf_diffs.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/otf_diffs.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/pagination.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/pagination.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/path_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/path_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/policy.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/policy.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/policy_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/policy_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/prepare_gc_uncommitted_request.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/prepare_gc_uncommitted_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/prepare_gc_uncommitted_response.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/prepare_gc_uncommitted_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/presign_multipart_upload.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/range_metadata.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/range_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/ref.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/ref.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/ref_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/ref_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/refs_dump.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/refs_dump.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/refs_restore.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/refs_restore.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/repository.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/repository_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/repository_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/repository_dump_status.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/repository_dump_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/repository_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/repository_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/repository_metadata_keys.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/repository_metadata_keys.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/repository_metadata_set.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/repository_metadata_set.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/repository_restore_status.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/repository_restore_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/reset_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/reset_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/revert_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/revert_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/setup.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/setup.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/setup_state.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/setup_state.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/staging_location.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/staging_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/staging_metadata.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/staging_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/statement.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/statement.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/stats_event.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/stats_event.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/stats_events_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/stats_events_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/storage_config.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/storage_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/storage_uri.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/storage_uri.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/tag_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/tag_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/task_info.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/task_info.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/underlying_object_properties.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/underlying_object_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/update_token.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/update_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/upload_part.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/upload_part.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/usage_report.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/usage_report.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/user.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/user_creation.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/user_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/user_list.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/user_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/models/version_config.py` & `lakefs-sdk-1.9.1/lakefs_sdk/models/version_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk/rest.py` & `lakefs-sdk-1.9.1/lakefs_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk.egg-info/PKG-INFO` & `lakefs-sdk-1.9.1/lakefs_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: lakeFS API
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API
 Requires-Python: >=3.6
@@ -16,15 +16,15 @@
 
 # lakefs-sdk
 lakeFS HTTP API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `lakefs-sdk-1.9.0/lakefs_sdk.egg-info/SOURCES.txt` & `lakefs-sdk-1.9.1/lakefs_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/pyproject.toml` & `lakefs-sdk-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lakefs_sdk"
-version = "1.9.0"
+version = "1.9.1"
 description = "lakeFS API"
 authors = ["Treeverse <services@treeverse.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/treeverse/lakeFS"
 keywords = ["OpenAPI", "OpenAPI-Generator", "lakeFS API"]
 include = ["lakefs_sdk/py.typed"]
```

### Comparing `lakefs-sdk-1.9.0/setup.py` & `lakefs-sdk-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "lakefs-sdk"
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `lakefs-sdk-1.9.0/test/test_abort_presign_multipart_upload.py` & `lakefs-sdk-1.9.1/test/test_abort_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_access_key_credentials.py` & `lakefs-sdk-1.9.1/test/test_access_key_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_acl.py` & `lakefs-sdk-1.9.1/test/test_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_action_run.py` & `lakefs-sdk-1.9.1/test/test_action_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_action_run_list.py` & `lakefs-sdk-1.9.1/test/test_action_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_actions_api.py` & `lakefs-sdk-1.9.1/test/test_actions_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_auth_api.py` & `lakefs-sdk-1.9.1/test/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_auth_capabilities.py` & `lakefs-sdk-1.9.1/test/test_auth_capabilities.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_authentication_token.py` & `lakefs-sdk-1.9.1/test/test_authentication_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_branch_creation.py` & `lakefs-sdk-1.9.1/test/test_branch_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_branch_protection_rule.py` & `lakefs-sdk-1.9.1/test/test_branch_protection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_branches_api.py` & `lakefs-sdk-1.9.1/test/test_branches_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_cherry_pick_creation.py` & `lakefs-sdk-1.9.1/test/test_cherry_pick_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_comm_prefs_input.py` & `lakefs-sdk-1.9.1/test/test_comm_prefs_input.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_commit.py` & `lakefs-sdk-1.9.1/test/test_commit.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,16 +59,14 @@
                 parents = [
                     ''
                     ],
                 committer = '',
                 message = '',
                 creation_date = 56,
                 meta_range_id = '',
-                generation = 56,
-                version = 0,
         )
         """
 
     def testCommit(self):
         """Test Commit"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `lakefs-sdk-1.9.0/test/test_commit_creation.py` & `lakefs-sdk-1.9.1/test/test_commit_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_commit_list.py` & `lakefs-sdk-1.9.1/test/test_commit_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_commit_record_creation.py` & `lakefs-sdk-1.9.1/test/test_commit_record_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_commits_api.py` & `lakefs-sdk-1.9.1/test/test_commits_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_complete_presign_multipart_upload.py` & `lakefs-sdk-1.9.1/test/test_complete_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_config.py` & `lakefs-sdk-1.9.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_config_api.py` & `lakefs-sdk-1.9.1/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_credentials.py` & `lakefs-sdk-1.9.1/test/test_credentials.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_credentials_list.py` & `lakefs-sdk-1.9.1/test/test_credentials_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_credentials_with_secret.py` & `lakefs-sdk-1.9.1/test/test_credentials_with_secret.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_current_user.py` & `lakefs-sdk-1.9.1/test/test_current_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_diff.py` & `lakefs-sdk-1.9.1/test/test_diff.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_diff_list.py` & `lakefs-sdk-1.9.1/test/test_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_diff_properties.py` & `lakefs-sdk-1.9.1/test/test_diff_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_error.py` & `lakefs-sdk-1.9.1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_error_no_acl.py` & `lakefs-sdk-1.9.1/test/test_error_no_acl.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_experimental_api.py` & `lakefs-sdk-1.9.1/test/test_experimental_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_find_merge_base_result.py` & `lakefs-sdk-1.9.1/test/test_find_merge_base_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_garbage_collection_config.py` & `lakefs-sdk-1.9.1/test/test_garbage_collection_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_garbage_collection_prepare_response.py` & `lakefs-sdk-1.9.1/test/test_garbage_collection_prepare_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_garbage_collection_rule.py` & `lakefs-sdk-1.9.1/test/test_garbage_collection_rule.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_garbage_collection_rules.py` & `lakefs-sdk-1.9.1/test/test_garbage_collection_rules.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_group.py` & `lakefs-sdk-1.9.1/test/test_group.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_group_creation.py` & `lakefs-sdk-1.9.1/test/test_group_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_group_list.py` & `lakefs-sdk-1.9.1/test/test_group_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_health_check_api.py` & `lakefs-sdk-1.9.1/test/test_health_check_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_hook_run.py` & `lakefs-sdk-1.9.1/test/test_hook_run.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_hook_run_list.py` & `lakefs-sdk-1.9.1/test/test_hook_run_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_import_api.py` & `lakefs-sdk-1.9.1/test/test_import_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_import_creation.py` & `lakefs-sdk-1.9.1/test/test_import_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_import_creation_response.py` & `lakefs-sdk-1.9.1/test/test_import_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_import_location.py` & `lakefs-sdk-1.9.1/test/test_import_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_import_status.py` & `lakefs-sdk-1.9.1/test/test_import_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_installation_usage_report.py` & `lakefs-sdk-1.9.1/test/test_installation_usage_report.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_internal_api.py` & `lakefs-sdk-1.9.1/test/test_internal_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_internal_delete_branch_protection_rule_request.py` & `lakefs-sdk-1.9.1/test/test_internal_delete_branch_protection_rule_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_login_config.py` & `lakefs-sdk-1.9.1/test/test_login_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_login_information.py` & `lakefs-sdk-1.9.1/test/test_login_information.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_merge.py` & `lakefs-sdk-1.9.1/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_merge_result.py` & `lakefs-sdk-1.9.1/test/test_merge_result.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_meta_range_creation.py` & `lakefs-sdk-1.9.1/test/test_meta_range_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_meta_range_creation_response.py` & `lakefs-sdk-1.9.1/test/test_meta_range_creation_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_metadata_api.py` & `lakefs-sdk-1.9.1/test/test_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_object_copy_creation.py` & `lakefs-sdk-1.9.1/test/test_object_copy_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_object_error.py` & `lakefs-sdk-1.9.1/test/test_object_error.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_object_error_list.py` & `lakefs-sdk-1.9.1/test/test_object_error_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_object_stage_creation.py` & `lakefs-sdk-1.9.1/test/test_object_stage_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_object_stats.py` & `lakefs-sdk-1.9.1/test/test_object_stats.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_object_stats_list.py` & `lakefs-sdk-1.9.1/test/test_object_stats_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_objects_api.py` & `lakefs-sdk-1.9.1/test/test_objects_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_otf_diff_entry.py` & `lakefs-sdk-1.9.1/test/test_otf_diff_entry.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_otf_diff_list.py` & `lakefs-sdk-1.9.1/test/test_otf_diff_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_otf_diffs.py` & `lakefs-sdk-1.9.1/test/test_otf_diffs.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_pagination.py` & `lakefs-sdk-1.9.1/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_path_list.py` & `lakefs-sdk-1.9.1/test/test_path_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_policy.py` & `lakefs-sdk-1.9.1/test/test_policy.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_policy_list.py` & `lakefs-sdk-1.9.1/test/test_policy_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_prepare_gc_uncommitted_request.py` & `lakefs-sdk-1.9.1/test/test_prepare_gc_uncommitted_request.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_prepare_gc_uncommitted_response.py` & `lakefs-sdk-1.9.1/test/test_prepare_gc_uncommitted_response.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_presign_multipart_upload.py` & `lakefs-sdk-1.9.1/test/test_presign_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_range_metadata.py` & `lakefs-sdk-1.9.1/test/test_range_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_ref.py` & `lakefs-sdk-1.9.1/test/test_ref.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_ref_list.py` & `lakefs-sdk-1.9.1/test/test_ref_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_refs_api.py` & `lakefs-sdk-1.9.1/test/test_refs_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_refs_dump.py` & `lakefs-sdk-1.9.1/test/test_refs_dump.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_refs_restore.py` & `lakefs-sdk-1.9.1/test/test_refs_restore.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_repositories_api.py` & `lakefs-sdk-1.9.1/test/test_repositories_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_repository.py` & `lakefs-sdk-1.9.1/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_repository_creation.py` & `lakefs-sdk-1.9.1/test/test_repository_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_repository_dump_status.py` & `lakefs-sdk-1.9.1/test/test_repository_dump_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_repository_list.py` & `lakefs-sdk-1.9.1/test/test_repository_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_repository_metadata_keys.py` & `lakefs-sdk-1.9.1/test/test_repository_metadata_keys.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_repository_metadata_set.py` & `lakefs-sdk-1.9.1/test/test_repository_metadata_set.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_repository_restore_status.py` & `lakefs-sdk-1.9.1/test/test_repository_restore_status.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_reset_creation.py` & `lakefs-sdk-1.9.1/test/test_reset_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_revert_creation.py` & `lakefs-sdk-1.9.1/test/test_revert_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_setup.py` & `lakefs-sdk-1.9.1/test/test_setup.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_setup_state.py` & `lakefs-sdk-1.9.1/test/test_setup_state.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_staging_api.py` & `lakefs-sdk-1.9.1/test/test_staging_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_staging_location.py` & `lakefs-sdk-1.9.1/test/test_staging_location.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_staging_metadata.py` & `lakefs-sdk-1.9.1/test/test_staging_metadata.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_statement.py` & `lakefs-sdk-1.9.1/test/test_statement.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_stats_event.py` & `lakefs-sdk-1.9.1/test/test_stats_event.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_stats_events_list.py` & `lakefs-sdk-1.9.1/test/test_stats_events_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_storage_config.py` & `lakefs-sdk-1.9.1/test/test_storage_config.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_storage_uri.py` & `lakefs-sdk-1.9.1/test/test_storage_uri.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_tag_creation.py` & `lakefs-sdk-1.9.1/test/test_tag_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_tags_api.py` & `lakefs-sdk-1.9.1/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_task_info.py` & `lakefs-sdk-1.9.1/test/test_task_info.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_underlying_object_properties.py` & `lakefs-sdk-1.9.1/test/test_underlying_object_properties.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_update_token.py` & `lakefs-sdk-1.9.1/test/test_update_token.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_upload_part.py` & `lakefs-sdk-1.9.1/test/test_upload_part.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_usage_report.py` & `lakefs-sdk-1.9.1/test/test_usage_report.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_user.py` & `lakefs-sdk-1.9.1/test/test_user.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_user_creation.py` & `lakefs-sdk-1.9.1/test/test_user_creation.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_user_list.py` & `lakefs-sdk-1.9.1/test/test_user_list.py`

 * *Files identical despite different names*

### Comparing `lakefs-sdk-1.9.0/test/test_version_config.py` & `lakefs-sdk-1.9.1/test/test_version_config.py`

 * *Files identical despite different names*

