# Comparing `tmp/proma-0.0.1.tar.gz` & `tmp/proma-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proma-0.0.1.tar", max compression
+gzip compressed data, was "proma-0.0.2.tar", max compression
```

## Comparing `proma-0.0.1.tar` & `proma-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1070 2024-04-11 16:38:12.991778 proma-0.0.1/LICENSE
--rw-r--r--   0        0        0      575 2024-04-11 17:08:28.793851 proma-0.0.1/README.rst
--rw-r--r--   0        0        0        0 2024-03-20 22:05:07.102573 proma-0.0.1/proma/__init__.py
--rw-r--r--   0        0        0        0 2022-04-05 16:05:17.780922 proma-0.0.1/proma/draw/__init__.py
--rw-r--r--   0        0        0      210 2024-03-20 22:06:18.786261 proma-0.0.1/proma/draw/base/__init__.py
--rw-r--r--   0        0        0      773 2024-04-11 17:09:58.882121 proma-0.0.1/proma/draw/base/consts.py
--rw-r--r--   0        0        0     7384 2024-04-11 17:09:59.048739 proma-0.0.1/proma/draw/base/dimension.py
--rw-r--r--   0        0        0     1261 2024-03-20 21:35:36.543550 proma-0.0.1/proma/draw/base/listener.py
--rw-r--r--   0        0        0      939 2024-03-20 21:35:14.730798 proma-0.0.1/proma/draw/base/margin.py
--rw-r--r--   0        0        0      945 2024-03-20 21:34:59.609054 proma-0.0.1/proma/draw/base/padding.py
--rw-r--r--   0        0        0     2473 2024-04-11 17:09:58.963348 proma-0.0.1/proma/draw/base/position.py
--rw-r--r--   0        0        0     2625 2024-04-11 17:09:59.130040 proma-0.0.1/proma/draw/base/size.py
--rw-r--r--   0        0        0      391 2024-03-20 21:33:22.558570 proma-0.0.1/proma/draw/shapes/__init__.py
--rw-r--r--   0        0        0     2280 2024-04-11 17:09:58.641734 proma-0.0.1/proma/draw/shapes/bar.py
--rw-r--r--   0        0        0     3292 2024-04-11 17:09:58.724852 proma-0.0.1/proma/draw/shapes/box.py
--rw-r--r--   0        0        0     2969 2024-04-11 17:09:58.169122 proma-0.0.1/proma/draw/shapes/cell.py
--rw-r--r--   0        0        0     3797 2024-04-11 17:09:58.402163 proma-0.0.1/proma/draw/shapes/label.py
--rw-r--r--   0        0        0     1341 2024-04-11 17:09:58.558031 proma-0.0.1/proma/draw/shapes/line.py
--rw-r--r--   0        0        0     2419 2024-04-11 17:09:58.245901 proma-0.0.1/proma/draw/shapes/linewithmarker.py
--rw-r--r--   0        0        0     9060 2024-04-11 17:09:58.481131 proma-0.0.1/proma/draw/shapes/marker.py
--rw-r--r--   0        0        0     2702 2024-04-11 17:09:58.804326 proma-0.0.1/proma/draw/shapes/pathwitharrow.py
--rw-r--r--   0        0        0     1728 2024-04-11 17:09:58.325270 proma-0.0.1/proma/draw/shapes/text.py
--rw-r--r--   0        0        0       46 2024-03-20 21:23:18.460000 proma-0.0.1/proma/draw/widgets/gantt/__init__.py
--rw-r--r--   0        0        0     6473 2024-04-11 17:09:57.799309 proma-0.0.1/proma/draw/widgets/gantt/gantt.py
--rw-r--r--   0        0        0      138 2024-03-20 21:22:11.089162 proma-0.0.1/proma/draw/widgets/grid/__init__.py
--rw-r--r--   0        0        0     3311 2024-04-11 17:09:58.088984 proma-0.0.1/proma/draw/widgets/grid/grid.py
--rw-r--r--   0        0        0     5578 2024-04-11 17:09:58.001512 proma-0.0.1/proma/draw/widgets/grid/gridrow.py
--rw-r--r--   0        0        0     4528 2024-04-11 17:09:57.972473 proma-0.0.1/proma/draw/widgets/grid/gridwithbars.py
--rw-r--r--   0        0        0      419 2024-04-11 18:01:49.438381 proma-0.0.1/proma/models/__init__.py
--rw-r--r--   0        0        0      148 2024-03-20 21:49:33.211866 proma-0.0.1/proma/models/event.py
--rw-r--r--   0        0        0      193 2024-03-20 22:08:06.005209 proma-0.0.1/proma/models/milestone.py
--rw-r--r--   0        0        0     3297 2024-04-11 18:01:38.141932 proma-0.0.1/proma/models/project.py
--rw-r--r--   0        0        0     3052 2024-04-11 18:01:40.280263 proma-0.0.1/proma/models/schema.py
--rw-r--r--   0        0        0      932 2024-03-20 22:08:26.908661 proma-0.0.1/proma/models/task.py
--rw-r--r--   0        0        0      990 2024-03-22 11:56:36.814751 proma-0.0.1/proma/models/timetableitem.py
--rw-r--r--   0        0        0     1091 2024-03-22 12:06:42.814922 proma-0.0.1/proma/models/timetablelevel.py
--rw-r--r--   0        0        0      173 2024-03-21 15:00:45.127164 proma-0.0.1/proma/models/types.py
--rw-r--r--   0        0        0      527 2024-03-22 11:52:31.352041 proma-0.0.1/proma/models/workpackage.py
--rwxr-xr-x   0        0        0     1643 2024-04-11 17:09:57.720907 proma-0.0.1/proma/proma.py
--rw-r--r--   0        0        0       59 2024-03-20 21:56:58.851665 proma-0.0.1/proma/utils/__init__.py
--rw-r--r--   0        0        0     5631 2024-04-11 17:09:06.591676 proma-0.0.1/proma/utils/timetable.py
--rw-r--r--   0        0        0      620 2024-04-14 13:38:44.592335 proma-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 proma-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-11 16:38:12.991778 proma-0.0.2/LICENSE
+-rw-r--r--   0        0        0      575 2024-04-11 17:08:28.793851 proma-0.0.2/README.rst
+-rw-r--r--   0        0        0        0 2024-03-20 22:05:07.102573 proma-0.0.2/proma/__init__.py
+-rwxr-xr-x   0        0        0     1643 2024-04-11 17:09:57.720907 proma-0.0.2/proma/cmd.py
+-rw-r--r--   0        0        0        0 2022-04-05 16:05:17.780922 proma-0.0.2/proma/draw/__init__.py
+-rw-r--r--   0        0        0      210 2024-03-20 22:06:18.786261 proma-0.0.2/proma/draw/base/__init__.py
+-rw-r--r--   0        0        0      773 2024-04-11 17:09:58.882121 proma-0.0.2/proma/draw/base/consts.py
+-rw-r--r--   0        0        0     7384 2024-04-11 17:09:59.048739 proma-0.0.2/proma/draw/base/dimension.py
+-rw-r--r--   0        0        0     1261 2024-03-20 21:35:36.543550 proma-0.0.2/proma/draw/base/listener.py
+-rw-r--r--   0        0        0      939 2024-03-20 21:35:14.730798 proma-0.0.2/proma/draw/base/margin.py
+-rw-r--r--   0        0        0      945 2024-03-20 21:34:59.609054 proma-0.0.2/proma/draw/base/padding.py
+-rw-r--r--   0        0        0     2473 2024-04-11 17:09:58.963348 proma-0.0.2/proma/draw/base/position.py
+-rw-r--r--   0        0        0     2625 2024-04-11 17:09:59.130040 proma-0.0.2/proma/draw/base/size.py
+-rw-r--r--   0        0        0      391 2024-03-20 21:33:22.558570 proma-0.0.2/proma/draw/shapes/__init__.py
+-rw-r--r--   0        0        0     2280 2024-04-11 17:09:58.641734 proma-0.0.2/proma/draw/shapes/bar.py
+-rw-r--r--   0        0        0     3292 2024-04-11 17:09:58.724852 proma-0.0.2/proma/draw/shapes/box.py
+-rw-r--r--   0        0        0     2969 2024-04-11 17:09:58.169122 proma-0.0.2/proma/draw/shapes/cell.py
+-rw-r--r--   0        0        0     3797 2024-04-11 17:09:58.402163 proma-0.0.2/proma/draw/shapes/label.py
+-rw-r--r--   0        0        0     1341 2024-04-11 17:09:58.558031 proma-0.0.2/proma/draw/shapes/line.py
+-rw-r--r--   0        0        0     2419 2024-04-11 17:09:58.245901 proma-0.0.2/proma/draw/shapes/linewithmarker.py
+-rw-r--r--   0        0        0     9060 2024-04-11 17:09:58.481131 proma-0.0.2/proma/draw/shapes/marker.py
+-rw-r--r--   0        0        0     2702 2024-04-11 17:09:58.804326 proma-0.0.2/proma/draw/shapes/pathwitharrow.py
+-rw-r--r--   0        0        0     1728 2024-04-11 17:09:58.325270 proma-0.0.2/proma/draw/shapes/text.py
+-rw-r--r--   0        0        0       46 2024-03-20 21:23:18.460000 proma-0.0.2/proma/draw/widgets/gantt/__init__.py
+-rw-r--r--   0        0        0     6473 2024-04-11 17:09:57.799309 proma-0.0.2/proma/draw/widgets/gantt/gantt.py
+-rw-r--r--   0        0        0      138 2024-03-20 21:22:11.089162 proma-0.0.2/proma/draw/widgets/grid/__init__.py
+-rw-r--r--   0        0        0     3311 2024-04-11 17:09:58.088984 proma-0.0.2/proma/draw/widgets/grid/grid.py
+-rw-r--r--   0        0        0     5578 2024-04-11 17:09:58.001512 proma-0.0.2/proma/draw/widgets/grid/gridrow.py
+-rw-r--r--   0        0        0     4528 2024-04-11 17:09:57.972473 proma-0.0.2/proma/draw/widgets/grid/gridwithbars.py
+-rw-r--r--   0        0        0      419 2024-04-11 18:01:49.438381 proma-0.0.2/proma/models/__init__.py
+-rw-r--r--   0        0        0      148 2024-03-20 21:49:33.211866 proma-0.0.2/proma/models/event.py
+-rw-r--r--   0        0        0      193 2024-03-20 22:08:06.005209 proma-0.0.2/proma/models/milestone.py
+-rw-r--r--   0        0        0     3297 2024-04-11 18:01:38.141932 proma-0.0.2/proma/models/project.py
+-rw-r--r--   0        0        0     3052 2024-04-11 18:01:40.280263 proma-0.0.2/proma/models/schema.py
+-rw-r--r--   0        0        0      932 2024-03-20 22:08:26.908661 proma-0.0.2/proma/models/task.py
+-rw-r--r--   0        0        0      990 2024-03-22 11:56:36.814751 proma-0.0.2/proma/models/timetableitem.py
+-rw-r--r--   0        0        0     1091 2024-03-22 12:06:42.814922 proma-0.0.2/proma/models/timetablelevel.py
+-rw-r--r--   0        0        0      173 2024-03-21 15:00:45.127164 proma-0.0.2/proma/models/types.py
+-rw-r--r--   0        0        0      527 2024-03-22 11:52:31.352041 proma-0.0.2/proma/models/workpackage.py
+-rw-r--r--   0        0        0       59 2024-03-20 21:56:58.851665 proma-0.0.2/proma/utils/__init__.py
+-rw-r--r--   0        0        0     5631 2024-04-11 17:09:06.591676 proma-0.0.2/proma/utils/timetable.py
+-rw-r--r--   0        0        0      614 2024-04-14 13:41:19.467305 proma-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 proma-0.0.2/PKG-INFO
```

### Comparing `proma-0.0.1/LICENSE` & `proma-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/README.rst` & `proma-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/base/consts.py` & `proma-0.0.2/proma/draw/base/consts.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/base/dimension.py` & `proma-0.0.2/proma/draw/base/dimension.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/base/listener.py` & `proma-0.0.2/proma/draw/base/listener.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/base/margin.py` & `proma-0.0.2/proma/draw/base/margin.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/base/padding.py` & `proma-0.0.2/proma/draw/base/padding.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/base/position.py` & `proma-0.0.2/proma/draw/base/position.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/base/size.py` & `proma-0.0.2/proma/draw/base/size.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/bar.py` & `proma-0.0.2/proma/draw/shapes/bar.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/box.py` & `proma-0.0.2/proma/draw/shapes/box.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/cell.py` & `proma-0.0.2/proma/draw/shapes/cell.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/label.py` & `proma-0.0.2/proma/draw/shapes/label.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/line.py` & `proma-0.0.2/proma/draw/shapes/line.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/linewithmarker.py` & `proma-0.0.2/proma/draw/shapes/linewithmarker.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/marker.py` & `proma-0.0.2/proma/draw/shapes/marker.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/pathwitharrow.py` & `proma-0.0.2/proma/draw/shapes/pathwitharrow.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/shapes/text.py` & `proma-0.0.2/proma/draw/shapes/text.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/widgets/gantt/gantt.py` & `proma-0.0.2/proma/draw/widgets/gantt/gantt.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/widgets/grid/grid.py` & `proma-0.0.2/proma/draw/widgets/grid/grid.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/widgets/grid/gridrow.py` & `proma-0.0.2/proma/draw/widgets/grid/gridrow.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/draw/widgets/grid/gridwithbars.py` & `proma-0.0.2/proma/draw/widgets/grid/gridwithbars.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/models/project.py` & `proma-0.0.2/proma/models/project.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/models/schema.py` & `proma-0.0.2/proma/models/schema.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/models/task.py` & `proma-0.0.2/proma/models/task.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/models/timetableitem.py` & `proma-0.0.2/proma/models/timetableitem.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/models/timetablelevel.py` & `proma-0.0.2/proma/models/timetablelevel.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/models/workpackage.py` & `proma-0.0.2/proma/models/workpackage.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/proma.py` & `proma-0.0.2/proma/cmd.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/proma/utils/timetable.py` & `proma-0.0.2/proma/utils/timetable.py`

 * *Files identical despite different names*

### Comparing `proma-0.0.1/pyproject.toml` & `proma-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "proma"
-version = "0.0.1"
+version = "0.0.2"
 description = "Project manager that can create Gantt diagrams as SVGs."
 authors = ["Ansgar Kellner <keans@gmx.de>"]
 license = "MIT"
 readme = "README.rst"
 
 [project.scripts]
-my-client = "proma.proma:cli"
+proma = "proma.cmd:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0.1"
 svgwrite = "^1.4.3"
 cerberus = "^1.3.5"
 python-dateutil = "^2.9.0.post0"
```

### Comparing `proma-0.0.1/PKG-INFO` & `proma-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proma
-Version: 0.0.1
+Version: 0.0.2
 Summary: Project manager that can create Gantt diagrams as SVGs.
 License: MIT
 Author: Ansgar Kellner
 Author-email: keans@gmx.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

