# Comparing `tmp/roadmapper-1.4.0.tar.gz` & `tmp/roadmapper-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadmapper-1.4.0.tar", last modified: Sun Nov 19 18:57:34 2023, max compression
+gzip compressed data, was "roadmapper-1.5.0.tar", last modified: Sun Apr 14 03:35:11 2024, max compression
```

## Comparing `roadmapper-1.4.0.tar` & `roadmapper-1.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-11-19 18:57:34.813017 roadmapper-1.4.0/
--rw-rw-rw-   0        0        0     1092 2023-01-07 22:57:29.000000 roadmapper-1.4.0/LICENSE.md
--rw-rw-rw-   0        0        0     4713 2023-11-19 18:57:34.812016 roadmapper-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4056 2023-07-26 09:36:51.000000 roadmapper-1.4.0/README.md
--rw-rw-rw-   0        0        0     1522 2023-10-15 07:02:46.000000 roadmapper-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-19 18:57:34.813017 roadmapper-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-19 18:57:34.760944 roadmapper-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-11-19 18:57:34.782461 roadmapper-1.4.0/src/roadmapper/
--rw-rw-rw-   0        0        0        0 2023-01-07 22:57:29.000000 roadmapper-1.4.0/src/roadmapper/__init__.py
--rw-rw-rw-   0        0        0     4207 2023-11-19 18:52:38.000000 roadmapper-1.4.0/src/roadmapper/alignment.py
--rw-rw-rw-   0        0        0    16949 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/roadmapper/colourtheme.py
--rw-rw-rw-   0        0        0     2888 2023-04-23 20:31:54.000000 roadmapper-1.4.0/src/roadmapper/footer.py
--rw-rw-rw-   0        0        0     7072 2023-09-16 23:50:43.000000 roadmapper-1.4.0/src/roadmapper/group.py
--rw-rw-rw-   0        0        0     4352 2023-09-16 23:50:43.000000 roadmapper-1.4.0/src/roadmapper/logo.py
--rw-rw-rw-   0        0        0     4831 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/roadmapper/marker.py
--rw-rw-rw-   0        0        0     3840 2023-11-19 18:52:38.000000 roadmapper-1.4.0/src/roadmapper/milestone.py
--rw-rw-rw-   0        0        0    35337 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/roadmapper/painter.py
--rw-rw-rw-   0        0        0    17633 2023-09-16 23:50:43.000000 roadmapper-1.4.0/src/roadmapper/roadmap.py
--rw-rw-rw-   0        0        0     2769 2023-07-09 09:15:03.000000 roadmapper-1.4.0/src/roadmapper/subtitle.py
--rw-rw-rw-   0        0        0    21157 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/roadmapper/task.py
--rw-rw-rw-   0        0        0    21951 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/roadmapper/timeline.py
--rw-rw-rw-   0        0        0    13382 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/roadmapper/timelineitem.py
--rw-rw-rw-   0        0        0     3846 2023-04-23 20:32:50.000000 roadmapper-1.4.0/src/roadmapper/timelineitemyear.py
--rw-rw-rw-   0        0        0     4384 2023-09-16 23:50:43.000000 roadmapper-1.4.0/src/roadmapper/timelinelocale.py
--rw-rw-rw-   0        0        0     1330 2023-04-09 00:51:50.000000 roadmapper-1.4.0/src/roadmapper/timelinemode.py
--rw-rw-rw-   0        0        0     2976 2023-09-16 23:50:43.000000 roadmapper-1.4.0/src/roadmapper/title.py
--rw-rw-rw-   0        0        0       24 2023-11-19 18:53:25.000000 roadmapper-1.4.0/src/roadmapper/version.py
-drwxrwxrwx   0        0        0        0 2023-11-19 18:57:34.797639 roadmapper-1.4.0/src/roadmapper.egg-info/
--rw-rw-rw-   0        0        0     4713 2023-11-19 18:57:34.000000 roadmapper-1.4.0/src/roadmapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1351 2023-11-19 18:57:34.000000 roadmapper-1.4.0/src/roadmapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-19 18:57:34.000000 roadmapper-1.4.0/src/roadmapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-11-19 18:57:34.000000 roadmapper-1.4.0/src/roadmapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-11-19 18:57:34.000000 roadmapper-1.4.0/src/roadmapper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-19 18:57:34.807018 roadmapper-1.4.0/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 00:51:50.000000 roadmapper-1.4.0/src/tests/__init__.py
--rw-rw-rw-   0        0        0     4459 2023-11-19 18:52:38.000000 roadmapper-1.4.0/src/tests/compare_generated_roadmaps_test.py
--rw-rw-rw-   0        0        0      869 2023-07-16 01:14:47.000000 roadmapper-1.4.0/src/tests/conftest.py
--rw-rw-rw-   0        0        0     1056 2023-05-26 11:05:58.000000 roadmapper-1.4.0/src/tests/roadmap_draw_test.py
-drwxrwxrwx   0        0        0        0 2023-11-19 18:57:34.811017 roadmapper-1.4.0/src/tests/roadmap_generators/
--rw-rw-rw-   0        0        0        0 2023-05-26 11:05:58.000000 roadmapper-1.4.0/src/tests/roadmap_generators/__init__.py
--rw-rw-rw-   0        0        0     2452 2023-07-09 09:15:03.000000 roadmapper-1.4.0/src/tests/roadmap_generators/colour_theme.py
--rw-rw-rw-   0        0        0     7122 2023-07-09 09:15:03.000000 roadmapper-1.4.0/src/tests/roadmap_generators/colour_theme_extensive.py
--rw-rw-rw-   0        0        0     2957 2023-11-19 18:52:38.000000 roadmapper-1.4.0/src/tests/roadmap_generators/milestone_text_alignment.py
--rw-rw-rw-   0        0        0      233 2023-05-26 11:05:58.000000 roadmapper-1.4.0/src/tests/roadmap_generators/roadmap_abc.py
--rw-rw-rw-   0        0        0     2585 2023-11-19 18:52:38.000000 roadmapper-1.4.0/src/tests/roadmap_generators/roadmap_generator.py
--rw-rw-rw-   0        0        0     3741 2023-11-19 18:52:38.000000 roadmapper-1.4.0/src/tests/test_alignment.py
--rw-rw-rw-   0        0        0    45136 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/tests/test_cases.py
--rw-rw-rw-   0        0        0    45975 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/tests/test_cases_svg.py
--rw-rw-rw-   0        0        0     3002 2023-11-19 18:52:38.000000 roadmapper-1.4.0/src/tests/test_milestone.py
--rw-rw-rw-   0        0        0     3192 2023-11-19 18:52:38.000000 roadmapper-1.4.0/src/tests/test_painter.py
--rw-rw-rw-   0        0        0    13589 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/tests/test_roadmapper.py
--rw-rw-rw-   0        0        0    13974 2023-10-15 07:02:46.000000 roadmapper-1.4.0/src/tests/test_roadmapper_svg.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:35:11.645279 roadmapper-1.5.0/
+-rw-rw-rw-   0        0        0     1092 2023-01-07 22:57:29.000000 roadmapper-1.5.0/LICENSE.md
+-rw-rw-rw-   0        0        0     4713 2024-04-14 03:35:11.645279 roadmapper-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4056 2024-04-14 03:30:58.000000 roadmapper-1.5.0/README.md
+-rw-rw-rw-   0        0        0     1549 2024-04-14 03:30:58.000000 roadmapper-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 03:35:11.645279 roadmapper-1.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 03:35:11.600651 roadmapper-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 03:35:11.617372 roadmapper-1.5.0/src/roadmapper/
+-rw-rw-rw-   0        0        0        0 2023-01-07 22:57:29.000000 roadmapper-1.5.0/src/roadmapper/__init__.py
+-rw-rw-rw-   0        0        0     4207 2023-11-19 18:52:38.000000 roadmapper-1.5.0/src/roadmapper/alignment.py
+-rw-rw-rw-   0        0        0    16949 2023-10-15 07:02:46.000000 roadmapper-1.5.0/src/roadmapper/colourtheme.py
+-rw-rw-rw-   0        0        0     2888 2023-04-23 20:31:54.000000 roadmapper-1.5.0/src/roadmapper/footer.py
+-rw-rw-rw-   0        0        0     7072 2023-09-16 23:50:43.000000 roadmapper-1.5.0/src/roadmapper/group.py
+-rw-rw-rw-   0        0        0     4352 2023-09-16 23:50:43.000000 roadmapper-1.5.0/src/roadmapper/logo.py
+-rw-rw-rw-   0        0        0     4831 2023-10-15 07:02:46.000000 roadmapper-1.5.0/src/roadmapper/marker.py
+-rw-rw-rw-   0        0        0     3840 2023-11-19 18:52:38.000000 roadmapper-1.5.0/src/roadmapper/milestone.py
+-rw-rw-rw-   0        0        0    40400 2024-04-14 03:30:58.000000 roadmapper-1.5.0/src/roadmapper/painter.py
+-rw-rw-rw-   0        0        0    17633 2023-09-16 23:50:43.000000 roadmapper-1.5.0/src/roadmapper/roadmap.py
+-rw-rw-rw-   0        0        0     2769 2023-07-09 09:15:03.000000 roadmapper-1.5.0/src/roadmapper/subtitle.py
+-rw-rw-rw-   0        0        0    21339 2024-04-14 03:30:58.000000 roadmapper-1.5.0/src/roadmapper/task.py
+-rw-rw-rw-   0        0        0    21951 2023-10-15 07:02:46.000000 roadmapper-1.5.0/src/roadmapper/timeline.py
+-rw-rw-rw-   0        0        0    13382 2023-10-15 07:02:46.000000 roadmapper-1.5.0/src/roadmapper/timelineitem.py
+-rw-rw-rw-   0        0        0     3846 2023-04-23 20:32:50.000000 roadmapper-1.5.0/src/roadmapper/timelineitemyear.py
+-rw-rw-rw-   0        0        0     4384 2023-09-16 23:50:43.000000 roadmapper-1.5.0/src/roadmapper/timelinelocale.py
+-rw-rw-rw-   0        0        0     1330 2023-04-09 00:51:50.000000 roadmapper-1.5.0/src/roadmapper/timelinemode.py
+-rw-rw-rw-   0        0        0     2976 2023-09-16 23:50:43.000000 roadmapper-1.5.0/src/roadmapper/title.py
+-rw-rw-rw-   0        0        0       23 2024-04-14 03:34:58.000000 roadmapper-1.5.0/src/roadmapper/version.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:35:11.645279 roadmapper-1.5.0/src/roadmapper.egg-info/
+-rw-rw-rw-   0        0        0     4713 2024-04-14 03:35:11.000000 roadmapper-1.5.0/src/roadmapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1351 2024-04-14 03:35:11.000000 roadmapper-1.5.0/src/roadmapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 03:35:11.000000 roadmapper-1.5.0/src/roadmapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-14 03:35:11.000000 roadmapper-1.5.0/src/roadmapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-14 03:35:11.000000 roadmapper-1.5.0/src/roadmapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 03:35:11.642320 roadmapper-1.5.0/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 00:51:50.000000 roadmapper-1.5.0/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     4459 2023-11-19 18:52:38.000000 roadmapper-1.5.0/src/tests/compare_generated_roadmaps_test.py
+-rw-rw-rw-   0        0        0      869 2023-07-16 01:14:47.000000 roadmapper-1.5.0/src/tests/conftest.py
+-rw-rw-rw-   0        0        0     1056 2023-05-26 11:05:58.000000 roadmapper-1.5.0/src/tests/roadmap_draw_test.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:35:11.645279 roadmapper-1.5.0/src/tests/roadmap_generators/
+-rw-rw-rw-   0        0        0        0 2023-05-26 11:05:58.000000 roadmapper-1.5.0/src/tests/roadmap_generators/__init__.py
+-rw-rw-rw-   0        0        0     2452 2023-07-09 09:15:03.000000 roadmapper-1.5.0/src/tests/roadmap_generators/colour_theme.py
+-rw-rw-rw-   0        0        0     7122 2023-07-09 09:15:03.000000 roadmapper-1.5.0/src/tests/roadmap_generators/colour_theme_extensive.py
+-rw-rw-rw-   0        0        0     2957 2023-11-19 18:52:38.000000 roadmapper-1.5.0/src/tests/roadmap_generators/milestone_text_alignment.py
+-rw-rw-rw-   0        0        0      233 2023-05-26 11:05:58.000000 roadmapper-1.5.0/src/tests/roadmap_generators/roadmap_abc.py
+-rw-rw-rw-   0        0        0     2585 2023-11-19 18:52:38.000000 roadmapper-1.5.0/src/tests/roadmap_generators/roadmap_generator.py
+-rw-rw-rw-   0        0        0     3741 2023-11-19 18:52:38.000000 roadmapper-1.5.0/src/tests/test_alignment.py
+-rw-rw-rw-   0        0        0    45161 2024-04-14 03:30:58.000000 roadmapper-1.5.0/src/tests/test_cases.py
+-rw-rw-rw-   0        0        0    45975 2023-10-15 07:02:46.000000 roadmapper-1.5.0/src/tests/test_cases_svg.py
+-rw-rw-rw-   0        0        0     3002 2023-11-19 18:52:38.000000 roadmapper-1.5.0/src/tests/test_milestone.py
+-rw-rw-rw-   0        0        0     3192 2023-11-19 18:52:38.000000 roadmapper-1.5.0/src/tests/test_painter.py
+-rw-rw-rw-   0        0        0    13589 2024-04-14 03:30:58.000000 roadmapper-1.5.0/src/tests/test_roadmapper.py
+-rw-rw-rw-   0        0        0    13974 2023-10-15 07:02:46.000000 roadmapper-1.5.0/src/tests/test_roadmapper_svg.py
```

### Comparing `roadmapper-1.4.0/LICENSE.md` & `roadmapper-1.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/PKG-INFO` & `roadmapper-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadmapper
-Version: 1.4.0
+Version: 1.5.0
 Summary: Roadmapper. A Roadmap-as-Code (RaC) python library for generating a roadmap by using python code
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/roadmapper
 Project-URL: Bug Tracker, https://github.com/csgoh/roadmapper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,16 +47,16 @@
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
 * python-dateutil >= 2.8.2
-* Pillow >= 10.0.0
-* drawsvg >= 2.2.0
+* Pillow >= 10.3.0
+* drawsvg >= 2.3.0
 
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
@@ -85,28 +85,28 @@
 ```python 
 from roadmapper.roadmap import Roadmap
 from roadmapper.timelinemode import TimelineMode
 
 roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
 roadmap.set_title("My Demo Roadmap")
 roadmap.set_subtitle("Matariki Technologies Ltd")
-roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=12)
+roadmap.set_timeline(TimelineMode.MONTHLY, start="2024-01-01", number_of_items=12)
 roadmap.add_logo("matariki-tech-logo.png", "top-right", 50, 50)
 
 group = roadmap.add_group("Core Product Work Stream")
 
-task = group.add_task("Base Functionality", "2023-01-01", "2023-10-31")
-task.add_milestone("v.1.0", "2023-02-15")
-task.add_milestone("v.1.1", "2023-08-01")
+task = group.add_task("Base Functionality", "2024-01-01", "2024-10-31")
+task.add_milestone("v.1.0", "2024-02-15")
+task.add_milestone("v.1.1", "2024-08-01")
 
-parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
-parellel_task.add_milestone("v.2.0", "2024-03-30")
+parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2025-03-31")
+parellel_task.add_milestone("v.2.0", "2025-03-30")
 
-task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
 roadmap.set_footer("Generated by Roadmapper")
 roadmap.draw()
 roadmap.save("demo01.png")
 ```
 
 ### Output
```

### Comparing `roadmapper-1.4.0/README.md` & `roadmapper-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
 * python-dateutil >= 2.8.2
-* Pillow >= 10.0.0
-* drawsvg >= 2.2.0
+* Pillow >= 10.3.0
+* drawsvg >= 2.3.0
 
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
@@ -68,28 +68,28 @@
 ```python 
 from roadmapper.roadmap import Roadmap
 from roadmapper.timelinemode import TimelineMode
 
 roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
 roadmap.set_title("My Demo Roadmap")
 roadmap.set_subtitle("Matariki Technologies Ltd")
-roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=12)
+roadmap.set_timeline(TimelineMode.MONTHLY, start="2024-01-01", number_of_items=12)
 roadmap.add_logo("matariki-tech-logo.png", "top-right", 50, 50)
 
 group = roadmap.add_group("Core Product Work Stream")
 
-task = group.add_task("Base Functionality", "2023-01-01", "2023-10-31")
-task.add_milestone("v.1.0", "2023-02-15")
-task.add_milestone("v.1.1", "2023-08-01")
+task = group.add_task("Base Functionality", "2024-01-01", "2024-10-31")
+task.add_milestone("v.1.0", "2024-02-15")
+task.add_milestone("v.1.1", "2024-08-01")
 
-parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
-parellel_task.add_milestone("v.2.0", "2024-03-30")
+parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2025-03-31")
+parellel_task.add_milestone("v.2.0", "2025-03-30")
 
-task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
 roadmap.set_footer("Generated by Roadmapper")
 roadmap.draw()
 roadmap.save("demo01.png")
 ```
 
 ### Output
```

### Comparing `roadmapper-1.4.0/pyproject.toml` & `roadmapper-1.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 [project.urls]
 "Homepage" = "https://github.com/csgoh/roadmapper"
 "Bug Tracker" = "https://github.com/csgoh/roadmapper/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"] # list of folders that contain the packages (["."] by default)
 exclude = [
+    "ci",
     "demo",
     "generate_gallery",
     "test_cases",
     "tempCodeRunnerFile",
 ] # exclude packages matching these glob patterns (empty by default)
 
 [tool.setuptools.dynamic]
@@ -40,12 +41,12 @@
     "ubuntu: Tests which only apply to Ubuntu environment",
     "macos: Tests which only apply to macOS environment",
     "windows: Tests which only apply to Windows environment",
 ]
 
 [tool.ruff]
 
-# Lint only dir `src`
-src = ["src"]
+# Lint only mentioned dirs
+src = ["src", "ci"]
 
 # Ignore line length limitation
-ignore = ["E501"]
+lint.ignore = ["E501"]
```

### Comparing `roadmapper-1.4.0/src/roadmapper/alignment.py` & `roadmapper-1.5.0/src/roadmapper/alignment.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/colourtheme.py` & `roadmapper-1.5.0/src/roadmapper/colourtheme.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/footer.py` & `roadmapper-1.5.0/src/roadmapper/footer.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/group.py` & `roadmapper-1.5.0/src/roadmapper/group.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/logo.py` & `roadmapper-1.5.0/src/roadmapper/logo.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/marker.py` & `roadmapper-1.5.0/src/roadmapper/marker.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/milestone.py` & `roadmapper-1.5.0/src/roadmapper/milestone.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/painter.py` & `roadmapper-1.5.0/src/roadmapper/painter.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,14 +327,30 @@
         return (
             box_x,
             box_y,
             box_x + box_width,
             box_y + box_height,
         )
 
+    def draw_text_on_box(
+        self,
+        box_x: int,
+        box_y: int,
+        box_width: int,
+        box_height: int,
+        box_fill_colour: int,
+        text: str,
+        text_alignment: str,
+        text_font: str,
+        text_font_size: int,
+        text_font_colour: str,
+        style: str = "rectangle",
+    ) -> None:
+        raise NotImplementedError
+
     def draw_diamond(
         self, x: int, y: int, width: int, height: int, fill_colour: str
     ) -> list:
         """Draw a diamond
 
         Args:
             x (int): X coordinate
@@ -517,21 +533,94 @@
                 raise ValueError("Invalid style")
 
         font = ImageFont.truetype(self.get_font_path(text_font), size=text_font_size)
 
         multi_lines = []
         wrap_lines = []
 
-        ### Make '\n' work
+        # ** Make '\n' work
         multi_lines = text.splitlines()
 
         left, _, right, _ = font.getbbox("a")
         single_char_width = right - left
 
-        ### wrap text
+        # ** wrap text
+        for line in multi_lines:
+            wrap_lines.extend(textwrap.wrap(line, int(box_width / single_char_width)))
+
+        pad = 4
+        line_count = len(wrap_lines)
+
+        for i, line in enumerate(wrap_lines):
+            font_width, font_height = self.get_text_dimension(
+                line, text_font, text_font_size
+            )
+
+            match text_alignment:
+                case "centre":
+                    x = box_x1 + (box_width - font_width) / 2
+                case "left":
+                    x = box_x1 + 15
+                case "right":
+                    x = box_x2 - font_width - 15
+                case _:
+                    x = box_x1 + (box_width - font_width) / 2
+
+            total_line_height = (font_height * line_count) + (pad * (line_count - 1))
+
+            single_line_height = font_height
+
+            y = (
+                box_y1
+                + ((box_height - total_line_height) / 2)
+                + ((single_line_height * i) + (pad * i))
+            )
+
+            self.__cr.text((x, y), line, fill=text_font_colour, anchor="la", font=font)
+
+    def draw_text_on_box(
+        self,
+        box_x: int,
+        box_y: int,
+        box_width: int,
+        box_height: int,
+        box_fill_colour: int,
+        text: str,
+        text_alignment: str,
+        text_font: str,
+        text_font_size: int,
+        text_font_colour: str,
+        style: str = "rectangle",
+    ) -> None:
+        box_x1, box_y1, box_x2, box_y2 = super().draw_box_with_text(
+            box_x,
+            box_y,
+            box_width,
+            box_height,
+            box_fill_colour,
+            text,
+            text_alignment,
+            text_font,
+            text_font_size,
+            text_font_colour,
+            style,
+        )
+
+        font = ImageFont.truetype(self.get_font_path(text_font), size=text_font_size)
+
+        multi_lines = []
+        wrap_lines = []
+
+        # ** Make '\n' work
+        multi_lines = text.splitlines()
+
+        left, _, right, _ = font.getbbox("a")
+        single_char_width = right - left
+
+        # ** wrap text
         for line in multi_lines:
             wrap_lines.extend(textwrap.wrap(line, int(box_width / single_char_width)))
 
         pad = 4
         line_count = len(wrap_lines)
 
         for i, line in enumerate(wrap_lines):
@@ -575,14 +664,15 @@
         """
 
         # Calculate the coordinates of the four points of the diamond.
         points = super().draw_diamond(x, y, width, height, fill_colour)
 
         # Use Pillow's ImageDraw module to draw a polygon with the given points and fill color.
         self.__cr.polygon(points, fill=fill_colour)
+        # self.__cr.polygon(points, outline=fill_colour, width=2)
 
     def draw_text(
         self, x: int, y: int, text: str, font: str, font_size: int, font_colour: str
     ) -> None:
         """Draw text
 
         Args:
@@ -872,14 +962,97 @@
         for line in multi_lines:
             wrap_lines.extend(textwrap.wrap(line, int(box_width / single_char_width)))
 
         pad = 4
         line_count = len(wrap_lines)
 
         for i, line in enumerate(wrap_lines):
+            font_width, font_height = self.get_text_dimension(
+                line, text_font, text_font_size
+            )
+
+            match text_alignment:
+                case "centre":
+                    x = box_x1 + (box_width - font_width) / 2
+                case "left":
+                    x = box_x1 + 15
+                case "right":
+                    x = box_x2 - font_width - 15
+                case _:
+                    x = box_x1 + (box_width - font_width) / 2
+
+            total_line_height = (font_height * line_count) + (pad * (line_count - 1))
+
+            single_line_height = font_height
+
+            y = (
+                box_y1
+                + ((box_height - total_line_height) / 2)
+                + ((single_line_height * i) + (pad * i))
+            )
+
+            txt = dw.Text(
+                line,
+                x=x,
+                y=y,
+                font_size=text_font_size,
+                stroke=text_font_colour,
+                text_anchor="start",
+                dominant_baseline="hanging",
+                font_family=text_font,
+            )
+            self.elements.append(txt)
+
+    def draw_text_on_box(
+        self,
+        box_x: int,
+        box_y: int,
+        box_width: int,
+        box_height: int,
+        box_fill_colour: int,
+        text: str,
+        text_alignment: str,
+        text_font: str,
+        text_font_size: int,
+        text_font_colour: str,
+        style: str = "rectangle",
+    ) -> None:
+        box_x1, box_y1, box_x2, box_y2 = super().draw_box_with_text(
+            box_x,
+            box_y,
+            box_width,
+            box_height,
+            box_fill_colour,
+            text,
+            text_alignment,
+            text_font,
+            text_font_size,
+            text_font_colour,
+            style,
+        )
+
+        font = ImageFont.truetype(self.get_font_path(text_font), size=text_font_size)
+
+        multi_lines = []
+        wrap_lines = []
+
+        # ** Make '\n' work
+        multi_lines = text.splitlines()
+
+        left, _, right, _ = font.getbbox("a")
+        single_char_width = right - left
+
+        # ** wrap text
+        for line in multi_lines:
+            wrap_lines.extend(textwrap.wrap(line, int(box_width / single_char_width)))
+
+        pad = 4
+        line_count = len(wrap_lines)
+
+        for i, line in enumerate(wrap_lines):
             font_width, font_height = self.get_text_dimension(
                 line, text_font, text_font_size
             )
 
             match text_alignment:
                 case "centre":
                     x = box_x1 + (box_width - font_width) / 2
```

### Comparing `roadmapper-1.4.0/src/roadmapper/roadmap.py` & `roadmapper-1.5.0/src/roadmapper/roadmap.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/subtitle.py` & `roadmapper-1.5.0/src/roadmapper/subtitle.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/task.py` & `roadmapper-1.5.0/src/roadmapper/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,49 +542,53 @@
         width = 0
         height = 0
 
         for i, box in enumerate(self.boxes):
             if i == 0:
                 box_x = box[0]
                 box_y = box[1]
-            ### Fix for [69] - factored in gap spaces width
+            # ** Fix for [69] - factored in gap spaces width
             width += int(box[2]) + 2
-            ###
+            # **
             height = box[3]
 
-        ### Fix for [69] - ignore the last gap space
+        # ** Fix for [69] - ignore the last gap space
         if width >= 2:
             width -= 2
-        ###
+        # **
 
         box_width, box_height = (
             width,
             height,
         )
 
-        if box_x != 0 or box_y != 0 or box_width != 0 or box_height != 0:
-            painter.draw_box_with_text(
+        if box_x != 0 and box_y != 0 and box_width > 0 and box_height != 0:
+            painter.draw_box(box_x, box_y, box_width, box_height, self.fill_colour)
+
+            # ** Fix for v1.4.1 - Draw milestone first before task text
+            for task in self.tasks:
+                task.draw(painter)
+
+            for milestone in self.milestones:
+                milestone.draw(painter)
+
+            painter.draw_text_on_box(
                 box_x,
                 box_y,
                 box_width,
                 box_height,
                 self.fill_colour,
                 self.text,
                 self.text_alignment,
                 self.font,
                 self.font_size,
                 self.font_colour,
                 style=self.style,
             )
-
-            for task in self.tasks:
-                task.draw(painter)
-
-            for milestone in self.milestones:
-                milestone.draw(painter)
+            # **
 
     def __enter__(self):
         """This method is called when the 'with' statement is used"""
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         """This method is called when the 'with' statement is used"""
```

### Comparing `roadmapper-1.4.0/src/roadmapper/timeline.py` & `roadmapper-1.5.0/src/roadmapper/timeline.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/timelineitem.py` & `roadmapper-1.5.0/src/roadmapper/timelineitem.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/timelineitemyear.py` & `roadmapper-1.5.0/src/roadmapper/timelineitemyear.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/timelinelocale.py` & `roadmapper-1.5.0/src/roadmapper/timelinelocale.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/timelinemode.py` & `roadmapper-1.5.0/src/roadmapper/timelinemode.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper/title.py` & `roadmapper-1.5.0/src/roadmapper/title.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/roadmapper.egg-info/PKG-INFO` & `roadmapper-1.5.0/src/roadmapper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadmapper
-Version: 1.4.0
+Version: 1.5.0
 Summary: Roadmapper. A Roadmap-as-Code (RaC) python library for generating a roadmap by using python code
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/roadmapper
 Project-URL: Bug Tracker, https://github.com/csgoh/roadmapper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,16 +47,16 @@
 ![multilingual roadmappper](https://github.com/csgoh/roadmapper/blob/main/images/roadmapper-banner-multilingual.png?raw=true)
 
 ### Python version requirements:
 * Python 3.10+
   
 ### Library Dependencies
 * python-dateutil >= 2.8.2
-* Pillow >= 10.0.0
-* drawsvg >= 2.2.0
+* Pillow >= 10.3.0
+* drawsvg >= 2.3.0
 
 
 Any feedback or suggestions are welcome. Please feel free to create an issue or pull request.
 <br/>
 <hr>
 
 
@@ -85,28 +85,28 @@
 ```python 
 from roadmapper.roadmap import Roadmap
 from roadmapper.timelinemode import TimelineMode
 
 roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
 roadmap.set_title("My Demo Roadmap")
 roadmap.set_subtitle("Matariki Technologies Ltd")
-roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=12)
+roadmap.set_timeline(TimelineMode.MONTHLY, start="2024-01-01", number_of_items=12)
 roadmap.add_logo("matariki-tech-logo.png", "top-right", 50, 50)
 
 group = roadmap.add_group("Core Product Work Stream")
 
-task = group.add_task("Base Functionality", "2023-01-01", "2023-10-31")
-task.add_milestone("v.1.0", "2023-02-15")
-task.add_milestone("v.1.1", "2023-08-01")
+task = group.add_task("Base Functionality", "2024-01-01", "2024-10-31")
+task.add_milestone("v.1.0", "2024-02-15")
+task.add_milestone("v.1.1", "2024-08-01")
 
-parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
-parellel_task.add_milestone("v.2.0", "2024-03-30")
+parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2025-03-31")
+parellel_task.add_milestone("v.2.0", "2025-03-30")
 
-task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
 roadmap.set_footer("Generated by Roadmapper")
 roadmap.draw()
 roadmap.save("demo01.png")
 ```
 
 ### Output
```

### Comparing `roadmapper-1.4.0/src/roadmapper.egg-info/SOURCES.txt` & `roadmapper-1.5.0/src/roadmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/compare_generated_roadmaps_test.py` & `roadmapper-1.5.0/src/tests/compare_generated_roadmaps_test.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/conftest.py` & `roadmapper-1.5.0/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/roadmap_draw_test.py` & `roadmapper-1.5.0/src/tests/roadmap_draw_test.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/roadmap_generators/colour_theme.py` & `roadmapper-1.5.0/src/tests/roadmap_generators/colour_theme.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/roadmap_generators/colour_theme_extensive.py` & `roadmapper-1.5.0/src/tests/roadmap_generators/colour_theme_extensive.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/roadmap_generators/milestone_text_alignment.py` & `roadmapper-1.5.0/src/tests/roadmap_generators/milestone_text_alignment.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/roadmap_generators/roadmap_generator.py` & `roadmapper-1.5.0/src/tests/roadmap_generators/roadmap_generator.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/test_alignment.py` & `roadmapper-1.5.0/src/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/test_cases.py` & `roadmapper-1.5.0/src/tests/test_cases_svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,29 @@
 
 def colour_theme_demo(
     width: int = 1200,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "colour_theme_demo.png",
+    file_name: str = "colour_theme_demo.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
-        width, 1000, auto_height=True, colour_theme=colour_theme, show_marker=False
+        width,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=False,
+        painter_type="SVG",
     )
     roadmap.set_title("STRATEGY ROADMAP 2023")
     roadmap.set_subtitle("Mars Software Inc.")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -200,24 +205,29 @@
 
 def unicode_demo(
     width: int = 1200,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "unicode_demo.png",
+    file_name: str = "unicode_demo.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
-        width, 1000, auto_height=True, colour_theme=colour_theme, show_marker=False
+        width,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=False,
+        painter_type="SVG",
     )
     roadmap.set_title("2023 年戰略路線圖")
     roadmap.set_subtitle("火星科技公司")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -384,24 +394,29 @@
 
 def sample_roadmap(
     width: int = 1200,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "sample_roadmap.png",
+    file_name: str = "sample_roadmap.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
-        width, 1000, auto_height=True, colour_theme=colour_theme, show_marker=False
+        width,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=False,
+        painter_type="SVG",
     )
     roadmap.set_title("STRATEGY ROADMAP 2023")
     roadmap.set_subtitle("Matariki Technologies Inc.")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -573,24 +588,29 @@
 
 def colour_theme_roadmap(
     width: int = 1200,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "colour_theme_roadmap.png",
+    file_name: str = "colour_theme_roadmap.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
-        width, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        width,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="SVG",
     )
     roadmap.set_title("SAMPLE ROADMAP 2022/2023")
     roadmap.set_subtitle("GodZone Corporation")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -622,28 +642,29 @@
     width: int = 1200,
     height: int = 1000,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-11-01",
     number_of_items: int = 24,
     show_marker: bool = False,
     show_generic_dates: bool = False,
-    file_name: str = "custom_colour_roadmap.png",
+    file_name: str = "custom_colour_roadmap.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
         width,
         height,
         auto_height=True,
         colour_theme=colour_theme,
         show_marker=show_marker,
+        painter_type="SVG",
     )
     roadmap.set_title("My Demo Roadmap!!!")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
@@ -666,55 +687,55 @@
     roadmap.draw()
     roadmap.save(output_file)
 
     assert os.path.exists(output_file)
 
 
 def banner_roadmap():
-    color_theme_roadmap("../../images/color-theme01.png", "DEFAULT")
-    color_theme_roadmap("../../images/color-theme02.png", "GREYWOOF")
-    color_theme_roadmap("../../images/color-theme03.png", "ORANGEPEEL")
-    color_theme_roadmap("../../images/color-theme04.png", "BLUEMOUNTAIN")
-    color_theme_roadmap("../../images/color-theme05.png", "GREENTURTLE")
+    color_theme_roadmap("../../images/color-theme01.svg", "DEFAULT")
+    color_theme_roadmap("../../images/color-theme02.svg", "GREYWOOF")
+    color_theme_roadmap("../../images/color-theme03.svg", "ORANGEPEEL")
+    color_theme_roadmap("../../images/color-theme04.svg", "BLUEMOUNTAIN")
+    color_theme_roadmap("../../images/color-theme05.svg", "GREENTURTLE")
 
 
 def multilingual_roadmap():
-    en_NZ_roadmap("../../images/en_NZ-roadmap.png", "../json/rainbow.json", "en_US")
+    en_NZ_roadmap("../../images/en_NZ-roadmap.svg", "../json/rainbow.json", "en_US")
     zh_TW_with_locale_roadmap(
-        "../../images/zh_TW-roadmap.png",
+        "../../images/zh_TW-roadmap.svg",
         "../json/rainbow-unicode.json",
         "../json/zh_TW_timeline_settings.json",
     )
     zh_TW_roadmap(
-        "../../images/zh_TW-timeline-roadmap.png",
+        "../../images/zh_TW-timeline-roadmap.svg",
         "../json/rainbow-unicode.json",
     )
     ja_JP_roadmap(
-        "../../images/ja_JP-roadmap.png",
+        "../../images/ja_JP-roadmap.svg",
         "../json/rainbow-unicode.json",
         "../json/ja_JP_timeline_settings.json",
     )
     ko_KR_roadmap(
-        "../../images/ko-KR-roadmap.png",
+        "../../images/ko-KR-roadmap.svg",
         "../json/rainbow-unicode.json",
         "../json/ko_KR_timeline_settings.json",
     )
 
 
 ### Wiki Images
 def home_roadmap():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/my_roadmap.png"
+    output_file = "../../images/my_roadmap.svg"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    my_roadmap = Roadmap(width=500, height=400)
+    my_roadmap = Roadmap(width=500, height=400, painter_type="SVG")
     my_roadmap.set_title("My Roadmap")
     my_roadmap.set_timeline(
         mode=TimelineMode.MONTHLY, start="2022-11-14", number_of_items=6
     )
 
     group = my_roadmap.add_group("Development")
     group.add_task("Activity 1", "2022-12-01", "2023-02-10")
@@ -727,20 +748,20 @@
     assert os.path.exists(output_file)
 
 
 def readme_roadmap():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/demo01.png"
+    output_file = "../../images/demo01.svg"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
+    roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN", painter_type="SVG")
     roadmap.set_title("My Demo Roadmap")
     roadmap.set_subtitle("Matariki Technologies Ltd")
     roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=12)
     roadmap.add_logo(
         "../../images/logo/matariki-tech-logo.png",
         position="top-right",
         width=50,
@@ -767,41 +788,45 @@
 
 def color_theme_roadmap(filename: str, colour_theme: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(600, 500, colour_theme=colour_theme, show_marker=True)
+    roadmap = Roadmap(
+        600, 500, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
+    )
     roadmap.set_title("My Demo Roadmap")
-    roadmap.set_timeline(TimelineMode.QUARTERLY, start="2023-07-01", number_of_items=4)
+    roadmap.set_timeline(TimelineMode.QUARTERLY, start="2023-01-01", number_of_items=4)
     roadmap.set_footer("Generated by Roadmapper")
 
     group = roadmap.add_group("Workstream 1")
-    task = group.add_task("Task 1-A", "2023-07-01", "2023-10-30")
-    task.add_parallel_task("Task 2-B", "2023-11-15", "2024-02-28")
-    group.add_task("Task 3-C", "2023-10-01", "2023-12-31")
+    task = group.add_task("Task 1-A", "2023-01-01", "2023-04-30")
+    task.add_parallel_task("Task 2-B", "2023-05-15", "2023-08-30")
+    group.add_task("Task 3-C", "2023-04-01", "2023-06-30")
 
     group = roadmap.add_group("Workstream 2")
-    group.add_task("Task 2-A", "2023-10-01", "2023-12-30")
-    group.add_task("Task 2-B", "2023-11-01", "2024-01-30")
-    group.add_task("Task 2-C", "2023-12-01", "2024-02-28")
+    group.add_task("Task 2-A", "2023-04-01", "2023-06-30")
+    group.add_task("Task 2-B", "2023-05-01", "2023-07-30")
+    group.add_task("Task 2-C", "2023-06-01", "2023-08-30")
 
     roadmap.draw()
     roadmap.save(filename)
     assert os.path.exists(output_file)
 
 
 def en_NZ_roadmap(filename: str, colour_theme: str, locale_name: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap = Roadmap(
+        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
+    )
     roadmap.set_title("Strategy Roadmap 2023")
     roadmap.set_subtitle("Matariki Technologies Ltd")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
         start="2023-01-01",
         number_of_items=4,
         timeline_locale=locale_name,
@@ -836,15 +861,17 @@
 
 def zh_TW_with_locale_roadmap(filename: str, colour_theme: str, locale_name: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap = Roadmap(
+        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
+    )
     roadmap.set_title("戰略路線圖 2023")
     roadmap.set_subtitle("瑪塔里奇太陽科技有限公司")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
         start="2023-01-01",
         number_of_items=4,
         timeline_locale=locale_name,
@@ -875,15 +902,17 @@
 
 def zh_TW_roadmap(filename: str, colour_theme: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap = Roadmap(
+        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
+    )
     roadmap.set_title("戰略路線圖 2023")
     roadmap.set_subtitle("瑪塔里奇太陽科技有限公司")
     roadmap.set_timeline(TimelineMode.QUARTERLY, start="2023-01-01", number_of_items=4)
     roadmap.set_footer("由 Roadmapper 生成")
 
     group = roadmap.add_group("人員流程")
     task = group.add_task("制定包容戰略", "2023-01-01", "2023-04-30")
@@ -909,15 +938,17 @@
 
 def ja_JP_roadmap(filename: str, colour_theme: str, locale_name: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap = Roadmap(
+        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
+    )
     roadmap.set_title("戦略的ロードマップ 2023")
     roadmap.set_subtitle("マタリッチサンテクノロジー株式会社")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
         start="2023-01-01",
         number_of_items=4,
         timeline_locale=locale_name,
@@ -948,15 +979,17 @@
 
 def ko_KR_roadmap(filename: str, colour_theme: str, locale_name: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap = Roadmap(
+        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
+    )
     roadmap.set_title("전략 로드맵 2023")
     roadmap.set_subtitle("마타리키 테크놀로지스")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
         start="2023-01-01",
         number_of_items=4,
         timeline_locale=locale_name,
@@ -989,69 +1022,71 @@
 
 
 def test_sample_case1():
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
     colour_theme_demo(
         width=2500,
-        file_name="../../images/test/test-ORANGEPEEL-weekly.png",
+        file_name="../../images/test/test-ORANGEPEEL-weekly.svg",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.WEEKLY,
         number_of_items=52,
         start_date="2023-01-01",
     )
 
 
 def test_sample_case2():
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
     colour_theme_demo(
-        file_name="../../images/test/test-ORANGEPEEL-monthly.png",
+        file_name="../../images/test/test-ORANGEPEEL-monthly.svg",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
 
 def test_sample_case3():
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
     colour_theme_demo(
-        file_name="../../images/test/test-ORANGEPEEL-quarter.png",
+        file_name="../../images/test/test-ORANGEPEEL-quarter.svg",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.QUARTERLY,
         number_of_items=4,
         start_date="2023-01-01",
     )
 
 
 def test_sample_unicase1():
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
     unicode_demo(
-        file_name="../../images/test/test-unicode-monthly.png",
+        file_name="../../images/test/test-unicode-monthly.svg",
         # colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
     assert True
 
 
 def test_draw_anatomy():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/roadmapper-anatomy-base.png"
+    output_file = "../../images/roadmapper-anatomy-base.svg"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(1200, 380, colour_theme="BLUEMOUNTAIN", show_marker=True)
+    roadmap = Roadmap(
+        1200, 380, colour_theme="BLUEMOUNTAIN", show_marker=True, painter_type="SVG"
+    )
     roadmap.set_title("Product Roadmap")
     roadmap.set_subtitle("Matariki Tech Ltd")
     roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=9)
     roadmap.set_footer("Generated by Roadmapper")
 
     group = roadmap.add_group("Workstream 1")
     task = group.add_task("Task 1-A", "2023-01-01", "2023-05-15")
@@ -1065,20 +1100,22 @@
     assert os.path.exists(output_file)
 
 
 def test_draw_banner_theme():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/theme-demo01.png"
+    output_file = "../../images/theme-demo01.svg"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(600, 380, colour_theme="BLUEMOUNTAIN", show_marker=True)
+    roadmap = Roadmap(
+        600, 380, colour_theme="BLUEMOUNTAIN", show_marker=True, painter_type="SVG"
+    )
     roadmap.set_title("My Demo Roadmap")
     roadmap.set_timeline(TimelineMode.QUARTERLY, start="2023-01-01", number_of_items=4)
     roadmap.set_footer("Generated by Roadmapper")
 
     group = roadmap.add_group("Workstream 1")
     task = group.add_task("Task 1-A", "2023-01-01", "2023-04-30")
     task.add_parallel_task("Task 2-B", "2023-05-15", "2023-08-30")
@@ -1094,20 +1131,20 @@
     assert os.path.exists(output_file)
 
 
 def test_draw_banner():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/demo01.png"
+    output_file = "../../images/demo01.svg"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(600, 500, show_marker=False, auto_height=True)
+    roadmap = Roadmap(600, 500, show_marker=False, auto_height=True, painter_type="SVG")
     roadmap.set_title("My Demo Roadmap")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
         start="2023-01-01",
         number_of_items=3,
         year_fill_colour="#7CC1AC",
         year_font_colour="black",
@@ -1170,121 +1207,121 @@
     assert os.path.exists(output_file)
 
 
 def test_gallery_images():
     ### Sample Roadmap ###
     sample_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-sample-01.png",
+        file_name="../../images/gallery/gallery-sample-01.svg",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     ### Colour Theme Roadmap ###
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-DEFAULT-monthly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-monthly.svg",
         # colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-ORANGEPEEL-monthly.png",
+        file_name="../../images/gallery/gallery-ORANGEPEEL-monthly.svg",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-BLUEMOUNTAIN-monthly.png",
+        file_name="../../images/gallery/gallery-BLUEMOUNTAIN-monthly.svg",
         colour_theme="BLUEMOUNTAIN",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-GREENTURTLE-monthly.png",
+        file_name="../../images/gallery/gallery-GREENTURTLE-monthly.svg",
         colour_theme="GREENTURTLE",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-GREYWOOF-monthly.png",
+        file_name="../../images/gallery/gallery-GREYWOOF-monthly.svg",
         colour_theme="GREYWOOF",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
     )
 
     ### Marker Roadmap ###
     custom_colour_roadmap(
         width=1200,
-        file_name="../../images/gallery/gallery-marker-monthly.png",
+        file_name="../../images/gallery/gallery-marker-monthly.svg",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2022-11-01",
         show_marker=True,
         show_generic_dates=False,
     )
 
     ### WEEKLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=2400,
-        file_name="../../images/gallery/gallery-DEFAULT-weekly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-weekly.svg",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.WEEKLY,
         number_of_items=52,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### QUARTERLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-DEFAULT-quarterly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-quarterly.svg",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.QUARTERLY,
         number_of_items=6,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### HALF-YEARLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-DEFAULT-halfyearly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-halfyearly.svg",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.HALF_YEARLY,
         number_of_items=4,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### YEARLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-DEFAULT-yearly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-yearly.svg",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.YEARLY,
         number_of_items=2,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### Generic Dates Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-DEFAULT-generic-monthly.png",
+        file_name="../../images/gallery/gallery-DEFAULT-generic-monthly.svg",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
         start_date="2023-01-01",
         show_generic_dates=True,
     )
 
@@ -1294,15 +1331,20 @@
     home_roadmap()
     banner_roadmap()
     multilingual_roadmap()
 
 
 def test_with_context_manager():
     with Roadmap(
-        1200, 500, show_marker=False, auto_height=True, colour_theme="ORANGEPEEL"
+        1200,
+        500,
+        show_marker=False,
+        auto_height=True,
+        colour_theme="ORANGEPEEL",
+        painter_type="SVG",
     ) as my_roadmap:
         my_roadmap.set_title("Context Manager Test Roadmap")
         my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01")
         with my_roadmap.add_group("Workstream 1") as group1:
             with group1.add_task(
                 "Task 1-A",
                 "2023-01-01",
@@ -1315,20 +1357,25 @@
                 ) as parallel_task1:
                     parallel_task1.add_milestone("Milestone 2", "2023-08-10")
                 task1.add_milestone(
                     "Milestone 1",
                     "2023-04-01",
                 )
         my_roadmap.draw()
-        my_roadmap.save("../../images/with_context_manager.png")
+        my_roadmap.save("../../images/with_context_manager.svg")
 
 
 def test_black_blackground():
     with Roadmap(
-        1200, 500, show_marker=False, auto_height=True, colour_theme="ORANGEPEEL"
+        1200,
+        500,
+        show_marker=False,
+        auto_height=True,
+        colour_theme="ORANGEPEEL",
+        painter_type="SVG",
     ) as my_roadmap:
         my_roadmap.set_background_colour("black")
         my_roadmap.set_title("Black Background Test Roadmap")
         my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01")
         with my_roadmap.add_group("Workstream 1") as group1:
             with group1.add_task(
                 "Task 1-A",
@@ -1342,20 +1389,25 @@
                 ) as parallel_task1:
                     parallel_task1.add_milestone("Milestone 2", "2023-08-10")
                 task1.add_milestone(
                     "Milestone 1",
                     "2023-04-01",
                 )
         my_roadmap.draw()
-        my_roadmap.save("../../images/black_roadmap.png")
+        my_roadmap.save("../../images/black_roadmap.svg")
 
 
 def test_transparent_blackground():
     with Roadmap(
-        1200, 500, show_marker=False, auto_height=True, colour_theme="ORANGEPEEL"
+        1200,
+        500,
+        show_marker=False,
+        auto_height=True,
+        colour_theme="ORANGEPEEL",
+        painter_type="SVG",
     ) as my_roadmap:
         my_roadmap.set_background_colour("transparent")
         my_roadmap.set_title("Transparent Background Test Roadmap")
         my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01")
         with my_roadmap.add_group("Workstream 1") as group1:
             with group1.add_task(
                 "Task 1-A",
@@ -1369,8 +1421,8 @@
                 ) as parallel_task1:
                     parallel_task1.add_milestone("Milestone 2", "2023-08-10")
                 task1.add_milestone(
                     "Milestone 1",
                     "2023-04-01",
                 )
         my_roadmap.draw()
-        my_roadmap.save("../../images/transparent_roadmap.png")
+        my_roadmap.save("../../images/transparent_roadmap.svg")
```

### Comparing `roadmapper-1.4.0/src/tests/test_cases_svg.py` & `roadmapper-1.5.0/src/tests/test_cases.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,200 +1,195 @@
 import os
 from datetime import datetime
 from src.roadmapper.roadmap import Roadmap
 from src.roadmapper.timelinemode import TimelineMode
 
 
-### Roadmap Tests ###
+# ** Roadmap Tests
 
 
 def colour_theme_demo(
     width: int = 1200,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-12-01",
+    start_date: str = "2024-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "colour_theme_demo.svg",
+    file_name: str = "colour_theme_demo.png",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
-        width,
-        1000,
-        auto_height=True,
-        colour_theme=colour_theme,
-        show_marker=False,
-        painter_type="SVG",
+        width, 1000, auto_height=True, colour_theme=colour_theme, show_marker=False
     )
-    roadmap.set_title("STRATEGY ROADMAP 2023")
+    roadmap.set_title("STRATEGY ROADMAP 2024")
     roadmap.set_subtitle("Mars Software Inc.")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
         year_fill_colour="#404040",
         item_fill_colour="#404040",
         year_font_colour="white",
         item_font_colour="white",
     )
 
     group = roadmap.add_group("Planning", fill_colour="#FFC000", font_colour="black")
     task = group.add_task(
-        "Vision", "2023-01-01", "2023-03-31", fill_colour="#FFC000", font_colour="black"
+        "Vision", "2024-01-01", "2024-03-31", fill_colour="#FFC000", font_colour="black"
     )
     task = group.add_task(
-        "Goals", "2023-02-15", "2023-03-31", fill_colour="#FFC000", font_colour="black"
+        "Goals", "2024-02-15", "2024-03-31", fill_colour="#FFC000", font_colour="black"
     )
     task.add_parallel_task(
         "Strategic Intent",
-        "2023-04-01",
-        "2023-05-31",
+        "2024-04-01",
+        "2024-05-31",
         fill_colour="#FFC000",
         font_colour="black",
     )
     task.add_parallel_task(
         "Sales Budget",
-        "2023-06-01",
-        "2023-07-15",
+        "2024-06-01",
+        "2024-07-15",
         fill_colour="#FFC000",
         font_colour="black",
     )
     task.add_parallel_task(
         "Release Plans",
-        "2023-07-16",
-        "2023-09-30",
+        "2024-07-16",
+        "2024-09-30",
         fill_colour="#FFC000",
         font_colour="black",
     )
 
     group = roadmap.add_group("Strategy", fill_colour="#ED7D31", font_colour="black")
     task = group.add_task(
         "Market Analysis",
-        "2023-02-01",
-        "2023-03-30",
+        "2024-02-01",
+        "2024-03-30",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     task.add_milestone(
-        "Competitor Review", "2023-03-30", fill_colour="#843C0C", font_colour="black"
+        "Competitor Review", "2024-03-30", fill_colour="#843C0C", font_colour="black"
     )
     task.add_parallel_task(
-        "SWOT", "2023-04-01", "2023-04-30", fill_colour="#ED7D31", font_colour="black"
+        "SWOT", "2024-04-01", "2024-04-30", fill_colour="#ED7D31", font_colour="black"
     )
     task = group.add_task(
         "Business Model",
-        "2023-04-01",
-        "2023-05-31",
+        "2024-04-01",
+        "2024-05-31",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     task.add_milestone(
-        "Price List (Draft)", "2023-06-01", fill_colour="#843C0C", font_colour="black"
+        "Price List (Draft)", "2024-06-01", fill_colour="#843C0C", font_colour="black"
     )
     parallel_task = task.add_parallel_task(
-        "Price Reseach",
-        "2023-06-01",
-        "2023-08-05",
+        "Price Reseach XXXXXXXXXXX",
+        "2024-06-01",
+        "2024-08-05",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     parallel_task.add_milestone(
-        "Price List (Final)", "2023-07-28", fill_colour="#843C0C", font_colour="black"
+        "Price List (Final)", "2024-07-28", fill_colour="#843C0C", font_colour="black"
     )
     group.add_task(
         "Objectives",
-        "2023-06-20",
-        "2023-09-10",
+        "2024-06-20",
+        "2024-09-10",
         fill_colour="#ED7D31",
         font_colour="black",
     )
 
     group.add_task(
         "Sales Trends Analysis",
-        "2023-08-15",
-        "2023-10-10",
+        "2024-08-15",
+        "2024-10-10",
         fill_colour="#ED7D31",
         font_colour="black",
     )
 
     group = roadmap.add_group(
         "Service Development", fill_colour="#70AD47", font_colour="black"
     )
     task = group.add_task(
         "Product Roadmap",
-        "2023-02-15",
-        "2023-03-31",
+        "2024-02-15",
+        "2024-03-31",
         fill_colour="#70AD47",
         font_colour="black",
     )
     parallel_task = task.add_parallel_task(
         "Development",
-        "2023-04-01",
-        "2023-08-30",
+        "2024-04-01",
+        "2024-08-30",
         fill_colour="#70AD47",
         font_colour="black",
     )
     parallel_task.add_milestone(
-        "Alpha May 20", "2023-05-20", fill_colour="#385723", font_colour="black"
+        "Alpha May 20", "2024-05-20", fill_colour="#385723", font_colour="black"
     )
     parallel_task.add_milestone(
-        "Private Beta Jun 30", "2023-06-30", fill_colour="#385723", font_colour="black"
+        "Private Beta Jun 30", "2024-06-30", fill_colour="#385723", font_colour="black"
     )
     parallel_task.add_milestone(
-        "Public Beta Jun 30", "2023-08-10", fill_colour="#385723", font_colour="black"
+        "Public Beta Jun 30", "2024-08-10", fill_colour="#385723", font_colour="black"
     )
 
     parallel_task = task.add_parallel_task(
         "Release Candidate",
-        "2023-09-01",
-        "2023-10-15",
+        "2024-09-01",
+        "2024-10-15",
         fill_colour="#70AD47",
         font_colour="black",
     )
 
     parallel_task = task.add_parallel_task(
         "Release To Public",
-        "2023-10-16",
-        "2023-12-31",
+        "2024-10-16",
+        "2024-12-31",
         fill_colour="#70AD47",
         font_colour="black",
     )
 
     parallel_task.add_milestone(
-        "Go Live Dec 20", "2023-12-20", fill_colour="#385723", font_colour="black"
+        "Go Live Dec 20", "2024-12-20", fill_colour="#385723", font_colour="black"
     )
 
     group = roadmap.add_group(
         "Business Intelligence",
         fill_colour="#4472C4",
         font_colour="black",
     )
     task = group.add_task(
         "BI Development",
-        "2023-04-15",
-        "2023-12-31",
+        "2024-04-15",
+        "2024-12-31",
         fill_colour="#4472C4",
         font_colour="black",
     )
 
     task.add_milestone(
-        "Service Dashboard", "2023-05-15", fill_colour="#162641", font_colour="black"
+        "Service Dashboard", "2024-05-15", fill_colour="#162641", font_colour="black"
     )
 
     task.add_milestone(
-        "Real-Time Analytics", "2023-08-01", fill_colour="#162641", font_colour="black"
+        "Real-Time Analytics", "2024-08-01", fill_colour="#162641", font_colour="black"
     )
 
     task.add_milestone(
-        "Sales Dashboard", "2023-12-15", fill_colour="#162641", font_colour="black"
+        "Sales Dashboard", "2024-12-15", fill_colour="#162641", font_colour="black"
     )
 
     roadmap.set_footer(
         "Generated by Roadmapper on " + datetime.now().strftime("%Y-%m-%d")
     )
     roadmap.draw()
 
@@ -205,188 +200,185 @@
 
 def unicode_demo(
     width: int = 1200,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "unicode_demo.svg",
+    file_name: str = "unicode_demo.png",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
-        width,
-        1000,
-        auto_height=True,
-        colour_theme=colour_theme,
-        show_marker=False,
-        painter_type="SVG",
+        width, 1000, auto_height=True, colour_theme=colour_theme, show_marker=False
     )
-    roadmap.set_title("2023 年戰略路線圖")
+    roadmap.set_title("2024 年戰略路線圖")
     roadmap.set_subtitle("火星科技公司")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
         year_fill_colour="#404040",
         item_fill_colour="#404040",
         year_font_colour="white",
         item_font_colour="white",
     )
 
     group = roadmap.add_group("規劃", fill_colour="#FFC000", font_colour="black")
     task = group.add_task(
-        "願景", "2023-01-01", "2023-03-31", fill_colour="#FFC000", font_colour="black"
+        "願景", "2024-01-01", "2024-03-31", fill_colour="#FFC000", font_colour="black"
     )
     task = group.add_task(
-        "目標", "2023-02-15", "2023-03-31", fill_colour="#FFC000", font_colour="black"
+        "目標", "2024-02-15", "2024-03-31", fill_colour="#FFC000", font_colour="black"
     )
     task.add_parallel_task(
         "戰略意圖",
-        "2023-04-01",
-        "2023-05-31",
+        "2024-04-01",
+        "2024-05-31",
         fill_colour="#FFC000",
         font_colour="black",
     )
     task.add_parallel_task(
         "銷售預算",
-        "2023-06-01",
-        "2023-07-15",
+        "2024-06-01",
+        "2024-07-15",
         fill_colour="#FFC000",
         font_colour="black",
     )
     task.add_parallel_task(
         "發布計劃",
-        "2023-07-16",
-        "2023-09-30",
+        "2024-07-16",
+        "2024-09-30",
         fill_colour="#FFC000",
         font_colour="black",
     )
 
     group = roadmap.add_group("戰略", fill_colour="#ED7D31", font_colour="black")
     task = group.add_task(
         "市場分析",
-        "2023-02-01",
-        "2023-03-30",
+        "2024-02-01",
+        "2024-03-30",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     task.add_milestone(
-        "競爭對手審查", "2023-03-30", fill_colour="#843C0C", font_colour="black"
+        "競爭對手審查", "2024-03-30", fill_colour="#843C0C", font_colour="black"
     )
     task.add_parallel_task(
-        "SWOT", "2023-04-01", "2023-04-30", fill_colour="#ED7D31", font_colour="black"
+        "SWOT", "2024-04-01", "2024-04-30", fill_colour="#ED7D31", font_colour="black"
     )
     task = group.add_task(
         "商業模式",
-        "2023-04-01",
-        "2023-05-31",
+        "2024-04-01",
+        "2024-05-31",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     task.add_milestone(
-        "價目表（草稿）", "2023-06-01", fill_colour="#843C0C", font_colour="black"
+        "價目表（草稿）", "2024-06-01", fill_colour="#843C0C", font_colour="black"
     )
     parallel_task = task.add_parallel_task(
         "價格研究",
-        "2023-06-01",
-        "2023-08-05",
+        "2024-06-01",
+        "2024-08-05",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     parallel_task.add_milestone(
-        "價目表（最終）", "2023-07-28", fill_colour="#843C0C", font_colour="black"
+        "價目表（最終）", "2024-07-28", fill_colour="#843C0C", font_colour="black"
     )
     group.add_task(
         "目標",
-        "2023-06-20",
-        "2023-09-10",
+        "2024-06-20",
+        "2024-09-10",
         fill_colour="#ED7D31",
         font_colour="black",
     )
 
     group.add_task(
         "銷售趨勢分析",
-        "2023-08-15",
-        "2023-10-10",
+        "2024-08-15",
+        "2024-10-10",
         fill_colour="#ED7D31",
         font_colour="black",
     )
 
     group = roadmap.add_group("服務發展", fill_colour="#70AD47", font_colour="black")
     task = group.add_task(
         "產品路線圖",
-        "2023-02-15",
-        "2023-03-31",
+        "2024-02-15",
+        "2024-03-31",
         fill_colour="#70AD47",
         font_colour="black",
     )
     parallel_task = task.add_parallel_task(
         "軟件開發",
-        "2023-04-01",
-        "2023-08-30",
+        "2024-04-01",
+        "2024-08-30",
         fill_colour="#70AD47",
         font_colour="black",
     )
     parallel_task.add_milestone(
-        "阿尔法 5月20", "2023-05-20", fill_colour="#385723", font_colour="black"
+        "阿尔法 5月20", "2024-05-20", fill_colour="#385723", font_colour="black"
     )
     parallel_task.add_milestone(
-        "私人測試 6月30", "2023-06-30", fill_colour="#385723", font_colour="black"
+        "私人測試 6月30", "2024-06-30", fill_colour="#385723", font_colour="black"
     )
     parallel_task.add_milestone(
-        "公開測試 8月30", "2023-08-10", fill_colour="#385723", font_colour="black"
+        "公開測試 8月30", "2024-08-10", fill_colour="#385723", font_colour="black"
     )
 
     parallel_task = task.add_parallel_task(
         "候选版本",
-        "2023-09-01",
-        "2023-10-15",
+        "2024-09-01",
+        "2024-10-15",
         fill_colour="#70AD47",
         font_colour="black",
     )
 
     parallel_task = task.add_parallel_task(
         "公開發布",
-        "2023-10-16",
-        "2023-12-31",
+        "2024-10-16",
+        "2024-12-31",
         fill_colour="#70AD47",
         font_colour="black",
     )
 
     parallel_task.add_milestone(
-        "上綫 12月20", "2023-12-20", fill_colour="#385723", font_colour="black"
+        "上綫 12月20", "2024-12-20", fill_colour="#385723", font_colour="black"
     )
 
     group = roadmap.add_group(
         "商業智能",
         fill_colour="#4472C4",
         font_colour="black",
     )
     task = group.add_task(
         "商業智能開發",
-        "2023-04-15",
-        "2023-12-31",
+        "2024-04-15",
+        "2024-12-31",
         fill_colour="#4472C4",
         font_colour="black",
     )
 
     task.add_milestone(
-        "服務儀表板", "2023-05-15", fill_colour="#162641", font_colour="black"
+        "服務儀表板", "2024-05-15", fill_colour="#162641", font_colour="black"
     )
 
-    task.add_milestone("實時分析", "2023-08-01", fill_colour="#162641", font_colour="black")
+    task.add_milestone(
+        "實時分析", "2024-08-01", fill_colour="#162641", font_colour="black"
+    )
 
     task.add_milestone(
-        "Sales Dashboard", "2023-12-15", fill_colour="#162641", font_colour="black"
+        "Sales Dashboard", "2024-12-15", fill_colour="#162641", font_colour="black"
     )
 
     roadmap.set_footer("由 Roadmapper 生成於 " + datetime.now().strftime("%Y-%m-%d"))
     roadmap.draw()
 
     roadmap.save(output_file)
     assert os.path.exists(output_file)
@@ -394,1035 +386,993 @@
 
 def sample_roadmap(
     width: int = 1200,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "sample_roadmap.svg",
+    file_name: str = "sample_roadmap.png",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
-        width,
-        1000,
-        auto_height=True,
-        colour_theme=colour_theme,
-        show_marker=False,
-        painter_type="SVG",
+        width, 1000, auto_height=True, colour_theme=colour_theme, show_marker=False
     )
-    roadmap.set_title("STRATEGY ROADMAP 2023")
+    roadmap.set_title("STRATEGY ROADMAP 2024")
     roadmap.set_subtitle("Matariki Technologies Inc.")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
         year_fill_colour="#404040",
         year_font_colour="white",
         item_fill_colour="#404040",
         item_font_colour="white",
     )
 
     group = roadmap.add_group("Planning", fill_colour="#FFC000", font_colour="black")
     task = group.add_task(
-        "Vision", "2023-01-01", "2023-03-31", fill_colour="#FFC000", font_colour="black"
+        "Vision", "2024-01-01", "2024-03-31", fill_colour="#FFC000", font_colour="black"
     )
     task = group.add_task(
-        "Goals", "2023-02-15", "2023-03-31", fill_colour="#FFC000", font_colour="black"
+        "Goals", "2024-02-15", "2024-03-31", fill_colour="#FFC000", font_colour="black"
     )
     task.add_parallel_task(
         "Strategic Intent",
-        "2023-04-01",
-        "2023-05-31",
+        "2024-04-01",
+        "2024-05-31",
         fill_colour="#FFC000",
         font_colour="black",
     )
     task.add_parallel_task(
         "Sales Budget",
-        "2023-06-01",
-        "2023-07-15",
+        "2024-06-01",
+        "2024-07-15",
         fill_colour="#FFC000",
         font_colour="black",
     )
     task.add_parallel_task(
         "Release Plans",
-        "2023-07-16",
-        "2023-09-30",
+        "2024-07-16",
+        "2024-09-30",
         fill_colour="#FFC000",
         font_colour="black",
     )
 
     group = roadmap.add_group("Strategy", fill_colour="#ED7D31", font_colour="black")
     task = group.add_task(
         "Market Analysis",
-        "2023-02-01",
-        "2023-03-30",
+        "2024-02-01",
+        "2024-03-30",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     task.add_milestone(
-        "Competitor Review", "2023-03-30", fill_colour="#843C0C", font_colour="black"
+        "Competitor Review", "2024-03-30", fill_colour="#843C0C", font_colour="black"
     )
     task.add_parallel_task(
-        "SWOT", "2023-04-01", "2023-04-30", fill_colour="#ED7D31", font_colour="black"
+        "SWOT", "2024-04-01", "2024-04-30", fill_colour="#ED7D31", font_colour="black"
     )
     task = group.add_task(
         "Business Model",
-        "2023-04-01",
-        "2023-05-31",
+        "2024-04-01",
+        "2024-05-31",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     task.add_milestone(
-        "Price List (Draft)", "2023-06-01", fill_colour="#843C0C", font_colour="black"
+        "Price List (Draft)", "2024-06-01", fill_colour="#843C0C", font_colour="black"
     )
     parallel_task = task.add_parallel_task(
         "Price Reseach",
-        "2023-06-01",
-        "2023-08-05",
+        "2024-06-01",
+        "2024-08-05",
         fill_colour="#ED7D31",
         font_colour="black",
     )
     parallel_task.add_milestone(
-        "Price List (Final)", "2023-07-28", fill_colour="#843C0C", font_colour="black"
+        "Price List (Final)", "2024-07-28", fill_colour="#843C0C", font_colour="black"
     )
     group.add_task(
         "Objectives",
-        "2023-06-20",
-        "2023-09-10",
+        "2024-06-20",
+        "2024-09-10",
         fill_colour="#ED7D31",
         font_colour="black",
     )
 
     group.add_task(
         "Sales Trends Analysis",
-        "2023-08-15",
-        "2023-10-10",
+        "2024-08-15",
+        "2024-10-10",
         fill_colour="#ED7D31",
         font_colour="black",
     )
 
     group = roadmap.add_group(
         "Service Development", fill_colour="#70AD47", font_colour="black"
     )
     task = group.add_task(
         "Product Roadmap",
-        "2023-02-15",
-        "2023-03-31",
+        "2024-02-15",
+        "2024-03-31",
         fill_colour="#70AD47",
         font_colour="black",
     )
     parallel_task = task.add_parallel_task(
         "Development",
-        "2023-04-01",
-        "2023-08-30",
+        "2024-04-01",
+        "2024-08-30",
         fill_colour="#70AD47",
         font_colour="black",
     )
     parallel_task.add_milestone(
-        "Alpha May 20", "2023-05-20", fill_colour="#385723", font_colour="black"
+        "Alpha May 20", "2024-05-20", fill_colour="#385723", font_colour="black"
     )
     parallel_task.add_milestone(
-        "Private Beta Jul 02", "2023-07-02", fill_colour="#385723", font_colour="black"
+        "Private Beta Jul 02", "2024-07-02", fill_colour="#385723", font_colour="black"
     )
     parallel_task.add_milestone(
-        "Public Beta Aug 15", "2023-08-15", fill_colour="#385723", font_colour="black"
+        "Public Beta Aug 15", "2024-08-15", fill_colour="#385723", font_colour="black"
     )
 
     parallel_task = task.add_parallel_task(
         "Release Candidate",
-        "2023-09-01",
-        "2023-10-15",
+        "2024-09-01",
+        "2024-10-15",
         fill_colour="#70AD47",
         font_colour="black",
     )
 
     parallel_task = task.add_parallel_task(
         "Release To Public",
-        "2023-10-16",
-        "2023-12-31",
+        "2024-10-16",
+        "2024-12-31",
         fill_colour="#70AD47",
         font_colour="black",
     )
 
     parallel_task.add_milestone(
-        "Go Live Dec 20", "2023-12-20", fill_colour="#385723", font_colour="black"
+        "Go Live Dec 20", "2024-12-20", fill_colour="#385723", font_colour="black"
     )
 
     group = roadmap.add_group(
         "Business Intelligence",
         fill_colour="#4472C4",
         font_colour="black",
     )
     task = group.add_task(
         "BI Development",
-        "2023-04-15",
-        "2023-12-31",
+        "2024-04-15",
+        "2024-12-31",
         fill_colour="#4472C4",
         font_colour="black",
     )
 
     task.add_milestone(
-        "Service Dashboard", "2023-05-15", fill_colour="#162641", font_colour="black"
+        "Service Dashboard", "2024-05-15", fill_colour="#162641", font_colour="black"
     )
 
     task.add_milestone(
-        "Real-Time Analytics", "2023-08-01", fill_colour="#162641", font_colour="black"
+        "Real-Time Analytics", "2024-08-01", fill_colour="#162641", font_colour="black"
     )
 
     task.add_milestone(
-        "Sales Dashboard", "2023-12-15", fill_colour="#162641", font_colour="black"
+        "Sales Dashboard", "2024-12-15", fill_colour="#162641", font_colour="black"
     )
 
     roadmap.set_footer("Generated by Roadmapper")
     roadmap.draw()
 
     roadmap.save(output_file)
 
     assert os.path.exists(output_file)
 
 
 def colour_theme_roadmap(
     width: int = 1200,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-12-01",
+    start_date: str = "2023-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "colour_theme_roadmap.svg",
+    file_name: str = "colour_theme_roadmap.png",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
-        width,
-        1000,
-        auto_height=True,
-        colour_theme=colour_theme,
-        show_marker=True,
-        painter_type="SVG",
+        width, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
     )
-    roadmap.set_title("SAMPLE ROADMAP 2022/2023")
+    roadmap.set_title("SAMPLE ROADMAP 2023/2024")
     roadmap.set_subtitle("GodZone Corporation")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
     )
 
     group = roadmap.add_group("Core Product Work Stream", text_alignment="left")
-    task = group.add_task("Base Functionality", "2022-11-01", "2023-10-31")
-    task.add_milestone("v.1.0", "2023-02-15")
-    task.add_milestone("v.1.1", "2023-08-01")
-    parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
+    task = group.add_task("Base Functionality", "2023-11-01", "2024-10-31")
+    task.add_milestone("v.1.0", "2024-02-15")
+    task.add_milestone("v.1.1", "2024-08-01")
+    parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2024-03-31")
     parellel_task.add_milestone("v.2.0", "2024-03-30")
 
-    task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-    task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+    task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+    task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
     group = roadmap.add_group("Mobility Work Stream", text_alignment="left")
-    group.add_task("Mobile App Development", "2023-02-01", "2024-12-07")
+    group.add_task("Mobile App Development", "2024-02-01", "2024-12-07")
 
     roadmap.set_footer("Generated by Roadmapper")
     roadmap.draw()
 
     roadmap.save(output_file)
 
     assert os.path.exists(output_file)
 
 
 def custom_colour_roadmap(
     width: int = 1200,
     height: int = 1000,
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-11-01",
+    start_date: str = "2023-11-01",
     number_of_items: int = 24,
     show_marker: bool = False,
     show_generic_dates: bool = False,
-    file_name: str = "custom_colour_roadmap.svg",
+    file_name: str = "custom_colour_roadmap.png",
     colour_theme: str = "DEFAULT",
 ) -> None:
     output_file = file_name
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     roadmap = Roadmap(
         width,
         height,
         auto_height=True,
         colour_theme=colour_theme,
         show_marker=show_marker,
-        painter_type="SVG",
     )
     roadmap.set_title("My Demo Roadmap!!!")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
     )
 
     group = roadmap.add_group("Core Product Work Stream")
-    task = group.add_task("Base Functionality", "2022-11-01", "2023-10-31")
-    task.add_milestone("v.1.0", "2023-02-15")
-    task.add_milestone("v.1.1", "2023-08-01")
-    parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
+    task = group.add_task("Base Functionality", "2023-11-01", "2024-10-31")
+    task.add_milestone("v.1.0", "2024-02-15")
+    task.add_milestone("v.1.1", "2024-08-01")
+    parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2024-03-31")
     parellel_task.add_milestone("v.2.0", "2024-03-30")
 
-    task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-    task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+    task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+    task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
     group = roadmap.add_group("Mobility Work Stream")
-    group.add_task("Mobile App Development", "2023-02-01", "2024-12-07")
+    group.add_task("Mobile App Development", "2024-02-01", "2024-12-07")
 
     roadmap.set_footer("Generated by Roadmapper")
     roadmap.draw()
     roadmap.save(output_file)
 
     assert os.path.exists(output_file)
 
 
 def banner_roadmap():
-    color_theme_roadmap("../../images/color-theme01.svg", "DEFAULT")
-    color_theme_roadmap("../../images/color-theme02.svg", "GREYWOOF")
-    color_theme_roadmap("../../images/color-theme03.svg", "ORANGEPEEL")
-    color_theme_roadmap("../../images/color-theme04.svg", "BLUEMOUNTAIN")
-    color_theme_roadmap("../../images/color-theme05.svg", "GREENTURTLE")
+    color_theme_roadmap("../../images/color-theme01.png", "DEFAULT")
+    color_theme_roadmap("../../images/color-theme02.png", "GREYWOOF")
+    color_theme_roadmap("../../images/color-theme03.png", "ORANGEPEEL")
+    color_theme_roadmap("../../images/color-theme04.png", "BLUEMOUNTAIN")
+    color_theme_roadmap("../../images/color-theme05.png", "GREENTURTLE")
 
 
 def multilingual_roadmap():
-    en_NZ_roadmap("../../images/en_NZ-roadmap.svg", "../json/rainbow.json", "en_US")
+    en_NZ_roadmap("../../images/en_NZ-roadmap.png", "../json/rainbow.json", "en_US")
     zh_TW_with_locale_roadmap(
-        "../../images/zh_TW-roadmap.svg",
+        "../../images/zh_TW-roadmap.png",
         "../json/rainbow-unicode.json",
         "../json/zh_TW_timeline_settings.json",
     )
     zh_TW_roadmap(
-        "../../images/zh_TW-timeline-roadmap.svg",
+        "../../images/zh_TW-timeline-roadmap.png",
         "../json/rainbow-unicode.json",
     )
     ja_JP_roadmap(
-        "../../images/ja_JP-roadmap.svg",
+        "../../images/ja_JP-roadmap.png",
         "../json/rainbow-unicode.json",
         "../json/ja_JP_timeline_settings.json",
     )
     ko_KR_roadmap(
-        "../../images/ko-KR-roadmap.svg",
+        "../../images/ko-KR-roadmap.png",
         "../json/rainbow-unicode.json",
         "../json/ko_KR_timeline_settings.json",
     )
 
 
 ### Wiki Images
 def home_roadmap():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/my_roadmap.svg"
+    output_file = "../../images/my_roadmap.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    my_roadmap = Roadmap(width=500, height=400, painter_type="SVG")
+    my_roadmap = Roadmap(width=500, height=400)
     my_roadmap.set_title("My Roadmap")
     my_roadmap.set_timeline(
         mode=TimelineMode.MONTHLY, start="2022-11-14", number_of_items=6
     )
 
     group = my_roadmap.add_group("Development")
-    group.add_task("Activity 1", "2022-12-01", "2023-02-10")
-    group.add_task("Activity 2", "2023-01-11", "2023-03-20")
-    group.add_task("Activity 3", "2023-01-21", "2023-06-30")
+    group.add_task("Activity 1", "2022-12-01", "2024-02-10")
+    group.add_task("Activity 2", "2024-01-11", "2024-03-20")
+    group.add_task("Activity 3", "2024-01-21", "2024-06-30")
 
     my_roadmap.set_footer("Generated by Roadmapper")
     my_roadmap.draw()
     my_roadmap.save(output_file)
     assert os.path.exists(output_file)
 
 
 def readme_roadmap():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/demo01.svg"
+    output_file = "../../images/demo01.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN", painter_type="SVG")
+    roadmap = Roadmap(1200, 400, colour_theme="BLUEMOUNTAIN")
     roadmap.set_title("My Demo Roadmap")
     roadmap.set_subtitle("Matariki Technologies Ltd")
-    roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=12)
+    roadmap.set_timeline(TimelineMode.MONTHLY, start="2024-01-01", number_of_items=12)
     roadmap.add_logo(
         "../../images/logo/matariki-tech-logo.png",
         position="top-right",
         width=50,
         height=50,
     )
 
     group = roadmap.add_group("Core Product Work Stream")
 
-    task = group.add_task("Base Functionality", "2023-01-01", "2023-10-31")
-    task.add_milestone("v.1.0", "2023-02-15")
-    task.add_milestone("v.1.1", "2023-08-01")
+    task = group.add_task("Base Functionality", "2024-01-01", "2024-10-31")
+    task.add_milestone("v.1.0", "2024-02-15")
+    task.add_milestone("v.1.1", "2024-08-01")
 
-    parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
+    parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2024-03-31")
     parellel_task.add_milestone("v.2.0", "2024-03-30")
 
-    task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-    task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+    task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+    task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
     roadmap.set_footer("Generated by Roadmapper")
     roadmap.draw()
     roadmap.save(output_file)
     assert os.path.exists(output_file)
 
 
 def color_theme_roadmap(filename: str, colour_theme: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(
-        600, 500, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
-    )
+    roadmap = Roadmap(600, 500, colour_theme=colour_theme, show_marker=True)
     roadmap.set_title("My Demo Roadmap")
-    roadmap.set_timeline(TimelineMode.QUARTERLY, start="2023-01-01", number_of_items=4)
+    roadmap.set_timeline(TimelineMode.QUARTERLY, start="2024-07-01", number_of_items=4)
     roadmap.set_footer("Generated by Roadmapper")
 
     group = roadmap.add_group("Workstream 1")
-    task = group.add_task("Task 1-A", "2023-01-01", "2023-04-30")
-    task.add_parallel_task("Task 2-B", "2023-05-15", "2023-08-30")
-    group.add_task("Task 3-C", "2023-04-01", "2023-06-30")
+    task = group.add_task("Task 1-A", "2024-07-01", "2024-10-30")
+    task.add_parallel_task("Task 2-B", "2024-11-15", "2024-02-28")
+    group.add_task("Task 3-C", "2024-10-01", "2024-12-31")
 
     group = roadmap.add_group("Workstream 2")
-    group.add_task("Task 2-A", "2023-04-01", "2023-06-30")
-    group.add_task("Task 2-B", "2023-05-01", "2023-07-30")
-    group.add_task("Task 2-C", "2023-06-01", "2023-08-30")
+    group.add_task("Task 2-A", "2024-10-01", "2024-12-30")
+    group.add_task("Task 2-B", "2024-11-01", "2024-01-30")
+    group.add_task("Task 2-C", "2024-12-01", "2024-02-28")
 
     roadmap.draw()
     roadmap.save(filename)
     assert os.path.exists(output_file)
 
 
 def en_NZ_roadmap(filename: str, colour_theme: str, locale_name: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(
-        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
-    )
-    roadmap.set_title("Strategy Roadmap 2023")
+    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap.set_title("Strategy Roadmap 2024")
     roadmap.set_subtitle("Matariki Technologies Ltd")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
-        start="2023-01-01",
+        start="2024-01-01",
         number_of_items=4,
         timeline_locale=locale_name,
     )
     roadmap.set_footer("Generated by Roadmapper")
 
     group = roadmap.add_group("People Stream")
-    task = group.add_task("Develop Inclusion Strategy", "2023-01-01", "2023-04-30")
+    task = group.add_task("Develop Inclusion Strategy", "2024-01-01", "2024-04-30")
     task.add_parallel_task(
-        "Promote diversity, equity, and inclusion", "2023-05-01", "2023-12-30"
+        "Promote diversity, equity, and inclusion", "2024-05-01", "2024-12-30"
     )
-    group.add_task("Implement a sustainability programme", "2023-03-01", "2023-11-30")
+    group.add_task("Implement a sustainability programme", "2024-03-01", "2024-11-30")
 
     group = roadmap.add_group("Process Stream")
     group.add_task(
-        "Implement Business Improvement Programme", "2023-02-01", "2023-11-30"
+        "Implement Business Improvement Programme", "2024-02-01", "2024-11-30"
     )
-    task = group.add_task("Automate processes", "2023-07-01", "2023-12-30")
-    task.add_milestone("30% Automated ", "2023-8-01")
-    task.add_milestone("60% Automated ", "2023-12-01")
+    task = group.add_task("Automate processes", "2024-07-01", "2024-12-30")
+    task.add_milestone("30% Automated ", "2024-8-01")
+    task.add_milestone("60% Automated ", "2024-12-01")
 
     group = roadmap.add_group("Tool Stream")
-    group.add_task("Implement strategy", "2023-01-01", "2023-04-30")
-    group.add_task("Tools Selection", "2023-02-01", "2023-08-30")
-    task = group.add_task("Centralized Tool Administration", "2023-04-01", "2023-11-30")
-    task.add_milestone("Admin Centralised", "2023-12-01")
+    group.add_task("Implement strategy", "2024-01-01", "2024-04-30")
+    group.add_task("Tools Selection", "2024-02-01", "2024-08-30")
+    task = group.add_task("Centralized Tool Administration", "2024-04-01", "2024-11-30")
+    task.add_milestone("Admin Centralised", "2024-12-01")
 
     roadmap.draw()
     roadmap.save(filename)
     assert os.path.exists(output_file)
 
 
 def zh_TW_with_locale_roadmap(filename: str, colour_theme: str, locale_name: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(
-        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
-    )
-    roadmap.set_title("戰略路線圖 2023")
+    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap.set_title("戰略路線圖 2024")
     roadmap.set_subtitle("瑪塔里奇太陽科技有限公司")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
-        start="2023-01-01",
+        start="2024-01-01",
         number_of_items=4,
         timeline_locale=locale_name,
     )
     roadmap.set_footer("由 Roadmapper 生成")
 
     group = roadmap.add_group("人員流程")
-    task = group.add_task("制定包容戰略", "2023-01-01", "2023-04-30")
-    task.add_parallel_task("促進多樣性、公平性和包容性", "2023-05-01", "2023-12-30")
-    group.add_task("實施可持續發展計劃", "2023-03-01", "2023-11-30")
+    task = group.add_task("制定包容戰略", "2024-01-01", "2024-04-30")
+    task.add_parallel_task("促進多樣性、公平性和包容性", "2024-05-01", "2024-12-30")
+    group.add_task("實施可持續發展計劃", "2024-03-01", "2024-11-30")
 
     group = roadmap.add_group("工作流程")
-    group.add_task("實施業務改進計劃", "2023-02-01", "2023-11-30")
-    task = group.add_task("自動化流程", "2023-07-01", "2023-12-30")
-    task.add_milestone("30%自動化 ", "2023-8-01")
-    task.add_milestone("60%自動化 ", "2023-12-01")
+    group.add_task("實施業務改進計劃", "2024-02-01", "2024-11-30")
+    task = group.add_task("自動化流程", "2024-07-01", "2024-12-30")
+    task.add_milestone("30%自動化 ", "2024-8-01")
+    task.add_milestone("60%自動化 ", "2024-12-01")
 
     group = roadmap.add_group("工具流程")
-    group.add_task("實施工具選擇策略", "2023-01-01", "2023-04-30")
-    group.add_task("工具選擇", "2023-02-01", "2023-08-30")
-    task = group.add_task("集中工具管理", "2023-04-01", "2023-11-30")
-    task.add_milestone("系統集中完成", "2023-12-01")
+    group.add_task("實施工具選擇策略", "2024-01-01", "2024-04-30")
+    group.add_task("工具選擇", "2024-02-01", "2024-08-30")
+    task = group.add_task("集中工具管理", "2024-04-01", "2024-11-30")
+    task.add_milestone("系統集中完成", "2024-12-01")
 
     roadmap.draw()
     roadmap.save(filename)
     assert os.path.exists(output_file)
 
 
 def zh_TW_roadmap(filename: str, colour_theme: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(
-        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
-    )
-    roadmap.set_title("戰略路線圖 2023")
+    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap.set_title("戰略路線圖 2024")
     roadmap.set_subtitle("瑪塔里奇太陽科技有限公司")
-    roadmap.set_timeline(TimelineMode.QUARTERLY, start="2023-01-01", number_of_items=4)
+    roadmap.set_timeline(TimelineMode.QUARTERLY, start="2024-01-01", number_of_items=4)
     roadmap.set_footer("由 Roadmapper 生成")
 
     group = roadmap.add_group("人員流程")
-    task = group.add_task("制定包容戰略", "2023-01-01", "2023-04-30")
-    task.add_parallel_task("促進多樣性、公平性和包容性", "2023-05-01", "2023-12-30")
-    group.add_task("實施可持續發展計劃", "2023-03-01", "2023-11-30")
+    task = group.add_task("制定包容戰略", "2024-01-01", "2024-04-30")
+    task.add_parallel_task("促進多樣性、公平性和包容性", "2024-05-01", "2024-12-30")
+    group.add_task("實施可持續發展計劃", "2024-03-01", "2024-11-30")
 
     group = roadmap.add_group("工作流程")
-    group.add_task("實施業務改進計劃", "2023-02-01", "2023-11-30")
-    task = group.add_task("自動化流程", "2023-07-01", "2023-12-30")
-    task.add_milestone("30%自動化 ", "2023-8-01")
-    task.add_milestone("60%自動化 ", "2023-12-01")
+    group.add_task("實施業務改進計劃", "2024-02-01", "2024-11-30")
+    task = group.add_task("自動化流程", "2024-07-01", "2024-12-30")
+    task.add_milestone("30%自動化 ", "2024-8-01")
+    task.add_milestone("60%自動化 ", "2024-12-01")
 
     group = roadmap.add_group("工具流程")
-    group.add_task("實施工具選擇策略", "2023-01-01", "2023-04-30")
-    group.add_task("工具選擇", "2023-02-01", "2023-08-30")
-    task = group.add_task("集中工具管理", "2023-04-01", "2023-11-30")
-    task.add_milestone("系統集中完成", "2023-12-01")
+    group.add_task("實施工具選擇策略", "2024-01-01", "2024-04-30")
+    group.add_task("工具選擇", "2024-02-01", "2024-08-30")
+    task = group.add_task("集中工具管理", "2024-04-01", "2024-11-30")
+    task.add_milestone("系統集中完成", "2024-12-01")
 
     roadmap.draw()
     roadmap.save(filename)
     assert os.path.exists(output_file)
 
 
 def ja_JP_roadmap(filename: str, colour_theme: str, locale_name: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(
-        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
-    )
-    roadmap.set_title("戦略的ロードマップ 2023")
+    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap.set_title("戦略的ロードマップ 2024")
     roadmap.set_subtitle("マタリッチサンテクノロジー株式会社")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
-        start="2023-01-01",
+        start="2024-01-01",
         number_of_items=4,
         timeline_locale=locale_name,
     )
     roadmap.set_footer("ロードマッパーによって生成")
 
     group = roadmap.add_group("人事プロセス")
-    task = group.add_task("インクルージョン戦略を策定する", "2023-01-01", "2023-04-30")
-    task.add_parallel_task("多様性、公平性、包括性の促進", "2023-05-01", "2023-12-30")
-    group.add_task("持続可能な開発計画の実施", "2023-03-01", "2023-11-30")
+    task = group.add_task("インクルージョン戦略を策定する", "2024-01-01", "2024-04-30")
+    task.add_parallel_task("多様性、公平性、包括性の促進", "2024-05-01", "2024-12-30")
+    group.add_task("持続可能な開発計画の実施", "2024-03-01", "2024-11-30")
 
     group = roadmap.add_group("作業過程")
-    group.add_task("業務改善計画の実施", "2023-02-01", "2023-11-30")
-    task = group.add_task("自動化されたプロセス", "2023-07-01", "2023-12-30")
-    task.add_milestone("30%自動化", "2023-8-01")
-    task.add_milestone("60%自動化", "2023-12-01")
+    group.add_task("業務改善計画の実施", "2024-02-01", "2024-11-30")
+    task = group.add_task("自動化されたプロセス", "2024-07-01", "2024-12-30")
+    task.add_milestone("30%自動化", "2024-8-01")
+    task.add_milestone("60%自動化", "2024-12-01")
 
     group = roadmap.add_group("ツールフロー")
-    group.add_task("ツール選択戦略を実装する", "2023-01-01", "2023-04-30")
-    group.add_task("ツールの選択", "2023-02-01", "2023-08-30")
-    task = group.add_task("集中ツール管理", "2023-04-01", "2023-11-30")
-    task.add_milestone("システムは集中型", "2023-12-01")
+    group.add_task("ツール選択戦略を実装する", "2024-01-01", "2024-04-30")
+    group.add_task("ツールの選択", "2024-02-01", "2024-08-30")
+    task = group.add_task("集中ツール管理", "2024-04-01", "2024-11-30")
+    task.add_milestone("システムは集中型", "2024-12-01")
 
     roadmap.draw()
     roadmap.save(filename)
     assert os.path.exists(output_file)
 
 
 def ko_KR_roadmap(filename: str, colour_theme: str, locale_name: str):
     output_file = filename
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(
-        800, 700, colour_theme=colour_theme, show_marker=True, painter_type="SVG"
-    )
-    roadmap.set_title("전략 로드맵 2023")
+    roadmap = Roadmap(800, 700, colour_theme=colour_theme, show_marker=True)
+    roadmap.set_title("전략 로드맵 2024")
     roadmap.set_subtitle("마타리키 테크놀로지스")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
-        start="2023-01-01",
+        start="2024-01-01",
         number_of_items=4,
         timeline_locale=locale_name,
     )
     roadmap.set_footer("로드매퍼에서 생성")
 
     group = roadmap.add_group("인사 프로세스")
-    task = group.add_task("포함 전략을 수립", "2023-01-01", "2023-04-30")
-    task.add_parallel_task("다양성, 공정성, 포괄성 촉진", "2023-05-01", "2023-12-30")
-    group.add_task("지속 가능한 개발 계획 실시", "2023-03-01", "2023-11-30")
+    task = group.add_task("포함 전략을 수립", "2024-01-01", "2024-04-30")
+    task.add_parallel_task("다양성, 공정성, 포괄성 촉진", "2024-05-01", "2024-12-30")
+    group.add_task("지속 가능한 개발 계획 실시", "2024-03-01", "2024-11-30")
 
     group = roadmap.add_group("작업 과정")
-    group.add_task("업무 개선 계획 실시", "2023-02-01", "2023-11-30")
-    task = group.add_task("자동화된 프로세스", "2023-07-01", "2023-12-30")
-    task.add_milestone("30% 자동화", "2023-8-01")
-    task.add_milestone("60% 자동화", "2023-12-01")
+    group.add_task("업무 개선 계획 실시", "2024-02-01", "2024-11-30")
+    task = group.add_task("자동화된 프로세스", "2024-07-01", "2024-12-30")
+    task.add_milestone("30% 자동화", "2024-8-01")
+    task.add_milestone("60% 자동화", "2024-12-01")
 
     group = roadmap.add_group("공구 흐름")
-    group.add_task("도구 선택 전략 구현", "2023-01-01", "2023-04-30")
-    group.add_task("도구 선택", "2023-02-01", "2023-08-30")
-    task = group.add_task("중앙 집중식 도구 관리", "2023-04-01", "2023-11-30")
-    task.add_milestone("시스템은 중앙 집중식", "2023-12-01")
+    group.add_task("도구 선택 전략 구현", "2024-01-01", "2024-04-30")
+    group.add_task("도구 선택", "2024-02-01", "2024-08-30")
+    task = group.add_task("중앙 집중식 도구 관리", "2024-04-01", "2024-11-30")
+    task.add_milestone("시스템은 중앙 집중식", "2024-12-01")
 
     roadmap.draw()
     roadmap.save(filename)
     assert os.path.exists(output_file)
 
 
 ### Test case functions ###
 
 
 def test_sample_case1():
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
     colour_theme_demo(
         width=2500,
-        file_name="../../images/test/test-ORANGEPEEL-weekly.svg",
+        file_name="../../images/test/test-ORANGEPEEL-weekly.png",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.WEEKLY,
         number_of_items=52,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
 
 def test_sample_case2():
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
     colour_theme_demo(
-        file_name="../../images/test/test-ORANGEPEEL-monthly.svg",
+        file_name="../../images/test/test-ORANGEPEEL-monthly.png",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
 
 def test_sample_case3():
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
     colour_theme_demo(
-        file_name="../../images/test/test-ORANGEPEEL-quarter.svg",
+        file_name="../../images/test/test-ORANGEPEEL-quarter.png",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.QUARTERLY,
         number_of_items=4,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
 
 def test_sample_unicase1():
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
     unicode_demo(
-        file_name="../../images/test/test-unicode-monthly.svg",
+        file_name="../../images/test/test-unicode-monthly.png",
         # colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
     assert True
 
 
 def test_draw_anatomy():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/roadmapper-anatomy-base.svg"
+    output_file = "../../images/roadmapper-anatomy-base.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(
-        1200, 380, colour_theme="BLUEMOUNTAIN", show_marker=True, painter_type="SVG"
-    )
+    roadmap = Roadmap(1200, 380, colour_theme="BLUEMOUNTAIN", show_marker=True)
     roadmap.set_title("Product Roadmap")
     roadmap.set_subtitle("Matariki Tech Ltd")
-    roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01", number_of_items=9)
+    roadmap.set_timeline(TimelineMode.MONTHLY, start="2024-01-01", number_of_items=9)
     roadmap.set_footer("Generated by Roadmapper")
 
     group = roadmap.add_group("Workstream 1")
-    task = group.add_task("Task 1-A", "2023-01-01", "2023-05-15")
-    task.add_parallel_task("Task 2-B", "2023-05-16", "2023-08-30")
-    task = group.add_task("Task 3-C", "2023-04-01", "2023-06-30")
-    task.add_milestone("Milestone 1", "2023-06-30")
+    task = group.add_task("Task 1-A", "2024-01-01", "2024-05-15")
+    task.add_parallel_task("Task 2-B", "2024-05-16", "2024-08-30")
+    task = group.add_task("Task 3-C", "2024-04-01", "2024-06-30")
+    task.add_milestone("Milestone 1", "2024-06-30")
 
     roadmap.draw()
 
     roadmap.save(output_file)
     assert os.path.exists(output_file)
 
 
 def test_draw_banner_theme():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/theme-demo01.svg"
+    output_file = "../../images/theme-demo01.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(
-        600, 380, colour_theme="BLUEMOUNTAIN", show_marker=True, painter_type="SVG"
-    )
+    roadmap = Roadmap(600, 380, colour_theme="BLUEMOUNTAIN", show_marker=True)
     roadmap.set_title("My Demo Roadmap")
-    roadmap.set_timeline(TimelineMode.QUARTERLY, start="2023-01-01", number_of_items=4)
+    roadmap.set_timeline(TimelineMode.QUARTERLY, start="2024-01-01", number_of_items=4)
     roadmap.set_footer("Generated by Roadmapper")
 
     group = roadmap.add_group("Workstream 1")
-    task = group.add_task("Task 1-A", "2023-01-01", "2023-04-30")
-    task.add_parallel_task("Task 2-B", "2023-05-15", "2023-08-30")
-    group.add_task("Task 3-C", "2023-04-01", "2023-06-30")
+    task = group.add_task("Task 1-A", "2024-01-01", "2024-04-30")
+    task.add_parallel_task("Task 2-B", "2024-05-15", "2024-08-30")
+    group.add_task("Task 3-C", "2024-04-01", "2024-06-30")
 
     group = roadmap.add_group("Workstream 2")
-    group.add_task("Task 2-A", "2023-04-01", "2023-06-30")
-    group.add_task("Task 2-B", "2023-05-01", "2023-07-30")
-    group.add_task("Task 2-C", "2023-06-01", "2023-08-30")
+    group.add_task("Task 2-A", "2024-04-01", "2024-06-30")
+    group.add_task("Task 2-B", "2024-05-01", "2024-07-30")
+    group.add_task("Task 2-C", "2024-06-01", "2024-08-30")
 
     roadmap.draw()
     roadmap.save(output_file)
     assert os.path.exists(output_file)
 
 
 def test_draw_banner():
     if not os.path.exists("images"):
         os.mkdir("images")
 
-    output_file = "../../images/demo01.svg"
+    output_file = "../../images/demo01.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
-    roadmap = Roadmap(600, 500, show_marker=False, auto_height=True, painter_type="SVG")
+    roadmap = Roadmap(600, 500, show_marker=False, auto_height=True)
     roadmap.set_title("My Demo Roadmap")
     roadmap.set_timeline(
         TimelineMode.QUARTERLY,
-        start="2023-01-01",
+        start="2024-01-01",
         number_of_items=3,
         year_fill_colour="#7CC1AC",
         year_font_colour="black",
         item_fill_colour="#7CC1AC",
         item_font_colour="black",
     )
     roadmap.set_footer("Generated by Roadmapper")
     group = roadmap.add_group(
         "Workstream 1", font_colour="black", fill_colour="#C38D9D", font_size=12
     )
     task = group.add_task(
         "Task 1-A",
-        "2023-01-01",
-        "2023-04-30",
+        "2024-01-01",
+        "2024-04-30",
         font_colour="black",
         fill_colour="#D7B3BD",
     )
     task.add_parallel_task(
         "Task 2-B",
-        "2023-05-15",
-        "2023-08-30",
+        "2024-05-15",
+        "2024-08-30",
         font_colour="black",
         fill_colour="#D7B3BD",
     )
     group.add_task(
         "Task 3-C",
-        "2023-04-01",
-        "2023-06-30",
+        "2024-04-01",
+        "2024-06-30",
         font_colour="black",
         fill_colour="#D7B3BD",
     )
 
     group = roadmap.add_group(
         "Workstream 2", font_colour="black", fill_colour="#E8A87C", font_size=12
     )
     group.add_task(
         "Task 2-A",
-        "2023-04-01",
-        "2023-06-30",
+        "2024-04-01",
+        "2024-06-30",
         font_colour="black",
         fill_colour="#EFC5A7",
     )
     group.add_task(
         "Task 2-B",
-        "2023-05-01",
-        "2023-07-30",
+        "2024-05-01",
+        "2024-07-30",
         font_colour="black",
         fill_colour="#EFC5A7",
     )
     group.add_task(
         "Task 2-C",
-        "2023-06-01",
-        "2023-08-30",
+        "2024-06-01",
+        "2024-08-30",
         font_colour="black",
         fill_colour="#EFC5A7",
     )
 
     roadmap.draw()
     roadmap.save(output_file)
     assert os.path.exists(output_file)
 
 
 def test_gallery_images():
     ### Sample Roadmap ###
     sample_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-sample-01.svg",
+        file_name="../../images/gallery/gallery-sample-01.png",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
     ### Colour Theme Roadmap ###
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-DEFAULT-monthly.svg",
+        file_name="../../images/gallery/gallery-DEFAULT-monthly.png",
         # colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-ORANGEPEEL-monthly.svg",
+        file_name="../../images/gallery/gallery-ORANGEPEEL-monthly.png",
         colour_theme="ORANGEPEEL",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-BLUEMOUNTAIN-monthly.svg",
+        file_name="../../images/gallery/gallery-BLUEMOUNTAIN-monthly.png",
         colour_theme="BLUEMOUNTAIN",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-GREENTURTLE-monthly.svg",
+        file_name="../../images/gallery/gallery-GREENTURTLE-monthly.png",
         colour_theme="GREENTURTLE",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
     colour_theme_roadmap(
-        file_name="../../images/gallery/gallery-GREYWOOF-monthly.svg",
+        file_name="../../images/gallery/gallery-GREYWOOF-monthly.png",
         colour_theme="GREYWOOF",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
     )
 
     ### Marker Roadmap ###
     custom_colour_roadmap(
         width=1200,
-        file_name="../../images/gallery/gallery-marker-monthly.svg",
+        file_name="../../images/gallery/gallery-marker-monthly.png",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2022-11-01",
+        start_date="2023-11-01",
         show_marker=True,
         show_generic_dates=False,
     )
 
     ### WEEKLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=2400,
-        file_name="../../images/gallery/gallery-DEFAULT-weekly.svg",
+        file_name="../../images/gallery/gallery-DEFAULT-weekly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.WEEKLY,
         number_of_items=52,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
         show_generic_dates=False,
     )
 
     ### QUARTERLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-DEFAULT-quarterly.svg",
+        file_name="../../images/gallery/gallery-DEFAULT-quarterly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.QUARTERLY,
         number_of_items=6,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
         show_generic_dates=False,
     )
 
     ### HALF-YEARLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-DEFAULT-halfyearly.svg",
+        file_name="../../images/gallery/gallery-DEFAULT-halfyearly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.HALF_YEARLY,
         number_of_items=4,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
         show_generic_dates=False,
     )
 
     ### YEARLY Timeline Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-DEFAULT-yearly.svg",
+        file_name="../../images/gallery/gallery-DEFAULT-yearly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.YEARLY,
         number_of_items=2,
         start_date="2023-01-01",
         show_generic_dates=False,
     )
 
     ### Generic Dates Roadmap ###
     colour_theme_roadmap(
         width=1400,
-        file_name="../../images/gallery/gallery-DEFAULT-generic-monthly.svg",
+        file_name="../../images/gallery/gallery-DEFAULT-generic-monthly.png",
         colour_theme="DEFAULT",
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=12,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
         show_generic_dates=True,
     )
 
 
 def test_draw_wiki_roadmap():
     readme_roadmap()
     home_roadmap()
     banner_roadmap()
     multilingual_roadmap()
 
 
 def test_with_context_manager():
     with Roadmap(
-        1200,
-        500,
-        show_marker=False,
-        auto_height=True,
-        colour_theme="ORANGEPEEL",
-        painter_type="SVG",
+        1200, 500, show_marker=False, auto_height=True, colour_theme="ORANGEPEEL"
     ) as my_roadmap:
         my_roadmap.set_title("Context Manager Test Roadmap")
-        my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01")
+        my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2024-01-01")
         with my_roadmap.add_group("Workstream 1") as group1:
             with group1.add_task(
                 "Task 1-A",
-                "2023-01-01",
-                "2023-04-30",
+                "2024-01-01",
+                "2024-04-30",
             ) as task1:
                 with task1.add_parallel_task(
                     "Task 2-B",
-                    "2023-05-15",
-                    "2023-08-30",
+                    "2024-05-15",
+                    "2024-08-30",
                 ) as parallel_task1:
-                    parallel_task1.add_milestone("Milestone 2", "2023-08-10")
+                    parallel_task1.add_milestone("Milestone 2", "2024-07-10")
                 task1.add_milestone(
                     "Milestone 1",
-                    "2023-04-01",
+                    "2024-04-01",
                 )
         my_roadmap.draw()
-        my_roadmap.save("../../images/with_context_manager.svg")
+        my_roadmap.save("../../images/with_context_manager.png")
 
 
 def test_black_blackground():
     with Roadmap(
-        1200,
-        500,
-        show_marker=False,
-        auto_height=True,
-        colour_theme="ORANGEPEEL",
-        painter_type="SVG",
+        1200, 500, show_marker=False, auto_height=True, colour_theme="ORANGEPEEL"
     ) as my_roadmap:
         my_roadmap.set_background_colour("black")
         my_roadmap.set_title("Black Background Test Roadmap")
-        my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01")
+        my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2024-01-01")
         with my_roadmap.add_group("Workstream 1") as group1:
             with group1.add_task(
                 "Task 1-A",
-                "2023-01-01",
-                "2023-04-30",
+                "2024-01-01",
+                "2024-04-30",
             ) as task1:
                 with task1.add_parallel_task(
                     "Task 2-B",
-                    "2023-05-15",
-                    "2023-08-30",
+                    "2024-05-15",
+                    "2024-08-30",
                 ) as parallel_task1:
-                    parallel_task1.add_milestone("Milestone 2", "2023-08-10")
+                    parallel_task1.add_milestone("Milestone 2", "2024-08-10")
                 task1.add_milestone(
                     "Milestone 1",
-                    "2023-04-01",
+                    "2024-04-01",
                 )
         my_roadmap.draw()
-        my_roadmap.save("../../images/black_roadmap.svg")
+        my_roadmap.save("../../images/black_roadmap.png")
 
 
 def test_transparent_blackground():
     with Roadmap(
-        1200,
-        500,
-        show_marker=False,
-        auto_height=True,
-        colour_theme="ORANGEPEEL",
-        painter_type="SVG",
+        1200, 500, show_marker=False, auto_height=True, colour_theme="ORANGEPEEL"
     ) as my_roadmap:
         my_roadmap.set_background_colour("transparent")
         my_roadmap.set_title("Transparent Background Test Roadmap")
-        my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2023-01-01")
+        my_roadmap.set_timeline(TimelineMode.MONTHLY, start="2024-01-01")
         with my_roadmap.add_group("Workstream 1") as group1:
             with group1.add_task(
                 "Task 1-A",
-                "2023-01-01",
-                "2023-04-30",
+                "2024-01-01",
+                "2024-04-30",
             ) as task1:
                 with task1.add_parallel_task(
                     "Task 2-B",
-                    "2023-05-15",
-                    "2023-08-30",
+                    "2024-05-15",
+                    "2024-08-30",
                 ) as parallel_task1:
-                    parallel_task1.add_milestone("Milestone 2", "2023-08-10")
+                    parallel_task1.add_milestone("Milestone 2", "2024-08-10")
                 task1.add_milestone(
                     "Milestone 1",
-                    "2023-04-01",
+                    "2024-04-01",
                 )
         my_roadmap.draw()
-        my_roadmap.save("../../images/transparent_roadmap.svg")
+        my_roadmap.save("../../images/transparent_roadmap.png")
```

### Comparing `roadmapper-1.4.0/src/tests/test_milestone.py` & `roadmapper-1.5.0/src/tests/test_milestone.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/test_painter.py` & `roadmapper-1.5.0/src/tests/test_painter.py`

 * *Files identical despite different names*

### Comparing `roadmapper-1.4.0/src/tests/test_roadmapper.py` & `roadmapper-1.5.0/src/tests/test_roadmapper_svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,25 @@
 
 
 def colour_theme_demo(
     mode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        1200,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("SAMPLE ROADMAP 2022/2023")
     roadmap.set_subtitle("ABC Corporation")
     roadmap.set_timeline(
         mode,
         start_date,
         number_of_items,
@@ -48,19 +53,24 @@
 
 
 def colour_theme_demo_without_locale(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     roadmap = Roadmap(
-        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        1200,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("SAMPLE ROADMAP 2022/2023")
     roadmap.set_subtitle("ABC Corporation")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -88,20 +98,25 @@
 
 def chinese_theme_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
     show_first_day_of_week=False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        1200,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("示例路線圖 2022/2023")
     roadmap.set_subtitle("甲乙丙有限公司")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -131,20 +146,25 @@
 
 def japanese_theme_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
     show_first_day_of_week=False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
+        1200,
+        1000,
+        auto_height=True,
+        colour_theme=colour_theme,
+        show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("ロードマップの例 2022/2023")
     roadmap.set_subtitle("株式会社エー・ビー・シー")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -174,18 +194,20 @@
 
 def generic_date_test(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-11-01",
     number_of_items: int = 24,
     show_generic_dates: bool = False,
     show_first_day_of_week: bool = False,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
-    roadmap = Roadmap(4400, 2000, colour_theme=colour_theme, show_marker=True)
+    roadmap = Roadmap(
+        4400, 2000, colour_theme=colour_theme, show_marker=True, painter_type="svg"
+    )
     roadmap.set_title("My Demo Roadmap!!!")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
         show_first_day_of_week=show_first_day_of_week,
@@ -209,23 +231,24 @@
     roadmap.save(file_name)
 
 
 def parallel_task_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2022-12-01",
     number_of_items: int = 14,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "DEFAULT",
 ) -> None:
     roadmap = Roadmap(
         1200,
         612,
         auto_height=False,
         colour_theme=colour_theme,
         show_marker=True,
+        painter_type="svg",
     )
     roadmap.set_title("ROADMAP EXAMPLE 2022/2023")
     roadmap.set_subtitle("This is a subtitle")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -250,24 +273,24 @@
     roadmap.save(file_name)
 
 
 def singleton_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2023-01-01",
     number_of_items: int = 2,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "BLUEMOUNTAIN",
 ) -> None:
-
     roadmap = Roadmap(
         600,
         612,
         auto_height=True,
         colour_theme=colour_theme,
         show_marker=False,
+        painter_type="svg",
     )
     roadmap.set_title("ROADMAP EXAMPLE")
     # roadmap.set_subtitle("This is a subtitle")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
@@ -287,26 +310,27 @@
     roadmap.save(file_name)
 
 
 def logo_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
     start_date: str = "2023-01-01",
     number_of_items: int = 2,
-    file_name: str = "demo01.png",
+    file_name: str = "demo01.svg",
     colour_theme: str = "BLUEMOUNTAIN",
     auto_height: bool = True,
     logo_position: str = "top-left",
 ) -> None:
     file_name = "T_" + file_name
     roadmap = Roadmap(
         800,
         612,
         auto_height=auto_height,
         colour_theme=colour_theme,
         show_marker=False,
+        painter_type="svg",
     )
     frameinfo = inspect.getframeinfo(inspect.currentframe())
     title = f"{frameinfo.function}(), theme={colour_theme}, mode={timelinemode}"
 
     roadmap.add_logo("../../images/logo/matariki-tech-logo.png", logo_position, 50, 50)
     roadmap.set_title(title)
     roadmap.set_subtitle("This is a subtitle")
@@ -331,57 +355,56 @@
 def test_dev():
     if not os.path.exists("images"):
         os.mkdir("images")
 
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
 
-    output_file = "../../images/test/colour_theme_demo_without_locale.png"
+    output_file = "../../images/test/colour_theme_demo_without_locale.svg"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     colour_theme_demo_without_locale(
         file_name=output_file,
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=14,
     )
 
     assert os.path.exists(output_file)
 
-    output_file = "../../images/test/demo-my-colour-chinese.png"
+    output_file = "../../images/test/demo-my-colour-chinese.svg"
     chinese_theme_demo(
         file_name=output_file,
         colour_theme="../json/chinese.json",
         timelinemode=TimelineMode.WEEKLY,
         start_date="2023-01-01",
         number_of_items=14,
         locale_name="../json/zh_TW_timeline_settings.json",
         show_generic_dates=False,
         show_first_day_of_week=True,
     )
     assert os.path.exists(output_file)
 
-    output_file = "../../images/test/demo-my-colour-japanese.png"
+    output_file = "../../images/test/demo-my-colour-japanese.svg"
     japanese_theme_demo(
         file_name=output_file,
         colour_theme="../json/chinese.json",
         timelinemode=TimelineMode.MONTHLY,
         start_date="2023-01-01",
         number_of_items=14,
         locale_name="../json/ja_JP_timeline_settings.json",
         show_generic_dates=False,
         show_first_day_of_week=True,
     )
 
     assert os.path.exists(output_file)
 
 
-
 # check if calling from main
 if __name__ == "__main__":
-    output_file = "../../images/test/colour_theme_demo_without_locale.png"
+    output_file = "../../images/test/colour_theme_demo_without_locale.svg"
     colour_theme_demo_without_locale(
         file_name=output_file,
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=14,
-    )
+    )
```

### Comparing `roadmapper-1.4.0/src/tests/test_roadmapper_svg.py` & `roadmapper-1.5.0/src/tests/test_roadmapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,333 +4,307 @@
 from src.roadmapper.roadmap import Roadmap
 from src.roadmapper.timelinemode import TimelineMode
 import inspect
 
 
 def colour_theme_demo(
     mode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-12-01",
+    start_date: str = "2023-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "demo01.svg",
+    file_name: str = "demo01.png",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200,
-        1000,
-        auto_height=True,
-        colour_theme=colour_theme,
-        show_marker=True,
-        painter_type="svg",
+        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
     )
-    roadmap.set_title("SAMPLE ROADMAP 2022/2023")
+    roadmap.set_title("SAMPLE ROADMAP 2023/2024")
     roadmap.set_subtitle("ABC Corporation")
     roadmap.set_timeline(
         mode,
         start_date,
         number_of_items,
         show_generic_dates=show_generic_dates,
         timeline_locale=locale_name,
     )
 
     group = roadmap.add_group("Core Product Work Stream", text_alignment="left")
-    task = group.add_task("Base Functionality", "2022-11-01", "2023-10-31")
-    task.add_milestone("v.1.0", "2023-02-15")
-    task.add_milestone("v.1.1", "2023-08-01")
-    parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
-    parellel_task.add_milestone("v.2.0", "2024-03-30")
+    task = group.add_task("Base Functionality", "2023-11-01", "2024-10-31")
+    task.add_milestone("v.1.0", "2024-02-15")
+    task.add_milestone("v.1.1", "2024-08-01")
+    parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2025-03-31")
+    parellel_task.add_milestone("v.2.0", "2025-03-30")
 
-    task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-    task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+    task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+    task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
     group = roadmap.add_group("Mobility Work Stream", text_alignment="left")
-    group.add_task("Mobile App Development", "2023-02-01", "2024-12-07")
+    group.add_task("Mobile App Development", "2024-02-01", "2025-12-07")
 
     roadmap.set_footer("Updated on " + datetime.now().strftime("%Y-%m-%d"))
     roadmap.draw()
 
     roadmap.save(file_name)
 
 
 def colour_theme_demo_without_locale(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-12-01",
+    start_date: str = "2023-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
-    file_name: str = "demo01.svg",
+    file_name: str = "demo01.png",
     colour_theme: str = "DEFAULT",
 ) -> None:
     roadmap = Roadmap(
-        1200,
-        1000,
-        auto_height=True,
-        colour_theme=colour_theme,
-        show_marker=True,
-        painter_type="svg",
+        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
     )
-    roadmap.set_title("SAMPLE ROADMAP 2022/2023")
+    roadmap.set_title("SAMPLE ROADMAP 2023/2024")
     roadmap.set_subtitle("ABC Corporation")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
     )
 
     group = roadmap.add_group("Core Product Work Stream", text_alignment="left")
-    task = group.add_task("Base Functionality", "2022-11-01", "2023-10-31")
-    task.add_milestone("v.1.0", "2023-02-15")
-    task.add_milestone("v.1.1", "2023-08-01")
-    parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
-    parellel_task.add_milestone("v.2.0", "2024-03-30")
+    task = group.add_task("Base Functionality", "2023-11-01", "2024-10-31")
+    task.add_milestone("v.1.0", "2024-02-15")
+    task.add_milestone("v.1.1", "2024-08-01")
+    parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2025-03-31")
+    parellel_task.add_milestone("v.2.0", "2025-03-30")
 
-    task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-    task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+    task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+    task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
     group = roadmap.add_group("Mobility Work Stream", text_alignment="left")
-    group.add_task("Mobile App Development", "2023-02-01", "2024-12-07")
+    group.add_task("Mobile App Development", "2024-02-01", "2025-12-07")
 
     roadmap.set_footer("Updated on " + datetime.now().strftime("%Y-%m-%d"))
     roadmap.draw()
 
     roadmap.save(file_name)
 
 
 def chinese_theme_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-12-01",
+    start_date: str = "2023-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
     show_first_day_of_week=False,
-    file_name: str = "demo01.svg",
+    file_name: str = "demo01.png",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200,
-        1000,
-        auto_height=True,
-        colour_theme=colour_theme,
-        show_marker=True,
-        painter_type="svg",
+        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
     )
-    roadmap.set_title("示例路線圖 2022/2023")
+    roadmap.set_title("示例路線圖 2023/2024")
     roadmap.set_subtitle("甲乙丙有限公司")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
         timeline_locale=locale_name,
         show_first_day_of_week=show_first_day_of_week,
     )
 
     group = roadmap.add_group("核心產品工作流程", text_alignment="left")
-    task = group.add_task("基本功能", "2022-11-01", "2023-10-31")
-    task.add_milestone("版本 1.0", "2023-02-15")
-    task.add_milestone("版本 1.1", "2023-08-01")
-    parellel_task = task.add_parallel_task("增強功能", "2023-11-15", "2024-03-31")
-    parellel_task.add_milestone("版本 2.0", "2024-01-30")
+    task = group.add_task("基本功能", "2023-11-01", "2024-10-31")
+    task.add_milestone("版本 1.0", "2024-02-15")
+    task.add_milestone("版本 1.1", "2024-08-01")
+    parellel_task = task.add_parallel_task("增強功能", "2024-11-15", "2025-03-31")
+    parellel_task.add_milestone("版本 2.0", "2025-01-30")
 
-    task = group.add_task("陳列 #1", "2023-03-01", "2023-05-07")
-    task.add_parallel_task("陳列 #2", "2023-06-01", "2023-08-07")
+    task = group.add_task("陳列 #1", "2024-03-01", "2024-05-07")
+    task.add_parallel_task("陳列 #2", "2024-06-01", "2024-08-07")
 
     group = roadmap.add_group("移動工作流程", text_alignment="left")
-    group.add_task("移動應用程序開發", "2023-02-01", "2024-12-07")
+    group.add_task("移動應用程序開發", "2024-02-01", "2024-12-07")
 
     roadmap.set_footer("更新於 " + datetime.now().strftime("%Y-%m-%d"))
     roadmap.draw()
 
     roadmap.save(file_name)
 
 
 def japanese_theme_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-12-01",
+    start_date: str = "2023-12-01",
     number_of_items: int = 12,
     show_generic_dates: bool = False,
     show_first_day_of_week=False,
-    file_name: str = "demo01.svg",
+    file_name: str = "demo01.png",
     colour_theme: str = "DEFAULT",
     locale_name: str = "en_US",
 ) -> None:
     roadmap = Roadmap(
-        1200,
-        1000,
-        auto_height=True,
-        colour_theme=colour_theme,
-        show_marker=True,
-        painter_type="svg",
+        1200, 1000, auto_height=True, colour_theme=colour_theme, show_marker=True
     )
-    roadmap.set_title("ロードマップの例 2022/2023")
+    roadmap.set_title("ロードマップの例 2024/2025")
     roadmap.set_subtitle("株式会社エー・ビー・シー")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
         timeline_locale=locale_name,
         show_first_day_of_week=show_first_day_of_week,
     )
 
     group = roadmap.add_group("コア製品のワークフロー", text_alignment="left")
-    task = group.add_task("基本的なスキル", "2022-11-01", "2023-10-31")
-    task.add_milestone("バージョン 1.0", "2023-02-15")
-    task.add_milestone("バージョン 1.1", "2023-08-01")
-    parellel_task = task.add_parallel_task("強化", "2023-11-15", "2024-03-31")
-    parellel_task.add_milestone("バージョン 2.0", "2024-01-30")
+    task = group.add_task("基本的なスキル", "2023-11-01", "2024-10-31")
+    task.add_milestone("バージョン 1.0", "2024-02-15")
+    task.add_milestone("バージョン 1.1", "2024-08-01")
+    parellel_task = task.add_parallel_task("強化", "2024-11-15", "2025-03-31")
+    parellel_task.add_milestone("バージョン 2.0", "2025-01-30")
 
-    task = group.add_task("ショーケース #1", "2023-03-01", "2023-05-07")
-    task.add_parallel_task("ショーケース #2", "2023-06-01", "2023-08-07")
+    task = group.add_task("ショーケース #1", "2024-03-01", "2024-05-07")
+    task.add_parallel_task("ショーケース #2", "2024-06-01", "2024-08-07")
 
     group = roadmap.add_group("モバイル ワークフロー", text_alignment="left")
-    group.add_task("モバイルアプリ開発", "2023-02-01", "2024-12-07")
+    group.add_task("モバイルアプリ開発", "2024-02-01", "2025-12-07")
 
     roadmap.set_footer("更新日 " + datetime.now().strftime("%Y-%m-%d"))
     roadmap.draw()
 
     roadmap.save(file_name)
 
 
 def generic_date_test(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-11-01",
+    start_date: str = "2023-11-01",
     number_of_items: int = 24,
     show_generic_dates: bool = False,
     show_first_day_of_week: bool = False,
-    file_name: str = "demo01.svg",
+    file_name: str = "demo01.png",
     colour_theme: str = "DEFAULT",
 ) -> None:
-    roadmap = Roadmap(
-        4400, 2000, colour_theme=colour_theme, show_marker=True, painter_type="svg"
-    )
+    roadmap = Roadmap(4400, 2000, colour_theme=colour_theme, show_marker=True)
     roadmap.set_title("My Demo Roadmap!!!")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=show_generic_dates,
         show_first_day_of_week=show_first_day_of_week,
     )
 
     group = roadmap.add_group("Core Product Work Stream")
-    task = group.add_task("Base Functionality", "2022-11-01", "2023-10-31")
-    task.add_milestone("v.1.0", "2023-02-15")
-    task.add_milestone("v.1.1", "2023-08-01")
-    parellel_task = task.add_parallel_task("Enhancements", "2023-11-15", "2024-03-31")
-    parellel_task.add_milestone("v.2.0", "2024-03-30")
+    task = group.add_task("Base Functionality", "2023-11-01", "2024-10-31")
+    task.add_milestone("v.1.0", "2024-02-15")
+    task.add_milestone("v.1.1", "2024-08-01")
+    parellel_task = task.add_parallel_task("Enhancements", "2024-11-15", "2025-03-31")
+    parellel_task.add_milestone("v.2.0", "2025-03-30")
 
-    task = group.add_task("Showcase #1", "2023-03-01", "2023-05-07")
-    task.add_parallel_task("Showcase #2", "2023-06-01", "2023-08-07")
+    task = group.add_task("Showcase #1", "2024-03-01", "2024-05-07")
+    task.add_parallel_task("Showcase #2", "2024-06-01", "2024-08-07")
 
     group = roadmap.add_group("Mobility Work Stream")
-    group.add_task("Mobile App Development", "2023-02-01", "2024-12-07")
+    group.add_task("Mobile App Development", "2024-02-01", "2025-12-07")
 
     roadmap.set_footer("Generated by Roadmapper")
     roadmap.draw()
     roadmap.save(file_name)
 
 
 def parallel_task_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2022-12-01",
+    start_date: str = "2023-12-01",
     number_of_items: int = 14,
-    file_name: str = "demo01.svg",
+    file_name: str = "demo01.png",
     colour_theme: str = "DEFAULT",
 ) -> None:
     roadmap = Roadmap(
         1200,
         612,
         auto_height=False,
         colour_theme=colour_theme,
         show_marker=True,
-        painter_type="svg",
     )
-    roadmap.set_title("ROADMAP EXAMPLE 2022/2023")
+    roadmap.set_title("ROADMAP EXAMPLE 2023/2024")
     roadmap.set_subtitle("This is a subtitle")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=False,
     )
 
     group = roadmap.add_group("Core Product Work Stream")
 
-    task = group.add_task("Base Functionality", "2022-11-01", "2023-01-31")
-    parellel_task = task.add_parallel_task("Enhancements", "2023-02-15", "2024-03-31")
-    parellel_task.add_milestone("v.2.0", "2023-04-30")
-
-    task = group.add_task("Showcase #1", "2023-01-01", "2023-01-31")
-    parellel_task = task.add_parallel_task("Showcase #2", "2023-02-02", "2023-03-15")
-    parellel_task.add_milestone("v.2.0", "2023-04-15")
+    task = group.add_task("Base Functionality", "2023-11-01", "2024-01-31")
+    parellel_task = task.add_parallel_task("Enhancements", "2024-02-15", "2025-03-31")
+    parellel_task.add_milestone("v.2.0", "2024-04-30")
+
+    task = group.add_task("Showcase #1", "2024-01-01", "2024-01-31")
+    parellel_task = task.add_parallel_task("Showcase #2", "2024-02-02", "2024-03-15")
+    parellel_task.add_milestone("v.2.0", "2024-04-15")
 
     # group = roadmap.add_group("Core Product Work Stream 2")
     # task = group.add_task("Base Functionality", "2022-11-01", "2023-01-31")
 
     roadmap.set_footer("Author: CS Goh " + datetime.now().strftime("%Y-%m-%d"))
     roadmap.draw()
     roadmap.save(file_name)
 
 
 def singleton_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2023-01-01",
+    start_date: str = "2024-01-01",
     number_of_items: int = 2,
-    file_name: str = "demo01.svg",
+    file_name: str = "demo01.png",
     colour_theme: str = "BLUEMOUNTAIN",
 ) -> None:
+
     roadmap = Roadmap(
         600,
         612,
         auto_height=True,
         colour_theme=colour_theme,
         show_marker=False,
-        painter_type="svg",
     )
     roadmap.set_title("ROADMAP EXAMPLE")
     # roadmap.set_subtitle("This is a subtitle")
     roadmap.set_timeline(
         timelinemode,
         start=start_date,
         number_of_items=number_of_items,
         show_generic_dates=False,
     )
 
     group = roadmap.add_group("Showcase Task Styles")
 
-    group.add_task("Rectangle Style", "2023-01-15", "2023-02-15")
-    group.add_task("Rounded Style", "2023-01-15", "2023-02-15", style="rounded")
-    group.add_task(
-        "Arrowhead Style", "2023-01-15", "2023-02-15", style="arrowhead"
-    )
+    group.add_task("Rectangle Style", "2024-01-15", "2024-02-15")
+    group.add_task("Rounded Style", "2024-01-15", "2024-02-15", style="rounded")
+    group.add_task("Arrowhead Style", "2024-01-15", "2024-02-15", style="arrowhead")
 
     # roadmap.set_footer("Author: CS Goh " + datetime.now().strftime("%Y-%m-%d"))
     roadmap.draw()
     roadmap.save(file_name)
 
 
 def logo_demo(
     timelinemode: TimelineMode = TimelineMode.MONTHLY,
-    start_date: str = "2023-01-01",
+    start_date: str = "2025-01-01",
     number_of_items: int = 2,
-    file_name: str = "demo01.svg",
+    file_name: str = "demo01.png",
     colour_theme: str = "BLUEMOUNTAIN",
     auto_height: bool = True,
     logo_position: str = "top-left",
 ) -> None:
     file_name = "T_" + file_name
     roadmap = Roadmap(
         800,
         612,
         auto_height=auto_height,
         colour_theme=colour_theme,
         show_marker=False,
-        painter_type="svg",
     )
     frameinfo = inspect.getframeinfo(inspect.currentframe())
     title = f"{frameinfo.function}(), theme={colour_theme}, mode={timelinemode}"
 
     roadmap.add_logo("../../images/logo/matariki-tech-logo.png", logo_position, 50, 50)
     roadmap.set_title(title)
     roadmap.set_subtitle("This is a subtitle")
@@ -341,70 +315,70 @@
         show_generic_dates=False,
     )
 
     group = roadmap.add_group("Showcase Task Styles")
 
     text = "I love Python"
     # emojized_text = emojize(text)
-    group.add_task(text, "2023-01-15", "2023-02-15")
+    group.add_task(text, "2024-01-15", "2024-02-15")
 
     roadmap.set_footer("Author: CS Goh " + datetime.now().strftime("%Y-%m-%d"))
     roadmap.draw()
     roadmap.save(file_name)
 
 
 def test_dev():
     if not os.path.exists("images"):
         os.mkdir("images")
 
     if not os.path.exists("../../images/test"):
         os.mkdir("../../images/test")
 
-    output_file = "../../images/test/colour_theme_demo_without_locale.svg"
+    output_file = "../../images/test/colour_theme_demo_without_locale.png"
     # if file exist, then delete it first
     if os.path.exists(output_file):
         os.remove(output_file)
 
     colour_theme_demo_without_locale(
         file_name=output_file,
         timelinemode=TimelineMode.MONTHLY,
         number_of_items=14,
     )
 
     assert os.path.exists(output_file)
 
-    output_file = "../../images/test/demo-my-colour-chinese.svg"
+    output_file = "../../images/test/demo-my-colour-chinese.png"
     chinese_theme_demo(
         file_name=output_file,
         colour_theme="../json/chinese.json",
         timelinemode=TimelineMode.WEEKLY,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
         number_of_items=14,
         locale_name="../json/zh_TW_timeline_settings.json",
         show_generic_dates=False,
         show_first_day_of_week=True,
     )
     assert os.path.exists(output_file)
 
-    output_file = "../../images/test/demo-my-colour-japanese.svg"
+    output_file = "../../images/test/demo-my-colour-japanese.png"
     japanese_theme_demo(
         file_name=output_file,
         colour_theme="../json/chinese.json",
         timelinemode=TimelineMode.MONTHLY,
-        start_date="2023-01-01",
+        start_date="2024-01-01",
         number_of_items=14,
         locale_name="../json/ja_JP_timeline_settings.json",
         show_generic_dates=False,
         show_first_day_of_week=True,
     )
 
     assert os.path.exists(output_file)
 
 
-# check if calling from main
-if __name__ == "__main__":
-    output_file = "../../images/test/colour_theme_demo_without_locale.svg"
-    colour_theme_demo_without_locale(
-        file_name=output_file,
-        timelinemode=TimelineMode.MONTHLY,
-        number_of_items=14,
-    )
+# # check if calling from main
+# if __name__ == "__main__":
+#     output_file = "../../images/test/colour_theme_demo_without_locale.png"
+#     colour_theme_demo_without_locale(
+#         file_name=output_file,
+#         timelinemode=TimelineMode.MONTHLY,
+#         number_of_items=14,
+#     )
```

