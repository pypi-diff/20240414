# Comparing `tmp/prometheus_pve_sd-3.2.7.tar.gz` & `tmp/prometheus_pve_sd-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_pve_sd-3.2.7.tar", max compression
+gzip compressed data, was "prometheus_pve_sd-3.2.8.tar", max compression
```

## Comparing `prometheus_pve_sd-3.2.7.tar` & `prometheus_pve_sd-3.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1123 2024-03-07 11:04:20.928104 prometheus_pve_sd-3.2.7/LICENSE
--rw-r--r--   0        0        0     2497 2024-03-07 11:04:20.928104 prometheus_pve_sd-3.2.7/README.md
--rw-r--r--   0        0        0        0 2024-03-07 11:04:22.260098 prometheus_pve_sd-3.2.7/prometheuspvesd/.drone.yml
--rw-r--r--   0        0        0       46 2024-03-07 11:04:45.104001 prometheus_pve_sd-3.2.7/prometheuspvesd/__init__.py
--rw-r--r--   0        0        0     6197 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/cli.py
--rw-r--r--   0        0        0     3981 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/client.py
--rw-r--r--   0        0        0     9929 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/config.py
--rw-r--r--   0        0        0     8123 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/discovery.py
--rw-r--r--   0        0        0      498 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/exception.py
--rw-r--r--   0        0        0     7685 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/logger.py
--rw-r--r--   0        0        0     1904 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/model.py
--rw-r--r--   0        0        0       30 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/__init__.py
--rw-r--r--   0        0        0      451 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/data/config.yml
--rw-r--r--   0        0        0       28 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/fixtures/__init__.py
--rw-r--r--   0        0        0    10561 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/fixtures/fixtures.py
--rw-r--r--   0        0        0     1366 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/conftest.py
--rw-r--r--   0        0        0     4861 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/test_cli.py
--rw-r--r--   0        0        0     1117 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/test_config.py
--rw-r--r--   0        0        0     3972 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/test_discovery.py
--rw-r--r--   0        0        0     1505 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/test_model.py
--rw-r--r--   0        0        0      900 2024-03-07 11:04:20.936104 prometheus_pve_sd-3.2.7/prometheuspvesd/utils.py
--rw-r--r--   0        0        0     3094 2024-03-07 11:04:45.100001 prometheus_pve_sd-3.2.7/pyproject.toml
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 prometheus_pve_sd-3.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1123 2024-04-14 09:46:59.460627 prometheus_pve_sd-3.2.8/LICENSE
+-rw-r--r--   0        0        0     2497 2024-04-14 09:46:59.460627 prometheus_pve_sd-3.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 09:47:00.236628 prometheus_pve_sd-3.2.8/prometheuspvesd/.drone.yml
+-rw-r--r--   0        0        0       46 2024-04-14 09:47:13.496636 prometheus_pve_sd-3.2.8/prometheuspvesd/__init__.py
+-rw-r--r--   0        0        0     6197 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/cli.py
+-rw-r--r--   0        0        0     3981 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/client.py
+-rw-r--r--   0        0        0     9929 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/config.py
+-rw-r--r--   0        0        0     8123 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/discovery.py
+-rw-r--r--   0        0        0      498 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/exception.py
+-rw-r--r--   0        0        0     7685 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/logger.py
+-rw-r--r--   0        0        0     1904 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/model.py
+-rw-r--r--   0        0        0       30 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/data/config.yml
+-rw-r--r--   0        0        0       28 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/fixtures/__init__.py
+-rw-r--r--   0        0        0    10561 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/fixtures/fixtures.py
+-rw-r--r--   0        0        0     1366 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/conftest.py
+-rw-r--r--   0        0        0     4861 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_cli.py
+-rw-r--r--   0        0        0     1117 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_config.py
+-rw-r--r--   0        0        0     3972 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_discovery.py
+-rw-r--r--   0        0        0     1505 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_model.py
+-rw-r--r--   0        0        0      900 2024-04-14 09:46:59.464627 prometheus_pve_sd-3.2.8/prometheuspvesd/utils.py
+-rw-r--r--   0        0        0     3094 2024-04-14 09:47:13.492636 prometheus_pve_sd-3.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 prometheus_pve_sd-3.2.8/PKG-INFO
```

### Comparing `prometheus_pve_sd-3.2.7/LICENSE` & `prometheus_pve_sd-3.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/README.md` & `prometheus_pve_sd-3.2.8/README.md`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/cli.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/client.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/client.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/config.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/config.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/discovery.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/discovery.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/logger.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/logger.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/model.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/model.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/test/fixtures/fixtures.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/test/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/conftest.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/test_cli.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/test_config.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/test_discovery.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/test/unit/test_model.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/test/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/prometheuspvesd/utils.py` & `prometheus_pve_sd-3.2.8/prometheuspvesd/utils.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_sd-3.2.7/pyproject.toml` & `prometheus_pve_sd-3.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 include = ["LICENSE"]
 keywords = ["prometheus", "sd", "pve", "metrics"]
 license = "MIT"
 name = "prometheus-pve-sd"
 packages = [{ include = "prometheuspvesd" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/prometheus-pve-sd/"
-version = "3.2.7"
+version = "3.2.8"
 
 [tool.poetry.dependencies]
 anyconfig = "0.14.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 environs = "11.0.0"
 jsonschema = "4.21.1"
@@ -43,18 +43,18 @@
 requests = "2.31.0"
 "ruamel.yaml" = "0.18.6"
 
 [tool.poetry.scripts]
 prometheus-pve-sd = "prometheuspvesd.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.3.1"
-pytest = "8.0.2"
-pytest-mock = "3.12.0"
-pytest-cov = "4.1.0"
+ruff = "0.3.5"
+pytest = "8.1.1"
+pytest-mock = "3.14.0"
+pytest-cov = "5.0.0"
 toml = "0.10.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "semver"
 vcs = "git"
```

### Comparing `prometheus_pve_sd-3.2.7/PKG-INFO` & `prometheus_pve_sd-3.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-sd
-Version: 3.2.7
+Version: 3.2.8
 Summary: Prometheus Service Discovery for Proxmox VE.
 Home-page: https://github.com/thegeeklab/prometheus-pve-sd/
 License: MIT
 Keywords: prometheus,sd,pve,metrics
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.8.0,<4.0.0
```

