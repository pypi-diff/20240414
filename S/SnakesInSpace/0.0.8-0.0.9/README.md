# Comparing `tmp/SnakesInSpace-0.0.8.tar.gz` & `tmp/SnakesInSpace-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SnakesInSpace-0.0.8.tar", last modified: Wed Mar 20 20:24:41 2024, max compression
+gzip compressed data, was "SnakesInSpace-0.0.9.tar", last modified: Thu Mar 21 14:23:48 2024, max compression
```

## Comparing `SnakesInSpace-0.0.8.tar` & `SnakesInSpace-0.0.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-20 20:24:41.046749 SnakesInSpace-0.0.8/
--rw-r--r--   0 sam        (501) staff       (20)     1930 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/.gitignore
--rw-r--r--   0 sam        (501) staff       (20)     1072 2024-03-20 14:58:49.000000 SnakesInSpace-0.0.8/LICENSE
--rw-r--r--   0 sam        (501) staff       (20)    58252 2024-03-20 20:24:41.046526 SnakesInSpace-0.0.8/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)    57754 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/README.md
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-20 20:24:41.046195 SnakesInSpace-0.0.8/SnakesInSpace.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)    58252 2024-03-20 20:24:40.000000 SnakesInSpace-0.0.8/SnakesInSpace.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)     2138 2024-03-20 20:24:41.000000 SnakesInSpace-0.0.8/SnakesInSpace.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2024-03-20 20:24:40.000000 SnakesInSpace-0.0.8/SnakesInSpace.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)        6 2024-03-20 20:24:40.000000 SnakesInSpace-0.0.8/SnakesInSpace.egg-info/requires.txt
--rw-r--r--   0 sam        (501) staff       (20)       17 2024-03-20 20:24:40.000000 SnakesInSpace-0.0.8/SnakesInSpace.egg-info/top_level.txt
--rw-r--r--   0 sam        (501) staff       (20)      657 2024-03-20 20:24:24.000000 SnakesInSpace-0.0.8/pyproject.toml
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-20 20:24:41.024768 SnakesInSpace-0.0.8/recipes/
--rw-r--r--   0 sam        (501) staff       (20)      234 2024-03-20 20:01:06.000000 SnakesInSpace-0.0.8/recipes/README.md
--rw-r--r--   0 sam        (501) staff       (20)     4477 2024-03-20 20:01:06.000000 SnakesInSpace-0.0.8/recipes/mine_asteroids.py
--rw-r--r--   0 sam        (501) staff       (20)     4098 2024-03-20 20:06:51.000000 SnakesInSpace-0.0.8/recipes/probe_markets.py
--rw-r--r--   0 sam        (501) staff       (20)       38 2024-03-20 20:24:41.046795 SnakesInSpace-0.0.8/setup.cfg
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-20 20:24:41.029939 SnakesInSpace-0.0.8/snisp/
--rw-r--r--   0 sam        (501) staff       (20)      451 2024-03-11 18:16:09.000000 SnakesInSpace-0.0.8/snisp/__init__.py
--rw-r--r--   0 sam        (501) staff       (20)     7859 2024-03-20 14:56:28.000000 SnakesInSpace-0.0.8/snisp/__main__.py
--rw-r--r--   0 sam        (501) staff       (20)     2952 2024-03-20 14:56:36.000000 SnakesInSpace-0.0.8/snisp/agent.py
--rw-r--r--   0 sam        (501) staff       (20)     2403 2024-03-11 15:33:30.000000 SnakesInSpace-0.0.8/snisp/cache.py
--rw-r--r--   0 sam        (501) staff       (20)     6949 2024-03-13 16:34:01.000000 SnakesInSpace-0.0.8/snisp/client.py
--rw-r--r--   0 sam        (501) staff       (20)     6356 2024-03-20 14:56:36.000000 SnakesInSpace-0.0.8/snisp/contracts.py
--rw-r--r--   0 sam        (501) staff       (20)     3636 2024-03-13 15:21:04.000000 SnakesInSpace-0.0.8/snisp/database.py
--rw-r--r--   0 sam        (501) staff       (20)     5086 2024-03-20 15:05:01.000000 SnakesInSpace-0.0.8/snisp/decorators.py
--rw-r--r--   0 sam        (501) staff       (20)    11802 2024-03-11 03:12:06.000000 SnakesInSpace-0.0.8/snisp/exceptions.py
--rw-r--r--   0 sam        (501) staff       (20)     1781 2024-03-20 14:56:36.000000 SnakesInSpace-0.0.8/snisp/factions.py
--rw-r--r--   0 sam        (501) staff       (20)    51373 2024-03-20 16:15:10.000000 SnakesInSpace-0.0.8/snisp/fleet.py
--rw-r--r--   0 sam        (501) staff       (20)    25389 2024-03-20 15:05:01.000000 SnakesInSpace-0.0.8/snisp/markets.py
--rw-r--r--   0 sam        (501) staff       (20)     8978 2024-03-20 15:02:32.000000 SnakesInSpace-0.0.8/snisp/shipyards.py
--rw-r--r--   0 sam        (501) staff       (20)     4222 2024-03-20 16:12:02.000000 SnakesInSpace-0.0.8/snisp/systems.py
--rw-r--r--   0 sam        (501) staff       (20)     3853 2024-03-20 14:56:28.000000 SnakesInSpace-0.0.8/snisp/tail.py
--rw-r--r--   0 sam        (501) staff       (20)    17791 2024-03-20 16:12:02.000000 SnakesInSpace-0.0.8/snisp/utils.py
--rw-r--r--   0 sam        (501) staff       (20)    29214 2024-03-20 15:46:02.000000 SnakesInSpace-0.0.8/snisp/waypoints.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-20 20:24:41.033998 SnakesInSpace-0.0.8/tests/
--rw-r--r--   0 sam        (501) staff       (20)       43 2024-03-11 03:12:10.000000 SnakesInSpace-0.0.8/tests/README.md
--rw-r--r--   0 sam        (501) staff       (20)     1598 2024-03-11 03:12:10.000000 SnakesInSpace-0.0.8/tests/__init__.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-20 20:24:41.045905 SnakesInSpace-0.0.8/tests/data/
--rw-r--r--   0 sam        (501) staff       (20)      199 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/agent_data.json
--rw-r--r--   0 sam        (501) staff       (20)      905 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/chart.json
--rw-r--r--   0 sam        (501) staff       (20)      215 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/construction_site.json
--rw-r--r--   0 sam        (501) staff       (20)      627 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/contract.json
--rw-r--r--   0 sam        (501) staff       (20)      860 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/contract_delivery.json
--rw-r--r--   0 sam        (501) staff       (20)     1273 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/contracts.json
--rw-r--r--   0 sam        (501) staff       (20)      602 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/dock.json
--rw-r--r--   0 sam        (501) staff       (20)      543 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/extraction.json
--rw-r--r--   0 sam        (501) staff       (20)      281 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/faction.json
--rw-r--r--   0 sam        (501) staff       (20)      381 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/factions.json
--rw-r--r--   0 sam        (501) staff       (20)     6266 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fleet_list.json
--rw-r--r--   0 sam        (501) staff       (20)     6266 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fleet_list_drones.json
--rw-r--r--   0 sam        (501) staff       (20)     6270 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fleet_list_freighters.json
--rw-r--r--   0 sam        (501) staff       (20)     6271 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fleet_list_mining_drones.json
--rw-r--r--   0 sam        (501) staff       (20)     6266 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fleet_list_probes.json
--rw-r--r--   0 sam        (501) staff       (20)     6272 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fleet_list_ships.json
--rw-r--r--   0 sam        (501) staff       (20)     6270 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fleet_list_shuttles.json
--rw-r--r--   0 sam        (501) staff       (20)     6266 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fleet_list_siphon_drones.json
--rw-r--r--   0 sam        (501) staff       (20)     2392 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/fuel_stations.json
--rw-r--r--   0 sam        (501) staff       (20)     1429 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/market.json
--rw-r--r--   0 sam        (501) staff       (20)     1429 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/market_data.json
--rw-r--r--   0 sam        (501) staff       (20)     3096 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/mining_drone.json
--rw-r--r--   0 sam        (501) staff       (20)     1240 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/mount.json
--rw-r--r--   0 sam        (501) staff       (20)      780 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/navigate.json
--rw-r--r--   0 sam        (501) staff       (20)      604 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/orbit.json
--rw-r--r--   0 sam        (501) staff       (20)      787 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/purchase.json
--rw-r--r--   0 sam        (501) staff       (20)      583 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/refine.json
--rw-r--r--   0 sam        (501) staff       (20)      619 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/refuel.json
--rw-r--r--   0 sam        (501) staff       (20)     2468 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/scan.json
--rw-r--r--   0 sam        (501) staff       (20)     2468 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/scan_ships.json
--rw-r--r--   0 sam        (501) staff       (20)      790 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/scan_waypoints.json
--rw-r--r--   0 sam        (501) staff       (20)      738 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/sell.json
--rw-r--r--   0 sam        (501) staff       (20)     3436 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/ship_info.json
--rw-r--r--   0 sam        (501) staff       (20)     3514 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/ship_purchase.json
--rw-r--r--   0 sam        (501) staff       (20)     2345 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/shipyards.json
--rw-r--r--   0 sam        (501) staff       (20)      539 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/siphon.json
--rw-r--r--   0 sam        (501) staff       (20)     3090 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/siphon_drone.json
--rw-r--r--   0 sam        (501) staff       (20)      495 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/supply_construction_site.json
--rw-r--r--   0 sam        (501) staff       (20)     1163 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/survey.json
--rw-r--r--   0 sam        (501) staff       (20)      439 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/system.json
--rw-r--r--   0 sam        (501) staff       (20)      376 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/system_scan.json
--rw-r--r--   0 sam        (501) staff       (20)     1043 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/systems.json
--rw-r--r--   0 sam        (501) staff       (20)      252 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/transfer.json
--rw-r--r--   0 sam        (501) staff       (20)      543 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/update_nav.json
--rw-r--r--   0 sam        (501) staff       (20)      761 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/warp.json
--rw-r--r--   0 sam        (501) staff       (20)      701 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/waypoint.json
--rw-r--r--   0 sam        (501) staff       (20)     2534 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.8/tests/data/waypoints.json
--rw-r--r--   0 sam        (501) staff       (20)      892 2024-03-11 15:28:42.000000 SnakesInSpace-0.0.8/tests/test_agent.py
--rw-r--r--   0 sam        (501) staff       (20)     2186 2024-03-11 15:28:54.000000 SnakesInSpace-0.0.8/tests/test_cache.py
--rw-r--r--   0 sam        (501) staff       (20)     1982 2024-03-11 15:29:20.000000 SnakesInSpace-0.0.8/tests/test_client.py
--rw-r--r--   0 sam        (501) staff       (20)    17108 2024-03-11 15:32:30.000000 SnakesInSpace-0.0.8/tests/test_contract.py
--rw-r--r--   0 sam        (501) staff       (20)     1665 2024-03-11 15:32:21.000000 SnakesInSpace-0.0.8/tests/test_factions.py
--rw-r--r--   0 sam        (501) staff       (20)   153665 2024-03-20 16:15:10.000000 SnakesInSpace-0.0.8/tests/test_fleet.py
--rw-r--r--   0 sam        (501) staff       (20)    65129 2024-03-20 16:12:02.000000 SnakesInSpace-0.0.8/tests/test_markets.py
--rw-r--r--   0 sam        (501) staff       (20)    20202 2024-03-11 15:31:02.000000 SnakesInSpace-0.0.8/tests/test_shipyards.py
--rw-r--r--   0 sam        (501) staff       (20)     5063 2024-03-11 15:31:17.000000 SnakesInSpace-0.0.8/tests/test_systems.py
--rw-r--r--   0 sam        (501) staff       (20)    44335 2024-03-20 16:15:10.000000 SnakesInSpace-0.0.8/tests/test_waypoints.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-21 14:23:48.831628 SnakesInSpace-0.0.9/
+-rw-r--r--   0 sam        (501) staff       (20)     1930 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/.gitignore
+-rw-r--r--   0 sam        (501) staff       (20)     1072 2024-03-20 14:58:49.000000 SnakesInSpace-0.0.9/LICENSE
+-rw-r--r--   0 sam        (501) staff       (20)    58219 2024-03-21 14:23:48.831396 SnakesInSpace-0.0.9/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)    57721 2024-03-21 14:22:42.000000 SnakesInSpace-0.0.9/README.md
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-21 14:23:48.831030 SnakesInSpace-0.0.9/SnakesInSpace.egg-info/
+-rw-r--r--   0 sam        (501) staff       (20)    58219 2024-03-21 14:23:48.000000 SnakesInSpace-0.0.9/SnakesInSpace.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (501) staff       (20)     2138 2024-03-21 14:23:48.000000 SnakesInSpace-0.0.9/SnakesInSpace.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (501) staff       (20)        1 2024-03-21 14:23:48.000000 SnakesInSpace-0.0.9/SnakesInSpace.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (501) staff       (20)        6 2024-03-21 14:23:48.000000 SnakesInSpace-0.0.9/SnakesInSpace.egg-info/requires.txt
+-rw-r--r--   0 sam        (501) staff       (20)       17 2024-03-21 14:23:48.000000 SnakesInSpace-0.0.9/SnakesInSpace.egg-info/top_level.txt
+-rw-r--r--   0 sam        (501) staff       (20)      657 2024-03-21 14:23:36.000000 SnakesInSpace-0.0.9/pyproject.toml
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-21 14:23:48.807854 SnakesInSpace-0.0.9/recipes/
+-rw-r--r--   0 sam        (501) staff       (20)      234 2024-03-20 20:01:06.000000 SnakesInSpace-0.0.9/recipes/README.md
+-rw-r--r--   0 sam        (501) staff       (20)     4477 2024-03-20 20:01:06.000000 SnakesInSpace-0.0.9/recipes/mine_asteroids.py
+-rw-r--r--   0 sam        (501) staff       (20)     4098 2024-03-20 20:06:51.000000 SnakesInSpace-0.0.9/recipes/probe_markets.py
+-rw-r--r--   0 sam        (501) staff       (20)       38 2024-03-21 14:23:48.831683 SnakesInSpace-0.0.9/setup.cfg
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-21 14:23:48.813178 SnakesInSpace-0.0.9/snisp/
+-rw-r--r--   0 sam        (501) staff       (20)      451 2024-03-11 18:16:09.000000 SnakesInSpace-0.0.9/snisp/__init__.py
+-rw-r--r--   0 sam        (501) staff       (20)     7859 2024-03-20 14:56:28.000000 SnakesInSpace-0.0.9/snisp/__main__.py
+-rw-r--r--   0 sam        (501) staff       (20)     2952 2024-03-20 14:56:36.000000 SnakesInSpace-0.0.9/snisp/agent.py
+-rw-r--r--   0 sam        (501) staff       (20)     2403 2024-03-11 15:33:30.000000 SnakesInSpace-0.0.9/snisp/cache.py
+-rw-r--r--   0 sam        (501) staff       (20)     6949 2024-03-13 16:34:01.000000 SnakesInSpace-0.0.9/snisp/client.py
+-rw-r--r--   0 sam        (501) staff       (20)     6356 2024-03-20 14:56:36.000000 SnakesInSpace-0.0.9/snisp/contracts.py
+-rw-r--r--   0 sam        (501) staff       (20)     3636 2024-03-13 15:21:04.000000 SnakesInSpace-0.0.9/snisp/database.py
+-rw-r--r--   0 sam        (501) staff       (20)     5086 2024-03-20 15:05:01.000000 SnakesInSpace-0.0.9/snisp/decorators.py
+-rw-r--r--   0 sam        (501) staff       (20)    11802 2024-03-11 03:12:06.000000 SnakesInSpace-0.0.9/snisp/exceptions.py
+-rw-r--r--   0 sam        (501) staff       (20)     1781 2024-03-20 14:56:36.000000 SnakesInSpace-0.0.9/snisp/factions.py
+-rw-r--r--   0 sam        (501) staff       (20)    51373 2024-03-20 16:15:10.000000 SnakesInSpace-0.0.9/snisp/fleet.py
+-rw-r--r--   0 sam        (501) staff       (20)    25389 2024-03-20 15:05:01.000000 SnakesInSpace-0.0.9/snisp/markets.py
+-rw-r--r--   0 sam        (501) staff       (20)     8978 2024-03-20 15:02:32.000000 SnakesInSpace-0.0.9/snisp/shipyards.py
+-rw-r--r--   0 sam        (501) staff       (20)     4222 2024-03-20 16:12:02.000000 SnakesInSpace-0.0.9/snisp/systems.py
+-rw-r--r--   0 sam        (501) staff       (20)     3853 2024-03-20 14:56:28.000000 SnakesInSpace-0.0.9/snisp/tail.py
+-rw-r--r--   0 sam        (501) staff       (20)    17791 2024-03-20 16:12:02.000000 SnakesInSpace-0.0.9/snisp/utils.py
+-rw-r--r--   0 sam        (501) staff       (20)    29705 2024-03-21 14:22:42.000000 SnakesInSpace-0.0.9/snisp/waypoints.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-21 14:23:48.817618 SnakesInSpace-0.0.9/tests/
+-rw-r--r--   0 sam        (501) staff       (20)       43 2024-03-11 03:12:10.000000 SnakesInSpace-0.0.9/tests/README.md
+-rw-r--r--   0 sam        (501) staff       (20)     1598 2024-03-11 03:12:10.000000 SnakesInSpace-0.0.9/tests/__init__.py
+drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-21 14:23:48.830756 SnakesInSpace-0.0.9/tests/data/
+-rw-r--r--   0 sam        (501) staff       (20)      199 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/agent_data.json
+-rw-r--r--   0 sam        (501) staff       (20)      905 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/chart.json
+-rw-r--r--   0 sam        (501) staff       (20)      215 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/construction_site.json
+-rw-r--r--   0 sam        (501) staff       (20)      627 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/contract.json
+-rw-r--r--   0 sam        (501) staff       (20)      860 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/contract_delivery.json
+-rw-r--r--   0 sam        (501) staff       (20)     1273 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/contracts.json
+-rw-r--r--   0 sam        (501) staff       (20)      602 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/dock.json
+-rw-r--r--   0 sam        (501) staff       (20)      543 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/extraction.json
+-rw-r--r--   0 sam        (501) staff       (20)      281 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/faction.json
+-rw-r--r--   0 sam        (501) staff       (20)      381 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/factions.json
+-rw-r--r--   0 sam        (501) staff       (20)     6266 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fleet_list.json
+-rw-r--r--   0 sam        (501) staff       (20)     6266 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fleet_list_drones.json
+-rw-r--r--   0 sam        (501) staff       (20)     6270 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fleet_list_freighters.json
+-rw-r--r--   0 sam        (501) staff       (20)     6271 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fleet_list_mining_drones.json
+-rw-r--r--   0 sam        (501) staff       (20)     6266 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fleet_list_probes.json
+-rw-r--r--   0 sam        (501) staff       (20)     6272 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fleet_list_ships.json
+-rw-r--r--   0 sam        (501) staff       (20)     6270 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fleet_list_shuttles.json
+-rw-r--r--   0 sam        (501) staff       (20)     6266 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fleet_list_siphon_drones.json
+-rw-r--r--   0 sam        (501) staff       (20)     2392 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/fuel_stations.json
+-rw-r--r--   0 sam        (501) staff       (20)     1429 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/market.json
+-rw-r--r--   0 sam        (501) staff       (20)     1429 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/market_data.json
+-rw-r--r--   0 sam        (501) staff       (20)     3096 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/mining_drone.json
+-rw-r--r--   0 sam        (501) staff       (20)     1240 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/mount.json
+-rw-r--r--   0 sam        (501) staff       (20)      780 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/navigate.json
+-rw-r--r--   0 sam        (501) staff       (20)      604 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/orbit.json
+-rw-r--r--   0 sam        (501) staff       (20)      787 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/purchase.json
+-rw-r--r--   0 sam        (501) staff       (20)      583 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/refine.json
+-rw-r--r--   0 sam        (501) staff       (20)      619 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/refuel.json
+-rw-r--r--   0 sam        (501) staff       (20)     2468 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/scan.json
+-rw-r--r--   0 sam        (501) staff       (20)     2468 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/scan_ships.json
+-rw-r--r--   0 sam        (501) staff       (20)      790 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/scan_waypoints.json
+-rw-r--r--   0 sam        (501) staff       (20)      738 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/sell.json
+-rw-r--r--   0 sam        (501) staff       (20)     3436 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/ship_info.json
+-rw-r--r--   0 sam        (501) staff       (20)     3514 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/ship_purchase.json
+-rw-r--r--   0 sam        (501) staff       (20)     2345 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/shipyards.json
+-rw-r--r--   0 sam        (501) staff       (20)      539 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/siphon.json
+-rw-r--r--   0 sam        (501) staff       (20)     3090 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/siphon_drone.json
+-rw-r--r--   0 sam        (501) staff       (20)      495 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/supply_construction_site.json
+-rw-r--r--   0 sam        (501) staff       (20)     1163 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/survey.json
+-rw-r--r--   0 sam        (501) staff       (20)      439 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/system.json
+-rw-r--r--   0 sam        (501) staff       (20)      376 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/system_scan.json
+-rw-r--r--   0 sam        (501) staff       (20)     1043 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/systems.json
+-rw-r--r--   0 sam        (501) staff       (20)      252 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/transfer.json
+-rw-r--r--   0 sam        (501) staff       (20)      543 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/update_nav.json
+-rw-r--r--   0 sam        (501) staff       (20)      761 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/warp.json
+-rw-r--r--   0 sam        (501) staff       (20)      701 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/waypoint.json
+-rw-r--r--   0 sam        (501) staff       (20)     2534 2024-03-20 20:06:45.000000 SnakesInSpace-0.0.9/tests/data/waypoints.json
+-rw-r--r--   0 sam        (501) staff       (20)      892 2024-03-11 15:28:42.000000 SnakesInSpace-0.0.9/tests/test_agent.py
+-rw-r--r--   0 sam        (501) staff       (20)     2186 2024-03-11 15:28:54.000000 SnakesInSpace-0.0.9/tests/test_cache.py
+-rw-r--r--   0 sam        (501) staff       (20)     1982 2024-03-11 15:29:20.000000 SnakesInSpace-0.0.9/tests/test_client.py
+-rw-r--r--   0 sam        (501) staff       (20)    17108 2024-03-11 15:32:30.000000 SnakesInSpace-0.0.9/tests/test_contract.py
+-rw-r--r--   0 sam        (501) staff       (20)     1665 2024-03-11 15:32:21.000000 SnakesInSpace-0.0.9/tests/test_factions.py
+-rw-r--r--   0 sam        (501) staff       (20)   153665 2024-03-20 16:15:10.000000 SnakesInSpace-0.0.9/tests/test_fleet.py
+-rw-r--r--   0 sam        (501) staff       (20)    65129 2024-03-20 16:12:02.000000 SnakesInSpace-0.0.9/tests/test_markets.py
+-rw-r--r--   0 sam        (501) staff       (20)    20202 2024-03-11 15:31:02.000000 SnakesInSpace-0.0.9/tests/test_shipyards.py
+-rw-r--r--   0 sam        (501) staff       (20)     5063 2024-03-11 15:31:17.000000 SnakesInSpace-0.0.9/tests/test_systems.py
+-rw-r--r--   0 sam        (501) staff       (20)    44664 2024-03-21 14:22:42.000000 SnakesInSpace-0.0.9/tests/test_waypoints.py
```

### Comparing `SnakesInSpace-0.0.8/.gitignore` & `SnakesInSpace-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/LICENSE` & `SnakesInSpace-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/PKG-INFO` & `SnakesInSpace-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SnakesInSpace
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for the SpaceTraders game
 Author-email: Samuel Woodward <sam@woodward.fyi>
 Project-URL: Homepage, https://github.com/PyWoody/SnakesInSpace
 Keywords: SpaceTraders
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -1289,24 +1289,24 @@
 </details>
 
 <details>
 <summary>Construction Sites</summary>
 
 Select `Waypoints` will need construction materials delivered to them before they'll function correctly. Currently, all `JumpGate`s  in new Systems will need to be completed before you'll be able to use them to `jump` between Systems.
 
-You can see the required materials by calling `.data` on the `ConstructionSite`.
+The `ConstructionSite` will list the required materials in its `.materials`.
 
 ```python3
 >>> ship = next(iter(agent.fleet))
 >>> construction_sites = list(ship.waypoints.construction_sites())
->>> all(construction_site.is_under_construction for construction_site in construction_sites)
+>>> all(not construction_site.is_complete for construction_site in construction_sites)
 True
->>> construction_sites[0].data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
->>> jump_gate = ship.waypoints.get(waypoint_symbol=construction_site.symbol)
+>>> construction_sites[0]
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> jump_gate = ship.waypoints.get(waypoint_symbol=construction_sites[0].symbol)
 >>> jump_gate
 JumpGate({'systemSymbol': 'X1-CC27', 'symbol': 'X1-CC27-I56', 'type': 'JUMP_GATE', 'x': -335, 'y': 298, 'orbitals': [], 'traits': [{'symbol': 'MARKETPLACE', 'name': 'Marketplace', 'description': 'A thriving center of commerce where traders from across the galaxy gather to buy, sell, and exchange goods.'}], 'modifiers': [], 'chart': {'submittedBy': 'COSMIC', 'submittedOn': '2024-03-10T02:51:05.063Z'}, 'faction': {'symbol': 'COSMIC'}, 'isUnderConstruction': True})
 >>> jump_gate.is_under_construction
 True
 >>> jump_gate.symbol == construction_sites[0].symbol
 True
 ```
@@ -1314,22 +1314,22 @@
 This particular `JumpGate` won't become functional until 4,000 Units of `FAB_MATS` and 1,200 Units of `ADVANCED_CIRCUITRY` has been delivered to it.
 
 You can supply materials to a `ConstructionSite` in much the same way as you can deliver materials to a `Contract`. Diffferences being, a `ConstructionSite` uses `.supply` instead of `.deliver` and a `ConstructionSite` requires kwargs of `ship`, `trade_symbol`, and `units`.
 
 ```python3
 >>> ship = next(iter(agent.fleet))
 >>> construction_site = next(iter(ship.waypoints.construction_sites()))
->>> construction_site.data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> construction_site
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
 >>> ship.autopilot(construction_site)
 >>> ship.cargo.inventory
 [Inventory({'symbol': 'FAB_MATS', 'name': 'Fab Mats', 'description': 'DESCRIPTION', 'units': 40})]
 >>> construction_site.supply(ship=ship, trade_symbol='FAB_MATS', units=40)
->>> construction_site.data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 40}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> construction_site
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 40}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
 >>> ship.cargo
 Cargo({'capacity': 40, 'units': 0, 'inventory': []})
 ```
 
 Once all of the materials have been supplied to the `ConstructionSite`, it will no longer be returned by `ship.waypoints.construction_sites()` as it is no longer `.is_under_construction`.
 </details>
```

### Comparing `SnakesInSpace-0.0.8/README.md` & `SnakesInSpace-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1274,24 +1274,24 @@
 </details>
 
 <details>
 <summary>Construction Sites</summary>
 
 Select `Waypoints` will need construction materials delivered to them before they'll function correctly. Currently, all `JumpGate`s  in new Systems will need to be completed before you'll be able to use them to `jump` between Systems.
 
-You can see the required materials by calling `.data` on the `ConstructionSite`.
+The `ConstructionSite` will list the required materials in its `.materials`.
 
 ```python3
 >>> ship = next(iter(agent.fleet))
 >>> construction_sites = list(ship.waypoints.construction_sites())
->>> all(construction_site.is_under_construction for construction_site in construction_sites)
+>>> all(not construction_site.is_complete for construction_site in construction_sites)
 True
->>> construction_sites[0].data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
->>> jump_gate = ship.waypoints.get(waypoint_symbol=construction_site.symbol)
+>>> construction_sites[0]
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> jump_gate = ship.waypoints.get(waypoint_symbol=construction_sites[0].symbol)
 >>> jump_gate
 JumpGate({'systemSymbol': 'X1-CC27', 'symbol': 'X1-CC27-I56', 'type': 'JUMP_GATE', 'x': -335, 'y': 298, 'orbitals': [], 'traits': [{'symbol': 'MARKETPLACE', 'name': 'Marketplace', 'description': 'A thriving center of commerce where traders from across the galaxy gather to buy, sell, and exchange goods.'}], 'modifiers': [], 'chart': {'submittedBy': 'COSMIC', 'submittedOn': '2024-03-10T02:51:05.063Z'}, 'faction': {'symbol': 'COSMIC'}, 'isUnderConstruction': True})
 >>> jump_gate.is_under_construction
 True
 >>> jump_gate.symbol == construction_sites[0].symbol
 True
 ```
@@ -1299,22 +1299,22 @@
 This particular `JumpGate` won't become functional until 4,000 Units of `FAB_MATS` and 1,200 Units of `ADVANCED_CIRCUITRY` has been delivered to it.
 
 You can supply materials to a `ConstructionSite` in much the same way as you can deliver materials to a `Contract`. Diffferences being, a `ConstructionSite` uses `.supply` instead of `.deliver` and a `ConstructionSite` requires kwargs of `ship`, `trade_symbol`, and `units`.
 
 ```python3
 >>> ship = next(iter(agent.fleet))
 >>> construction_site = next(iter(ship.waypoints.construction_sites()))
->>> construction_site.data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> construction_site
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
 >>> ship.autopilot(construction_site)
 >>> ship.cargo.inventory
 [Inventory({'symbol': 'FAB_MATS', 'name': 'Fab Mats', 'description': 'DESCRIPTION', 'units': 40})]
 >>> construction_site.supply(ship=ship, trade_symbol='FAB_MATS', units=40)
->>> construction_site.data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 40}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> construction_site
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 40}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
 >>> ship.cargo
 Cargo({'capacity': 40, 'units': 0, 'inventory': []})
 ```
 
 Once all of the materials have been supplied to the `ConstructionSite`, it will no longer be returned by `ship.waypoints.construction_sites()` as it is no longer `.is_under_construction`.
 </details>
```

### Comparing `SnakesInSpace-0.0.8/SnakesInSpace.egg-info/PKG-INFO` & `SnakesInSpace-0.0.9/SnakesInSpace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SnakesInSpace
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for the SpaceTraders game
 Author-email: Samuel Woodward <sam@woodward.fyi>
 Project-URL: Homepage, https://github.com/PyWoody/SnakesInSpace
 Keywords: SpaceTraders
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -1289,24 +1289,24 @@
 </details>
 
 <details>
 <summary>Construction Sites</summary>
 
 Select `Waypoints` will need construction materials delivered to them before they'll function correctly. Currently, all `JumpGate`s  in new Systems will need to be completed before you'll be able to use them to `jump` between Systems.
 
-You can see the required materials by calling `.data` on the `ConstructionSite`.
+The `ConstructionSite` will list the required materials in its `.materials`.
 
 ```python3
 >>> ship = next(iter(agent.fleet))
 >>> construction_sites = list(ship.waypoints.construction_sites())
->>> all(construction_site.is_under_construction for construction_site in construction_sites)
+>>> all(not construction_site.is_complete for construction_site in construction_sites)
 True
->>> construction_sites[0].data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
->>> jump_gate = ship.waypoints.get(waypoint_symbol=construction_site.symbol)
+>>> construction_sites[0]
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> jump_gate = ship.waypoints.get(waypoint_symbol=construction_sites[0].symbol)
 >>> jump_gate
 JumpGate({'systemSymbol': 'X1-CC27', 'symbol': 'X1-CC27-I56', 'type': 'JUMP_GATE', 'x': -335, 'y': 298, 'orbitals': [], 'traits': [{'symbol': 'MARKETPLACE', 'name': 'Marketplace', 'description': 'A thriving center of commerce where traders from across the galaxy gather to buy, sell, and exchange goods.'}], 'modifiers': [], 'chart': {'submittedBy': 'COSMIC', 'submittedOn': '2024-03-10T02:51:05.063Z'}, 'faction': {'symbol': 'COSMIC'}, 'isUnderConstruction': True})
 >>> jump_gate.is_under_construction
 True
 >>> jump_gate.symbol == construction_sites[0].symbol
 True
 ```
@@ -1314,22 +1314,22 @@
 This particular `JumpGate` won't become functional until 4,000 Units of `FAB_MATS` and 1,200 Units of `ADVANCED_CIRCUITRY` has been delivered to it.
 
 You can supply materials to a `ConstructionSite` in much the same way as you can deliver materials to a `Contract`. Diffferences being, a `ConstructionSite` uses `.supply` instead of `.deliver` and a `ConstructionSite` requires kwargs of `ship`, `trade_symbol`, and `units`.
 
 ```python3
 >>> ship = next(iter(agent.fleet))
 >>> construction_site = next(iter(ship.waypoints.construction_sites()))
->>> construction_site.data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> construction_site
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 0}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
 >>> ship.autopilot(construction_site)
 >>> ship.cargo.inventory
 [Inventory({'symbol': 'FAB_MATS', 'name': 'Fab Mats', 'description': 'DESCRIPTION', 'units': 40})]
 >>> construction_site.supply(ship=ship, trade_symbol='FAB_MATS', units=40)
->>> construction_site.data
-ConstructionSiteData({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 40}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
+>>> construction_site
+ConstructionSite({'symbol': 'X1-CC27-I56', 'materials': [{'tradeSymbol': 'FAB_MATS', 'required': 4000, 'fulfilled': 40}, {'tradeSymbol': 'ADVANCED_CIRCUITRY', 'required': 1200, 'fulfilled': 0}, {'tradeSymbol': 'QUANTUM_STABILIZERS', 'required': 1, 'fulfilled': 1}], 'isComplete': False, 'systemSymbol': 'X1-CC27'})
 >>> ship.cargo
 Cargo({'capacity': 40, 'units': 0, 'inventory': []})
 ```
 
 Once all of the materials have been supplied to the `ConstructionSite`, it will no longer be returned by `ship.waypoints.construction_sites()` as it is no longer `.is_under_construction`.
 </details>
```

### Comparing `SnakesInSpace-0.0.8/SnakesInSpace.egg-info/SOURCES.txt` & `SnakesInSpace-0.0.9/SnakesInSpace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/pyproject.toml` & `SnakesInSpace-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 keywords = ["SpaceTraders"]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "0.0.8"
+version = "0.0.9"
 dependencies = ["httpx"]
 
 [project.urls]
 Homepage = "https://github.com/PyWoody/SnakesInSpace"
 
 [tool.setuptools.packages.find]
 exclude = ["recipes"]
```

### Comparing `SnakesInSpace-0.0.8/recipes/mine_asteroids.py` & `SnakesInSpace-0.0.9/recipes/mine_asteroids.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/recipes/probe_markets.py` & `SnakesInSpace-0.0.9/recipes/probe_markets.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/__main__.py` & `SnakesInSpace-0.0.9/snisp/__main__.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/agent.py` & `SnakesInSpace-0.0.9/snisp/agent.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/cache.py` & `SnakesInSpace-0.0.9/snisp/cache.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/client.py` & `SnakesInSpace-0.0.9/snisp/client.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/contracts.py` & `SnakesInSpace-0.0.9/snisp/contracts.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/database.py` & `SnakesInSpace-0.0.9/snisp/database.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/decorators.py` & `SnakesInSpace-0.0.9/snisp/decorators.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/exceptions.py` & `SnakesInSpace-0.0.9/snisp/exceptions.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/factions.py` & `SnakesInSpace-0.0.9/snisp/factions.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/fleet.py` & `SnakesInSpace-0.0.9/snisp/fleet.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/markets.py` & `SnakesInSpace-0.0.9/snisp/markets.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/shipyards.py` & `SnakesInSpace-0.0.9/snisp/shipyards.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/systems.py` & `SnakesInSpace-0.0.9/snisp/systems.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/tail.py` & `SnakesInSpace-0.0.9/snisp/tail.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/utils.py` & `SnakesInSpace-0.0.9/snisp/utils.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/snisp/waypoints.py` & `SnakesInSpace-0.0.9/snisp/waypoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,19 +322,19 @@
 
         Kwargs:
             system_symbol: System to search. Default is None for current System
 
         Yields:
             ConstructionSite
         """
-        for construction_site in self(
+        for waypoint in self(
             system_symbol=system_symbol
         ):
-            if construction_site.is_under_construction:
-                yield ConstructionSite(self.agent, construction_site.to_dict())
+            if waypoint.is_under_construction:
+                yield ConstructionSite.get(self.agent, waypoint)
 
     def shipyards(self, *, system_symbol=None):
         """
         Convenience method for finding Shipyards
 
         Kwargs:
             system_symbol: System to search. Default is None for current System
@@ -664,24 +664,56 @@
 
 class ConstructionSite(utils.AbstractJSONItem):
 
     def __init__(self, agent, waypoint):
         self.agent = agent
         self._data = waypoint
 
-    @property
-    def data(self):
+    @classmethod
+    @retry()
+    def get(cls, agent, waypoint):
+        """
+        Class method that creates a ConstructionSite instance from a Waypiont
+        Useful for when going from JumpGate Waypoint type to 
+        a ConstrutionSite type, for instance
+
+        Args:
+            cls: Automatically supplied by classmethod
+            agent: Your Agent
+            waypoint: The Waypoint to generate the ConstructionSite from
+
+        Returns:
+            ConstructionSite
+        """
+        response = agent.client.get(
+            f'/systems/{waypoint.system_symbol}/'
+            f'waypoints/{waypoint.symbol}/construction'
+        )
+        data = response.json()['data']
+        data['systemSymbol'] = waypoint.system_symbol
+        data['symbol'] = waypoint.symbol
+        return cls(agent, data)
+
+    @retry()
+    def refresh(self):
+        """
+        Returns a new ConstructionSite class object of the
+        current ConstructionSite and its current status
+
+        Returns:
+            A new ConstructionSite instance from self
+        """
         response = self.agent.client.get(
             f'/systems/{self.system_symbol}/waypoints/'
             f'{self.symbol}/construction'
         )
         data = response.json()['data']
         data['systemSymbol'] = self.system_symbol
         data['symbol'] = self.symbol
-        return ConstructionSiteData(self.agent, data)
+        return ConstructionSite(self.agent, data)
 
     @retry()
     @transit
     @docked
     def supply(
         self,
         *,
@@ -720,31 +752,14 @@
             f'{ship.registration.role}: {ship.symbol} | '
             f'Supplied {units:,} units of '
             f'{trade_symbol} to {self.symbol}'
         )
         return data
 
 
-class ConstructionSiteData(utils.AbstractJSONItem):
-
-    def __init__(self, agent, data):
-        self.agent = agent
-        self._data = data
-
-    def refresh(self):
-        response = self.agent.client.get(
-            f'/systems/{self.system_symbol}/waypoints/'
-            f'{self.symbol}/construction'
-        )
-        data = response.json()['data']
-        data['systemSymbol'] = self.system_symbol
-        data['symbol'] = self.symbol
-        return ConstructionSiteData(self.agent, data)
-
-
 # NOTE: These can be convient for isinstance checking
 
 
 class Planet(utils.AbstractJSONItem):
 
     def __init__(self, agent, planet):
         self.agent = agent
```

### Comparing `SnakesInSpace-0.0.8/tests/__init__.py` & `SnakesInSpace-0.0.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/chart.json` & `SnakesInSpace-0.0.9/tests/data/chart.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/contract.json` & `SnakesInSpace-0.0.9/tests/data/contract.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/contract_delivery.json` & `SnakesInSpace-0.0.9/tests/data/contract_delivery.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/contracts.json` & `SnakesInSpace-0.0.9/tests/data/contracts.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/dock.json` & `SnakesInSpace-0.0.9/tests/data/dock.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/extraction.json` & `SnakesInSpace-0.0.9/tests/data/extraction.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fleet_list.json` & `SnakesInSpace-0.0.9/tests/data/fleet_list.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fleet_list_drones.json` & `SnakesInSpace-0.0.9/tests/data/fleet_list_drones.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fleet_list_freighters.json` & `SnakesInSpace-0.0.9/tests/data/fleet_list_freighters.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fleet_list_mining_drones.json` & `SnakesInSpace-0.0.9/tests/data/fleet_list_mining_drones.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fleet_list_probes.json` & `SnakesInSpace-0.0.9/tests/data/fleet_list_probes.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fleet_list_ships.json` & `SnakesInSpace-0.0.9/tests/data/fleet_list_ships.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fleet_list_shuttles.json` & `SnakesInSpace-0.0.9/tests/data/fleet_list_shuttles.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fleet_list_siphon_drones.json` & `SnakesInSpace-0.0.9/tests/data/fleet_list_siphon_drones.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/fuel_stations.json` & `SnakesInSpace-0.0.9/tests/data/fuel_stations.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/market.json` & `SnakesInSpace-0.0.9/tests/data/market.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/market_data.json` & `SnakesInSpace-0.0.9/tests/data/market_data.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/mining_drone.json` & `SnakesInSpace-0.0.9/tests/data/mining_drone.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/mount.json` & `SnakesInSpace-0.0.9/tests/data/mount.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/navigate.json` & `SnakesInSpace-0.0.9/tests/data/navigate.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/orbit.json` & `SnakesInSpace-0.0.9/tests/data/orbit.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/purchase.json` & `SnakesInSpace-0.0.9/tests/data/purchase.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/refine.json` & `SnakesInSpace-0.0.9/tests/data/refine.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/refuel.json` & `SnakesInSpace-0.0.9/tests/data/refuel.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/scan.json` & `SnakesInSpace-0.0.9/tests/data/scan.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/scan_ships.json` & `SnakesInSpace-0.0.9/tests/data/scan_ships.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/scan_waypoints.json` & `SnakesInSpace-0.0.9/tests/data/scan_waypoints.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/sell.json` & `SnakesInSpace-0.0.9/tests/data/sell.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/ship_info.json` & `SnakesInSpace-0.0.9/tests/data/ship_info.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/ship_purchase.json` & `SnakesInSpace-0.0.9/tests/data/ship_purchase.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/shipyards.json` & `SnakesInSpace-0.0.9/tests/data/shipyards.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/siphon.json` & `SnakesInSpace-0.0.9/tests/data/siphon.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/siphon_drone.json` & `SnakesInSpace-0.0.9/tests/data/siphon_drone.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/survey.json` & `SnakesInSpace-0.0.9/tests/data/survey.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/systems.json` & `SnakesInSpace-0.0.9/tests/data/systems.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/update_nav.json` & `SnakesInSpace-0.0.9/tests/data/update_nav.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/warp.json` & `SnakesInSpace-0.0.9/tests/data/warp.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/waypoint.json` & `SnakesInSpace-0.0.9/tests/data/waypoint.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/data/waypoints.json` & `SnakesInSpace-0.0.9/tests/data/waypoints.json`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_agent.py` & `SnakesInSpace-0.0.9/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_cache.py` & `SnakesInSpace-0.0.9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_client.py` & `SnakesInSpace-0.0.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_contract.py` & `SnakesInSpace-0.0.9/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_factions.py` & `SnakesInSpace-0.0.9/tests/test_factions.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_fleet.py` & `SnakesInSpace-0.0.9/tests/test_fleet.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_markets.py` & `SnakesInSpace-0.0.9/tests/test_markets.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_shipyards.py` & `SnakesInSpace-0.0.9/tests/test_shipyards.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_systems.py` & `SnakesInSpace-0.0.9/tests/test_systems.py`

 * *Files identical despite different names*

### Comparing `SnakesInSpace-0.0.8/tests/test_waypoints.py` & `SnakesInSpace-0.0.9/tests/test_waypoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,22 +524,18 @@
             return_value=httpx.Response(200, json=construction_data)
         )
 
         construction_site = snisp.waypoints.ConstructionSite(
             self.agent, construction_data['data']
         )
 
-        assert construction_site.data.to_dict() == construction_site.to_dict()  # noqa: E501
-        assert construction_site.data.to_dict() == construction_data['data']
-
-        construction_site_data = snisp.waypoints.ConstructionSiteData(
-            self.agent, construction_data['data']
-        )
-        assert construction_site_data.refresh().to_dict() == construction_site_data.to_dict()  # noqa: E501
-        assert construction_site_data.refresh().to_dict() == construction_data['data']  # noqa: E501
+        assert construction_site.to_dict() == construction_data['data']
+        assert construction_site.refresh().to_dict() == construction_site.to_dict()  # noqa: E501
+        assert construction_site.refresh().refresh().to_dict() == construction_site.to_dict()  # noqa: E501
+        assert construction_site.refresh().to_dict() == construction_data['data']  # noqa: E501
 
     @pytest.mark.respx(base_url='https://api.spacetraders.io/v2')
     def test_refresh(self, respx_mock):
         ship_data = json.load(
             open(os.path.join(DATA_DIR, 'ship_info.json'), encoding='utf8')
         )
         ship_data['data']['nav']['systemSymbol'] = 'TEST-SYSTEM'
@@ -624,14 +620,28 @@
         waypoints_data = json.load(
             open(os.path.join(DATA_DIR, 'waypoints.json'), encoding='utf8')
         )
         waypoints_side_effect = WaypointsSideEffect(waypoints_data)
         waypoints_route = respx_mock.get('/systems/TEST-SYSTEM/waypoints')
         waypoints_route.side_effect = waypoints_side_effect
 
+        construction_data = json.load(
+            open(
+                os.path.join(DATA_DIR, 'construction_site.json'),
+                encoding='utf8'
+            )
+        )
+        for waypoint in waypoints_data['data']:
+            respx_mock.get(
+                '/systems/TEST-SYSTEM/waypoints/'
+                f'{waypoint["symbol"]}/construction'
+            ).mock(
+                return_value=httpx.Response(200, json=construction_data)
+            )
+
         ship = self.agent.fleet('TEST_SHIP_SYMBOL')
 
         with waypoints_side_effect as tmp:
             assert snisp.utils.ilen(
                 ship.waypoints.construction_sites()
             ) == 3
```

