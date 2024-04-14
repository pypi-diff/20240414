# Comparing `tmp/PySAGA-cmd-1.2.2.tar.gz` & `tmp/PySAGA-cmd-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySAGA-cmd-1.2.2.tar", last modified: Sat Mar 30 05:58:07 2024, max compression
+gzip compressed data, was "PySAGA-cmd-1.2.3.tar", last modified: Sun Apr 14 07:52:04 2024, max compression
```

## Comparing `PySAGA-cmd-1.2.2.tar` & `PySAGA-cmd-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-30 05:58:07.954433 PySAGA-cmd-1.2.2/
--rw-r--r--   0 alex      (1000) alex      (1000)      304 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/CITATION.cff
--rw-r--r--   0 alex      (1000) alex      (1000)     1076 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      306 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)     7135 2024-03-30 05:58:07.954433 PySAGA-cmd-1.2.2/PKG-INFO
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-30 05:58:07.950433 PySAGA-cmd-1.2.2/PySAGA_cmd/
--rw-r--r--   0 alex      (1000) alex      (1000)       59 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd/__init__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-30 05:58:07.950433 PySAGA-cmd-1.2.2/PySAGA_cmd/assets/
--rw-r--r--   0 alex      (1000) alex      (1000)   282855 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd/assets/DEM_30m.tif
--rw-r--r--   0 alex      (1000) alex      (1000)     6760 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd/objects.py
--rw-r--r--   0 alex      (1000) alex      (1000)    27574 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd/saga.py
--rw-r--r--   0 alex      (1000) alex      (1000)     7999 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd/utils.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-03-30 05:58:07.950433 PySAGA-cmd-1.2.2/PySAGA_cmd.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     7135 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      340 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       17 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/PySAGA_cmd.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)     5750 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/README.md
--rw-r--r--   0 alex      (1000) alex      (1000)     1409 2024-03-30 05:58:07.000000 PySAGA-cmd-1.2.2/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2024-03-30 05:58:07.954433 PySAGA-cmd-1.2.2/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:52:04.749991 PySAGA-cmd-1.2.3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      304 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/CITATION.cff
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1076 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)      306 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)     7177 2024-04-14 07:52:04.749991 PySAGA-cmd-1.2.3/PKG-INFO
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:52:04.745991 PySAGA-cmd-1.2.3/PySAGA_cmd/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       59 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:52:04.745991 PySAGA-cmd-1.2.3/PySAGA_cmd/assets/
+-rw-rw-r--   0 alex      (1000) alex      (1000)   282855 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/assets/DEM_30m.tif
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6760 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/objects.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    27736 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/saga.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8153 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd/utils.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2024-04-14 07:52:04.749991 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     7177 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      340 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      177 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5792 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/README.md
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2024-04-14 07:52:04.000000 PySAGA-cmd-1.2.3/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2024-04-14 07:52:04.749991 PySAGA-cmd-1.2.3/setup.cfg
```

### Comparing `PySAGA-cmd-1.2.2/LICENSE` & `PySAGA-cmd-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PySAGA-cmd-1.2.2/PKG-INFO` & `PySAGA-cmd-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySAGA-cmd
-Version: 1.2.2
+Version: 1.2.3
 Summary: A package that allows you to run SAGA GIS tools using Python.
 Author-email: Alex-Andrei Cuvuliuc <cuvuliucalexandrei@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/alecsandrei/PySAGA-cmd
 Keywords: PySAGA-cmd
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -199,7 +199,8 @@
 
 
 # TODOs
 
 - [x] Implement recursive search for the saga_cmd file.
 - [x] Improve the verbose behaviour of tool execution (add a progress bar?).
 - [ ] Improve flags.
+- [ ] Add "elapsed time" to progress bar.
```

### Comparing `PySAGA-cmd-1.2.2/PySAGA_cmd/assets/DEM_30m.tif` & `PySAGA-cmd-1.2.3/PySAGA_cmd/assets/DEM_30m.tif`

 * *Files identical despite different names*

### Comparing `PySAGA-cmd-1.2.2/PySAGA_cmd/objects.py` & `PySAGA-cmd-1.2.3/PySAGA_cmd/objects.py`

 * *Files identical despite different names*

### Comparing `PySAGA-cmd-1.2.2/PySAGA_cmd/saga.py` & `PySAGA-cmd-1.2.3/PySAGA_cmd/saga.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,17 @@
             self._raster_formats = formats.union(
                 ['sdat', 'sgrd', 'sg-grd-z']
             )
         return self._raster_formats
 
     def get_vector_formats(self):
         if self._vector_formats is None:
-            self._vector_formats = get_formats(self, type_='vector')
+            formats = get_formats(self, type_='vector')
+            if formats is None:
+                formats = set()
         return self._vector_formats
 
     @property
     def temp_dir(self) -> Path:
         if not self._temp_dir.exists():
             self._temp_dir = temp_dir()
         return self._temp_dir
@@ -881,33 +883,36 @@
     # Create an empty temporary file.
     with tempfile.NamedTemporaryFile(delete=False) as tmp:
         path = Path(tmp.name)
 
         gdal_formats_execute = partial(
             gdal_formats.execute,
             formats=path,
-            acces=2,
+            access=2,
             recognized=1,
             verbose=False,
             infer_obj_type=False,
         )
         assert type_ in ['raster', 'vector']
 
-        if type_ == 'raster':
-            gdal_formats_execute(type='0')
+        try:
+            if type_ == 'raster':
+                gdal_formats_execute(type='0')
+            else:
+                gdal_formats_execute(type='1')
+        except:
+            return None
         else:
-            gdal_formats_execute(type='1')
-
-        reader = csv.reader(
-            [string.decode('utf-8') for string in tmp.readlines()],
-            dialect="excel-tab"
-        )
-        last_row = tuple(reader)[-1]
-        third_column = last_row[2]
-        extensions = re.findall(r'\.(\w+)', third_column)
+            reader = csv.reader(
+                [string.decode('utf-8') for string in tmp.readlines()],
+                dialect="excel-tab"
+            )
+            last_row = tuple(reader)[-1]
+            third_column = last_row[2]
+            extensions = re.findall(r'\.(\w+)', third_column)
     return set(extensions)
 
 
 class ExecutionError(Exception):
     """Raised when an execution outputs a stderr."""
     def __init__(self, stderr: str, saga_executable: SAGAExecutable):
         self.stderr = stderr
```

### Comparing `PySAGA-cmd-1.2.2/PySAGA_cmd/utils.py` & `PySAGA-cmd-1.2.3/PySAGA_cmd/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     Generator
 )
 from pathlib import Path
 from enum import (
     Enum,
     auto
 )
+import time
+import datetime
 
 
 HERE = Path(__file__).parent
 
 
 class Platforms(Enum):
     WINDOWS = auto()
@@ -137,24 +139,25 @@
     size: int = 60
 ) -> Generator[None, Optional[int], None]:
     # Inspired by https://stackoverflow.com/a/34482761
     count = 100
     size = 60
     j = 0
     out = sys.stdout
+    start = time.time()
     while True:
         j = yield  # type: ignore
         if j is None:
             continue
         elif j > 100:
             j = 100
         x = int(size*j/count)
-
+        elapsed = datetime.timedelta(seconds=round(time.time()-start))
         print(
-            f"[{u'█'*x}{('.'*(size-x))}] {j}/{count}% {len(str(j))*' '}",
+            f"[{u'█'*x}{('.'*(size-x))}] {j}/{count}% | Elapsed time: {elapsed} {len(str(elapsed))*' '}",
             end='\r',
             flush=True,
             file=out
         )
 
 
 class NotExecutableError(Exception):
```

### Comparing `PySAGA-cmd-1.2.2/PySAGA_cmd.egg-info/PKG-INFO` & `PySAGA-cmd-1.2.3/PySAGA_cmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySAGA-cmd
-Version: 1.2.2
+Version: 1.2.3
 Summary: A package that allows you to run SAGA GIS tools using Python.
 Author-email: Alex-Andrei Cuvuliuc <cuvuliucalexandrei@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/alecsandrei/PySAGA-cmd
 Keywords: PySAGA-cmd
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -199,7 +199,8 @@
 
 
 # TODOs
 
 - [x] Implement recursive search for the saga_cmd file.
 - [x] Improve the verbose behaviour of tool execution (add a progress bar?).
 - [ ] Improve flags.
+- [ ] Add "elapsed time" to progress bar.
```

### Comparing `PySAGA-cmd-1.2.2/README.md` & `PySAGA-cmd-1.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -163,7 +163,8 @@
 
 
 # TODOs
 
 - [x] Implement recursive search for the saga_cmd file.
 - [x] Improve the verbose behaviour of tool execution (add a progress bar?).
 - [ ] Improve flags.
+- [ ] Add "elapsed time" to progress bar.
```

### Comparing `PySAGA-cmd-1.2.2/pyproject.toml` & `PySAGA-cmd-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PySAGA-cmd"
-version = "1.2.2"
+version = "1.2.3"
 dynamic = [
     "dependencies",
 ]
 description = "A package that allows you to run SAGA GIS tools using Python."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
```

