# Comparing `tmp/openai_cost_logger-0.1.0.tar.gz` & `tmp/openai_cost_logger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_cost_logger-0.1.0.tar", last modified: Tue Apr  9 22:02:18 2024, max compression
+gzip compressed data, was "openai_cost_logger-0.2.0.tar", last modified: Sun Apr 14 21:03:51 2024, max compression
```

## Comparing `openai_cost_logger-0.1.0.tar` & `openai_cost_logger-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/openai_cost_logger/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 22:02:18.000000 openai_cost_logger-0.1.0/openai_cost_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:02:18.221767 openai_cost_logger-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 22:02:11.000000 openai_cost_logger-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:03:51.283762 openai_cost_logger-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-14 21:03:46.000000 openai_cost_logger-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-14 21:03:51.283762 openai_cost_logger-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-14 21:03:46.000000 openai_cost_logger-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:03:51.283762 openai_cost_logger-0.2.0/openai_cost_logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-14 21:03:46.000000 openai_cost_logger-0.2.0/openai_cost_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-14 21:03:46.000000 openai_cost_logger-0.2.0/openai_cost_logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-14 21:03:46.000000 openai_cost_logger-0.2.0/openai_cost_logger/openai_cost_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-14 21:03:46.000000 openai_cost_logger-0.2.0/openai_cost_logger/openai_cost_logger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-14 21:03:46.000000 openai_cost_logger-0.2.0/openai_cost_logger/openai_cost_logger_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:03:51.283762 openai_cost_logger-0.2.0/openai_cost_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-14 21:03:51.000000 openai_cost_logger-0.2.0/openai_cost_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-14 21:03:51.000000 openai_cost_logger-0.2.0/openai_cost_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:03:51.000000 openai_cost_logger-0.2.0/openai_cost_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-14 21:03:51.000000 openai_cost_logger-0.2.0/openai_cost_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 21:03:51.000000 openai_cost_logger-0.2.0/openai_cost_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:03:51.283762 openai_cost_logger-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-14 21:03:46.000000 openai_cost_logger-0.2.0/setup.py
```

### Comparing `openai_cost_logger-0.1.0/LICENSE` & `openai_cost_logger-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.1.0/PKG-INFO` & `openai_cost_logger-0.2.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: openai_cost_logger
-Version: 0.1.0
-Summary: OpenAI Cost Logger
-Home-page: https://github.com/drudilorenzo/openai-cost-tracker
-Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
-Author-email: lorenzodrudi11@gmail.com
-License: MIT
-Keywords: openai,cost,logger,tracker
-Platform: UNKNOWN
-Requires: openai
-Requires: pandas
-Requires: matplotlib
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 .. image:: https://img.shields.io/badge/chatGPT-74aa9c.svg?logo=openai
 .. image:: https://img.shields.io/pypi/pyversions/setuptools.svg
 
 ==================
 OpenAI Cost Logger
 ==================
 
@@ -38,16 +22,30 @@
       from openai_cost_logger.openai_cost_logger import OpenAICostLogger
 
 * See also the homepage on `PyPI <https://pypi.org/project/openai-cost-logger/>`_.
 * See the `demo file <https://github.com/drudilorenzo/track-openai-cost/blob/master/demo.ipynb>`_ for a usage example.
 
 Key Features:
 -------------
-* Track the cost of every request you make to OpenAI and save them in a csv file.
-* Visualize the cost of all the requests you have made.
+* Track the cost of every request you make and save them in a JSON file.
+* Choose the feature you want to track (prompt_tokens, completion_tokens, completion, prompt, etc.).
+* Check the cost of your requests filtering by model or strftime aggregation (see the docs).
 
 Endpoint supported:
 -------------------
 * Chat completion.
-* Every endpoint which response contains the field "*usage.prompt_tokens*" and "*usage.completion_tokens*".
+* Every response passed to *OpenAICostLogger* should contain the fields "*usage.prompt_tokens*" and "*usage.completion_tokens*".
+  This is the only strict requirement of the library, the way you call the OpenAI API is totally up to you. If needed, you can
+  find an easy example in the demo file.
 
+Viz examples:
+-------------
+.. image::images/viz_prints.png
+   :alt: Viz prints examples.
+   :align: center
+   :width: 500px
+
+.. image::images/strftime_agg.png
+   :alt: Strftime aggregation example.
+   :align: center
+   :width: 500px
```

### Comparing `openai_cost_logger-0.1.0/openai_cost_logger/constants.py` & `openai_cost_logger-0.2.0/openai_cost_logger/constants.py`

 * *Files identical despite different names*

### Comparing `openai_cost_logger-0.1.0/openai_cost_logger/openai_cost_logger_viz.py` & `openai_cost_logger-0.2.0/openai_cost_logger/openai_cost_logger_viz.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,122 @@
 import os
-import csv
+import json
+from datetime import datetime
 from typing import Dict
 from pathlib import Path
 import matplotlib.pyplot as plt
 from collections import defaultdict
 
 from openai_cost_logger.constants import DEFAULT_LOG_PATH
 
+"""Cost logger visualizer."""
 class OpenAICostLoggerViz:
     
     @staticmethod
     def get_total_cost(path: str = DEFAULT_LOG_PATH) -> float:
         """Return the total cost of all the logs in the directory.
 
         Args:
             log_folder (str, optional): Cost logs directory. Defaults to DEFAULT_LOG_PATH.
                                         This method reads all the files in the specified directory.
         Returns:
             float: the total cost.
         """
         cost = 0
         for filename in os.listdir(path):
-            with open(Path(path, filename), mode='r') as file:
-                csvreader = csv.reader(file)
-                next(csvreader)
-                for row in csvreader:
-                    cost += float(row[2])
+            if filename.endswith(".json"):
+                with open(Path(path, filename), mode='r') as file:
+                    data = json.load(file)
+                    cost += data["total_cost"]
         return cost
     
+    
     @staticmethod
     def print_total_cost(path: str = DEFAULT_LOG_PATH) -> None:
         """Print the total cost of all the logs in the directory.
 
         Args:
             log_folder (str, optional): Cost logs directory. Defaults to DEFAULT_LOG_PATH.
                                         This method reads all the files in the specified directory.
         """
-        
         print(f"Total cost: {round(OpenAICostLoggerViz.get_total_cost(path), 6)} (USD)")
-        
+    
+    
     @staticmethod
     def get_total_cost_by_model(path: str = DEFAULT_LOG_PATH) -> Dict[str, float]:
         """Return the total cost by model of all the logs in the directory.
 
         Args:
             log_folder (str, optional): Cost logs directory. Defaults to DEFAULT_LOG_PATH.
                                         This method reads all the files in the specified directory.
 
         Returns:
             Dict[str, float]: the total cost by model.
         """
         cost_by_model = defaultdict(float)
         for filename in os.listdir(path):
-            with open(Path(path, filename), mode='r') as file:
-                csvreader = csv.reader(file)
-                next(csvreader)
-                for row in csvreader:
-                    if row[1] not in cost_by_model:
-                        cost_by_model[row[1]] = 0
-                    cost_by_model[row[1]] += float(row[2])
+            if filename.endswith(".json"):
+                with open(Path(path, filename), mode='r') as file:
+                    data = json.load(file)
+                    if data["model"] not in cost_by_model:
+                        cost_by_model[data["model"]] = 0
+                    cost_by_model[data["model"]] += data["total_cost"]
         return cost_by_model
-    
+
+
     def print_total_cost_by_model(path: str = DEFAULT_LOG_PATH) -> None:
         """Print the total cost by model of all the logs in the directory.
 
         Args:
             log_folder (str, optional): Cost logs directory. Defaults to DEFAULT_LOG_PATH.
                                         This method reads all the files in the specified directory.
         """
         cost_by_model = OpenAICostLoggerViz.get_total_cost_by_model(path)
         for model, cost in cost_by_model.items():
             print(f"{model}: {round(cost, 6)} (USD)")
-        
+
+
     @staticmethod
-    def plot_cost_by_day(path: str = DEFAULT_LOG_PATH, last_n_days: int = None) -> None:
-        """Plot the cost by day of all the logs in the directory.
+    def plot_cost_by_strftime(path: str = DEFAULT_LOG_PATH, strftime_aggregator: str = "%Y-%m-%d", last_n_days: int = None) -> None:
+        """Plot the cost by day of all the logs in the directory aggregated using strftime_aggregator.
 
         Args:
             path (str, optional): Cost logs directory. Defaults to DEFAULT_LOG_PATH.
                                   This method reads all the files in the specified directory.
             last_n_days (int, optional): The number of last days to plot. Defaults to None.
         """
-        cost_by_day = defaultdict(float)
+        cost_by_aggregation_key = defaultdict(float)
         for filename in os.listdir(path):
-            with open(Path(path, filename), mode='r') as file:
-                csvreader = csv.reader(file)
-                next(csvreader)
-                for row in csvreader:
-                    day = filename.split("_")[2]
-                    cost_by_day[day] += float(row[2])
+            if filename.endswith(".json"):
+                with open(Path(path, filename), mode='r') as file:
+                    data = json.load(file)
+                    creation_datetime = datetime.strptime(data["creation_datetime"], "%Y-%m-%d %H:%M:%S")
+                    aggregation_key = creation_datetime.strftime(strftime_aggregator)
+                    cost_by_aggregation_key[aggregation_key] += data["total_cost"]
         
-        cost_by_day = dict(sorted(cost_by_day.items(), key=lambda x: x[0]))
+        cost_by_aggregation_key = dict(sorted(cost_by_aggregation_key.items(), key=lambda x: x[0]))
         if last_n_days:
-            cost_by_day = dict(list(cost_by_day.items())[-last_n_days:])
+            cost_by_aggregation_key = dict(list(cost_by_aggregation_key.items())[-last_n_days:])
         
-        plt.bar(cost_by_day.keys(), cost_by_day.values(), width=0.5)
+        plt.bar(cost_by_aggregation_key.keys(), cost_by_aggregation_key.values(), width=0.5)
+        plt.xticks(rotation=30, fontsize=8)
         plt.xlabel('Day')
         plt.ylabel('Cost [$]')
         plt.title('Cost by day')
-        plt.show()
+        plt.tight_layout()
+        plt.show()
+        
+        
+    @staticmethod
+    def plot_cost_by_day(path: str = DEFAULT_LOG_PATH, last_n_days: int = None) -> None:
+        """Plot the cost by day of all the logs in the directory.
+
+        Args:
+            path (str, optional): Cost logs directory. Defaults to DEFAULT_LOG_PATH.
+                                  This method reads all the files in the specified directory.
+            last_n_days (int, optional): The number of last days to plot. Defaults to None.
+        """
+        OpenAICostLoggerViz.plot_cost_by_strftime(
+            path=path,
+            strftime_aggregator="%Y-%m-%d", 
+            last_n_days=last_n_days
+        )
```

### Comparing `openai_cost_logger-0.1.0/openai_cost_logger.egg-info/PKG-INFO` & `openai_cost_logger-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openai-cost-logger
-Version: 0.1.0
+Name: openai_cost_logger
+Version: 0.2.0
 Summary: OpenAI Cost Logger
 Home-page: https://github.com/drudilorenzo/openai-cost-tracker
 Author: Lorenzo Drudi | Mikolaj Boronski | Ivan Zakazov
 Author-email: lorenzodrudi11@gmail.com
 License: MIT
 Keywords: openai,cost,logger,tracker
 Platform: UNKNOWN
@@ -38,16 +38,32 @@
       from openai_cost_logger.openai_cost_logger import OpenAICostLogger
 
 * See also the homepage on `PyPI <https://pypi.org/project/openai-cost-logger/>`_.
 * See the `demo file <https://github.com/drudilorenzo/track-openai-cost/blob/master/demo.ipynb>`_ for a usage example.
 
 Key Features:
 -------------
-* Track the cost of every request you make to OpenAI and save them in a csv file.
-* Visualize the cost of all the requests you have made.
+* Track the cost of every request you make and save them in a JSON file.
+* Choose the feature you want to track (prompt_tokens, completion_tokens, completion, prompt, etc.).
+* Check the cost of your requests filtering by model or strftime aggregation (see the docs).
 
 Endpoint supported:
 -------------------
 * Chat completion.
-* Every endpoint which response contains the field "*usage.prompt_tokens*" and "*usage.completion_tokens*".
+* Every response passed to *OpenAICostLogger* should contain the fields "*usage.prompt_tokens*" and "*usage.completion_tokens*".
+  This is the only strict requirement of the library, the way you call the OpenAI API is totally up to you. If needed, you can
+  find an easy example in the demo file.
+
+Viz examples:
+-------------
+.. image::images/viz_prints.png
+   :alt: Viz prints examples.
+   :align: center
+   :width: 500px
+
+.. image::images/strftime_agg.png
+   :alt: Strftime aggregation example.
+   :align: center
+   :width: 500px   
+
```

### Comparing `openai_cost_logger-0.1.0/setup.py` & `openai_cost_logger-0.2.0/setup.py`

 * *Files identical despite different names*

