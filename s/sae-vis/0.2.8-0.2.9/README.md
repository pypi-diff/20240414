# Comparing `tmp/sae-vis-0.2.8.tar.gz` & `tmp/sae-vis-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae-vis-0.2.8.tar", last modified: Sat Apr  6 16:00:54 2024, max compression
+gzip compressed data, was "sae-vis-0.2.9.tar", last modified: Sat Apr  6 16:10:14 2024, max compression
```

## Comparing `sae-vis-0.2.8.tar` & `sae-vis-0.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:00:54.057817 sae-vis-0.2.8/
--rw-rw-rw-   0        0        0     1092 2024-04-06 14:20:39.000000 sae-vis-0.2.8/LICENSE
--rw-rw-rw-   0        0        0       27 2024-02-21 04:51:02.000000 sae-vis-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1305 2024-04-06 16:00:54.056816 sae-vis-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     2636 2024-03-29 09:56:38.000000 sae-vis-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 16:00:53.994294 sae-vis-0.2.8/sae_vis/
--rw-rw-rw-   0        0        0      165 2024-02-21 04:27:15.000000 sae-vis-0.2.8/sae_vis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:00:54.038301 sae-vis-0.2.8/sae_vis/__pycache__/
--rw-rw-rw-   0        0        0      373 2024-02-21 16:51:55.000000 sae-vis-0.2.8/sae_vis/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    24181 2024-04-06 15:28:15.000000 sae-vis-0.2.8/sae_vis/__pycache__/data_config_classes.cpython-311.pyc
--rw-rw-rw-   0        0        0    50492 2024-04-06 15:40:47.000000 sae-vis-0.2.8/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    58256 2024-04-06 15:40:47.000000 sae-vis-0.2.8/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    13155 2024-04-06 15:09:38.000000 sae-vis-0.2.8/sae_vis/__pycache__/html_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    13416 2024-04-06 15:09:38.000000 sae-vis-0.2.8/sae_vis/__pycache__/model_fns.cpython-311.pyc
--rw-rw-rw-   0        0        0    47426 2024-04-06 15:40:47.000000 sae-vis-0.2.8/sae_vis/__pycache__/utils_fns.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-06 16:00:54.042818 sae-vis-0.2.8/sae_vis/css/
--rw-rw-rw-   0        0        0      796 2024-03-24 10:41:36.000000 sae-vis-0.2.8/sae_vis/css/dropdown.css
--rw-rw-rw-   0        0        0     1289 2024-03-17 20:10:53.000000 sae-vis-0.2.8/sae_vis/css/general.css
--rw-rw-rw-   0        0        0     1464 2024-03-17 15:54:46.000000 sae-vis-0.2.8/sae_vis/css/sequences.css
--rw-rw-rw-   0        0        0     1671 2024-03-17 18:07:59.000000 sae-vis-0.2.8/sae_vis/css/tables.css
--rw-rw-rw-   0        0        0    18023 2024-04-06 15:22:47.000000 sae-vis-0.2.8/sae_vis/data_config_classes.py
--rw-rw-rw-   0        0        0    49956 2024-04-06 15:36:52.000000 sae-vis-0.2.8/sae_vis/data_fetching_fns.py
--rw-rw-rw-   0        0        0    49922 2024-04-06 15:35:49.000000 sae-vis-0.2.8/sae_vis/data_storing_fns.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:00:54.048814 sae-vis-0.2.8/sae_vis/html/
--rw-rw-rw-   0        0        0      137 2024-03-17 17:41:09.000000 sae-vis-0.2.8/sae_vis/html/acts_histogram_template.html
--rw-rw-rw-   0        0        0       87 2024-03-17 17:41:07.000000 sae-vis-0.2.8/sae_vis/html/feature_tables_template.html
--rw-rw-rw-   0        0        0      125 2024-03-17 17:40:27.000000 sae-vis-0.2.8/sae_vis/html/logits_histogram_template.html
--rw-rw-rw-   0        0        0       78 2024-03-17 17:40:08.000000 sae-vis-0.2.8/sae_vis/html/logits_table_template.html
--rw-rw-rw-   0        0        0       79 2024-03-17 17:43:18.000000 sae-vis-0.2.8/sae_vis/html/sequences_group_template.html
--rw-rw-rw-   0        0        0    13674 2024-04-01 09:31:33.000000 sae-vis-0.2.8/sae_vis/html_fns.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:00:54.055813 sae-vis-0.2.8/sae_vis/js/
--rw-rw-rw-   0        0        0     4378 2024-03-24 10:12:02.000000 sae-vis-0.2.8/sae_vis/js/_createDropdownsScript.js
--rw-rw-rw-   0        0        0     3077 2024-03-24 09:43:39.000000 sae-vis-0.2.8/sae_vis/js/actsHistogramScript.js
--rw-rw-rw-   0        0        0     3083 2024-04-06 15:06:27.000000 sae-vis-0.2.8/sae_vis/js/featureTablesScript.js
--rw-rw-rw-   0        0        0      533 2024-03-17 19:15:57.000000 sae-vis-0.2.8/sae_vis/js/gridColumnTitlesScript.js
--rw-rw-rw-   0        0        0     3512 2024-03-24 09:43:08.000000 sae-vis-0.2.8/sae_vis/js/logitsHistogramScript.js
--rw-rw-rw-   0        0        0     2769 2024-03-17 16:48:34.000000 sae-vis-0.2.8/sae_vis/js/logitsTableScript.js
--rw-rw-rw-   0        0        0    10991 2024-03-24 09:55:09.000000 sae-vis-0.2.8/sae_vis/js/tokenScript.js
--rw-rw-rw-   0        0        0     8967 2024-04-01 10:10:41.000000 sae-vis-0.2.8/sae_vis/model_fns.py
--rw-rw-rw-   0        0        0    36140 2024-04-06 15:40:24.000000 sae-vis-0.2.8/sae_vis/utils_fns.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:00:54.026296 sae-vis-0.2.8/sae_vis.egg-info/
--rw-rw-rw-   0        0        0     1305 2024-04-06 16:00:53.000000 sae-vis-0.2.8/sae_vis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1252 2024-04-06 16:00:53.000000 sae-vis-0.2.8/sae_vis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:00:53.000000 sae-vis-0.2.8/sae_vis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-06 16:00:53.000000 sae-vis-0.2.8/sae_vis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-06 16:00:53.000000 sae-vis-0.2.8/sae_vis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 16:00:54.057817 sae-vis-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1648 2024-04-06 15:13:21.000000 sae-vis-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:10:14.708652 sae-vis-0.2.9/
+-rw-rw-rw-   0        0        0     1092 2024-04-06 14:20:39.000000 sae-vis-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-02-21 04:51:02.000000 sae-vis-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1305 2024-04-06 16:10:14.707654 sae-vis-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2636 2024-03-29 09:56:38.000000 sae-vis-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 16:10:14.660131 sae-vis-0.2.9/sae_vis/
+-rw-rw-rw-   0        0        0      165 2024-02-21 04:27:15.000000 sae-vis-0.2.9/sae_vis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:10:14.685654 sae-vis-0.2.9/sae_vis/__pycache__/
+-rw-rw-rw-   0        0        0      373 2024-02-21 16:51:55.000000 sae-vis-0.2.9/sae_vis/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    24181 2024-04-06 15:28:15.000000 sae-vis-0.2.9/sae_vis/__pycache__/data_config_classes.cpython-311.pyc
+-rw-rw-rw-   0        0        0    50492 2024-04-06 15:40:47.000000 sae-vis-0.2.9/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    58256 2024-04-06 15:40:47.000000 sae-vis-0.2.9/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13155 2024-04-06 15:09:38.000000 sae-vis-0.2.9/sae_vis/__pycache__/html_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13416 2024-04-06 15:09:38.000000 sae-vis-0.2.9/sae_vis/__pycache__/model_fns.cpython-311.pyc
+-rw-rw-rw-   0        0        0    47426 2024-04-06 15:40:47.000000 sae-vis-0.2.9/sae_vis/__pycache__/utils_fns.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-06 16:10:14.691654 sae-vis-0.2.9/sae_vis/css/
+-rw-rw-rw-   0        0        0      796 2024-03-24 10:41:36.000000 sae-vis-0.2.9/sae_vis/css/dropdown.css
+-rw-rw-rw-   0        0        0     1289 2024-03-17 20:10:53.000000 sae-vis-0.2.9/sae_vis/css/general.css
+-rw-rw-rw-   0        0        0     1464 2024-03-17 15:54:46.000000 sae-vis-0.2.9/sae_vis/css/sequences.css
+-rw-rw-rw-   0        0        0     1671 2024-03-17 18:07:59.000000 sae-vis-0.2.9/sae_vis/css/tables.css
+-rw-rw-rw-   0        0        0    18023 2024-04-06 15:22:47.000000 sae-vis-0.2.9/sae_vis/data_config_classes.py
+-rw-rw-rw-   0        0        0    49956 2024-04-06 15:36:52.000000 sae-vis-0.2.9/sae_vis/data_fetching_fns.py
+-rw-rw-rw-   0        0        0    49922 2024-04-06 15:35:49.000000 sae-vis-0.2.9/sae_vis/data_storing_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:10:14.698653 sae-vis-0.2.9/sae_vis/html/
+-rw-rw-rw-   0        0        0      138 2024-04-06 16:06:17.000000 sae-vis-0.2.9/sae_vis/html/acts_histogram_template.html
+-rw-rw-rw-   0        0        0       87 2024-03-17 17:41:07.000000 sae-vis-0.2.9/sae_vis/html/feature_tables_template.html
+-rw-rw-rw-   0        0        0      125 2024-03-17 17:40:27.000000 sae-vis-0.2.9/sae_vis/html/logits_histogram_template.html
+-rw-rw-rw-   0        0        0       78 2024-03-17 17:40:08.000000 sae-vis-0.2.9/sae_vis/html/logits_table_template.html
+-rw-rw-rw-   0        0        0       79 2024-03-17 17:43:18.000000 sae-vis-0.2.9/sae_vis/html/sequences_group_template.html
+-rw-rw-rw-   0        0        0    13674 2024-04-01 09:31:33.000000 sae-vis-0.2.9/sae_vis/html_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:10:14.706652 sae-vis-0.2.9/sae_vis/js/
+-rw-rw-rw-   0        0        0     4378 2024-03-24 10:12:02.000000 sae-vis-0.2.9/sae_vis/js/_createDropdownsScript.js
+-rw-rw-rw-   0        0        0     3077 2024-03-24 09:43:39.000000 sae-vis-0.2.9/sae_vis/js/actsHistogramScript.js
+-rw-rw-rw-   0        0        0     3083 2024-04-06 15:06:27.000000 sae-vis-0.2.9/sae_vis/js/featureTablesScript.js
+-rw-rw-rw-   0        0        0      533 2024-03-17 19:15:57.000000 sae-vis-0.2.9/sae_vis/js/gridColumnTitlesScript.js
+-rw-rw-rw-   0        0        0     3512 2024-03-24 09:43:08.000000 sae-vis-0.2.9/sae_vis/js/logitsHistogramScript.js
+-rw-rw-rw-   0        0        0     2769 2024-03-17 16:48:34.000000 sae-vis-0.2.9/sae_vis/js/logitsTableScript.js
+-rw-rw-rw-   0        0        0    10991 2024-03-24 09:55:09.000000 sae-vis-0.2.9/sae_vis/js/tokenScript.js
+-rw-rw-rw-   0        0        0     8967 2024-04-01 10:10:41.000000 sae-vis-0.2.9/sae_vis/model_fns.py
+-rw-rw-rw-   0        0        0    36140 2024-04-06 15:40:24.000000 sae-vis-0.2.9/sae_vis/utils_fns.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:10:14.673137 sae-vis-0.2.9/sae_vis.egg-info/
+-rw-rw-rw-   0        0        0     1305 2024-04-06 16:10:14.000000 sae-vis-0.2.9/sae_vis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1252 2024-04-06 16:10:14.000000 sae-vis-0.2.9/sae_vis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 16:10:14.000000 sae-vis-0.2.9/sae_vis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-06 16:10:14.000000 sae-vis-0.2.9/sae_vis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 16:10:14.000000 sae-vis-0.2.9/sae_vis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 16:10:14.708652 sae-vis-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1648 2024-04-06 16:03:55.000000 sae-vis-0.2.9/setup.py
```

### Comparing `sae-vis-0.2.8/LICENSE` & `sae-vis-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/PKG-INFO` & `sae-vis-0.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-vis
-Version: 0.2.8
+Version: 0.2.9
 Summary: Open-source SAE visualizer, based on Anthropic's published visualizer.
 Home-page: https://github.com/callummcdougall/sae_vis
 Author: Callum McDougall
 Author-email: cal.s.mcdougall@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `sae-vis-0.2.8/README.md` & `sae-vis-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/__pycache__/data_config_classes.cpython-311.pyc` & `sae-vis-0.2.9/sae_vis/__pycache__/data_config_classes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc` & `sae-vis-0.2.9/sae_vis/__pycache__/data_fetching_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc` & `sae-vis-0.2.9/sae_vis/__pycache__/data_storing_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/__pycache__/html_fns.cpython-311.pyc` & `sae-vis-0.2.9/sae_vis/__pycache__/html_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/__pycache__/model_fns.cpython-311.pyc` & `sae-vis-0.2.9/sae_vis/__pycache__/model_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/__pycache__/utils_fns.cpython-311.pyc` & `sae-vis-0.2.9/sae_vis/__pycache__/utils_fns.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/css/dropdown.css` & `sae-vis-0.2.9/sae_vis/css/dropdown.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/css/general.css` & `sae-vis-0.2.9/sae_vis/css/general.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/css/sequences.css` & `sae-vis-0.2.9/sae_vis/css/sequences.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/css/tables.css` & `sae-vis-0.2.9/sae_vis/css/tables.css`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/data_config_classes.py` & `sae-vis-0.2.9/sae_vis/data_config_classes.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/data_fetching_fns.py` & `sae-vis-0.2.9/sae_vis/data_fetching_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/data_storing_fns.py` & `sae-vis-0.2.9/sae_vis/data_storing_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/html_fns.py` & `sae-vis-0.2.9/sae_vis/html_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/js/_createDropdownsScript.js` & `sae-vis-0.2.9/sae_vis/js/_createDropdownsScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/js/actsHistogramScript.js` & `sae-vis-0.2.9/sae_vis/js/actsHistogramScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/js/featureTablesScript.js` & `sae-vis-0.2.9/sae_vis/js/featureTablesScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/js/gridColumnTitlesScript.js` & `sae-vis-0.2.9/sae_vis/js/gridColumnTitlesScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/js/logitsHistogramScript.js` & `sae-vis-0.2.9/sae_vis/js/logitsHistogramScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/js/logitsTableScript.js` & `sae-vis-0.2.9/sae_vis/js/logitsTableScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/js/tokenScript.js` & `sae-vis-0.2.9/sae_vis/js/tokenScript.js`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/model_fns.py` & `sae-vis-0.2.9/sae_vis/model_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis/utils_fns.py` & `sae-vis-0.2.9/sae_vis/utils_fns.py`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/sae_vis.egg-info/PKG-INFO` & `sae-vis-0.2.9/sae_vis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-vis
-Version: 0.2.8
+Version: 0.2.9
 Summary: Open-source SAE visualizer, based on Anthropic's published visualizer.
 Home-page: https://github.com/callummcdougall/sae_vis
 Author: Callum McDougall
 Author-email: cal.s.mcdougall@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `sae-vis-0.2.8/sae_vis.egg-info/SOURCES.txt` & `sae-vis-0.2.9/sae_vis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sae-vis-0.2.8/setup.py` & `sae-vis-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sae-vis',
-    version = '0.2.8',
+    version = '0.2.9',
     packages = find_packages(),
     install_requires = [
         'torch',
         'einops',
         'datasets',
         'dataclasses-json',
         'jaxtyping',
```

