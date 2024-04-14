# Comparing `tmp/s360tools-0.1.8.tar.gz` & `tmp/s360tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s360tools-0.1.8.tar", last modified: Mon Feb 26 08:27:32 2024, max compression
+gzip compressed data, was "s360tools-0.1.9.tar", last modified: Tue Mar 19 09:02:36 2024, max compression
```

## Comparing `s360tools-0.1.8.tar` & `s360tools-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 08:27:32.212079 s360tools-0.1.8/
--rw-rw-rw-   0        0        0     1091 2024-01-09 13:37:25.000000 s360tools-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      474 2024-02-26 08:27:32.212079 s360tools-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      545 2024-02-26 08:25:45.000000 s360tools-0.1.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-02-26 08:27:32.138316 s360tools-0.1.8/s360tools/
--rw-rw-rw-   0        0        0       28 2024-01-12 08:07:47.000000 s360tools-0.1.8/s360tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-26 08:27:32.209443 s360tools-0.1.8/s360tools/logger/
--rw-rw-rw-   0        0        0       36 2024-01-16 13:04:39.000000 s360tools-0.1.8/s360tools/logger/__init__.py
--rw-rw-rw-   0        0        0     5314 2024-01-16 17:00:47.000000 s360tools-0.1.8/s360tools/logger/errormessenger.py
-drwxrwxrwx   0        0        0        0 2024-02-26 08:27:32.210443 s360tools-0.1.8/s360tools/sheets/
--rw-rw-rw-   0        0        0      146 2024-01-09 16:19:22.000000 s360tools-0.1.8/s360tools/sheets/__init__.py
--rw-rw-rw-   0        0        0    12404 2024-02-26 08:25:30.000000 s360tools-0.1.8/s360tools/sheets/sheethandler.py
-drwxrwxrwx   0        0        0        0 2024-02-26 08:27:32.211443 s360tools-0.1.8/s360tools.egg-info/
--rw-rw-rw-   0        0        0      474 2024-02-26 08:27:32.000000 s360tools-0.1.8/s360tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-02-26 08:27:32.000000 s360tools-0.1.8/s360tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 08:27:32.000000 s360tools-0.1.8/s360tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-02-26 08:27:32.000000 s360tools-0.1.8/s360tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-26 08:27:32.000000 s360tools-0.1.8/s360tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 08:27:32.212079 s360tools-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-19 09:02:36.136610 s360tools-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2024-01-09 13:37:25.000000 s360tools-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      474 2024-03-19 09:02:36.135611 s360tools-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2024-03-19 09:02:19.000000 s360tools-0.1.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-03-19 09:02:36.125864 s360tools-0.1.9/s360tools/
+-rw-rw-rw-   0        0        0       28 2024-01-12 08:07:47.000000 s360tools-0.1.9/s360tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-19 09:02:36.131610 s360tools-0.1.9/s360tools/logger/
+-rw-rw-rw-   0        0        0       36 2024-01-16 13:04:39.000000 s360tools-0.1.9/s360tools/logger/__init__.py
+-rw-rw-rw-   0        0        0     5314 2024-01-16 17:00:47.000000 s360tools-0.1.9/s360tools/logger/errormessenger.py
+drwxrwxrwx   0        0        0        0 2024-03-19 09:02:36.134610 s360tools-0.1.9/s360tools/sheets/
+-rw-rw-rw-   0        0        0      146 2024-01-09 16:19:22.000000 s360tools-0.1.9/s360tools/sheets/__init__.py
+-rw-rw-rw-   0        0        0    12365 2024-03-19 09:01:59.000000 s360tools-0.1.9/s360tools/sheets/sheethandler.py
+drwxrwxrwx   0        0        0        0 2024-03-19 09:02:36.135611 s360tools-0.1.9/s360tools.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-03-19 09:02:36.000000 s360tools-0.1.9/s360tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-03-19 09:02:36.000000 s360tools-0.1.9/s360tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-19 09:02:36.000000 s360tools-0.1.9/s360tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-03-19 09:02:36.000000 s360tools-0.1.9/s360tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-03-19 09:02:36.000000 s360tools-0.1.9/s360tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-19 09:02:36.136610 s360tools-0.1.9/setup.cfg
```

### Comparing `s360tools-0.1.8/LICENSE.txt` & `s360tools-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `s360tools-0.1.8/pyproject.toml` & `s360tools-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0" ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s360tools"
-version = "0.1.8"
+version = "0.1.9"
 description = "A collection of simple tools for SEO analysis for s360"
 authors = [
     { name="Mikkel Almind" },
     { name="Mikkel Almind", email="mje@s360digital.com" }
 ]
 requires-python = ">=3.10.12"
 classifiers = ["License :: OSI Approved :: MIT License"]
```

### Comparing `s360tools-0.1.8/s360tools/logger/errormessenger.py` & `s360tools-0.1.9/s360tools/logger/errormessenger.py`

 * *Files identical despite different names*

### Comparing `s360tools-0.1.8/s360tools/sheets/sheethandler.py` & `s360tools-0.1.9/s360tools/sheets/sheethandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,18 @@
         ]
     )
 
     if "google.colab" in str(get_ipython()):
         # Authenticating in Google Colab
         auth.authenticate_user()
         google_client = gspread.authorize(credentials)
-    elif "GCF_RUNTIME" in os.environ:
+    else:
         # Authenticating in Google Cloud Function
         google_client = gspread.Client(auth=credentials)
         google_client.session = AuthorizedSession(credentials)
-    else:
         raise EnvironmentError("Unknown environment, cannot authorize")
     return google_client
 
 class SheetHandler:
     """
     Wrapper object for ease of interacting with the gspread sheet api
     """
```

