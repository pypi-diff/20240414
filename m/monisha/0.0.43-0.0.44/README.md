# Comparing `tmp/monisha-0.0.43.tar.gz` & `tmp/monisha-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.43.tar", last modified: Sun Apr 14 03:03:48 2024, max compression
+gzip compressed data, was "monisha-0.0.44.tar", last modified: Sun Apr 14 05:24:30 2024, max compression
```

## Comparing `monisha-0.0.43.tar` & `monisha-0.0.44.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:03:48.490599 monisha-0.0.43/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-14 03:03:39.000000 monisha-0.0.43/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:03:48.482599 monisha-0.0.43/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:03:48.486599 monisha-0.0.43/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/functions/function14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:03:48.486599 monisha-0.0.43/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-14 03:03:39.000000 monisha-0.0.43/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-14 03:03:48.490599 monisha-0.0.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-14 03:03:39.000000 monisha-0.0.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:03:48.486599 monisha-0.0.43/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-14 03:03:48.000000 monisha-0.0.43/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 03:03:48.000000 monisha-0.0.43/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 03:03:48.000000 monisha-0.0.43/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 03:03:48.000000 monisha-0.0.43/monisha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 03:03:48.000000 monisha-0.0.43/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 03:03:48.490599 monisha-0.0.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-14 03:03:39.000000 monisha-0.0.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:30.000549 monisha-0.0.44/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-14 05:24:25.000000 monisha-0.0.44/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:29.992549 monisha-0.0.44/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:29.996549 monisha-0.0.44/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:29.996549 monisha-0.0.44/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-14 05:24:29.996549 monisha-0.0.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-14 05:24:25.000000 monisha-0.0.44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:29.996549 monisha-0.0.44/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:24:30.000549 monisha-0.0.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-14 05:24:25.000000 monisha-0.0.44/setup.py
```

### Comparing `monisha-0.0.43/LICENSE` & `monisha-0.0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/__init__.py` & `monisha-0.0.44/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/function01.py` & `monisha-0.0.44/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/function02.py` & `monisha-0.0.44/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/function03.py` & `monisha-0.0.44/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/function04.py` & `monisha-0.0.44/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/function06.py` & `monisha-0.0.44/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/function07.py` & `monisha-0.0.44/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/function10.py` & `monisha-0.0.44/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/Monisha/functions/function14.py` & `monisha-0.0.44/Monisha/functions/function14.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 from ..scripts.en import Scripted
 #===========================================================================
 
 async def CDirectory(dname=Folder.DATA07, fname=Scripted.DATA01):
     name01 = str(dname)
     name02 = str(fname)
     osemse = os.getcwd()
-    moonse = os.path.join(osemse, name01, name02)
+    moonse = os.path.join(osemse, name01) + name02
     moonse if os.path.isdir(moonse) else os.makedirs(moonse)
     return moonse
 
 #===========================================================================
 
 async def UDirectory(dname=Folder.DATA07, fname=Scripted.DATA01):
     name01 = str(dname)
     name02 = str(fname)
     osemse = os.getcwd()
     timeso = str(round(time.time()))
-    moonse = os.path.join(osemse, name01, timeso, name02)
+    moonse = os.path.join(osemse, name01, timeso) + name02
     moonse if os.path.isdir(moonse) else os.makedirs(moonse)
     return moonse
 
 #===========================================================================
 
 async def BDirectory(uid, dname=Folder.DATA07, fname=Scripted.DATA01):
     usered = str(uid)
     name01 = str(dname)
     name02 = str(fname)
     osemse = os.getcwd()
     timeso = str(round(time.time()))
-    moonse = os.path.join(osemse, name01, usered, timeso, name02)
+    moonse = os.path.join(osemse, name01, usered, timeso) + name02
     moonse if os.path.isdir(moonse) else os.makedirs(moonse)
     return moonse
 
 #===========================================================================
```

### Comparing `monisha-0.0.43/Monisha/scripts/es.py` & `monisha-0.0.44/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/PKG-INFO` & `monisha-0.0.44/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.43
-Summary: python helper modules
+Version: 0.0.44
+Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: ~=3.8
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.43 Summary: python helper
-modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
-Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
-python,clinton,abraham Classifier: Natural Language :: English Classifier:
-Intended Audience :: Developers Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: License :: OSI Approved :: GNU Lesser General
-Public License v3 (LGPLv3) Requires-Python: ~=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: monisha Version: 0.0.44 Summary: ã¤ Home-page:
+https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
+clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
+Classifier: Natural Language :: English Classifier: Intended Audience ::
+Developers Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Software Development ::
+Libraries Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: License :: OSI Approved :: GNU Lesser General Public
+License v3 (LGPLv3) Requires-Python: ~=3.10 Description-Content-Type: text/
+markdown License-File: LICENSE
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.43/monisha.egg-info/PKG-INFO` & `monisha-0.0.44/monisha.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.43
-Summary: python helper modules
+Version: 0.0.44
+Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: ~=3.8
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
  📦 <a href="https://pypi.org/project/monisha" style="text-decoration:none;">MONISHA</a>
 </p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.43 Summary: python helper
-modules Home-page: https://github.com/Clinton-Abraham Author: Clinton-Abraham
-Author-email: clintonabrahamc@gmail.com License: MIT Keywords:
-python,clinton,abraham Classifier: Natural Language :: English Classifier:
-Intended Audience :: Developers Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: License :: OSI Approved :: GNU Lesser General
-Public License v3 (LGPLv3) Requires-Python: ~=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: monisha Version: 0.0.44 Summary: ã¤ Home-page:
+https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
+clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
+Classifier: Natural Language :: English Classifier: Intended Audience ::
+Developers Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Software Development ::
+Libraries Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: License :: OSI Approved :: GNU Lesser General Public
+License v3 (LGPLv3) Requires-Python: ~=3.10 Description-Content-Type: text/
+markdown License-File: LICENSE
                                  ð¦ _M_O_N_I_S_H_A
```

### Comparing `monisha-0.0.43/monisha.egg-info/SOURCES.txt` & `monisha-0.0.44/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.43/setup.py` & `monisha-0.0.44/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,18 @@
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)']
 
 setup(
     name='monisha',
     license='MIT',
     zip_safe=False,
-    version='0.0.43',
+    description='ㅤ',
+    version='0.0.44',
     classifiers=DATA02,
     author_email=DATA01,
-    python_requires='~=3.8',
+    python_requires='~=3.10',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
-    description='python helper modules',
     url='https://github.com/Clinton-Abraham',
     keywords=['python', 'clinton', 'abraham'],
     long_description_content_type="text/markdown")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

