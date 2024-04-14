# Comparing `tmp/pdfToAudio-1.0.0.tar.gz` & `tmp/pdfToAudio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfToAudio-1.0.0.tar", last modified: Sun Apr 14 21:33:33 2024, max compression
+gzip compressed data, was "pdfToAudio-1.0.1.tar", last modified: Sun Apr 14 21:51:10 2024, max compression
```

## Comparing `pdfToAudio-1.0.0.tar` & `pdfToAudio-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-04-14 21:33:33.272133 pdfToAudio-1.0.0/
--rw-r--r--   0 thiagoadriano   (501) staff       (20)     1210 2024-04-14 21:33:33.271976 pdfToAudio-1.0.0/PKG-INFO
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      925 2024-04-14 21:32:35.000000 pdfToAudio-1.0.0/README.md
-drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-04-14 21:33:33.271100 pdfToAudio-1.0.0/pdfToAudio/
--rw-r--r--   0 thiagoadriano   (501) staff       (20)       36 2024-04-14 10:00:41.000000 pdfToAudio-1.0.0/pdfToAudio/__init__.py
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      318 2024-04-14 10:03:16.000000 pdfToAudio-1.0.0/pdfToAudio/pdf_to_audio.py
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      831 2024-04-14 10:04:15.000000 pdfToAudio-1.0.0/pdfToAudio/tests_pdf_to_audio.py
-drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-04-14 21:33:33.271754 pdfToAudio-1.0.0/pdfToAudio.egg-info/
--rw-r--r--   0 thiagoadriano   (501) staff       (20)     1210 2024-04-14 21:33:33.000000 pdfToAudio-1.0.0/pdfToAudio.egg-info/PKG-INFO
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      237 2024-04-14 21:33:33.000000 pdfToAudio-1.0.0/pdfToAudio.egg-info/SOURCES.txt
--rw-r--r--   0 thiagoadriano   (501) staff       (20)        1 2024-04-14 21:33:33.000000 pdfToAudio-1.0.0/pdfToAudio.egg-info/dependency_links.txt
--rw-r--r--   0 thiagoadriano   (501) staff       (20)       11 2024-04-14 21:33:33.000000 pdfToAudio-1.0.0/pdfToAudio.egg-info/top_level.txt
--rw-r--r--   0 thiagoadriano   (501) staff       (20)       38 2024-04-14 21:33:33.272304 pdfToAudio-1.0.0/setup.cfg
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      527 2024-04-14 10:09:22.000000 pdfToAudio-1.0.0/setup.py
+drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-04-14 21:51:10.708979 pdfToAudio-1.0.1/
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)     1274 2024-04-14 21:51:10.708845 pdfToAudio-1.0.1/PKG-INFO
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      989 2024-04-14 21:42:02.000000 pdfToAudio-1.0.1/README.md
+drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-04-14 21:51:10.707919 pdfToAudio-1.0.1/pdfToAudio/
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)       36 2024-04-14 10:00:41.000000 pdfToAudio-1.0.1/pdfToAudio/__init__.py
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      318 2024-04-14 10:03:16.000000 pdfToAudio-1.0.1/pdfToAudio/pdf_to_audio.py
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      831 2024-04-14 10:04:15.000000 pdfToAudio-1.0.1/pdfToAudio/tests_pdf_to_audio.py
+drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-04-14 21:51:10.708685 pdfToAudio-1.0.1/pdfToAudio.egg-info/
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)     1274 2024-04-14 21:51:10.000000 pdfToAudio-1.0.1/pdfToAudio.egg-info/PKG-INFO
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      270 2024-04-14 21:51:10.000000 pdfToAudio-1.0.1/pdfToAudio.egg-info/SOURCES.txt
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)        1 2024-04-14 21:51:10.000000 pdfToAudio-1.0.1/pdfToAudio.egg-info/dependency_links.txt
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)       25 2024-04-14 21:51:10.000000 pdfToAudio-1.0.1/pdfToAudio.egg-info/requires.txt
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)       11 2024-04-14 21:51:10.000000 pdfToAudio-1.0.1/pdfToAudio.egg-info/top_level.txt
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)       38 2024-04-14 21:51:10.709032 pdfToAudio-1.0.1/setup.cfg
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      603 2024-04-14 21:51:07.000000 pdfToAudio-1.0.1/setup.py
```

### Comparing `pdfToAudio-1.0.0/PKG-INFO` & `pdfToAudio-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfToAudio
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package creates audiobooks from PDF files
 Home-page: https://github.com/programadriano/is-even
 Author: Thiago S Adriano
 Author-email: prof.thiagoadriano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -16,18 +16,25 @@
 ## Features
 * Convert PDFs to audio: Turn any PDF document into an audio file.
 * Multi-language support: Uses Google's Text-to-Speech which supports various languages.
 
 
 ## Installation
 Install from PyPI with pip:
-
 ```bash
 pip install pdfToAudio
 ```
+
+## Requiriments
+
+```bash
+pip install gTTS pypdf PdfReader
+```
+
+
 ## Quick Start
 
 
 Here is how you can use the pdf_to_audio function to convert a PDF document into an audio file:
 
 
 ```bash
```

### Comparing `pdfToAudio-1.0.0/README.md` & `pdfToAudio-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,25 @@
 ## Features
 * Convert PDFs to audio: Turn any PDF document into an audio file.
 * Multi-language support: Uses Google's Text-to-Speech which supports various languages.
 
 
 ## Installation
 Install from PyPI with pip:
-
 ```bash
 pip install pdfToAudio
 ```
+
+## Requiriments
+
+```bash
+pip install gTTS pypdf PdfReader
+```
+
+
 ## Quick Start
 
 
 Here is how you can use the pdf_to_audio function to convert a PDF document into an audio file:
 
 
 ```bash
```

### Comparing `pdfToAudio-1.0.0/pdfToAudio/tests_pdf_to_audio.py` & `pdfToAudio-1.0.1/pdfToAudio/tests_pdf_to_audio.py`

 * *Files identical despite different names*

### Comparing `pdfToAudio-1.0.0/pdfToAudio.egg-info/PKG-INFO` & `pdfToAudio-1.0.1/pdfToAudio.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfToAudio
-Version: 1.0.0
+Version: 1.0.1
 Summary: This package creates audiobooks from PDF files
 Home-page: https://github.com/programadriano/is-even
 Author: Thiago S Adriano
 Author-email: prof.thiagoadriano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
@@ -16,18 +16,25 @@
 ## Features
 * Convert PDFs to audio: Turn any PDF document into an audio file.
 * Multi-language support: Uses Google's Text-to-Speech which supports various languages.
 
 
 ## Installation
 Install from PyPI with pip:
-
 ```bash
 pip install pdfToAudio
 ```
+
+## Requiriments
+
+```bash
+pip install gTTS pypdf PdfReader
+```
+
+
 ## Quick Start
 
 
 Here is how you can use the pdf_to_audio function to convert a PDF document into an audio file:
 
 
 ```bash
```

### Comparing `pdfToAudio-1.0.0/setup.py` & `pdfToAudio-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='pdfToAudio',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     description='This package creates audiobooks from PDF files',
     author='Thiago S Adriano',
     author_email='prof.thiagoadriano@gmail.com',
+    install_requires=[
+        'gTTS==2.2.3',
+        'pypdf==2.4.0'
+    ],
     url='https://github.com/programadriano/is-even',  
     license='MIT',  
     long_description=long_description,
     long_description_content_type='text/markdown' 
 )
```

