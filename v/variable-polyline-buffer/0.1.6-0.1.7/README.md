# Comparing `tmp/variable_polyline_buffer-0.1.6.tar.gz` & `tmp/variable_polyline_buffer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_polyline_buffer-0.1.6.tar", last modified: Fri Apr 12 15:07:37 2024, max compression
+gzip compressed data, was "variable_polyline_buffer-0.1.7.tar", last modified: Sun Apr 14 16:18:18 2024, max compression
```

## Comparing `variable_polyline_buffer-0.1.6.tar` & `variable_polyline_buffer-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:07:37.676891 variable_polyline_buffer-0.1.6/
--rw-r--r--   0 stephan    (501) staff       (20)     1069 2024-04-12 14:13:03.000000 variable_polyline_buffer-0.1.6/LICENSE
--rw-r--r--   0 stephan    (501) staff       (20)     2479 2024-04-12 15:07:37.676668 variable_polyline_buffer-0.1.6/PKG-INFO
--rw-r--r--   0 stephan    (501) staff       (20)     2084 2024-04-12 15:07:20.000000 variable_polyline_buffer-0.1.6/README.md
--rw-r--r--   0 stephan    (501) staff       (20)       38 2024-04-12 15:07:37.676939 variable_polyline_buffer-0.1.6/setup.cfg
--rw-r--r--   0 stephan    (501) staff       (20)      592 2024-04-12 15:05:55.000000 variable_polyline_buffer-0.1.6/setup.py
-drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:07:37.675162 variable_polyline_buffer-0.1.6/src/
-drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:07:37.675790 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer/
--rw-r--r--   0 stephan    (501) staff       (20)       54 2024-04-12 15:03:48.000000 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer/__init__.py
--rw-r--r--   0 stephan    (501) staff       (20)     3935 2024-04-12 13:52:24.000000 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer/polyline_buffer.py
-drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:07:37.676511 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer.egg-info/
--rw-r--r--   0 stephan    (501) staff       (20)     2479 2024-04-12 15:07:37.000000 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer.egg-info/PKG-INFO
--rw-r--r--   0 stephan    (501) staff       (20)      374 2024-04-12 15:07:37.000000 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer.egg-info/SOURCES.txt
--rw-r--r--   0 stephan    (501) staff       (20)        1 2024-04-12 15:07:37.000000 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer.egg-info/dependency_links.txt
--rw-r--r--   0 stephan    (501) staff       (20)        6 2024-04-12 15:07:37.000000 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer.egg-info/requires.txt
--rw-r--r--   0 stephan    (501) staff       (20)       25 2024-04-12 15:07:37.000000 variable_polyline_buffer-0.1.6/src/variable_polyline_buffer.egg-info/top_level.txt
+drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-14 16:18:18.412526 variable_polyline_buffer-0.1.7/
+-rw-r--r--   0 stephan    (501) staff       (20)     1069 2024-04-12 14:13:03.000000 variable_polyline_buffer-0.1.7/LICENSE
+-rw-r--r--   0 stephan    (501) staff       (20)     2479 2024-04-14 16:18:18.412243 variable_polyline_buffer-0.1.7/PKG-INFO
+-rw-r--r--   0 stephan    (501) staff       (20)     2084 2024-04-12 15:07:20.000000 variable_polyline_buffer-0.1.7/README.md
+-rw-r--r--   0 stephan    (501) staff       (20)       38 2024-04-14 16:18:18.412567 variable_polyline_buffer-0.1.7/setup.cfg
+-rw-r--r--   0 stephan    (501) staff       (20)      592 2024-04-14 16:14:34.000000 variable_polyline_buffer-0.1.7/setup.py
+drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-14 16:18:18.410806 variable_polyline_buffer-0.1.7/src/
+drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-14 16:18:18.411369 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer/
+-rw-r--r--   0 stephan    (501) staff       (20)       54 2024-04-12 15:03:48.000000 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer/__init__.py
+-rw-r--r--   0 stephan    (501) staff       (20)     4322 2024-04-14 16:14:26.000000 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer/polyline_buffer.py
+drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-14 16:18:18.412059 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer.egg-info/
+-rw-r--r--   0 stephan    (501) staff       (20)     2479 2024-04-14 16:18:18.000000 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer.egg-info/PKG-INFO
+-rw-r--r--   0 stephan    (501) staff       (20)      374 2024-04-14 16:18:18.000000 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer.egg-info/SOURCES.txt
+-rw-r--r--   0 stephan    (501) staff       (20)        1 2024-04-14 16:18:18.000000 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer.egg-info/dependency_links.txt
+-rw-r--r--   0 stephan    (501) staff       (20)        6 2024-04-14 16:18:18.000000 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer.egg-info/requires.txt
+-rw-r--r--   0 stephan    (501) staff       (20)       25 2024-04-14 16:18:18.000000 variable_polyline_buffer-0.1.7/src/variable_polyline_buffer.egg-info/top_level.txt
```

### Comparing `variable_polyline_buffer-0.1.6/LICENSE` & `variable_polyline_buffer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `variable_polyline_buffer-0.1.6/PKG-INFO` & `variable_polyline_buffer-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable_polyline_buffer
-Version: 0.1.6
+Version: 0.1.7
 Summary: A function for calculating a buffer around a polyline, defining the contours of a line with variable thickness.
 Home-page: https://github.com/stephtr/variable-polyline-buffer
 Author: Stephan Troyer
 Author-email: stephantroyer@live.at
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `variable_polyline_buffer-0.1.6/README.md` & `variable_polyline_buffer-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `variable_polyline_buffer-0.1.6/setup.py` & `variable_polyline_buffer-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="variable_polyline_buffer",
-    version="0.1.6",
+    version="0.1.7",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     description="A function for calculating a buffer around a polyline, defining the contours of a line with variable thickness.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Stephan Troyer",
     author_email="stephantroyer@live.at",
```

### Comparing `variable_polyline_buffer-0.1.6/src/variable_polyline_buffer/polyline_buffer.py` & `variable_polyline_buffer-0.1.7/src/variable_polyline_buffer/polyline_buffer.py`

 * *Files 13% similar despite different names*

```diff
@@ -72,37 +72,45 @@
         if prev_dist[0] is False or prev_dist[1] is False:
             raise ValueError("Taper segments can't be at the end or follow each other")
 
     for path in [left, right]:  # let's cleanup the paths
         i_segment = 1
         i_line = 2
         iteration = 0
+        local_points = points[:]
         while i_segment < len(path) - 2:
             segment = path[i_segment + 1] - path[i_segment]
-            line = points[i_line + 1] - points[i_line]
-            if (
-                segment.dot(line) < 0
-            ):  # if one of the segments is inversed, eliminate it and extend the adjacent ones such that they meet
+            line = local_points[i_line + 1] - local_points[i_line]
+            if segment.dot(line) < 0:
+                # if one of the segments is inversed, eliminate it and extend the adjacent ones such that they meet
                 normal_before = rot_mat @ (path[i_segment] - path[i_segment - 1])
                 normal_after = rot_mat @ (path[i_segment + 2] - path[i_segment + 1])
                 A = np.array([normal_before, normal_after])
+                A_inv = np.linalg.inv(A)
                 b = np.array(
                     [
                         normal_before @ path[i_segment],
                         normal_after @ path[i_segment + 1],
                     ]
                 )
                 path.pop(i_segment + 1)
-                path[i_segment] = np.linalg.inv(A) @ b
-                if (
-                    i_segment > 1
-                ):  # now that we modified the path, we need to check the previous segment again
+                path[i_segment] = A_inv @ b
+                # in addition, we also need to modify the according segment in the original line
+                b = np.array(
+                    [
+                        normal_before @ local_points[i_line],
+                        normal_after @ local_points[i_line + 1],
+                    ]
+                )
+                local_points.pop(i_segment + 1)
+                local_points[i_line] = A_inv @ b
+
+                if i_segment > 1:
+                    # now that we modified the path, we need to check the previous segment again
                     i_segment -= 1
-                else:
-                    i_line += 1
+                    i_line -= 1
                 iteration += 1
-                # if iteration > 1: break
             else:
                 i_segment += 1
                 i_line += 1
 
     return left, right
```

### Comparing `variable_polyline_buffer-0.1.6/src/variable_polyline_buffer.egg-info/PKG-INFO` & `variable_polyline_buffer-0.1.7/src/variable_polyline_buffer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variable-polyline-buffer
-Version: 0.1.6
+Version: 0.1.7
 Summary: A function for calculating a buffer around a polyline, defining the contours of a line with variable thickness.
 Home-page: https://github.com/stephtr/variable-polyline-buffer
 Author: Stephan Troyer
 Author-email: stephantroyer@live.at
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

