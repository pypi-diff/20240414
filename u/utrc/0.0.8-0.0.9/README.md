# Comparing `tmp/utrc-0.0.8.tar.gz` & `tmp/utrc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utrc-0.0.8.tar", last modified: Sun Apr 14 12:24:58 2024, max compression
+gzip compressed data, was "utrc-0.0.9.tar", last modified: Sun Apr 14 12:44:07 2024, max compression
```

## Comparing `utrc-0.0.8.tar` & `utrc-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 12:24:58.363374 utrc-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3903 2024-04-14 12:24:58.363135 utrc-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.8/README.md
--rw-r--r--   0 solst      (501) staff       (20)      937 2024-04-14 12:24:18.000000 utrc-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-14 12:24:58.363417 utrc-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.8/setup.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 12:24:58.361113 utrc-0.0.8/utrc/
--rw-r--r--   0 solst      (501) staff       (20)      980 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    24786 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     3146 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/attr.py
--rw-r--r--   0 solst      (501) staff       (20)     7932 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/bend.py
--rw-r--r--   0 solst      (501) staff       (20)    10268 2024-04-04 17:50:33.000000 utrc-0.0.8/utrc/cols.py
--rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     1285 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/data.py
--rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/diff.py
--rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/dims.py
--rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/init.py
--rw-r--r--   0 solst      (501) staff       (20)    33611 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/kwds.py
--rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/logs.py
--rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/loss.py
--rw-r--r--   0 solst      (501) staff       (20)     9046 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/misc.py
--rw-r--r--   0 solst      (501) staff       (20)    12556 2024-04-04 19:18:05.000000 utrc-0.0.8/utrc/pand.py
--rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-06 14:04:05.000000 utrc-0.0.8/utrc/perc.py
--rw-r--r--   0 solst      (501) staff       (20)     2198 2024-04-06 14:04:05.000000 utrc-0.0.8/utrc/seed.py
--rw-r--r--   0 solst      (501) staff       (20)     6822 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/smpl.py
--rw-r--r--   0 solst      (501) staff       (20)     2449 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/strs.py
--rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/tens.py
--rw-r--r--   0 solst      (501) staff       (20)     5808 2024-04-14 12:24:46.000000 utrc-0.0.8/utrc/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 12:24:58.362105 utrc-0.0.8/utrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3903 2024-04-14 12:24:58.000000 utrc-0.0.8/utrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      541 2024-04-14 12:24:58.000000 utrc-0.0.8/utrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-14 12:24:58.000000 utrc-0.0.8/utrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-14 12:24:58.000000 utrc-0.0.8/utrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.8/utrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      154 2024-04-14 12:24:58.000000 utrc-0.0.8/utrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-14 12:24:58.000000 utrc-0.0.8/utrc.egg-info/top_level.txt
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 12:44:07.171767 utrc-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3923 2024-04-14 12:44:07.171490 utrc-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.9/README.md
+-rw-r--r--   0 solst      (501) staff       (20)      942 2024-04-14 12:43:49.000000 utrc-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-14 12:44:07.171816 utrc-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.9/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 12:44:07.169072 utrc-0.0.9/utrc/
+-rw-r--r--   0 solst      (501) staff       (20)      980 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    24786 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3146 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/attr.py
+-rw-r--r--   0 solst      (501) staff       (20)     7932 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/bend.py
+-rw-r--r--   0 solst      (501) staff       (20)    10268 2024-04-04 17:50:33.000000 utrc-0.0.9/utrc/cols.py
+-rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     1285 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/data.py
+-rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/diff.py
+-rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/dims.py
+-rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/init.py
+-rw-r--r--   0 solst      (501) staff       (20)    33611 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/kwds.py
+-rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/logs.py
+-rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/loss.py
+-rw-r--r--   0 solst      (501) staff       (20)     9046 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/misc.py
+-rw-r--r--   0 solst      (501) staff       (20)    12556 2024-04-04 19:18:05.000000 utrc-0.0.9/utrc/pand.py
+-rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-06 14:04:05.000000 utrc-0.0.9/utrc/perc.py
+-rw-r--r--   0 solst      (501) staff       (20)     2198 2024-04-06 14:04:05.000000 utrc-0.0.9/utrc/seed.py
+-rw-r--r--   0 solst      (501) staff       (20)     6822 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/smpl.py
+-rw-r--r--   0 solst      (501) staff       (20)     2449 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/strs.py
+-rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/tens.py
+-rw-r--r--   0 solst      (501) staff       (20)     5808 2024-04-14 12:43:52.000000 utrc-0.0.9/utrc/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 12:44:07.170256 utrc-0.0.9/utrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3923 2024-04-14 12:44:07.000000 utrc-0.0.9/utrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      541 2024-04-14 12:44:07.000000 utrc-0.0.9/utrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-14 12:44:07.000000 utrc-0.0.9/utrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-14 12:44:07.000000 utrc-0.0.9/utrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.9/utrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      159 2024-04-14 12:44:07.000000 utrc-0.0.9/utrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-14 12:44:07.000000 utrc-0.0.9/utrc.egg-info/top_level.txt
```

### Comparing `utrc-0.0.8/LICENSE` & `utrc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/PKG-INFO` & `utrc-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.8
+Version: 0.0.9
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
@@ -25,14 +25,15 @@
 Requires-Dist: lmsg
 Requires-Dist: lull
 Requires-Dist: nchr
 Requires-Dist: nlit
 Requires-Dist: pcts
 Requires-Dist: quac
 Requires-Dist: seeder
+Requires-Dist: sigr
 Requires-Dist: slcs
 Requires-Dist: uscr
 Requires-Dist: zipr
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
```

### Comparing `utrc-0.0.8/README.md` & `utrc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/settings.ini` & `utrc-0.0.9/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utrc
 lib_name = utrc
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = utrc
 nbs_path = nbs
 recursive = True
@@ -29,10 +29,10 @@
 conda_user = dsm-72
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
-requirements = asto astr atup chck dref dtyp etrc lmsg lull nchr nlit pcts quac seeder slcs uscr zipr
+requirements = asto astr atup chck dref dtyp etrc lmsg lull nchr nlit pcts quac seeder sigr slcs uscr zipr
 dev_requirements = numpy pandas matplotlib torch pytorch_lightning torchvision
```

### Comparing `utrc-0.0.8/setup.py` & `utrc-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/__init__.py` & `utrc-0.0.9/utrc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `utrc-0.0.8/utrc/_modidx.py` & `utrc-0.0.9/utrc/_modidx.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/attr.py` & `utrc-0.0.9/utrc/attr.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/atyp.py` & `utrc-0.0.9/utrc/atyp.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/bend.py` & `utrc-0.0.9/utrc/bend.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/cols.py` & `utrc-0.0.9/utrc/cols.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/cons.py` & `utrc-0.0.9/utrc/cons.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/data.py` & `utrc-0.0.9/utrc/data.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/diff.py` & `utrc-0.0.9/utrc/diff.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/dims.py` & `utrc-0.0.9/utrc/dims.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/init.py` & `utrc-0.0.9/utrc/init.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/kwds.py` & `utrc-0.0.9/utrc/kwds.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/logs.py` & `utrc-0.0.9/utrc/logs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/loss.py` & `utrc-0.0.9/utrc/loss.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/misc.py` & `utrc-0.0.9/utrc/misc.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/pand.py` & `utrc-0.0.9/utrc/pand.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/perc.py` & `utrc-0.0.9/utrc/perc.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/seed.py` & `utrc-0.0.9/utrc/seed.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/smpl.py` & `utrc-0.0.9/utrc/smpl.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/strs.py` & `utrc-0.0.9/utrc/strs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/tens.py` & `utrc-0.0.9/utrc/tens.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc/util.py` & `utrc-0.0.9/utrc/util.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.8/utrc.egg-info/PKG-INFO` & `utrc-0.0.9/utrc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.8
+Version: 0.0.9
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
@@ -25,14 +25,15 @@
 Requires-Dist: lmsg
 Requires-Dist: lull
 Requires-Dist: nchr
 Requires-Dist: nlit
 Requires-Dist: pcts
 Requires-Dist: quac
 Requires-Dist: seeder
+Requires-Dist: sigr
 Requires-Dist: slcs
 Requires-Dist: uscr
 Requires-Dist: zipr
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
```

### Comparing `utrc-0.0.8/utrc.egg-info/SOURCES.txt` & `utrc-0.0.9/utrc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

