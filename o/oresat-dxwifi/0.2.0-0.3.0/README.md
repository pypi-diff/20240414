# Comparing `tmp/oresat-dxwifi-0.2.0.tar.gz` & `tmp/oresat_dxwifi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-dxwifi-0.2.0.tar", last modified: Sat Apr 29 16:26:36 2023, max compression
+gzip compressed data, was "oresat_dxwifi-0.3.0.tar", last modified: Sun Apr 14 21:02:49 2024, max compression
```

## Comparing `oresat-dxwifi-0.2.0.tar` & `oresat_dxwifi-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:26:36.444094 oresat-dxwifi-0.2.0/oresat_dxwifi/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/oresat_dxwifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/oresat_dxwifi/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/oresat_dxwifi/data/
--rw-r--r--   0 runner    (1001) docker     (123)    82338 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/oresat_dxwifi/data/oresat_dxwifi.dcf
--rw-r--r--   0 runner    (1001) docker     (123)    82187 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/oresat_dxwifi/data/oresat_dxwifi.eds
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-29 16:26:36.000000 oresat-dxwifi-0.2.0/oresat_dxwifi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-29 16:26:21.000000 oresat-dxwifi-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-29 16:26:36.448094 oresat-dxwifi-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.603958 oresat_dxwifi-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.607958 oresat_dxwifi-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2384 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/build-deb.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.603958 oresat_dxwifi-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.607958 oresat_dxwifi-0.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   100917 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/docs/images/hgs-browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90640 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/docs/images/olaf-browser.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      176 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/kill-olaf
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat-dxwifi-software-server.service
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat-mon-iface.service
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat-vcan-iface.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.607958 oresat_dxwifi-0.3.0/oresat_dxwifi/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/camera/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/resources/temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/services/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/services/configs/camera_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/services/oresat_live.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/services/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/services/static/SMPTE_Color_Bars.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/templates/oresat_live.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.611958 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/configs/transmission_configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      661 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/startmonitor.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/transmission.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4381644 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/oresat_dxwifi/transmission/tx_module.so
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 21:02:49.000000 oresat_dxwifi-0.3.0/oresat_dxwifi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:02:49.619958 oresat_dxwifi-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      336 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/start-vcan
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-04-14 21:02:45.000000 oresat_dxwifi-0.3.0/startmonitor.sh
```

### Comparing `oresat-dxwifi-0.2.0/LICENSE` & `oresat_dxwifi-0.3.0/LICENSE`

 * *Files identical despite different names*

