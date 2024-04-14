# Comparing `tmp/pastream-0.2.0.post0.tar.gz` & `tmp/pastream-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pastream-0.2.0.post0.tar", last modified: Sat Jun  9 22:25:54 2018, max compression
+gzip compressed data, was "pastream-0.2.0.post1.tar", last modified: Sun Apr 14 18:39:36 2024, max compression
```

## Comparing `pastream-0.2.0.post0.tar` & `pastream-0.2.0.post1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/fake_sounddevice.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1012 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     8522 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      308 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/fake_cffi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     7812 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/fake_soundfile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/fake_pastream.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6814 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7883 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1566 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/dev-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)      127 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/examples/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/examples/plot_stft.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/examples/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1408 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/examples/plot_rec.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/etc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/etc/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/etc/plot_filepolling.m
--rw-rw-r--   0 travis    (2000) travis    (2000)     1059 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/setup-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/portaudio/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/portaudio/include/
--rw-rw-r--   0 travis    (2000) travis    (2000)    47638 2018-06-09 22:23:10.000000 pastream-0.2.0.post0/portaudio/include/portaudio.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/portaudio/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/portaudio/src/common/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9403 2018-06-09 22:23:10.000000 pastream-0.2.0.post0/portaudio/src/common/pa_ringbuffer.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     5977 2018-06-09 22:23:10.000000 pastream-0.2.0.post0/portaudio/src/common/pa_memorybarrier.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8848 2018-06-09 22:23:10.000000 pastream-0.2.0.post0/portaudio/src/common/pa_ringbuffer.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/tests/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    16875 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/tests/test_pastream.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7240 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      614 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    10410 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      887 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/build_pastream.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    69703 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/src/pastream.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2320 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/src/py_pastream.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/pastream.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/pastream.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/pastream.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/pastream.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    10410 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/pastream.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/pastream.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/pastream.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2018-06-09 22:25:54.000000 pastream-0.2.0.post0/src/pastream.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    10194 2018-06-09 22:23:07.000000 pastream-0.2.0.post0/src/py_pastream.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.027265 pastream-0.2.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-14 18:39:36.027265 pastream-0.2.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/build_pastream.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.023265 pastream-0.2.0.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/fake_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/fake_pastream.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/fake_sounddevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/fake_soundfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.023265 pastream-0.2.0.post1/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/etc/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/etc/plot_filepolling.m
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.027265 pastream-0.2.0.post1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/examples/plot_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/examples/plot_stft.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/examples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.023265 pastream-0.2.0.post1/portaudio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.027265 pastream-0.2.0.post1/portaudio/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    47638 2024-04-14 18:39:28.000000 pastream-0.2.0.post1/portaudio/include/portaudio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.023265 pastream-0.2.0.post1/portaudio/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.027265 pastream-0.2.0.post1/portaudio/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-14 18:39:28.000000 pastream-0.2.0.post1/portaudio/src/common/pa_memorybarrier.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-14 18:39:28.000000 pastream-0.2.0.post1/portaudio/src/common/pa_ringbuffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-14 18:39:28.000000 pastream-0.2.0.post1/portaudio/src/common/pa_ringbuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/setup-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 18:39:36.031265 pastream-0.2.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.027265 pastream-0.2.0.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.027265 pastream-0.2.0.post1/src/pastream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-04-14 18:39:36.000000 pastream-0.2.0.post1/src/pastream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-14 18:39:36.000000 pastream-0.2.0.post1/src/pastream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:39:36.000000 pastream-0.2.0.post1/src/pastream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-14 18:39:36.000000 pastream-0.2.0.post1/src/pastream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:39:36.000000 pastream-0.2.0.post1/src/pastream.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-14 18:39:36.000000 pastream-0.2.0.post1/src/pastream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 18:39:36.000000 pastream-0.2.0.post1/src/pastream.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    69703 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/src/pastream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/src/py_pastream.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/src/py_pastream.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:39:36.027265 pastream-0.2.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16875 2024-04-14 18:39:26.000000 pastream-0.2.0.post1/tests/test_pastream.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pastream-0.2.0.post0/docs/index.rst` & `pastream-0.2.0.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/docs/Makefile` & `pastream-0.2.0.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/docs/make.bat` & `pastream-0.2.0.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/docs/conf.py` & `pastream-0.2.0.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/README.rst` & `pastream-0.2.0.post1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 .. image:: https://badge.fury.io/py/pastream.svg
     :target: https://badge.fury.io/py/pastream
 
-.. image:: https://travis-ci.org/tgarc/pastream.svg?branch=master
-    :target: https://travis-ci.org/tgarc/pastream
-
-.. image:: https://ci.appveyor.com/api/projects/status/wk52r5jy9ri7dsi9/branch/master?svg=true
-    :target: https://ci.appveyor.com/project/tgarc/pastream/branch/master
-
 
 GIL-less Portaudio Streams for Python
 =====================================
 `pastream` builds on top of `portaudio <http://www.portaudio.com/>`__ and the
 excellent `sounddevice <http://github.com/spatialaudio/python-sounddevice>`__
 python bindings to provide some more advanced functionality right out of the
 box. Note that in addition to the pastream *library*, pastream includes a
```

### Comparing `pastream-0.2.0.post0/setup.py` & `pastream-0.2.0.post1/setup.py`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/examples/plot_stft.py` & `pastream-0.2.0.post1/examples/plot_stft.py`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/examples/plot_rec.py` & `pastream-0.2.0.post1/examples/plot_rec.py`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/etc/plot_filepolling.m` & `pastream-0.2.0.post1/etc/plot_filepolling.m`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/LICENSE` & `pastream-0.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/portaudio/include/portaudio.h` & `pastream-0.2.0.post1/portaudio/include/portaudio.h`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/portaudio/src/common/pa_ringbuffer.c` & `pastream-0.2.0.post1/portaudio/src/common/pa_ringbuffer.c`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/portaudio/src/common/pa_memorybarrier.h` & `pastream-0.2.0.post1/portaudio/src/common/pa_memorybarrier.h`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/portaudio/src/common/pa_ringbuffer.h` & `pastream-0.2.0.post1/portaudio/src/common/pa_ringbuffer.h`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/tests/test_pastream.py` & `pastream-0.2.0.post1/tests/test_pastream.py`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/CHANGELOG.rst` & `pastream-0.2.0.post1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/MANIFEST.in` & `pastream-0.2.0.post1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/PKG-INFO` & `pastream-0.2.0.post1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,263 +1,263 @@
 Metadata-Version: 2.1
 Name: pastream
-Version: 0.2.0.post0
+Version: 0.2.0.post1
 Summary: GIL-less Portaudio Streams for Python
 Home-page: http://github.com/tgarc/pastream
 Author: Thomas J. Garcia
 Author-email: toemossgarcia@gmail.com
 License: MIT
-Description: .. image:: https://badge.fury.io/py/pastream.svg
-            :target: https://badge.fury.io/py/pastream
-        
-        .. image:: https://travis-ci.org/tgarc/pastream.svg?branch=master
-            :target: https://travis-ci.org/tgarc/pastream
-        
-        .. image:: https://ci.appveyor.com/api/projects/status/wk52r5jy9ri7dsi9/branch/master?svg=true
-            :target: https://ci.appveyor.com/project/tgarc/pastream/branch/master
-        
-        
-        GIL-less Portaudio Streams for Python
-        =====================================
-        `pastream` builds on top of `portaudio <http://www.portaudio.com/>`__ and the
-        excellent `sounddevice <http://github.com/spatialaudio/python-sounddevice>`__
-        python bindings to provide some more advanced functionality right out of the
-        box. Note that in addition to the pastream *library*, pastream includes a
-        `command line application`_ for playing
-        and recording audio files.
-        
-        Documentation:
-           http://pastream.readthedocs.io/
-        
-        Source code repository and issue tracker:
-           http://github.com/tgarc/pastream/
-        
-        
-        Features
-        ========
-        GIL-less Audio Callbacks
-            Having the portaudio callback implemented in C means audio interrupts can
-            be serviced quickly and reliably without ever needing to acquire the Python
-            Global Interpreter Lock (GIL). This is crucial when working with libraries
-            like `Pillow <https://python-pillow.org/>`__ which may greedily grab and
-            hold the GIL subsequently causing audio overruns/underruns.
-        
-        Input Stream iterators
-            Efficiently retrieve live audio capture data through an iterable. As simple as:
-        
-            .. code-block:: python
-        
-               import pastream as ps
-               for chunk in ps.chunks():
-                   process(chunk)
-        
-            See ``pastream.chunks`` and ``pastream.InputStream.chunks`` method.
-        
-        Built-in support for working with SoundFiles and numpy ndarrays
-            Seamless support for playback/recording of numpy ndarrays, generic buffer
-            types, and SoundFiles.
-        
-        Reader/Writer Threads
-            pastream simplifies the process of implementing stream reader and writer
-            threads to manipulate and/or generate data in the background while leaving
-            the main thread free for higher level management tasks.
-        
-        
-        External Dependencies
-        =====================
-        
-        There are a few compiled libraries pastream requires which *may* need to be
-        installed separately depending on your operating system. Windows users are
-        luckiest, they can skip this section entirely.
-        
-        `libffi <https://sourceware.org/libffi/>`__ (Linux/Unix/MacOSX):
-           Under Linux/Unix/MacOSX platforms you'll need to install the ffi
-           library. (For Windows users, ffi is already included with the python cffi
-           package.)  libffi is available through most package managers::
-        
-             $ yum install libffi-devel # Red-hat/CentOS Linux
-             $ apt-get install libffi-dev # Ubuntu/debian derivatives
-             $ brew install libffi # Homebrew on OSX
-        
-           More information on installing ``libffi`` is available in the cffi
-           documentation `here
-           <https://cffi.readthedocs.io/en/latest/installation.html#platform-specific-instructions>`__.
-        
-        `PortAudio <http://www.portaudio.com>`__ and `libsndfile <http://www.mega-nerd.com/libsndfile/>`__ (Linux/Unix):
-           Linux and Unix users will also need to install a recent version of the
-           ``PortAudio`` and ``libsndfile`` libraries. (For Windows and OSX, the
-           sounddevice and soundfile python packages include prebuilt versions for
-           you.) You can either install the latest available from your package manager
-           (e.g. ``apt-get install libportaudio2 libsndfile`` for debian/raspbian) or
-           install the latest stable build from the package website (Recommended).
-        
-        
-        Installation
-        ============
-        Once the above dependencies have been resolved, you can install pastream using
-        pip::
-        
-            $ pip install pastream
-        
-        
-        Building From Source
-        =====================
-        Clone pastream with the ``--recursive`` flag::
-        
-            $ git clone --recursive http://github.com/tgarc/pastream
-        
-        Or, if you already have a checkout::
-        
-            $ cd <path/to/checkout>
-            $ git submodule update --init
-        
-        Finally, do a pip install from your local working copy::
-        
-            $ pip install <path/to/checkout>
-        
-        
-        Building Documentation
-        ======================
-        Documentation for pastream can be easily generated in a wide variety of formats
-        using Sphinx. Just follow the steps below. 
-        
-        Checkout the repository and cd into it::
-        
-            $ git clone http://github.com/tgarc/pastream
-            $ cd pastream
-        
-        Install documentation dependencies using requirements file::
-        
-            $ pip install -r docs/requirements.txt
-        
-        Then use the included Makefile/make.bat to generate documentation. (Here we
-        output to the html format)::
-        
-            $ cd docs
-            $ make html
-        
-        
-        Examples
-        ========
-        Record one second of audio to memory, then play it back:
-        
-        .. code-block:: python
-        
-           import pastream as ps
-        
-           # Use *with* statements to auto-close the stream
-           with ps.DuplexStream() as stream:
-               out = stream.record(int(stream.samplerate), blocking=True)
-               stream.play(out, blocking=True)
-        
-        Playback 10 seconds of a file, adding zero padding if the file is shorter, and
-        record the result to memory:
-        
-        .. code-block:: python
-        
-           import pastream as ps, soundfile as sf
-        
-           with sf.SoundFile('my-file.wav') as infile, ps.DuplexStream.from_file(infile) as stream:
-               out = stream.playrec(infile, frames=10 * int(stream.samplerate), pad=-1, blocking=True)
-        
-        Grab (real) frequency transformed live audio stream with 50% overlap:
-        
-        .. code-block:: python
-        
-           import pastream as ps, numpy as np
-        
-           chunksize = 1024
-           window = np.hanning(chunksize)
-           for x_l in ps.chunks(chunksize, overlap=chunksize//2, channels=1):
-               X_l = np.fft.rfft(x_l * window)
-        
-        Generate a pure tone on-the-fly
-        
-        .. code-block:: python
-        
-           import time
-           import pastream as ps
-           import numpy as np
-        
-           # A simple tone generator
-           def tone_generator(stream, buffer, f, loop=False):
-               fs = stream.samplerate
-        
-               # Create a time index
-               t = 2*np.pi*f*np.arange(len(buffer), dtype=stream.dtype) / fs
-        
-               # Loop until the stream stops
-               while not stream.finished:
-                   frames = buffer.write_available
-                   if not frames:
-                       time.sleep(0.010)
-                       continue
-        
-                   # Get the write buffers directly to avoid making any extra copies
-                   frames, part1, part2 = buffer.get_write_buffers(frames)
-        
-                   out = np.frombuffer(part1, dtype=stream.dtype)
-                   np.sin(t[:len(out)], out=out)
-        
-                   if len(part2):
-                       # part2 will be nonempty whenever we wrap around the end of the ring buffer
-                       out = np.frombuffer(part2, dtype=stream.dtype)
-                       np.sin(t[:len(out)], out=out)
-        
-                   # flag that we've added data to the buffer
-                   buffer.advance_write_index(frames)
-        
-                   # advance the time index
-                   t += 2*np.pi*f*frames / fs
-        
-           with ps.OutputStream(channels=1) as stream:
-               # Set our tone generator as the source and pass along the frequency
-               freq = 1000
-               stream.set_source(tone_generator, args=(freq,))
-        
-               # Busy-wait to allow for keyboard interrupt
-               stream.start()
-               while stream.active:
-                   time.sleep(0.1)
-        
-        See also the included examples under `/examples`.
-        
-        
-        Command Line Application
-        ========================
-        Once installed, the pastream application should be callable from your command
-        line. If you're familiar with `SoX <http://sox.sourceforge.net/>`__ you'll
-        notice that some of the command line syntax is quite similar. Here are a few
-        examples to help get you started.
-        
-        Display the help file::
-        
-            $ pastream -h
-        
-        List available audio devices::
-        
-            $ pastream -l
-        
-        Simultaneous play and record from the default audio device::
-        
-            $ pastream input.wav output.wav
-        
-        Pipe input from sox using the AU format and record the playback::
-        
-            $ sox -n -t au - synth sine 440 | pastream - output.wav
-        
-        Play a RAW file::
-        
-            $ pastream -c1 -r48k -e=pcm_16 output.raw
-        
-        Record 10 minutes of audio at 48kHz::
-        
-            $ pastream null output.wav -r48k -d10:00
-        
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
+License-File: LICENSE
+Requires-Dist: pa_ringbuffer>=0.1.2
+Requires-Dist: cffi>=1.0.0
+Requires-Dist: soundfile>=0.9.0
+Requires-Dist: sounddevice>=0.3.9
 Provides-Extra: numpy
+Requires-Dist: numpy; extra == "numpy"
+
+.. image:: https://badge.fury.io/py/pastream.svg
+    :target: https://badge.fury.io/py/pastream
+
+
+GIL-less Portaudio Streams for Python
+=====================================
+`pastream` builds on top of `portaudio <http://www.portaudio.com/>`__ and the
+excellent `sounddevice <http://github.com/spatialaudio/python-sounddevice>`__
+python bindings to provide some more advanced functionality right out of the
+box. Note that in addition to the pastream *library*, pastream includes a
+`command line application`_ for playing
+and recording audio files.
+
+Documentation:
+   http://pastream.readthedocs.io/
+
+Source code repository and issue tracker:
+   http://github.com/tgarc/pastream/
+
+
+Features
+========
+GIL-less Audio Callbacks
+    Having the portaudio callback implemented in C means audio interrupts can
+    be serviced quickly and reliably without ever needing to acquire the Python
+    Global Interpreter Lock (GIL). This is crucial when working with libraries
+    like `Pillow <https://python-pillow.org/>`__ which may greedily grab and
+    hold the GIL subsequently causing audio overruns/underruns.
+
+Input Stream iterators
+    Efficiently retrieve live audio capture data through an iterable. As simple as:
+
+    .. code-block:: python
+
+       import pastream as ps
+       for chunk in ps.chunks():
+           process(chunk)
+
+    See ``pastream.chunks`` and ``pastream.InputStream.chunks`` method.
+
+Built-in support for working with SoundFiles and numpy ndarrays
+    Seamless support for playback/recording of numpy ndarrays, generic buffer
+    types, and SoundFiles.
+
+Reader/Writer Threads
+    pastream simplifies the process of implementing stream reader and writer
+    threads to manipulate and/or generate data in the background while leaving
+    the main thread free for higher level management tasks.
+
+
+External Dependencies
+=====================
+
+There are a few compiled libraries pastream requires which *may* need to be
+installed separately depending on your operating system. Windows users are
+luckiest, they can skip this section entirely.
+
+`libffi <https://sourceware.org/libffi/>`__ (Linux/Unix/MacOSX):
+   Under Linux/Unix/MacOSX platforms you'll need to install the ffi
+   library. (For Windows users, ffi is already included with the python cffi
+   package.)  libffi is available through most package managers::
+
+     $ yum install libffi-devel # Red-hat/CentOS Linux
+     $ apt-get install libffi-dev # Ubuntu/debian derivatives
+     $ brew install libffi # Homebrew on OSX
+
+   More information on installing ``libffi`` is available in the cffi
+   documentation `here
+   <https://cffi.readthedocs.io/en/latest/installation.html#platform-specific-instructions>`__.
+
+`PortAudio <http://www.portaudio.com>`__ and `libsndfile <http://www.mega-nerd.com/libsndfile/>`__ (Linux/Unix):
+   Linux and Unix users will also need to install a recent version of the
+   ``PortAudio`` and ``libsndfile`` libraries. (For Windows and OSX, the
+   sounddevice and soundfile python packages include prebuilt versions for
+   you.) You can either install the latest available from your package manager
+   (e.g. ``apt-get install libportaudio2 libsndfile`` for debian/raspbian) or
+   install the latest stable build from the package website (Recommended).
+
+
+Installation
+============
+Once the above dependencies have been resolved, you can install pastream using
+pip::
+
+    $ pip install pastream
+
+
+Building From Source
+=====================
+Clone pastream with the ``--recursive`` flag::
+
+    $ git clone --recursive http://github.com/tgarc/pastream
+
+Or, if you already have a checkout::
+
+    $ cd <path/to/checkout>
+    $ git submodule update --init
+
+Finally, do a pip install from your local working copy::
+
+    $ pip install <path/to/checkout>
+
+
+Building Documentation
+======================
+Documentation for pastream can be easily generated in a wide variety of formats
+using Sphinx. Just follow the steps below. 
+
+Checkout the repository and cd into it::
+
+    $ git clone http://github.com/tgarc/pastream
+    $ cd pastream
+
+Install documentation dependencies using requirements file::
+
+    $ pip install -r docs/requirements.txt
+
+Then use the included Makefile/make.bat to generate documentation. (Here we
+output to the html format)::
+
+    $ cd docs
+    $ make html
+
+
+Examples
+========
+Record one second of audio to memory, then play it back:
+
+.. code-block:: python
+
+   import pastream as ps
+
+   # Use *with* statements to auto-close the stream
+   with ps.DuplexStream() as stream:
+       out = stream.record(int(stream.samplerate), blocking=True)
+       stream.play(out, blocking=True)
+
+Playback 10 seconds of a file, adding zero padding if the file is shorter, and
+record the result to memory:
+
+.. code-block:: python
+
+   import pastream as ps, soundfile as sf
+
+   with sf.SoundFile('my-file.wav') as infile, ps.DuplexStream.from_file(infile) as stream:
+       out = stream.playrec(infile, frames=10 * int(stream.samplerate), pad=-1, blocking=True)
+
+Grab (real) frequency transformed live audio stream with 50% overlap:
+
+.. code-block:: python
+
+   import pastream as ps, numpy as np
+
+   chunksize = 1024
+   window = np.hanning(chunksize)
+   for x_l in ps.chunks(chunksize, overlap=chunksize//2, channels=1):
+       X_l = np.fft.rfft(x_l * window)
+
+Generate a pure tone on-the-fly
+
+.. code-block:: python
+
+   import time
+   import pastream as ps
+   import numpy as np
+
+   # A simple tone generator
+   def tone_generator(stream, buffer, f, loop=False):
+       fs = stream.samplerate
+
+       # Create a time index
+       t = 2*np.pi*f*np.arange(len(buffer), dtype=stream.dtype) / fs
+
+       # Loop until the stream stops
+       while not stream.finished:
+           frames = buffer.write_available
+           if not frames:
+               time.sleep(0.010)
+               continue
+
+           # Get the write buffers directly to avoid making any extra copies
+           frames, part1, part2 = buffer.get_write_buffers(frames)
+
+           out = np.frombuffer(part1, dtype=stream.dtype)
+           np.sin(t[:len(out)], out=out)
+
+           if len(part2):
+               # part2 will be nonempty whenever we wrap around the end of the ring buffer
+               out = np.frombuffer(part2, dtype=stream.dtype)
+               np.sin(t[:len(out)], out=out)
+
+           # flag that we've added data to the buffer
+           buffer.advance_write_index(frames)
+
+           # advance the time index
+           t += 2*np.pi*f*frames / fs
+
+   with ps.OutputStream(channels=1) as stream:
+       # Set our tone generator as the source and pass along the frequency
+       freq = 1000
+       stream.set_source(tone_generator, args=(freq,))
+
+       # Busy-wait to allow for keyboard interrupt
+       stream.start()
+       while stream.active:
+           time.sleep(0.1)
+
+See also the included examples under `/examples`.
+
+
+Command Line Application
+========================
+Once installed, the pastream application should be callable from your command
+line. If you're familiar with `SoX <http://sox.sourceforge.net/>`__ you'll
+notice that some of the command line syntax is quite similar. Here are a few
+examples to help get you started.
+
+Display the help file::
+
+    $ pastream -h
+
+List available audio devices::
+
+    $ pastream -l
+
+Simultaneous play and record from the default audio device::
+
+    $ pastream input.wav output.wav
+
+Pipe input from sox using the AU format and record the playback::
+
+    $ sox -n -t au - synth sine 440 | pastream - output.wav
+
+Play a RAW file::
+
+    $ pastream -c1 -r48k -e=pcm_16 output.raw
+
+Record 10 minutes of audio at 48kHz::
+
+    $ pastream null output.wav -r48k -d10:00
```

### Comparing `pastream-0.2.0.post0/build_pastream.py` & `pastream-0.2.0.post1/build_pastream.py`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/src/pastream.py` & `pastream-0.2.0.post1/src/pastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from pa_ringbuffer import _RingBufferBase
 
 
 # For debugging
 ## from timeit import default_timer as timer
 ## gtime = None
 
-__version__ = '0.2.0.post0'
+__version__ = '0.2.0.post1'
 
 
 # Set a default size for the audio callback ring buffer
 _PA_BUFFERSIZE = 1 << 16
 
 # Determines the blocksize for reading/writing sound files
 _FILECHUNKSIZE = 4096
```

### Comparing `pastream-0.2.0.post0/src/py_pastream.h` & `pastream-0.2.0.post1/src/py_pastream.h`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/src/pastream.egg-info/PKG-INFO` & `pastream-0.2.0.post1/src/pastream.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,263 +1,263 @@
 Metadata-Version: 2.1
 Name: pastream
-Version: 0.2.0.post0
+Version: 0.2.0.post1
 Summary: GIL-less Portaudio Streams for Python
 Home-page: http://github.com/tgarc/pastream
 Author: Thomas J. Garcia
 Author-email: toemossgarcia@gmail.com
 License: MIT
-Description: .. image:: https://badge.fury.io/py/pastream.svg
-            :target: https://badge.fury.io/py/pastream
-        
-        .. image:: https://travis-ci.org/tgarc/pastream.svg?branch=master
-            :target: https://travis-ci.org/tgarc/pastream
-        
-        .. image:: https://ci.appveyor.com/api/projects/status/wk52r5jy9ri7dsi9/branch/master?svg=true
-            :target: https://ci.appveyor.com/project/tgarc/pastream/branch/master
-        
-        
-        GIL-less Portaudio Streams for Python
-        =====================================
-        `pastream` builds on top of `portaudio <http://www.portaudio.com/>`__ and the
-        excellent `sounddevice <http://github.com/spatialaudio/python-sounddevice>`__
-        python bindings to provide some more advanced functionality right out of the
-        box. Note that in addition to the pastream *library*, pastream includes a
-        `command line application`_ for playing
-        and recording audio files.
-        
-        Documentation:
-           http://pastream.readthedocs.io/
-        
-        Source code repository and issue tracker:
-           http://github.com/tgarc/pastream/
-        
-        
-        Features
-        ========
-        GIL-less Audio Callbacks
-            Having the portaudio callback implemented in C means audio interrupts can
-            be serviced quickly and reliably without ever needing to acquire the Python
-            Global Interpreter Lock (GIL). This is crucial when working with libraries
-            like `Pillow <https://python-pillow.org/>`__ which may greedily grab and
-            hold the GIL subsequently causing audio overruns/underruns.
-        
-        Input Stream iterators
-            Efficiently retrieve live audio capture data through an iterable. As simple as:
-        
-            .. code-block:: python
-        
-               import pastream as ps
-               for chunk in ps.chunks():
-                   process(chunk)
-        
-            See ``pastream.chunks`` and ``pastream.InputStream.chunks`` method.
-        
-        Built-in support for working with SoundFiles and numpy ndarrays
-            Seamless support for playback/recording of numpy ndarrays, generic buffer
-            types, and SoundFiles.
-        
-        Reader/Writer Threads
-            pastream simplifies the process of implementing stream reader and writer
-            threads to manipulate and/or generate data in the background while leaving
-            the main thread free for higher level management tasks.
-        
-        
-        External Dependencies
-        =====================
-        
-        There are a few compiled libraries pastream requires which *may* need to be
-        installed separately depending on your operating system. Windows users are
-        luckiest, they can skip this section entirely.
-        
-        `libffi <https://sourceware.org/libffi/>`__ (Linux/Unix/MacOSX):
-           Under Linux/Unix/MacOSX platforms you'll need to install the ffi
-           library. (For Windows users, ffi is already included with the python cffi
-           package.)  libffi is available through most package managers::
-        
-             $ yum install libffi-devel # Red-hat/CentOS Linux
-             $ apt-get install libffi-dev # Ubuntu/debian derivatives
-             $ brew install libffi # Homebrew on OSX
-        
-           More information on installing ``libffi`` is available in the cffi
-           documentation `here
-           <https://cffi.readthedocs.io/en/latest/installation.html#platform-specific-instructions>`__.
-        
-        `PortAudio <http://www.portaudio.com>`__ and `libsndfile <http://www.mega-nerd.com/libsndfile/>`__ (Linux/Unix):
-           Linux and Unix users will also need to install a recent version of the
-           ``PortAudio`` and ``libsndfile`` libraries. (For Windows and OSX, the
-           sounddevice and soundfile python packages include prebuilt versions for
-           you.) You can either install the latest available from your package manager
-           (e.g. ``apt-get install libportaudio2 libsndfile`` for debian/raspbian) or
-           install the latest stable build from the package website (Recommended).
-        
-        
-        Installation
-        ============
-        Once the above dependencies have been resolved, you can install pastream using
-        pip::
-        
-            $ pip install pastream
-        
-        
-        Building From Source
-        =====================
-        Clone pastream with the ``--recursive`` flag::
-        
-            $ git clone --recursive http://github.com/tgarc/pastream
-        
-        Or, if you already have a checkout::
-        
-            $ cd <path/to/checkout>
-            $ git submodule update --init
-        
-        Finally, do a pip install from your local working copy::
-        
-            $ pip install <path/to/checkout>
-        
-        
-        Building Documentation
-        ======================
-        Documentation for pastream can be easily generated in a wide variety of formats
-        using Sphinx. Just follow the steps below. 
-        
-        Checkout the repository and cd into it::
-        
-            $ git clone http://github.com/tgarc/pastream
-            $ cd pastream
-        
-        Install documentation dependencies using requirements file::
-        
-            $ pip install -r docs/requirements.txt
-        
-        Then use the included Makefile/make.bat to generate documentation. (Here we
-        output to the html format)::
-        
-            $ cd docs
-            $ make html
-        
-        
-        Examples
-        ========
-        Record one second of audio to memory, then play it back:
-        
-        .. code-block:: python
-        
-           import pastream as ps
-        
-           # Use *with* statements to auto-close the stream
-           with ps.DuplexStream() as stream:
-               out = stream.record(int(stream.samplerate), blocking=True)
-               stream.play(out, blocking=True)
-        
-        Playback 10 seconds of a file, adding zero padding if the file is shorter, and
-        record the result to memory:
-        
-        .. code-block:: python
-        
-           import pastream as ps, soundfile as sf
-        
-           with sf.SoundFile('my-file.wav') as infile, ps.DuplexStream.from_file(infile) as stream:
-               out = stream.playrec(infile, frames=10 * int(stream.samplerate), pad=-1, blocking=True)
-        
-        Grab (real) frequency transformed live audio stream with 50% overlap:
-        
-        .. code-block:: python
-        
-           import pastream as ps, numpy as np
-        
-           chunksize = 1024
-           window = np.hanning(chunksize)
-           for x_l in ps.chunks(chunksize, overlap=chunksize//2, channels=1):
-               X_l = np.fft.rfft(x_l * window)
-        
-        Generate a pure tone on-the-fly
-        
-        .. code-block:: python
-        
-           import time
-           import pastream as ps
-           import numpy as np
-        
-           # A simple tone generator
-           def tone_generator(stream, buffer, f, loop=False):
-               fs = stream.samplerate
-        
-               # Create a time index
-               t = 2*np.pi*f*np.arange(len(buffer), dtype=stream.dtype) / fs
-        
-               # Loop until the stream stops
-               while not stream.finished:
-                   frames = buffer.write_available
-                   if not frames:
-                       time.sleep(0.010)
-                       continue
-        
-                   # Get the write buffers directly to avoid making any extra copies
-                   frames, part1, part2 = buffer.get_write_buffers(frames)
-        
-                   out = np.frombuffer(part1, dtype=stream.dtype)
-                   np.sin(t[:len(out)], out=out)
-        
-                   if len(part2):
-                       # part2 will be nonempty whenever we wrap around the end of the ring buffer
-                       out = np.frombuffer(part2, dtype=stream.dtype)
-                       np.sin(t[:len(out)], out=out)
-        
-                   # flag that we've added data to the buffer
-                   buffer.advance_write_index(frames)
-        
-                   # advance the time index
-                   t += 2*np.pi*f*frames / fs
-        
-           with ps.OutputStream(channels=1) as stream:
-               # Set our tone generator as the source and pass along the frequency
-               freq = 1000
-               stream.set_source(tone_generator, args=(freq,))
-        
-               # Busy-wait to allow for keyboard interrupt
-               stream.start()
-               while stream.active:
-                   time.sleep(0.1)
-        
-        See also the included examples under `/examples`.
-        
-        
-        Command Line Application
-        ========================
-        Once installed, the pastream application should be callable from your command
-        line. If you're familiar with `SoX <http://sox.sourceforge.net/>`__ you'll
-        notice that some of the command line syntax is quite similar. Here are a few
-        examples to help get you started.
-        
-        Display the help file::
-        
-            $ pastream -h
-        
-        List available audio devices::
-        
-            $ pastream -l
-        
-        Simultaneous play and record from the default audio device::
-        
-            $ pastream input.wav output.wav
-        
-        Pipe input from sox using the AU format and record the playback::
-        
-            $ sox -n -t au - synth sine 440 | pastream - output.wav
-        
-        Play a RAW file::
-        
-            $ pastream -c1 -r48k -e=pcm_16 output.raw
-        
-        Record 10 minutes of audio at 48kHz::
-        
-            $ pastream null output.wav -r48k -d10:00
-        
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
+License-File: LICENSE
+Requires-Dist: pa_ringbuffer>=0.1.2
+Requires-Dist: cffi>=1.0.0
+Requires-Dist: soundfile>=0.9.0
+Requires-Dist: sounddevice>=0.3.9
 Provides-Extra: numpy
+Requires-Dist: numpy; extra == "numpy"
+
+.. image:: https://badge.fury.io/py/pastream.svg
+    :target: https://badge.fury.io/py/pastream
+
+
+GIL-less Portaudio Streams for Python
+=====================================
+`pastream` builds on top of `portaudio <http://www.portaudio.com/>`__ and the
+excellent `sounddevice <http://github.com/spatialaudio/python-sounddevice>`__
+python bindings to provide some more advanced functionality right out of the
+box. Note that in addition to the pastream *library*, pastream includes a
+`command line application`_ for playing
+and recording audio files.
+
+Documentation:
+   http://pastream.readthedocs.io/
+
+Source code repository and issue tracker:
+   http://github.com/tgarc/pastream/
+
+
+Features
+========
+GIL-less Audio Callbacks
+    Having the portaudio callback implemented in C means audio interrupts can
+    be serviced quickly and reliably without ever needing to acquire the Python
+    Global Interpreter Lock (GIL). This is crucial when working with libraries
+    like `Pillow <https://python-pillow.org/>`__ which may greedily grab and
+    hold the GIL subsequently causing audio overruns/underruns.
+
+Input Stream iterators
+    Efficiently retrieve live audio capture data through an iterable. As simple as:
+
+    .. code-block:: python
+
+       import pastream as ps
+       for chunk in ps.chunks():
+           process(chunk)
+
+    See ``pastream.chunks`` and ``pastream.InputStream.chunks`` method.
+
+Built-in support for working with SoundFiles and numpy ndarrays
+    Seamless support for playback/recording of numpy ndarrays, generic buffer
+    types, and SoundFiles.
+
+Reader/Writer Threads
+    pastream simplifies the process of implementing stream reader and writer
+    threads to manipulate and/or generate data in the background while leaving
+    the main thread free for higher level management tasks.
+
+
+External Dependencies
+=====================
+
+There are a few compiled libraries pastream requires which *may* need to be
+installed separately depending on your operating system. Windows users are
+luckiest, they can skip this section entirely.
+
+`libffi <https://sourceware.org/libffi/>`__ (Linux/Unix/MacOSX):
+   Under Linux/Unix/MacOSX platforms you'll need to install the ffi
+   library. (For Windows users, ffi is already included with the python cffi
+   package.)  libffi is available through most package managers::
+
+     $ yum install libffi-devel # Red-hat/CentOS Linux
+     $ apt-get install libffi-dev # Ubuntu/debian derivatives
+     $ brew install libffi # Homebrew on OSX
+
+   More information on installing ``libffi`` is available in the cffi
+   documentation `here
+   <https://cffi.readthedocs.io/en/latest/installation.html#platform-specific-instructions>`__.
+
+`PortAudio <http://www.portaudio.com>`__ and `libsndfile <http://www.mega-nerd.com/libsndfile/>`__ (Linux/Unix):
+   Linux and Unix users will also need to install a recent version of the
+   ``PortAudio`` and ``libsndfile`` libraries. (For Windows and OSX, the
+   sounddevice and soundfile python packages include prebuilt versions for
+   you.) You can either install the latest available from your package manager
+   (e.g. ``apt-get install libportaudio2 libsndfile`` for debian/raspbian) or
+   install the latest stable build from the package website (Recommended).
+
+
+Installation
+============
+Once the above dependencies have been resolved, you can install pastream using
+pip::
+
+    $ pip install pastream
+
+
+Building From Source
+=====================
+Clone pastream with the ``--recursive`` flag::
+
+    $ git clone --recursive http://github.com/tgarc/pastream
+
+Or, if you already have a checkout::
+
+    $ cd <path/to/checkout>
+    $ git submodule update --init
+
+Finally, do a pip install from your local working copy::
+
+    $ pip install <path/to/checkout>
+
+
+Building Documentation
+======================
+Documentation for pastream can be easily generated in a wide variety of formats
+using Sphinx. Just follow the steps below. 
+
+Checkout the repository and cd into it::
+
+    $ git clone http://github.com/tgarc/pastream
+    $ cd pastream
+
+Install documentation dependencies using requirements file::
+
+    $ pip install -r docs/requirements.txt
+
+Then use the included Makefile/make.bat to generate documentation. (Here we
+output to the html format)::
+
+    $ cd docs
+    $ make html
+
+
+Examples
+========
+Record one second of audio to memory, then play it back:
+
+.. code-block:: python
+
+   import pastream as ps
+
+   # Use *with* statements to auto-close the stream
+   with ps.DuplexStream() as stream:
+       out = stream.record(int(stream.samplerate), blocking=True)
+       stream.play(out, blocking=True)
+
+Playback 10 seconds of a file, adding zero padding if the file is shorter, and
+record the result to memory:
+
+.. code-block:: python
+
+   import pastream as ps, soundfile as sf
+
+   with sf.SoundFile('my-file.wav') as infile, ps.DuplexStream.from_file(infile) as stream:
+       out = stream.playrec(infile, frames=10 * int(stream.samplerate), pad=-1, blocking=True)
+
+Grab (real) frequency transformed live audio stream with 50% overlap:
+
+.. code-block:: python
+
+   import pastream as ps, numpy as np
+
+   chunksize = 1024
+   window = np.hanning(chunksize)
+   for x_l in ps.chunks(chunksize, overlap=chunksize//2, channels=1):
+       X_l = np.fft.rfft(x_l * window)
+
+Generate a pure tone on-the-fly
+
+.. code-block:: python
+
+   import time
+   import pastream as ps
+   import numpy as np
+
+   # A simple tone generator
+   def tone_generator(stream, buffer, f, loop=False):
+       fs = stream.samplerate
+
+       # Create a time index
+       t = 2*np.pi*f*np.arange(len(buffer), dtype=stream.dtype) / fs
+
+       # Loop until the stream stops
+       while not stream.finished:
+           frames = buffer.write_available
+           if not frames:
+               time.sleep(0.010)
+               continue
+
+           # Get the write buffers directly to avoid making any extra copies
+           frames, part1, part2 = buffer.get_write_buffers(frames)
+
+           out = np.frombuffer(part1, dtype=stream.dtype)
+           np.sin(t[:len(out)], out=out)
+
+           if len(part2):
+               # part2 will be nonempty whenever we wrap around the end of the ring buffer
+               out = np.frombuffer(part2, dtype=stream.dtype)
+               np.sin(t[:len(out)], out=out)
+
+           # flag that we've added data to the buffer
+           buffer.advance_write_index(frames)
+
+           # advance the time index
+           t += 2*np.pi*f*frames / fs
+
+   with ps.OutputStream(channels=1) as stream:
+       # Set our tone generator as the source and pass along the frequency
+       freq = 1000
+       stream.set_source(tone_generator, args=(freq,))
+
+       # Busy-wait to allow for keyboard interrupt
+       stream.start()
+       while stream.active:
+           time.sleep(0.1)
+
+See also the included examples under `/examples`.
+
+
+Command Line Application
+========================
+Once installed, the pastream application should be callable from your command
+line. If you're familiar with `SoX <http://sox.sourceforge.net/>`__ you'll
+notice that some of the command line syntax is quite similar. Here are a few
+examples to help get you started.
+
+Display the help file::
+
+    $ pastream -h
+
+List available audio devices::
+
+    $ pastream -l
+
+Simultaneous play and record from the default audio device::
+
+    $ pastream input.wav output.wav
+
+Pipe input from sox using the AU format and record the playback::
+
+    $ sox -n -t au - synth sine 440 | pastream - output.wav
+
+Play a RAW file::
+
+    $ pastream -c1 -r48k -e=pcm_16 output.raw
+
+Record 10 minutes of audio at 48kHz::
+
+    $ pastream null output.wav -r48k -d10:00
```

### Comparing `pastream-0.2.0.post0/src/pastream.egg-info/SOURCES.txt` & `pastream-0.2.0.post1/src/pastream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pastream-0.2.0.post0/src/py_pastream.c` & `pastream-0.2.0.post1/src/py_pastream.c`

 * *Files identical despite different names*

