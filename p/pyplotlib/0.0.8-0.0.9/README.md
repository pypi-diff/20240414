# Comparing `tmp/pyplotlib-0.0.8.tar.gz` & `tmp/pyplotlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplotlib-0.0.8.tar", last modified: Sat Mar 30 07:05:11 2024, max compression
+gzip compressed data, was "pyplotlib-0.0.9.tar", last modified: Sat Mar 30 07:13:54 2024, max compression
```

## Comparing `pyplotlib-0.0.8.tar` & `pyplotlib-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:05:10.994241 pyplotlib-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-30 07:05:03.000000 pyplotlib-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-30 07:05:10.994241 pyplotlib-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-30 07:05:03.000000 pyplotlib-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:05:10.994241 pyplotlib-0.0.8/pyplotlib/
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-03-30 07:05:03.000000 pyplotlib-0.0.8/pyplotlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:05:10.994241 pyplotlib-0.0.8/pyplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-30 07:05:10.000000 pyplotlib-0.0.8/pyplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-30 07:05:10.000000 pyplotlib-0.0.8/pyplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 07:05:10.000000 pyplotlib-0.0.8/pyplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-30 07:05:10.000000 pyplotlib-0.0.8/pyplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-30 07:05:10.000000 pyplotlib-0.0.8/pyplotlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 07:05:10.994241 pyplotlib-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3617 2024-03-30 07:05:03.000000 pyplotlib-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:13:54.395634 pyplotlib-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-30 07:13:46.000000 pyplotlib-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-30 07:13:54.395634 pyplotlib-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-30 07:13:46.000000 pyplotlib-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:13:54.391634 pyplotlib-0.0.9/pyplotlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-03-30 07:13:46.000000 pyplotlib-0.0.9/pyplotlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 07:13:54.391634 pyplotlib-0.0.9/pyplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-30 07:13:54.000000 pyplotlib-0.0.9/pyplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-30 07:13:54.000000 pyplotlib-0.0.9/pyplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 07:13:54.000000 pyplotlib-0.0.9/pyplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-30 07:13:54.000000 pyplotlib-0.0.9/pyplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-30 07:13:54.000000 pyplotlib-0.0.9/pyplotlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 07:13:54.395634 pyplotlib-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3617 2024-03-30 07:13:46.000000 pyplotlib-0.0.9/setup.py
```

### Comparing `pyplotlib-0.0.8/LICENSE` & `pyplotlib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplotlib-0.0.8/PKG-INFO` & `pyplotlib-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/pyplotlib
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pyplotlib-0.0.8/pyplotlib/__init__.py` & `pyplotlib-0.0.9/pyplotlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,14 @@
             'layout.yaxis.linecolor': 'black',
             'layout.yaxis.ticks': 'outside',
             'layout.yaxis.mirror': True,
             'layout.yaxis.showline': True,
             'layout.autosize': True,
             'layout.showlegend': True,
             'layout.legend.bgcolor': 'rgba(0, 0, 0, 0)',
-            'layout.legend.xanchor': 'right',
             'layout.legend.x': 1,
             'layout.legend.font.family': font,
             'layout.legend.font.size': font_size,
             # Specialized:
             # 'layout.xaxis.range': (2.3, 2.5),
             'layout.yaxis.range': (0, +50),
             'layout.xaxis.title': r'$x$', #Latex Style
```

### Comparing `pyplotlib-0.0.8/pyplotlib.egg-info/PKG-INFO` & `pyplotlib-0.0.9/pyplotlib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: My short description for my project.
 Home-page: https://github.com/franceme/pyplotlib
 Author: Miles Frantz
 Author-email: frantzme@vt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pyplotlib-0.0.8/setup.py` & `pyplotlib-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

