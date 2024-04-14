# Comparing `tmp/thepipe_api-0.1.3.tar.gz` & `tmp/thepipe_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.1.3.tar", last modified: Sat Apr 13 19:50:04 2024, max compression
+gzip compressed data, was "thepipe_api-0.1.4.tar", last modified: Sat Apr 13 20:49:26 2024, max compression
```

## Comparing `thepipe_api-0.1.3.tar` & `thepipe_api-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 19:50:04.337923 thepipe_api-0.1.3/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     9603 2024-04-13 19:50:04.336924 thepipe_api-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     8534 2024-04-13 17:32:17.000000 thepipe_api-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-13 19:50:04.337923 thepipe_api-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      740 2024-04-13 19:49:58.000000 thepipe_api-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:50:04.313921 thepipe_api-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0     9511 2024-04-13 18:51:15.000000 thepipe_api-0.1.3/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:50:04.317921 thepipe_api-0.1.3/thepipe_api/
--rw-rw-rw-   0        0        0       48 2024-04-13 19:44:21.000000 thepipe_api-0.1.3/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 18:49:04.000000 thepipe_api-0.1.3/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2835 2024-04-13 18:07:10.000000 thepipe_api-0.1.3/thepipe_api/core.py
--rw-rw-rw-   0        0        0    19468 2024-04-13 18:50:12.000000 thepipe_api-0.1.3/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3504 2024-04-13 19:44:28.000000 thepipe_api-0.1.3/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-13 19:50:04.335923 thepipe_api-0.1.3/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9603 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      256 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 19:50:04.000000 thepipe_api-0.1.3/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 20:49:26.456596 thepipe_api-0.1.4/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     9329 2024-04-13 20:49:26.455596 thepipe_api-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8603 2024-04-13 20:45:01.000000 thepipe_api-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 20:49:26.456596 thepipe_api-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      740 2024-04-13 20:49:14.000000 thepipe_api-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:49:26.432596 thepipe_api-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     9523 2024-04-13 20:12:45.000000 thepipe_api-0.1.4/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:49:26.437606 thepipe_api-0.1.4/thepipe_api/
+-rw-rw-rw-   0        0        0       48 2024-04-13 19:44:21.000000 thepipe_api-0.1.4/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.4/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2835 2024-04-13 18:07:10.000000 thepipe_api-0.1.4/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19616 2024-04-13 20:47:49.000000 thepipe_api-0.1.4/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3504 2024-04-13 20:43:49.000000 thepipe_api-0.1.4/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:49:26.454603 thepipe_api-0.1.4/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9329 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.1.3/LICENSE` & `thepipe_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.3/PKG-INFO` & `thepipe_api-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.8.3
-Requires-Dist: charset-normalizer<3.0,>=2.0
-Requires-Dist: playwright
-Requires-Dist: docx2txt
-Requires-Dist: python-pptx
+Requires-Dist: aiohttp
+Requires-Dist: charset-normalizer
 Requires-Dist: Pyarrow
-Requires-Dist: unstructured[all-docs]
-Requires-Dist: poppler-utils
 Requires-Dist: python-magic
-Requires-Dist: magika
-Requires-Dist: pandas
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: pillow
-Requires-Dist: pytesseract
 Requires-Dist: cssutils
 Requires-Dist: beautifulsoup4
-Requires-Dist: torch
-Requires-Dist: llmlingua
 Requires-Dist: PyMuPDF
-Requires-Dist: pdf2image
-Requires-Dist: python-magic
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
 
 ### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
 
 The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
@@ -96,19 +84,19 @@
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## Installation 📦
 
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the python requirements:
+To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
 
 ```bash
 git clone https://github.com/emcf/thepipe
-pip install -r requirements.txt
+pip install -r requirements_local.txt
 ```
 
 Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
 
 Now you can use The Pipe:
 ```bash
 python thepipe.py path/to/directory
```

#### html2text {}

```diff
@@ -1,25 +1,20 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.3 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.4 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-aiohttp==3.8.3 Requires-Dist: charset-normalizer<3.0,>=2.0 Requires-Dist:
-playwright Requires-Dist: docx2txt Requires-Dist: python-pptx Requires-Dist:
-Pyarrow Requires-Dist: unstructured[all-docs] Requires-Dist: poppler-utils
-Requires-Dist: python-magic Requires-Dist: magika Requires-Dist: pandas
-Requires-Dist: colorama Requires-Dist: requests Requires-Dist: pillow Requires-
-Dist: pytesseract Requires-Dist: cssutils Requires-Dist: beautifulsoup4
-Requires-Dist: torch Requires-Dist: llmlingua Requires-Dist: PyMuPDF Requires-
-Dist: pdf2image Requires-Dist: python-magic # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/
-badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
-badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
+python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
+pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
+PyMuPDF # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e [![codecov](https://codecov.io/gh/
+emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/
+thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/
+python-ci.yml/badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_A_p_p_l_y_%_2_0_h_e_r_e_-_b_l_u_e_) ### Prepare PDFs, word
 docs, slides, web pages and more for Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision
 language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG
 applications that require a deep understanding of complex sources. The Pipe is
 available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone
@@ -82,26 +77,26 @@
 with image (or images if scrollable); text-only extraction available | | GitHub
 Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
 repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
 âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
 ## Installation ð¦ ## Local Installation ð ï¸ To use The Pipe locally, you
 will need [playwright](https://github.com/microsoft/playwright), [ctags](https:
 //github.com/universal-ctags/), [pytesseract](https://github.com/h/
-pytesseract), and the python requirements: ```bash git clone https://
-github.com/emcf/thepipe pip install -r requirements.txt ``` Tip for windows
-users: you may need to install the python-libmagic binaries with `pip install
-python-magic-bin`. Now you can use The Pipe: ```bash python thepipe.py path/to/
-directory ``` This command will process all supported files within the
-specified directory, compressing any information over the token limit if
-necessary, and outputting the resulting prompt and images to a folder.
-Arguments are: - The input source (required): can be a file path, a URL, or a
-directory path. - `--local` (optional): Use the local version of The Pipe
-instead of the hosted API. - `--match` (optional): Regex pattern to match files
-in the directory. - `--ignore` (optional): Regex pattern to ignore files in the
-directory. - `--limit` (optional): The token limit for the output prompt,
-defaults to 100K. Prompts exceeding the limit will be compressed. - `--
-ai_extraction` (optional): Extract tables, figures, and math from PDFs using
-our extractor. Incurs extra costs. - `--text_only` (optional): Do not extract
-images from documents or websites. Additionally, image files will be
-represented with OCR instead of as images. ![Demo](https://
-ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
-demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
+pytesseract), and the local python requirements, which differ from the more
+lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
+pip install -r requirements_local.txt ``` Tip for windows users: you may need
+to install the python-libmagic binaries with `pip install python-magic-bin`.
+Now you can use The Pipe: ```bash python thepipe.py path/to/directory ``` This
+command will process all supported files within the specified directory,
+compressing any information over the token limit if necessary, and outputting
+the resulting prompt and images to a folder. Arguments are: - The input source
+(required): can be a file path, a URL, or a directory path. - `--local`
+(optional): Use the local version of The Pipe instead of the hosted API. - `--
+match` (optional): Regex pattern to match files in the directory. - `--ignore`
+(optional): Regex pattern to ignore files in the directory. - `--limit`
+(optional): The token limit for the output prompt, defaults to 100K. Prompts
+exceeding the limit will be compressed. - `--ai_extraction` (optional): Extract
+tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
+`--text_only` (optional): Do not extract images from documents or websites.
+Additionally, image files will be represented with OCR instead of as images. !
+[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
```

### Comparing `thepipe_api-0.1.3/README.md` & `thepipe_api-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## Installation 📦
 
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the python requirements:
+To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
 
 ```bash
 git clone https://github.com/emcf/thepipe
-pip install -r requirements.txt
+pip install -r requirements_local.txt
 ```
 
 Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
 
 Now you can use The Pipe:
 ```bash
 python thepipe.py path/to/directory
```

#### html2text {}

```diff
@@ -68,26 +68,26 @@
 with image (or images if scrollable); text-only extraction available | | GitHub
 Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
 repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
 âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
 ## Installation ð¦ ## Local Installation ð ï¸ To use The Pipe locally, you
 will need [playwright](https://github.com/microsoft/playwright), [ctags](https:
 //github.com/universal-ctags/), [pytesseract](https://github.com/h/
-pytesseract), and the python requirements: ```bash git clone https://
-github.com/emcf/thepipe pip install -r requirements.txt ``` Tip for windows
-users: you may need to install the python-libmagic binaries with `pip install
-python-magic-bin`. Now you can use The Pipe: ```bash python thepipe.py path/to/
-directory ``` This command will process all supported files within the
-specified directory, compressing any information over the token limit if
-necessary, and outputting the resulting prompt and images to a folder.
-Arguments are: - The input source (required): can be a file path, a URL, or a
-directory path. - `--local` (optional): Use the local version of The Pipe
-instead of the hosted API. - `--match` (optional): Regex pattern to match files
-in the directory. - `--ignore` (optional): Regex pattern to ignore files in the
-directory. - `--limit` (optional): The token limit for the output prompt,
-defaults to 100K. Prompts exceeding the limit will be compressed. - `--
-ai_extraction` (optional): Extract tables, figures, and math from PDFs using
-our extractor. Incurs extra costs. - `--text_only` (optional): Do not extract
-images from documents or websites. Additionally, image files will be
-represented with OCR instead of as images. ![Demo](https://
-ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
-demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
+pytesseract), and the local python requirements, which differ from the more
+lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
+pip install -r requirements_local.txt ``` Tip for windows users: you may need
+to install the python-libmagic binaries with `pip install python-magic-bin`.
+Now you can use The Pipe: ```bash python thepipe.py path/to/directory ``` This
+command will process all supported files within the specified directory,
+compressing any information over the token limit if necessary, and outputting
+the resulting prompt and images to a folder. Arguments are: - The input source
+(required): can be a file path, a URL, or a directory path. - `--local`
+(optional): Use the local version of The Pipe instead of the hosted API. - `--
+match` (optional): Regex pattern to match files in the directory. - `--ignore`
+(optional): Regex pattern to ignore files in the directory. - `--limit`
+(optional): The token limit for the output prompt, defaults to 100K. Prompts
+exceeding the limit will be compressed. - `--ai_extraction` (optional): Extract
+tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
+`--text_only` (optional): Do not extract images from documents or websites.
+Additionally, image files will be represented with OCR instead of as images. !
+[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
```

### Comparing `thepipe_api-0.1.3/setup.py` & `thepipe_api-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.1.3',
+    version='0.1.4',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.1.3/tests/test_thepipe.py` & `thepipe_api-0.1.4/tests/test_thepipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         self.assertIn('Hello, World!', text)
         # test with images
         chunks = extractor.extract_from_source(source=self.files_directory+"/example.jpg")
         thepipe.save_outputs(chunks)
         self.assertTrue(any('.jpg' in f for f in os.listdir(self.outputs_directory)))
 
     def test_extract(self):
-        chunks = thepipe.extract(source=self.files_directory+"/example.md")
+        chunks = thepipe.extract(source=self.files_directory+"/example.md", local=True)
         self.assertEqual(type(chunks), list)
         self.assertNotEqual(len(chunks), 0)
         self.assertEqual(type(chunks[0]), dict)
         # verify it still contains vital information from the markdown file
         self.assertIn('markdown', str(chunks).lower())
 
     def test_extract_api(self):
```

### Comparing `thepipe_api-0.1.3/thepipe_api/compressor.py` & `thepipe_api-0.1.4/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.3/thepipe_api/core.py` & `thepipe_api-0.1.4/thepipe_api/core.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.3/thepipe_api/extractor.py` & `thepipe_api-0.1.4/thepipe_api/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,21 @@
 import re
 from typing import Dict, List, Optional
 import glob
 import os
 import tempfile
 from urllib.parse import urlparse
 import zipfile
-import pandas as pd
 from PIL import Image
 import requests
 import json
-from playwright.sync_api import sync_playwright
 import fitz
 from .core import Chunk, print_status, SourceTypes, create_chunks_from_messages, API_URL
-import docx2txt
 import tempfile
-from pptx import Presentation
-from pptx.enum.shapes import MSO_SHAPE_TYPE
 import mimetypes
-from magika import Magika
 
 FILES_TO_IGNORE = {'package-lock.json', '.gitignore', '.bin', '.pyc', '.pyo', '.exe', '.bat', '.dll', '.obj', '.o', '.a', '.lib', '.so', '.dylib', '.ncb', '.sdf', '.suo', '.pdb', '.idb', '.pyd', '.ipynb_checkpoints', '.npy', '.pth'} # Files to ignore, please feel free to customize!
 CODE_EXTENSIONS = {'.h', '.json', '.js', '.jsx', '.ts', '.tsx',  '.cs', '.java', '.html', '.css', '.ini', '.xml', '.yaml', '.xaml', '.sh'} # Plaintext files that should not be compressed with LLMLingua
 CTAGS_CODE_EXTENSIONS = {'.c', '.cpp', '.py'} # code files that work with ctags
 PLAINTEXT_EXTENSIONS = {'.txt', '.md', '.rtf'}
 IMAGE_EXTENSIONS = {'.jpg', '.jpeg', '.png'}
 SPREADSHEET_EXTENSIONS = {'.csv', '.xls', '.xlsx'}
@@ -42,15 +36,15 @@
     if source_type == SourceTypes.DIR or source == '.' or source == './':
         if source == '.' or source == './':
             source = os.getcwd()
         return extract_from_directory(dir_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
     elif source_type == SourceTypes.GITHUB:
         return extract_github(github_url=source, file_path='', match=match, ignore=ignore, text_only=text_only, verbose=verbose, ai_extraction=ai_extraction, branch='master')
     elif source_type == SourceTypes.URL:
-        return extract_url(url=source, text_only=text_only)
+        return extract_url(url=source, text_only=text_only, local=local)
     elif source_type == SourceTypes.ZIP:
         return extract_zip(file_path=source, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
     return extract_from_file(file_path=source, source_type=source_type, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only, local=local)
 
 def extract_from_file(file_path: str, source_type: str, verbose: bool = False, ai_extraction: bool = False, text_only: bool = False, local: bool = True) -> List[Chunk]:
     if not local:
         with open(file_path, 'rb') as f:
@@ -99,14 +93,15 @@
         return SourceTypes.ZIP
     elif os.path.isdir(source) or source == '.' or source == './':
         return SourceTypes.DIR
     # try splitting the source into a filename and extension
     _, extension = os.path.splitext(source)
     # if that fails, try to detect the file type using Magika
     if (not extension) or (extension not in KNOWN_EXTENSIONS):
+        from magika import Magika # import only if needed
         magika = Magika()
         try:
             with open(source, 'rb') as file:
                 result = magika.identify_bytes(file.read())
         except Exception as e:
             return None
         mimetype = result.output.mime_type
@@ -176,15 +171,14 @@
     if ai_extraction:
         with open(file_path, "rb") as f:
             response = requests.post(
                 url=API_URL,
                 files={'file': (file_path, f)},
                 data={'api_key': THEPIPE_API_KEY, 'ai_extraction': ai_extraction, 'text_only': text_only}
             )
-            response.raise_for_status()
             response_json = response.json()
             if 'error' in response_json:
                 raise ValueError(f"{response_json['error']}")
             messages = response_json['messages']
             chunks = create_chunks_from_messages(messages)
     else:
         # extract text and images of each page from the PDF
@@ -223,14 +217,15 @@
         import pytesseract # import only if needed
         text = pytesseract.image_to_string(img)
         return Chunk(path=file_path, text=text, image=None, source_type=SourceTypes.IMAGE)
     else:
         return Chunk(path=file_path, text=None, image=img, source_type=SourceTypes.IMAGE)
     
 def extract_spreadsheet(file_path: str) -> Chunk:
+    import pandas as pd # import only if needed
     if file_path.endswith(".csv"):
         df = pd.read_csv(file_path)
     elif file_path.endswith(".xls") or file_path.endswith(".xlsx"):
         df = pd.read_excel(file_path)
     dict = df.to_dict(orient='records')
     json_dict = json.dumps(dict, indent=4)
     return Chunk(path=file_path, text=json_dict, image=None, source_type=SourceTypes.SPREADSHEET)
@@ -253,14 +248,15 @@
             file_path = os.path.join(temp_dir, os.path.basename(url))
             response = requests.get(url)
             with open(file_path, 'wb') as file:
                 file.write(response.content)
             chunks = extract_from_source(source=file_path, text_only=text_only)
     else:
         # use playwright to extract text and images from the URL
+        from playwright.sync_api import sync_playwright # import only if needed
         with sync_playwright() as p:
             browser = p.chromium.launch()
             page = browser.new_page()
             page.goto(url)
             if not text_only:
                 # Get the viewport size and document size to scroll
                 viewport_height = page.viewport_size['height']
@@ -292,14 +288,15 @@
     with tempfile.TemporaryDirectory() as temp_dir:
         os.system(f"git clone {github_url} {temp_dir} --quiet")
         files_contents = extract_from_directory(dir_path=temp_dir, match=match, ignore=ignore, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
     return files_contents
 
 def extract_docx(file_path: str, verbose: bool = False, text_only: bool = False) -> List[Chunk]:
     # make new temp image directory
+    import docx2txt # import only if needed
     chunks = []
     temp_image_dir = tempfile.mkdtemp()
     text = docx2txt.process(file_path, temp_image_dir)
     chunks.append(Chunk(path=file_path, text=text, image=None, source_type=SourceTypes.DOCX))
     if not text_only:
         for image_name in os.listdir(temp_image_dir):
             image_path = os.path.join(temp_image_dir, image_name)
@@ -311,14 +308,16 @@
             for image_name in os.listdir(temp_image_dir):
                 image_path = os.path.join(temp_image_dir, image_name)
                 os.remove(image_path)
             os.rmdir(temp_image_dir)
     return chunks
 
 def extract_pptx(file_path: str, verbose: bool = False, text_only: bool = False) -> List[Chunk]:
+    from pptx import Presentation # import only if needed
+    from pptx.enum.shapes import MSO_SHAPE_TYPE # import only if needed
     prs = Presentation(file_path)
     chunks = []
     # parse shapes inside slides
     for slide in prs.slides:
         slide_text = ""
         slide_images = []
         for shape in slide.shapes:
```

### Comparing `thepipe_api-0.1.3/thepipe_api/thepipe.py` & `thepipe_api-0.1.4/thepipe_api/thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.3/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.1.4/thepipe_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.8.3
-Requires-Dist: charset-normalizer<3.0,>=2.0
-Requires-Dist: playwright
-Requires-Dist: docx2txt
-Requires-Dist: python-pptx
+Requires-Dist: aiohttp
+Requires-Dist: charset-normalizer
 Requires-Dist: Pyarrow
-Requires-Dist: unstructured[all-docs]
-Requires-Dist: poppler-utils
 Requires-Dist: python-magic
-Requires-Dist: magika
-Requires-Dist: pandas
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: pillow
-Requires-Dist: pytesseract
 Requires-Dist: cssutils
 Requires-Dist: beautifulsoup4
-Requires-Dist: torch
-Requires-Dist: llmlingua
 Requires-Dist: PyMuPDF
-Requires-Dist: pdf2image
-Requires-Dist: python-magic
 
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
 [![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
 
 ### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
 
 The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
@@ -96,19 +84,19 @@
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
 ## Installation 📦
 
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the python requirements:
+To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
 
 ```bash
 git clone https://github.com/emcf/thepipe
-pip install -r requirements.txt
+pip install -r requirements_local.txt
 ```
 
 Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
 
 Now you can use The Pipe:
 ```bash
 python thepipe.py path/to/directory
```

#### html2text {}

```diff
@@ -1,25 +1,20 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.3 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.4 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-aiohttp==3.8.3 Requires-Dist: charset-normalizer<3.0,>=2.0 Requires-Dist:
-playwright Requires-Dist: docx2txt Requires-Dist: python-pptx Requires-Dist:
-Pyarrow Requires-Dist: unstructured[all-docs] Requires-Dist: poppler-utils
-Requires-Dist: python-magic Requires-Dist: magika Requires-Dist: pandas
-Requires-Dist: colorama Requires-Dist: requests Requires-Dist: pillow Requires-
-Dist: pytesseract Requires-Dist: cssutils Requires-Dist: beautifulsoup4
-Requires-Dist: torch Requires-Dist: llmlingua Requires-Dist: PyMuPDF Requires-
-Dist: pdf2image Requires-Dist: python-magic # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/
-badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
-badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
+python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
+pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
+PyMuPDF # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e [![codecov](https://codecov.io/gh/
+emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/
+thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/
+python-ci.yml/badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
 _A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_A_p_p_l_y_%_2_0_h_e_r_e_-_b_l_u_e_) ### Prepare PDFs, word
 docs, slides, web pages and more for Vision-LLMs with one line of code â¡ The
 Pipe is a multimodal-first tool for feeding files and web pages into vision
 language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG
 applications that require a deep understanding of complex sources. The Pipe is
 available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone
@@ -82,26 +77,26 @@
 with image (or images if scrollable); text-only extraction available | | GitHub
 Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
 repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
 âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
 ## Installation ð¦ ## Local Installation ð ï¸ To use The Pipe locally, you
 will need [playwright](https://github.com/microsoft/playwright), [ctags](https:
 //github.com/universal-ctags/), [pytesseract](https://github.com/h/
-pytesseract), and the python requirements: ```bash git clone https://
-github.com/emcf/thepipe pip install -r requirements.txt ``` Tip for windows
-users: you may need to install the python-libmagic binaries with `pip install
-python-magic-bin`. Now you can use The Pipe: ```bash python thepipe.py path/to/
-directory ``` This command will process all supported files within the
-specified directory, compressing any information over the token limit if
-necessary, and outputting the resulting prompt and images to a folder.
-Arguments are: - The input source (required): can be a file path, a URL, or a
-directory path. - `--local` (optional): Use the local version of The Pipe
-instead of the hosted API. - `--match` (optional): Regex pattern to match files
-in the directory. - `--ignore` (optional): Regex pattern to ignore files in the
-directory. - `--limit` (optional): The token limit for the output prompt,
-defaults to 100K. Prompts exceeding the limit will be compressed. - `--
-ai_extraction` (optional): Extract tables, figures, and math from PDFs using
-our extractor. Incurs extra costs. - `--text_only` (optional): Do not extract
-images from documents or websites. Additionally, image files will be
-represented with OCR instead of as images. ![Demo](https://
-ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/
-demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
+pytesseract), and the local python requirements, which differ from the more
+lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
+pip install -r requirements_local.txt ``` Tip for windows users: you may need
+to install the python-libmagic binaries with `pip install python-magic-bin`.
+Now you can use The Pipe: ```bash python thepipe.py path/to/directory ``` This
+command will process all supported files within the specified directory,
+compressing any information over the token limit if necessary, and outputting
+the resulting prompt and images to a folder. Arguments are: - The input source
+(required): can be a file path, a URL, or a directory path. - `--local`
+(optional): Use the local version of The Pipe instead of the hosted API. - `--
+match` (optional): Regex pattern to match files in the directory. - `--ignore`
+(optional): Regex pattern to ignore files in the directory. - `--limit`
+(optional): The token limit for the output prompt, defaults to 100K. Prompts
+exceeding the limit will be compressed. - `--ai_extraction` (optional): Extract
+tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
+`--text_only` (optional): Do not extract images from documents or websites.
+Additionally, image files will be represented with OCR instead of as images. !
+[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
+assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
```

