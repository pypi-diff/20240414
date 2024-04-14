# Comparing `tmp/wristwatch-1.0.1.tar.gz` & `tmp/wristwatch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wristwatch-1.0.1.tar", last modified: Sat Apr 13 18:44:01 2024, max compression
+gzip compressed data, was "wristwatch-1.0.2.tar", last modified: Sat Apr 13 19:23:52 2024, max compression
```

## Comparing `wristwatch-1.0.1.tar` & `wristwatch-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 18:44:01.316981 wristwatch-1.0.1/
--rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1086 2022-12-24 08:05:26.000000 wristwatch-1.0.1/LICENSE
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     2091 2024-04-13 18:44:01.316981 wristwatch-1.0.1/PKG-INFO
--rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1887 2024-04-13 17:52:50.000000 wristwatch-1.0.1/README.md
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       38 2024-04-13 18:44:01.316981 wristwatch-1.0.1/setup.cfg
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      480 2024-04-13 18:43:17.000000 wristwatch-1.0.1/setup.py
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 18:44:01.316981 wristwatch-1.0.1/wristwatch/
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 17:46:48.000000 wristwatch-1.0.1/wristwatch/__init__.py
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     7381 2024-04-13 17:40:50.000000 wristwatch-1.0.1/wristwatch/wristwatch.py
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 18:44:01.316981 wristwatch-1.0.1/wristwatch.egg-info/
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     2091 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/PKG-INFO
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      280 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        1 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       59 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/entry_points.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       56 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/requires.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       11 2024-04-13 18:44:01.000000 wristwatch-1.0.1/wristwatch.egg-info/top_level.txt
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 19:23:52.152977 wristwatch-1.0.2/
+-rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1086 2022-12-24 08:05:26.000000 wristwatch-1.0.2/LICENSE
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     2123 2024-04-13 19:23:52.152977 wristwatch-1.0.2/PKG-INFO
+-rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1887 2024-04-13 17:52:50.000000 wristwatch-1.0.2/README.md
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       38 2024-04-13 19:23:52.152977 wristwatch-1.0.2/setup.cfg
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      528 2024-04-13 19:23:08.000000 wristwatch-1.0.2/setup.py
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 19:23:52.152977 wristwatch-1.0.2/wristwatch/
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 17:46:48.000000 wristwatch-1.0.2/wristwatch/__init__.py
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     7422 2024-04-13 19:23:06.000000 wristwatch-1.0.2/wristwatch/wristwatch.py
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 19:23:52.152977 wristwatch-1.0.2/wristwatch.egg-info/
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     2123 2024-04-13 19:23:52.000000 wristwatch-1.0.2/wristwatch.egg-info/PKG-INFO
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      280 2024-04-13 19:23:52.000000 wristwatch-1.0.2/wristwatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        1 2024-04-13 19:23:52.000000 wristwatch-1.0.2/wristwatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       59 2024-04-13 19:23:52.000000 wristwatch-1.0.2/wristwatch.egg-info/entry_points.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       56 2024-04-13 19:23:52.000000 wristwatch-1.0.2/wristwatch.egg-info/requires.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       11 2024-04-13 19:23:52.000000 wristwatch-1.0.2/wristwatch.egg-info/top_level.txt
```

### Comparing `wristwatch-1.0.1/LICENSE` & `wristwatch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wristwatch-1.0.1/PKG-INFO` & `wristwatch-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wristwatch
-Version: 1.0.1
+Version: 1.0.2
 Summary: Yet another Python watcher for website updates.
-Home-page: UNKNOWN
+Home-page: https://github.com/zWolfrost/wristwatch
 Author: zWolfrost
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wristwatch
```

### Comparing `wristwatch-1.0.1/README.md` & `wristwatch-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wristwatch-1.0.1/wristwatch/wristwatch.py` & `wristwatch-1.0.2/wristwatch/wristwatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 	parser.add_argument("-q", "--quiet", help="Decrease output verbosity.", action="store_true")
 	parser.add_argument("-l", "--loop", help="Keep watching for changes even after the first one.", action="store_true")
 
 	parser.add_argument("-o", "--output", type=str, help="Save the last fetch to a file.", metavar="FILE")
 	parser.add_argument("-i", "--input", type=str, help="Load the first fetch from a file.", metavar="FILE")
 
-	parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.0.0")
+	parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.0.2")
 
 	return vars(parser.parse_args())
 
 
 def init_driver():
 	options = Options()
 
@@ -227,15 +227,17 @@
 					with open(ARGS["output"], "w") as f:
 						f.write(current_fetch)
 
 				if (ARGS["email"]):
 					print(f"Sending email to {ARGS['email']}...")
 					send_email(ARGS["email"], ARGS["email"], ARGS["password"], subject=f"Changes detected on {ARGS['webpage']}", body=diff)
 
-				if (not ARGS["loop"]):
+				if (ARGS["loop"]):
+					first_fetch = current_fetch
+				else:
 					break
 			else:
 				print(f"\rNo changes detected ({fetches} fetches).", end="")
 	except KeyboardInterrupt:
 		print(f"\nStopped watching.")
```

### Comparing `wristwatch-1.0.1/wristwatch.egg-info/PKG-INFO` & `wristwatch-1.0.2/wristwatch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wristwatch
-Version: 1.0.1
+Version: 1.0.2
 Summary: Yet another Python watcher for website updates.
-Home-page: UNKNOWN
+Home-page: https://github.com/zWolfrost/wristwatch
 Author: zWolfrost
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wristwatch
```

