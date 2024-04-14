# Comparing `tmp/pyconn-monitor-0.1.0.tar.gz` & `tmp/pyconn-monitor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconn-monitor-0.1.0.tar", last modified: Sun Apr 14 15:16:07 2024, max compression
+gzip compressed data, was "pyconn-monitor-0.1.1.tar", last modified: Sun Apr 14 15:19:22 2024, max compression
```

## Comparing `pyconn-monitor-0.1.0.tar` & `pyconn-monitor-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:16:07.299143 pyconn-monitor-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-04-14 12:24:33.000000 pyconn-monitor-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4730 2024-04-14 15:16:07.298142 pyconn-monitor-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3818 2024-04-14 15:15:44.000000 pyconn-monitor-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 15:16:07.285869 pyconn-monitor-0.1.0/pyconn_monitor/
--rw-rw-rw-   0        0        0      232 2024-04-14 12:26:06.000000 pyconn-monitor-0.1.0/pyconn_monitor/__init__.py
--rw-rw-rw-   0        0        0     2321 2024-04-14 15:00:35.000000 pyconn-monitor-0.1.0/pyconn_monitor/cli.py
--rw-rw-rw-   0        0        0     6625 2024-04-14 15:07:49.000000 pyconn-monitor-0.1.0/pyconn_monitor/connection_monitor.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:16:07.298142 pyconn-monitor-0.1.0/pyconn_monitor.egg-info/
--rw-rw-rw-   0        0        0     4730 2024-04-14 15:16:07.000000 pyconn-monitor-0.1.0/pyconn_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2024-04-14 15:16:07.000000 pyconn-monitor-0.1.0/pyconn_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:16:07.000000 pyconn-monitor-0.1.0/pyconn_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-14 15:16:07.000000 pyconn-monitor-0.1.0/pyconn_monitor.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-04-14 15:16:07.000000 pyconn-monitor-0.1.0/pyconn_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-14 15:16:07.000000 pyconn-monitor-0.1.0/pyconn_monitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 15:16:07.300142 pyconn-monitor-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1275 2024-04-14 12:30:37.000000 pyconn-monitor-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:16:07.296144 pyconn-monitor-0.1.0/tests/
--rw-rw-rw-   0        0        0      182 2024-04-14 14:50:33.000000 pyconn-monitor-0.1.0/tests/test_connection_monitor.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:19:22.771501 pyconn-monitor-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-14 12:24:33.000000 pyconn-monitor-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4759 2024-04-14 15:19:22.769501 pyconn-monitor-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3818 2024-04-14 15:15:44.000000 pyconn-monitor-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 15:19:22.746622 pyconn-monitor-0.1.1/pyconn_monitor/
+-rw-rw-rw-   0        0        0      232 2024-04-14 12:26:06.000000 pyconn-monitor-0.1.1/pyconn_monitor/__init__.py
+-rw-rw-rw-   0        0        0     2321 2024-04-14 15:00:35.000000 pyconn-monitor-0.1.1/pyconn_monitor/cli.py
+-rw-rw-rw-   0        0        0     6625 2024-04-14 15:07:49.000000 pyconn-monitor-0.1.1/pyconn_monitor/connection_monitor.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:19:22.768506 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/
+-rw-rw-rw-   0        0        0     4759 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-14 15:19:22.000000 pyconn-monitor-0.1.1/pyconn_monitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:19:22.771501 pyconn-monitor-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2024-04-14 15:19:18.000000 pyconn-monitor-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:19:22.767503 pyconn-monitor-0.1.1/tests/
+-rw-rw-rw-   0        0        0      182 2024-04-14 14:50:33.000000 pyconn-monitor-0.1.1/tests/test_connection_monitor.py
```

### Comparing `pyconn-monitor-0.1.0/LICENSE` & `pyconn-monitor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.0/PKG-INFO` & `pyconn-monitor-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconn-monitor
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library to monitor and log network connections of untrusted programs
 Home-page: https://github.com/ParisNeo/pyconn-monitor
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
+Requires-Dist: ascii_colors
 
 # pyconn-monitor
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg)](https://python.org)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pyconn-monitor-0.1.0/README.md` & `pyconn-monitor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.0/pyconn_monitor/cli.py` & `pyconn-monitor-0.1.1/pyconn_monitor/cli.py`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.0/pyconn_monitor/connection_monitor.py` & `pyconn-monitor-0.1.1/pyconn_monitor/connection_monitor.py`

 * *Files identical despite different names*

### Comparing `pyconn-monitor-0.1.0/pyconn_monitor.egg-info/PKG-INFO` & `pyconn-monitor-0.1.1/pyconn_monitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconn-monitor
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library to monitor and log network connections of untrusted programs
 Home-page: https://github.com/ParisNeo/pyconn-monitor
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
+Requires-Dist: ascii_colors
 
 # pyconn-monitor
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg)](https://python.org)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pyconn-monitor-0.1.0/setup.py` & `pyconn-monitor-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
+with open('requirements.txt', 'r') as f:
+    install_requires = f.read().splitlines()
+
 setup(
     name='pyconn-monitor',
-    version='0.1.0',
+    version='0.1.1',
     author='ParisNeo',
     author_email='parisneoai@gmail.com',
     description='A Python library to monitor and log network connections of untrusted programs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ParisNeo/pyconn-monitor',
     packages=find_packages(),
-    install_requires=[
-        'psutil',
-    ],
+    install_requires=install_requires,
     entry_points={
         'console_scripts': [
             'pyconn-monitor=pyconn_monitor.cli:main',
         ],
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
```

