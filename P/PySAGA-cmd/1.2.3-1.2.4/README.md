# Comparing `tmp/PySAGA-cmd-1.2.3.tar.gz` & `tmp/PySAGA-cmd-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySAGA-cmd-1.2.3.tar", last modified: Sun Apr 14 07:52:04 2024, max compression
+gzip compressed data, was "PySAGA-cmd-1.2.4.tar", last modified: Sun Apr 14 07:55:05 2024, max compression
```

## Comparing `PySAGA-cmd-1.2.3.tar` & `PySAGA-cmd-1.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:52:04.749991 PySAGA-cmd-1.2.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)      304 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/CITATION.cff
--rw-rw-r--   0 alex      (1000) alex      (1000)     1076 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)      306 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)     7177 2024-04-14 07:52:04.749991 PySAGA-cmd-1.2.3/PKG-INFO
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:52:04.745991 PySAGA-cmd-1.2.3/PySAGA_cmd/
--rw-rw-r--   0 alex      (1000) alex      (1000)       59 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:52:04.745991 PySAGA-cmd-1.2.3/PySAGA_cmd/assets/
--rw-rw-r--   0 alex      (1000) alex      (1000)   282855 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/assets/DEM_30m.tif
--rw-rw-r--   0 alex      (1000) alex      (1000)     6760 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/objects.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    27736 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/saga.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8153 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/utils.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:52:04.749991 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     7177 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      340 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      177 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)     5792 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/README.md
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2024-04-14 07:52:04.749991 PySAGA-cmd-1.2.3/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:55:05.877568 PySAGA-cmd-1.2.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      304 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/CITATION.cff
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1076 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)      306 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)     7177 2024-04-14 07:55:05.877568 PySAGA-cmd-1.2.4/PKG-INFO
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:55:05.873568 PySAGA-cmd-1.2.4/PySAGA_cmd/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       59 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:55:05.873568 PySAGA-cmd-1.2.4/PySAGA_cmd/assets/
+-rw-rw-r--   0 alex      (1000) alex      (1000)   282855 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd/assets/DEM_30m.tif
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6760 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd/objects.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    27775 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd/saga.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8153 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd/utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:55:05.877568 PySAGA-cmd-1.2.4/PySAGA_cmd.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     7177 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      340 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      177 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/PySAGA_cmd.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5792 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2024-04-14 07:55:05.000000 PySAGA-cmd-1.2.4/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2024-04-14 07:55:05.877568 PySAGA-cmd-1.2.4/setup.cfg
```

### Comparing `PySAGA-cmd-1.2.3/LICENSE` & `PySAGA-cmd-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PySAGA-cmd-1.2.3/PKG-INFO` & `PySAGA-cmd-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySAGA-cmd
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package that allows you to run SAGA GIS tools using Python.
 Author-email: Alex-Andrei Cuvuliuc <cuvuliucalexandrei@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/alecsandrei/PySAGA-cmd
 Keywords: PySAGA-cmd
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PySAGA-cmd-1.2.3/PySAGA_cmd/assets/DEM_30m.tif` & `PySAGA-cmd-1.2.4/PySAGA_cmd/assets/DEM_30m.tif`

 * *Files identical despite different names*

### Comparing `PySAGA-cmd-1.2.3/PySAGA_cmd/objects.py` & `PySAGA-cmd-1.2.4/PySAGA_cmd/objects.py`

 * *Files identical despite different names*

### Comparing `PySAGA-cmd-1.2.3/PySAGA_cmd/saga.py` & `PySAGA-cmd-1.2.4/PySAGA_cmd/saga.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,17 +301,17 @@
             self._raster_formats = formats.union(
                 ['sdat', 'sgrd', 'sg-grd-z']
             )
         return self._raster_formats
 
     def get_vector_formats(self):
         if self._vector_formats is None:
-            formats = get_formats(self, type_='vector')
-            if formats is None:
-                formats = set()
+            self._vector_formats = get_formats(self, type_='vector')
+            if self._vector_formats is None:
+                self._vector_formats = set()
         return self._vector_formats
 
     @property
     def temp_dir(self) -> Path:
         if not self._temp_dir.exists():
             self._temp_dir = temp_dir()
         return self._temp_dir
```

### Comparing `PySAGA-cmd-1.2.3/PySAGA_cmd/utils.py` & `PySAGA-cmd-1.2.4/PySAGA_cmd/utils.py`

 * *Files identical despite different names*

### Comparing `PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/PKG-INFO` & `PySAGA-cmd-1.2.4/PySAGA_cmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySAGA-cmd
-Version: 1.2.3
+Version: 1.2.4
 Summary: A package that allows you to run SAGA GIS tools using Python.
 Author-email: Alex-Andrei Cuvuliuc <cuvuliucalexandrei@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/alecsandrei/PySAGA-cmd
 Keywords: PySAGA-cmd
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PySAGA-cmd-1.2.3/README.md` & `PySAGA-cmd-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `PySAGA-cmd-1.2.3/pyproject.toml` & `PySAGA-cmd-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PySAGA-cmd"
-version = "1.2.3"
+version = "1.2.4"
 dynamic = [
     "dependencies",
 ]
 description = "A package that allows you to run SAGA GIS tools using Python."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
```

