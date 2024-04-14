# Comparing `tmp/gasflux-0.1.0.tar.gz` & `tmp/gasflux-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gasflux-0.1.0.tar", last modified: Sun Apr 14 13:41:10 2024, max compression
+gzip compressed data, was "gasflux-0.1.1.tar", last modified: Sun Apr 14 14:37:02 2024, max compression
```

## Comparing `gasflux-0.1.0.tar` & `gasflux-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 13:41:10.043107 gasflux-0.1.0/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    35184 2024-04-14 13:40:10.000000 gasflux-0.1.0/LICENSE
--rw-r--r--   0 a71546jm  (1001) a71546jm  (1001)     6456 2024-04-14 13:41:10.043107 gasflux-0.1.0/PKG-INFO
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     5013 2024-04-14 13:40:10.000000 gasflux-0.1.0/README.md
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      126 2024-04-14 13:40:33.000000 gasflux-0.1.0/dev-requirements.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2977 2024-04-14 13:40:10.000000 gasflux-0.1.0/pyproject.toml
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      351 2024-04-14 13:40:10.000000 gasflux-0.1.0/requirements.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)       38 2024-04-14 13:41:10.043107 gasflux-0.1.0/setup.cfg
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)       38 2024-04-03 14:12:12.000000 gasflux-0.1.0/setup.py
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 13:41:10.039107 gasflux-0.1.0/src/
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 13:41:10.039107 gasflux-0.1.0/src/gasflux/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      469 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/__init__.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1333 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/background.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     8575 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/cli.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2170 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/gas.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4688 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/interpolation.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2463 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/ml.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    13985 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/plotting.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4391 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/pre_processing.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    26870 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/processing.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    10582 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/processing_pipelines.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4250 2024-04-14 13:40:10.000000 gasflux-0.1.0/src/gasflux/reporting.py
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 13:41:10.043107 gasflux-0.1.0/src/gasflux.egg-info/
--rw-r--r--   0 a71546jm  (1001) a71546jm  (1001)     6456 2024-04-14 13:41:10.000000 gasflux-0.1.0/src/gasflux.egg-info/PKG-INFO
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      627 2024-04-14 13:41:10.000000 gasflux-0.1.0/src/gasflux.egg-info/SOURCES.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)        1 2024-04-14 13:41:10.000000 gasflux-0.1.0/src/gasflux.egg-info/dependency_links.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)       49 2024-04-14 13:41:10.000000 gasflux-0.1.0/src/gasflux.egg-info/entry_points.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      397 2024-04-14 13:41:10.000000 gasflux-0.1.0/src/gasflux.egg-info/requires.txt
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)        8 2024-04-14 13:41:10.000000 gasflux-0.1.0/src/gasflux.egg-info/top_level.txt
-drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 13:41:10.043107 gasflux-0.1.0/tests/
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     7500 2024-04-14 13:40:10.000000 gasflux-0.1.0/tests/test_processing.py
--rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2251 2024-04-14 13:40:10.000000 gasflux-0.1.0/tests/test_processing_pipelines.py
+drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 14:37:02.824042 gasflux-0.1.1/
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    35184 2024-04-14 13:40:10.000000 gasflux-0.1.1/LICENSE
+-rw-r--r--   0 a71546jm  (1001) a71546jm  (1001)     6493 2024-04-14 14:37:02.824042 gasflux-0.1.1/PKG-INFO
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     5013 2024-04-14 13:40:10.000000 gasflux-0.1.1/README.md
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      132 2024-04-14 14:28:45.000000 gasflux-0.1.1/dev-requirements.txt
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2977 2024-04-14 14:30:47.000000 gasflux-0.1.1/pyproject.toml
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      351 2024-04-14 13:40:10.000000 gasflux-0.1.1/requirements.txt
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)       38 2024-04-14 14:37:02.824042 gasflux-0.1.1/setup.cfg
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)       38 2024-04-03 14:12:12.000000 gasflux-0.1.1/setup.py
+drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 14:37:02.816042 gasflux-0.1.1/src/
+drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 14:37:02.820042 gasflux-0.1.1/src/gasflux/
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      469 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/__init__.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     1333 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/background.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     8544 2024-04-14 14:28:45.000000 gasflux-0.1.1/src/gasflux/cli.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2170 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/gas.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    14691 2024-04-14 14:28:45.000000 gasflux-0.1.1/src/gasflux/generate_test_data.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4688 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/interpolation.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2463 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/ml.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    13985 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/plotting.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4391 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/pre_processing.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    26870 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/processing.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)    10582 2024-04-14 13:40:10.000000 gasflux-0.1.1/src/gasflux/processing_pipelines.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     4246 2024-04-14 14:28:45.000000 gasflux-0.1.1/src/gasflux/reporting.py
+drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 14:37:02.820042 gasflux-0.1.1/src/gasflux.egg-info/
+-rw-r--r--   0 a71546jm  (1001) a71546jm  (1001)     6493 2024-04-14 14:37:02.000000 gasflux-0.1.1/src/gasflux.egg-info/PKG-INFO
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      661 2024-04-14 14:37:02.000000 gasflux-0.1.1/src/gasflux.egg-info/SOURCES.txt
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)        1 2024-04-14 14:37:02.000000 gasflux-0.1.1/src/gasflux.egg-info/dependency_links.txt
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)       49 2024-04-14 14:37:02.000000 gasflux-0.1.1/src/gasflux.egg-info/entry_points.txt
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)      403 2024-04-14 14:37:02.000000 gasflux-0.1.1/src/gasflux.egg-info/requires.txt
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)        8 2024-04-14 14:37:02.000000 gasflux-0.1.1/src/gasflux.egg-info/top_level.txt
+drwxrwxr-x   0 a71546jm  (1001) a71546jm  (1001)        0 2024-04-14 14:37:02.820042 gasflux-0.1.1/tests/
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     7565 2024-04-14 14:28:45.000000 gasflux-0.1.1/tests/test_processing.py
+-rw-rw-r--   0 a71546jm  (1001) a71546jm  (1001)     2291 2024-04-14 14:28:45.000000 gasflux-0.1.1/tests/test_processing_pipelines.py
```

### Comparing `gasflux-0.1.0/LICENSE` & `gasflux-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/PKG-INFO` & `gasflux-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasflux
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to calculate gas emissions fluxes from natural and anthropogenic sources
 Author-email: Jamie McQuilkin <jamie.mcquilkin@gmail.com>
 License: AGPL-3.0
 Project-URL: Homepage, https://gasflux.github.io
 Project-URL: Bug Tracker, https://github.com/gasflux/gasflux/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -34,14 +34,15 @@
 Requires-Dist: pip>23.3; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: safety; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Requires-Dist: vulture; extra == "dev"
 
 
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Tests](https://github.com/gasflux/gasflux/workflows/CI/badge.svg)](https://github.com/gasflux/gasflux/actions?query=workflow%3A%22CI%22)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![format - Black](https://img.shields.io/badge/format-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `gasflux-0.1.0/README.md` & `gasflux-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/pyproject.toml` & `gasflux-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gasflux"
-version = "0.1.0"
+version = "0.1.1"
 description = "A package to calculate gas emissions fluxes from natural and anthropogenic sources"
 authors = [{ name = "Jamie McQuilkin", email = "jamie.mcquilkin@gmail.com" }]
 license = { text = "AGPL-3.0" }
 readme = "README.md"
 requires-python = ">=3.9"
 
 dynamic = ["dependencies", "optional-dependencies"]
```

### Comparing `gasflux-0.1.0/src/gasflux/background.py` & `gasflux-0.1.1/src/gasflux/background.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/src/gasflux/cli.py` & `gasflux-0.1.1/src/gasflux/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         raise ValueError("Multiple config files found: {}".format(", ".join(str(file) for file in config_files)))
     else:
         raise FileNotFoundError("No config file found in the supplied path or its child folders")
 
 
 def process_command(data_path: str, config_path: str, test: bool):
     if test:
-        data_file = Path(__file__).parent.parent.parent / "tests" / "data" / "testdata.csv"
-        config_file = Path(__file__).parent.parent.parent / "tests" / "testconfig.yaml"
+        data_file = Path(__file__).parent / "testdata" / "testdata.csv"
+        config_file = Path(__file__).parent / "testdata" / "testconfig.yaml"
         process_main(data_file, config_file)
     else:
         dpath_obj = Path(data_path)
         if dpath_obj.is_dir():
             data_files = dpath_obj.rglob("*.csv")
             if config_path is None:
                 config_file = find_config_file(dpath_obj)
```

### Comparing `gasflux-0.1.0/src/gasflux/gas.py` & `gasflux-0.1.1/src/gasflux/gas.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/src/gasflux/interpolation.py` & `gasflux-0.1.1/src/gasflux/interpolation.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/src/gasflux/ml.py` & `gasflux-0.1.1/src/gasflux/ml.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/src/gasflux/plotting.py` & `gasflux-0.1.1/src/gasflux/plotting.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/src/gasflux/pre_processing.py` & `gasflux-0.1.1/src/gasflux/pre_processing.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/src/gasflux/processing.py` & `gasflux-0.1.1/src/gasflux/processing.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/src/gasflux/processing_pipelines.py` & `gasflux-0.1.1/src/gasflux/processing_pipelines.py`

 * *Files identical despite different names*

### Comparing `gasflux-0.1.0/src/gasflux/reporting.py` & `gasflux-0.1.1/src/gasflux/reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     wind_fig: go.Figure,
     background_fig: go.Figure,
     threed_fig: go.Figure,
     krig_fig: go.Figure,
     windrose_fig: go.Figure,
 ) -> str:
     """Generate a mass balance report."""
-    template_path = Path(__file__).parents[2] / "templates" / "mass_balance_template.html"
+    template_path = Path(__file__).parent / "templates" / "mass_balance_template.html"
 
     # Convert the figures to HTML
     plot_htmls = {}
     for name, fig in zip(
         ["3D", "krig", "windrose", "wind", "background"],
         [threed_fig, krig_fig, windrose_fig, wind_fig, background_fig],
         strict=False,
```

### Comparing `gasflux-0.1.0/src/gasflux.egg-info/PKG-INFO` & `gasflux-0.1.1/src/gasflux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gasflux
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to calculate gas emissions fluxes from natural and anthropogenic sources
 Author-email: Jamie McQuilkin <jamie.mcquilkin@gmail.com>
 License: AGPL-3.0
 Project-URL: Homepage, https://gasflux.github.io
 Project-URL: Bug Tracker, https://github.com/gasflux/gasflux/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -34,14 +34,15 @@
 Requires-Dist: pip>23.3; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: safety; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Requires-Dist: vulture; extra == "dev"
 
 
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Tests](https://github.com/gasflux/gasflux/workflows/CI/badge.svg)](https://github.com/gasflux/gasflux/actions?query=workflow%3A%22CI%22)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![format - Black](https://img.shields.io/badge/format-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `gasflux-0.1.0/src/gasflux.egg-info/SOURCES.txt` & `gasflux-0.1.1/src/gasflux.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 requirements.txt
 setup.py
 src/gasflux/__init__.py
 src/gasflux/background.py
 src/gasflux/cli.py
 src/gasflux/gas.py
+src/gasflux/generate_test_data.py
 src/gasflux/interpolation.py
 src/gasflux/ml.py
 src/gasflux/plotting.py
 src/gasflux/pre_processing.py
 src/gasflux/processing.py
 src/gasflux/processing_pipelines.py
 src/gasflux/reporting.py
```

### Comparing `gasflux-0.1.0/tests/test_processing.py` & `gasflux-0.1.1/tests/test_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import yaml
 from pathlib import Path
 import numpy as np
 from gasflux.processing import min_angular_displacement
 import pytest
 
 
-testdf = pd.read_csv(Path(__file__).parent / "data" / "testdata.csv")
-testconfig = yaml.safe_load(open(Path(__file__).parent / "testconfig.yaml"))
+testdf = pd.read_csv(Path(__file__).parents[1] / "src" / "gasflux" / "testdata" / "testdata.csv")
+testconfig = yaml.safe_load(open(Path(__file__).parents[1] / "src" / "gasflux" / "testdata" / "testconfig.yaml"))
 
 
 def load_cols(cols):
     return testdf[cols]
 
 
 def test_min_angular_diff_def():
```

### Comparing `gasflux-0.1.0/tests/test_processing_pipelines.py` & `gasflux-0.1.1/tests/test_processing_pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from pathlib import Path
 import pytest
 
 
 @pytest.fixture
 def setup_test_environment(tmp_path):
     """Prepare actual test data and configuration with a modified output directory."""
-    df_path = Path(__file__).parent / "data" / "testdata.csv"
-    config_path = Path(__file__).parent / "testconfig.yaml"
+    df_path = Path(__file__).parents[1] / "src" / "gasflux" / "testdata" / "testdata.csv"
+    config_path = Path(__file__).parents[1] / "src" / "gasflux" / "testdata" / "testconfig.yaml"
 
     with open(config_path) as f:
         config = yaml.safe_load(f)
     config["output_dir"] = str(tmp_path)
 
     temp_config_path = tmp_path / "temp_testconfig.yaml"
     with open(temp_config_path, "w") as f:
@@ -28,15 +28,15 @@
         temp_config = yaml.safe_load(f)
     output_dir = Path(temp_config["output_dir"]) / df_path.stem
     assert output_dir.exists(), "Output directory does not exist."
     processing_run_dirs = [d for d in output_dir.iterdir() if d.is_dir()]
     assert len(processing_run_dirs) > 0, "No processing run directory found."
     processing_run_dir = processing_run_dirs[0]
 
-    with open(Path(__file__).parent / "testconfig.yaml") as f:
+    with open(temp_config_path) as f:
         original_config = yaml.safe_load(f)
 
     for gas in original_config.get("gases", []):
         report_path = processing_run_dir / f"{df_path.stem}_{gas}_report.html"
         assert report_path.exists(), f"Report for {gas} does not exist."
 
     config_dump_path = processing_run_dir / f"{df_path.stem}_config.yaml"
```

