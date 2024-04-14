# Comparing `tmp/pyflame-0.3.1.tar.gz` & `tmp/pyflame-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflame-0.3.1.tar", last modified: Tue May 23 13:10:14 2023, max compression
+gzip compressed data, was "pyflame-0.3.2.tar", last modified: Sun Apr 14 12:09:33 2024, max compression
```

## Comparing `pyflame-0.3.1.tar` & `pyflame-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.130819 pyflame-0.3.1/
--rw-r--r--   0 dharding  (1000) dharding  (1000)       33 2021-05-19 13:20:43.000000 pyflame-0.3.1/.gitignore
--rw-r--r--   0 dharding  (1000) dharding  (1000)      635 2023-05-23 13:08:33.000000 pyflame-0.3.1/CHANGELOG.rst
--rw-r--r--   0 dharding  (1000) dharding  (1000)     1059 2022-02-17 13:57:58.000000 pyflame-0.3.1/LICENSE
--rw-r--r--   0 dharding  (1000) dharding  (1000)       43 2021-12-02 18:05:59.000000 pyflame-0.3.1/MANIFEST.in
--rw-r--r--   0 dharding  (1000) dharding  (1000)     5947 2023-05-23 13:10:14.130819 pyflame-0.3.1/PKG-INFO
--rw-r--r--   0 dharding  (1000) dharding  (1000)     5025 2023-05-23 11:42:38.000000 pyflame-0.3.1/README.rst
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.127485 pyflame-0.3.1/pyflame/
--rw-r--r--   0 dharding  (1000) dharding  (1000)      207 2023-05-23 13:08:33.000000 pyflame-0.3.1/pyflame/__init__.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)      158 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/__main__.py
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.127485 pyflame-0.3.1/pyflame/djdt/
--rw-r--r--   0 dharding  (1000) dharding  (1000)        0 2021-05-19 13:20:43.000000 pyflame-0.3.1/pyflame/djdt/__init__.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     1376 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/djdt/panel.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)      421 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/djdt/settings.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)      170 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/exceptions.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     3255 2022-02-20 12:55:14.000000 pyflame-0.3.1/pyflame/ipython.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     1865 2022-02-20 12:58:37.000000 pyflame-0.3.1/pyflame/render.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     3110 2022-02-21 09:43:00.000000 pyflame-0.3.1/pyflame/runner.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)     1370 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/sampler.py
--rw-r--r--   0 dharding  (1000) dharding  (1000)      733 2022-02-17 13:57:58.000000 pyflame-0.3.1/pyflame/stack.py
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.124152 pyflame-0.3.1/pyflame/templates/
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.127485 pyflame-0.3.1/pyflame/templates/pyflame/
--rw-r--r--   0 dharding  (1000) dharding  (1000)      883 2022-02-20 13:22:15.000000 pyflame-0.3.1/pyflame/templates/pyflame/panel.html
-drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2023-05-23 13:10:14.127485 pyflame-0.3.1/pyflame.egg-info/
--rw-rw-r--   0 dharding  (1000) dharding  (1000)     5947 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/PKG-INFO
--rw-rw-r--   0 dharding  (1000) dharding  (1000)      535 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/SOURCES.txt
--rw-rw-r--   0 dharding  (1000) dharding  (1000)        1 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/dependency_links.txt
--rw-rw-r--   0 dharding  (1000) dharding  (1000)        1 2021-05-16 13:26:47.000000 pyflame-0.3.1/pyflame.egg-info/not-zip-safe
--rw-r--r--   0 dharding  (1000) dharding  (1000)       75 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/requires.txt
--rw-rw-r--   0 dharding  (1000) dharding  (1000)        8 2023-05-23 13:10:14.000000 pyflame-0.3.1/pyflame.egg-info/top_level.txt
--rw-r--r--   0 dharding  (1000) dharding  (1000)      105 2021-05-19 13:20:43.000000 pyflame-0.3.1/pyproject.toml
--rw-r--r--   0 dharding  (1000) dharding  (1000)      984 2023-05-23 13:10:14.130819 pyflame-0.3.1/setup.cfg
--rwxr-xr-x   0 dharding  (1000) dharding  (1000)       62 2023-05-23 11:34:03.000000 pyflame-0.3.1/setup.py
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2024-04-14 12:09:33.008390 pyflame-0.3.2/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)       33 2021-05-19 13:20:43.000000 pyflame-0.3.2/.gitignore
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      635 2024-04-14 12:01:29.000000 pyflame-0.3.2/CHANGELOG.rst
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     1059 2022-02-17 13:57:58.000000 pyflame-0.3.2/LICENSE
+-rw-r--r--   0 dharding  (1000) dharding  (1000)       43 2021-12-02 18:05:59.000000 pyflame-0.3.2/MANIFEST.in
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     6139 2024-04-14 12:09:33.008390 pyflame-0.3.2/PKG-INFO
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     5025 2024-04-14 12:01:29.000000 pyflame-0.3.2/README.rst
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2024-04-14 12:09:33.005056 pyflame-0.3.2/pyflame/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      207 2024-04-14 12:01:29.000000 pyflame-0.3.2/pyflame/__init__.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      158 2022-02-17 13:57:58.000000 pyflame-0.3.2/pyflame/__main__.py
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2024-04-14 12:09:33.008390 pyflame-0.3.2/pyflame/djdt/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)        0 2021-05-19 13:20:43.000000 pyflame-0.3.2/pyflame/djdt/__init__.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     1376 2022-02-17 13:57:58.000000 pyflame-0.3.2/pyflame/djdt/panel.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      421 2022-02-17 13:57:58.000000 pyflame-0.3.2/pyflame/djdt/settings.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      170 2022-02-17 13:57:58.000000 pyflame-0.3.2/pyflame/exceptions.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     3255 2022-02-20 12:55:14.000000 pyflame-0.3.2/pyflame/ipython.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     1865 2022-02-20 12:58:37.000000 pyflame-0.3.2/pyflame/render.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     3110 2022-02-21 09:43:00.000000 pyflame-0.3.2/pyflame/runner.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     1370 2022-02-17 13:57:58.000000 pyflame-0.3.2/pyflame/sampler.py
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      733 2022-02-17 13:57:58.000000 pyflame-0.3.2/pyflame/stack.py
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2024-04-14 12:09:33.001723 pyflame-0.3.2/pyflame/templates/
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2024-04-14 12:09:33.008390 pyflame-0.3.2/pyflame/templates/pyflame/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      883 2022-02-20 13:22:15.000000 pyflame-0.3.2/pyflame/templates/pyflame/panel.html
+drwxr-xr-x   0 dharding  (1000) dharding  (1000)        0 2024-04-14 12:09:33.008390 pyflame-0.3.2/pyflame.egg-info/
+-rw-r--r--   0 dharding  (1000) dharding  (1000)     6139 2024-04-14 12:09:32.000000 pyflame-0.3.2/pyflame.egg-info/PKG-INFO
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)      535 2024-04-14 12:09:33.000000 pyflame-0.3.2/pyflame.egg-info/SOURCES.txt
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)        1 2024-04-14 12:09:32.000000 pyflame-0.3.2/pyflame.egg-info/dependency_links.txt
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)        1 2021-05-16 13:26:47.000000 pyflame-0.3.2/pyflame.egg-info/not-zip-safe
+-rw-r--r--   0 dharding  (1000) dharding  (1000)       75 2024-04-14 12:09:32.000000 pyflame-0.3.2/pyflame.egg-info/requires.txt
+-rw-rw-r--   0 dharding  (1000) dharding  (1000)        8 2024-04-14 12:09:32.000000 pyflame-0.3.2/pyflame.egg-info/top_level.txt
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      105 2021-05-19 13:20:43.000000 pyflame-0.3.2/pyproject.toml
+-rw-r--r--   0 dharding  (1000) dharding  (1000)      965 2024-04-14 12:09:33.008390 pyflame-0.3.2/setup.cfg
+-rwxr-xr-x   0 dharding  (1000) dharding  (1000)       62 2024-04-14 12:01:29.000000 pyflame-0.3.2/setup.py
```

### Comparing `pyflame-0.3.1/CHANGELOG.rst` & `pyflame-0.3.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/LICENSE` & `pyflame-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/PKG-INFO` & `pyflame-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflame
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Flamegraph generator for Python
 Home-page: https://gitlab.com/living180/pyflame
 Author: Daniel Harding
 Author-email: dharding@living180.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Django
@@ -16,17 +16,21 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: jupyter
+Requires-Dist: ipython; extra == "jupyter"
+Requires-Dist: traitlets>=5; extra == "jupyter"
 Provides-Extra: django
-License-File: LICENSE
+Requires-Dist: django>=3.2; extra == "django"
+Requires-Dist: django-debug-toolbar; extra == "django"
 
 ..
   Copyright 2020-2022 Daniel Harding
   Distributed as part of the pyflame project under the terms of the MIT license
 
 Generate flamegraphs for Python code, using Brendan Gregg's excellent FlameGraph_
 project to perform the heavy lifting.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_da6twcxq_/tmpx8s1e_j__TarContainer/0/5", line 162, column 0: CDATA terminal not found*

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1 Name: pyflame Version: 0.3.1 Summary: A Flamegraph
+Metadata-Version: 2.1 Name: pyflame Version: 0.3.2 Summary: A Flamegraph
 generator for Python Home-page: https://gitlab.com/living180/pyflame Author:
 Daniel Harding Author-email: dharding@living180.net Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Console Classifier: Framework ::
 Django Classifier: Framework :: Jupyter Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
-Type: text/x-rst Provides-Extra: jupyter Provides-Extra: django License-File:
-LICENSE .. Copyright 2020-2022 Daniel Harding Distributed as part of the
-pyflame project under the terms of the MIT license Generate flamegraphs for
-Python code, using Brendan Gregg's excellent FlameGraph_ project to perform the
-heavy lifting. pyflame can be used to invoke a Python script from the command
-line and generate a flamegraph of its execution. It also provides a panel for
-`Django Debug Toolbar`_ that generates a flamegraph for each request, as well
-as an IPython_ extension that provides a cell magic to generate flamegraphs for
-display within a `Jupyter Notebook`_. Basic Installation ------------------ *
-Run ``python -m pip install pyflame``. * Download flamegraph.pl_ and then
-either: - make it available via the ``PATH`` environment variable, or - set up
-the appropriate configuration as described below to indicate where the script
-is located on the filesystem. Command Line Usage ------------------ Invoke
-using ``python -m pyflame []
+Type: text/x-rst License-File: LICENSE Provides-Extra: jupyter Requires-Dist:
+ipython; extra == "jupyter" Requires-Dist: traitlets>=5; extra == "jupyter"
+Provides-Extra: django Requires-Dist: django>=3.2; extra == "django" Requires-
+Dist: django-debug-toolbar; extra == "django" .. Copyright 2020-2022 Daniel
+Harding Distributed as part of the pyflame project under the terms of the MIT
+license Generate flamegraphs for Python code, using Brendan Gregg's excellent
+FlameGraph_ project to perform the heavy lifting. pyflame can be used to invoke
+a Python script from the command line and generate a flamegraph of its
+execution. It also provides a panel for `Django Debug Toolbar`_ that generates
+a flamegraph for each request, as well as an IPython_ extension that provides a
+cell magic to generate flamegraphs for display within a `Jupyter Notebook`_.
+Basic Installation ------------------ * Run ``python -m pip install pyflame``.
+* Download flamegraph.pl_ and then either: - make it available via the ``PATH``
+environment variable, or - set up the appropriate configuration as described
+below to indicate where the script is located on the filesystem. Command Line
+Usage ------------------ Invoke using ``python -m pyflame []
```

### Comparing `pyflame-0.3.1/README.rst` & `pyflame-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/pyflame/djdt/panel.py` & `pyflame-0.3.2/pyflame/djdt/panel.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/pyflame/ipython.py` & `pyflame-0.3.2/pyflame/ipython.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/pyflame/render.py` & `pyflame-0.3.2/pyflame/render.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/pyflame/runner.py` & `pyflame-0.3.2/pyflame/runner.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/pyflame/sampler.py` & `pyflame-0.3.2/pyflame/sampler.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/pyflame/stack.py` & `pyflame-0.3.2/pyflame/stack.py`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/pyflame/templates/pyflame/panel.html` & `pyflame-0.3.2/pyflame/templates/pyflame/panel.html`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/pyflame.egg-info/PKG-INFO` & `pyflame-0.3.2/pyflame.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflame
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Flamegraph generator for Python
 Home-page: https://gitlab.com/living180/pyflame
 Author: Daniel Harding
 Author-email: dharding@living180.net
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Django
@@ -16,17 +16,21 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 Provides-Extra: jupyter
+Requires-Dist: ipython; extra == "jupyter"
+Requires-Dist: traitlets>=5; extra == "jupyter"
 Provides-Extra: django
-License-File: LICENSE
+Requires-Dist: django>=3.2; extra == "django"
+Requires-Dist: django-debug-toolbar; extra == "django"
 
 ..
   Copyright 2020-2022 Daniel Harding
   Distributed as part of the pyflame project under the terms of the MIT license
 
 Generate flamegraphs for Python code, using Brendan Gregg's excellent FlameGraph_
 project to perform the heavy lifting.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_da6twcxq_/tmpx8s1e_j__TarContainer/0/24", line 162, column 0: CDATA terminal not found*

```diff
@@ -1,25 +1,27 @@
-Metadata-Version: 2.1 Name: pyflame Version: 0.3.1 Summary: A Flamegraph
+Metadata-Version: 2.1 Name: pyflame Version: 0.3.2 Summary: A Flamegraph
 generator for Python Home-page: https://gitlab.com/living180/pyflame Author:
 Daniel Harding Author-email: dharding@living180.net Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: Console Classifier: Framework ::
 Django Classifier: Framework :: Jupyter Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
-Type: text/x-rst Provides-Extra: jupyter Provides-Extra: django License-File:
-LICENSE .. Copyright 2020-2022 Daniel Harding Distributed as part of the
-pyflame project under the terms of the MIT license Generate flamegraphs for
-Python code, using Brendan Gregg's excellent FlameGraph_ project to perform the
-heavy lifting. pyflame can be used to invoke a Python script from the command
-line and generate a flamegraph of its execution. It also provides a panel for
-`Django Debug Toolbar`_ that generates a flamegraph for each request, as well
-as an IPython_ extension that provides a cell magic to generate flamegraphs for
-display within a `Jupyter Notebook`_. Basic Installation ------------------ *
-Run ``python -m pip install pyflame``. * Download flamegraph.pl_ and then
-either: - make it available via the ``PATH`` environment variable, or - set up
-the appropriate configuration as described below to indicate where the script
-is located on the filesystem. Command Line Usage ------------------ Invoke
-using ``python -m pyflame []
+Type: text/x-rst License-File: LICENSE Provides-Extra: jupyter Requires-Dist:
+ipython; extra == "jupyter" Requires-Dist: traitlets>=5; extra == "jupyter"
+Provides-Extra: django Requires-Dist: django>=3.2; extra == "django" Requires-
+Dist: django-debug-toolbar; extra == "django" .. Copyright 2020-2022 Daniel
+Harding Distributed as part of the pyflame project under the terms of the MIT
+license Generate flamegraphs for Python code, using Brendan Gregg's excellent
+FlameGraph_ project to perform the heavy lifting. pyflame can be used to invoke
+a Python script from the command line and generate a flamegraph of its
+execution. It also provides a panel for `Django Debug Toolbar`_ that generates
+a flamegraph for each request, as well as an IPython_ extension that provides a
+cell magic to generate flamegraphs for display within a `Jupyter Notebook`_.
+Basic Installation ------------------ * Run ``python -m pip install pyflame``.
+* Download flamegraph.pl_ and then either: - make it available via the ``PATH``
+environment variable, or - set up the appropriate configuration as described
+below to indicate where the script is located on the filesystem. Command Line
+Usage ------------------ Invoke using ``python -m pyflame []
```

### Comparing `pyflame-0.3.1/pyflame.egg-info/SOURCES.txt` & `pyflame-0.3.2/pyflame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflame-0.3.1/setup.cfg` & `pyflame-0.3.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyflame
-version = 0.3.1
+version = 0.3.2
 url = https://gitlab.com/living180/pyflame
 author = Daniel Harding
 author_email = dharding@living180.net
 description = A Flamegraph generator for Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 classifiers = 
@@ -20,15 +20,14 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 
 [options]
 python_requires = >= 3.7
-packages = pyflame
 include_package_data = true
 zip_safe = false
 
 [options.extras_require]
 jupyter = 
 	ipython
 	traitlets >= 5
```

