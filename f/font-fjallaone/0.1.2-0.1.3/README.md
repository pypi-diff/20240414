# Comparing `tmp/font_fjallaone-0.1.2.tar.gz` & `tmp/font_fjallaone-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "font_fjallaone-0.1.2.tar", max compression
+gzip compressed data, was "font_fjallaone-0.1.3.tar", max compression
```

## Comparing `font_fjallaone-0.1.2.tar` & `font_fjallaone-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1906 2022-12-30 11:49:11.672277 font_fjallaone-0.1.2/README.md
--rw-r--r--   0        0        0      472 2022-12-30 11:49:11.672277 font_fjallaone-0.1.2/font_fjallaone/__init__.py
--rw-r--r--   0        0        0    34848 2022-12-30 11:49:11.672277 font_fjallaone-0.1.2/font_fjallaone/files/FjallaOne-Regular.ttf
--rw-r--r--   0        0        0     1265 2022-12-30 11:49:45.292531 font_fjallaone-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 font_fjallaone-0.1.2/setup.py
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 font_fjallaone-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1904 2024-04-14 19:35:55.250742 font_fjallaone-0.1.3/README.md
+-rw-r--r--   0        0        0      472 2024-04-14 19:35:55.250742 font_fjallaone-0.1.3/font_fjallaone/__init__.py
+-rw-r--r--   0        0        0    34848 2024-04-14 19:35:55.250742 font_fjallaone-0.1.3/font_fjallaone/files/FjallaOne-Regular.ttf
+-rw-r--r--   0        0        0     1460 2024-04-14 19:36:13.439016 font_fjallaone-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 font_fjallaone-0.1.3/PKG-INFO
```

### Comparing `font_fjallaone-0.1.2/README.md` & `font_fjallaone-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ```bash
 pip install font_fjallaone
 ```
 
 ## Usage
 
 ```python
-from font_fjallaone import FjallaOne
+import font_fjallaone as FjallaOne
 ```
 
 ## Release Management
 
 The CI/CD setup uses semantic commit messages following the [conventional commits standard](https://www.conventionalcommits.org/en/v1.0.0/).
 There is a GitHub Action in [.github/workflows/semantic-release.yaml](./.github/workflows/semantic-release.yaml)
 that uses [go-semantic-commit](https://go-semantic-release.xyz/) to create new
```

### Comparing `font_fjallaone-0.1.2/font_fjallaone/files/FjallaOne-Regular.ttf` & `font_fjallaone-0.1.3/font_fjallaone/files/FjallaOne-Regular.ttf`

 * *Files identical despite different names*

### Comparing `font_fjallaone-0.1.2/PKG-INFO` & `font_fjallaone-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: font-fjallaone
-Version: 0.1.2
+Version: 0.1.3
 Summary: Fjalla One from from Sorkin Type as distributed by Google Fonts
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Python Package with Fjalla One Font
 
 Python Package with [Fjalla One](https://fonts.google.com/specimen/Fjalla+One) from
 [Sorkin Type](https://github.com/pimoroni/fonts-python) as distributed by
 [Google Fonts](https://fonts.google.com) for use with
@@ -23,15 +24,15 @@
 ```bash
 pip install font_fjallaone
 ```
 
 ## Usage
 
 ```python
-from font_fjallaone import FjallaOne
+import font_fjallaone as FjallaOne
 ```
 
 ## Release Management
 
 The CI/CD setup uses semantic commit messages following the [conventional commits standard](https://www.conventionalcommits.org/en/v1.0.0/).
 There is a GitHub Action in [.github/workflows/semantic-release.yaml](./.github/workflows/semantic-release.yaml)
 that uses [go-semantic-commit](https://go-semantic-release.xyz/) to create new
```

