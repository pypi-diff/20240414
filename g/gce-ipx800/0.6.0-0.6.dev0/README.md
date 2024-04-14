# Comparing `tmp/gce_ipx800-0.6.0.tar.gz` & `tmp/gce_ipx800-0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gce_ipx800-0.6.0.tar", max compression
+gzip compressed data, was "gce_ipx800-0.6.dev0.tar", max compression
```

## Comparing `gce_ipx800-0.6.0.tar` & `gce_ipx800-0.6.dev0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11358 2024-04-14 07:05:27.194662 gce_ipx800-0.6.0/LICENSE
--rw-r--r--   0        0        0     1675 2024-04-14 07:05:27.194662 gce_ipx800-0.6.0/README.rst
--rw-r--r--   0        0        0      153 2024-04-14 07:05:27.194662 gce_ipx800-0.6.0/ipx800/__init__.py
--rw-r--r--   0        0        0     6773 2024-04-14 07:05:27.194662 gce_ipx800-0.6.0/ipx800/ipx800.py
--rw-r--r--   0        0        0     1620 2024-04-14 07:05:27.194662 gce_ipx800-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 gce_ipx800-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-10-02 19:38:59.383157 gce_ipx800-0.6.dev0/LICENSE
+-rw-r--r--   0        0        0     1674 2023-10-02 19:38:59.383157 gce_ipx800-0.6.dev0/README.rst
+-rw-r--r--   0        0        0      156 2023-10-02 19:38:59.383157 gce_ipx800-0.6.dev0/ipx800/__init__.py
+-rw-r--r--   0        0        0     6773 2023-10-02 19:38:59.383157 gce_ipx800-0.6.dev0/ipx800/ipx800.py
+-rw-r--r--   0        0        0     1570 2023-10-02 19:38:59.383157 gce_ipx800-0.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 gce_ipx800-0.6.dev0/PKG-INFO
```

### Comparing `gce_ipx800-0.6.0/LICENSE` & `gce_ipx800-0.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `gce_ipx800-0.6.0/README.rst` & `gce_ipx800-0.6.dev0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     r4.status  # => return a Boolean
 
     r4.on()
 
     r4.off()
 
-    r4.toggle()
+    r4.togle()
 
     len(ipx.relays)  # => 56
 
 Links
 -----
 
 * GCE IPX800 V4 API: https://gce.ovh/wiki/index.php?title=API_V4
```

### Comparing `gce_ipx800-0.6.0/ipx800/ipx800.py` & `gce_ipx800-0.6.dev0/ipx800/ipx800.py`

 * *Files identical despite different names*

### Comparing `gce_ipx800-0.6.0/pyproject.toml` & `gce_ipx800-0.6.dev0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gce-ipx800"
-version = "0.6.0"
+version = "0.6.dev0"
 description = "Library to interact with the GCE Electronics IPX800 device"
 authors = ["Marc-Aurèle Brothier <m@brothier.org>"]
 license = "Apache-2.0"
 readme = 'README.rst'
 repository = "https://github.com/marcaurele/gce-ipx800"
 homepage = "https://github.com/marcaurele/gce-ipx800"
 keywords = ['ipx800', 'GCE-Electronics', 'GCE', 'home-automation']
@@ -14,38 +14,39 @@
                "Operating System :: OS Independent",
 	       "Programming Language :: Python",
 	       "Programming Language :: Python :: 3",
 	       "Programming Language :: Python :: 3.8",
 	       "Programming Language :: Python :: 3.9",
 	       "Programming Language :: Python :: 3.10",
 	       "Programming Language :: Python :: 3.11",
-	       "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "ipx800" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.26"
 
+[tool.poetry.dev-dependencies]
+pytest = "^7.0"
+pytest-cov = "^4.0"
+coverage = {version = "^7.0", extras = ["toml"]}
+codecov = "^2.1"
+black = "^23.1.0"
+
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/marcaurele/gce-ipx800/issues"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7,<9"
-pytest-cov = ">=4,<6"
-coverage = {version = "^7.0", extras = ["toml"]}
-codecov = "^2.1"
-black = ">=23.1,<25.0"
-ruff = ">=0.0.292,<0.3.5"
+ruff = "^0.0.292"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-target-version = ["py38", "py39", "py310", "py311", "py312"]
+target-version = ["py38", "py39", "py310"]
 line-length = 79
 
 [tool.coverage.report]
 exclude_lines = ["def __repr__"]
```

### Comparing `gce_ipx800-0.6.0/PKG-INFO` & `gce_ipx800-0.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gce-ipx800
-Version: 0.6.0
+Version: 0.6.dev0
 Summary: Library to interact with the GCE Electronics IPX800 device
 Home-page: https://github.com/marcaurele/gce-ipx800
 License: Apache-2.0
 Keywords: ipx800,GCE-Electronics,GCE,home-automation
 Author: Marc-Aurèle Brothier
 Author-email: m@brothier.org
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Dist: requests (>=2.26,<3.0)
 Project-URL: Bug Tracker, https://github.com/marcaurele/gce-ipx800/issues
 Project-URL: Repository, https://github.com/marcaurele/gce-ipx800
 Description-Content-Type: text/x-rst
 
@@ -86,15 +85,15 @@
 
     r4.status  # => return a Boolean
 
     r4.on()
 
     r4.off()
 
-    r4.toggle()
+    r4.togle()
 
     len(ipx.relays)  # => 56
 
 Links
 -----
 
 * GCE IPX800 V4 API: https://gce.ovh/wiki/index.php?title=API_V4
```

