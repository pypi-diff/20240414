# Comparing `tmp/librecell-lib-0.0.8.tar.gz` & `tmp/librecell-lib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/librecell-lib-0.0.8.tar", last modified: Wed Dec 30 17:35:43 2020, max compression
+gzip compressed data, was "dist/librecell-lib-0.0.9.tar", last modified: Wed Dec 30 17:45:39 2020, max compression
```

## Comparing `librecell-lib-0.0.8.tar` & `librecell-lib-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/
--rw-r--r--   0 kramert   (1000) kramert   (1000)     3267 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/PKG-INFO
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2148 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/README.md
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/lclib/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      795 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/__init__.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/lclib/characterization/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      781 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/characterization/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    12110 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/input_capacitance.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    19663 2020-12-30 17:31:13.000000 librecell-lib-0.0.8/lclib/characterization/main_lctime.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     4818 2020-12-30 16:48:52.000000 librecell-lib-0.0.8/lclib/characterization/main_sp2bool.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     5555 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/ngspice_simulation.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    10268 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/ngspice_subprocess.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    13396 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/piece_wise_linear.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     5439 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/test_ngspice_shared.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1361 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/test_ngspice_subprocess.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    14922 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/timing_combinatorial.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    40549 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/timing_sequential.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     8214 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/characterization/util.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/lclib/liberty/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      781 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/liberty/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     5499 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/liberty/merge.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2603 2020-12-30 16:48:52.000000 librecell-lib-0.0.8/lclib/liberty/util.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     4538 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/liberty/visualize.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/lclib/logic/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      781 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/logic/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     7142 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/logic/cmos_sim.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    11218 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/logic/cmos_synth.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    33329 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/logic/functional_abstraction.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     3148 2020-12-30 17:25:54.000000 librecell-lib-0.0.8/lclib/logic/graph_enumeration.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1734 2020-12-30 16:48:52.000000 librecell-lib-0.0.8/lclib/logic/smt_4value_logic_scratch.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     3286 2020-12-30 16:48:52.000000 librecell-lib-0.0.8/lclib/logic/util.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/lclib/transistor_sizing/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      781 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/transistor_sizing/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     9392 2020-07-09 17:09:02.000000 librecell-lib-0.0.8/lclib/transistor_sizing/width_opt.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/librecell_lib.egg-info/
--rw-r--r--   0 kramert   (1000) kramert   (1000)     3267 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/librecell_lib.egg-info/PKG-INFO
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1180 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/librecell_lib.egg-info/SOURCES.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/librecell_lib.egg-info/dependency_links.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)      261 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/librecell_lib.egg-info/entry_points.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2019-10-11 19:52:27.000000 librecell-lib-0.0.8/librecell_lib.egg-info/not-zip-safe
--rw-r--r--   0 kramert   (1000) kramert   (1000)      141 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/librecell_lib.egg-info/requires.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        6 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/librecell_lib.egg-info/top_level.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-12-30 17:35:43.000000 librecell-lib-0.0.8/setup.cfg
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2501 2020-12-30 17:33:09.000000 librecell-lib-0.0.8/setup.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     3267 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2148 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/README.md
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/lclib/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      795 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/__init__.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/lclib/characterization/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      781 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/characterization/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    12110 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/input_capacitance.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    19663 2020-12-30 17:31:13.000000 librecell-lib-0.0.9/lclib/characterization/main_lctime.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     4818 2020-12-30 16:48:52.000000 librecell-lib-0.0.9/lclib/characterization/main_sp2bool.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     5555 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/ngspice_simulation.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    10268 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/ngspice_subprocess.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    13396 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/piece_wise_linear.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     5439 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/test_ngspice_shared.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1361 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/test_ngspice_subprocess.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    14922 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/timing_combinatorial.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    40549 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/timing_sequential.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     8214 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/characterization/util.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/lclib/liberty/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      781 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/liberty/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     5499 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/liberty/merge.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2603 2020-12-30 16:48:52.000000 librecell-lib-0.0.9/lclib/liberty/util.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     4538 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/liberty/visualize.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/lclib/logic/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      781 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/logic/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     7142 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/logic/cmos_sim.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    11218 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/logic/cmos_synth.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    33329 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/logic/functional_abstraction.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     3148 2020-12-30 17:25:54.000000 librecell-lib-0.0.9/lclib/logic/graph_enumeration.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1734 2020-12-30 16:48:52.000000 librecell-lib-0.0.9/lclib/logic/smt_4value_logic_scratch.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     3286 2020-12-30 16:48:52.000000 librecell-lib-0.0.9/lclib/logic/util.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/lclib/transistor_sizing/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      781 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/transistor_sizing/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     9392 2020-07-09 17:09:02.000000 librecell-lib-0.0.9/lclib/transistor_sizing/width_opt.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/librecell_lib.egg-info/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     3267 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/librecell_lib.egg-info/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1180 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/librecell_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/librecell_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      261 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/librecell_lib.egg-info/entry_points.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2019-10-11 19:52:27.000000 librecell-lib-0.0.9/librecell_lib.egg-info/not-zip-safe
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      141 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/librecell_lib.egg-info/requires.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        6 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/librecell_lib.egg-info/top_level.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-12-30 17:45:39.000000 librecell-lib-0.0.9/setup.cfg
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2501 2020-12-30 17:43:59.000000 librecell-lib-0.0.9/setup.py
```

### Comparing `librecell-lib-0.0.8/PKG-INFO` & `librecell-lib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librecell-lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: CMOS standard cell characterization kit.
 Home-page: https://codeberg.org/tok/librecell
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: AGPL
 Description: # LibreCell - Lib
         Characterization kit for CMOS cells.
```

### Comparing `librecell-lib-0.0.8/README.md` & `librecell-lib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/__init__.py` & `librecell-lib-0.0.9/lclib/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/__init__.py` & `librecell-lib-0.0.9/lclib/characterization/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/input_capacitance.py` & `librecell-lib-0.0.9/lclib/characterization/input_capacitance.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/main_lctime.py` & `librecell-lib-0.0.9/lclib/characterization/main_lctime.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/main_sp2bool.py` & `librecell-lib-0.0.9/lclib/characterization/main_sp2bool.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/ngspice_simulation.py` & `librecell-lib-0.0.9/lclib/characterization/ngspice_simulation.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/ngspice_subprocess.py` & `librecell-lib-0.0.9/lclib/characterization/ngspice_subprocess.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/piece_wise_linear.py` & `librecell-lib-0.0.9/lclib/characterization/piece_wise_linear.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/test_ngspice_shared.py` & `librecell-lib-0.0.9/lclib/characterization/test_ngspice_shared.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/test_ngspice_subprocess.py` & `librecell-lib-0.0.9/lclib/characterization/test_ngspice_subprocess.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/timing_combinatorial.py` & `librecell-lib-0.0.9/lclib/characterization/timing_combinatorial.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/timing_sequential.py` & `librecell-lib-0.0.9/lclib/characterization/timing_sequential.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/characterization/util.py` & `librecell-lib-0.0.9/lclib/characterization/util.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/liberty/__init__.py` & `librecell-lib-0.0.9/lclib/liberty/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/liberty/merge.py` & `librecell-lib-0.0.9/lclib/liberty/merge.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/liberty/util.py` & `librecell-lib-0.0.9/lclib/liberty/util.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/liberty/visualize.py` & `librecell-lib-0.0.9/lclib/liberty/visualize.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/logic/__init__.py` & `librecell-lib-0.0.9/lclib/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/logic/cmos_sim.py` & `librecell-lib-0.0.9/lclib/logic/cmos_sim.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/logic/cmos_synth.py` & `librecell-lib-0.0.9/lclib/logic/cmos_synth.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/logic/functional_abstraction.py` & `librecell-lib-0.0.9/lclib/logic/functional_abstraction.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/logic/graph_enumeration.py` & `librecell-lib-0.0.9/lclib/logic/graph_enumeration.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/logic/smt_4value_logic_scratch.py` & `librecell-lib-0.0.9/lclib/logic/smt_4value_logic_scratch.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/logic/util.py` & `librecell-lib-0.0.9/lclib/logic/util.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/transistor_sizing/__init__.py` & `librecell-lib-0.0.9/lclib/transistor_sizing/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/lclib/transistor_sizing/width_opt.py` & `librecell-lib-0.0.9/lclib/transistor_sizing/width_opt.py`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/librecell_lib.egg-info/PKG-INFO` & `librecell-lib-0.0.9/librecell_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librecell-lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: CMOS standard cell characterization kit.
 Home-page: https://codeberg.org/tok/librecell
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: AGPL
 Description: # LibreCell - Lib
         Characterization kit for CMOS cells.
```

### Comparing `librecell-lib-0.0.8/librecell_lib.egg-info/SOURCES.txt` & `librecell-lib-0.0.9/librecell_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librecell-lib-0.0.8/setup.py` & `librecell-lib-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(name='librecell-lib',
-      version='0.0.8',
+      version='0.0.9',
       description='CMOS standard cell characterization kit.',
       long_description=readme(),
       long_description_content_type="text/markdown",
       keywords='cmos cell characterization vlsi asic',
       classifiers=[
           'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
           'Development Status :: 3 - Alpha',
@@ -50,15 +50,15 @@
               'libertymerge = lclib.liberty.merge:main',
               'lcsize = lclib.transistor_sizing.width_opt:main',
               'lctime = lclib.characterization.main_lctime:main',
               'sp2bool = lclib.characterization.main_sp2bool:main'
           ]
       },
       install_requires=[
-          'librecell-common==0.0.7',
+          'librecell-common>=0.0.9',
           'numpy==1.*',  # BSD
           'sympy==1.6.*',  # BSD
           'matplotlib==3.*',
           'networkx==2.5',  # BSD
           'pyspice==1.4.3',  # GPLv3
           'scipy>=1.5.*',  # BSD
           'liberty-parser==0.0.8',  # GPLv3
```

