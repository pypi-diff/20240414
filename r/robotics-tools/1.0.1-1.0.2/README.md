# Comparing `tmp/robotics_tools-1.0.1.tar.gz` & `tmp/robotics_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotics_tools-1.0.1.tar", last modified: Sat Mar 30 11:23:54 2024, max compression
+gzip compressed data, was "robotics_tools-1.0.2.tar", last modified: Sun Apr 14 03:43:27 2024, max compression
```

## Comparing `robotics_tools-1.0.1.tar` & `robotics_tools-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxr-x   0 ghz       (1000) ghz       (1000)        0 2024-03-30 11:23:54.610506 robotics_tools-1.0.1/
--rw-rw-r--   0 ghz       (1000) ghz       (1000)     1067 2024-01-28 06:49:04.000000 robotics_tools-1.0.1/LICENSE
--rw-r--r--   0 ghz       (1000) ghz       (1000)      510 2024-03-30 11:23:54.610506 robotics_tools-1.0.1/PKG-INFO
--rw-rw-r--   0 ghz       (1000) ghz       (1000)      988 2024-03-28 08:14:10.000000 robotics_tools-1.0.1/README.md
-drwxrwxr-x   0 ghz       (1000) ghz       (1000)        0 2024-03-30 11:23:54.610506 robotics_tools-1.0.1/robot_tools/
--rw-rw-r--   0 ghz       (1000) ghz       (1000)       95 2024-01-28 06:49:04.000000 robotics_tools-1.0.1/robot_tools/__init__.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)    24401 2024-01-28 06:49:04.000000 robotics_tools-1.0.1/robot_tools/base_control.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)     4619 2024-03-15 07:40:32.000000 robotics_tools-1.0.1/robot_tools/biner.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)    12281 2024-03-15 11:17:46.000000 robotics_tools-1.0.1/robot_tools/caner.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)     4521 2024-03-28 08:12:17.000000 robotics_tools-1.0.1/robot_tools/conversions.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)    12244 2024-03-28 07:31:12.000000 robotics_tools-1.0.1/robot_tools/coordinate.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)     3780 2024-02-17 08:14:15.000000 robotics_tools-1.0.1/robot_tools/datar.py
--rwxrwxr-x   0 ghz       (1000) ghz       (1000)     9456 2024-01-28 06:49:04.000000 robotics_tools-1.0.1/robot_tools/interpolate.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)     1764 2024-02-17 08:23:17.000000 robotics_tools-1.0.1/robot_tools/modeler.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)    16649 2024-02-11 07:23:18.000000 robotics_tools-1.0.1/robot_tools/painter.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)     3568 2024-02-24 18:12:51.000000 robotics_tools-1.0.1/robot_tools/pather.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)     1715 2024-02-10 11:10:40.000000 robotics_tools-1.0.1/robot_tools/recorder.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)    46556 2024-02-17 14:17:49.000000 robotics_tools-1.0.1/robot_tools/trajer.py
--rw-rw-r--   0 ghz       (1000) ghz       (1000)    57957 2024-01-28 06:49:04.000000 robotics_tools-1.0.1/robot_tools/transformations.py
-drwxrwxr-x   0 ghz       (1000) ghz       (1000)        0 2024-03-30 11:23:54.610506 robotics_tools-1.0.1/robotics_tools.egg-info/
--rw-r--r--   0 ghz       (1000) ghz       (1000)      510 2024-03-30 11:23:54.000000 robotics_tools-1.0.1/robotics_tools.egg-info/PKG-INFO
--rw-rw-r--   0 ghz       (1000) ghz       (1000)      583 2024-03-30 11:23:54.000000 robotics_tools-1.0.1/robotics_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 ghz       (1000) ghz       (1000)        1 2024-03-30 11:23:54.000000 robotics_tools-1.0.1/robotics_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 ghz       (1000) ghz       (1000)       31 2024-03-30 11:23:54.000000 robotics_tools-1.0.1/robotics_tools.egg-info/requires.txt
--rw-rw-r--   0 ghz       (1000) ghz       (1000)       12 2024-03-30 11:23:54.000000 robotics_tools-1.0.1/robotics_tools.egg-info/top_level.txt
--rw-rw-r--   0 ghz       (1000) ghz       (1000)       38 2024-03-30 11:23:54.610506 robotics_tools-1.0.1/setup.cfg
--rwxrwxr-x   0 ghz       (1000) ghz       (1000)      626 2024-03-28 07:40:16.000000 robotics_tools-1.0.1/setup.py
+drwxrwxr-x   0 ghz       (1000) ghz       (1000)        0 2024-04-14 03:43:27.181936 robotics_tools-1.0.2/
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     1067 2024-01-28 06:49:04.000000 robotics_tools-1.0.2/LICENSE
+-rw-r--r--   0 ghz       (1000) ghz       (1000)      510 2024-04-14 03:43:27.181936 robotics_tools-1.0.2/PKG-INFO
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)      988 2024-03-28 08:14:10.000000 robotics_tools-1.0.2/README.md
+drwxrwxr-x   0 ghz       (1000) ghz       (1000)        0 2024-04-14 03:43:27.181936 robotics_tools-1.0.2/robot_tools/
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)       95 2024-01-28 06:49:04.000000 robotics_tools-1.0.2/robot_tools/__init__.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)    24401 2024-01-28 06:49:04.000000 robotics_tools-1.0.2/robot_tools/base_control.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     4619 2024-03-15 07:40:32.000000 robotics_tools-1.0.2/robot_tools/biner.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)    12281 2024-03-15 11:17:46.000000 robotics_tools-1.0.2/robot_tools/caner.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     4521 2024-04-09 06:57:48.000000 robotics_tools-1.0.2/robot_tools/conversions.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)    12244 2024-03-28 07:31:12.000000 robotics_tools-1.0.2/robot_tools/coordinate.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     4154 2024-04-11 03:32:24.000000 robotics_tools-1.0.2/robot_tools/datar.py
+-rwxrwxr-x   0 ghz       (1000) ghz       (1000)     9456 2024-01-28 06:49:04.000000 robotics_tools-1.0.2/robot_tools/interpolate.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     1764 2024-02-17 08:23:17.000000 robotics_tools-1.0.2/robot_tools/modeler.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     3461 2024-04-13 05:36:39.000000 robotics_tools-1.0.2/robot_tools/multi_tp.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)    16649 2024-02-11 07:23:18.000000 robotics_tools-1.0.2/robot_tools/painter.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     3623 2024-04-12 08:33:42.000000 robotics_tools-1.0.2/robot_tools/pather.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     1965 2024-04-11 06:13:21.000000 robotics_tools-1.0.2/robot_tools/performancer.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)    11489 2024-04-11 15:16:53.000000 robotics_tools-1.0.2/robot_tools/recorder.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)     2398 2024-04-13 03:03:52.000000 robotics_tools-1.0.2/robot_tools/roser.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)    46556 2024-02-17 14:17:49.000000 robotics_tools-1.0.2/robot_tools/trajer.py
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)    57957 2024-01-28 06:49:04.000000 robotics_tools-1.0.2/robot_tools/transformations.py
+drwxrwxr-x   0 ghz       (1000) ghz       (1000)        0 2024-04-14 03:43:27.181936 robotics_tools-1.0.2/robotics_tools.egg-info/
+-rw-r--r--   0 ghz       (1000) ghz       (1000)      510 2024-04-14 03:43:27.000000 robotics_tools-1.0.2/robotics_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)      662 2024-04-14 03:43:27.000000 robotics_tools-1.0.2/robotics_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)        1 2024-04-14 03:43:27.000000 robotics_tools-1.0.2/robotics_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)       31 2024-04-14 03:43:27.000000 robotics_tools-1.0.2/robotics_tools.egg-info/requires.txt
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)       12 2024-04-14 03:43:27.000000 robotics_tools-1.0.2/robotics_tools.egg-info/top_level.txt
+-rw-rw-r--   0 ghz       (1000) ghz       (1000)       38 2024-04-14 03:43:27.181936 robotics_tools-1.0.2/setup.cfg
+-rwxrwxr-x   0 ghz       (1000) ghz       (1000)      626 2024-04-14 03:43:18.000000 robotics_tools-1.0.2/setup.py
```

### Comparing `robotics_tools-1.0.1/LICENSE` & `robotics_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/README.md` & `robotics_tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/base_control.py` & `robotics_tools-1.0.2/robot_tools/base_control.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/biner.py` & `robotics_tools-1.0.2/robot_tools/biner.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/caner.py` & `robotics_tools-1.0.2/robot_tools/caner.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/conversions.py` & `robotics_tools-1.0.2/robot_tools/conversions.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/coordinate.py` & `robotics_tools-1.0.2/robot_tools/coordinate.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/datar.py` & `robotics_tools-1.0.2/robot_tools/datar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import numpy as np
 from typing import Tuple
 import os
 import glob
 
 
+def get_values_by_names(
+    sub_names: tuple, all_names: tuple, all_values: tuple
+) -> tuple:
+    """根据子名称列表获取所有值列表中对应的值列表，返回子值列表"""
+    sub_values = [0.0 for _ in range(len(sub_names))]
+    for i, name in enumerate(sub_names):
+        sub_values[i] = all_values[all_names.index(name)]
+    return tuple(sub_values)
+
+
 def remove_target(arr: np.ndarray, target) -> Tuple[np.ndarray, np.ndarray]:
     """删除一维数组中等于0的元素并返回原数组和被删除元素的索引"""
     return arr[arr != 0], np.where(arr == target)[0]
 
 
 def send_to_trash(pattern: str):
     # 定义要匹配的文件名模式
```

### Comparing `robotics_tools-1.0.1/robot_tools/interpolate.py` & `robotics_tools-1.0.2/robot_tools/interpolate.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/modeler.py` & `robotics_tools-1.0.2/robot_tools/modeler.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/painter.py` & `robotics_tools-1.0.2/robot_tools/painter.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/pather.py` & `robotics_tools-1.0.2/robot_tools/pather.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 
 
 def create_dir(path: str):
     """如果目录不存在则创建目录"""
     if not os.path.exists(path):
         os.makedirs(path)
 
+def get_home_dir():
+    return os.path.expanduser("~")
 
 try:
     import rospkg
 except:
     __ROS_PKG_NOT_FOUND__ = True
 else:
     __ROS_PKG_NOT_FOUND__ = False
```

### Comparing `robotics_tools-1.0.1/robot_tools/trajer.py` & `robotics_tools-1.0.2/robot_tools/trajer.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robot_tools/transformations.py` & `robotics_tools-1.0.2/robot_tools/transformations.py`

 * *Files identical despite different names*

### Comparing `robotics_tools-1.0.1/robotics_tools.egg-info/SOURCES.txt` & `robotics_tools-1.0.2/robotics_tools.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 ./robot_tools/biner.py
 ./robot_tools/caner.py
 ./robot_tools/conversions.py
 ./robot_tools/coordinate.py
 ./robot_tools/datar.py
 ./robot_tools/interpolate.py
 ./robot_tools/modeler.py
+./robot_tools/multi_tp.py
 ./robot_tools/painter.py
 ./robot_tools/pather.py
+./robot_tools/performancer.py
 ./robot_tools/recorder.py
+./robot_tools/roser.py
 ./robot_tools/trajer.py
 ./robot_tools/transformations.py
 robotics_tools.egg-info/PKG-INFO
 robotics_tools.egg-info/SOURCES.txt
 robotics_tools.egg-info/dependency_links.txt
 robotics_tools.egg-info/requires.txt
 robotics_tools.egg-info/top_level.txt
```

### Comparing `robotics_tools-1.0.1/setup.py` & `robotics_tools-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='robotics_tools',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     package_dir={"": "."},
     install_requires=['numpy>=1.19.5','scipy','matplotlib'],
     author='OpenGHz',
     author_email='ghz23@mails.tsinghua.edu.cn',
     description='Robot Tools for develop your robots.',
     url='https://gitlab.com/OpenGHz/airbot_play_vision_python.git',
```

