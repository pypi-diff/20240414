# Comparing `tmp/pdf_compression-0.1.0.tar.gz` & `tmp/pdf_compression-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_compression-0.1.0.tar", last modified: Sun Apr 14 06:50:16 2024, max compression
+gzip compressed data, was "pdf_compression-0.1.1.tar", last modified: Sun Apr 14 11:12:03 2024, max compression
```

## Comparing `pdf_compression-0.1.0.tar` & `pdf_compression-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 06:50:16.588208 pdf_compression-0.1.0/
--rw-rw-rw-   0        0        0      321 2024-04-14 06:50:16.582409 pdf_compression-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-22 11:15:17.000000 pdf_compression-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 06:50:16.537038 pdf_compression-0.1.0/pdf_compression/
-drwxrwxrwx   0        0        0        0 2024-04-14 06:50:16.566012 pdf_compression-0.1.0/pdf_compression/pdf_compression.egg-info/
--rw-rw-rw-   0        0        0      321 2024-04-14 06:50:16.000000 pdf_compression-0.1.0/pdf_compression/pdf_compression.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2024-04-14 06:50:16.000000 pdf_compression-0.1.0/pdf_compression/pdf_compression.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 06:50:16.000000 pdf_compression-0.1.0/pdf_compression/pdf_compression.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-14 06:50:16.000000 pdf_compression-0.1.0/pdf_compression/pdf_compression.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 06:50:16.000000 pdf_compression-0.1.0/pdf_compression/pdf_compression.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 06:50:16.588208 pdf_compression-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      618 2024-04-13 19:04:21.000000 pdf_compression-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:50:16.582409 pdf_compression-0.1.0/tests/
--rw-rw-rw-   0        0        0      351 2024-04-14 06:31:31.000000 pdf_compression-0.1.0/tests/test_empty.py
--rw-rw-rw-   0        0        0      379 2024-04-14 06:31:55.000000 pdf_compression-0.1.0/tests/test_nonexisting.py
--rw-rw-rw-   0        0        0      348 2024-04-14 06:02:06.000000 pdf_compression-0.1.0/tests/test_nonpdf.py
--rw-rw-rw-   0        0        0      380 2024-04-14 06:02:12.000000 pdf_compression-0.1.0/tests/test_protected_with_pass.py
--rw-rw-rw-   0        0        0      486 2024-04-14 06:03:53.000000 pdf_compression-0.1.0/tests/test_protected_with_wrong_pass.py
--rw-rw-rw-   0        0        0      476 2024-04-14 06:05:21.000000 pdf_compression-0.1.0/tests/test_protected_without_pass.py
--rw-rw-rw-   0        0        0      357 2024-04-14 06:02:27.000000 pdf_compression-0.1.0/tests/test_with_outfile.py
--rw-rw-rw-   0        0        0      353 2024-04-14 06:02:44.000000 pdf_compression-0.1.0/tests/test_without_outfile.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:12:03.972832 pdf_compression-0.1.1/
+-rw-rw-rw-   0        0        0      321 2024-04-14 11:12:03.972832 pdf_compression-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-22 11:15:17.000000 pdf_compression-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 11:12:03.921003 pdf_compression-0.1.1/pdf_compression/
+-rw-rw-rw-   0        0        0        0 2024-03-22 11:15:18.000000 pdf_compression-0.1.1/pdf_compression/__init__.py
+-rw-rw-rw-   0        0        0     3381 2024-04-14 06:17:24.000000 pdf_compression-0.1.1/pdf_compression/compress_pdf.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:12:03.951205 pdf_compression-0.1.1/pdf_compression.egg-info/
+-rw-rw-rw-   0        0        0      321 2024-04-14 11:12:03.000000 pdf_compression-0.1.1/pdf_compression.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-04-14 11:12:03.000000 pdf_compression-0.1.1/pdf_compression.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 11:12:03.000000 pdf_compression-0.1.1/pdf_compression.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-14 11:12:03.000000 pdf_compression-0.1.1/pdf_compression.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-04-14 11:12:03.000000 pdf_compression-0.1.1/pdf_compression.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 11:12:03.981216 pdf_compression-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      552 2024-04-14 11:11:47.000000 pdf_compression-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 11:12:03.972832 pdf_compression-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 11:15:19.000000 pdf_compression-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-04-14 06:31:31.000000 pdf_compression-0.1.1/tests/test_empty.py
+-rw-rw-rw-   0        0        0      379 2024-04-14 06:31:55.000000 pdf_compression-0.1.1/tests/test_nonexisting.py
+-rw-rw-rw-   0        0        0      348 2024-04-14 06:02:06.000000 pdf_compression-0.1.1/tests/test_nonpdf.py
+-rw-rw-rw-   0        0        0      380 2024-04-14 06:02:12.000000 pdf_compression-0.1.1/tests/test_protected_with_pass.py
+-rw-rw-rw-   0        0        0      486 2024-04-14 06:03:53.000000 pdf_compression-0.1.1/tests/test_protected_with_wrong_pass.py
+-rw-rw-rw-   0        0        0      476 2024-04-14 06:05:21.000000 pdf_compression-0.1.1/tests/test_protected_without_pass.py
+-rw-rw-rw-   0        0        0      357 2024-04-14 06:02:27.000000 pdf_compression-0.1.1/tests/test_with_outfile.py
+-rw-rw-rw-   0        0        0      353 2024-04-14 06:02:44.000000 pdf_compression-0.1.1/tests/test_without_outfile.py
```

### Comparing `pdf_compression-0.1.0/pdf_compression/pdf_compression.egg-info/SOURCES.txt` & `pdf_compression-0.1.1/pdf_compression.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 README.md
 setup.py
-pdf_compression/pdf_compression.egg-info/PKG-INFO
-pdf_compression/pdf_compression.egg-info/SOURCES.txt
-pdf_compression/pdf_compression.egg-info/dependency_links.txt
-pdf_compression/pdf_compression.egg-info/requires.txt
-pdf_compression/pdf_compression.egg-info/top_level.txt
+pdf_compression/__init__.py
+pdf_compression/compress_pdf.py
+pdf_compression.egg-info/PKG-INFO
+pdf_compression.egg-info/SOURCES.txt
+pdf_compression.egg-info/dependency_links.txt
+pdf_compression.egg-info/requires.txt
+pdf_compression.egg-info/top_level.txt
+tests/__init__.py
 tests/test_empty.py
 tests/test_nonexisting.py
 tests/test_nonpdf.py
 tests/test_protected_with_pass.py
 tests/test_protected_with_wrong_pass.py
 tests/test_protected_without_pass.py
 tests/test_with_outfile.py
```

### Comparing `pdf_compression-0.1.0/setup.py` & `pdf_compression-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pdf_compression',
-    package_dir = {"": "pdf_compression"},
-    packages=find_packages(where="pdf_compression"),
-    version='0.1.0',
+    packages=find_packages(),
+    version='0.1.1',
     description='A PDF compression library',
     long_description="A PDF compression library built upon PyMuPDF and Pillow. Quick, free of cost and open source.",
     author='Nishtha',
     author_email = 'nishthachitalia0309@gmail.com',
     license='MIT',
     install_requires=['pillow', 'pymupdf'],
     keywords=['python', 'pdf', 'compression', 'pdf_compression'],
```

