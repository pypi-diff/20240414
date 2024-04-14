# Comparing `tmp/pnu_portstreelint-1.4.0.tar.gz` & `tmp/pnu_portstreelint-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnu_portstreelint-1.4.0.tar", last modified: Sat Apr 13 16:50:02 2024, max compression
+gzip compressed data, was "pnu_portstreelint-1.4.1.tar", last modified: Sat Apr 13 17:08:44 2024, max compression
```

## Comparing `pnu_portstreelint-1.4.0.tar` & `pnu_portstreelint-1.4.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.255304 pnu_portstreelint-1.4.0/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1461 2024-03-01 21:23:12.000000 pnu_portstreelint-1.4.0/License
--rw-r--r--   0 hubert    (1001) hubert    (1001)    11253 2024-04-13 16:50:02.255269 pnu_portstreelint-1.4.0/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)    10018 2024-04-13 16:32:45.000000 pnu_portstreelint-1.4.0/README.md
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.250168 pnu_portstreelint-1.4.0/man/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     3468 2024-04-13 16:49:59.000000 pnu_portstreelint-1.4.0/man/portstreelint.8.gz
--rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-17 21:50:43.000000 pnu_portstreelint-1.4.0/pyproject.toml
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1437 2024-04-13 16:50:02.256016 pnu_portstreelint-1.4.0/setup.cfg
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.237448 pnu_portstreelint-1.4.0/src/
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.255001 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/
--rw-r--r--   0 hubert    (1001) hubert    (1001)    11253 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1099 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/SOURCES.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/dependency_links.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)      106 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/entry_points.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       35 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/requires.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)       14 2024-04-13 16:50:02.000000 pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/top_level.txt
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 16:50:02.254805 pnu_portstreelint-1.4.0/src/portstreelint/
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-01 21:22:20.000000 pnu_portstreelint-1.4.0/src/portstreelint/__init__.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3225 2024-04-13 16:17:29.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_categories.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2407 2024-04-13 16:17:36.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_comment.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3151 2024-04-13 16:17:46.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_description_file.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1516 2024-04-13 16:17:54.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_installation_prefix.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4530 2024-04-13 16:46:46.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_licenses.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1400 2024-04-13 16:18:12.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_maintainer.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4102 2024-04-13 16:18:18.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_marks.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3096 2024-04-13 16:18:24.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_plist.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)      976 2024-04-13 16:18:30.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_port_path.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1052 2024-04-13 16:18:35.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_unchanging_ports.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     5597 2024-04-13 16:18:41.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_vulnerabilities.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7050 2024-04-13 16:18:47.000000 pnu_portstreelint-1.4.0/src/portstreelint/check_www_site.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2147 2024-04-13 13:34:33.000000 pnu_portstreelint-1.4.0/src/portstreelint/library.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     8013 2024-04-13 16:16:47.000000 pnu_portstreelint-1.4.0/src/portstreelint/load_config.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4912 2024-04-13 16:19:07.000000 pnu_portstreelint-1.4.0/src/portstreelint/load_data.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)    16028 2024-04-13 16:19:37.000000 pnu_portstreelint-1.4.0/src/portstreelint/main.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1005 2024-03-03 22:54:02.000000 pnu_portstreelint-1.4.0/src/portstreelint/show_categories.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)      987 2024-03-03 22:54:09.000000 pnu_portstreelint-1.4.0/src/portstreelint/show_maintainers.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1756 2024-04-13 16:19:48.000000 pnu_portstreelint-1.4.0/src/portstreelint/show_notifications.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4314 2024-04-13 16:19:54.000000 pnu_portstreelint-1.4.0/src/portstreelint/show_summary.py
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 17:08:44.516640 pnu_portstreelint-1.4.1/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1461 2024-03-01 21:23:12.000000 pnu_portstreelint-1.4.1/License
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    11253 2024-04-13 17:08:44.516608 pnu_portstreelint-1.4.1/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    10018 2024-04-13 16:32:45.000000 pnu_portstreelint-1.4.1/README.md
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 17:08:44.511569 pnu_portstreelint-1.4.1/man/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     3468 2024-04-13 17:08:42.000000 pnu_portstreelint-1.4.1/man/portstreelint.8.gz
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       81 2024-03-17 21:50:43.000000 pnu_portstreelint-1.4.1/pyproject.toml
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1437 2024-04-13 17:08:44.517351 pnu_portstreelint-1.4.1/setup.cfg
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 17:08:44.510647 pnu_portstreelint-1.4.1/src/
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 17:08:44.516342 pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)    11253 2024-04-13 17:08:44.000000 pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1099 2024-04-13 17:08:44.000000 pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/SOURCES.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2024-04-13 17:08:44.000000 pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/dependency_links.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)      106 2024-04-13 17:08:44.000000 pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/entry_points.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       35 2024-04-13 17:08:44.000000 pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/requires.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)       14 2024-04-13 17:08:44.000000 pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/top_level.txt
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2024-04-13 17:08:44.516150 pnu_portstreelint-1.4.1/src/portstreelint/
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2024-03-01 21:22:20.000000 pnu_portstreelint-1.4.1/src/portstreelint/__init__.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3225 2024-04-13 16:17:29.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_categories.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2407 2024-04-13 16:17:36.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_comment.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3151 2024-04-13 16:17:46.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_description_file.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1516 2024-04-13 16:17:54.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_installation_prefix.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4530 2024-04-13 16:46:46.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_licenses.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1400 2024-04-13 16:18:12.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_maintainer.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4102 2024-04-13 16:18:18.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_marks.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     3096 2024-04-13 16:18:24.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_plist.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)      976 2024-04-13 16:18:30.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_port_path.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1052 2024-04-13 16:18:35.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_unchanging_ports.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     5597 2024-04-13 16:18:41.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_vulnerabilities.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     7050 2024-04-13 16:18:47.000000 pnu_portstreelint-1.4.1/src/portstreelint/check_www_site.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     2147 2024-04-13 13:34:33.000000 pnu_portstreelint-1.4.1/src/portstreelint/library.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     8013 2024-04-13 16:16:47.000000 pnu_portstreelint-1.4.1/src/portstreelint/load_config.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4912 2024-04-13 16:19:07.000000 pnu_portstreelint-1.4.1/src/portstreelint/load_data.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)    16004 2024-04-13 17:07:41.000000 pnu_portstreelint-1.4.1/src/portstreelint/main.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1005 2024-03-03 22:54:02.000000 pnu_portstreelint-1.4.1/src/portstreelint/show_categories.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)      987 2024-03-03 22:54:09.000000 pnu_portstreelint-1.4.1/src/portstreelint/show_maintainers.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     1756 2024-04-13 16:19:48.000000 pnu_portstreelint-1.4.1/src/portstreelint/show_notifications.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4314 2024-04-13 16:19:54.000000 pnu_portstreelint-1.4.1/src/portstreelint/show_summary.py
```

### Comparing `pnu_portstreelint-1.4.0/License` & `pnu_portstreelint-1.4.1/License`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/PKG-INFO` & `pnu_portstreelint-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-portstreelint
-Version: 1.4.0
+Version: 1.4.1
 Summary: FreeBSD ports tree lint
 Home-page: https://github.com/HubTou/portstreelint/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/portstreelint/issues
 Keywords: pnu-project
```

### Comparing `pnu_portstreelint-1.4.0/README.md` & `pnu_portstreelint-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/man/portstreelint.8.gz` & `pnu_portstreelint-1.4.1/man/portstreelint.8.gz`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/setup.cfg` & `pnu_portstreelint-1.4.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pnu-portstreelint
 description = FreeBSD ports tree lint
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 1.4.0
+version = 1.4.1
 license = BSD 3-Clause License
 license_files = License
 author = Hubert Tournier
 author_email = hubert.tournier@gmail.com
 url = https://github.com/HubTou/portstreelint/
 project_urls = 
 	Bug Tracker = https://github.com/HubTou/portstreelint/issues
```

### Comparing `pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/PKG-INFO` & `pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-portstreelint
-Version: 1.4.0
+Version: 1.4.1
 Summary: FreeBSD ports tree lint
 Home-page: https://github.com/HubTou/portstreelint/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/portstreelint/issues
 Keywords: pnu-project
```

### Comparing `pnu_portstreelint-1.4.0/src/pnu_portstreelint.egg-info/SOURCES.txt` & `pnu_portstreelint-1.4.1/src/pnu_portstreelint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_categories.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_categories.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_comment.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_comment.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_description_file.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_description_file.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_installation_prefix.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_installation_prefix.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_licenses.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_licenses.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_maintainer.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_maintainer.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_marks.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_marks.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_plist.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_plist.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_port_path.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_port_path.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_unchanging_ports.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_unchanging_ports.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_vulnerabilities.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/check_www_site.py` & `pnu_portstreelint-1.4.1/src/portstreelint/check_www_site.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/library.py` & `pnu_portstreelint-1.4.1/src/portstreelint/library.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/load_config.py` & `pnu_portstreelint-1.4.1/src/portstreelint/load_config.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/load_data.py` & `pnu_portstreelint-1.4.1/src/portstreelint/load_data.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/main.py` & `pnu_portstreelint-1.4.1/src/portstreelint/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from .check_www_site import check_www_site
 from .show_categories import show_categories
 from .show_maintainers import show_maintainers
 from .show_notifications import show_notifications, output_notifications
 from .show_summary import show_summary
 
 # Version string used by the what(1) and ident(1) commands:
-ID = "@(#) $Id: portstreelint - FreeBSD ports tree lint v1.4.0 (April 13, 2024) by Hubert Tournier $"
+ID = "@(#) $Id: portstreelint - FreeBSD ports tree lint v1.4.1 (April 13, 2024) by Hubert Tournier $"
 
 # Default parameters. Can be overcome by command line options:
 parameters = {
     "INI filename": "",
     "Ports dir": "/usr/ports",
     "CSV filename": "",
     "Show categories": False,
@@ -300,15 +300,14 @@
     #pylint: enable=C0103, W0602
 
     program_name = os.path.basename(sys.argv[0])
 
     libpnu.initialize_debugging(program_name)
     libpnu.handle_interrupt_signals(libpnu.interrupt_handler_function)
 
-    print(sys.argv[1:])
     if not "--nocfg" in sys.argv[1:]:
         parameters = load_config(parameters)
     _process_environment_variables()
     _ = _process_command_line()
 
     # Load the FreeBSD ports INDEX file
     # and verify structural integrity (ie: 13 pipe-separated fields)
```

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/show_categories.py` & `pnu_portstreelint-1.4.1/src/portstreelint/show_categories.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/show_maintainers.py` & `pnu_portstreelint-1.4.1/src/portstreelint/show_maintainers.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/show_notifications.py` & `pnu_portstreelint-1.4.1/src/portstreelint/show_notifications.py`

 * *Files identical despite different names*

### Comparing `pnu_portstreelint-1.4.0/src/portstreelint/show_summary.py` & `pnu_portstreelint-1.4.1/src/portstreelint/show_summary.py`

 * *Files identical despite different names*

