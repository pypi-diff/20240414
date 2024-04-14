# Comparing `tmp/WuttJamaican-0.1.8.tar.gz` & `tmp/WuttJamaican-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WuttJamaican-0.1.8.tar", last modified: Sat Nov 25 05:21:08 2023, max compression
+gzip compressed data, was "WuttJamaican-0.1.9.tar", last modified: Thu Nov 30 21:12:20 2023, max compression
```

## Comparing `WuttJamaican-0.1.8.tar` & `WuttJamaican-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-11-17 22:12:16.000000 WuttJamaican-0.1.8/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1370 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      138 2023-11-24 22:54:33.000000 WuttJamaican-0.1.8/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)     1372 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1047 2023-10-13 15:36:01.000000 WuttJamaican-0.1.8/setup.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-25 05:21:08.746236 WuttJamaican-0.1.8/src/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/src/WuttJamaican.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1370 2023-11-25 05:21:08.000000 WuttJamaican-0.1.8/src/WuttJamaican.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      925 2023-11-25 05:21:08.000000 WuttJamaican-0.1.8/src/WuttJamaican.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-11-25 05:21:08.000000 WuttJamaican-0.1.8/src/WuttJamaican.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      225 2023-11-25 05:21:08.000000 WuttJamaican-0.1.8/src/WuttJamaican.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      107 2023-11-25 05:21:08.000000 WuttJamaican-0.1.8/src/WuttJamaican.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       13 2023-11-25 05:21:08.000000 WuttJamaican-0.1.8/src/WuttJamaican.egg-info/top_level.txt
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/src/wuttjamaican/
--rw-r--r--   0 lance     (1000) lance     (1000)     1065 2023-11-19 06:51:42.000000 WuttJamaican-0.1.8/src/wuttjamaican/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-11-25 05:20:47.000000 WuttJamaican-0.1.8/src/wuttjamaican/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9313 2023-11-25 05:11:26.000000 WuttJamaican-0.1.8/src/wuttjamaican/app.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/src/wuttjamaican/cmd/
--rw-r--r--   0 lance     (1000) lance     (1000)     1235 2023-11-23 00:55:50.000000 WuttJamaican-0.1.8/src/wuttjamaican/cmd/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14591 2023-11-24 20:21:55.000000 WuttJamaican-0.1.8/src/wuttjamaican/cmd/base.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2145 2023-11-23 02:54:22.000000 WuttJamaican-0.1.8/src/wuttjamaican/cmd/date_organize.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2314 2023-11-22 16:52:23.000000 WuttJamaican-0.1.8/src/wuttjamaican/cmd/make_appdir.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1400 2023-11-22 17:01:25.000000 WuttJamaican-0.1.8/src/wuttjamaican/cmd/setup.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/src/wuttjamaican/commands/
--rw-r--r--   0 lance     (1000) lance     (1000)     1233 2023-11-22 17:06:59.000000 WuttJamaican-0.1.8/src/wuttjamaican/commands/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1236 2023-11-22 17:07:06.000000 WuttJamaican-0.1.8/src/wuttjamaican/commands/base.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1249 2023-11-22 17:07:11.000000 WuttJamaican-0.1.8/src/wuttjamaican/commands/make_appdir.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1237 2023-11-22 17:07:15.000000 WuttJamaican-0.1.8/src/wuttjamaican/commands/setup.py
--rw-r--r--   0 lance     (1000) lance     (1000)    31856 2023-11-25 00:43:25.000000 WuttJamaican-0.1.8/src/wuttjamaican/conf.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/src/wuttjamaican/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1357 2023-11-21 04:07:46.000000 WuttJamaican-0.1.8/src/wuttjamaican/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3055 2023-11-19 23:12:10.000000 WuttJamaican-0.1.8/src/wuttjamaican/db/conf.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3623 2023-10-28 21:31:07.000000 WuttJamaican-0.1.8/src/wuttjamaican/db/sess.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1218 2023-10-28 20:42:53.000000 WuttJamaican-0.1.8/src/wuttjamaican/exc.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2556 2023-11-23 03:47:48.000000 WuttJamaican-0.1.8/src/wuttjamaican/testing.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5181 2023-11-20 00:36:57.000000 WuttJamaican-0.1.8/src/wuttjamaican/util.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-25 05:21:08.750236 WuttJamaican-0.1.8/tests/
--rw-r--r--   0 lance     (1000) lance     (1000)     6244 2023-11-25 05:11:26.000000 WuttJamaican-0.1.8/tests/test_app.py
--rw-r--r--   0 lance     (1000) lance     (1000)    24665 2023-11-25 00:43:44.000000 WuttJamaican-0.1.8/tests/test_conf.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9496 2023-11-20 00:50:51.000000 WuttJamaican-0.1.8/tests/test_util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-30 21:12:20.192766 WuttJamaican-0.1.9/
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2018-11-17 22:12:16.000000 WuttJamaican-0.1.9/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1370 2023-11-30 21:12:20.192766 WuttJamaican-0.1.9/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      138 2023-11-24 22:54:33.000000 WuttJamaican-0.1.9/README.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)     1372 2023-11-30 21:12:20.192766 WuttJamaican-0.1.9/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1047 2023-10-13 15:36:01.000000 WuttJamaican-0.1.9/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-30 21:12:20.188766 WuttJamaican-0.1.9/src/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-30 21:12:20.192766 WuttJamaican-0.1.9/src/WuttJamaican.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1370 2023-11-30 21:12:20.000000 WuttJamaican-0.1.9/src/WuttJamaican.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      925 2023-11-30 21:12:20.000000 WuttJamaican-0.1.9/src/WuttJamaican.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-11-30 21:12:20.000000 WuttJamaican-0.1.9/src/WuttJamaican.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      225 2023-11-30 21:12:20.000000 WuttJamaican-0.1.9/src/WuttJamaican.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      107 2023-11-30 21:12:20.000000 WuttJamaican-0.1.9/src/WuttJamaican.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       13 2023-11-30 21:12:20.000000 WuttJamaican-0.1.9/src/WuttJamaican.egg-info/top_level.txt
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-30 21:12:20.188766 WuttJamaican-0.1.9/src/wuttjamaican/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1065 2023-11-19 06:51:42.000000 WuttJamaican-0.1.9/src/wuttjamaican/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-11-30 21:11:43.000000 WuttJamaican-0.1.9/src/wuttjamaican/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9758 2023-11-26 00:05:44.000000 WuttJamaican-0.1.9/src/wuttjamaican/app.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-30 21:12:20.188766 WuttJamaican-0.1.9/src/wuttjamaican/cmd/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1235 2023-11-23 00:55:50.000000 WuttJamaican-0.1.9/src/wuttjamaican/cmd/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    14591 2023-11-24 20:21:55.000000 WuttJamaican-0.1.9/src/wuttjamaican/cmd/base.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2145 2023-11-23 02:54:22.000000 WuttJamaican-0.1.9/src/wuttjamaican/cmd/date_organize.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2314 2023-11-22 16:52:23.000000 WuttJamaican-0.1.9/src/wuttjamaican/cmd/make_appdir.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1400 2023-11-22 17:01:25.000000 WuttJamaican-0.1.9/src/wuttjamaican/cmd/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-30 21:12:20.188766 WuttJamaican-0.1.9/src/wuttjamaican/commands/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1233 2023-11-22 17:06:59.000000 WuttJamaican-0.1.9/src/wuttjamaican/commands/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1236 2023-11-22 17:07:06.000000 WuttJamaican-0.1.9/src/wuttjamaican/commands/base.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1249 2023-11-22 17:07:11.000000 WuttJamaican-0.1.9/src/wuttjamaican/commands/make_appdir.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1237 2023-11-22 17:07:15.000000 WuttJamaican-0.1.9/src/wuttjamaican/commands/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    31852 2023-11-25 23:06:51.000000 WuttJamaican-0.1.9/src/wuttjamaican/conf.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-30 21:12:20.192766 WuttJamaican-0.1.9/src/wuttjamaican/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1357 2023-11-21 04:07:46.000000 WuttJamaican-0.1.9/src/wuttjamaican/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3055 2023-11-19 23:12:10.000000 WuttJamaican-0.1.9/src/wuttjamaican/db/conf.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3623 2023-10-28 21:31:07.000000 WuttJamaican-0.1.9/src/wuttjamaican/db/sess.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1218 2023-10-28 20:42:53.000000 WuttJamaican-0.1.9/src/wuttjamaican/exc.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2556 2023-11-23 03:47:48.000000 WuttJamaican-0.1.9/src/wuttjamaican/testing.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5181 2023-11-20 00:36:57.000000 WuttJamaican-0.1.9/src/wuttjamaican/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-30 21:12:20.192766 WuttJamaican-0.1.9/tests/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6620 2023-11-26 00:05:44.000000 WuttJamaican-0.1.9/tests/test_app.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    24669 2023-11-26 00:00:16.000000 WuttJamaican-0.1.9/tests/test_conf.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9496 2023-11-20 00:50:51.000000 WuttJamaican-0.1.9/tests/test_util.py
```

### Comparing `WuttJamaican-0.1.8/COPYING.txt` & `WuttJamaican-0.1.9/COPYING.txt`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/PKG-INFO` & `WuttJamaican-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WuttJamaican
-Version: 0.1.8
+Version: 0.1.9
 Summary: Base package for Wutta Framework
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `WuttJamaican-0.1.8/setup.cfg` & `WuttJamaican-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/setup.py` & `WuttJamaican-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/WuttJamaican.egg-info/PKG-INFO` & `WuttJamaican-0.1.9/src/WuttJamaican.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WuttJamaican
-Version: 0.1.8
+Version: 0.1.9
 Summary: Base package for Wutta Framework
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `WuttJamaican-0.1.8/src/WuttJamaican.egg-info/SOURCES.txt` & `WuttJamaican-0.1.9/src/WuttJamaican.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/__init__.py` & `WuttJamaican-0.1.9/src/wuttjamaican/__init__.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/app.py` & `WuttJamaican-0.1.9/src/wuttjamaican/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,7 +277,23 @@
             warnings.warn("passing app handler to app provider is deprecated; "
                           "must pass config object instead",
                           DeprecationWarning, stacklevel=2)
             config = config.config
 
         self.config = config
         self.app = config.get_app()
+
+
+class GenericHandler:
+    """
+    Generic base class for handlers.
+
+    When the :term:`app` defines a new *type* of :term:`handler` it
+    may subclass this when defining the handler base class.
+
+    :param config: Config object for the app.  This should be an
+       instance of :class:`~wuttjamaican.conf.WuttaConfig`.
+    """
+
+    def __init__(self, config, **kwargs):
+        self.config = config
+        self.app = self.config.get_app()
```

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/cmd/__init__.py` & `WuttJamaican-0.1.9/src/wuttjamaican/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/cmd/base.py` & `WuttJamaican-0.1.9/src/wuttjamaican/cmd/base.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/cmd/date_organize.py` & `WuttJamaican-0.1.9/src/wuttjamaican/cmd/date_organize.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/cmd/make_appdir.py` & `WuttJamaican-0.1.9/src/wuttjamaican/cmd/make_appdir.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/cmd/setup.py` & `WuttJamaican-0.1.9/src/wuttjamaican/cmd/setup.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/commands/__init__.py` & `WuttJamaican-0.1.9/src/wuttjamaican/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/commands/base.py` & `WuttJamaican-0.1.9/src/wuttjamaican/commands/base.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/commands/make_appdir.py` & `WuttJamaican-0.1.9/src/wuttjamaican/commands/make_appdir.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/commands/setup.py` & `WuttJamaican-0.1.9/src/wuttjamaican/commands/setup.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/conf.py` & `WuttJamaican-0.1.9/src/wuttjamaican/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,15 +806,15 @@
 
     # when running as a proper windows service, must first read
     # "default" file(s) and then consult config to see which file
     # should "really" be used.  because there isn't a way to specify
     # which config file as part of the actual service definition in
     # windows, so the service name is used for magic lookup here.
     if winsvc:
-        config = configparser.SafeConfigParser()
+        config = configparser.ConfigParser()
         config.read(files)
         section = f'{appname}.config'
         if config.has_section(section):
             option = f'winsvc.{winsvc}'
             if config.has_option(section, option):
                 # replace file paths with whatever config value says
                 files = parse_list(config.get(section, option))
```

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/db/__init__.py` & `WuttJamaican-0.1.9/src/wuttjamaican/db/__init__.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/db/conf.py` & `WuttJamaican-0.1.9/src/wuttjamaican/db/conf.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/db/sess.py` & `WuttJamaican-0.1.9/src/wuttjamaican/db/sess.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/exc.py` & `WuttJamaican-0.1.9/src/wuttjamaican/exc.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/testing.py` & `WuttJamaican-0.1.9/src/wuttjamaican/testing.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/src/wuttjamaican/util.py` & `WuttJamaican-0.1.9/src/wuttjamaican/util.py`

 * *Files identical despite different names*

### Comparing `WuttJamaican-0.1.8/tests/test_app.py` & `WuttJamaican-0.1.9/tests/test_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,7 +184,20 @@
 
         # custom attr does not exist yet
         self.assertRaises(AttributeError, getattr, self.app, 'foo_value')
 
         # but provider can supply the attr
         self.app.providers['mytest'] = MagicMock(foo_value='bar')
         self.assertEqual(self.app.foo_value, 'bar')
+
+
+class TestGenericHandler(TestCase):
+
+    def setUp(self):
+        self.config = WuttaConfig(appname='wuttatest')
+        self.app = app.AppHandler(self.config)
+        self.config.app = self.app
+
+    def test_constructor(self):
+        handler = app.GenericHandler(self.config)
+        self.assertIs(handler.config, self.config)
+        self.assertIs(handler.app, self.app)
```

### Comparing `WuttJamaican-0.1.8/tests/test_conf.py` & `WuttJamaican-0.1.9/tests/test_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,15 +596,15 @@
                 WuttaConfig.assert_called_once_with([], appname='wuttatest',
                                                     usedb=None, preferdb=None)
                 load_entry_points.assert_not_called()
 
                 # confirm entry points for default appname
                 load_entry_points.reset_mock()
                 WuttaConfig.reset_mock()
-                config = conf.make_config(appname='wutta')
+                config = conf.make_config([], appname='wutta')
                 WuttaConfig.assert_called_once_with([], appname='wutta',
                                                     usedb=None, preferdb=None)
                 load_entry_points.assert_called_once_with('wutta.config.extensions')
 
                 # confirm entry points for custom appname
                 load_entry_points.reset_mock()
                 WuttaConfig.reset_mock()
```

### Comparing `WuttJamaican-0.1.8/tests/test_util.py` & `WuttJamaican-0.1.9/tests/test_util.py`

 * *Files identical despite different names*

