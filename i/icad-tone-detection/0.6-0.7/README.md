# Comparing `tmp/icad_tone_detection-0.6.tar.gz` & `tmp/icad_tone_detection-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icad_tone_detection-0.6.tar", last modified: Sun Mar 31 19:37:42 2024, max compression
+gzip compressed data, was "icad_tone_detection-0.7.tar", last modified: Sat Apr 13 22:35:34 2024, max compression
```

## Comparing `icad_tone_detection-0.6.tar` & `icad_tone_detection-0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-03-31 19:37:42.722019 icad_tone_detection-0.6/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-03-31 19:37:42.722019 icad_tone_detection-0.6/.github/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-03-31 19:37:42.722019 icad_tone_detection-0.6/.github/workflows/
--rw-rw-r--   0 ian       (2000) ian       (2000)     1301 2024-03-18 00:28:15.000000 icad_tone_detection-0.6/.github/workflows/python-package.yml
--rw-rw-r--   0 ian       (2000) ian       (2000)     3084 2024-03-14 21:16:01.000000 icad_tone_detection-0.6/.gitignore
--rw-rw-r--   0 ian       (2000) ian       (2000)      555 2024-03-17 23:53:26.000000 icad_tone_detection-0.6/LICENSE
--rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-03-31 19:37:42.722019 icad_tone_detection-0.6/PKG-INFO
--rw-rw-r--   0 ian       (2000) ian       (2000)      457 2024-03-18 00:11:11.000000 icad_tone_detection-0.6/README.md
--rw-rw-r--   0 ian       (2000) ian       (2000)      592 2024-03-17 23:50:50.000000 icad_tone_detection-0.6/detect_test.py
--rw-rw-r--   0 ian       (2000) ian       (2000)      779 2024-03-31 19:37:33.000000 icad_tone_detection-0.6/pyproject.toml
--rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-03-31 19:37:42.722019 icad_tone_detection-0.6/setup.cfg
--rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-03-18 00:11:11.000000 icad_tone_detection-0.6/setup.py
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-03-31 19:37:42.722019 icad_tone_detection-0.6/src/
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-03-31 19:37:42.722019 icad_tone_detection-0.6/src/icad_tone_detection/
--rw-rw-r--   0 ian       (2000) ian       (2000)       57 2024-03-14 20:41:31.000000 icad_tone_detection-0.6/src/icad_tone_detection/__init__.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     2599 2024-03-18 01:16:38.000000 icad_tone_detection-0.6/src/icad_tone_detection/audio_loader.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     5855 2024-03-12 18:45:10.000000 icad_tone_detection-0.6/src/icad_tone_detection/frequency_extraction.py
--rw-rw-r--   0 ian       (2000) ian       (2000)     2454 2024-03-16 00:09:53.000000 icad_tone_detection-0.6/src/icad_tone_detection/main.py
--rw-rw-r--   0 ian       (2000) ian       (2000)    11437 2024-03-16 00:05:55.000000 icad_tone_detection-0.6/src/icad_tone_detection/tone_detection.py
-drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-03-31 19:37:42.722019 icad_tone_detection-0.6/src/icad_tone_detection.egg-info/
--rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-03-31 19:37:42.000000 icad_tone_detection-0.6/src/icad_tone_detection.egg-info/PKG-INFO
--rw-rw-r--   0 ian       (2000) ian       (2000)      536 2024-03-31 19:37:42.000000 icad_tone_detection-0.6/src/icad_tone_detection.egg-info/SOURCES.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)        1 2024-03-31 19:37:42.000000 icad_tone_detection-0.6/src/icad_tone_detection.egg-info/dependency_links.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)       59 2024-03-31 19:37:42.000000 icad_tone_detection-0.6/src/icad_tone_detection.egg-info/requires.txt
--rw-rw-r--   0 ian       (2000) ian       (2000)       20 2024-03-31 19:37:42.000000 icad_tone_detection-0.6/src/icad_tone_detection.egg-info/top_level.txt
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/.github/
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/.github/workflows/
+-rw-rw-r--   0 ian       (2000) ian       (2000)     1301 2024-03-18 00:28:15.000000 icad_tone_detection-0.7/.github/workflows/python-package.yml
+-rw-rw-r--   0 ian       (2000) ian       (2000)     3084 2024-03-14 21:16:01.000000 icad_tone_detection-0.7/.gitignore
+-rw-rw-r--   0 ian       (2000) ian       (2000)      555 2024-03-17 23:53:26.000000 icad_tone_detection-0.7/LICENSE
+-rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/PKG-INFO
+-rw-rw-r--   0 ian       (2000) ian       (2000)      457 2024-03-18 00:11:11.000000 icad_tone_detection-0.7/README.md
+-rw-rw-r--   0 ian       (2000) ian       (2000)      592 2024-03-17 23:50:50.000000 icad_tone_detection-0.7/detect_test.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)      779 2024-04-13 22:34:32.000000 icad_tone_detection-0.7/pyproject.toml
+-rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/setup.cfg
+-rw-rw-r--   0 ian       (2000) ian       (2000)       38 2024-03-18 00:11:11.000000 icad_tone_detection-0.7/setup.py
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/src/
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/src/icad_tone_detection/
+-rw-rw-r--   0 ian       (2000) ian       (2000)       57 2024-03-14 20:41:31.000000 icad_tone_detection-0.7/src/icad_tone_detection/__init__.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     2599 2024-03-18 01:16:38.000000 icad_tone_detection-0.7/src/icad_tone_detection/audio_loader.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     5855 2024-03-12 18:45:10.000000 icad_tone_detection-0.7/src/icad_tone_detection/frequency_extraction.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)     2454 2024-03-16 00:09:53.000000 icad_tone_detection-0.7/src/icad_tone_detection/main.py
+-rw-rw-r--   0 ian       (2000) ian       (2000)    11538 2024-04-13 22:34:32.000000 icad_tone_detection-0.7/src/icad_tone_detection/tone_detection.py
+drwxrwxr-x   0 ian       (2000) ian       (2000)        0 2024-04-13 22:35:34.677511 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/
+-rw-r--r--   0 ian       (2000) ian       (2000)     1166 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/PKG-INFO
+-rw-rw-r--   0 ian       (2000) ian       (2000)      536 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/SOURCES.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)        1 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/dependency_links.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)       59 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/requires.txt
+-rw-rw-r--   0 ian       (2000) ian       (2000)       20 2024-04-13 22:35:34.000000 icad_tone_detection-0.7/src/icad_tone_detection.egg-info/top_level.txt
```

### Comparing `icad_tone_detection-0.6/.github/workflows/python-package.yml` & `icad_tone_detection-0.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.6/.gitignore` & `icad_tone_detection-0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.6/LICENSE` & `icad_tone_detection-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.6/PKG-INFO` & `icad_tone_detection-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 0.6
+Version: 0.7
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-0.6/detect_test.py` & `icad_tone_detection-0.7/detect_test.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.6/pyproject.toml` & `icad_tone_detection-0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icad_tone_detection"
-version = "0.6"
+version = "0.7"
 authors = [
   {name = "TheGreatCodeholio", email = "ian@icarey.net"},
 ]
 description = "A Python library for extracting scanner radio tones from scanner audio."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `icad_tone_detection-0.6/src/icad_tone_detection/audio_loader.py` & `icad_tone_detection-0.7/src/icad_tone_detection/audio_loader.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.6/src/icad_tone_detection/frequency_extraction.py` & `icad_tone_detection-0.7/src/icad_tone_detection/frequency_extraction.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.6/src/icad_tone_detection/main.py` & `icad_tone_detection-0.7/src/icad_tone_detection/main.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-0.6/src/icad_tone_detection/tone_detection.py` & `icad_tone_detection-0.7/src/icad_tone_detection/tone_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 def detect_quickcall(frequency_matches):
     qc2_matches = []
     tone_id = 0
     last_set = None
+    if not frequency_matches or len(frequency_matches) < 1:
+        return qc2_matches
     for x in frequency_matches:
         if last_set is None and len(x[2]) >= 8 and 0 not in x[2] and 0.0 not in x[2]:
             last_set = x
         else:
             if len(x[2]) >= 8 and 0 not in x[2] and 0.0 not in x[2]:
                 if len(last_set[2]) <= 12 and len(x[2]) >= 28:
                     tone_data = {"tone_id": f'qc_{tone_id + 1}', "detected": [last_set[2][0], x[2][0]],
@@ -20,16 +22,17 @@
 
 
 def detect_long_tones(frequency_matches, detected_quickcall):
     tone_id = 0
     long_tone_matches = []
     excluded_frequencies = set([])
 
-    if not frequency_matches:
+    if not frequency_matches or len(frequency_matches) < 1:
         return long_tone_matches
+
     last_set = frequency_matches[0]
     # add detected quick call tones to a list, so we can exclude them from long tone matches.
     for ttd in detected_quickcall:
         excluded_frequencies.update(ttd["detected"][:2])
 
     for x in frequency_matches:
         if len(x[2]) >= 10:
@@ -222,16 +225,16 @@
 
     Returns:
     - A list of dictionaries, each representing a detected sequence of warble tones with its details.
     """
     sequences = []
     id_index = 1
 
-    if not frequency_matches:
-        raise ValueError("The frequency_matches list cannot be empty.")
+    if not frequency_matches or len(frequency_matches) < 1:
+        return sequences
 
     i = 0
     while i < len(frequency_matches):
         current_sequence = []
 
         while i < len(frequency_matches):
             group = frequency_matches[i]
```

### Comparing `icad_tone_detection-0.6/src/icad_tone_detection.egg-info/PKG-INFO` & `icad_tone_detection-0.7/src/icad_tone_detection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 0.6
+Version: 0.7
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-0.6/src/icad_tone_detection.egg-info/SOURCES.txt` & `icad_tone_detection-0.7/src/icad_tone_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

