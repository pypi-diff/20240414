# Comparing `tmp/zrb_extras-0.0.1.tar.gz` & `tmp/zrb_extras-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrb_extras-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "zrb_extras-0.0.2.tar", max compression
```

## Comparing `zrb_extras-0.0.1.tar` & `zrb_extras-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,210 @@
--rw-r--r--   0        0        0        6 2023-08-22 23:38:01.587139 zrb_extras-0.0.1/.gitignore
--rw-r--r--   0        0        0     1501 2023-08-22 23:38:01.607139 zrb_extras-0.0.1/README.md
--rw-r--r--   0        0        0      849 2023-08-23 05:08:42.385104 zrb_extras-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      165 2023-08-23 05:07:57.835126 zrb_extras-0.0.1/requirements.txt
--rw-r--r--   0        0        0       37 2023-08-22 23:38:01.597139 zrb_extras-0.0.1/src/zrb_extras/__init__.py
--rw-r--r--   0        0        0       37 2023-08-22 23:38:01.597139 zrb_extras-0.0.1/src/zrb_extras/__main__.py
--rw-r--r--   0        0        0       60 2023-08-22 23:38:01.597139 zrb_extras-0.0.1/src/zrb_extras/util.py
--rw-r--r--   0        0        0        0 2023-08-23 01:36:12.538560 zrb_extras-0.0.1/src/zrb_extras/zrb_init.py
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 zrb_extras-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1790 2024-04-13 23:26:35.443542 zrb_extras-0.0.2/README.md
+-rw-r--r--   0        0        0      771 2024-04-14 04:08:31.197276 zrb_extras-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-04-14 03:20:57.674901 zrb_extras-0.0.2/src/zrb_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 03:21:31.625909 zrb_extras-0.0.2/src/zrb_extras/__main__.py
+-rw-r--r--   0        0        0       53 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/__init__.py
+-rw-r--r--   0        0        0     1504 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/_input.py
+-rw-r--r--   0        0        0     3094 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/airflow.py
+-rw-r--r--   0        0        0      837 2024-04-14 03:32:50.073700 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_constant.py
+-rw-r--r--   0        0        0      847 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_env.py
+-rw-r--r--   0        0        0      208 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_group.py
+-rw-r--r--   0        0        0     1059 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/_input.py
+-rw-r--r--   0        0        0      334 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/activate-venv.sh
+-rw-r--r--   0        0        0      386 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-14 03:51:08.228048 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_env.py
+-rw-r--r--   0        0        0      240 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_group.py
+-rw-r--r--   0        0        0      289 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/_service_config.py
+-rw-r--r--   0        0        0     1157 2024-04-14 03:50:31.645663 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/init.py
+-rw-r--r--   0        0        0      963 2024-04-14 03:50:31.645663 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/remove.py
+-rw-r--r--   0        0        0     1685 2024-04-14 03:53:41.017291 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/start.py
+-rw-r--r--   0        0        0      948 2024-04-14 03:50:31.645663 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/container/stop.py
+-rw-r--r--   0        0        0     1335 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/deploy.py
+-rw-r--r--   0        0        0       24 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/deploy.sh
+-rw-r--r--   0        0        0     1161 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/destroy.py
+-rw-r--r--   0        0        0       29 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/destroy.sh
+-rw-r--r--   0        0        0      263 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_env.py
+-rw-r--r--   0        0        0      228 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_group.py
+-rw-r--r--   0        0        0      233 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/_input.py
+-rw-r--r--   0        0        0      902 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/build.py
+-rw-r--r--   0        0        0      903 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/image/push.py
+-rw-r--r--   0        0        0      126 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/_automate/snake_zrb_app_name/init-pulumi-stack.sh
+-rw-r--r--   0        0        0       36 2024-04-14 03:36:38.953378 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/.gitignore
+-rw-r--r--   0        0        0       64 2024-04-14 03:34:06.897550 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/config/airflow.cfg
+-rw-r--r--   0        0        0        0 2024-04-14 03:34:28.328202 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/dags/.gitkeep
+-rw-r--r--   0        0        0       12 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/.gitignore
+-rw-r--r--   0        0        0      137 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/Pulumi.yaml
+-rw-r--r--   0        0        0      437 2024-04-14 04:04:53.528320 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/__main__.py
+-rw-r--r--   0        0        0     1196 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/.helmignore
+-rw-r--r--   0        0        0      227 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/Chart.lock
+-rw-r--r--   0        0        0     2376 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/Chart.yaml
+-rw-r--r--   0        0        0      468 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/INSTALL
+-rw-r--r--   0        0        0    10850 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/LICENSE
+-rw-r--r--   0        0        0      863 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/NOTICE
+-rw-r--r--   0        0        0     2873 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/README.md
+-rw-r--r--   0        0        0    40813 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/RELEASE_NOTES.rst
+-rw-r--r--   0        0        0      333 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/.helmignore
+-rw-r--r--   0        0        0      226 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/Chart.lock
+-rw-r--r--   0        0        0     1076 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/Chart.yaml
+-rw-r--r--   0        0        0   126691 2024-04-14 03:58:36.497191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/README.md
+-rw-r--r--   0        0        0      342 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/.helmignore
+-rw-r--r--   0        0        0      531 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/Chart.yaml
+-rw-r--r--   0        0        0     7119 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/README.md
+-rw-r--r--   0        0        0     5480 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_affinities.tpl
+-rw-r--r--   0        0        0     7044 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_capabilities.tpl
+-rw-r--r--   0        0        0     1703 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_errors.tpl
+-rw-r--r--   0        0        0     4071 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_images.tpl
+-rw-r--r--   0        0        0     2431 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_ingress.tpl
+-rw-r--r--   0        0        0     2147 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_labels.tpl
+-rw-r--r--   0        0        0     2497 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_names.tpl
+-rw-r--r--   0        0        0     7500 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_secrets.tpl
+-rw-r--r--   0        0        0      698 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_storage.tpl
+-rw-r--r--   0        0        0     1385 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_tplvalues.tpl
+-rw-r--r--   0        0        0     2599 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_utils.tpl
+-rw-r--r--   0        0        0      650 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/_warnings.tpl
+-rw-r--r--   0        0        0     2644 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_cassandra.tpl
+-rw-r--r--   0        0        0     4059 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mariadb.tpl
+-rw-r--r--   0        0        0     4449 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mongodb.tpl
+-rw-r--r--   0        0        0     4003 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_mysql.tpl
+-rw-r--r--   0        0        0     5091 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_postgresql.tpl
+-rw-r--r--   0        0        0     3334 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_redis.tpl
+-rw-r--r--   0        0        0     2526 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/templates/validations/_validations.tpl
+-rw-r--r--   0        0        0      182 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/charts/common/values.yaml
+-rw-r--r--   0        0        0     7852 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/NOTES.txt
+-rw-r--r--   0        0        0    14792 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/_helpers.tpl
+-rw-r--r--   0        0        0     5485 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/cronjob.yaml
+-rw-r--r--   0        0        0     1617 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/backup/pvc.yaml
+-rw-r--r--   0        0        0      189 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/extra-list.yaml
+-rw-r--r--   0        0        0     1366 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/networkpolicy-egress.yaml
+-rw-r--r--   0        0        0     1047 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/configmap.yaml
+-rw-r--r--   0        0        0      818 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/extended-configmap.yaml
+-rw-r--r--   0        0        0      755 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/initialization-configmap.yaml
+-rw-r--r--   0        0        0      690 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-configmap.yaml
+-rw-r--r--   0        0        0     1418 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/metrics-svc.yaml
+-rw-r--r--   0        0        0     3727 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/networkpolicy.yaml
+-rw-r--r--   0        0        0     2314 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/servicemonitor.yaml
+-rw-r--r--   0        0        0    36405 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/statefulset.yaml
+-rw-r--r--   0        0        0     1827 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc-headless.yaml
+-rw-r--r--   0        0        0     2883 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/primary/svc.yaml
+-rw-r--r--   0        0        0     1043 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1069 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/psp.yaml
+-rw-r--r--   0        0        0      829 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/extended-configmap.yaml
+-rw-r--r--   0        0        0      734 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-configmap.yaml
+-rw-r--r--   0        0        0     1473 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/metrics-svc.yaml
+-rw-r--r--   0        0        0     2390 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/networkpolicy.yaml
+-rw-r--r--   0        0        0     2368 2024-04-14 03:58:36.507191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/servicemonitor.yaml
+-rw-r--r--   0        0        0    31450 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/statefulset.yaml
+-rw-r--r--   0        0        0     1910 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc-headless.yaml
+-rw-r--r--   0        0        0     3078 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/read/svc.yaml
+-rw-r--r--   0        0        0     1077 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/role.yaml
+-rw-r--r--   0        0        0      846 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/rolebinding.yaml
+-rw-r--r--   0        0        0     5145 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/secrets.yaml
+-rw-r--r--   0        0        0      837 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0     1963 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/templates/tls-secrets.yaml
+-rw-r--r--   0        0        0     4571 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.schema.json
+-rw-r--r--   0        0        0    74237 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/charts/postgresql/values.yaml
+-rw-r--r--   0        0        0     1201 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/README.md
+-rw-r--r--   0        0        0     3249 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/Dockerfile
+-rw-r--r--   0        0        0     2432 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer/build_and_push.sh
+-rw-r--r--   0        0        0     2243 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/Dockerfile
+-rw-r--r--   0        0        0     2466 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/dockerfiles/pgbouncer-exporter/build_and_push.sh
+-rw-r--r--   0        0        0     6199 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/pod-template-file.kubernetes-helm-yaml
+-rw-r--r--   0        0        0     2722 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/files/statsd-mappings.yml
+-rw-r--r--   0        0        0     1084 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/37197.significant.rst
+-rw-r--r--   0        0        0     1409 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/newsfragments/config.toml
+-rw-r--r--   0        0        0       83 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/reproducible_build.yaml
+-rw-r--r--   0        0        0     8276 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/NOTES.txt
+-rw-r--r--   0        0        0    40339 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/_helpers.yaml
+-rw-r--r--   0        0        0     2683 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/check-values.yaml
+-rw-r--r--   0        0        0     4982 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-cronjob.yaml
+-rw-r--r--   0        0        0     1582 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/cleanup/cleanup-serviceaccount.yaml
+-rw-r--r--   0        0        0     2531 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/configmap.yaml
+-rw-r--r--   0        0        0     1903 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/extra-configmaps.yaml
+-rw-r--r--   0        0        0     1753 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/statsd-configmap.yaml
+-rw-r--r--   0        0        0     1548 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/configmaps/webserver-configmap.yaml
+-rw-r--r--   0        0        0    13231 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-deployment.yaml
+-rw-r--r--   0        0        0     1633 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dag-processor/dag-processor-serviceaccount.yaml
+-rw-r--r--   0        0        0     1888 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/dags-persistent-volume-claim.yaml
+-rw-r--r--   0        0        0     7836 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-deployment.yaml
+-rw-r--r--   0        0        0     3276 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-ingress.yaml
+-rw-r--r--   0        0        0     2098 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-networkpolicy.yaml
+-rw-r--r--   0        0        0     2161 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-service.yaml
+-rw-r--r--   0        0        0     1700 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/flower/flower-serviceaccount.yaml
+-rw-r--r--   0        0        0     1692 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job-serviceaccount.yaml
+-rw-r--r--   0        0        0     6153 2024-04-14 03:58:36.517191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/create-user-job.yaml
+-rw-r--r--   0        0        0     1697 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job-serviceaccount.yaml
+-rw-r--r--   0        0        0     6314 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/jobs/migrate-database-job.yaml
+-rw-r--r--   0        0        0     1312 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/limitrange.yaml
+-rw-r--r--   0        0        0     1854 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/logs-persistent-volume-claim.yaml
+-rw-r--r--   0        0        0     9469 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-deployment.yaml
+-rw-r--r--   0        0        0     2818 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-networkpolicy.yaml
+-rw-r--r--   0        0        0     1537 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-poddisruptionbudget.yaml
+-rw-r--r--   0        0        0     1836 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-service.yaml
+-rw-r--r--   0        0        0     1554 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/pgbouncer/pgbouncer-serviceaccount.yaml
+-rw-r--r--   0        0        0     1400 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/priorityclasses/priority-classes.yaml
+-rw-r--r--   0        0        0     1394 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-role.yaml
+-rw-r--r--   0        0        0     1558 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-cleanup-rolebinding.yaml
+-rw-r--r--   0        0        0     2113 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-role.yaml
+-rw-r--r--   0        0        0     2657 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-launcher-rolebinding.yaml
+-rw-r--r--   0        0        0     1935 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-role.yaml
+-rw-r--r--   0        0        0     2420 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/pod-log-reader-rolebinding.yaml
+-rw-r--r--   0        0        0     3489 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/rbac/security-context-constraint-rolebinding.yaml
+-rw-r--r--   0        0        0     2058 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-networkpolicy.yaml
+-rw-r--r--   0        0        0     1595 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-service.yaml
+-rw-r--r--   0        0        0     1619 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-serviceaccount.yaml
+-rw-r--r--   0        0        0     5159 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/redis/redis-statefulset.yaml
+-rw-r--r--   0        0        0     1322 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/resourcequota.yaml
+-rw-r--r--   0        0        0    16802 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-deployment.yaml
+-rw-r--r--   0        0        0     1892 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-networkpolicy.yaml
+-rw-r--r--   0        0        0     1619 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-poddisruptionbudget.yaml
+-rw-r--r--   0        0        0     1715 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-service.yaml
+-rw-r--r--   0        0        0     1714 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/scheduler/scheduler-serviceaccount.yaml
+-rw-r--r--   0        0        0     1765 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/elasticsearch-secret.yaml
+-rw-r--r--   0        0        0     2083 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/extra-secrets.yaml
+-rw-r--r--   0        0        0     1515 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/fernetkey-secret.yaml
+-rw-r--r--   0        0        0     1368 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/flower-secret.yaml
+-rw-r--r--   0        0        0     1332 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/kerberos-keytab-secret.yaml
+-rw-r--r--   0        0        0     3280 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/metadata-connection-secret.yaml
+-rw-r--r--   0        0        0     1600 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-certificates-secret.yaml
+-rw-r--r--   0        0        0     1425 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-config-secret.yaml
+-rw-r--r--   0        0        0     1712 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/pgbouncer-stats-secret.yaml
+-rw-r--r--   0        0        0     3084 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/redis-secrets.yaml
+-rw-r--r--   0        0        0     1348 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/registry-secret.yaml
+-rw-r--r--   0        0        0     2489 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/result-backend-connection-secret.yaml
+-rw-r--r--   0        0        0     1494 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/secrets/webserver-secret-key-secret.yaml
+-rw-r--r--   0        0        0     5423 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-deployment.yaml
+-rw-r--r--   0        0        0     1880 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-networkpolicy.yaml
+-rw-r--r--   0        0        0     1914 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-service.yaml
+-rw-r--r--   0        0        0     1533 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/statsd/statsd-serviceaccount.yaml
+-rw-r--r--   0        0        0    15260 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-deployment.yaml
+-rw-r--r--   0        0        0     2266 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-kedaautoscaler.yaml
+-rw-r--r--   0        0        0     1981 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-networkpolicy.yaml
+-rw-r--r--   0        0        0     1760 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-service.yaml
+-rw-r--r--   0        0        0     1690 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/triggerer/triggerer-serviceaccount.yaml
+-rw-r--r--   0        0        0    14983 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-deployment.yaml
+-rw-r--r--   0        0        0     3760 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-ingress.yaml
+-rw-r--r--   0        0        0     2007 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-networkpolicy.yaml
+-rw-r--r--   0        0        0     1619 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-poddisruptionbudget.yaml
+-rw-r--r--   0        0        0     2081 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-service.yaml
+-rw-r--r--   0        0        0     1634 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/webserver/webserver-serviceaccount.yaml
+-rw-r--r--   0        0        0    22362 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-deployment.yaml
+-rw-r--r--   0        0        0     2015 2024-04-14 03:58:36.527191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-hpa.yaml
+-rw-r--r--   0        0        0     2674 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-kedaautoscaler.yaml
+-rw-r--r--   0        0        0     1865 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-networkpolicy.yaml
+-rw-r--r--   0        0        0     1656 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-service.yaml
+-rw-r--r--   0        0        0     1761 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/templates/workers/worker-serviceaccount.yaml
+-rw-r--r--   0        0        0   534941 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.schema.json
+-rw-r--r--   0        0        0    77957 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values.yaml
+-rw-r--r--   0        0        0     3242 2024-04-14 03:58:36.537191 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/helm-charts/airflow/values_schema.schema.json
+-rw-r--r--   0        0        0       74 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/state/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/deployment/template.env
+-rw-r--r--   0        0        0       68 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/docker-compose.env
+-rw-r--r--   0        0        0     9762 2024-04-14 03:53:41.017291 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/docker-compose.yml
+-rw-r--r--   0        0        0       22 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/.dockerignore
+-rw-r--r--   0        0        0       23 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/.gitignore
+-rw-r--r--   0        0        0      101 2024-04-14 03:28:18.708296 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/Dockerfile
+-rw-r--r--   0        0        0       57 2024-04-14 03:33:11.668826 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/requirements.txt
+-rw-r--r--   0        0        0       87 2024-04-14 03:17:30.590718 zrb_extras-0.0.2/src/zrb_extras/airflow/template/src/kebab-zrb-app-name/images/airflow/template.env
+-rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 zrb_extras-0.0.2/PKG-INFO
```

### Comparing `zrb_extras-0.0.1/README.md` & `zrb_extras-0.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 # Zrb extras
 
 zrb-extras is a [pypi](https://pypi.org) package.
 
-You can install zrb-extras by invoking:
+You can install zrb-extras by invoking the following command:
 
-```
+```bash
 pip install zrb-extras
 ```
 
+Once zrb-extras is installed, you can then run it by invoking the following command:
+
+```bash
+zrb-extras
+```
+
+You can also import `zrb-extras` into your Python program:
+
+```python
+from zrb_extras import hello
+
+print(hello())
+```
+
+
 # For maintainers
 
 ## Publish to pypi
 
 To publish zrb-extras, you need to have a `Pypi` account:
 
 - Log in or register to [https://pypi.org/](https://pypi.org/)
@@ -65,15 +80,15 @@
     "Jinja2==3.1.2",
     "jsons==1.6.3"
 ]
 ```
 
 ## Adding script
 
-To make zrb-package-name executable, you can edit the following section in `pyproject.toml`:
+To make zrb-extras executable, you can edit the following section in `pyproject.toml`:
 
 ```toml
 [project-scripts]
-zrb-extras = "zrb-extras.__main__:hello"
+zrb-extras-hello = "zrb_extras.__main__:hello"
 ```
 
-This will look for `hello` callable inside of your `__main__.py` file
+Now, whenever you run `zrb-extras-hello`, the `main` function on your `__main__.py` will be executed.
```

### Comparing `zrb_extras-0.0.1/PKG-INFO` & `zrb_extras-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 Metadata-Version: 2.1
 Name: zrb-extras
-Version: 0.0.1
-Summary: Collection of Zrb tasks and utilities
-Author-email: Go Frendi Gunawan <gofrendiasgard@gmail.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
+Version: 0.0.2
+Summary: Collection of Zrb additional utilities
+Home-page: https://github.com/goFrendiAsgard/zrb-extras
+License: AGPL-3.0-or-later
+Author: Go Frendi Gunawan
+Author-email: gofrendiasgard@gmail.com
+Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Dist: zrb>=0.0.89
-Project-URL: Bug Tracker, https://github.com/state-alchemists/zrb-extras/issues
-Project-URL: Homepage, https://github.com/state-alchemists/zrb-extras
-Provides-Extra: dev
-Provides-Extra: test
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: zrb (>=0.11.2)
+Project-URL: Documentation, https://github.com/goFrendiAsgard/zrb-extras
+Project-URL: Repository, https://github.com/goFrendiAsgard/zrb-extras
+Description-Content-Type: text/markdown
 
 # Zrb extras
 
 zrb-extras is a [pypi](https://pypi.org) package.
 
-You can install zrb-extras by invoking:
+You can install zrb-extras by invoking the following command:
 
-```
+```bash
 pip install zrb-extras
 ```
 
+Once zrb-extras is installed, you can then run it by invoking the following command:
+
+```bash
+zrb-extras
+```
+
+You can also import `zrb-extras` into your Python program:
+
+```python
+from zrb_extras import hello
+
+print(hello())
+```
+
+
 # For maintainers
 
 ## Publish to pypi
 
 To publish zrb-extras, you need to have a `Pypi` account:
 
 - Log in or register to [https://pypi.org/](https://pypi.org/)
@@ -81,16 +99,16 @@
     "Jinja2==3.1.2",
     "jsons==1.6.3"
 ]
 ```
 
 ## Adding script
 
-To make zrb-package-name executable, you can edit the following section in `pyproject.toml`:
+To make zrb-extras executable, you can edit the following section in `pyproject.toml`:
 
 ```toml
 [project-scripts]
-zrb-extras = "zrb-extras.__main__:hello"
+zrb-extras-hello = "zrb_extras.__main__:hello"
 ```
 
-This will look for `hello` callable inside of your `__main__.py` file
+Now, whenever you run `zrb-extras-hello`, the `main` function on your `__main__.py` will be executed.
```

