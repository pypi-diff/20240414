# Comparing `tmp/tetraframework-0.0.5.tar.gz` & `tmp/tetraframework-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tetraframework-0.0.5.tar", last modified: Mon Jun 13 19:39:48 2022, max compression
+gzip compressed data, was "tetraframework-0.0.6.tar", last modified: Wed Apr 10 09:16:21 2024, max compression
```

## Comparing `tetraframework-0.0.5.tar` & `tetraframework-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,13 @@
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.147059 tetraframework-0.0.5/
--rw-r--r--   0 samwillis   (501) staff       (20)      113 2022-05-24 11:41:31.000000 tetraframework-0.0.5/MANIFEST.in
--rw-r--r--   0 samwillis   (501) staff       (20)     3404 2022-06-13 19:39:48.146681 tetraframework-0.0.5/PKG-INFO
--rw-r--r--   0 samwillis   (501) staff       (20)     2464 2022-05-28 14:19:56.000000 tetraframework-0.0.5/README.md
--rw-r--r--   0 samwillis   (501) staff       (20)       38 2022-06-13 19:39:48.147204 tetraframework-0.0.5/setup.cfg
--rw-r--r--   0 samwillis   (501) staff       (20)      861 2022-06-13 19:38:35.000000 tetraframework-0.0.5/setup.py
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.127704 tetraframework-0.0.5/tetra/
--rw-r--r--   0 samwillis   (501) staff       (20)      182 2022-06-13 19:38:32.000000 tetraframework-0.0.5/tetra/__init__.py
--rw-r--r--   0 samwillis   (501) staff       (20)     1072 2022-06-05 17:39:52.000000 tetraframework-0.0.5/tetra/apps.py
--rw-r--r--   0 samwillis   (501) staff       (20)      426 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/build.py
--rw-r--r--   0 samwillis   (501) staff       (20)     3703 2022-06-02 11:05:47.000000 tetraframework-0.0.5/tetra/component_register.py
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.130293 tetraframework-0.0.5/tetra/components/
--rw-r--r--   0 samwillis   (501) staff       (20)      116 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/components/__init__.py
--rw-r--r--   0 samwillis   (501) staff       (20)    19028 2022-06-03 14:23:32.000000 tetraframework-0.0.5/tetra/components/base.py
--rw-r--r--   0 samwillis   (501) staff       (20)      698 2022-05-29 15:22:05.000000 tetraframework-0.0.5/tetra/components/callbacks.py
--rw-r--r--   0 samwillis   (501) staff       (20)      594 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/default_settings.py
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.131868 tetraframework-0.0.5/tetra/js/
--rw-r--r--   0 samwillis   (501) staff       (20)    10591 2022-05-29 14:47:11.000000 tetraframework-0.0.5/tetra/js/tetra.core.js
--rw-r--r--   0 samwillis   (501) staff       (20)      131 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/js/tetra.js
--rw-r--r--   0 samwillis   (501) staff       (20)     7934 2022-06-05 17:42:53.000000 tetraframework-0.0.5/tetra/library.py
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.132596 tetraframework-0.0.5/tetra/management/
--rw-r--r--   0 samwillis   (501) staff       (20)        0 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/management/__init__.py
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.134037 tetraframework-0.0.5/tetra/management/commands/
--rw-r--r--   0 samwillis   (501) staff       (20)        0 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/management/commands/__init__.py
--rw-r--r--   0 samwillis   (501) staff       (20)      519 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/management/commands/runserver.py
--rw-r--r--   0 samwillis   (501) staff       (20)     1426 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/management/commands/tetrabuild.py
--rw-r--r--   0 samwillis   (501) staff       (20)     2111 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/middleware.py
--rw-r--r--   0 samwillis   (501) staff       (20)     7399 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/state.py
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.134764 tetraframework-0.0.5/tetra/static/
--rw-r--r--   0 samwillis   (501) staff       (20)     6148 2022-06-08 08:38:32.000000 tetraframework-0.0.5/tetra/static/.DS_Store
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.135476 tetraframework-0.0.5/tetra/static/tetra/
--rw-r--r--   0 samwillis   (501) staff       (20)     6148 2022-06-08 08:38:32.000000 tetraframework-0.0.5/tetra/static/tetra/.DS_Store
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.141238 tetraframework-0.0.5/tetra/static/tetra/js/
--rw-r--r--   0 samwillis   (501) staff       (20)     6148 2022-05-06 16:17:47.000000 tetraframework-0.0.5/tetra/static/tetra/js/.DS_Store
--rw-r--r--   0 samwillis   (501) staff       (20)    38458 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/static/tetra/js/alpinejs.cdn.min.js
--rw-r--r--   0 samwillis   (501) staff       (20)     3943 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/static/tetra/js/alpinejs.morph.cdn.min.js
--rw-r--r--   0 samwillis   (501) staff       (20)    11701 2022-05-29 14:37:43.000000 tetraframework-0.0.5/tetra/static/tetra/js/tetra.js
--rw-r--r--   0 samwillis   (501) staff       (20)    17836 2022-05-29 14:37:43.000000 tetraframework-0.0.5/tetra/static/tetra/js/tetra.js.map
--rw-r--r--   0 samwillis   (501) staff       (20)     5402 2022-05-29 14:37:43.000000 tetraframework-0.0.5/tetra/static/tetra/js/tetra.min.js
--rw-r--r--   0 samwillis   (501) staff       (20)    16550 2022-05-29 14:37:43.000000 tetraframework-0.0.5/tetra/static/tetra/js/tetra.min.js.map
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.143762 tetraframework-0.0.5/tetra/templates/
--rw-r--r--   0 samwillis   (501) staff       (20)      509 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/templates/lib_scripts.html
--rw-r--r--   0 samwillis   (501) staff       (20)       88 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/templates/lib_styles.html
--rw-r--r--   0 samwillis   (501) staff       (20)      429 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/templates/script.js
--rw-r--r--   0 samwillis   (501) staff       (20)     2331 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/templates.py
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.144516 tetraframework-0.0.5/tetra/templatetags/
--rw-r--r--   0 samwillis   (501) staff       (20)        0 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/templatetags/__init__.py
--rw-r--r--   0 samwillis   (501) staff       (20)    15195 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/templatetags/tetra.py
--rw-r--r--   0 samwillis   (501) staff       (20)      247 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/urls.py
--rw-r--r--   0 samwillis   (501) staff       (20)     3111 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/utils.py
--rw-r--r--   0 samwillis   (501) staff       (20)     1220 2022-05-24 11:41:30.000000 tetraframework-0.0.5/tetra/views.py
-drwxr-xr-x   0 samwillis   (501) staff       (20)        0 2022-06-13 19:39:48.146247 tetraframework-0.0.5/tetraframework.egg-info/
--rw-r--r--   0 samwillis   (501) staff       (20)     3404 2022-06-13 19:39:48.000000 tetraframework-0.0.5/tetraframework.egg-info/PKG-INFO
--rw-r--r--   0 samwillis   (501) staff       (20)     1170 2022-06-13 19:39:48.000000 tetraframework-0.0.5/tetraframework.egg-info/SOURCES.txt
--rw-r--r--   0 samwillis   (501) staff       (20)        1 2022-06-13 19:39:48.000000 tetraframework-0.0.5/tetraframework.egg-info/dependency_links.txt
--rw-r--r--   0 samwillis   (501) staff       (20)       77 2022-06-13 19:39:48.000000 tetraframework-0.0.5/tetraframework.egg-info/requires.txt
--rw-r--r--   0 samwillis   (501) staff       (20)        6 2022-06-13 19:39:48.000000 tetraframework-0.0.5/tetraframework.egg-info/top_level.txt
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 09:16:21.304427 tetraframework-0.0.6/
+-rw-r--r--   0 christian  (1000) christian  (1000)     1066 2024-03-29 16:17:30.000000 tetraframework-0.0.6/LICENSE
+-rw-r--r--   0 christian  (1000) christian  (1000)        0 2024-04-10 08:58:51.000000 tetraframework-0.0.6/MANIFEST.in
+-rw-r--r--   0 christian  (1000) christian  (1000)     1100 2024-04-10 09:16:21.304427 tetraframework-0.0.6/PKG-INFO
+-rw-r--r--   0 christian  (1000) christian  (1000)      705 2024-04-10 08:58:51.000000 tetraframework-0.0.6/README.md
+-rw-r--r--   0 christian  (1000) christian  (1000)       38 2024-04-10 09:16:21.304427 tetraframework-0.0.6/setup.cfg
+-rw-r--r--   0 christian  (1000) christian  (1000)      615 2024-04-10 09:15:53.000000 tetraframework-0.0.6/setup.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 09:16:21.304427 tetraframework-0.0.6/tetraframework.egg-info/
+-rw-r--r--   0 christian  (1000) christian  (1000)     1100 2024-04-10 09:16:21.000000 tetraframework-0.0.6/tetraframework.egg-info/PKG-INFO
+-rw-r--r--   0 christian  (1000) christian  (1000)      227 2024-04-10 09:16:21.000000 tetraframework-0.0.6/tetraframework.egg-info/SOURCES.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)        1 2024-04-10 09:16:21.000000 tetraframework-0.0.6/tetraframework.egg-info/dependency_links.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)       13 2024-04-10 09:16:21.000000 tetraframework-0.0.6/tetraframework.egg-info/requires.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)        6 2024-04-10 09:16:21.000000 tetraframework-0.0.6/tetraframework.egg-info/top_level.txt
```

### Comparing `tetraframework-0.0.5/setup.py` & `tetraframework-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 import setuptools
-from tetra import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tetraframework",
-    version=__version__,
-    url='https://www.tetraframework.com',
+    version="0.0.6",
+    url="https://www.tetraframework.com",
     author="Sam Willis",
-    description="Full stack component framework for Django using Alpine.js",
+    description="Transition package to 'tetra'",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
-    packages=setuptools.find_packages(exclude='demosite'),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
     install_requires=[
-        'cryptography>=37.0.1',
-        'Django>=3.2.0',
-        'python-dateutil>=2.8.2',
-        'sourcetypes>=0.0.4',
-    ]
+        "tetra>=0.1.0",
+    ],
 )
```

