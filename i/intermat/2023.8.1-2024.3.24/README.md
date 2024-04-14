# Comparing `tmp/intermat-2023.8.1.tar.gz` & `tmp/intermat-2024.3.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intermat-2023.8.1.tar", last modified: Sun Sep 10 13:02:27 2023, max compression
+gzip compressed data, was "intermat-2024.3.24.tar", last modified: Sun Apr 14 16:02:30 2024, max compression
```

## Comparing `intermat-2023.8.1.tar` & `intermat-2024.3.24.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-09-10 13:02:29.468829 intermat-2023.8.1/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1103 2023-09-10 13:00:26.000000 intermat-2023.8.1/LICENSE
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      428 2023-09-10 13:02:29.463903 intermat-2023.8.1/PKG-INFO
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       10 2023-09-10 13:00:26.000000 intermat-2023.8.1/README.md
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-09-10 13:02:29.343486 intermat-2023.8.1/intermat/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        1 2023-09-10 13:00:26.000000 intermat-2023.8.1/intermat/__init__.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     2428 2023-09-10 13:00:26.000000 intermat-2023.8.1/intermat/generate.py
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-09-10 13:02:29.443374 intermat-2023.8.1/intermat.egg-info/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      428 2023-09-10 13:02:28.000000 intermat-2023.8.1/intermat.egg-info/PKG-INFO
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      227 2023-09-10 13:02:29.000000 intermat-2023.8.1/intermat.egg-info/SOURCES.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        1 2023-09-10 13:02:28.000000 intermat-2023.8.1/intermat.egg-info/dependency_links.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       52 2023-09-10 13:02:28.000000 intermat-2023.8.1/intermat.egg-info/requires.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        9 2023-09-10 13:02:28.000000 intermat-2023.8.1/intermat.egg-info/top_level.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       38 2023-09-10 13:02:29.470932 intermat-2023.8.1/setup.cfg
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      766 2023-09-10 13:02:09.000000 intermat-2023.8.1/setup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 16:02:30.813140 intermat-2024.3.24/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1878 2024-04-14 16:01:59.000000 intermat-2024.3.24/LICENSE.rst
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    30435 2024-04-14 16:02:30.813140 intermat-2024.3.24/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    29976 2024-04-14 16:01:59.000000 intermat-2024.3.24/README.md
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 16:02:30.749140 intermat-2024.3.24/intermat/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       50 2024-03-29 20:35:00.000000 intermat-2024.3.24/intermat/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    10110 2024-03-29 21:42:48.000000 intermat-2024.3.24/intermat/alignn_anderson.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11461 2024-04-02 02:52:37.000000 intermat-2024.3.24/intermat/analyze.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    22690 2024-04-13 13:01:36.000000 intermat-2024.3.24/intermat/calculators.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5055 2024-04-13 13:04:56.000000 intermat-2024.3.24/intermat/config.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 16:02:30.777140 intermat-2024.3.24/intermat/data/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2024-03-29 19:58:15.000000 intermat-2024.3.24/intermat/data/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7306 2024-03-29 19:58:15.000000 intermat-2024.3.24/intermat/data/classify.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     9510 2024-03-29 19:58:15.000000 intermat-2024.3.24/intermat/ewald.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    33580 2024-03-31 21:04:59.000000 intermat-2024.3.24/intermat/generate.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11467 2024-03-29 19:58:15.000000 intermat-2024.3.24/intermat/master.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1513 2024-04-02 03:09:53.000000 intermat-2024.3.24/intermat/p.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5692 2024-04-13 18:25:16.000000 intermat-2024.3.24/intermat/run_intermat.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3613 2024-03-29 19:58:15.000000 intermat-2024.3.24/intermat/surf_andersen.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 16:02:30.765140 intermat-2024.3.24/intermat.egg-info/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    30435 2024-04-14 16:02:29.000000 intermat-2024.3.24/intermat.egg-info/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      476 2024-04-14 16:02:30.000000 intermat-2024.3.24/intermat.egg-info/SOURCES.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2024-04-14 16:02:29.000000 intermat-2024.3.24/intermat.egg-info/dependency_links.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       70 2024-04-14 16:02:30.000000 intermat-2024.3.24/intermat.egg-info/requires.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        9 2024-04-14 16:02:30.000000 intermat-2024.3.24/intermat.egg-info/top_level.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2024-04-14 16:02:30.813140 intermat-2024.3.24/setup.cfg
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      873 2024-04-13 13:03:47.000000 intermat-2024.3.24/setup.py
```

### Comparing `intermat-2023.8.1/setup.py` & `intermat-2024.3.24/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="intermat",
-    version="2023.8.1",
+    version="2024.3.24",
     author="Kamal Choudhary",
     author_email="kamal.choudhary@nist.gov",
     description="intermat",
     install_requires=[
         "numpy>=1.22.0",
         "scipy>=1.6.3",
         "jarvis-tools>=2021.07.19",
+        "pydantic_settings",
+        # "alignn",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/usnistgov/intermat",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7",
+    scripts=[
+        "intermat/run_intermat.py",
+    ],
+    python_requires=">=3.8",
 )
```

