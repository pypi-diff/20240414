# Comparing `tmp/grafana-client-4.0.1.tar.gz` & `tmp/grafana_client-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana-client-4.0.1.tar", last modified: Fri Mar 29 15:29:56 2024, max compression
+gzip compressed data, was "grafana_client-4.1.0.tar", last modified: Sun Apr 14 13:59:48 2024, max compression
```

## Comparing `grafana-client-4.0.1.tar` & `grafana_client-4.1.0.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.849070 grafana-client-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    25606 2024-03-29 15:29:47.000000 grafana-client-4.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-29 15:29:47.000000 grafana-client-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-29 15:29:47.000000 grafana-client-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-03-29 15:29:56.849070 grafana-client-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-03-29 15:29:47.000000 grafana-client-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-29 15:29:47.000000 grafana-client-4.0.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.833070 grafana-client-4.0.1/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-29 15:29:47.000000 grafana-client-4.0.1/conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-29 15:29:47.000000 grafana-client-4.0.1/conda/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.833070 grafana-client-4.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 15:29:47.000000 grafana-client-4.0.1/docs/backlog.md
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-29 15:29:47.000000 grafana-client-4.0.1/docs/datasource-state.md
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-29 15:29:47.000000 grafana-client-4.0.1/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-29 15:29:47.000000 grafana-client-4.0.1/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.837070 grafana-client-4.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/async-folders-dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/datasource-health-check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/datasource-health-check.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/datasource-health-probe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/datasource-health-probe.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/datasource-smartquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/folders-dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/grafana-tokenauth-healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/grafanalib-upload-dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/service-account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-29 15:29:47.000000 grafana-client-4.0.1/examples/team.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.837070 grafana-client-4.0.1/grafana_client/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.841070 grafana-client-4.0.1/grafana_client/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.845070 grafana-client-4.0.1/grafana_client/elements/_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/alertingprovisioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/dashboard_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28591 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/libraryelement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/_async/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/alertingprovisioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/dashboard_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28121 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/libraryelement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/elements/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    15443 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-29 15:29:47.000000 grafana-client-4.0.1/grafana_client/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-29 15:29:56.000000 grafana-client-4.0.1/grafana_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.849070 grafana-client-4.0.1/grafana_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-03-29 15:29:56.000000 grafana-client-4.0.1/grafana_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-03-29 15:29:56.000000 grafana-client-4.0.1/grafana_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:29:56.000000 grafana-client-4.0.1/grafana_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:29:56.000000 grafana-client-4.0.1/grafana_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-29 15:29:56.000000 grafana-client-4.0.1/grafana_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-29 15:29:56.000000 grafana-client-4.0.1/grafana_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-29 15:29:47.000000 grafana-client-4.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.845070 grafana-client-4.0.1/script/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5982 2024-03-29 15:29:47.000000 grafana-client-4.0.1/script/generate_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-29 15:29:56.853070 grafana-client-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-29 15:29:47.000000 grafana-client-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.845070 grafana-client-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:29:56.849070 grafana-client-4.0.1/test/elements/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_alertingprovisioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_dashboard_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19699 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_datasource_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_datasource_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)    47350 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_datasource_health.py
--rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_health.py
--rw-r--r--   0 runner    (1001) docker     (127)    49875 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_libraryelement.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_rbac_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/elements/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/test_grafana_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/test_grafana_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/test_knowledge.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/test_package_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-29 15:29:47.000000 grafana-client-4.0.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.680839 grafana_client-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    25957 2024-04-14 13:59:43.000000 grafana_client-4.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-14 13:59:43.000000 grafana_client-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-14 13:59:43.000000 grafana_client-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-14 13:59:48.680839 grafana_client-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-04-14 13:59:43.000000 grafana_client-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-14 13:59:43.000000 grafana_client-4.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.664839 grafana_client-4.1.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-14 13:59:43.000000 grafana_client-4.1.0/conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-14 13:59:43.000000 grafana_client-4.1.0/conda/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.664839 grafana_client-4.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-14 13:59:43.000000 grafana_client-4.1.0/docs/backlog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-14 13:59:43.000000 grafana_client-4.1.0/docs/datasource-state.md
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 13:59:43.000000 grafana_client-4.1.0/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-14 13:59:43.000000 grafana_client-4.1.0/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.664839 grafana_client-4.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/async-folders-dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/datasource-health-check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/datasource-health-check.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/datasource-health-probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/datasource-health-probe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/datasource-smartquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/folders-dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/grafana-tokenauth-healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/grafanalib-upload-dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/service-account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-14 13:59:43.000000 grafana_client-4.1.0/examples/team.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.664839 grafana_client-4.1.0/grafana_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.668839 grafana_client-4.1.0/grafana_client/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.672839 grafana_client-4.1.0/grafana_client/elements/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/alertingprovisioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/dashboard_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28591 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/libraryelement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/_async/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/alertingprovisioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/dashboard_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28121 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/libraryelement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/elements/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15443 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-14 13:59:43.000000 grafana_client-4.1.0/grafana_client/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-14 13:59:48.000000 grafana_client-4.1.0/grafana_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.676839 grafana_client-4.1.0/grafana_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-04-14 13:59:48.000000 grafana_client-4.1.0/grafana_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-14 13:59:48.000000 grafana_client-4.1.0/grafana_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:59:48.000000 grafana_client-4.1.0/grafana_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:59:48.000000 grafana_client-4.1.0/grafana_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-14 13:59:48.000000 grafana_client-4.1.0/grafana_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-14 13:59:48.000000 grafana_client-4.1.0/grafana_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-14 13:59:43.000000 grafana_client-4.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.672839 grafana_client-4.1.0/script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5982 2024-04-14 13:59:43.000000 grafana_client-4.1.0/script/generate_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-14 13:59:48.680839 grafana_client-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-14 13:59:43.000000 grafana_client-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.672839 grafana_client-4.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:59:48.676839 grafana_client-4.1.0/test/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_alertingprovisioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_dashboard_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19699 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_datasource_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_datasource_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47350 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_datasource_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11378 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49875 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_libraryelement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10888 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_rbac_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/elements/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/test_grafana_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/test_grafana_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/test_knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/test_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-14 13:59:43.000000 grafana_client-4.1.0/test/test_util.py
```

### Comparing `grafana-client-4.0.1/CHANGELOG.md` & `grafana_client-4.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 # CHANGELOG
 
 ## unreleased
 
 
+## 4.1.0 (2024-04-14)
+
+* Fixed dashboard search endpoint wrapper.
+* Added support for query parameters on endpoints, also fixing `get_all_folders`.
+* Added missing API wrapper for Library Elements to the Async client.
+* Implemented teams read endpoints for user and actual user.
+
+All fixes and improvements submitted by @chintal. Thank you so much.
+
+
 ## 4.0.1 (2024-03-29)
 
 * Packaging: Do not mark package as "universal wheel" py2, py3.
   Thanks, @Ousret.
 
 
 ## 4.0.0 (2024-03-29)
```

### Comparing `grafana-client-4.0.1/LICENSE` & `grafana_client-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/PKG-INFO` & `grafana_client-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-client
-Version: 4.0.1
+Version: 4.1.0
 Summary: A client library for accessing the Grafana HTTP API, written in Python
 Home-page: https://github.com/panodata/grafana-client
 Author: Andrew Prokhorenkov
 Author-email: andrew.prokhorenkov@gmail.com
 Maintainer: Andreas Motl
 Maintainer-email: andreas.motl@panodata.org
 License: MIT
```

### Comparing `grafana-client-4.0.1/README.md` & `grafana_client-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/conda/meta.yaml` & `grafana_client-4.1.0/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/docs/backlog.md` & `grafana_client-4.1.0/docs/backlog.md`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/docs/datasource-state.md` & `grafana_client-4.1.0/docs/datasource-state.md`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/docs/development.md` & `grafana_client-4.1.0/docs/development.md`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/docs/index.html` & `grafana_client-4.1.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/async-folders-dashboard.py` & `grafana_client-4.1.0/examples/async-folders-dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/datasource-health-check.py` & `grafana_client-4.1.0/examples/datasource-health-check.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/datasource-health-check.rst` & `grafana_client-4.1.0/examples/datasource-health-check.rst`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/datasource-health-probe.py` & `grafana_client-4.1.0/examples/datasource-health-probe.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/datasource-health-probe.rst` & `grafana_client-4.1.0/examples/datasource-health-probe.rst`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/datasource-smartquery.py` & `grafana_client-4.1.0/examples/datasource-smartquery.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/folders-dashboard.py` & `grafana_client-4.1.0/examples/folders-dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/grafana-tokenauth-healthcheck.py` & `grafana_client-4.1.0/examples/grafana-tokenauth-healthcheck.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/grafanalib-upload-dashboard.py` & `grafana_client-4.1.0/examples/grafanalib-upload-dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/service-account.py` & `grafana_client-4.1.0/examples/service-account.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/examples/team.py` & `grafana_client-4.1.0/examples/team.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/api.py` & `grafana_client-4.1.0/grafana_client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     AsyncAlertingProvisioning,
     AsyncAnnotations,
     AsyncDashboard,
     AsyncDashboardVersions,
     AsyncDatasource,
     AsyncFolder,
     AsyncHealth,
+    AsyncLibraryElement,
     AsyncNotifications,
     AsyncOrganization,
     AsyncOrganizations,
     AsyncPlugin,
     AsyncRbac,
     AsyncSearch,
     AsyncServiceAccount,
@@ -231,14 +232,15 @@
         self.rbac = AsyncRbac(self.client)
         self.teams = AsyncTeams(self.client, self)
         self.annotations = AsyncAnnotations(self.client)
         self.snapshots = AsyncSnapshots(self.client)
         self.notifications = AsyncNotifications(self.client)
         self.plugin = AsyncPlugin(self.client)
         self.serviceaccount = AsyncServiceAccount(self.client)
+        self.libraryelement = AsyncLibraryElement(self.client, self)
 
         self._grafana_info = None
 
     async def connect(self):
         try:
             self._grafana_info = await self.health.check()
         except niquests.exceptions.ConnectionError as ex:  # pragma: no cover
```

### Comparing `grafana-client-4.0.1/grafana_client/client.py` & `grafana_client-4.1.0/grafana_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,25 +185,26 @@
         except JSONDecodeError:
             if accept_empty_json and r.text == "":
                 return ""
             else:
                 raise
 
     def __getattr__(self, item):
-        def __request_runner(url, json=None, data=None, headers=None, accept_empty_json=False):
+        def __request_runner(url, json=None, data=None, params=None, headers=None, accept_empty_json=False):
             __url = self._make_url(url)
             # Sanity checks.
             self._ensure_valid_json_arg(json)
 
             try:
                 r = self.s.request(
                     item.lower(),
                     __url,
                     json=json,
                     data=data,
+                    params=params,
                     headers=headers,
                     auth=self.auth,
                     verify=self.verify,
                     timeout=self.timeout,
                 )
             except Timeout as e:
                 raise GrafanaTimeoutError(0, None, str(e)) from e
@@ -240,25 +241,26 @@
             user_agent=user_agent,
             organization_id=organization_id,
         )
         self.s = niquests.AsyncSession()
         self.s.headers.setdefault("Connection", "keep-alive")
 
     def __getattr__(self, item):
-        async def __request_runner(url, json=None, data=None, headers=None, accept_empty_json=False):
+        async def __request_runner(url, json=None, data=None, params=None, headers=None, accept_empty_json=False):
             __url = self._make_url(url)
             # Sanity checks.
             self._ensure_valid_json_arg(json)
 
             try:
                 r = await self.s.request(
                     item.lower(),
                     __url,
                     json=json,
                     data=data,
+                    params=params,
                     headers=headers,
                     auth=self.auth,
                     verify=self.verify,
                     timeout=self.timeout,
                 )
             except Timeout as e:
                 raise GrafanaTimeoutError(0, None, str(e)) from e
```

### Comparing `grafana-client-4.0.1/grafana_client/elements/__init__.py` & `grafana_client-4.1.0/grafana_client/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/__init__.py` & `grafana_client-4.1.0/grafana_client/elements/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/admin.py` & `grafana_client-4.1.0/grafana_client/elements/_async/admin.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/alerting.py` & `grafana_client-4.1.0/grafana_client/elements/_async/alerting.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/alertingprovisioning.py` & `grafana_client-4.1.0/grafana_client/elements/_async/alertingprovisioning.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/annotations.py` & `grafana_client-4.1.0/grafana_client/elements/_async/annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/dashboard.py` & `grafana_client-4.1.0/grafana_client/elements/_async/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/dashboard_versions.py` & `grafana_client-4.1.0/grafana_client/elements/_async/dashboard_versions.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/datasource.py` & `grafana_client-4.1.0/grafana_client/elements/_async/datasource.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/folder.py` & `grafana_client-4.1.0/grafana_client/elements/_async/folder.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
     async def get_all_folders(self, parent_uid=None):
         """
 
         :return:
         """
         path = "/folders"
-        data = {}
+        params = {}
         if parent_uid:
-            data["parentUid"] = parent_uid
-        return await self.client.GET(path, data=data)
+            params["parentUid"] = parent_uid
+        return await self.client.GET(path, params=params)
 
     async def get_folder(self, uid):
         """
 
         :param uid:
         :return:
         """
```

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/libraryelement.py` & `grafana_client-4.1.0/grafana_client/elements/_async/libraryelement.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/notifications.py` & `grafana_client-4.1.0/grafana_client/elements/_async/notifications.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/organization.py` & `grafana_client-4.1.0/grafana_client/elements/_async/organization.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/plugin.py` & `grafana_client-4.1.0/grafana_client/elements/_async/plugin.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/rbac.py` & `grafana_client-4.1.0/grafana_client/elements/_async/rbac.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/service_account.py` & `grafana_client-4.1.0/grafana_client/elements/_async/service_account.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/snapshots.py` & `grafana_client-4.1.0/grafana_client/elements/_async/snapshots.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/team.py` & `grafana_client-4.1.0/grafana_client/elements/_async/team.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/_async/user.py` & `grafana_client-4.1.0/grafana_client/elements/_async/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,23 @@
 
         :param user_id:
         :return:
         """
         get_user_organisations_path = "/users/%s/orgs" % user_id
         return await self.client.GET(get_user_organisations_path)
 
+    async def get_user_teams(self, user_id):
+        """
+
+        :param user_id:
+        :return:
+        """
+        get_user_teams_path = "/users/%s/teams" % user_id
+        return await self.client.GET(get_user_teams_path)
+
 
 class User(Base):
     def __init__(self, client):
         super(User, self).__init__(client)
         self.client = client
         self.path = "/user"
 
@@ -141,14 +150,22 @@
         """
 
         :return:
         """
         get_actual_user_organisations_path = "/user/orgs"
         return await self.client.GET(get_actual_user_organisations_path)
 
+    async def get_actual_user_teams(self):
+        """
+
+        :return:
+        """
+        get_actual_user_teams_path = "/user/teams"
+        return await self.client.GET(get_actual_user_teams_path)
+
     async def star_actual_user_dashboard(self, dashboard_id):
         """
 
         :param dashboard_id:
         :return:
         """
         star_dashboard = "/user/stars/dashboard/%s" % dashboard_id
```

### Comparing `grafana-client-4.0.1/grafana_client/elements/admin.py` & `grafana_client-4.1.0/grafana_client/elements/admin.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/alerting.py` & `grafana_client-4.1.0/grafana_client/elements/alerting.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/alertingprovisioning.py` & `grafana_client-4.1.0/grafana_client/elements/alertingprovisioning.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/annotations.py` & `grafana_client-4.1.0/grafana_client/elements/annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/dashboard.py` & `grafana_client-4.1.0/grafana_client/elements/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/dashboard_versions.py` & `grafana_client-4.1.0/grafana_client/elements/dashboard_versions.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/datasource.py` & `grafana_client-4.1.0/grafana_client/elements/datasource.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/folder.py` & `grafana_client-4.1.0/grafana_client/elements/folder.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
     def get_all_folders(self, parent_uid=None):
         """
 
         :return:
         """
         path = "/folders"
-        data = {}
+        params = {}
         if parent_uid:
-            data["parentUid"] = parent_uid
-        return self.client.GET(path, data=data)
+            params["parentUid"] = parent_uid
+        return self.client.GET(path, params=params)
 
     def get_folder(self, uid):
         """
 
         :param uid:
         :return:
         """
```

### Comparing `grafana-client-4.0.1/grafana_client/elements/libraryelement.py` & `grafana_client-4.1.0/grafana_client/elements/libraryelement.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/notifications.py` & `grafana_client-4.1.0/grafana_client/elements/notifications.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/organization.py` & `grafana_client-4.1.0/grafana_client/elements/organization.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/plugin.py` & `grafana_client-4.1.0/grafana_client/elements/plugin.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/rbac.py` & `grafana_client-4.1.0/grafana_client/elements/rbac.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/search.py` & `grafana_client-4.1.0/grafana_client/elements/_async/search.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,66 @@
-from .base import Base
+from grafana_client.util import format_param_value
+
+from ..base import Base
 
 
 class Search(Base):
     def __init__(self, client):
         super(Search, self).__init__(client)
         self.client = client
 
-    def search_dashboards(
+    async def search_dashboards(
         self,
         query=None,
         tag=None,
         type_=None,
         dashboard_ids=None,
+        dashboard_uids=None,
         folder_ids=None,
+        folder_uids=None,
         starred=None,
         limit=None,
     ):
         """
 
         :param query:
         :param tag:
         :param type_:
         :param dashboard_ids:
+        :param dashboard_uids:
         :param folder_ids:
+        :param folder_uids:
         :param starred:
         :param limit:
         :return:
         """
         list_dashboard_path = "/search"
-        params = []
+        params = {}
 
         if query:
-            params.append("query=%s" % query)
+            params["query"] = query
 
         if tag:
-            params.append("tag=%s" % tag)
+            params["tag"] = format_param_value(tag)
 
         if type_:
-            params.append("type=%s" % type_)
+            params["type"] = type_
 
         if dashboard_ids:
-            params.append("dashboardIds=%s" % dashboard_ids)
+            params["dashboardIds"] = format_param_value(dashboard_ids)
+
+        if dashboard_uids:
+            params["dashboardUIDs"] = format_param_value(dashboard_uids)
 
         if folder_ids:
-            params.append("folderIds=%s" % folder_ids)
+            params["folderIds"] = format_param_value(folder_ids)
+
+        if folder_uids:
+            params["folderUIDs"] = format_param_value(folder_uids)
 
         if starred:
-            params.append("starred=%s" % starred)
+            params["starred"] = starred
 
         if limit:
-            params.append("limit=%s" % limit)
-
-        list_dashboard_path += "?"
-        list_dashboard_path += "&".join(params)
+            params["limit"] = limit
 
-        return self.client.GET(list_dashboard_path)
+        return await self.client.GET(list_dashboard_path, params=params)
```

### Comparing `grafana-client-4.0.1/grafana_client/elements/service_account.py` & `grafana_client-4.1.0/grafana_client/elements/service_account.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/snapshots.py` & `grafana_client-4.1.0/grafana_client/elements/snapshots.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/team.py` & `grafana_client-4.1.0/grafana_client/elements/team.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/elements/user.py` & `grafana_client-4.1.0/grafana_client/elements/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,14 +81,23 @@
 
         :param user_id:
         :return:
         """
         get_user_organisations_path = "/users/%s/orgs" % user_id
         return self.client.GET(get_user_organisations_path)
 
+    def get_user_teams(self, user_id):
+        """
+
+        :param user_id:
+        :return:
+        """
+        get_user_teams_path = "/users/%s/teams" % user_id
+        return self.client.GET(get_user_teams_path)
+
 
 class User(Base):
     def __init__(self, client):
         super(User, self).__init__(client)
         self.client = client
         self.path = "/user"
 
@@ -141,14 +150,22 @@
         """
 
         :return:
         """
         get_actual_user_organisations_path = "/user/orgs"
         return self.client.GET(get_actual_user_organisations_path)
 
+    def get_actual_user_teams(self):
+        """
+
+        :return:
+        """
+        get_actual_user_teams_path = "/user/teams"
+        return self.client.GET(get_actual_user_teams_path)
+
     def star_actual_user_dashboard(self, dashboard_id):
         """
 
         :param dashboard_id:
         :return:
         """
         star_dashboard = "/user/stars/dashboard/%s" % dashboard_id
```

### Comparing `grafana-client-4.0.1/grafana_client/knowledge.py` & `grafana_client-4.1.0/grafana_client/knowledge.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client/model.py` & `grafana_client-4.1.0/grafana_client/model.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/grafana_client.egg-info/PKG-INFO` & `grafana_client-4.1.0/grafana_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-client
-Version: 4.0.1
+Version: 4.1.0
 Summary: A client library for accessing the Grafana HTTP API, written in Python
 Home-page: https://github.com/panodata/grafana-client
 Author: Andrew Prokhorenkov
 Author-email: andrew.prokhorenkov@gmail.com
 Maintainer: Andreas Motl
 Maintainer-email: andreas.motl@panodata.org
 License: MIT
```

### Comparing `grafana-client-4.0.1/grafana_client.egg-info/SOURCES.txt` & `grafana_client-4.1.0/grafana_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/pyproject.toml` & `grafana_client-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/script/generate_async.py` & `grafana_client-4.1.0/script/generate_async.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/setup.cfg` & `grafana_client-4.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/compat.py` & `grafana_client-4.1.0/test/compat.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_admin.py` & `grafana_client-4.1.0/test/elements/test_admin.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_alerting.py` & `grafana_client-4.1.0/test/elements/test_alerting.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_alertingprovisioning.py` & `grafana_client-4.1.0/test/elements/test_alertingprovisioning.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_annotations.py` & `grafana_client-4.1.0/test/elements/test_annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_dashboard.py` & `grafana_client-4.1.0/test/elements/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_dashboard_versions.py` & `grafana_client-4.1.0/test/elements/test_dashboard_versions.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_datasource_base.py` & `grafana_client-4.1.0/test/elements/test_datasource_base.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_datasource_fixtures.py` & `grafana_client-4.1.0/test/elements/test_datasource_fixtures.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_datasource_health.py` & `grafana_client-4.1.0/test/elements/test_datasource_health.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_folder.py` & `grafana_client-4.1.0/test/elements/test_folder.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_health.py` & `grafana_client-4.1.0/test/elements/test_health.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_libraryelement.py` & `grafana_client-4.1.0/test/elements/test_libraryelement.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_notifications.py` & `grafana_client-4.1.0/test/elements/test_notifications.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_organization.py` & `grafana_client-4.1.0/test/elements/test_organization.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_plugin.py` & `grafana_client-4.1.0/test/elements/test_plugin.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_rbac.py` & `grafana_client-4.1.0/test/elements/test_rbac.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_rbac_fixtures.py` & `grafana_client-4.1.0/test/elements/test_rbac_fixtures.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_search.py` & `grafana_client-4.1.0/test/elements/test_search.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_service_account.py` & `grafana_client-4.1.0/test/elements/test_service_account.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_snapshot.py` & `grafana_client-4.1.0/test/elements/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_team.py` & `grafana_client-4.1.0/test/elements/test_team.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/elements/test_user.py` & `grafana_client-4.1.0/test/elements/test_user.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/test_async.py` & `grafana_client-4.1.0/test/test_async.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/test_grafana_api.py` & `grafana_client-4.1.0/test/test_grafana_api.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/test_grafana_client.py` & `grafana_client-4.1.0/test/test_grafana_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from unittest.mock import Mock, patch
 
 import niquests
 
 from grafana_client.api import GrafanaApi
 from grafana_client.client import (
     GrafanaClientError,
+    GrafanaServerError,
     GrafanaTimeoutError,
     HeaderAuth,
     TokenAuth,
 )
 
 
 class MockResponse:
@@ -91,14 +92,15 @@
         grafana.users.find_user("test@example.org")
         grafana.client.s.request.assert_called_once_with(
             "get",
             "https://localhost/api/users/lookup?loginOrEmail=test@example.org",
             auth=basic_auth,
             headers=None,
             json=None,
+            params=None,
             data=None,
             verify=False,
             timeout=5.0,
         )
 
     def test_grafana_client_timeout(self):
         grafana = GrafanaApi(
@@ -156,15 +158,15 @@
         mock_get.return_value = Mock()
         mock_get.return_value.return_value = {"commit": "14e988bd22", "database": "ok", "version": "9.0.1"}
         grafana = GrafanaApi(auth=None, host="localhost", url_path_prefix="", protocol="http", port="3000")
         self.assertEqual(grafana.version, "9.0.1")
 
     def test_grafana_client_non_json_response(self):
         grafana = GrafanaApi.from_url("https://example.org/")
-        self.assertRaises(GrafanaClientError, lambda: grafana.connect())
+        self.assertRaises((GrafanaClientError, GrafanaServerError), lambda: grafana.connect())
 
     def test_grafana_client_204_no_content_response(self):
         grafana = GrafanaApi.from_url()
         grafana.client.s.request = Mock(name="request")
         grafana.client.s.request.return_value = MockResponse(
             status_code=204,
         )
```

### Comparing `grafana-client-4.0.1/test/test_knowledge.py` & `grafana_client-4.1.0/test/test_knowledge.py`

 * *Files identical despite different names*

### Comparing `grafana-client-4.0.1/test/test_model.py` & `grafana_client-4.1.0/test/test_model.py`

 * *Files identical despite different names*

