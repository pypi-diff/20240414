# Comparing `tmp/thepipe_api-0.1.4.tar.gz` & `tmp/thepipe_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thepipe_api-0.1.4.tar", last modified: Sat Apr 13 20:49:26 2024, max compression
+gzip compressed data, was "thepipe_api-0.1.5.tar", last modified: Sun Apr 14 20:27:59 2024, max compression
```

## Comparing `thepipe_api-0.1.4.tar` & `thepipe_api-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 20:49:26.456596 thepipe_api-0.1.4/
--rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     9329 2024-04-13 20:49:26.455596 thepipe_api-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     8603 2024-04-13 20:45:01.000000 thepipe_api-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-13 20:49:26.456596 thepipe_api-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      740 2024-04-13 20:49:14.000000 thepipe_api-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:49:26.432596 thepipe_api-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0     9523 2024-04-13 20:12:45.000000 thepipe_api-0.1.4/tests/test_thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:49:26.437606 thepipe_api-0.1.4/thepipe_api/
--rw-rw-rw-   0        0        0       48 2024-04-13 19:44:21.000000 thepipe_api-0.1.4/thepipe_api/__init__.py
--rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.4/thepipe_api/compressor.py
--rw-rw-rw-   0        0        0     2835 2024-04-13 18:07:10.000000 thepipe_api-0.1.4/thepipe_api/core.py
--rw-rw-rw-   0        0        0    19616 2024-04-13 20:47:49.000000 thepipe_api-0.1.4/thepipe_api/extractor.py
--rw-rw-rw-   0        0        0     3504 2024-04-13 20:43:49.000000 thepipe_api-0.1.4/thepipe_api/thepipe.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:49:26.454603 thepipe_api-0.1.4/thepipe_api.egg-info/
--rw-rw-rw-   0        0        0     9329 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 20:49:26.000000 thepipe_api-0.1.4/thepipe_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:59.058854 thepipe_api-0.1.5/
+-rw-rw-rw-   0        0        0     1094 2024-03-27 18:15:40.000000 thepipe_api-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     9416 2024-04-14 20:27:59.057855 thepipe_api-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8688 2024-04-14 00:39:19.000000 thepipe_api-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-14 20:27:59.059854 thepipe_api-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      740 2024-04-14 20:27:54.000000 thepipe_api-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:59.026854 thepipe_api-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-23 01:45:32.000000 thepipe_api-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     9523 2024-04-13 23:06:00.000000 thepipe_api-0.1.5/tests/test_thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:59.031855 thepipe_api-0.1.5/thepipe_api/
+-rw-rw-rw-   0        0        0       48 2024-04-13 19:44:21.000000 thepipe_api-0.1.5/thepipe_api/__init__.py
+-rw-rw-rw-   0        0        0     4821 2024-04-13 20:40:22.000000 thepipe_api-0.1.5/thepipe_api/compressor.py
+-rw-rw-rw-   0        0        0     2842 2024-04-14 20:23:07.000000 thepipe_api-0.1.5/thepipe_api/core.py
+-rw-rw-rw-   0        0        0    19797 2024-04-14 00:54:40.000000 thepipe_api-0.1.5/thepipe_api/extractor.py
+-rw-rw-rw-   0        0        0     3504 2024-04-13 20:43:49.000000 thepipe_api-0.1.5/thepipe_api/thepipe.py
+drwxrwxrwx   0        0        0        0 2024-04-14 20:27:59.057855 thepipe_api-0.1.5/thepipe_api.egg-info/
+-rw-rw-rw-   0        0        0     9416 2024-04-14 20:27:58.000000 thepipe_api-0.1.5/thepipe_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2024-04-14 20:27:58.000000 thepipe_api-0.1.5/thepipe_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 20:27:58.000000 thepipe_api-0.1.5/thepipe_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-04-14 20:27:58.000000 thepipe_api-0.1.5/thepipe_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 20:27:58.000000 thepipe_api-0.1.5/thepipe_api.egg-info/top_level.txt
```

### Comparing `thepipe_api-0.1.4/LICENSE` & `thepipe_api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.4/PKG-INFO` & `thepipe_api-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,27 +18,35 @@
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: cssutils
 Requires-Dist: beautifulsoup4
 Requires-Dist: PyMuPDF
 
+
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
+<p>
+  <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
+</p>
 
-### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
+### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-## Getting Started 🚀
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
-First, install thepipe:
-```bash
+## Getting Started  🚀
+
+First, install The Pipe. 
+```
 pip install thepipe_api
 ```
+
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally instead? See the local installation section.
+
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf")
 ```
 Or any website:
 ```python
@@ -80,38 +88,32 @@
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
-## Installation 📦
-
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
+To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
 Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
 
 Now you can use The Pipe:
 ```bash
-python thepipe.py path/to/directory
+from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf", local=True)
 ```
 
-This command will process all supported files within the specified directory, compressing any information over the token limit if necessary, and outputting the resulting prompt and images to a folder.
-
 Arguments are:
-- The input source (required): can be a file path, a URL, or a directory path.
-- `--local` (optional): Use the local version of The Pipe instead of the hosted API.
-- `--match` (optional): Regex pattern to match files in the directory.
-- `--ignore` (optional): Regex pattern to ignore files in the directory.
-- `--limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
-- `--ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
-- `--text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
-
-![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
-
+- `source` (required): can be a file path, a URL, or a directory path.
+- `local` (optional): Use the local version of The Pipe instead of the hosted API.
+- `match` (optional): Regex pattern to match files in the directory.
+- `ignore` (optional): Regex pattern to ignore files in the directory.
+- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
+- `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
+- `text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
```

#### html2text {}

```diff
@@ -1,31 +1,35 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.4 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.5 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
 pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
-PyMuPDF # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e [![codecov](https://codecov.io/gh/
-emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/
-thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/
-python-ci.yml/badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+PyMuPDF # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
+_E_n_g_l_i_s_h | _ä_¸_­_æ__
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/
+badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
+action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
+badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
-_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_A_p_p_l_y_%_2_0_h_e_r_e_-_b_l_u_e_) ### Prepare PDFs, word
-docs, slides, web pages and more for Vision-LLMs with one line of code â¡ The
-Pipe is a multimodal-first tool for feeding files and web pages into vision
-language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG
-applications that require a deep understanding of complex sources. The Pipe is
-available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone
-tool you can use locally. ## Getting Started ð First, install thepipe:
-```bash pip install thepipe_api ``` Now you can extract comprehensive text and
-visuals from any file: ```python from thepipe_api import thepipe chunks =
-thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
+_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
+docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
+Pipe is a multimodal-first tool for feeding files and web pages into vision-
+language models such as GPT-4V. It is best for LLM and RAG applications that
+require a deep understanding of tricky data sources. The Pipe is available as a
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. ##
+Getting Started ð First, install The Pipe. ``` pip install thepipe_api ```
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key
+yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally
+instead? See the local installation section. Now you can extract comprehensive
+text and visuals from any file: ```python from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
 thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
 ```python response = client.chat.completions.create( model="gpt-4-vision-
 preview", messages = chunks, ) ``` The Pipe's output is a list of sensible
 "chunks", and thus can be used either for storage in a vector database or for
 direct use as a prompt. Extra features such as data table extraction, bar chart
 extraction, custom web authentications and more are available in the [API
 documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/
@@ -74,29 +78,26 @@
 PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
 from PowerPoint presentations | | Website | URLs (inputs containing `http`,
 `https`, `www`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along
 with image (or images if scrollable); text-only extraction available | | GitHub
 Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
 repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
 âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## Installation ð¦ ## Local Installation ð ï¸ To use The Pipe locally, you
-will need [playwright](https://github.com/microsoft/playwright), [ctags](https:
-//github.com/universal-ctags/), [pytesseract](https://github.com/h/
-pytesseract), and the local python requirements, which differ from the more
-lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
-pip install -r requirements_local.txt ``` Tip for windows users: you may need
-to install the python-libmagic binaries with `pip install python-magic-bin`.
-Now you can use The Pipe: ```bash python thepipe.py path/to/directory ``` This
-command will process all supported files within the specified directory,
-compressing any information over the token limit if necessary, and outputting
-the resulting prompt and images to a folder. Arguments are: - The input source
-(required): can be a file path, a URL, or a directory path. - `--local`
-(optional): Use the local version of The Pipe instead of the hosted API. - `--
-match` (optional): Regex pattern to match files in the directory. - `--ignore`
-(optional): Regex pattern to ignore files in the directory. - `--limit`
-(optional): The token limit for the output prompt, defaults to 100K. Prompts
-exceeding the limit will be compressed. - `--ai_extraction` (optional): Extract
-tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
-`--text_only` (optional): Do not extract images from documents or websites.
-Additionally, image files will be represented with OCR instead of as images. !
-[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
-assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
+## Local Installation ð ï¸ To use The Pipe locally, you will need
+[playwright](https://github.com/microsoft/playwright), [ctags](https://
+github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract),
+and the local python requirements, which differ from the more lightweight API
+requirements. You will also need to use the local version of the requirements
+file: ```bash git clone https://github.com/emcf/thepipe pip install -
+r requirements_local.txt ``` Tip for windows users: you may need to install the
+python-libmagic binaries with `pip install python-magic-bin`. Now you can use
+The Pipe: ```bash from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf", local=True) ``` Arguments are: - `source` (required): can be a
+file path, a URL, or a directory path. - `local` (optional): Use the local
+version of The Pipe instead of the hosted API. - `match` (optional): Regex
+pattern to match files in the directory. - `ignore` (optional): Regex pattern
+to ignore files in the directory. - `limit` (optional): The token limit for the
+output prompt, defaults to 100K. Prompts exceeding the limit will be
+compressed. - `ai_extraction` (optional): Extract tables, figures, and math
+from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
+not extract images from documents or websites. Additionally, image files will
+be represented with OCR instead of as images.
```

### Comparing `thepipe_api-0.1.4/README.md` & `thepipe_api-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
+<p>
+  <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
+</p>
 
-### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
+### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-## Getting Started 🚀
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
-First, install thepipe:
-```bash
+## Getting Started  🚀
+
+First, install The Pipe. 
+```
 pip install thepipe_api
 ```
+
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally instead? See the local installation section.
+
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf")
 ```
 Or any website:
 ```python
@@ -56,38 +64,32 @@
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
-## Installation 📦
-
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
+To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
 Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
 
 Now you can use The Pipe:
 ```bash
-python thepipe.py path/to/directory
+from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf", local=True)
 ```
 
-This command will process all supported files within the specified directory, compressing any information over the token limit if necessary, and outputting the resulting prompt and images to a folder.
-
 Arguments are:
-- The input source (required): can be a file path, a URL, or a directory path.
-- `--local` (optional): Use the local version of The Pipe instead of the hosted API.
-- `--match` (optional): Regex pattern to match files in the directory.
-- `--ignore` (optional): Regex pattern to ignore files in the directory.
-- `--limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
-- `--ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
-- `--text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
-
-![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
-
+- `source` (required): can be a file path, a URL, or a directory path.
+- `local` (optional): Use the local version of The Pipe instead of the hosted API.
+- `match` (optional): Regex pattern to match files in the directory.
+- `ignore` (optional): Regex pattern to ignore files in the directory.
+- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
+- `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
+- `text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
```

#### html2text {}

```diff
@@ -1,22 +1,26 @@
-# _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e [![codecov](https://codecov.io/gh/emcf/
-thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe)
-![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-
-ci.yml/badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+# _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
+_E_n_g_l_i_s_h | _ä_¸_­_æ__
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/
+badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
+action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
+badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
-_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_A_p_p_l_y_%_2_0_h_e_r_e_-_b_l_u_e_) ### Prepare PDFs, word
-docs, slides, web pages and more for Vision-LLMs with one line of code â¡ The
-Pipe is a multimodal-first tool for feeding files and web pages into vision
-language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG
-applications that require a deep understanding of complex sources. The Pipe is
-available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone
-tool you can use locally. ## Getting Started ð First, install thepipe:
-```bash pip install thepipe_api ``` Now you can extract comprehensive text and
-visuals from any file: ```python from thepipe_api import thepipe chunks =
-thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
+_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
+docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
+Pipe is a multimodal-first tool for feeding files and web pages into vision-
+language models such as GPT-4V. It is best for LLM and RAG applications that
+require a deep understanding of tricky data sources. The Pipe is available as a
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. ##
+Getting Started ð First, install The Pipe. ``` pip install thepipe_api ```
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key
+yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally
+instead? See the local installation section. Now you can extract comprehensive
+text and visuals from any file: ```python from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
 thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
 ```python response = client.chat.completions.create( model="gpt-4-vision-
 preview", messages = chunks, ) ``` The Pipe's output is a list of sensible
 "chunks", and thus can be used either for storage in a vector database or for
 direct use as a prompt. Extra features such as data table extraction, bar chart
 extraction, custom web authentications and more are available in the [API
 documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/
@@ -65,29 +69,26 @@
 PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
 from PowerPoint presentations | | Website | URLs (inputs containing `http`,
 `https`, `www`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along
 with image (or images if scrollable); text-only extraction available | | GitHub
 Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
 repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
 âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## Installation ð¦ ## Local Installation ð ï¸ To use The Pipe locally, you
-will need [playwright](https://github.com/microsoft/playwright), [ctags](https:
-//github.com/universal-ctags/), [pytesseract](https://github.com/h/
-pytesseract), and the local python requirements, which differ from the more
-lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
-pip install -r requirements_local.txt ``` Tip for windows users: you may need
-to install the python-libmagic binaries with `pip install python-magic-bin`.
-Now you can use The Pipe: ```bash python thepipe.py path/to/directory ``` This
-command will process all supported files within the specified directory,
-compressing any information over the token limit if necessary, and outputting
-the resulting prompt and images to a folder. Arguments are: - The input source
-(required): can be a file path, a URL, or a directory path. - `--local`
-(optional): Use the local version of The Pipe instead of the hosted API. - `--
-match` (optional): Regex pattern to match files in the directory. - `--ignore`
-(optional): Regex pattern to ignore files in the directory. - `--limit`
-(optional): The token limit for the output prompt, defaults to 100K. Prompts
-exceeding the limit will be compressed. - `--ai_extraction` (optional): Extract
-tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
-`--text_only` (optional): Do not extract images from documents or websites.
-Additionally, image files will be represented with OCR instead of as images. !
-[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
-assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
+## Local Installation ð ï¸ To use The Pipe locally, you will need
+[playwright](https://github.com/microsoft/playwright), [ctags](https://
+github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract),
+and the local python requirements, which differ from the more lightweight API
+requirements. You will also need to use the local version of the requirements
+file: ```bash git clone https://github.com/emcf/thepipe pip install -
+r requirements_local.txt ``` Tip for windows users: you may need to install the
+python-libmagic binaries with `pip install python-magic-bin`. Now you can use
+The Pipe: ```bash from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf", local=True) ``` Arguments are: - `source` (required): can be a
+file path, a URL, or a directory path. - `local` (optional): Use the local
+version of The Pipe instead of the hosted API. - `match` (optional): Regex
+pattern to match files in the directory. - `ignore` (optional): Regex pattern
+to ignore files in the directory. - `limit` (optional): The token limit for the
+output prompt, defaults to 100K. Prompts exceeding the limit will be
+compressed. - `ai_extraction` (optional): Extract tables, figures, and math
+from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
+not extract images from documents or websites. Additionally, image files will
+be represented with OCR instead of as images.
```

### Comparing `thepipe_api-0.1.4/setup.py` & `thepipe_api-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='thepipe_api',
-    version='0.1.4',
+    version='0.1.5',
     author='Emmett McFarlane',
     author_email='emmett@thepi.pe',
     description='Automate information extraction for multimodal LLMs.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/emcf/thepipe',
     packages=find_packages(),
```

### Comparing `thepipe_api-0.1.4/tests/test_thepipe.py` & `thepipe_api-0.1.5/tests/test_thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.4/thepipe_api/compressor.py` & `thepipe_api-0.1.5/thepipe_api/compressor.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.4/thepipe_api/core.py` & `thepipe_api-0.1.5/thepipe_api/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,10 +69,10 @@
     for chunk in chunks:
         content = []
         if chunk.text:
             content.append({"type": "text", "text": f"""{chunk.path}:\n```\n{chunk.text}\n```\n"""})
         if chunk.image:
             base64_image = image_to_base64(chunk.image)
             content.append({"type": "text", "text": f"""{chunk.path} image:"""})
-            content.append({"type": "image_url", "image_url": f"data:image/jpeg;base64,{base64_image}"})
-        messages.append({"role": "system", "content": content})
+            content.append({"type": "image_url", "image_url": {"url": f"data:image/jpeg;base64,{base64_image}"}})
+        messages.append({"role": "user", "content": content})
     return messages
```

### Comparing `thepipe_api-0.1.4/thepipe_api/extractor.py` & `thepipe_api-0.1.5/thepipe_api/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,16 @@
             extraction = [extract_plaintext(file_path=file_path)]
         elif source_type == SourceTypes.UNCOMPRESSIBLE_CODE:
             extraction = [extract_plaintext(file_path=file_path)]
             extraction = [Chunk(path=e.path, text=e.text, image=None, source_type=SourceTypes.UNCOMPRESSIBLE_CODE) for e in extraction] # change types to code
         elif source_type == SourceTypes.COMPRESSIBLE_CODE:
             extraction = [extract_plaintext(file_path=file_path)]
             extraction = [Chunk(path=e.path, text=e.text, image=None, source_type=SourceTypes.COMPRESSIBLE_CODE) for e in extraction]
+        elif source_type == SourceTypes.IPYNB:
+            extraction = extract_from_ipynb(file_path=file_path, verbose=verbose, ai_extraction=ai_extraction, text_only=text_only)
         else:
             extraction = [extract_plaintext(file_path=file_path)]
         if verbose: print_status(f"Extracted from {file_path}", status='success')
         return extraction
     except Exception as e:
         if verbose: print_status(f"Failed to extract from {file_path}: {e}", status='error')
         return [Chunk(path=file_path)]
```

### Comparing `thepipe_api-0.1.4/thepipe_api/thepipe.py` & `thepipe_api-0.1.5/thepipe_api/thepipe.py`

 * *Files identical despite different names*

### Comparing `thepipe_api-0.1.4/thepipe_api.egg-info/PKG-INFO` & `thepipe_api-0.1.5/thepipe_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thepipe_api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Automate information extraction for multimodal LLMs.
 Home-page: https://github.com/emcf/thepipe
 Author: Emmett McFarlane
 Author-email: emmett@thepi.pe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,27 +18,35 @@
 Requires-Dist: colorama
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: cssutils
 Requires-Dist: beautifulsoup4
 Requires-Dist: PyMuPDF
 
+
 # <a href="https://thepi.pe/"><img src="https://rpnutzemutbrumczwvue.supabase.co/storage/v1/object/public/assets/pipeline_small%20(1).png" alt="Pipeline Illustration" style="width:96px; height:72px; vertical-align:middle;"> The Pipe</a>
-[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-Apply%20here-blue)</a>
+<p>
+  <a href="https://github.com/emcf/thepipe/blob/main/README.md">English</a> | <a href="https://github.com/emcf/thepipe/blob/main/README_cn.md">中文</a>
+</p>
 
-### Prepare PDFs, word docs, slides, web pages and more for Vision-LLMs with one line of code ⚡
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/badge.svg) <a href="https://thepi.pe/">![Website](https://img.shields.io/website?url=https%3A%2F%2Fthepipe.up.railway.app%2F&label=API%20status)</a> <a href="https://thepi.pe/">![get API](https://img.shields.io/badge/API-get%20access-blue)</a>
 
-The Pipe is a multimodal-first tool for feeding files and web pages into vision language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG applications that require a deep understanding of complex sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone tool you can use locally.
+### Feed PDFs, word docs, slides, web pages and more into Vision-LLMs with one line of code ⚡
 
-## Getting Started 🚀
+The Pipe is a multimodal-first tool for feeding files and web pages into vision-language models such as GPT-4V. It is best for LLM and RAG applications that require a deep understanding of tricky data sources. The Pipe is available as a hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally.
 
-First, install thepipe:
-```bash
+## Getting Started  🚀
+
+First, install The Pipe. 
+```
 pip install thepipe_api
 ```
+
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally instead? See the local installation section.
+
 Now you can extract comprehensive text and visuals from any file:
 ```python
 from thepipe_api import thepipe
 chunks = thepipe.extract("example.pdf")
 ```
 Or any website:
 ```python
@@ -80,38 +88,32 @@
 | Jupyter Notebook                      | `.ipynb`                                | ❌               | ✔️               | Extracts code, markdown, and images from Jupyter notebooks                                  |
 | Microsoft Word Document               | `.docx`                                 | ✔️               | ✔️               | Extracts text and images from Word documents                                        |
 | Microsoft PowerPoint Presentation     | `.pptx`                                 | ✔️               | ✔️               | Extracts text and images from PowerPoint presentations                              |
 | Website                               | URLs (inputs containing `http`, `https`, `www`, `ftp`)             | ✔️                | ✔️    | Extracts text from web page along with image (or images if scrollable); text-only extraction available          |
 | GitHub Repository                     | GitHub repo URLs                         | ✔️               | ✔️                | Extracts from GitHub repositories; supports branch specification         |
 | ZIP File                              | `.zip`                                  | ✔️               | ✔️                | Extracts contents of ZIP files; supports nested directory extraction     |
 
-## Installation 📦
-
 ## Local Installation 🛠️
 
-To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements:
+To use The Pipe locally, you will need [playwright](https://github.com/microsoft/playwright), [ctags](https://github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract), and the local python requirements, which differ from the more lightweight API requirements. You will also need to use the local version of the requirements file:
 
 ```bash
 git clone https://github.com/emcf/thepipe
 pip install -r requirements_local.txt
 ```
 
 Tip for windows users: you may need to install the python-libmagic binaries with `pip install python-magic-bin`.
 
 Now you can use The Pipe:
 ```bash
-python thepipe.py path/to/directory
+from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf", local=True)
 ```
 
-This command will process all supported files within the specified directory, compressing any information over the token limit if necessary, and outputting the resulting prompt and images to a folder.
-
 Arguments are:
-- The input source (required): can be a file path, a URL, or a directory path.
-- `--local` (optional): Use the local version of The Pipe instead of the hosted API.
-- `--match` (optional): Regex pattern to match files in the directory.
-- `--ignore` (optional): Regex pattern to ignore files in the directory.
-- `--limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
-- `--ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
-- `--text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
-
-![Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
-
+- `source` (required): can be a file path, a URL, or a directory path.
+- `local` (optional): Use the local version of The Pipe instead of the hosted API.
+- `match` (optional): Regex pattern to match files in the directory.
+- `ignore` (optional): Regex pattern to ignore files in the directory.
+- `limit` (optional): The token limit for the output prompt, defaults to 100K. Prompts exceeding the limit will be compressed.
+- `ai_extraction` (optional): Extract tables, figures, and math from PDFs using our extractor. Incurs extra costs.
+- `text_only` (optional): Do not extract images from documents or websites. Additionally, image files will be represented with OCR instead of as images.
```

#### html2text {}

```diff
@@ -1,31 +1,35 @@
-Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.4 Summary: Automate
+Metadata-Version: 2.1 Name: thepipe_api Version: 0.1.5 Summary: Automate
 information extraction for multimodal LLMs. Home-page: https://github.com/emcf/
 thepipe Author: Emmett McFarlane Author-email: emmett@thepi.pe Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 aiohttp Requires-Dist: charset-normalizer Requires-Dist: Pyarrow Requires-Dist:
 python-magic Requires-Dist: colorama Requires-Dist: requests Requires-Dist:
 pillow Requires-Dist: cssutils Requires-Dist: beautifulsoup4 Requires-Dist:
-PyMuPDF # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e [![codecov](https://codecov.io/gh/
-emcf/thepipe/graph/badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/
-thepipe) ![python-gh-action](https://github.com/emcf/thepipe/actions/workflows/
-python-ci.yml/badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+PyMuPDF # _[_P_i_p_e_l_i_n_e_ _I_l_l_u_s_t_r_a_t_i_o_n_]_T_h_e_ _P_i_p_e
+_E_n_g_l_i_s_h | _ä_¸_­_æ__
+[![codecov](https://codecov.io/gh/emcf/thepipe/graph/
+badge.svg?token=OE7CUEFUL9)](https://codecov.io/gh/emcf/thepipe) ![python-gh-
+action](https://github.com/emcf/thepipe/actions/workflows/python-ci.yml/
+badge.svg) _!_[_W_e_b_s_i_t_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _w_e_b_s_i_t_e_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_t_h_e_p_i_p_e_._u_p_._r_a_i_l_w_a_y_._a_p_p_%_2_F_&_l_a_b_e_l_=_A_P_I_%_2_0_s_t_a_t_u_s_) _!_[_g_e_t
-_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_A_p_p_l_y_%_2_0_h_e_r_e_-_b_l_u_e_) ### Prepare PDFs, word
-docs, slides, web pages and more for Vision-LLMs with one line of code â¡ The
-Pipe is a multimodal-first tool for feeding files and web pages into vision
-language models like GPT-4V, Gemini Pro, and LLaVa. It is best for LLM and RAG
-applications that require a deep understanding of complex sources. The Pipe is
-available as a hosted API at [thepi.pe](https://thepi.pe) and as a standalone
-tool you can use locally. ## Getting Started ð First, install thepipe:
-```bash pip install thepipe_api ``` Now you can extract comprehensive text and
-visuals from any file: ```python from thepipe_api import thepipe chunks =
-thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
+_A_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_P_I_-_g_e_t_%_2_0_a_c_c_e_s_s_-_b_l_u_e_) ### Feed PDFs, word
+docs, slides, web pages and more into Vision-LLMs with one line of code â¡ The
+Pipe is a multimodal-first tool for feeding files and web pages into vision-
+language models such as GPT-4V. It is best for LLM and RAG applications that
+require a deep understanding of tricky data sources. The Pipe is available as a
+hosted API at [thepi.pe](https://thepi.pe), or it can be set up locally. ##
+Getting Started ð First, install The Pipe. ``` pip install thepipe_api ```
+Ensure the `THEPIPE_API_KEY` environment variable is set. Don't have an API key
+yet? [Get one here](https://thepi.pe). Looking to operate it yourself locally
+instead? See the local installation section. Now you can extract comprehensive
+text and visuals from any file: ```python from thepipe_api import thepipe
+chunks = thepipe.extract("example.pdf") ``` Or any website: ```python chunks =
 thepipe.extract("https://example.com") ``` Then feed it into GPT-4-Vision:
 ```python response = client.chat.completions.create( model="gpt-4-vision-
 preview", messages = chunks, ) ``` The Pipe's output is a list of sensible
 "chunks", and thus can be used either for storage in a vector database or for
 direct use as a prompt. Extra features such as data table extraction, bar chart
 extraction, custom web authentications and more are available in the [API
 documentation](https://thepi.pe/docs). [LiteLLM](https://github.com/BerriAI/
@@ -74,29 +78,26 @@
 PowerPoint Presentation | `.pptx` | âï¸ | âï¸ | Extracts text and images
 from PowerPoint presentations | | Website | URLs (inputs containing `http`,
 `https`, `www`, `ftp`) | âï¸ | âï¸ | Extracts text from web page along
 with image (or images if scrollable); text-only extraction available | | GitHub
 Repository | GitHub repo URLs | âï¸ | âï¸ | Extracts from GitHub
 repositories; supports branch specification | | ZIP File | `.zip` | âï¸ |
 âï¸ | Extracts contents of ZIP files; supports nested directory extraction |
-## Installation ð¦ ## Local Installation ð ï¸ To use The Pipe locally, you
-will need [playwright](https://github.com/microsoft/playwright), [ctags](https:
-//github.com/universal-ctags/), [pytesseract](https://github.com/h/
-pytesseract), and the local python requirements, which differ from the more
-lightweight API requirements: ```bash git clone https://github.com/emcf/thepipe
-pip install -r requirements_local.txt ``` Tip for windows users: you may need
-to install the python-libmagic binaries with `pip install python-magic-bin`.
-Now you can use The Pipe: ```bash python thepipe.py path/to/directory ``` This
-command will process all supported files within the specified directory,
-compressing any information over the token limit if necessary, and outputting
-the resulting prompt and images to a folder. Arguments are: - The input source
-(required): can be a file path, a URL, or a directory path. - `--local`
-(optional): Use the local version of The Pipe instead of the hosted API. - `--
-match` (optional): Regex pattern to match files in the directory. - `--ignore`
-(optional): Regex pattern to ignore files in the directory. - `--limit`
-(optional): The token limit for the output prompt, defaults to 100K. Prompts
-exceeding the limit will be compressed. - `--ai_extraction` (optional): Extract
-tables, figures, and math from PDFs using our extractor. Incurs extra costs. -
-`--text_only` (optional): Do not extract images from documents or websites.
-Additionally, image files will be represented with OCR instead of as images. !
-[Demo](https://ngrdaaykhfrmtpodlakn.supabase.co/storage/v1/object/public/
-assets/demo.gif?t=2024-03-24T19%3A13%3A46.695Z)
+## Local Installation ð ï¸ To use The Pipe locally, you will need
+[playwright](https://github.com/microsoft/playwright), [ctags](https://
+github.com/universal-ctags/), [pytesseract](https://github.com/h/pytesseract),
+and the local python requirements, which differ from the more lightweight API
+requirements. You will also need to use the local version of the requirements
+file: ```bash git clone https://github.com/emcf/thepipe pip install -
+r requirements_local.txt ``` Tip for windows users: you may need to install the
+python-libmagic binaries with `pip install python-magic-bin`. Now you can use
+The Pipe: ```bash from thepipe_api import thepipe chunks = thepipe.extract
+("example.pdf", local=True) ``` Arguments are: - `source` (required): can be a
+file path, a URL, or a directory path. - `local` (optional): Use the local
+version of The Pipe instead of the hosted API. - `match` (optional): Regex
+pattern to match files in the directory. - `ignore` (optional): Regex pattern
+to ignore files in the directory. - `limit` (optional): The token limit for the
+output prompt, defaults to 100K. Prompts exceeding the limit will be
+compressed. - `ai_extraction` (optional): Extract tables, figures, and math
+from PDFs using our extractor. Incurs extra costs. - `text_only` (optional): Do
+not extract images from documents or websites. Additionally, image files will
+be represented with OCR instead of as images.
```

