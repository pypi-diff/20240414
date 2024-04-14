# Comparing `tmp/prodsys-0.4.4.tar.gz` & `tmp/prodsys-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodsys-0.4.4.tar", max compression
+gzip compressed data, was "prodsys-0.5.0.tar", max compression
```

## Comparing `prodsys-0.4.4.tar` & `prodsys-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.4.4/LICENSE
--rw-r--r--   0        0        0      405 2024-02-27 20:59:44.879610 prodsys-0.4.4/prodsys/__init__.py
--rw-r--r--   0        0        0     1289 2024-01-07 23:00:16.870495 prodsys-0.4.4/prodsys/adapters/__init__.py
--rw-r--r--   0        0        0    50242 2024-02-08 21:28:59.058794 prodsys-0.4.4/prodsys/adapters/adapter.py
--rw-r--r--   0        0        0     8314 2024-02-27 20:59:44.884128 prodsys-0.4.4/prodsys/adapters/json_adapter.py
--rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.4.4/prodsys/conf/__init__.py
--rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.4.4/prodsys/conf/logging.ini
--rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.4.4/prodsys/conf/logging_config.py
--rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.4.4/prodsys/control/__init__.py
--rw-r--r--   0        0        0     9028 2023-12-24 15:55:37.172880 prodsys-0.4.4/prodsys/control/routing_control_env.py
--rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.4.4/prodsys/control/sequencing_control_env.py
--rw-r--r--   0        0        0     2138 2024-02-08 21:28:59.073027 prodsys-0.4.4/prodsys/express/__init__.py
--rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.4.4/prodsys/express/core.py
--rw-r--r--   0        0        0     6525 2024-02-08 21:28:59.073027 prodsys-0.4.4/prodsys/express/process.py
--rw-r--r--   0        0        0     2435 2024-02-08 21:28:59.073027 prodsys-0.4.4/prodsys/express/product.py
--rw-r--r--   0        0        0     6508 2024-02-08 21:28:59.073027 prodsys-0.4.4/prodsys/express/production_system.py
--rw-r--r--   0        0        0     8275 2024-02-08 21:28:59.073027 prodsys-0.4.4/prodsys/express/resources.py
--rw-r--r--   0        0        0     2558 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/express/sink.py
--rw-r--r--   0        0        0     3454 2024-01-07 23:00:16.874004 prodsys-0.4.4/prodsys/express/source.py
--rw-r--r--   0        0        0     7554 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/express/state.py
--rw-r--r--   0        0        0     4895 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/express/time_model.py
--rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/factories/__init__.py
--rw-r--r--   0        0        0     3439 2024-02-08 21:28:59.084884 prodsys-0.4.4/prodsys/factories/process_factory.py
--rw-r--r--   0        0        0     6358 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/factories/product_factory.py
--rw-r--r--   0        0        0     1992 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/factories/queue_factory.py
--rw-r--r--   0        0        0    10091 2024-02-08 21:28:59.089825 prodsys-0.4.4/prodsys/factories/resource_factory.py
--rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/factories/sink_factory.py
--rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.4.4/prodsys/factories/source_factory.py
--rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/factories/state_factory.py
--rw-r--r--   0        0        0     2045 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/factories/time_model_factory.py
--rw-r--r--   0        0        0     1436 2024-02-08 21:28:59.093974 prodsys-0.4.4/prodsys/models/__init__.py
--rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/models/core_asset.py
--rw-r--r--   0        0        0     2971 2024-02-27 19:26:17.985971 prodsys-0.4.4/prodsys/models/performance_data.py
--rw-r--r--   0        0        0     9369 2023-10-11 11:05:22.089564 prodsys-0.4.4/prodsys/models/performance_indicators.py
--rw-r--r--   0        0        0     8490 2024-02-08 21:28:59.093974 prodsys-0.4.4/prodsys/models/processes_data.py
--rw-r--r--   0        0        0     4481 2024-02-27 19:26:17.989823 prodsys-0.4.4/prodsys/models/product_data.py
--rw-r--r--   0        0        0     1680 2024-02-27 19:26:17.992220 prodsys-0.4.4/prodsys/models/queue_data.py
--rw-r--r--   0        0        0     8849 2024-02-08 21:28:59.093974 prodsys-0.4.4/prodsys/models/resource_data.py
--rw-r--r--   0        0        0    10615 2024-02-27 19:26:17.994121 prodsys-0.4.4/prodsys/models/scenario_data.py
--rw-r--r--   0        0        0     1481 2023-10-11 11:05:22.105207 prodsys-0.4.4/prodsys/models/sink_data.py
--rw-r--r--   0        0        0     2280 2024-01-07 23:00:16.890715 prodsys-0.4.4/prodsys/models/source_data.py
--rw-r--r--   0        0        0     9272 2023-10-11 11:05:22.105207 prodsys-0.4.4/prodsys/models/state_data.py
--rw-r--r--   0        0        0     5486 2023-10-11 11:05:22.105207 prodsys-0.4.4/prodsys/models/time_model_data.py
--rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.4.4/prodsys/optimization/__init__.py
--rw-r--r--   0        0        0    12399 2024-02-27 20:59:44.884128 prodsys-0.4.4/prodsys/optimization/evolutionary_algorithm.py
--rw-r--r--   0        0        0    28178 2024-02-27 20:59:44.887029 prodsys-0.4.4/prodsys/optimization/math_opt.py
--rw-r--r--   0        0        0     4640 2023-10-11 11:05:22.105207 prodsys-0.4.4/prodsys/optimization/optimization_analysis.py
--rw-r--r--   0        0        0    46085 2024-02-27 20:59:44.890000 prodsys-0.4.4/prodsys/optimization/optimization_util.py
--rw-r--r--   0        0        0     9324 2024-02-27 20:59:44.890000 prodsys-0.4.4/prodsys/optimization/simulated_annealing.py
--rw-r--r--   0        0        0    11576 2024-02-27 20:59:44.893146 prodsys-0.4.4/prodsys/optimization/tabu_search.py
--rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.4.4/prodsys/simulation/__init__.py
--rw-r--r--   0        0        0    26523 2024-02-27 20:59:44.895053 prodsys-0.4.4/prodsys/simulation/control.py
--rw-r--r--   0        0        0     6855 2023-10-11 11:05:22.105207 prodsys-0.4.4/prodsys/simulation/logger.py
--rw-r--r--   0        0        0     3763 2024-01-07 23:00:16.907148 prodsys-0.4.4/prodsys/simulation/observer.py
--rw-r--r--   0        0        0     9601 2024-02-08 21:28:59.106239 prodsys-0.4.4/prodsys/simulation/proces_models.py
--rw-r--r--   0        0        0     9097 2024-02-27 19:26:18.008307 prodsys-0.4.4/prodsys/simulation/process.py
--rw-r--r--   0        0        0    11882 2024-02-08 21:28:59.108394 prodsys-0.4.4/prodsys/simulation/product.py
--rw-r--r--   0        0        0     4004 2024-02-08 21:28:59.116934 prodsys-0.4.4/prodsys/simulation/request.py
--rw-r--r--   0        0        0    17261 2024-02-08 21:28:59.118426 prodsys-0.4.4/prodsys/simulation/resources.py
--rw-r--r--   0        0        0     9393 2024-02-08 21:28:59.122388 prodsys-0.4.4/prodsys/simulation/router.py
--rw-r--r--   0        0        0     3199 2023-10-11 11:05:22.120833 prodsys-0.4.4/prodsys/simulation/sim.py
--rw-r--r--   0        0        0     1785 2023-10-11 11:05:22.120833 prodsys-0.4.4/prodsys/simulation/sink.py
--rw-r--r--   0        0        0     3335 2024-01-07 23:00:16.918251 prodsys-0.4.4/prodsys/simulation/source.py
--rw-r--r--   0        0        0    29184 2024-02-08 21:28:59.124487 prodsys-0.4.4/prodsys/simulation/state.py
--rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.4.4/prodsys/simulation/store.py
--rw-r--r--   0        0        0     7193 2024-02-08 21:28:59.124487 prodsys-0.4.4/prodsys/simulation/time_model.py
--rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.4.4/prodsys/util/__init__.py
--rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.4.4/prodsys/util/kpi_visualization.py
--rw-r--r--   0        0        0    30298 2023-12-24 15:40:41.082915 prodsys-0.4.4/prodsys/util/post_processing.py
--rw-r--r--   0        0        0    12118 2024-02-08 21:28:59.124487 prodsys-0.4.4/prodsys/util/runner.py
--rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.4.4/prodsys/util/statistical_functions.py
--rw-r--r--   0        0        0     4260 2023-10-11 11:05:22.120833 prodsys-0.4.4/prodsys/util/util.py
--rw-r--r--   0        0        0     1313 2024-02-27 20:59:44.904632 prodsys-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     6238 2023-10-11 11:05:21.946526 prodsys-0.4.4/README.md
--rw-r--r--   0        0        0     8509 1970-01-01 00:00:00.000000 prodsys-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-10-11 11:05:21.946526 prodsys-0.5.0/LICENSE
+-rw-r--r--   0        0        0      405 2024-04-14 17:14:53.846311 prodsys-0.5.0/prodsys/__init__.py
+-rw-r--r--   0        0        0     1289 2024-01-07 23:00:16.870495 prodsys-0.5.0/prodsys/adapters/__init__.py
+-rw-r--r--   0        0        0    51413 2024-04-14 17:14:53.846311 prodsys-0.5.0/prodsys/adapters/adapter.py
+-rw-r--r--   0        0        0     8314 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/adapters/json_adapter.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:00:16.874004 prodsys-0.5.0/prodsys/conf/__init__.py
+-rw-r--r--   0        0        0     2487 2024-01-07 23:00:16.874004 prodsys-0.5.0/prodsys/conf/logging.ini
+-rw-r--r--   0        0        0     1155 2024-01-07 23:00:16.874004 prodsys-0.5.0/prodsys/conf/logging_config.py
+-rw-r--r--   0        0        0      148 2023-10-11 11:05:22.073479 prodsys-0.5.0/prodsys/control/__init__.py
+-rw-r--r--   0        0        0     9028 2023-12-24 15:55:37.172880 prodsys-0.5.0/prodsys/control/routing_control_env.py
+-rw-r--r--   0        0        0     8489 2023-10-11 11:05:22.073479 prodsys-0.5.0/prodsys/control/sequencing_control_env.py
+-rw-r--r--   0        0        0     2138 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/express/__init__.py
+-rw-r--r--   0        0        0      603 2023-10-11 11:05:22.073479 prodsys-0.5.0/prodsys/express/core.py
+-rw-r--r--   0        0        0     6525 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/express/process.py
+-rw-r--r--   0        0        0     2435 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/express/product.py
+-rw-r--r--   0        0        0     6508 2024-04-07 17:13:56.244883 prodsys-0.5.0/prodsys/express/production_system.py
+-rw-r--r--   0        0        0     8275 2024-04-07 17:13:56.260662 prodsys-0.5.0/prodsys/express/resources.py
+-rw-r--r--   0        0        0     2558 2024-02-27 21:06:20.429295 prodsys-0.5.0/prodsys/express/sink.py
+-rw-r--r--   0        0        0     3454 2024-01-07 23:00:16.874004 prodsys-0.5.0/prodsys/express/source.py
+-rw-r--r--   0        0        0     7554 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/express/state.py
+-rw-r--r--   0        0        0     4895 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/express/time_model.py
+-rw-r--r--   0        0        0      913 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/factories/__init__.py
+-rw-r--r--   0        0        0     3439 2024-04-07 17:13:56.261200 prodsys-0.5.0/prodsys/factories/process_factory.py
+-rw-r--r--   0        0        0     6358 2024-03-10 14:05:36.923357 prodsys-0.5.0/prodsys/factories/product_factory.py
+-rw-r--r--   0        0        0     1992 2024-03-10 14:05:36.923357 prodsys-0.5.0/prodsys/factories/queue_factory.py
+-rw-r--r--   0        0        0    10419 2024-04-12 11:17:17.974120 prodsys-0.5.0/prodsys/factories/resource_factory.py
+-rw-r--r--   0        0        0     3268 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/factories/sink_factory.py
+-rw-r--r--   0        0        0     5089 2024-01-07 23:00:16.890715 prodsys-0.5.0/prodsys/factories/source_factory.py
+-rw-r--r--   0        0        0     2856 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/factories/state_factory.py
+-rw-r--r--   0        0        0     2045 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/factories/time_model_factory.py
+-rw-r--r--   0        0        0     1436 2024-04-07 17:13:56.263212 prodsys-0.5.0/prodsys/models/__init__.py
+-rw-r--r--   0        0        0      541 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/models/core_asset.py
+-rw-r--r--   0        0        0     2971 2024-02-27 19:26:17.985971 prodsys-0.5.0/prodsys/models/performance_data.py
+-rw-r--r--   0        0        0     9369 2023-10-11 11:05:22.089564 prodsys-0.5.0/prodsys/models/performance_indicators.py
+-rw-r--r--   0        0        0    11648 2024-04-14 17:14:53.855074 prodsys-0.5.0/prodsys/models/processes_data.py
+-rw-r--r--   0        0        0     6357 2024-04-14 17:14:53.857017 prodsys-0.5.0/prodsys/models/product_data.py
+-rw-r--r--   0        0        0     1931 2024-04-14 17:14:53.857017 prodsys-0.5.0/prodsys/models/queue_data.py
+-rw-r--r--   0        0        0    12337 2024-04-14 17:14:53.862626 prodsys-0.5.0/prodsys/models/resource_data.py
+-rw-r--r--   0        0        0    10730 2024-04-12 11:17:17.974120 prodsys-0.5.0/prodsys/models/scenario_data.py
+-rw-r--r--   0        0        0     2846 2024-04-14 17:14:53.863598 prodsys-0.5.0/prodsys/models/sink_data.py
+-rw-r--r--   0        0        0     4059 2024-04-14 17:14:53.865574 prodsys-0.5.0/prodsys/models/source_data.py
+-rw-r--r--   0        0        0    13852 2024-04-14 17:14:53.865574 prodsys-0.5.0/prodsys/models/state_data.py
+-rw-r--r--   0        0        0     6642 2024-04-14 17:14:53.865574 prodsys-0.5.0/prodsys/models/time_model_data.py
+-rw-r--r--   0        0        0     2870 2023-10-11 11:05:22.105207 prodsys-0.5.0/prodsys/optimization/__init__.py
+-rw-r--r--   0        0        0    12476 2024-04-14 17:14:53.871089 prodsys-0.5.0/prodsys/optimization/evolutionary_algorithm.py
+-rw-r--r--   0        0        0    28223 2024-04-14 17:14:53.874200 prodsys-0.5.0/prodsys/optimization/math_opt.py
+-rw-r--r--   0        0        0     4640 2023-10-11 11:05:22.105207 prodsys-0.5.0/prodsys/optimization/optimization_analysis.py
+-rw-r--r--   0        0        0    46564 2024-04-14 17:14:53.874200 prodsys-0.5.0/prodsys/optimization/optimization_util.py
+-rw-r--r--   0        0        0     9396 2024-04-14 17:14:53.879309 prodsys-0.5.0/prodsys/optimization/simulated_annealing.py
+-rw-r--r--   0        0        0    11646 2024-04-14 17:14:53.880630 prodsys-0.5.0/prodsys/optimization/tabu_search.py
+-rw-r--r--   0        0        0     1704 2023-10-11 11:05:22.105207 prodsys-0.5.0/prodsys/simulation/__init__.py
+-rw-r--r--   0        0        0    27915 2024-04-12 11:17:17.986645 prodsys-0.5.0/prodsys/simulation/control.py
+-rw-r--r--   0        0        0     6855 2023-10-11 11:05:22.105207 prodsys-0.5.0/prodsys/simulation/logger.py
+-rw-r--r--   0        0        0     3763 2024-01-07 23:00:16.907148 prodsys-0.5.0/prodsys/simulation/observer.py
+-rw-r--r--   0        0        0     9601 2024-04-07 17:13:56.267724 prodsys-0.5.0/prodsys/simulation/proces_models.py
+-rw-r--r--   0        0        0     9097 2024-04-07 17:13:56.267724 prodsys-0.5.0/prodsys/simulation/process.py
+-rw-r--r--   0        0        0    11882 2024-04-07 17:13:56.267724 prodsys-0.5.0/prodsys/simulation/product.py
+-rw-r--r--   0        0        0     4004 2024-04-07 17:13:56.267724 prodsys-0.5.0/prodsys/simulation/request.py
+-rw-r--r--   0        0        0    17837 2024-04-12 11:17:17.986645 prodsys-0.5.0/prodsys/simulation/resources.py
+-rw-r--r--   0        0        0     9574 2024-04-12 11:17:17.989996 prodsys-0.5.0/prodsys/simulation/router.py
+-rw-r--r--   0        0        0     3199 2023-10-11 11:05:22.120833 prodsys-0.5.0/prodsys/simulation/sim.py
+-rw-r--r--   0        0        0     2260 2024-04-12 11:17:17.990877 prodsys-0.5.0/prodsys/simulation/sink.py
+-rw-r--r--   0        0        0     3809 2024-04-12 11:17:17.990877 prodsys-0.5.0/prodsys/simulation/source.py
+-rw-r--r--   0        0        0    29184 2024-04-07 17:13:56.277897 prodsys-0.5.0/prodsys/simulation/state.py
+-rw-r--r--   0        0        0     2232 2024-01-07 23:00:16.919358 prodsys-0.5.0/prodsys/simulation/store.py
+-rw-r--r--   0        0        0     7193 2024-04-07 17:13:56.277897 prodsys-0.5.0/prodsys/simulation/time_model.py
+-rw-r--r--   0        0        0       61 2023-10-11 11:05:22.120833 prodsys-0.5.0/prodsys/util/__init__.py
+-rw-r--r--   0        0        0     8056 2023-11-06 17:14:55.559034 prodsys-0.5.0/prodsys/util/kpi_visualization.py
+-rw-r--r--   0        0        0    30298 2023-12-24 15:40:41.082915 prodsys-0.5.0/prodsys/util/post_processing.py
+-rw-r--r--   0        0        0    12118 2024-04-07 17:13:56.277897 prodsys-0.5.0/prodsys/util/runner.py
+-rw-r--r--   0        0        0     2657 2023-12-24 16:10:02.245387 prodsys-0.5.0/prodsys/util/statistical_functions.py
+-rw-r--r--   0        0        0     4260 2023-10-11 11:05:22.120833 prodsys-0.5.0/prodsys/util/util.py
+-rw-r--r--   0        0        0     1313 2024-04-14 17:14:53.888155 prodsys-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6238 2023-10-11 11:05:21.946526 prodsys-0.5.0/README.md
+-rw-r--r--   0        0        0     8509 1970-01-01 00:00:00.000000 prodsys-0.5.0/PKG-INFO
```

### Comparing `prodsys-0.4.4/LICENSE` & `prodsys-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/adapters/__init__.py` & `prodsys-0.5.0/prodsys/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/adapters/adapter.py` & `prodsys-0.5.0/prodsys/adapters/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from hashlib import md5
 import warnings
 from typing import List, Any, Set, Optional, Tuple, Union
 from pydantic import BaseModel, validator, ValidationError
 
 import logging
 logger = logging.getLogger(__name__)
 
@@ -290,15 +291,15 @@
     queue_data: List[queue_data.QueueData] = []
     resource_data: List[resource_data.RESOURCE_DATA_UNION] = []
     product_data: List[product_data.ProductData] = []
     sink_data: List[sink_data.SinkData] = []
     source_data: List[source_data.SourceData] = []
     scenario_data: Optional[scenario_data.ScenarioData] = None
 
-    
+
     valid_configuration: bool = True
     reconfiguration_cost: float = 0
 
     class Config:
         validate = True
         validate_assignment = True
         schema_extra = {
@@ -668,14 +669,36 @@
                         "output_queues": ["SourceQueue"],
                     },
                 ],
                 "scenario_data": None,
             }
         }
 
+    def hash(self) -> str:
+        """
+        Generates a hash of the adapter based on the hash of all contained entities. Only information describing the physical structure and functionality of the production system is considered. Can be used to compare two production systems of adapters for functional equality.
+
+        Returns:
+            str: Hash of the adapter
+        """
+        return md5(
+            ("".join(
+                [
+                *sorted([time_model.hash() for time_model in self.time_model_data]),
+                *sorted([state.hash(self) for state in self.state_data]),
+                *sorted([process.hash(self) for process in self.process_data]),
+                *sorted([res.hash(self) for res in self.resource_data]),
+                *sorted([queue.hash() for queue in self.queue_data]),
+                *sorted([product.hash(self) for product in self.product_data]),
+                *sorted([sink.hash(self) for sink in self.sink_data]),
+                *sorted([source.hash(self) for source in self.source_data])
+                ]
+            )).encode("utf-8")
+            ).hexdigest()
+
     @validator("state_data", each_item=True)
     def check_states(cls, state: state_data.STATE_DATA_UNION, values):
         time_models = get_set_of_IDs(values["time_model_data"])
         if state.time_model_id not in time_models:
             raise ValueError(
                 f"The time model {state.time_model_id} of state {state.ID} is not a valid time model of {time_models}."
             )
```

### Comparing `prodsys-0.4.4/prodsys/adapters/json_adapter.py` & `prodsys-0.5.0/prodsys/adapters/json_adapter.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/conf/logging.ini` & `prodsys-0.5.0/prodsys/conf/logging.ini`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/conf/logging_config.py` & `prodsys-0.5.0/prodsys/conf/logging_config.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/control/routing_control_env.py` & `prodsys-0.5.0/prodsys/control/routing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/control/sequencing_control_env.py` & `prodsys-0.5.0/prodsys/control/sequencing_control_env.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/__init__.py` & `prodsys-0.5.0/prodsys/express/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/core.py` & `prodsys-0.5.0/prodsys/express/core.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/process.py` & `prodsys-0.5.0/prodsys/express/process.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/product.py` & `prodsys-0.5.0/prodsys/express/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/production_system.py` & `prodsys-0.5.0/prodsys/express/production_system.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/resources.py` & `prodsys-0.5.0/prodsys/express/resources.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/sink.py` & `prodsys-0.5.0/prodsys/express/sink.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/source.py` & `prodsys-0.5.0/prodsys/express/source.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/state.py` & `prodsys-0.5.0/prodsys/express/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/express/time_model.py` & `prodsys-0.5.0/prodsys/express/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/factories/__init__.py` & `prodsys-0.5.0/prodsys/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/factories/process_factory.py` & `prodsys-0.5.0/prodsys/factories/process_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/factories/product_factory.py` & `prodsys-0.5.0/prodsys/factories/product_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/factories/queue_factory.py` & `prodsys-0.5.0/prodsys/factories/queue_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/factories/resource_factory.py` & `prodsys-0.5.0/prodsys/factories/resource_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 }
 
 CONTROL_POLICY_DICT: Dict = {
     ResourceControlPolicy.FIFO: control.FIFO_control_policy,
     ResourceControlPolicy.LIFO: control.LIFO_control_policy,
     ResourceControlPolicy.SPT: control.SPT_control_policy,
     TransportControlPolicy.SPT_transport: control.SPT_transport_control_policy,
+    TransportControlPolicy.NEAREST_ORIGIN_AND_LONGEST_TARGET_QUEUES_TRANSPORT : control.nearest_origin_and_longest_target_queues_transport_control_policy,
+    TransportControlPolicy.NEAREST_ORIGIN_AND_SHORTEST_TARGET_INPUT_QUEUES_TRANSPORT : control.nearest_origin_and_shortest_target_input_queues_transport_control_policy,
+
 }
 
 
 def register_states(
     resource: resources.Resource,
     states: List[state.STATE_UNION],
     _env: sim.Environment,
```

### Comparing `prodsys-0.4.4/prodsys/factories/sink_factory.py` & `prodsys-0.5.0/prodsys/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/factories/source_factory.py` & `prodsys-0.5.0/prodsys/factories/source_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/factories/state_factory.py` & `prodsys-0.5.0/prodsys/factories/state_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/factories/time_model_factory.py` & `prodsys-0.5.0/prodsys/factories/time_model_factory.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/models/__init__.py` & `prodsys-0.5.0/prodsys/models/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/models/core_asset.py` & `prodsys-0.5.0/prodsys/models/core_asset.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/models/performance_data.py` & `prodsys-0.5.0/prodsys/models/performance_data.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/models/performance_indicators.py` & `prodsys-0.5.0/prodsys/models/performance_indicators.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/models/processes_data.py` & `prodsys-0.5.0/prodsys/simulation/proces_models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,247 +1,253 @@
-"""
-The `processes_data` module contains the `prodsys.models` classes to represent the processes that can 
-be performed on products by resources.
-
-The following processes are possible:
-- `ProductionProcessData`: A process that can be performed on a product by a production resource.
-- `CapabilityProcessData`: A process that can be performed on a product by a resource, based on the capability of the resource.
-- `TransportProcessData`: A process that can be performed on a product by a transport resource.
-"""
-
 from __future__ import annotations
 
-from enum import Enum
-from typing import Literal, Union, Optional, List
+from abc import ABC, abstractmethod
+from typing import List, Optional, Dict
+import random
+from pydantic import BaseModel, Field
 
-from prodsys.models.core_asset import CoreAsset
+from prodsys.simulation import process
+from prodsys.util.util import flatten
 
 
-class ProcessTypeEnum(str, Enum):
+class ProcessModel(ABC, BaseModel):
     """
-    Enum that represents the different kind of processes.
-
-    - ProductionProcesses: A process that can be performed on a product by a production resource.
-    - TransportProcesses: A process that can be performed on a product by a transport resource.
-    - CapabilityProcesses: A process that can be performed on a product by a resource, based on the capability of the resource.
+    Abstract process model base class that defines the interface for all process models.
     """
 
-    ProductionProcesses = "ProductionProcesses"
-    TransportProcesses = "TransportProcesses"
-    CapabilityProcesses = "CapabilityProcesses"
-    CompoundProcesses = "CompoundProcesses"
-    RequiredCapabilityProcesses = "RequiredCapabilityProcesses"
-
+    @abstractmethod
+    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
+        """
+        Returns the next possible processes.
 
-class ProcessData(CoreAsset):
-    """
-    Class that represents process data. Acts as a base class for all process data classes.
+        Returns:
+            Optional[List[process.PROCESS_UNION]]: List of possible processes.
+        """
+        pass
 
-    Args:
-        ID (str): ID of the process.
-        description (str): Description of the process.
-        time_model_id (str): ID of the time model of the process.
-    """
+    @abstractmethod
+    def update_marking_from_transition(
+        self, chosen_process: process.PROCESS_UNION
+    ) -> None:
+        """
+        Updates the marking of the process model based on the chosen process.
 
-    time_model_id: str
+        Args:
+            chosen_process (process.PROCESS_UNION): The chosen process that is executed.
+        """
+        pass
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "ID": "P1",
-                "description": "Process 1",
-                "time_model_id": "function_time_model_1",
-            }
-        }
 
-
-class ProductionProcessData(ProcessData):
+class ListProcessModel(ProcessModel):
     """
-    Class that represents production process data.
+    Process model that is based on a list of processes. The processes are executed sequentially in the order of the list.
 
     Args:
-        ID (str): ID of the process.
-        description (str): Description of the process.
-        time_model_id (str): ID of the time model of the process.
-        type (Literal[ProcessTypeEnum.ProductionProcesses]): Type of the process.
-
-    Examples:
-        A production process with ID "P1", description "Process 1" and time model ID "function_time_model_1":
-        ``` py
-        import prodsys
-        prodsys.processes_data.ProductionProcessData(
-            ID="P1",
-            description="Process 1",
-            time_model_id="function_time_model_1",
-            type="ProductionProcesses",
-        )
-        ```
+        process_list (List[process.PROCESS_UNION]): List of processes that are executed sequentially.
     """
 
-    type: Literal[ProcessTypeEnum.ProductionProcesses]
+    process_list: List[process.PROCESS_UNION]
+    current_marking: int = Field(default=0, init=False)
+
+    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
+        if self.current_marking == len(self.process_list):
+            return None
+        return [self.process_list[self.current_marking]]
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Production process",
-                "value": {
-                    "ID": "P1",
-                    "description": "Process 1",
-                    "time_model_id": "function_time_model_1",
-                    "type": "ProductionProcesses",
-                },
-            }
-        }
+    def update_marking_from_transition(
+        self, chosen_process: process.PROCESS_UNION
+    ) -> None:
+        self.current_marking += 1
 
 
-class CapabilityProcessData(ProcessData):
+class PrecendeGraphNode(BaseModel):
     """
-    Class that represents capability process data. Capability processes are not compared by their IDs but their Capabilities.
+    Class that represents a node in a precedence graph.
 
     Args:
-        ID (str): ID of the process.
-        description (str): Description of the process.
-        time_model_id (str): ID of the time model of the process.
-        type (Literal[ProcessTypeEnum.CapabilityProcesses]): Type of the process.
-        capability (str): Capability of the process.
-
-    Examples:
-        A capability process with ID "P1", description "Process 1", time model ID "function_time_model_1" and capability "C1":
-        ``` py
-        import prodsys
-        prodsys.processes_data.CapabilityProcessData(
-            ID="P1",
-            description="Process 1",
-            time_model_id="function_time_model_1",
-            type="CapabilityProcesses",
-            capability="C1",
-        )
-        ```
+        process (process.PROCESS_UNION): The process that is represented by the node.
+        successors (Optional[List[PrecendeGraphNode]]): List of successor nodes.
+        predecessors (Optional[List[PrecendeGraphNode]]): List of predecessor nodes.
+
+    Attributes:
+        marking (bool): Indicates if the node is marked.
     """
 
-    type: Literal[ProcessTypeEnum.CapabilityProcesses]
-    capability: str
+    process: process.PROCESS_UNION
+    successors: Optional[List[PrecendeGraphNode]] = []
+    predecessors: Optional[List[PrecendeGraphNode]] = []
+    marking: bool = Field(default=False, init=False)
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Capability process",
-                "value": {
-                    "ID": "P1",
-                    "description": "Process 1",
-                    "time_model_id": "function_time_model_1",
-                    "type": "CapabilityProcesses",
-                    "capability": "C1",
-                },
-            }
-        }
+    def update_marking(self):
+        """
+        Updates the marking of the node, to save that the process has been executed.
+        """
+        self.marking = True
 
-class TransportProcessData(ProcessData):
-    """
-    Class that represents transport process data.
 
-    Args:
-        ID (str): ID of the process.
-        description (str): Description of the process.
-        time_model_id (str): ID of the time model of the process
-        type (Literal[ProcessTypeEnum.TransportProcesses]): Type of the process.
-
-    Examples:
-        A transport process with ID "TP1", description "Transport Process 1" and time model ID "manhattan_time_model_1":
-        ``` py
-        import prodsys
-        prodsys.processes_data.TransportProcessData(
-            ID="TP1",
-            description="Transport Process 1",
-            time_model_id="manhattan_time_model_1",
-            type="TransportProcesses",
-        )
-        ```
+def get_predecessor_processes(
+    target_process_id: str, adjacency_matrix: Dict[str, List[str]]
+) -> List[process.PROCESS_UNION]:
     """
+    Returns the predecessing processes' IDs of a ID of a process.
 
-    type: Literal[ProcessTypeEnum.TransportProcesses]
+    Args:
+        target_process_id (str): process ID of the process for which the predecessing processes' IDs are returned.
+        adjacency_matrix (Dict[str, List[str]]): Adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the successor processes.
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Transport process",
-                "value": {
-                    "ID": "TP1",
-                    "description": "Transport Process 1",
-                    "time_model_id": "manhattan_time_model_1",
-                    "type": "TransportProcesses",
-                },
-            }
-        }
+    Returns:
+        List[process.PROCESS_UNION]: List of predecessing processes' IDs.
+    """
+    predecessors = []
+    for process_id, successors in adjacency_matrix.items():
+        if target_process_id in successors:
+            predecessors.append(process_id)
+    return predecessors
 
 
-class CompoundProcessData(CoreAsset):
+def get_predecessors_adjacency_matrix(
+    adjacency_matrix: Dict[str, List[str]]
+) -> Dict[str, List[str]]:
     """
-    Class that represents a compound process. A compound process is a container for multiple processes that belong together, e.g. if a hardware module enables all processes of a CompoundProcess or if multiple similar processes can be performed.
-    
+    Returns the predecessing processes' IDs of all processes in a process model.
+
     Args:
-        ID (str): ID of the process module.
-        description (str): Description of the process module.
-        process_ids (List[str]): Process IDs of the process module.
-    """
-    process_ids: List[str]
-    type: Literal[ProcessTypeEnum.CompoundProcesses]
-
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Compound Process",
-                "value": {
-                    "ID": "CP1",
-                    "description": "Compound Process 1",
-                    "process_ids": ["P1", "P2"],
-                    "type": "CompoundProcesses",
-                },
-            }
-        }
+        adjacency_matrix (Dict[str, List[str]]): Adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the successor processes.
 
+    Returns:
+        Dict[str, List[str]]: Predecessor adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the predecessing processes.
+    """
+    predecessors_adjacency_matrix = {}
+    for process_id in adjacency_matrix.keys():
+        predecessors_adjacency_matrix[process_id] = get_predecessor_processes(
+            process_id, adjacency_matrix
+        )
+    return predecessors_adjacency_matrix
 
 
-class RequiredCapabilityProcessData(CoreAsset):
+def get_adjacency_matrix_from_edges(edges: List[List[str]]) -> Dict[str, List[str]]:
     """
-    Class that represents required capability process data. Capability processes are not compared by their IDs but their Capabilities. The required capability process data does not specify a time model ID, as it is not a process that can be performed, but a capability that is required.
+    Returns the adjacency matrix of a process model from a list of edges.
 
     Args:
-        ID (str): ID of the process.
-        description (str): Description of the process.
-        type (Literal[ProcessTypeEnum.CapabilityProcesses]): Type of the process.
-        capability (str): Capability of the process.
-
-    Examples:
-        A required capability process with ID "P1", description "Process 1", and capability "C1":
-        ``` py
-        import prodsys
-        prodsys.processes_data.CapabilityProcessData(
-            ID="P1",
-            description="Process 1",
-            type="RequiredCapabilityProcesses",
-            capability="C1",
-        )
-        ```
-    """
-
-    type: Literal[ProcessTypeEnum.RequiredCapabilityProcesses]
-    capability: str
+        edges (List[List[str]]): List of edges. Each edge is a list of two process IDs. The first process ID is the predecessor and the second process ID is the successor.
+
+    Returns:
+        Dict[str, List[str]]: Adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the successor processes.
+    """
+    nodes = list(set(flatten(edges)))
+    adjacency_matrix = {}
+    for node in nodes:
+        successors = [edge[1] for edge in edges if edge[0] == node]
+        adjacency_matrix[node] = successors
+    return adjacency_matrix
+
+
+class PrecedenceGraphProcessModel(ProcessModel):
+    """
+    Process model that is based on a precedence graph.
+
+    Attributes:
+        nodes (List[PrecendeGraphNode]): List of nodes in the precedence graph.
+        current_marking (Optional[PrecendeGraphNode]): The current marking, i.e. the node that represents the previously executed process, of the process model.
+    """
+
+    nodes: List[PrecendeGraphNode] = Field(default_factory=list, init=False)
+    current_marking: Optional[PrecendeGraphNode] = Field(init=False)
+
+    def __str__(self) -> str:
+        """
+        Returns a string representation of the adjacency matrix of the process model.
+
+        Returns:
+            str: String representation of the adjacency matrix of the process model.
+        """
+        adjacency_matrix = {}
+        for node in self.nodes:
+            adjacency_matrix[node.process.process_data.ID] = [
+                successor.process.process_data.ID for successor in node.successors
+            ]
+        return str(adjacency_matrix)
+
+    def set_initial_marking(self):
+        """
+        Sets the initial marking of the process model. The initial marking is a node that has no predecessing nodes.
+
+        Raises:
+            ValueError: If no initial marking is found.
+        """
+        possible_starts = []
+        for node in self.nodes:
+            if not node.predecessors:
+                possible_starts.append(node)
+        if not possible_starts:
+            raise ValueError("No initial marking found")
+        self.current_marking = random.choice(possible_starts)
+
+    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
+        if not self.current_marking:
+            self.set_initial_marking()
+        possible_processes = [
+            node.process
+            for node in self.nodes
+            if not node.marking
+            and (not node.predecessors or all(n.marking for n in node.predecessors))
+        ]
+        return possible_processes
+
+    def update_marking_from_transition(
+        self, chosen_process: process.PROCESS_UNION
+    ) -> None:
+        chosen_node = [
+            node for node in self.nodes if node.process == chosen_process
+        ].pop()
+        chosen_node.update_marking()
+        self.current_marking = chosen_node
+
+    def get_node_process_ids(self) -> List[str]:
+        """
+        Returns the process IDs of all nodes in the process model.
+
+        Returns:
+            List[str]: List of process IDs of all nodes in the process model.
+        """
+        return [node.process.process_data.ID for node in self.nodes]
+
+    def add_node(
+        self,
+        process: process.PROCESS_UNION,
+        successors: List[process.PROCESS_UNION],
+        predecessors: List[process.PROCESS_UNION],
+    ) -> None:
+        """
+        Adds a node to the process model. If the processes of the successors and predecessors are not in the process model, they are added as well, with for now empty lists of successors and predecessors.
+
+        Args:
+            process (process.PROCESS_UNION): Process that is represented by the node.
+            successors (List[process.PROCESS_UNION]): List of successor processes.
+            predecessors (List[process.PROCESS_UNION]): List of predecessor processes.
+        """
+        if not process.process_data.ID in self.get_node_process_ids():
+            node = PrecendeGraphNode(process=process, successors=[], predecessors=[])
+            self.nodes.append(node)
+        else:
+            node = [node for node in self.nodes if node.process == process].pop()
+
+        successor_nodes: List[PrecendeGraphNode] = []
+        for successor in successors:
+            if successor.process_data.ID not in self.get_node_process_ids():
+                self.add_node(successor, [], [])
+
+            successor_nodes.append(
+                [node for node in self.nodes if node.process == successor].pop()
+            )
+        node.successors = successor_nodes
+
+        predecessor_nodes: List[PrecendeGraphNode] = []
+        for predecessor in predecessors:
+            if predecessor.process_data.ID not in self.get_node_process_ids():
+                self.add_node(predecessor, [], [])
+            predecessor_nodes.append(
+                [node for node in self.nodes if node.process == predecessor].pop()
+            )
 
-    class Config:
-        schema_extra = {
-            "example": {
-                "summary": "Required Capability process",
-                "value": {
-                    "ID": "P1",
-                    "description": "Process 1",
-                    "type": "RequiredCapabilityProcesses",
-                    "capability": "C1",
-                },
-            }
-        }
-
-
-PROCESS_DATA_UNION = Union[
-    CompoundProcessData, RequiredCapabilityProcessData,
-    ProductionProcessData, TransportProcessData, CapabilityProcessData
-]
+        node.predecessors = predecessor_nodes
```

### Comparing `prodsys-0.4.4/prodsys/models/product_data.py` & `prodsys-0.5.0/prodsys/models/product_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
-
-from typing import Union, List, Dict
-
+from hashlib import md5
+from typing import Union, List, Dict, TYPE_CHECKING
 from pydantic import root_validator
-
 from prodsys.models.core_asset import CoreAsset
 
+if TYPE_CHECKING:
+    from prodsys.adapters.adapter import ProductionSystemAdapter
+
 
 class ProductData(CoreAsset):
     """
     Class that represents product data, specifically the required processes and the allows tranport process.
 
     The processes describe thereby the process model that needs to be completed for the product to be finished. There are three different ways to describe the process model:
 
@@ -73,14 +74,51 @@
         ```
     """
 
     product_type: str
     processes: Union[List[str], List[List[str]], Dict[str, List[str]]]
     transport_process: str
 
+    def hash(self, adapter: ProductionSystemAdapter) -> str:
+        """
+        Returns a unique hash of the product considering the processes and the transport process. Can be used to compare products for equal functionality.
+
+        Args:
+            adapter (ProductionSystemAdapter): Adapter that contains the process data.
+
+        Raises:
+            ValueError: If the process or transport process is not found in the adapter.
+
+        Returns:
+            str: Hash of the product.
+        """
+        processes_hashes = []
+        transport_process_hash = ""
+
+        if not isinstance(self.processes, list) or isinstance(self.processes[0], list):
+            # TODO: Implement hash for adjacency matrix and edges process models
+            raise NotImplementedError("Only list of processes is supported for hashing. Complex process models are not supported yet.")
+        
+        for process_id in self.processes:
+            for process in adapter.process_data:
+                if process.ID == process_id:
+                    processes_hashes.append(process.hash(adapter))
+                    break
+            else:
+                raise ValueError(f"Process with ID {self.processes} not found for product {self.ID}.")
+        
+        for transport_process in adapter.process_data:
+            if transport_process.ID == self.transport_process:
+                transport_process_hash = transport_process.hash(adapter)
+                break
+        else:
+            raise ValueError(f"Transport process with ID {self.transport_process} not found for product {self.ID}.")
+        
+        return md5("".join([*processes_hashes, transport_process_hash]).encode("utf-8")).hexdigest()
+                   
     @root_validator(pre=True)
     def check_processes(cls, values):
         if "product_type" in values and values["product_type"]:
             values["ID"] = values["product_type"]
         else:
             values["product_type"] = values["ID"]
         return values
```

### Comparing `prodsys-0.4.4/prodsys/models/queue_data.py` & `prodsys-0.5.0/prodsys/models/queue_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Union
+from hashlib import md5
 
 from prodsys.models.core_asset import CoreAsset
-from pydantic import validator
 
 
 class QueueData(CoreAsset):
     """
     Class that represents a queue. If capacity is 0, the queue is considered infinite. Otherwise, the queue can hold a finite number of products cooresponding to the capacity.
 
     Args:
@@ -34,14 +34,25 @@
             capacity=0,
         )
         ```
     """
 
     capacity: Union[int, float] = 0.0
 
+    def hash(self) -> str:
+        """
+        Returns a unique hash for the queue considering its capacity.
+
+
+        Returns:
+            str: Hash of the queue.
+        """
+        return md5((str(self.capacity)).encode("utf-8")).hexdigest()
+
+
     class Config:
         schema_extra = {
             "examples": [
                 {
                     "ID": "Q1",
                     "description": "Finte Queue",
                     "capacity": 10,
```

### Comparing `prodsys-0.4.4/prodsys/models/resource_data.py` & `prodsys-0.5.0/prodsys/models/resource_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 The following resources are available:
 
 - `ProductionResourceData`: Class that represents a production resource.
 - `TransportResourceData`: Class that represents a transport resource.
 """
 
 from __future__ import annotations
-
-from typing import Literal, Union, List, Tuple, Optional
+from hashlib import md5
+from typing import Literal, Union, List, Optional, TYPE_CHECKING
 from enum import Enum
 
 from pydantic import validator, conlist
-
 from prodsys.models.core_asset import CoreAsset
 
+if TYPE_CHECKING:
+    from prodsys.adapters.adapter import ProductionSystemAdapter
+
 
 class ControllerEnum(str, Enum):
     """
     Enum that represents the controller of a resource.
 
     - PipelineController: Pipeline controller.
     - TransportController: Transport controller.
@@ -44,19 +46,23 @@
 
 
 class TransportControlPolicy(str, Enum):
     """
     Enum that represents the control policy of a transport resource.
 
     - FIFO: First in first out.
-    - SPT_transport: Shortest transport time first.
+    - SPT_transport: Shortest raw transport time first. Does not consider distance to start of the transport.
+    - NEAREST_ORIGIN_AND_LONGEST_TARGET_QUEUES_TRANSPORT: Nearest_Origin but also sorts by the length of the target queue to make sure, something can be picked up at the target.
+    - NEAREST_ORIGIN_AND_SHORTEST_TARGET_INPUT_QUEUES_TRANSPORT: Nearest_Origin but also sorts by the length of the target input queue to prefer target machines, that have lower number of products waiting to be processed.
     """
 
     FIFO = "FIFO"
     SPT_transport = "SPT_transport"
+    NEAREST_ORIGIN_AND_LONGEST_TARGET_QUEUES_TRANSPORT = "Nearest_origin_and_longest_target_queues_transport"
+    NEAREST_ORIGIN_AND_SHORTEST_TARGET_INPUT_QUEUES_TRANSPORT = "Nearest_origin_and_shortest_target_input_queues_transport"
 
 
 class ResourceData(CoreAsset):
     """
     Class that represents resource data. Base class for ProductionResourceData and TransportResourceData.
 
     Args:
@@ -68,15 +74,15 @@
         control_policy (Union[ResourceControlPolicy, TransportControlPolicy]): Control policy of the resource.
         process_ids (List[str]): Process IDs of the resource.
         process_capacities (Optional[List[int]], optional): Process capacities of the resource (in sequence of the capacity of the resource). Defaults to None.
         state_ids (Optional[List[str]], optional): State IDs of the resource. Defaults to [].
     """
 
     capacity: int
-    location: conlist(float, min_items=2, max_items=2)
+    location: conlist(float, min_items=2, max_items=2) # type: ignore
 
     controller: ControllerEnum
     control_policy: Union[ResourceControlPolicy, TransportControlPolicy]
 
     process_ids: List[str]
     process_capacities: Optional[List[int]]
     state_ids: Optional[List[str]] = []
@@ -87,16 +93,51 @@
             return [values["capacity"] for _ in values["process_ids"]]
         if len(v) != len(values["process_ids"]):
             raise ValueError(
                 f"process_capacities {v} must have the same length as processes {values['process_ids']}"
             )
         if max(v) > values["capacity"]:
             raise ValueError("process_capacities must be smaller than capacity")
-        return v
+        return v 
+    
+    def hash(self, adapter: ProductionSystemAdapter) -> str:
+        """
+        Returns a unique hash of the resource considering the capacity, location, controller, processes, process capacities and states. Can be used to compare resources for equal functionality.
+
+        Args:
+            adapter (ProductionSystemAdapter): Adapter that contains the process and state data.
+
+        Raises:
+            ValueError: If a state or process is not found in the adapter.
+
+        Returns:
+            str: Hash of the resource.
+        """
+        state_hashes = []
+        process_hashes = []
+
+        for state_id in self.state_ids:
+            for state in adapter.state_data:
+                if state.ID == state_id:
+                    state_hashes.append(state.hash(adapter))
+                    break
+            else:
+                raise ValueError(f"State with ID {state_id} not found for resource {self.ID}.")
+            
+
+        for process_id in self.process_ids:
+            for process in adapter.process_data:
+                if process.ID == process_id:
+                    process_hashes.append(process.hash(adapter))
+                    break
+            else:
+                raise ValueError(f"Process with ID {process_id} not found for resource {self.ID}.")
 
+        return md5(("".join([str(self.capacity), *map(str, self.location), self.controller, *sorted(process_hashes), *map(str, self.process_capacities), *sorted(state_hashes)])).encode("utf-8")).hexdigest()
+    
 
 class ProductionResourceData(ResourceData):
     """
     Class that represents production resource data.
 
     Args:
         ID (str): ID of the resource.
@@ -136,14 +177,41 @@
 
     controller: Literal[ControllerEnum.PipelineController]
     control_policy: ResourceControlPolicy
 
     input_queues: Optional[List[str]]
     output_queues: Optional[List[str]]
 
+    def hash(self, adapter: ProductionSystemAdapter) -> str:
+        """
+        Returns a unique hash of the resource considering the capacity, location, controller, processes, process capacities, states, input queues and output queues. Can be used to compare resources for equal functionality.
+
+        Args:
+            adapter (ProductionSystemAdapter): Adapter that contains the process and queue data.
+
+        Raises:
+            ValueError: If a queue, state or process is not found in the adapter.
+
+        Returns:
+            str: Hash of the resource.
+        """
+        base_class_hash = super().hash(adapter)
+        queue_hashes = []
+        for queue_id in self.input_queues + self.output_queues:
+            for queue in adapter.queue_data:
+                if queue.ID == queue_id:
+                    queue_hashes.append(queue.hash())
+                    break
+            else:
+                raise ValueError(f"Queue with ID {queue_id} not found for resource {self.ID}.")
+
+        return md5(("".join([base_class_hash, *sorted(queue_hashes)])).encode("utf-8")).hexdigest()
+
+
+
     class Config:
         schema_extra = {
             "example": {
                 "summary": "Production Resource Data",
                 "value": {
                     "ID": "R1",
                     "description": "Resource 1",
```

### Comparing `prodsys-0.4.4/prodsys/models/scenario_data.py` & `prodsys-0.5.0/prodsys/models/scenario_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     optimization scenario, i.e. the different possibilities to adjust the configuration to find a solution with higher
     performance. Options consider possible transformations of the configuration, possible logics of controllers and routers
     and possible positions of machines in the layout.
 
     Args:
         transformations (List[ReconfigurationEnum]): List of possible transformations of the configuration.
         machine_controllers (List[Literal["FIFO", "LIFO", "SPT"]]): List of possible controllers for machines.
-        transport_controllers (List[Literal["FIFO", "SPT_transport"]]): List of possible controllers for transport resources.
+        transport_controllers (List[Literal["FIFO", "SPT_transport", "Nearest_origin_and_longest_target_queues_transport", "Nearest_origin_and_shortest_target_input_queues_transport"]]): List of possible controllers for transport resources.
         routing_heuristics (List[Literal["shortest_queue", "random", "FIFO"]]): List of possible routing heuristics for sources.
         positions (List[conlist(float, min_items=2, max_items=2)]): List of possible positions for machines in the layout.
 
     Raises:
         ValueError: If the positions are not a list of tuples of length 2.
     """
```

### Comparing `prodsys-0.4.4/prodsys/models/sink_data.py` & `prodsys-0.5.0/prodsys/models/sink_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
+from hashlib import md5
+from typing import List, Optional, TYPE_CHECKING
+from pydantic import conlist
 
-from typing import Literal, Union, List, Tuple, Optional
+from prodsys.models.core_asset import CoreAsset
 
-from pydantic import validator, conlist
+if TYPE_CHECKING:
+    from prodsys.adapters.adapter import ProductionSystemAdapter
 
-from prodsys.models.core_asset import CoreAsset
 
 
 class SinkData(CoreAsset):
     """
     Class that represents a sink.
 
     Args:
@@ -28,24 +31,55 @@
             location=[50.0, 50.0],
             product_type="Product_1",
             input_queues=["SinkQueue"],
         )
         ```
     """
 
-    location: conlist(float, min_items=2, max_items=2)
+    location: conlist(float, min_items=2, max_items=2) # type: ignore
     product_type: str
     input_queues: Optional[List[str]]
-
+    
     class Config:
         schema_extra = {
             "example": {
                 "summary": "Sink",
                 "value": {
                     "ID": "SK1",
                     "description": "Sink 1",
                     "location": [50.0, 50.0],
                     "product_type": "Product_1",
                     "input_queues": ["SinkQueue"],
                 },
             }
         }
+    
+    def hash(self, adapter: ProductionSystemAdapter) -> str:
+        """
+        Returns a unique hash for the sink considering its location, product type and input queues.
+
+        Args:
+            adapter (ProductionSystemAdapter): Adapter of the production system.
+
+        Raises:
+            ValueError: If the product or input queue is not found in the adapter.
+
+        Returns:
+            str: Hash of the sink.
+        """
+        for product in adapter.product_data:
+            if product.product_type == self.product_type:
+                product_hash = product.hash(adapter)
+                break
+        else:
+            raise ValueError(f"Product with ID {self.product_type} not found for sink {self.ID}.")
+        
+        input_queue_hashes = []
+        for queue_id in self.input_queues:
+            for queue in adapter.queue_data:
+                if queue.ID == queue_id:
+                    input_queue_hashes.append(queue.hash())
+                    break
+            else:
+                raise ValueError(f"Queue with ID {queue_id} not found for sink {self.ID}.")
+
+        return md5("".join([*map(str, self.location), product_hash, *sorted(input_queue_hashes)]).encode("utf-8")).hexdigest()
```

### Comparing `prodsys-0.4.4/prodsys/models/source_data.py` & `prodsys-0.5.0/prodsys/models/source_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
-
-from typing import Literal, Union, List, Tuple, Optional
-
-from pydantic import validator, conlist
-
+from hashlib import md5
+from typing import List, Optional, TYPE_CHECKING
+from pydantic import conlist
 from enum import Enum
 
 from prodsys.models.core_asset import CoreAsset
 
+if TYPE_CHECKING:
+    from prodsys.adapters.adapter import ProductionSystemAdapter
+
+
 class RoutingHeuristic(str, Enum):
     """
     Enum that represents the routing heuristic of a source.
     """
     random = "random"
     shortest_queue = "shortest_queue"
     FIFO = "FIFO"
@@ -42,20 +44,58 @@
             product_type="Product_1",
             time_model_id="function_time_model_4",
             router="SimpleRouter",
             routing_heuristic="shortest_queue",
             output_queues=["SourceQueue"],
         )
     """
-    location: conlist(float, min_items=2, max_items=2)
+    location: conlist(float, min_items=2, max_items=2) # type: ignore
     product_type: str
     time_model_id: str
     routing_heuristic: RoutingHeuristic
     output_queues: Optional[List[str]]
+    
+    def hash(self, adapter: ProductionSystemAdapter) -> str:
+        """
+        Returns a unique hash for the source considering its location, product type, time model, routing heuristic and output queues.
+
+        Args:
+            adapter (ProductionSystemAdapter): Adapter of the production system.
+
+        Raises:
+            ValueError: If the product, time model or output queue is not found in the adapter.
+
+        Returns:
+            str: Hash of the source.
+        """
+        for product in adapter.product_data:
+            if product.product_type == self.product_type:
+                product_hash = product.hash(adapter)
+                break
+        else:
+            raise ValueError(f"Product with ID {self.product_type} not found for source {self.ID}.")
+
+        for time_model in adapter.time_model_data:
+            if time_model.ID == self.time_model_id:
+                time_model_hash = time_model.hash()
+                break
+        else:
+            raise ValueError(f"Time model with ID {self.time_model_id} not found for source {self.ID}.")
+        
+        output_queue_hashes = []
+        for output_queue in self.output_queues:
+            for queue in adapter.queue_data:
+                if queue.ID == output_queue:
+                    output_queue_hashes.append(queue.hash())
+                    break
+            else:
+                raise ValueError(f"Queue with ID {output_queue} not found for source {self.ID}.")
 
+        return md5(("".join([*map(str, self.location), product_hash, time_model_hash, self.routing_heuristic, *sorted(output_queue_hashes)])).encode("utf-8")).hexdigest()
+    
     class Config:
         schema_extra = {
             "example": {
                 "summary": "Source",
                 "value": {
                     "ID": "S1",
                     "description": "Source 1",
```

### Comparing `prodsys-0.4.4/prodsys/models/time_model_data.py` & `prodsys-0.5.0/prodsys/models/time_model_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 The following time models are possible:
 - `SequentialTimeModelData`: A time model that is based on a sequence of values.
 - `FunctionTimeModelData`: A time model that is based on a distribution function which gets sampled.
 - `ManhattanDistanceTimeModelData`: A time model that is based on the manhattan distance between two nodes and a constant velocity.
 """
 
 from __future__ import annotations
+from hashlib import md5
+from typing import List, Union
+from enum import Enum
 
-from typing import List, Literal, Union
 from pydantic import Field
 
-from enum import Enum
 from prodsys.models.core_asset import CoreAsset
 from prodsys.util.statistical_functions import FunctionTimeModelEnum
 
 
 class TimeModelEnum(str, Enum):
     """
     Enum that represents the different kind time models.
@@ -51,14 +52,23 @@
             sequence=[25.0, 13.0, 15.0, 16.0, 17.0, 20.0, 21.0],
         )
         ```
     """
 
     sequence: List[float]
 
+    def hash(self) -> str:
+        """
+        Returns a unique hash for the time model considering its sequence. Can be used to compare time models for equal functionality.
+
+        Returns:
+            str: Hash of the time model.
+        """
+        return md5(("".join([*map(str, self.sequence)])).encode("utf-8")).hexdigest()
+    
     class Config:
         schema_extra = {
             "example": {
                 "summary": "Sequential time model",
                 "value": {
                     "ID": "sequence_time_model_1",
                     "description": "Examplary sequence time model",
@@ -107,16 +117,23 @@
                     "description": "normal distribution time model with 20 minutes",
                     "distribution_function": "normal",
                     "location": 20.0,
                     "scale": 5.0,
                 },
             }
         }
-
-
+    def hash(self) -> str:
+        """
+        Returns a unique hash for the time model considering its distribution function, location and scale. Can be used to compare time models for equal functionality.
+
+        Returns:
+            str: Hash of the time model.
+        """
+        return md5(("".join([*map(str, [self.distribution_function, self.location, self.scale])])).encode("utf-8")).hexdigest()
+    
 class ManhattanDistanceTimeModelData(CoreAsset):
     """
     Class that represents a time model that is based on the manhattan distance between two nodes and a constant velocity.
 
     Args:
         ID (str): ID of the time model.
         description (str): Description of the time model.
@@ -134,14 +151,23 @@
             reaction_time=0.15,
         )
     """
 
     speed: float
     reaction_time: float
 
+    def hash(self) -> str:
+        """
+        Returns a unique hash for the time model considering its speed and reaction time. Can be used to compare time models for equal functionality.
+
+        Returns:
+            str: Hash of the time model.
+        """
+        return md5(("".join([*map(str, [self.speed, self.reaction_time])])).encode("utf-8")).hexdigest()
+    
     class Config:
         schema_extra = {
             "example": {
                 "summary": "Manhattan time model",
                 "value": {
                     "ID": "manhattan_time_model_1",
                     "description": "manhattan time model with speed 180 m/min = 3 m/s",
```

### Comparing `prodsys-0.4.4/prodsys/optimization/__init__.py` & `prodsys-0.5.0/prodsys/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/optimization/evolutionary_algorithm.py` & `prodsys-0.5.0/prodsys/optimization/evolutionary_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         ind.fitness.values = fit
         aggregated_fitness = sum(ind.fitness.wvalues)
         generation_performances.append(aggregated_fitness)
         performances[str(solution_dict["current_generation"])][ind[0].ID] = {
             "agg_fitness": aggregated_fitness,
             "fitness": [float(value) for value in ind.fitness.values],
             "time_stamp": time.perf_counter() - start,
+            "hash": ind[0].hash(),
         }
 
     if optimization.VERBOSE:
         print("Best Performance: ", max(generation_performances))
         print(
             "Average Performance: ",
             sum(generation_performances) / len(generation_performances),
@@ -267,15 +268,19 @@
         create_default_breakdown_states(base_configuration)
 
     util.prepare_save_folder(save_folder + "/")
     set_seed(hyper_parameters.seed)
 
     weights = get_weights(base_configuration, "max")
 
-    solution_dict = {"current_generation": "0", "0": []}
+    # TODO: rework solution_dict and performances to classes
+    solution_dict = {
+        "current_generation": "0", 
+        "hashes": {} 
+    }
     performances = {}
     performances["0"] = {}
     start = time.perf_counter()
 
     toolbox = register_functions_in_toolbox(
         base_configuration=base_configuration,
         solution_dict=solution_dict,
@@ -302,15 +307,14 @@
 
     for g in range(hyper_parameters.number_of_generations):
         current_generation = g + 1
         optimization.VERBOSE = True
         if optimization.VERBOSE:
             print(f"\nGeneration: {current_generation}")
         solution_dict["current_generation"] = str(current_generation)
-        solution_dict[str(current_generation)] = []
         performances[str(current_generation)] = {}
 
         # Vary population
         offspring = tools.selTournamentDCD(population, len(population))
         offspring = [toolbox.clone(ind) for ind in offspring]
         offspring = algorithms.varAnd(
             offspring, toolbox, cxpb=hyper_parameters.crossover_rate, mutpb=hyper_parameters.mutation_rate
```

### Comparing `prodsys-0.4.4/prodsys/optimization/math_opt.py` & `prodsys-0.5.0/prodsys/optimization/math_opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -519,14 +519,15 @@
             optimization_util.document_individual(
                 solution_dict, save_folder, [new_adapter]
             )
             performances["00"][new_adapter.ID] = {
                 "agg_fitness": 0.0,
                 "fitness": [float(value) for value in simulation_results],
                 "time_stamp": 0.0,
+                "hash": new_adapter.hash(),
             }
         with open(f"{save_folder}/optimization_results.json", "w") as json_file:
             json.dump(performances, json_file)
 
 
 class MathOptHyperparameters(BaseModel):
     """
```

### Comparing `prodsys-0.4.4/prodsys/optimization/optimization_analysis.py` & `prodsys-0.5.0/prodsys/optimization/optimization_analysis.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/optimization/optimization_util.py` & `prodsys-0.5.0/prodsys/optimization/optimization_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,21 +210,23 @@
         Tuple[float, ...]: Tuple of weights for the objectives.
     """
     weights = []
     for objective in adapter.scenario_data.objectives:
         kpi = parse_obj_as(performance_indicators.KPI_UNION, {"name": objective.name})
         if kpi.target != direction:
             objective.weight *= -1
+        # if direction == "min":
+        #     objective.weight *= -1
         weights.append(objective.weight)
     return tuple(weights)
 
 
 def crossover(ind1, ind2):
-    ind1[0].ID = ""
-    ind2[0].ID = ""
+    ind1[0].ID = str(uuid1())
+    ind2[0].ID = str(uuid1())
 
     crossover_type = random.choice(["machine", "partial_machine", "transport_resource"])
     adapter1: adapters.ProductionSystemAdapter = ind1[0]
     adapter2: adapters.ProductionSystemAdapter = ind2[0]
     machines_1 = adapters.get_machines(adapter1)
     machines_2 = adapters.get_machines(adapter2)
     transport_resources_1 = adapters.get_transport_resources(adapter1)
@@ -278,15 +280,15 @@
     return mutations_operations
 
 
 def mutation(individual):
     mutation_operation = random.choice(get_mutation_operations(individual[0]))
     adapter_object = individual[0]
     if mutation_operation(adapter_object):
-        individual[0].ID = ""
+        individual[0].ID = str(uuid1())
     add_default_queues_to_resources(adapter_object)
     clean_out_breakdown_states_of_resources(adapter_object)
     adjust_process_capacities(adapter_object)
 
     return (individual,)
 
 
@@ -847,14 +849,16 @@
     Returns:
         adapters.ProductionSystemAdapter: Random configuration based on a baseline configuration.
     """
     transformations = baseline.scenario_data.options.transformations
     invalid_configuration_counter = 0
     while True:
         adapter_object = baseline.copy(deep=True)
+        adapter_object.ID = str(uuid1())
+
         if scenario_data.ReconfigurationEnum.PRODUCTION_CAPACITY in transformations:
             get_random_production_capacity(adapter_object)
         if scenario_data.ReconfigurationEnum.TRANSPORT_CAPACITY in transformations:
             get_random_transport_capacity(adapter_object)
         if (
             scenario_data.ReconfigurationEnum.LAYOUT in transformations
             and scenario_data.ReconfigurationEnum.PRODUCTION_CAPACITY
@@ -1001,15 +1005,20 @@
     solution_dict: Dict[str, Union[list, str]],
     save_folder: str,
     individual,
 ):
     adapter_object: adapters.ProductionSystemAdapter = individual[0]
     current_generation = solution_dict["current_generation"]
 
-    solution_dict[current_generation].append(adapter_object.ID)
+    if adapter_object.hash() not in solution_dict["hashes"]:
+        print(f"new solution in generation {current_generation} with ID {adapter_object.ID} and hash {adapter_object.hash()}.")
+        solution_dict["hashes"][adapter_object.hash()] = {
+            "generation": current_generation,
+            "ID": adapter_object.ID,
+        }
 
     adapters.JsonProductionSystemAdapter(**adapter_object.dict()).write_data(
         f"{save_folder}/generation_{current_generation}_{adapter_object.ID}.json"
     )
 
 
 def evaluate(
@@ -1021,41 +1030,36 @@
     individual,
 ) -> List[float]:
     """
     Function that evaluates a configuration.
 
     Args:
         base_scenario (adapters.ProductionSystemAdapter): Baseline configuration.
-        solution_dict (Dict[str, Union[list, str]]): Dictionary containing the solutions of the current and previous generations.
+        solution_dict (Dict[str, Union[list, str]]): Dictionary containing the ids of existing solutions.
         performances (dict): Dictionary containing the performances of the current and previous generations.
         number_of_seeds (int): Number of seeds for the simulation runs.
         individual (List[adapters.ProductionSystemAdapter]): List if length 1 containing the configuration to be evaluated.
 
     Raises:
         ValueError: If the time range is not defined in the scenario data.
 
     Returns:
         List[float]: List of the fitness values of the configuration.
     """
 
     adapter_object: adapters.ProductionSystemAdapter = individual[0]
-    current_generation = solution_dict["current_generation"]
-    if adapter_object.ID:
-        for generation in solution_dict.keys():
-            if (
-                generation != "current_generation"
-                and not generation == current_generation
-                and adapter_object.ID in solution_dict[generation]
-            ):
-                return performances[generation][adapter_object.ID]["fitness"]
-    else:
-        adapter_object.ID = str(uuid1())
+    adapter_object_hash = adapter_object.hash()
+    if adapter_object_hash in solution_dict["hashes"]:
+        evaluated_adapter_generation = solution_dict["hashes"][adapter_object_hash]["generation"]
+        evaluated_adapter_id = solution_dict["hashes"][adapter_object_hash]["ID"]
+        print(f"{adapter_object.ID}: adapter with equal hash already evaluated. Returning fitness of generation {evaluated_adapter_generation} and ID {evaluated_adapter_id}.")
+        return performances[evaluated_adapter_generation][evaluated_adapter_id]["fitness"]
 
     if not check_valid_configuration(adapter_object, base_scenario):
-        # TODO: check if this function is always correct, either max or min for all algorithms?
+        # FIXME: check if this function is always correct, either max or min for all algorithms?
         return [-100000 * weight for weight in get_weights(base_scenario, "max")]
 
     fitness_values = []
 
     for seed in range(number_of_seeds):
         runner_object = runner.Runner(adapter=adapter_object) 
         if not adapter_object.scenario_data.info.time_range:
```

### Comparing `prodsys-0.4.4/prodsys/optimization/simulated_annealing.py` & `prodsys-0.5.0/prodsys/optimization/simulated_annealing.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         # print("\n\t########## Evaluted ind", self.counter, "for value:", performance)
         counter = len(self.performances["0"]) - 1
         document_individual(self.solution_dict, self.save_folder, [self.state])
         self.performances["0"][str(counter)] = {
             "agg_fitness": performance,
             "fitness": [float(value) for value in values],
             "time_stamp": time.perf_counter() - self.start,
+            "hash": self.state.hash(),
         }
         with open(f"{self.save_folder}/optimization_results.json", "w") as json_file:
             json.dump(self.performances, json_file)
 
         return performance
     
 class SimulatedAnnealingHyperparameters(BaseModel):
@@ -195,15 +196,18 @@
     if not initial_solution:
         initial_solution = base_configuration.copy(deep=True)
 
     set_seed(hyper_parameters.seed)
 
     weights = get_weights(base_configuration, "min")
 
-    solution_dict = {"current_generation": "0", "0": []}
+    solution_dict = {
+        "current_generation": "0", 
+        "hashes": {} 
+    }
     performances = {}
     performances["0"] = {}
     start = time.perf_counter()
 
     pso = ProductionSystemOptimization(
         base_configuration=base_configuration,
         save_folder=save_folder,
```

### Comparing `prodsys-0.4.4/prodsys/optimization/tabu_search.py` & `prodsys-0.5.0/prodsys/optimization/tabu_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,18 @@
     if not check_breakdown_states_available(base_configuration):
         create_default_breakdown_states(base_configuration)
 
     set_seed(hyper_parameters.seed)
 
     weights = get_weights(base_configuration, "max")
 
-    solution_dict = {"current_generation": "0", "0": []}
+    solution_dict = {
+        "current_generation": "0", 
+        "hashes": {} 
+    }
     performances = {}
     performances["0"] = {}
     start = time.perf_counter()
 
     class Algorithm(TabuSearch):
         def _score(self, state):
             values = evaluate(
@@ -263,14 +266,15 @@
             print(counter, performance)
             document_individual(solution_dict, save_folder, [state])
 
             performances["0"][str(counter)] = {
                 "agg_fitness": performance,
                 "fitness": [float(value) for value in values],
                 "time_stamp": time.perf_counter() - start,
+                "hash": state.hash()
             }
             with open(f"{save_folder}/optimization_results.json", "w") as json_file:
                 json.dump(performances, json_file)
 
             return performance
 
         def _neighborhood(self):
```

### Comparing `prodsys-0.4.4/prodsys/simulation/__init__.py` & `prodsys-0.5.0/prodsys/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/simulation/control.py` & `prodsys-0.5.0/prodsys/simulation/control.py`

 * *Files 3% similar despite different names*

```diff
@@ -554,15 +554,44 @@
         requests (List[request.TransportResquest]): The list of requests.
     """
     requests.sort(
         key=lambda x: x.process.get_expected_process_time(
             x.origin.get_location(), x.target.get_location()
         )
     )
+def nearest_origin_and_longest_target_queues_transport_control_policy(requests: List[request.TransportResquest]) -> None:
+    """
+    Sort the requests according to nearest origin without considering the target location. 
+    Second order sorting by descending length of the target output queues, to prefer targets where a product can be picked up.
+    Args:
+        requests (List[request.TransportResquest]): The list of requests.
+    """
+    requests.sort(
+        key=lambda x: (
+            x.process.get_expected_process_time(
+                x.resource.data.location, x.origin.get_location()),
+                - x.target.get_output_queue_length()
+                )
+    )
 
+def nearest_origin_and_shortest_target_input_queues_transport_control_policy(requests: List[request.TransportResquest]) -> None:
+    """
+    Sort the requests according to nearest origin without considering the target location.
+    Second order sorting by ascending length of the target input queue so that resources with empty input queues get material to process.
+
+    Args:
+        requests (List[request.TransportResquest]): The list of requests.
+    """
+    requests.sort(
+        key=lambda x: (
+            x.process.get_expected_process_time(
+                x.resource.data.location, x.origin.get_location()),
+            x.target.get_input_queue_length()
+            )
+    )
 
 def agent_control_policy(
     gym_env: sequencing_control_env.AbstractSequencingControlEnv, requests: List[request.Request]
 ) -> None:
     """
     Sort the requests according to the agent's policy.
```

### Comparing `prodsys-0.4.4/prodsys/simulation/logger.py` & `prodsys-0.5.0/prodsys/simulation/logger.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/simulation/observer.py` & `prodsys-0.5.0/prodsys/simulation/observer.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/simulation/proces_models.py` & `prodsys-0.5.0/prodsys/simulation/process.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,253 +1,259 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import List, Optional, Dict
-import random
-from pydantic import BaseModel, Field
+from typing import Union, List, Optional
 
-from prodsys.simulation import process
-from prodsys.util.util import flatten
+from pydantic import BaseModel
 
+from prodsys.simulation import time_model, request
+from prodsys.models import processes_data
 
-class ProcessModel(ABC, BaseModel):
+
+class Process(ABC, BaseModel):
     """
-    Abstract process model base class that defines the interface for all process models.
+    Abstract process base class that defines the interface for all processes.
     """
 
+    process_data: processes_data.PROCESS_DATA_UNION
+    time_model: Optional[time_model.TimeModel]
+
     @abstractmethod
-    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
+    def matches_request(self, request: request.Request) -> bool:
         """
-        Returns the next possible processes.
+        Returns True if the process matches the request.
+
+        Args:
+            request (request.Request): The request.
 
         Returns:
-            Optional[List[process.PROCESS_UNION]]: List of possible processes.
+            bool: True if the process matches the request.
         """
         pass
 
     @abstractmethod
-    def update_marking_from_transition(
-        self, chosen_process: process.PROCESS_UNION
-    ) -> None:
+    def get_process_time(self, *args) -> float:
         """
-        Updates the marking of the process model based on the chosen process.
+        Returns the time it takes to execute the process.
 
-        Args:
-            chosen_process (process.PROCESS_UNION): The chosen process that is executed.
+        Returns:
+            float: Time it takes to execute the process.
         """
         pass
 
+    @abstractmethod
+    def get_expected_process_time(self, *args) -> float:
+        """
+        Returns the expected time it takes to execute the process.
 
-class ListProcessModel(ProcessModel):
-    """
-    Process model that is based on a list of processes. The processes are executed sequentially in the order of the list.
+        Returns:
+            float: Expected time it takes to execute the process.
+        """
+        pass
+
+
+class ProductionProcess(Process):
+    """Class that represents a production process.
 
     Args:
-        process_list (List[process.PROCESS_UNION]): List of processes that are executed sequentially.
+        process_data (processes_data.ProductionProcessData): The process data.
+        time_model (time_model.TimeModel): The time model.
     """
 
-    process_list: List[process.PROCESS_UNION]
-    current_marking: int = Field(default=0, init=False)
+    process_data: processes_data.ProductionProcessData
+
+    def matches_request(self, request: request.Request) -> bool:
+        requested_process = request.process
+        if not isinstance(requested_process, ProductionProcess) and not isinstance(
+            requested_process, CompoundProcess
+        ):
+            return False
+        if isinstance(requested_process, CompoundProcess):
+            return self.process_data.ID in requested_process.process_data.process_ids
+        return requested_process.process_data.ID == self.process_data.ID
 
-    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
-        if self.current_marking == len(self.process_list):
-            return None
-        return [self.process_list[self.current_marking]]
+    def get_process_time(self) -> float:
+        return self.time_model.get_next_time()
 
-    def update_marking_from_transition(
-        self, chosen_process: process.PROCESS_UNION
-    ) -> None:
-        self.current_marking += 1
+    def get_expected_process_time(self) -> float:
+        return self.time_model.get_expected_time()
 
 
-class PrecendeGraphNode(BaseModel):
+class CapabilityProcess(Process):
     """
-    Class that represents a node in a precedence graph.
+    Class that represents a capability process.
 
     Args:
-        process (process.PROCESS_UNION): The process that is represented by the node.
-        successors (Optional[List[PrecendeGraphNode]]): List of successor nodes.
-        predecessors (Optional[List[PrecendeGraphNode]]): List of predecessor nodes.
-
-    Attributes:
-        marking (bool): Indicates if the node is marked.
+        process_data (processes_data.CapabilityProcessData): The process data.
+        time_model (time_model.TimeModel): The time model.
     """
+    process_data: processes_data.CapabilityProcessData
 
-    process: process.PROCESS_UNION
-    successors: Optional[List[PrecendeGraphNode]] = []
-    predecessors: Optional[List[PrecendeGraphNode]] = []
-    marking: bool = Field(default=False, init=False)
+    def matches_request(self, request: request.Request) -> bool:
+        requested_process = request.process
+        if (
+            not isinstance(requested_process, CapabilityProcess)
+            and not isinstance(requested_process, CompoundProcess)
+            and not isinstance(requested_process, RequiredCapabilityProcess)
+        ):
+            return False
+        if isinstance(requested_process, CompoundProcess):
+            return self.process_data.capability in [
+                p.process_data.capability
+                for p in requested_process.contained_processes_data
+                if isinstance(p, CapabilityProcess)
+            ]
+        return requested_process.process_data.capability == self.process_data.capability
 
-    def update_marking(self):
-        """
-        Updates the marking of the node, to save that the process has been executed.
-        """
-        self.marking = True
+    def get_process_time(self) -> float:
+        return self.time_model.get_next_time()
 
+    def get_expected_process_time(self) -> float:
+        return self.time_model.get_expected_time()
 
-def get_predecessor_processes(
-    target_process_id: str, adjacency_matrix: Dict[str, List[str]]
-) -> List[process.PROCESS_UNION]:
+
+class TransportProcess(Process):
     """
-    Returns the predecessing processes' IDs of a ID of a process.
+    Class that represents a transport process.
 
     Args:
-        target_process_id (str): process ID of the process for which the predecessing processes' IDs are returned.
-        adjacency_matrix (Dict[str, List[str]]): Adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the successor processes.
-
-    Returns:
-        List[process.PROCESS_UNION]: List of predecessing processes' IDs.
+        process_data (processes_data.TransportProcessData): The process data.
+        time_model (time_model.TimeModel): The time model.
     """
-    predecessors = []
-    for process_id, successors in adjacency_matrix.items():
-        if target_process_id in successors:
-            predecessors.append(process_id)
-    return predecessors
-
+    process_data: processes_data.TransportProcessData
 
-def get_predecessors_adjacency_matrix(
-    adjacency_matrix: Dict[str, List[str]]
-) -> Dict[str, List[str]]:
-    """
-    Returns the predecessing processes' IDs of all processes in a process model.
+    def matches_request(self, request: request.Request) -> bool:
+        requested_process = request.process
+        if not isinstance(requested_process, TransportProcess) and not isinstance(
+            requested_process, CompoundProcess
+        ):
+            return False
+        if isinstance(requested_process, TransportProcess):
+            return requested_process.process_data.ID == self.process_data.ID
+        return self.process_data.ID in requested_process.process_data.process_ids
 
-    Args:
-        adjacency_matrix (Dict[str, List[str]]): Adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the successor processes.
+    def get_process_time(self, origin: List[float], target: List[float]) -> float:
+        return self.time_model.get_next_time(origin=origin, target=target)
 
-    Returns:
-        Dict[str, List[str]]: Predecessor adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the predecessing processes.
-    """
-    predecessors_adjacency_matrix = {}
-    for process_id in adjacency_matrix.keys():
-        predecessors_adjacency_matrix[process_id] = get_predecessor_processes(
-            process_id, adjacency_matrix
-        )
-    return predecessors_adjacency_matrix
+    def get_expected_process_time(self, *args) -> float:
+        return self.time_model.get_expected_time(*args)
 
 
-def get_adjacency_matrix_from_edges(edges: List[List[str]]) -> Dict[str, List[str]]:
+class CompoundProcess(Process):
     """
-    Returns the adjacency matrix of a process model from a list of edges.
+    Class that represents a compound process.
 
     Args:
-        edges (List[List[str]]): List of edges. Each edge is a list of two process IDs. The first process ID is the predecessor and the second process ID is the successor.
-
-    Returns:
-        Dict[str, List[str]]: Adjacency matrix of the process model. The keys are the process IDs and the values are the IDs of the successor processes.
+        process_data (processes_data.CompoundProcessData): The process data.
+        processes (List[Union[ProductionProcess, TransportProcess, CapabilityProcess, RequiredCapabilityProcess]]): The processes.
     """
-    nodes = list(set(flatten(edges)))
-    adjacency_matrix = {}
-    for node in nodes:
-        successors = [edge[1] for edge in edges if edge[0] == node]
-        adjacency_matrix[node] = successors
-    return adjacency_matrix
+    process_data: processes_data.CompoundProcessData
+    contained_processes_data: List[
+        Union[
+            processes_data.ProductionProcessData,
+            processes_data.TransportProcessData,
+            processes_data.CapabilityProcessData,
+            processes_data.RequiredCapabilityProcessData,
+        ]
+    ]
 
+    def matches_request(self, request: request.Request) -> bool:
+        requested_process = request.process
+        if isinstance(requested_process, ProductionProcess) or isinstance(
+            requested_process, TransportProcess
+        ):
+            return requested_process.process_data.ID in self.process_data.process_ids
+        elif isinstance(requested_process, CapabilityProcess) or isinstance(
+            requested_process, RequiredCapabilityProcess
+        ):
+            return requested_process.process_data.capability in [
+                p.process_data.capability
+                for p in self.contained_processes_data
+                if isinstance(p, CapabilityProcess)
+            ]
+        elif isinstance(requested_process, CompoundProcess):
+            return any(
+                p.ID in self.process_data.process_ids
+                for p in requested_process.contained_processes_data
+                if isinstance(p, ProductionProcess)
+            ) or any(
+                p.capability
+                in [
+                    p.process_data.capability
+                    for p in self.contained_processes_data
+                    if isinstance(p, CapabilityProcess)
+                ]
+                for p in requested_process.contained_processes_data
+                if isinstance(p, CapabilityProcess)
+            )
 
-class PrecedenceGraphProcessModel(ProcessModel):
-    """
-    Process model that is based on a precedence graph.
+    def get_process_time(self) -> float:
+        raise NotImplementedError("CompoundProcess does not have a process time.")
 
-    Attributes:
-        nodes (List[PrecendeGraphNode]): List of nodes in the precedence graph.
-        current_marking (Optional[PrecendeGraphNode]): The current marking, i.e. the node that represents the previously executed process, of the process model.
-    """
+    def get_expected_process_time(self) -> float:
+        raise NotImplementedError("CompoundProcess does not have a process time.")
 
-    nodes: List[PrecendeGraphNode] = Field(default_factory=list, init=False)
-    current_marking: Optional[PrecendeGraphNode] = Field(init=False)
 
-    def __str__(self) -> str:
-        """
-        Returns a string representation of the adjacency matrix of the process model.
+class RequiredCapabilityProcess(Process):
+    """
+    Class that represents a required capability process.
 
-        Returns:
-            str: String representation of the adjacency matrix of the process model.
-        """
-        adjacency_matrix = {}
-        for node in self.nodes:
-            adjacency_matrix[node.process.process_data.ID] = [
-                successor.process.process_data.ID for successor in node.successors
-            ]
-        return str(adjacency_matrix)
+    Args:
+        process_data (processes_data.RequiredCapabilityProcessData): The process data.
+        time_model (time_model.TimeModel): The time model.
+    """
 
-    def set_initial_marking(self):
-        """
-        Sets the initial marking of the process model. The initial marking is a node that has no predecessing nodes.
+    process_data: processes_data.RequiredCapabilityProcessData
 
-        Raises:
-            ValueError: If no initial marking is found.
-        """
-        possible_starts = []
-        for node in self.nodes:
-            if not node.predecessors:
-                possible_starts.append(node)
-        if not possible_starts:
-            raise ValueError("No initial marking found")
-        self.current_marking = random.choice(possible_starts)
-
-    def get_next_possible_processes(self) -> Optional[List[process.PROCESS_UNION]]:
-        if not self.current_marking:
-            self.set_initial_marking()
-        possible_processes = [
-            node.process
-            for node in self.nodes
-            if not node.marking
-            and (not node.predecessors or all(n.marking for n in node.predecessors))
-        ]
-        return possible_processes
+    def matches_request(self, request: request.Request) -> bool:
+        raise NotImplementedError(
+            "RequiredCapabilityProcess cannot be matched but should only request."
+        )
 
-    def update_marking_from_transition(
-        self, chosen_process: process.PROCESS_UNION
-    ) -> None:
-        chosen_node = [
-            node for node in self.nodes if node.process == chosen_process
-        ].pop()
-        chosen_node.update_marking()
-        self.current_marking = chosen_node
+    def get_process_time(self) -> float:
+        raise NotImplementedError(
+            "RequiredCapabilityProcess does not have a process time."
+        )
 
-    def get_node_process_ids(self) -> List[str]:
-        """
-        Returns the process IDs of all nodes in the process model.
+    def get_expected_process_time(self) -> float:
+        raise NotImplementedError(
+            "RequiredCapabilityProcess does not have a process time."
+        )
+    
 
-        Returns:
-            List[str]: List of process IDs of all nodes in the process model.
-        """
-        return [node.process.process_data.ID for node in self.nodes]
+class TransportLinkProcess(Process):
+    """
+    Class that represents a transport link process.
+    """
 
-    def add_node(
-        self,
-        process: process.PROCESS_UNION,
-        successors: List[process.PROCESS_UNION],
-        predecessors: List[process.PROCESS_UNION],
-    ) -> None:
-        """
-        Adds a node to the process model. If the processes of the successors and predecessors are not in the process model, they are added as well, with for now empty lists of successors and predecessors.
+    # TODO: Implement LinkTransportProcess and RouteTransportProcess and their associatd data models.
 
-        Args:
-            process (process.PROCESS_UNION): Process that is represented by the node.
-            successors (List[process.PROCESS_UNION]): List of successor processes.
-            predecessors (List[process.PROCESS_UNION]): List of predecessor processes.
-        """
-        if not process.process_data.ID in self.get_node_process_ids():
-            node = PrecendeGraphNode(process=process, successors=[], predecessors=[])
-            self.nodes.append(node)
-        else:
-            node = [node for node in self.nodes if node.process == process].pop()
-
-        successor_nodes: List[PrecendeGraphNode] = []
-        for successor in successors:
-            if successor.process_data.ID not in self.get_node_process_ids():
-                self.add_node(successor, [], [])
+    def matches_request(self, request: request.Request) -> bool:
+        # 1. check if request is a transport request (if not, return False)
+        # 2. check if transport request is a link request (if not, return False)
 
-            successor_nodes.append(
-                [node for node in self.nodes if node.process == successor].pop()
-            )
-        node.successors = successor_nodes
+        # 3. check for compatibility -> transport links can links from origin to target of resquest
+        # path: List[Links] = path_finder.find_path(request.origin, request.target, self.links)
+        # return not path:
+        #     return False
+        # 4. set path of request
+        # request.path = path
+        # return True
+        pass
+    
+    def get_process_time(self) -> float:
+        # TODO: calculate based on request and path
+        pass
 
-        predecessor_nodes: List[PrecendeGraphNode] = []
-        for predecessor in predecessors:
-            if predecessor.process_data.ID not in self.get_node_process_ids():
-                self.add_node(predecessor, [], [])
-            predecessor_nodes.append(
-                [node for node in self.nodes if node.process == predecessor].pop()
-            )
+    def get_expected_process_time(self) -> float:
+        pass
 
-        node.predecessors = predecessor_nodes
+PROCESS_UNION = Union[
+    CompoundProcess,
+    RequiredCapabilityProcess,
+    ProductionProcess,
+    TransportProcess,
+    CapabilityProcess,
+]
+"""
+Union type for all processes.
+"""
```

### Comparing `prodsys-0.4.4/prodsys/simulation/product.py` & `prodsys-0.5.0/prodsys/simulation/product.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/simulation/request.py` & `prodsys-0.5.0/prodsys/simulation/request.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/simulation/resources.py` & `prodsys-0.5.0/prodsys/simulation/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -238,14 +238,33 @@
         """
         Returns the location of the resource.
 
         Returns:
             List[float]: The location of the resource. Has to have length 2.
         """
         return self.data.location
+    
+
+    def get_input_queue_length(self) -> int:
+        """
+        Returns total number of items in all input_queues.
+
+        Returns:
+            int: Sum of items in the resources input-queues.
+        """
+        return sum([len(q.items) for q in self.input_queues])
+
+    def get_output_queue_length(self) -> int:
+        """
+        Returns total number of items in all output_queues.
+        
+        Returns:
+            int: Sum of items in the resources output-queues.
+        """
+        return sum([len(q.items) for q in self.output_queues])
 
     def set_location(self, new_location: List[float]) -> None:
         """
         Sets the location of the resource.
 
         Args:
             new_location (List[float]): The new location of the resource. Has to have length 2.
```

### Comparing `prodsys-0.4.4/prodsys/simulation/router.py` & `prodsys-0.5.0/prodsys/simulation/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,20 +186,22 @@
 
 
 def shortest_queue_routing_heuristic(
     possible_resources: List[resources.Resource],
 ):
     """
     Sorts the list of possible resources by the length of their input queues and returns the first resource.
+    For Transport resources, the next resource is chosen by the resource with the shortest request queue.
 
     Args:
         possible_resources (List[resources.Resource]): A list of possible resources.
     """
     if any(not isinstance(resource, resources.ProductionResource) for resource in possible_resources):
-        random_routing_heuristic(possible_resources)
+        np.random.shuffle(possible_resources)
+        possible_resources.sort(key=lambda x: len(x.get_controller().requests))
         return
     np.random.shuffle(possible_resources)
     possible_resources.sort(key=lambda x: sum([len(q.items) for q in x.input_queues]))
 
 
 def agent_routing_heuristic(
     gym_env: routing_control_env.AbstractRoutingControlEnv,
```

### Comparing `prodsys-0.4.4/prodsys/simulation/sim.py` & `prodsys-0.5.0/prodsys/simulation/sim.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/simulation/sink.py` & `prodsys-0.5.0/prodsys/simulation/sink.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,14 +42,31 @@
         """
         Returns the location of the sink.
 
         Returns:
             List[float]: The location. Has to be a list of length 2.
         """
         return self.data.location
+
+    def get_input_queue_length(self) -> int:
+        """
+        Returns total number of items in all input_queues. Defaults to 0 for a sink.
+
+        Returns:
+            int(0)
+        """
+        return 0
+
+    def get_output_queue_length(self) -> int:
+        """
+        Returns zero. Needed for transport control policies that use the target locations output queue for request ordering.
+        Returns:
+            int(0)
+        """
+        return 0
     
     def register_finished_product(self, product: product.Product):
         """
         Registers a finished product when it reaches the sink.
 
         Args:
             product (product.Product): The finished product.
```

### Comparing `prodsys-0.4.4/prodsys/simulation/source.py` & `prodsys-0.5.0/prodsys/simulation/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,33 @@
 
     def start_source(self):
         """
         Starts the source simpy process.
         """
         self.env.process(self.create_product_loop())
 
+    def get_output_queue_length(self) -> int:
+        """
+        Returns total number of items in all output_queues.
+
+        Returns:
+            int: Sum of items in the source output-queues.
+        """
+        return sum([len(q.items) for q in self.output_queues])
+
+
+    def get_input_queue_length(self) -> int:
+        """
+        Returns total number of items in all input_queues.
+
+        Returns:
+            int(0)
+        """
+        return 0
+
     def create_product_loop(self) -> Generator:
         """
         Simpy process that creates products and puts them in the output queues.
 
         Yields:
             Generator: Yields when a product is created or when a product is put in an output queue.
         """
```

### Comparing `prodsys-0.4.4/prodsys/simulation/state.py` & `prodsys-0.5.0/prodsys/simulation/state.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/simulation/store.py` & `prodsys-0.5.0/prodsys/simulation/store.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/simulation/time_model.py` & `prodsys-0.5.0/prodsys/simulation/time_model.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/util/kpi_visualization.py` & `prodsys-0.5.0/prodsys/util/kpi_visualization.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/util/post_processing.py` & `prodsys-0.5.0/prodsys/util/post_processing.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/util/runner.py` & `prodsys-0.5.0/prodsys/util/runner.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/util/statistical_functions.py` & `prodsys-0.5.0/prodsys/util/statistical_functions.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/prodsys/util/util.py` & `prodsys-0.5.0/prodsys/util/util.py`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/pyproject.toml` & `prodsys-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodsys"
-version = "0.4.4"
+version = "0.5.0"
 description = "A useful module for production system simulation and optimization"
 authors = ["Sebastian Behrendt <sebastia.behrendt@kit.edu>"]
 license = "MIT"
 readme = ["README.md", "LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
```

### Comparing `prodsys-0.4.4/README.md` & `prodsys-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prodsys-0.4.4/PKG-INFO` & `prodsys-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodsys
-Version: 0.4.4
+Version: 0.5.0
 Summary: A useful module for production system simulation and optimization
 License: MIT
 Author: Sebastian Behrendt
 Author-email: sebastia.behrendt@kit.edu
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

