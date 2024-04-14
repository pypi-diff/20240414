# Comparing `tmp/emlabpkg-4.8.tar.gz` & `tmp/emlabpkg-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emlabpkg-4.8.tar", last modified: Sat Oct 14 18:46:07 2023, max compression
+gzip compressed data, was "emlabpkg-4.9.tar", last modified: Sat Oct 14 21:41:13 2023, max compression
```

## Comparing `emlabpkg-4.8.tar` & `emlabpkg-4.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-10-14 18:46:07.131843 emlabpkg-4.8/
--rw-rw-rw-   0        0        0      386 2023-10-14 18:46:07.130734 emlabpkg-4.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-10-14 18:46:07.096605 emlabpkg-4.8/emlabpkg/
-drwxrwxrwx   0        0        0        0 2023-10-14 18:46:07.116277 emlabpkg-4.8/emlabpkg/NF_ZM2376_Driver/
--rw-rw-rw-   0        0        0     8808 2023-09-19 00:06:34.000000 emlabpkg-4.8/emlabpkg/NF_ZM2376_Driver/NF_ZM2376_Driver_QCodes.py
--rw-rw-rw-   0        0        0       37 2023-08-18 20:49:28.000000 emlabpkg-4.8/emlabpkg/NF_ZM2376_Driver/__init__.py
--rw-rw-rw-   0        0        0       79 2023-08-18 20:52:09.000000 emlabpkg-4.8/emlabpkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-14 18:46:07.120717 emlabpkg-4.8/emlabpkg/gdspy_layouts/
--rw-rw-rw-   0        0        0       15 2023-10-07 04:05:28.000000 emlabpkg-4.8/emlabpkg/gdspy_layouts/__init__.py
--rw-rw-rw-   0        0        0    28994 2023-10-11 03:25:54.000000 emlabpkg-4.8/emlabpkg/gdspy_layouts/resonator_meanders.py
-drwxrwxrwx   0        0        0        0 2023-10-14 18:46:07.129258 emlabpkg-4.8/emlabpkg/sweep/
--rw-rw-rw-   0        0        0       19 2023-08-18 20:45:09.000000 emlabpkg-4.8/emlabpkg/sweep/__init__.py
--rw-rw-rw-   0        0        0     6679 2023-03-16 19:38:08.000000 emlabpkg-4.8/emlabpkg/sweep/db.py
--rw-rw-rw-   0        0        0     2755 2023-08-18 20:38:48.000000 emlabpkg-4.8/emlabpkg/sweep/db_test.py
--rw-rw-rw-   0        0        0     9093 2023-07-28 23:05:56.000000 emlabpkg-4.8/emlabpkg/sweep/plot.py
--rw-rw-rw-   0        0        0    13109 2023-08-18 20:40:36.000000 emlabpkg-4.8/emlabpkg/sweep/sweep.py
--rw-rw-rw-   0        0        0     2149 2023-08-18 20:39:31.000000 emlabpkg-4.8/emlabpkg/sweep/sweep_test.py
-drwxrwxrwx   0        0        0        0 2023-10-14 18:46:07.108523 emlabpkg-4.8/emlabpkg.egg-info/
--rw-rw-rw-   0        0        0      386 2023-10-14 18:46:06.000000 emlabpkg-4.8/emlabpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-10-14 18:46:06.000000 emlabpkg-4.8/emlabpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-14 18:46:06.000000 emlabpkg-4.8/emlabpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-10-14 18:46:06.000000 emlabpkg-4.8/emlabpkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-10-14 18:46:06.000000 emlabpkg-4.8/emlabpkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-14 18:46:07.131843 emlabpkg-4.8/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-10-14 18:44:55.000000 emlabpkg-4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-14 21:41:13.880311 emlabpkg-4.9/
+-rw-rw-rw-   0        0        0      386 2023-10-14 21:41:13.879314 emlabpkg-4.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-10-14 21:41:13.852871 emlabpkg-4.9/emlabpkg/
+drwxrwxrwx   0        0        0        0 2023-10-14 21:41:13.865352 emlabpkg-4.9/emlabpkg/NF_ZM2376_Driver/
+-rw-rw-rw-   0        0        0     8808 2023-09-19 00:06:34.000000 emlabpkg-4.9/emlabpkg/NF_ZM2376_Driver/NF_ZM2376_Driver_QCodes.py
+-rw-rw-rw-   0        0        0       37 2023-08-18 20:49:28.000000 emlabpkg-4.9/emlabpkg/NF_ZM2376_Driver/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-08-18 20:52:09.000000 emlabpkg-4.9/emlabpkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-14 21:41:13.868343 emlabpkg-4.9/emlabpkg/gdspy_layouts/
+-rw-rw-rw-   0        0        0       15 2023-10-07 04:05:28.000000 emlabpkg-4.9/emlabpkg/gdspy_layouts/__init__.py
+-rw-rw-rw-   0        0        0    29250 2023-10-14 21:12:34.000000 emlabpkg-4.9/emlabpkg/gdspy_layouts/resonator_meanders.py
+drwxrwxrwx   0        0        0        0 2023-10-14 21:41:13.877321 emlabpkg-4.9/emlabpkg/sweep/
+-rw-rw-rw-   0        0        0       19 2023-08-18 20:45:09.000000 emlabpkg-4.9/emlabpkg/sweep/__init__.py
+-rw-rw-rw-   0        0        0     6679 2023-03-16 19:38:08.000000 emlabpkg-4.9/emlabpkg/sweep/db.py
+-rw-rw-rw-   0        0        0     2755 2023-08-18 20:38:48.000000 emlabpkg-4.9/emlabpkg/sweep/db_test.py
+-rw-rw-rw-   0        0        0     9093 2023-07-28 23:05:56.000000 emlabpkg-4.9/emlabpkg/sweep/plot.py
+-rw-rw-rw-   0        0        0    13109 2023-08-18 20:40:36.000000 emlabpkg-4.9/emlabpkg/sweep/sweep.py
+-rw-rw-rw-   0        0        0     2149 2023-08-18 20:39:31.000000 emlabpkg-4.9/emlabpkg/sweep/sweep_test.py
+drwxrwxrwx   0        0        0        0 2023-10-14 21:41:13.860850 emlabpkg-4.9/emlabpkg.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-10-14 21:41:13.000000 emlabpkg-4.9/emlabpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-10-14 21:41:13.000000 emlabpkg-4.9/emlabpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-14 21:41:13.000000 emlabpkg-4.9/emlabpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-10-14 21:41:13.000000 emlabpkg-4.9/emlabpkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-10-14 21:41:13.000000 emlabpkg-4.9/emlabpkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-14 21:41:13.880311 emlabpkg-4.9/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-10-14 19:43:29.000000 emlabpkg-4.9/setup.py
```

### Comparing `emlabpkg-4.8/emlabpkg/NF_ZM2376_Driver/NF_ZM2376_Driver_QCodes.py` & `emlabpkg-4.9/emlabpkg/NF_ZM2376_Driver/NF_ZM2376_Driver_QCodes.py`

 * *Files identical despite different names*

### Comparing `emlabpkg-4.8/emlabpkg/gdspy_layouts/resonator_meanders.py` & `emlabpkg-4.9/emlabpkg/gdspy_layouts/resonator_meanders.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.feedline_extend_length = feedline_extend_length
         self.feedline_width = feedline_width
         self.feedline_path_width = feedline_path_width
         self.coupler_gap = coupler_gap
         self.outer_angle = self.inner_angle + self.gap + self.path_width
 
 class HangerArrayConfiguration:
-    def __init__(self, config, num_hangers_bottom, num_hangers_top, feedline_width=50, feedline_path_width=15, x_dist_pad_from_feedline=100):
+    def __init__(self, config, num_hangers_bottom, num_hangers_top, distance_between_meanders=100, feedline_width=50, feedline_path_width=15, feedline_extend_length=100, x_dist_pad_from_feedline=100):
         if isinstance(config, list):
             if len(config) == 2:
                 if len(config[0]) == num_hangers_bottom and len(config[1]) == num_hangers_top:
                     self.configs = config
                 elif len(config[0]) == 1 and len(config[1]) == 1:
                     self.configs = [config[0] * num_hangers_bottom, config[1] * num_hangers_top]
                 else:
@@ -48,14 +48,16 @@
                     raise AttributeError("The configurator passed to this function cannot have 'want_feedline_and_pads' set to True.")
         
         self.x_dist_pad_from_feedline = x_dist_pad_from_feedline
         self.num_hangers_top = num_hangers_top
         self.num_hangers_bottom = num_hangers_bottom
         self.feedline_width = feedline_width
         self.feedline_path_width = feedline_path_width
+        self.feedline_extend_length = feedline_extend_length
+        self.distance_between_meanders = distance_between_meanders
 
 class TransmissionConfiguration:
     def __init__(self, path_width, path3_width, gap, inner_angle, length_of_one_segment, total_loops, padding=40, rotation_angle=0, layers=[0, 1], points=43,
                  x=0, y=0, first_seg_length=None, last_seg_length=None, want_touch_pads=False):
         self.path_width = path_width
         self.path3_width = path3_width
         self.gap = gap
@@ -321,16 +323,16 @@
 def create_hangers_array(super_config: HangerArrayConfiguration):
     
     x_dist_pad_from_feedline = super_config.x_dist_pad_from_feedline
     configs = super_config.configs
     num_reson_bottom = len(super_config.configs[0])
     num_reson_top = len(super_config.configs[1])
     
-    distance_between_meanders = 100
-    feedline_extend_length = 300
+    distance_between_meanders = super_config.distance_between_meanders
+    feedline_extend_length = super_config.feedline_extend_length
     feedline_width = super_config.feedline_width
     feedline_path_width = super_config.feedline_path_width
     
     path1s_left = []
     path2s_left = []
     path3s_left = []
     feedlines = []
```

### Comparing `emlabpkg-4.8/emlabpkg/sweep/db.py` & `emlabpkg-4.9/emlabpkg/sweep/db.py`

 * *Files identical despite different names*

### Comparing `emlabpkg-4.8/emlabpkg/sweep/db_test.py` & `emlabpkg-4.9/emlabpkg/sweep/db_test.py`

 * *Files identical despite different names*

### Comparing `emlabpkg-4.8/emlabpkg/sweep/plot.py` & `emlabpkg-4.9/emlabpkg/sweep/plot.py`

 * *Files identical despite different names*

### Comparing `emlabpkg-4.8/emlabpkg/sweep/sweep.py` & `emlabpkg-4.9/emlabpkg/sweep/sweep.py`

 * *Files identical despite different names*

### Comparing `emlabpkg-4.8/emlabpkg/sweep/sweep_test.py` & `emlabpkg-4.9/emlabpkg/sweep/sweep_test.py`

 * *Files identical despite different names*

### Comparing `emlabpkg-4.8/setup.py` & `emlabpkg-4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="emlabpkg",
-    version="4.8",
+    version="4.9",
     summary="Univeristy of Cincinnati, Physics Department, Dr. Mikheev's Lab Package.",
     url="https://github.com/Sushant1708/emlabpkg",
     author="Sushant Padhye",
     author_email="padhyesm@mail.uc.edu",
     packages=find_packages(),
     install_requires=["qcodes", "gdspy"],
     description="Lab package for physics sweeps and LCR meter.",
```

