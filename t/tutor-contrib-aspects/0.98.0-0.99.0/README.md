# Comparing `tmp/tutor-contrib-aspects-0.98.0.tar.gz` & `tmp/tutor-contrib-aspects-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.98.0.tar", last modified: Sun Apr 14 20:10:21 2024, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.99.0.tar", last modified: Sun Apr 14 20:11:43 2024, max compression
```

## Comparing `tutor-contrib-aspects-0.98.0.tar` & `tutor-contrib-aspects-0.99.0.tar`

### file list

```diff
@@ -1,285 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.355970 tutor-contrib-aspects-0.98.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-14 20:10:21.355970 tutor-contrib-aspects-0.98.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.315970 tutor-contrib-aspects-0.98.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 20:10:21.355970 tutor-contrib-aspects-0.98.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.355970 tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-14 20:10:21.000000 tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19494 2024-04-14 20:10:21.000000 tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:10:21.000000 tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 20:10:21.000000 tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 20:10:21.000000 tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 20:10:21.000000 tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.315970 tutor-contrib-aspects-0.98.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/asset_command_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/commands_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/commands_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.319970 tutor-contrib-aspects-0.98.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/clickhouse-extra-sql
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/clickhouse-server-config
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/clickhouse-user-config
--rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/openedx-common-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/openedx-development-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/superset-extra-asset-translations
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/superset-extra-roles
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/superset-row-level-security
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/superset-sso-assignment-rules
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/patches/xapi-db-load-config-yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28116 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.319970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.311970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.319970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.307970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.319970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.319970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.319970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.307970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/clickhouse/users/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.307970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/ralph/config/env
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.327970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/security/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/security/partials/
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.331970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/localization/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.311970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.311970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.343970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Information.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Cumulative_Enrollments_by_Track.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Cumulative_Interactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Current_Enrollees.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_of_Current_Course_Grade.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollees_per_Enrollment_Track.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Evolution_of_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Learners_with_Passing_Grade.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Page_views_per_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_Interactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_Results.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problems_attempted_per_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Section_Summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Subsection_Summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_views_per_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.343970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)    23415 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Course_Dashboard_V1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.343970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.351970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollment_status.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_navigation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_navigation_completion.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_student_status.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/int_problem_results.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.311970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.351970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.351970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.351970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.351970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/lms/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.351970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.351970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/superset/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2373 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/base-docker-compose-services
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.311970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:10:21.355970 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/common_filters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-14 20:10:13.000000 tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.330823 tutor-contrib-aspects-0.99.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-14 20:11:43.330823 tutor-contrib-aspects-0.99.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.290823 tutor-contrib-aspects-0.99.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 20:11:43.330823 tutor-contrib-aspects-0.99.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.330823 tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-14 20:11:43.000000 tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19429 2024-04-14 20:11:43.000000 tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:11:43.000000 tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 20:11:43.000000 tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 20:11:43.000000 tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 20:11:43.000000 tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.294823 tutor-contrib-aspects-0.99.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/asset_command_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/commands_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/commands_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.298823 tutor-contrib-aspects-0.99.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/clickhouse-extra-sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/clickhouse-server-config
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/clickhouse-user-config
+-rw-r--r--   0 runner    (1001) docker     (127)    17804 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/openedx-common-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/openedx-development-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/superset-extra-asset-translations
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/superset-extra-roles
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/superset-row-level-security
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/superset-sso-assignment-rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/patches/xapi-db-load-config-yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    23422 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.298823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.290823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.298823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.286823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.298823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.298823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.298823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.286823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/clickhouse/users/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.286823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/ralph/config/env
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.302823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10687 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/security/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/security/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.306823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.310823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/localization/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.290823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.290823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.318823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Information.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Cumulative_Enrollments_by_Track.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Cumulative_Interactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Current_Enrollees.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_of_Current_Course_Grade.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollees_per_Enrollment_Track.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Evolution_of_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Learners_with_Passing_Grade.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Page_views_per_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_Interactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_Results.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problems_attempted_per_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Section_Summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Subsection_Summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_views_per_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.318823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)    23415 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Course_Dashboard_V1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.318823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.322823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollment_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_navigation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_navigation_completion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_student_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/int_problem_results.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.290823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.322823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.326823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.326823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.326823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/lms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.326823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.326823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2373 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.290823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:11:43.330823 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/common_filters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-14 20:11:34.000000 tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
```

### Comparing `tutor-contrib-aspects-0.98.0/LICENSE` & `tutor-contrib-aspects-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/PKG-INFO` & `tutor-contrib-aspects-0.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.98.0
+Version: 0.99.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.98.0/README.rst` & `tutor-contrib-aspects-0.99.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/setup.py` & `tutor-contrib-aspects-0.99.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.98.0
+Version: 0.99.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.98.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.99.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 tutoraspects/patches/superset-jinja-filters
 tutoraspects/patches/superset-row-level-security
 tutoraspects/patches/superset-sso-assignment-rules
 tutoraspects/patches/xapi-db-load-config-yaml
 tutoraspects/templates/base-docker-compose-services
 tutoraspects/templates/aspects/apps/.gitignore
 tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
-tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
 tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
 tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
 tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
 tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
 tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
 tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
 tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/asset_command_helpers.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/asset_command_helpers.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/commands_v0.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/commands_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/commands_v1.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/commands_v1.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/clickhouse-server-config` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/clickhouse-server-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/clickhouse-user-config` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/clickhouse-user-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/k8s-deployments`

 * *Files 4% similar despite different names*

```diff
@@ -108,24 +108,14 @@
               value: "0.0.0.0"
             - name: RALPH_RUNSERVER_MAX_SEARCH_HITS_COUNT
               value: "100"
             - name: RALPH_RUNSERVER_POINT_IN_TIME_KEEP_ALIVE
               value: "1m"
             - name: RALPH_RUNSERVER_PORT
               value: "{{RALPH_PORT}}"
-            - name: RALPH_SENTRY_DSN
-              value: "{{RALPH_SENTRY_DSN}}"
-            - name: RALPH_EXECUTION_ENVIRONMENT
-              value: "{{RALPH_EXECUTION_ENVIRONMENT}}"
-            - name: RALPH_SENTRY_CLI_TRACES_SAMPLE_RATE
-              value: "{{RALPH_SENTRY_CLI_TRACES_SAMPLE_RATE}}"
-            - name: RALPH_SENTRY_LRS_TRACES_SAMPLE_RATE
-              value: "{{RALPH_SENTRY_LRS_TRACES_SAMPLE_RATE}}"
-            - name: RALPH_SENTRY_IGNORE_HEALTH_CHECKS
-              value: "{{RALPH_SENTRY_IGNORE_HEALTH_CHECKS}}"
             {% if RALPH_EXTRA_SETTINGS %}
             {% for key, value in RALPH_EXTRA_SETTINGS.items() %}
             - name: {{key}}
               value: "{{value}}"
             {% endfor %}
             {% endif %}
           image: {{DOCKER_IMAGE_RALPH}}
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/k8s-jobs`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,14 @@
       containers:
       - name: aspects
         env:
           - name: VENV_DIR
             value: /opt/venv
           - name: XAPI_SCHEMA
             value: {{ ASPECTS_XAPI_DATABASE }}
-          - name: ASPECTS_ENROLLMENT_EVENTS_TABLE
-            value: {{ ASPECTS_ENROLLMENT_EVENTS_TABLE }}
           - name: DBT_STATE
             value: {{ DBT_STATE_DIR }}
         image: {{ DOCKER_IMAGE_ASPECTS }}
         securityContext:
           allowPrivilegeEscalation: false
           runAsUser: 0
         volumeMounts:
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 aspects-job:
   user: root
   image: {{ DOCKER_IMAGE_ASPECTS }}
   environment:
     - XAPI_SCHEMA={{ ASPECTS_XAPI_DATABASE }}
-    - ASPECTS_ENROLLMENT_EVENTS_TABLE={{ ASPECTS_ENROLLMENT_EVENTS_TABLE }}
   volumes:
     - ../../env/plugins/aspects/apps/aspects:/app/aspects
     - ../../env/plugins/aspects/apps/aspects/scripts/:/app/aspects/scripts:ro
     - ../../data/aspects-dbt:{{ DBT_STATE_DIR }}
   {% if RUN_SUPERSET or RUN_CLICKHOUSE or RUN_RALPH %}depends_on:{% if RUN_SUPERSET %}
     - superset{% endif %}{% if RUN_CLICKHOUSE%}
     - clickhouse{% endif %}{% if RUN_RALPH %}
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/openedx-common-settings` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/openedx-common-settings`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 	"service_url": "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ SUPERSET_HOST }}",
 	"username": "{{ SUPERSET_LMS_USERNAME }}",
 	"password": "{{ SUPERSET_LMS_PASSWORD }}",
 }
 EVENT_SINK_CLICKHOUSE_PII_MODELS = {{ EVENT_SINK_PII_MODELS }}
 
 ASPECTS_INSTRUCTOR_DASHBOARDS = {{ ASPECTS_INSTRUCTOR_DASHBOARDS }}
-SUPERSET_EXTRA_FILTERS_FORMAT = {{ ASPECTS_SUPERSET_EXTRA_FILTERS_FORMAT }}
 SUPERSET_DASHBOARD_LOCALES = {{ SUPERSET_DASHBOARD_LOCALES }}
 {% if ASPECTS_ENABLE_INSTRUCTOR_DASHBOARD_PLUGIN %}
 try:
     not OPEN_EDX_FILTERS_CONFIG
 except NameError:  # OPEN_EDX_FILTERS_CONFIG is not defined
     OPEN_EDX_FILTERS_CONFIG = {}
 if not OPEN_EDX_FILTERS_CONFIG.get("org.openedx.learning.instructor.dashboard.render.started.v1"):
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/patches/xapi-db-load-config-yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/patches/xapi-db-load-config-yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -106,45 +106,20 @@
             "SUPERSET_EMBEDDABLE_DASHBOARDS",
             {
                 "course-dashboard-v1": "c0e64194-33d1-4d5a-8c10-4f51530c5ee9",
                 "learner-groups": "8661d20c-cee6-4245-9fcc-610daea5fd24",
                 "individual-learner": "abae8a25-1ba4-4653-81bd-d3937a162a11",
             },
         ),
-        ("ASPECTS_SUPERSET_EXTRA_FILTERS_FORMAT", []),
         # ClickHouse xAPI settings
         ("ASPECTS_XAPI_DATABASE", "xapi"),
         ("ASPECTS_RAW_XAPI_TABLE", "xapi_events_all"),
-        ("ASPECTS_XAPI_TRANSFORM_MV", "xapi_events_all_parsed_mv"),
-        ("ASPECTS_XAPI_TABLE", "xapi_events_all_parsed"),
-        # ClickHouse top-level materialized views
-        ("ASPECTS_ENROLLMENT_TRANSFORM_MV", "enrollment_events_mv"),
-        ("ASPECTS_ENROLLMENT_EVENTS_TABLE", "enrollment_events"),
-        ("ASPECTS_VIDEO_PLAYBACK_TRANSFORM_MV", "video_playback_events_mv"),
-        ("ASPECTS_VIDEO_PLAYBACK_EVENTS_TABLE", "video_playback_events"),
-        ("ASPECTS_PROBLEM_TRANSFORM_MV", "problem_events_mv"),
-        ("ASPECTS_PROBLEM_EVENTS_TABLE", "problem_events"),
-        ("ASPECTS_NAVIGATION_TRANSFORM_MV", "navigation_events_mv"),
-        ("ASPECTS_NAVIGATION_EVENTS_TABLE", "navigation_events"),
-        ("ASPECTS_GRADING_TRANSFORM_MV", "grading_events_mv"),
-        ("ASPECTS_GRADING_EVENTS_TABLE", "grading_events"),
-        ("ASPECTS_FORUM_TRANSFORM_MV", "forum_events_mv"),
-        ("ASPECTS_FORUM_EVENTS_TABLE", "forum_events"),
-        ("ASPECTS_COMPLETION_EVENTS_TABLE", "completion_events"),
-        ("ASPECTS_COMPLETION_TRANSFORM_MV", "completion_events_mv"),
         # ClickHouse event sink settings
         ("ASPECTS_EVENT_SINK_DATABASE", "event_sink"),
-        ("ASPECTS_EVENT_SINK_NODES_TABLE", "course_blocks"),
-        ("ASPECTS_EVENT_SINK_RELATIONSHIPS_TABLE", "course_relationships"),
-        ("ASPECTS_EVENT_SINK_OVERVIEWS_TABLE", "course_overviews"),
-        ("ASPECTS_EVENT_SINK_USER_PROFILE_TABLE", "user_profile"),
-        ("ASPECTS_EVENT_SINK_EXTERNAL_ID_TABLE", "external_id"),
-        ("ASPECTS_EVENT_SINK_CLICKHOUSE_TIMEOUT_SECS", "5"),
-        ("ASPECTS_EVENT_SINK_RECENT_BLOCKS_TABLE", "most_recent_course_blocks"),
-        ("ASPECTS_EVENT_SINK_RECENT_BLOCKS_MV", "most_recent_course_blocks_mv"),
+        ("ASPECTS_EVENT_SINK_CLICKHOUSE_TIMEOUT_SECS", 5),
         # Vector settings
         ("ASPECTS_DOCKER_HOST_SOCK_PATH", "/var/run/docker.sock"),
         ("ASPECTS_VECTOR_STORE_TRACKING_LOGS", False),
         ("ASPECTS_VECTOR_STORE_XAPI", True),
         ("ASPECTS_VECTOR_DATABASE", "openedx"),
         ("ASPECTS_VECTOR_RAW_TRACKING_LOGS_TABLE", "_tracking"),
         ("ASPECTS_VECTOR_RAW_XAPI_TABLE", "xapi_events_all"),
@@ -238,19 +213,14 @@
         ######################
         # Ralph Settings
         # Change to https:// if the public interface to it is secure
         ("RALPH_HOST", "ralph"),
         ("RALPH_PORT", "8100"),
         ("RALPH_ENABLE_PUBLIC_URL", False),
         ("RALPH_RUN_HTTPS", False),
-        ("RALPH_SENTRY_DSN", ""),
-        ("RALPH_EXECUTION_ENVIRONMENT", "development"),
-        ("RALPH_SENTRY_CLI_TRACES_SAMPLE_RATE", 1.0),
-        ("RALPH_SENTRY_LRS_TRACES_SAMPLE_RATE", 0.1),
-        ("RALPH_SENTRY_IGNORE_HEALTH_CHECKS", True),
         ("RALPH_EXTRA_SETTINGS", {}),
         ######################
         # Superset Settings
         ("SUPERSET_HOST", "superset.{{ LMS_HOST }}"),
         ("SUPERSET_PORT", "8088"),
         ("SUPERSET_DB_DIALECT", "mysql"),
         ("SUPERSET_DB_HOST", "{{ MYSQL_HOST }}"),
@@ -275,48 +245,28 @@
                 "student": "Student",
             },
         ),
         ("SUPERSET_ADMIN_EMAIL", "admin@openedx.org"),
         ("SUPERSET_LMS_EMAIL", "superset/lms-admin@aspects.invalid"),
         ("SUPERSET_OWNERS", []),
         # Set to 0 to have no row limit.
-        ("SUPERSET_ROW_LIMIT", 100_000),
         (
             "SUPERSET_METADATA_SQLALCHEMY_URI",
             "mysql://{{SUPERSET_DB_USERNAME}}:{{SUPERSET_DB_PASSWORD}}"
             "@{{SUPERSET_DB_HOST}}/{{SUPERSET_DB_METADATA_NAME}}",
         ),
         (
             "SUPERSET_DATABASES",
             {
                 "OpenedX Clickhouse": "{{CLICKHOUSE_REPORT_SQLALCHEMY_URI}}",
                 "Superset Metadata": "{{SUPERSET_METADATA_SQLALCHEMY_URI}}",
             },
         ),
-        ("SUPERSET_SENTRY_DSN", ""),
-        (
-            "SUPERSET_TALISMAN_CONFIG",
-            {
-                "content_security_policy": {
-                    "default-src": ["'self'", "'unsafe-inline'", "'unsafe-eval'"],
-                    "img-src": ["'self'", "data:"],
-                    "worker-src": ["'self'", "blob:"],
-                    "connect-src": [
-                        "'self'",
-                        "https://api.mapbox.com",
-                        "https://events.mapbox.com",
-                    ],
-                    "object-src": "'none'",
-                }
-            },
-        ),
-        ("SUPERSET_TALISMAN_ENABLED", True),
         # These are languages that Superset itself supports, it does not currently
         # support different locales for a language.
-        ("SUPERSET_DEFAULT_LOCALE", "en"),
         (
             "SUPERSET_SUPPORTED_LANGUAGES",
             {
                 "en": {"flag": "us", "name": "English"},
                 "es": {"flag": "es", "name": "Español"},
                 "it": {"flag": "it", "name": "Italian"},
                 "fr": {"flag": "fr", "name": "French"},
@@ -361,72 +311,37 @@
         # This controls the cache time of the can_view_courses
         # wrapper, which controls the course-based permissions.
         # This includes the user roles and course list. This
         # does not get cleared on login, and so should be kept
         # short since mostly most of the savings comes from the
         # course cache anyway.
         ("SUPERSET_USER_PERMISSIONS_CACHE_TIMEOUT", 120),
-        # This controls the cache time of the user's course list
-        # only, limiting the number of LMS calls since they are
-        # rate limited. This can be cleared by logging back in.
-        ("SUPERSET_USER_COURSES_CACHE_TIMEOUT", 300),
         ("SUPERSET_BLOCK_STUDENT_ACCESS", True),
         # This setting allows Superset to run behind a reverse proxy in HTTPS and
         # redirect to the correct http/s based on the headers sent from the proxy.
         # By default it is on if Caddy is enabled, but it can be set separately in
         # case you are running a different proxy or otherwise have different needs.
         ("SUPERSET_ENABLE_PROXY_FIX", "{{ENABLE_WEB_PROXY}}"),
         # This setting allows operators to automatically refresh the datasets
         # in the Superset database. This is useful for keeping the columns up to
         # date with the latest changes in DBT.
         ("SUPERSET_REFRESH_DATASETS", False),
+        ("SUPERSET_SENTRY_DSN", ""),
         ######################
         # dbt Settings
         # For the most part you shouldn't have to touch these
         # DBT_PROFILE_* settings get passed into the dbt_profile.yml file.
         # For now we are pulling this from github, which should allow maximum
         # flexibility for forking, running branches, specific versions, etc.
         ("DBT_REPOSITORY", "https://github.com/openedx/aspects-dbt"),
         ("DBT_BRANCH", "v3.12.0"),
         ("DBT_SSH_KEY", ""),
         ("DBT_STATE_DIR", "/app/aspects/dbt_state/"),
-        # This is a pip compliant list of Python packages to install to run dbt
-        # make sure packages with versions are enclosed in double quotes
-        ("EXTRA_DBT_PACKAGES", []),
         # This is the name of the database dbt will write to
         ("DBT_PROFILE_TARGET_DATABASE", "reporting"),
-        # Validate TLS certificate if using TLS/SSL
-        ("DBT_PROFILE_VERIFY", "True"),
-        # Use TLS (native protocol) or HTTPS (http protocol)
-        ("DBT_PROFILE_SECURE", "{{ CLICKHOUSE_SECURE_CONNECTION }}"),
-        # Number of times to retry a "retryable" database exception (such as a 503
-        # 'Service Unavailable' error)
-        ("DBT_PROFILE_RETRIES", "3"),
-        # Use gzip compression if truthy (http), or compression type for a native
-        # connection
-        ("DBT_PROFILE_COMPRESSION", "lz4"),
-        # Timeout in seconds to establish a connection to ClickHouse
-        ("DBT_PROFILE_CONNECT_TIMEOUT", "10"),
-        # Timeout in seconds to receive data from the ClickHouse server
-        ("DBT_PROFILE_SEND_RECEIVE_TIMEOUT", "300"),
-        # Use specific settings designed to improve operation on replicated databases
-        # (recommended for ClickHouse Cloud)
-        ("DBT_PROFILE_CLUSTER_MODE", "False"),
-        # Use the experimental `delete+insert` as the default incremental strategy.
-        ("DBT_PROFILE_USE_LW_DELETES", "False"),
-        # Validate that clickhouse support the atomic EXCHANGE TABLES command.  (Not
-        # needed for most ClickHouse versions)
-        ("DBT_PROFILE_CHECK_EXCHANGE", "False"),
-        # A dictionary/mapping of custom ClickHouse settings for the connection -
-        # default is empty.
-        ("DBT_PROFILE_CUSTOM_SETTINGS", ""),
-        # Timeout for server ping
-        ("DBT_PROFILE_SYNC_REQUEST_TIMEOUT", "5"),
-        # Compression block size if compression is enabled, this is the default value
-        ("DBT_PROFILE_COMPRESS_BLOCK_SIZE", "1048576"),
     ]
 )
 
 # Ralph requires us to write out a file with pre-encrypted values, so we encrypt
 # them here per: https://openfun.github.io/ralph/api/#creating_a_credentials_file
 #
 # They will remain unchanged between config saves as usual and the unencryted
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 on_cluster = " ON CLUSTER '{{CLICKHOUSE_CLUSTER_NAME}}' " if "{{CLICKHOUSE_CLUSTER_NAME}}" else ""
 engine = "ReplicatedMergeTree" if "{{CLICKHOUSE_CLUSTER_NAME}}" else "MergeTree"
 
 
 def upgrade():
     op.execute(
         f"""
-        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_OVERVIEWS_TABLE }}
+        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.course_overviews
         {on_cluster}
         (
             org String NOT NULL,
             course_key String NOT NULL,
             display_name String NOT NULL,
             course_start String NOT NULL,
             course_end String NOT NULL,
@@ -31,15 +31,15 @@
         ) engine = {engine}
             PRIMARY KEY (org, course_key, modified, time_last_dumped)
             ORDER BY (org, course_key, modified, time_last_dumped);
         """
     )
     op.execute(
         f"""
-        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_NODES_TABLE }}
+        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.course_blocks
         {on_cluster}
         (
             org String NOT NULL,
             course_key String NOT NULL,
             location String NOT NULL,
             display_name String NOT NULL,
             xblock_data_json String NOT NULL,
@@ -50,15 +50,15 @@
         ) engine = {engine}
             PRIMARY KEY (org, course_key, location, edited_on)
             ORDER BY (org, course_key, location, edited_on, order);
         """
     )
     op.execute(
         f"""
-        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RELATIONSHIPS_TABLE }}
+        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.course_relationships
         {on_cluster}
         (
             course_key String NOT NULL,
             parent_location String NOT NULL,
             child_location String NOT NULL,
             order Int32 NOT NULL,
             dump_id UUID NOT NULL,
@@ -68,18 +68,18 @@
             ORDER BY (course_key, parent_location, child_location, time_last_dumped, order);
         """
     )
 
 
 def downgrade():
     op.execute(
-        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RELATIONSHIPS_TABLE }}"
+        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.course_relationships"
         f"{on_cluster}"
     )
     op.execute(
-        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_NODES_TABLE }}"
+        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.course_blocks"
         f"{on_cluster}"
     )
     op.execute(
-        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_OVERVIEWS_TABLE }}"
+        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.course_overviews"
         f"{on_cluster}"
     )
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 on_cluster = " ON CLUSTER '{{CLICKHOUSE_CLUSTER_NAME}}' " if "{{CLICKHOUSE_CLUSTER_NAME}}" else ""
 engine = "ReplicatedReplacingMergeTree" if "{{CLICKHOUSE_CLUSTER_NAME}}" else "ReplacingMergeTree"
 
 
 def upgrade():
     op.execute(
         f"""
-        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}
+        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         {on_cluster}
         (
             id Int32 NOT NULL,
             user_id Int32 NOT NULL,
             name String NOT NULL,
             meta String NOT NULL,
             courseware String NOT NULL,
@@ -49,10 +49,10 @@
         ORDER BY (id, time_last_dumped);
         """
     )
 
 
 def downgrade():
     op.execute(
-        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}"
+        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile"
         f"{on_cluster}"
     )
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     else "ReplacingMergeTree"
 )
 
 
 def drop_objects():
     op.execute(
         f"""
-        DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RECENT_BLOCKS_TABLE }}
+        DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.most_recent_course_blocks
         {on_cluster}
         """
     )
 
     op.execute(
         f"""
-        DROP VIEW IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RECENT_BLOCKS_MV }}
+        DROP VIEW IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.most_recent_course_blocks_mv
         {on_cluster}
         """
     )
 
     # We include these drop statements here because "CREATE OR REPLACE DICTIONARY"
     # currently throws a file rename error and you can't drop a dictionary with a
     # table referring to it.
@@ -49,15 +49,15 @@
 
 
 def upgrade():
     drop_objects()
 
     op.execute(
         f"""
-        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RECENT_BLOCKS_TABLE }}
+        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.most_recent_course_blocks
         {on_cluster}
         (
             location String NOT NULL,
             display_name String NOT NULL,
             display_name_with_location String NOT NULL,
             section Int32,
             subsection Int32,
@@ -69,49 +69,49 @@
         ) engine = {engine}
             PRIMARY KEY (location);
         """
     )
 
     op.execute(
         f"""
-        create materialized view if not exists {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RECENT_BLOCKS_MV }}
+        create materialized view if not exists {{ ASPECTS_EVENT_SINK_DATABASE }}.most_recent_course_blocks_mv
         {on_cluster}
-        to {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RECENT_BLOCKS_TABLE }} as
+        to {{ ASPECTS_EVENT_SINK_DATABASE }}.most_recent_course_blocks as
         select
             location,
             display_name,
             toString(section) || ':' || toString(subsection) || ':' || toString(unit) || ' - ' || display_name as display_name_with_location,
             JSONExtractInt(xblock_data_json, 'section') as section,
             JSONExtractInt(xblock_data_json, 'subsection') as subsection,
             JSONExtractInt(xblock_data_json, 'unit') as unit,
             JSONExtractBool(xblock_data_json, 'graded') as graded,
             course_key,
             dump_id,
             time_last_dumped
-        from {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_NODES_TABLE }}
+        from {{ ASPECTS_EVENT_SINK_DATABASE }}.course_blocks
         """
     )
 
     op.execute(
         """
-        insert into {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RECENT_BLOCKS_TABLE }} (
+        insert into {{ ASPECTS_EVENT_SINK_DATABASE }}.most_recent_course_blocks (
             location, display_name, display_name_with_location, section, subsection, unit, graded, course_key, dump_id, time_last_dumped
         )
         select
             location,
             display_name,
             toString(section) || ':' || toString(subsection) || ':' || toString(unit) || '- ' || display_name as display_name_with_location,
             JSONExtractInt(xblock_data_json, 'section') as section,
             JSONExtractInt(xblock_data_json, 'subsection') as subsection,
             JSONExtractInt(xblock_data_json, 'unit') as unit,
             JSONExtractBool(xblock_data_json, 'graded') as graded,
             course_key,
             dump_id,
             time_last_dumped
-        from {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_NODES_TABLE }};
+        from {{ ASPECTS_EVENT_SINK_DATABASE }}.course_blocks
         """
     )
 
     op.execute(
         f"""
         CREATE DICTIONARY {{ ASPECTS_EVENT_SINK_DATABASE }}.course_block_names_dict
         {on_cluster}
@@ -130,15 +130,15 @@
             query "
                 select
                     location,
                     display_name,
                     course_key,
                     graded,
                     display_name_with_location
-                from {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_RECENT_BLOCKS_TABLE }}
+                from {{ ASPECTS_EVENT_SINK_DATABASE }}.most_recent_course_blocks
                 final
             "
         ))
         LAYOUT(COMPLEX_KEY_SPARSE_HASHED())
         LIFETIME(120);
         """
     )
@@ -174,23 +174,23 @@
         PRIMARY KEY location
         SOURCE(CLICKHOUSE(
             user '{{ CLICKHOUSE_ADMIN_USER }}'
             password '{{ CLICKHOUSE_ADMIN_PASSWORD }}'
             db '{{ ASPECTS_EVENT_SINK_DATABASE }}'
             query "with most_recent_blocks as (
                     select org, course_key, location, max(edited_on) as last_modified
-                    from {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_NODES_TABLE }}
+                    from {{ ASPECTS_EVENT_SINK_DATABASE }}.course_blocks
                     group by org, course_key, location
                 )
                 select
                     location,
                     display_name,
                     course_key,
                     JSONExtractBool(xblock_data_json, 'graded') as graded
-                from {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_NODES_TABLE }} co
+                from {{ ASPECTS_EVENT_SINK_DATABASE }}.course_blocks co
                 inner join most_recent_blocks mrb on
                     co.org = mrb.org and
                     co.course_key = mrb.course_key and
                     co.location = mrb.location and
                     co.edited_on = mrb.last_modified
             "
         ))
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 on_cluster = " ON CLUSTER '{{CLICKHOUSE_CLUSTER_NAME}}' " if "{{CLICKHOUSE_CLUSTER_NAME}}" else ""
 engine = "ReplicatedReplacingMergeTree" if "{{CLICKHOUSE_CLUSTER_NAME}}" else "ReplacingMergeTree"
 
 
 def upgrade():
     op.execute(
         f"""
-        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_EXTERNAL_ID_TABLE }}
+        CREATE TABLE IF NOT EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.external_id
         {on_cluster}
         (
             `external_user_id` UUID NOT NULL,
             `external_id_type` String,
             `username` String,
             `user_id` Int32,
             `dump_id` UUID NOT NULL,
@@ -37,10 +37,10 @@
         ORDER BY (external_user_id, time_last_dumped)
         """
     )
 
 
 def downgrade():
     op.execute(
-        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_EXTERNAL_ID_TABLE }}"
+        "DROP TABLE IF EXISTS {{ ASPECTS_EVENT_SINK_DATABASE }}.external_id"
         f"{on_cluster}"
     )
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 revision = "0027"
 down_revision = "0026"
 branch_labels = None
 depends_on = None
 on_cluster = " ON CLUSTER '{{CLICKHOUSE_CLUSTER_NAME}}' " if "{{CLICKHOUSE_CLUSTER_NAME}}" else ""
 engine = "ReplicatedReplacingMergeTree" if "{{CLICKHOUSE_CLUSTER_NAME}}" else "ReplacingMergeTree"
 
-old_user_profile_table = "{{ASPECTS_EVENT_SINK_DATABASE}}.old_{{ASPECTS_EVENT_SINK_USER_PROFILE_TABLE}}"
+old_user_profile_table = "{{ASPECTS_EVENT_SINK_DATABASE}}.old_user_profile"
 
 def upgrade():
     # Partition event_sink.user_profile table
     # 1. Rename old table
     op.execute(
         f"""
-        RENAME TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}
+        RENAME TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         TO {old_user_profile_table}
         {on_cluster}
         """
     )
     # 2. Create partitioned table from old data
     op.execute(
         f"""
-        CREATE OR REPLACE TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}
+        CREATE OR REPLACE TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         {on_cluster}
         (
             id Int32 NOT NULL,
             user_id Int32 NOT NULL,
             name String NOT NULL,
             meta String NOT NULL,
             courseware String NOT NULL,
@@ -58,15 +58,15 @@
         PRIMARY KEY (id, time_last_dumped)
         ORDER BY (id, time_last_dumped)
         """
     )
     # 3. Insert data from the old table into the new one
     op.execute(
         f"""
-        INSERT INTO {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}
+        INSERT INTO {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         SELECT * FROM {old_user_profile_table}
         """
     )
     # 4. Drop the old table
     op.execute(
         f"""
         DROP TABLE {old_user_profile_table}
@@ -76,24 +76,24 @@
 
 
 def downgrade():
     # Un-partition the event_sink.user_profile table
     # 1a. Rename old table
     op.execute(
         f"""
-        RENAME TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}
+        RENAME TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         TO {old_user_profile_table}
         {on_cluster}
         """
     )
 
     # 2. Create un-partitioned table from old data
     op.execute(
         f"""
-        CREATE OR REPLACE TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}
+        CREATE OR REPLACE TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         {on_cluster}
         (
             id Int32 NOT NULL,
             user_id Int32 NOT NULL,
             name String NOT NULL,
             meta String NOT NULL,
             courseware String NOT NULL,
@@ -116,15 +116,15 @@
         PRIMARY KEY (id, time_last_dumped)
         ORDER BY (id, time_last_dumped)
         """
     )
     # 3. Insert into new table from old one
     op.execute(
         f"""
-        INSERT INTO {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}
+        INSERT INTO {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         SELECT * FROM {old_user_profile_table}
         """
 
     )
     # 4. Drop the old table
     op.execute(
         f"""
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                         country,
                         state,
                         goals,
                         bio,
                         profile_image_uploaded_at,
                         phone_number,
                     ROW_NUMBER() OVER (PARTITION BY user_id ORDER BY (id, time_last_dumped) DESC) as rn
-                    from {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }}
+                    from {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
                 )
                 select
                     mrup.user_id as user_id,
                     external_user_id,
                     external_id_type,
                     username,
                     name,
@@ -106,15 +106,15 @@
                     city,
                     country,
                     state,
                     goals,
                     bio,
                     profile_image_uploaded_at,
                     phone_number
-                FROM {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_EXTERNAL_ID_TABLE }} ex
+                FROM {{ ASPECTS_EVENT_SINK_DATABASE }}.external_id ex
                 RIGHT OUTER JOIN most_recent_user_profile mrup ON
                     mrup.user_id = ex.user_id and (
                        ex.external_id_type = 'xapi' OR
                        ex.external_id_type is NULL
                     )
                 WHERE mrup.rn = 1
             "
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 depends_on = None
 on_cluster = " ON CLUSTER '{{CLICKHOUSE_CLUSTER_NAME}}' " if "{{CLICKHOUSE_CLUSTER_NAME}}" else ""
 
 
 def upgrade():
     op.execute(
         f"""
-        ALTER TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }} 
+        ALTER TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         {on_cluster}
         ADD COLUMN IF NOT EXISTS email String DEFAULT '' 
         AFTER name;
         """
     )
 
 
 def downgrade():
     op.execute(
         f"""
-        ALTER TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.{{ ASPECTS_EVENT_SINK_USER_PROFILE_TABLE }} 
+        ALTER TABLE {{ ASPECTS_EVENT_SINK_DATABASE }}.user_profile
         {on_cluster}
         DROP COLUMN IF EXISTS email;
         """
     )
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 echo "Installing aspects-dbt"
 echo "git clone -b {{ DBT_BRANCH }} {{ DBT_REPOSITORY }}"
 git clone -b {{ DBT_BRANCH }} {{ DBT_REPOSITORY }} aspects-dbt
 
 cd aspects-dbt || exit
 
 echo "Installing dbt python requirements"
-pip install -r ./requirements.txt
 pip install -r /app/aspects/dbt/requirements.txt
 
 export ASPECTS_EVENT_SINK_DATABASE={{ASPECTS_EVENT_SINK_DATABASE}}
 export ASPECTS_XAPI_DATABASE={{ASPECTS_XAPI_DATABASE}}
 export DBT_STATE={{ DBT_STATE_DIR }}
 
 echo "Installing dbt dependencies"
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/conf/README.md` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/conf/README.md`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -151,20 +151,30 @@
 sentry_sdk.init(
     dsn='{{ SUPERSET_SENTRY_DSN }}',
     integrations=[FlaskIntegration()],
 )
 {% endif %}
 
 {% if ENABLE_HTTPS %}
-TALISMAN_ENABLED = {{SUPERSET_TALISMAN_ENABLED}}
-TALISMAN_CONFIG = {{SUPERSET_TALISMAN_CONFIG}}
+TALISMAN_ENABLED = True
+TALISMAN_CONFIG = {
+    "content_security_policy": {
+        "default-src": ["'self'", "'unsafe-inline'", "'unsafe-eval'"],
+        "img-src": ["'self'", "data:"],
+        "worker-src": ["'self'", "blob:"],
+        "connect-src": [
+            "'self'",
+            "https://api.mapbox.com",
+            "https://events.mapbox.com",
+        ],
+        "object-src": "'none'",
+    }
+}
 {% endif %}
-#
-
-BABEL_DEFAULT_LOCALE = "{{ SUPERSET_DEFAULT_LOCALE }}"
+BABEL_DEFAULT_LOCALE = "en"
 
 {{ patch('superset-config')}}
 
 # Optionally import superset_config_docker.py (which will have been included on
 # the PYTHONPATH) in order to allow for local settings to be overridden
 #
 try:
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from flask_appbuilder.security.manager import AUTH_OAUTH
 
 # Application secret key
 
 SECRET_KEY = os.environ["SECRET_KEY"]
 
 # Don't limit the number of rows that can be used in queries
-ROW_LIMIT = int("{{ SUPERSET_ROW_LIMIT }}")
+ROW_LIMIT = 100_000
 SQL_MAX_ROW = ROW_LIMIT
 
 OPENEDX_LMS_ROOT_URL = os.environ["OPENEDX_LMS_ROOT_URL"]
 OPENEDX_API_URLS = {
     "get_courses": urljoin(OPENEDX_LMS_ROOT_URL, "{{ SUPERSET_OPENEDX_COURSES_LIST_PATH }}"),
     "get_preference": urljoin(OPENEDX_LMS_ROOT_URL, "{{ SUPERSET_OPENEDX_PREFERENCE_PATH }}"),
 }
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/k8s.toml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/k8s.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Information.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Information.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Cumulative_Enrollments_by_Track.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Cumulative_Enrollments_by_Track.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Cumulative_Interactions.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Cumulative_Interactions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Current_Enrollees.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Current_Enrollees.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_of_Current_Course_Grade.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_of_Current_Course_Grade.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollees_per_Enrollment_Track.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollees_per_Enrollment_Track.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Evolution_of_engagement.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Evolution_of_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Learners_with_Passing_Grade.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Learners_with_Passing_Grade.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Page_views_per_section_subsection.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Page_views_per_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_Interactions.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_Interactions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_Results.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_Results.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problems_attempted_per_section_subsection.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problems_attempted_per_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Section_Summary.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Section_Summary.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Subsection_Summary.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Subsection_Summary.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_views_per_section_subsection.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_views_per_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Course_Dashboard_V1.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Course_Dashboard_V1.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -125,12 +125,12 @@
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 offset: 0
 params: null
 schema: '{{ASPECTS_EVENT_SINK_DATABASE}}'
 sql: |-
-  select * from {{ASPECTS_EVENT_SINK_DATABASE}}.{{ ASPECTS_EVENT_SINK_NODES_TABLE }}
-table_name: "{{ ASPECTS_EVENT_SINK_NODES_TABLE }}"
+  select * from {{ASPECTS_EVENT_SINK_DATABASE}}.course_blocks
+table_name: "course_blocks"
 template_params: null
 uuid: 1b73d066-fd6c-411d-a99d-fc585f9474b1
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollment_status.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollment_status.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_navigation.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_navigation.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_navigation_completion.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_navigation_completion.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_student_status.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_student_status.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/int_problem_results.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/int_problem_results.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 echo "Clickhouse is up and running"
 
 echo "Running deduplication script..."
 
 clickhouse client --user "{{ CLICKHOUSE_ADMIN_USER }}" --password="{{ CLICKHOUSE_ADMIN_PASSWORD }}" --host "{{ CLICKHOUSE_HOST }}" {% if CLICKHOUSE_SECURE_CONNECTION %} --secure {% else %} --port {{ CLICKHOUSE_INTERNAL_NATIVE_PORT }}{% endif %} --multiquery <<'EOF'
 -- Optimize final
 OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.{{ASPECTS_RAW_XAPI_TABLE}} FINAL;
-OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.{{ASPECTS_ENROLLMENT_EVENTS_TABLE}} FINAL;
-OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.{{ASPECTS_XAPI_TABLE}} FINAL;
-OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.{{ASPECTS_NAVIGATION_EVENTS_TABLE}} FINAL;
-OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.{{ASPECTS_PROBLEM_EVENTS_TABLE}} FINAL;
-OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.{{ASPECTS_VIDEO_PLAYBACK_EVENTS_TABLE}} FINAL;
+OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.enrollment_events FINAL;
+OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.xapi_events_all_parsed FINAL;
+OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.navigation_events FINAL;
+OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.problem_events FINAL;
+OPTIMIZE TABLE {{ASPECTS_XAPI_DATABASE}}.video_playback_events FINAL;
 
 EOF
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         org,
         course_key,
         splitByString('/xblock/', object_id)[-1] as video_id,
         actor_id,
         verb_id,
         video_position,
         video_duration
-    from {{ ASPECTS_XAPI_DATABASE }}.{{ ASPECTS_VIDEO_PLAYBACK_EVENTS_TABLE }}
+    from {{ ASPECTS_XAPI_DATABASE }}.video_playback_events
     where 1=1
     {% include 'openedx-assets/queries/common_filters.sql' %}
 ), starts as (
     select *
     from video_events
     where verb_id = 'https://w3id.org/xapi/video/verbs/played'
 ), ends as (
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     event_id,
     CAST(emission_time, 'DateTime') AS emission_time,
     actor_id,
     object_id,
     splitByString('/', course_id)[-1] AS course_key,
     org,
     verb_id
-  FROM {{ ASPECTS_XAPI_DATABASE }}.{{ ASPECTS_XAPI_TABLE }}
+  FROM {{ ASPECTS_XAPI_DATABASE }}.xapi_events_all_parsed
 )
 
 SELECT
   courses.course_name as course_name,
   courses.course_run as course_run,
   event_id,
   actor_id,
```

### Comparing `tutor-contrib-aspects-0.98.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql` & `tutor-contrib-aspects-0.99.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql`

 * *Files identical despite different names*

