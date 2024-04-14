# Comparing `tmp/itkwasm_compare_images-5.0.1.tar.gz` & `tmp/itkwasm_compare_images-5.0.2.tar.gz`

## Comparing `itkwasm_compare_images-5.0.1.tar` & `itkwasm_compare_images-5.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/docs/Makefile
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/docs/conf.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/docs/make.bat
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/docs/_static/logo.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/itkwasm_compare_images/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/itkwasm_compare_images/_version.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/itkwasm_compare_images/compare_double_images.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/itkwasm_compare_images/compare_double_images_async.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/itkwasm_compare_images/compare_images.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/itkwasm_compare_images/compare_images_async.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/itkwasm_compare_images/vector_magnitude.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/itkwasm_compare_images/vector_magnitude_async.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/.gitignore
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/README.md
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/Makefile
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/conf.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/make.bat
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/_static/favicon.png
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/_static/logo.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/_version.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_double_images.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_double_images_async.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_images.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_images_async.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/vector_magnitude.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/vector_magnitude_async.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/.gitignore
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/README.md
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/PKG-INFO
```

### Comparing `itkwasm_compare_images-5.0.1/docs/Makefile` & `itkwasm_compare_images-5.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/docs/conf.py` & `itkwasm_compare_images-5.0.2/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 from datetime import date
+import os
 
 project = 'itkwasm-compare-images'
 copyright = f'{date.today().year}, NumFOCUS'
 author = 'Insight Software Consortium'
 
 extensions = [
     'sphinx.ext.autosummary',
@@ -42,15 +43,16 @@
 }
 
 html_theme = 'furo'
 html_static_path = ['_static']
 html_logo = "_static/logo.svg"
 html_favicon = "_static/favicon.png"
 html_title = f"{project}"
+html_baseurl = os.environ.get("SPHINX_BASE_URL", "")
 
 # Furo options
 html_theme_options = {
     "top_of_page_button": "edit",
     "source_repository": "https://github.com/InsightSoftwareConsortium/itk-wasm",
     "source_branch": "main",
-    "source_directory": "docs",
+    "source_directory": "packages/compare-images/python/itkwasm-compare-images/docs",
 }
```

### Comparing `itkwasm_compare_images-5.0.1/docs/index.md` & `itkwasm_compare_images-5.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/docs/make.bat` & `itkwasm_compare_images-5.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/docs/_static/favicon.png` & `itkwasm_compare_images-5.0.2/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/docs/_static/logo.svg` & `itkwasm_compare_images-5.0.2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/itkwasm_compare_images/compare_double_images.py` & `itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_double_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ignore_boundary_pixels: bool = False,
 ) -> Tuple[Any, Image, Image]:
     """Compare double pixel type images with a tolerance for regression testing.
 
     :param test_image: The input test image
     :type  test_image: Image
 
-    :param baseline_images: Baseline images compare against
+    :param baseline_images: Baseline images to compare against
     :type  baseline_images: Image
 
     :param difference_threshold: Intensity difference for pixels to be considered different.
     :type  difference_threshold: float
 
     :param radius_tolerance: Radius of the neighborhood around a pixel to search for similar intensity values.
     :type  radius_tolerance: int
```

### Comparing `itkwasm_compare_images-5.0.1/itkwasm_compare_images/compare_double_images_async.py` & `itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_double_images_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ignore_boundary_pixels: bool = False,
 ) -> Tuple[Any, Image, Image]:
     """Compare double pixel type images with a tolerance for regression testing.
 
     :param test_image: The input test image
     :type  test_image: Image
 
-    :param baseline_images: Baseline images compare against
+    :param baseline_images: Baseline images to compare against
     :type  baseline_images: Image
 
     :param difference_threshold: Intensity difference for pixels to be considered different.
     :type  difference_threshold: float
 
     :param radius_tolerance: Radius of the neighborhood around a pixel to search for similar intensity values.
     :type  radius_tolerance: int
```

### Comparing `itkwasm_compare_images-5.0.1/itkwasm_compare_images/compare_images.py` & `itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_images.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/itkwasm_compare_images/compare_images_async.py` & `itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_images_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/itkwasm_compare_images/vector_magnitude.py` & `itkwasm_compare_images-5.0.2/itkwasm_compare_images/vector_magnitude.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/itkwasm_compare_images/vector_magnitude_async.py` & `itkwasm_compare_images-5.0.2/itkwasm_compare_images/vector_magnitude_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.1/pyproject.toml` & `itkwasm_compare_images-5.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -29,44 +29,50 @@
   "webassembly",
   "wasi",
   "emscripten",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
-    "itkwasm >= 1.0.b131",
+    "itkwasm >= 1.0.b171",
     "itkwasm-compare-images-wasi >= 1.0.1; sys_platform != \"emscripten\"",
     "itkwasm-compare-images-emscripten >= 1.0.1; sys_platform == \"emscripten\"",
 
 ]
 
 [tool.hatch.version]
 path = "itkwasm_compare_images/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-pyodide",
-  "itk-webassemblyinterface >= 1.0.b127",
-  "itkwasm >= 1.0.b131",
+  "itk-webassemblyinterface >= 1.0.b173",
+  "itkwasm >= 1.0.b171",
 ]
 
 [project.urls]
 Home = "https://github.com/InsightSoftwareConsortium/itk-wasm"
 Source = "https://github.com/InsightSoftwareConsortium/itk-wasm"
 
 [tool.hatch.envs.default.scripts]
 test = [
-  "hatch build -t wheel",
-  "pytest -s --dist-dir=./dist --rt=chrome",
+  "hatch build -t wheel ./dist/pyodide/",
+  "pytest -s --dist-dir=./dist/pyodide --rt=chrome",
 ]
 download-pyodide = [
   "curl -L https://github.com/pyodide/pyodide/releases/download/0.24.1/pyodide-0.24.1.tar.bz2 -o pyodide.tar.bz2",
   "tar xjf pyodide.tar.bz2",
-  "rm -rf dist pyodide.tar.bz2",
+  "rm -rf dist/pyodide pyodide.tar.bz2",
+  "mkdir -p dist",
   "mv pyodide dist",
 ]
+serve = [
+  "hatch build -t wheel ./dist/pyodide",
+  'echo "\nVisit http://localhost:8877/console.html\n"',
+  "python -m http.server --directory=./dist/pyodide 8877",
+]
 
 [tool.hatch.build]
 exclude = [
   "/examples",
 ]
```

### Comparing `itkwasm_compare_images-5.0.1/PKG-INFO` & `itkwasm_compare_images-5.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: itkwasm-compare-images
-Version: 5.0.1
+Version: 5.0.2
 Summary: Compare images with a tolerance for regression testing.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: itkwasm-compare-images-emscripten>=1.0.1; sys_platform == 'emscripten'
 Requires-Dist: itkwasm-compare-images-wasi>=1.0.1; sys_platform != 'emscripten'
-Requires-Dist: itkwasm>=1.0.b131
+Requires-Dist: itkwasm>=1.0.b171
 Description-Content-Type: text/markdown
 
 # itkwasm-compare-images
 
 [![PyPI version](https://badge.fury.io/py/itkwasm-compare-images.svg)](https://badge.fury.io/py/itkwasm-compare-images)
 
 Compare images with a tolerance for regression testing.
```

