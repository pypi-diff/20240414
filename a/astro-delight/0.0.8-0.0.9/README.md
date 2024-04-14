# Comparing `tmp/astro-delight-0.0.8.tar.gz` & `tmp/astro-delight-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-delight-0.0.8.tar", last modified: Tue Mar 14 15:21:33 2023, max compression
+gzip compressed data, was "astro-delight-0.0.9.tar", last modified: Wed Feb 14 22:44:00 2024, max compression
```

## Comparing `astro-delight-0.0.8.tar` & `astro-delight-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2023-03-14 15:21:33.817544 astro-delight-0.0.8/
--rw-rw-r--   0 fforster  (1000) fforster  (1000)     5179 2023-03-14 15:21:33.817544 astro-delight-0.0.8/PKG-INFO
--rw-rw-r--   0 fforster  (1000) fforster  (1000)     4438 2023-01-17 14:00:07.000000 astro-delight-0.0.8/README.md
-drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2023-03-14 15:21:33.813544 astro-delight-0.0.8/astro_delight.egg-info/
--rw-rw-r--   0 fforster  (1000) fforster  (1000)     5179 2023-03-14 15:21:33.000000 astro-delight-0.0.8/astro_delight.egg-info/PKG-INFO
--rw-rw-r--   0 fforster  (1000) fforster  (1000)      287 2023-03-14 15:21:33.000000 astro-delight-0.0.8/astro_delight.egg-info/SOURCES.txt
--rw-rw-r--   0 fforster  (1000) fforster  (1000)        1 2023-03-14 15:21:33.000000 astro-delight-0.0.8/astro_delight.egg-info/dependency_links.txt
--rw-rw-r--   0 fforster  (1000) fforster  (1000)       64 2023-03-14 15:21:33.000000 astro-delight-0.0.8/astro_delight.egg-info/requires.txt
--rw-rw-r--   0 fforster  (1000) fforster  (1000)        8 2023-03-14 15:21:33.000000 astro-delight-0.0.8/astro_delight.egg-info/top_level.txt
-drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2023-03-14 15:21:33.809544 astro-delight-0.0.8/delight/
-drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2023-03-14 15:21:33.817544 astro-delight-0.0.8/delight/delight/
--rw-rw-r--   0 fforster  (1000) fforster  (1000)  9359688 2022-07-19 18:37:09.000000 astro-delight-0.0.8/delight/delight/DELIGHT_v1.h5
--rw-rw-r--   0 fforster  (1000) fforster  (1000)       23 2022-07-22 14:23:41.000000 astro-delight-0.0.8/delight/delight/__init__.py
--rw-rw-r--   0 fforster  (1000) fforster  (1000)    42486 2023-01-18 02:27:52.000000 astro-delight-0.0.8/delight/delight/delight.py
--rw-rw-r--   0 fforster  (1000) fforster  (1000)       38 2023-03-14 15:21:33.817544 astro-delight-0.0.8/setup.cfg
--rw-rw-r--   0 fforster  (1000) fforster  (1000)     1687 2023-03-14 15:21:12.000000 astro-delight-0.0.8/setup.py
+drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2024-02-14 22:44:00.817155 astro-delight-0.0.9/
+-rw-r--r--   0 fforster  (1000) fforster  (1000)     5341 2024-02-14 22:44:00.817155 astro-delight-0.0.9/PKG-INFO
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)     4438 2023-01-17 14:00:07.000000 astro-delight-0.0.9/README.md
+drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2024-02-14 22:44:00.817155 astro-delight-0.0.9/astro_delight.egg-info/
+-rw-r--r--   0 fforster  (1000) fforster  (1000)     5341 2024-02-14 22:44:00.000000 astro-delight-0.0.9/astro_delight.egg-info/PKG-INFO
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)      429 2024-02-14 22:44:00.000000 astro-delight-0.0.9/astro_delight.egg-info/SOURCES.txt
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)        1 2024-02-14 22:44:00.000000 astro-delight-0.0.9/astro_delight.egg-info/dependency_links.txt
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)       57 2024-02-14 22:44:00.000000 astro-delight-0.0.9/astro_delight.egg-info/requires.txt
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)        8 2024-02-14 22:44:00.000000 astro-delight-0.0.9/astro_delight.egg-info/top_level.txt
+drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2024-02-14 22:44:00.805155 astro-delight-0.0.9/data/
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)     1375 2022-07-22 15:50:36.000000 astro-delight-0.0.9/data/testcoords.csv
+drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2024-02-14 22:44:00.805155 astro-delight-0.0.9/delight/
+drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2024-02-14 22:44:00.809155 astro-delight-0.0.9/delight/delight/
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)  9359688 2022-07-19 18:37:09.000000 astro-delight-0.0.9/delight/delight/DELIGHT_v1.h5
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)       23 2022-07-22 14:23:41.000000 astro-delight-0.0.9/delight/delight/__init__.py
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)    42487 2024-02-14 22:38:23.000000 astro-delight-0.0.9/delight/delight/delight.py
+drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2024-02-14 22:44:00.813156 astro-delight-0.0.9/figures/
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)    45029 2022-07-20 13:54:57.000000 astro-delight-0.0.9/figures/Delight.png
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)   325592 2022-07-20 01:34:16.000000 astro-delight-0.0.9/figures/delight_architecture.png
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)   724999 2022-07-20 01:34:41.000000 astro-delight-0.0.9/figures/multi-resolution.png
+drwxrwxr-x   0 fforster  (1000) fforster  (1000)        0 2024-02-14 22:44:00.817155 astro-delight-0.0.9/notebook/
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)    15503 2023-01-18 02:42:17.000000 astro-delight-0.0.9/notebook/Delight_example_notebook.ipynb
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)       38 2024-02-14 22:44:00.817155 astro-delight-0.0.9/setup.cfg
+-rw-rw-r--   0 fforster  (1000) fforster  (1000)     1680 2024-02-14 22:40:29.000000 astro-delight-0.0.9/setup.py
```

### Comparing `astro-delight-0.0.8/PKG-INFO` & `astro-delight-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: astro-delight
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deep Learning Identification of Galaxy Hosts in Transients, a package to automatically identify host galaxies of transient candidates
 Home-page: https://github.com/fforster/delight
 Author: Francisco Förster
 Author-email: francisco.forster@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
+Requires-Dist: astropy
+Requires-Dist: sep
+Requires-Dist: xarray
+Requires-Dist: panstamps
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: tensorflow
 
 <p float="left">
 <img src="http://alerce.science/static/img/alerce_logo.cc79ccea2406.png" alt="drawing" width="300"/>
 &nbsp; &nbsp; &nbsp;&nbsp;
 <img src="https://raw.githubusercontent.com/fforster/DELIGHT/main/figures/Delight.png" alt="drawing" width="200"/>
 </p>
```

### Comparing `astro-delight-0.0.8/README.md` & `astro-delight-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `astro-delight-0.0.8/astro_delight.egg-info/PKG-INFO` & `astro-delight-0.0.9/astro_delight.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: astro-delight
-Version: 0.0.8
+Version: 0.0.9
 Summary: Deep Learning Identification of Galaxy Hosts in Transients, a package to automatically identify host galaxies of transient candidates
 Home-page: https://github.com/fforster/delight
 Author: Francisco Förster
 Author-email: francisco.forster@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/markdown
+Requires-Dist: astropy
+Requires-Dist: sep
+Requires-Dist: xarray
+Requires-Dist: panstamps
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: tensorflow
 
 <p float="left">
 <img src="http://alerce.science/static/img/alerce_logo.cc79ccea2406.png" alt="drawing" width="300"/>
 &nbsp; &nbsp; &nbsp;&nbsp;
 <img src="https://raw.githubusercontent.com/fforster/DELIGHT/main/figures/Delight.png" alt="drawing" width="200"/>
 </p>
```

### Comparing `astro-delight-0.0.8/delight/delight/DELIGHT_v1.h5` & `astro-delight-0.0.9/delight/delight/DELIGHT_v1.h5`

 * *Files identical despite different names*

### Comparing `astro-delight-0.0.8/delight/delight/delight.py` & `astro-delight-0.0.9/delight/delight/delight.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from astropy.coordinates import SkyCoord
 
 #import fitsio
 import sep
 from astropy.wcs import WCS
 from astropy.io import fits
 
-from mpl_toolkits.axes_grid.inset_locator import inset_axes
+from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 from matplotlib import cm
 
 import tensorflow as tf
 import panstamps # not really used here, but if we cannot import it is likely that it is not installed
 
 class Delight(object):
```

### Comparing `astro-delight-0.0.8/setup.py` & `astro-delight-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages, find_namespace_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='astro-delight',
-    version='0.0.8',    
+    version='0.0.9',    
     description='Deep Learning Identification of Galaxy Hosts in Transients, a package to automatically identify host galaxies of transient candidates',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/fforster/delight',
     author='Francisco Förster',
     author_email='francisco.forster@gmail.com',
     license='GNU GPLv3',
     packages=find_namespace_packages(include=["delight.*"]),
     install_requires=['astropy',
                       'sep',
                       'xarray',
-                      'panstamps==0.6.5',
+                      'panstamps',
                       'matplotlib',
                       'numpy',
                       'tensorflow'
                       ],
     build_requires=['astropy',
                       'sep',
                       'xarray',
```

