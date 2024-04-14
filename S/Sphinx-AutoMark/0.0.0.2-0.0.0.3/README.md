# Comparing `tmp/Sphinx-AutoMark-0.0.0.2.tar.gz` & `tmp/Sphinx-AutoMark-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sphinx-AutoMark-0.0.0.2.tar", last modified: Sun Apr 14 17:31:38 2024, max compression
+gzip compressed data, was "Sphinx-AutoMark-0.0.0.3.tar", last modified: Sun Apr 14 17:36:02 2024, max compression
```

## Comparing `Sphinx-AutoMark-0.0.0.2.tar` & `Sphinx-AutoMark-0.0.0.3.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:31:38.023369 Sphinx-AutoMark-0.0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-14 17:31:38.023369 Sphinx-AutoMark-0.0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:31:38.023369 Sphinx-AutoMark-0.0.0.2/Sphinx_AutoMark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-14 17:31:38.000000 Sphinx-AutoMark-0.0.0.2/Sphinx_AutoMark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-14 17:31:38.000000 Sphinx-AutoMark-0.0.0.2/Sphinx_AutoMark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:31:38.000000 Sphinx-AutoMark-0.0.0.2/Sphinx_AutoMark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-14 17:31:38.000000 Sphinx-AutoMark-0.0.0.2/Sphinx_AutoMark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 17:31:38.000000 Sphinx-AutoMark-0.0.0.2/Sphinx_AutoMark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:31:38.023369 Sphinx-AutoMark-0.0.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:31:38.023369 Sphinx-AutoMark-0.0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:31:38.023369 Sphinx-AutoMark-0.0.0.2/sphinx_automark/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/sphinx_automark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/sphinx_automark/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/sphinx_automark/_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/sphinx_automark/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/sphinx_automark/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-14 17:31:29.000000 Sphinx-AutoMark-0.0.0.2/sphinx_automark/multicategory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:36:02.987076 Sphinx-AutoMark-0.0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-14 17:36:02.987076 Sphinx-AutoMark-0.0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:36:02.987076 Sphinx-AutoMark-0.0.0.3/Sphinx_AutoMark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-14 17:36:02.000000 Sphinx-AutoMark-0.0.0.3/Sphinx_AutoMark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 17:36:02.000000 Sphinx-AutoMark-0.0.0.3/Sphinx_AutoMark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:36:02.000000 Sphinx-AutoMark-0.0.0.3/Sphinx_AutoMark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-14 17:36:02.000000 Sphinx-AutoMark-0.0.0.3/Sphinx_AutoMark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 17:36:02.000000 Sphinx-AutoMark-0.0.0.3/Sphinx_AutoMark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:36:02.983076 Sphinx-AutoMark-0.0.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:36:02.987076 Sphinx-AutoMark-0.0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:36:02.987076 Sphinx-AutoMark-0.0.0.3/sphinx_automark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/category.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:36:02.987076 Sphinx-AutoMark-0.0.0.3/sphinx_automark/items/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/items/category_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/items/class_category_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/items/func_category_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-14 17:35:58.000000 Sphinx-AutoMark-0.0.0.3/sphinx_automark/multicategory.py
```

### Comparing `Sphinx-AutoMark-0.0.0.2/LICENSE` & `Sphinx-AutoMark-0.0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Sphinx-AutoMark-0.0.0.2/PKG-INFO` & `Sphinx-AutoMark-0.0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sphinx-AutoMark
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: A tool for generating Sphinx Autodoc's directive based on decorated functions and classes in code.
 Author: David Hozic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `Sphinx-AutoMark-0.0.0.2/README.rst` & `Sphinx-AutoMark-0.0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `Sphinx-AutoMark-0.0.0.2/Sphinx_AutoMark.egg-info/PKG-INFO` & `Sphinx-AutoMark-0.0.0.3/Sphinx_AutoMark.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sphinx-AutoMark
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: A tool for generating Sphinx Autodoc's directive based on decorated functions and classes in code.
 Author: David Hozic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `Sphinx-AutoMark-0.0.0.2/pyproject.toml` & `Sphinx-AutoMark-0.0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -19,16 +19,15 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dynamic = ["optional-dependencies", "version"]
 
-[tool.setuptools]
-packages=["sphinx_automark"]
-include-package-data = true
+[tool.setuptools.packages.find]
+include=["sphinx_automark*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "sphinx_automark.__version__"}
 
 [tool.setuptools.dynamic.optional-dependencies.docs]
 file = "requirements/docs.txt"
```

### Comparing `Sphinx-AutoMark-0.0.0.2/sphinx_automark/__init__.py` & `Sphinx-AutoMark-0.0.0.3/sphinx_automark/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from .category import *
 from .multicategory import *
 
 
-__version__ = "0.0.0.2"
+__version__ = "0.0.0.3"
```

### Comparing `Sphinx-AutoMark-0.0.0.2/sphinx_automark/__main__.py` & `Sphinx-AutoMark-0.0.0.3/sphinx_automark/__main__.py`

 * *Files identical despite different names*

### Comparing `Sphinx-AutoMark-0.0.0.2/sphinx_automark/_doc.py` & `Sphinx-AutoMark-0.0.0.3/sphinx_automark/_doc.py`

 * *Files identical despite different names*

### Comparing `Sphinx-AutoMark-0.0.0.2/sphinx_automark/base.py` & `Sphinx-AutoMark-0.0.0.3/sphinx_automark/base.py`

 * *Files identical despite different names*

### Comparing `Sphinx-AutoMark-0.0.0.2/sphinx_automark/category.py` & `Sphinx-AutoMark-0.0.0.3/sphinx_automark/category.py`

 * *Files identical despite different names*

### Comparing `Sphinx-AutoMark-0.0.0.2/sphinx_automark/multicategory.py` & `Sphinx-AutoMark-0.0.0.3/sphinx_automark/multicategory.py`

 * *Files identical despite different names*

