# Comparing `tmp/europarser-0.1.5.tar.gz` & `tmp/europarser-0.1.6.tar.gz`

## Comparing `europarser-0.1.5.tar` & `europarser-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 europarser-0.1.5/.dockerignore
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 europarser-0.1.5/Dockerfile
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 europarser-0.1.5/README_en.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 europarser-0.1.5/docker_log.conf
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 europarser-0.1.5/log.conf
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.5/pyinstaller.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 europarser-0.1.5/start_europarser.sh
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 europarser-0.1.5/.github/workflows/docker-publish.yml
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 europarser-0.1.5/.github/workflows/hatch-build-and-publish.yml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/__about__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/__init__.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/daniel_light.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/endpoint.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/lang_detect.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/main.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/models.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/pipeline.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/pivot.py
--rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/api/__init__.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/api/api.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/api/utils.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/api/static/basic.min.css
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/api/static/dropzone.min.css
--rw-r--r--   0        0        0   114649 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/api/static/dropzone.min.js
--rw-r--r--   0        0        0    39237 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/api/static/favicon.ico
--rw-r--r--   0        0        0    14776 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/api/templates/main.html
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/to_csv.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/to_gephi.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/to_iramuteq.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/to_json.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/to_markdown.py
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/to_stats.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/to_txm.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 europarser-0.1.5/src/europarser/transformers/transformer.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 europarser-0.1.5/tests/api_tester.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 europarser-0.1.5/.gitignore
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 europarser-0.1.5/.hgignore
--rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 europarser-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 europarser-0.1.5/README.md
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 europarser-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 europarser-0.1.6/.dockerignore
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 europarser-0.1.6/Dockerfile
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 europarser-0.1.6/README_en.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 europarser-0.1.6/docker_log.conf
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 europarser-0.1.6/log.conf
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.6/pyinstaller.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 europarser-0.1.6/start_europarser.sh
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 europarser-0.1.6/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 europarser-0.1.6/.github/workflows/hatch-build-and-publish.yml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/__about__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/__init__.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/daniel_light.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/endpoint.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/lang_detect.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/main.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/models.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/pipeline.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/pivot.py
+-rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/api/__init__.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/api/api.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/api/utils.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/api/static/basic.min.css
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/api/static/dropzone.min.css
+-rw-r--r--   0        0        0   114649 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/api/static/dropzone.min.js
+-rw-r--r--   0        0        0    39237 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/api/static/favicon.ico
+-rw-r--r--   0        0        0    14776 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/api/templates/main.html
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/to_csv.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/to_gephi.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/to_iramuteq.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/to_json.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/to_markdown.py
+-rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/to_stats.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/to_txm.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 europarser-0.1.6/src/europarser/transformers/transformer.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 europarser-0.1.6/tests/api_tester.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 europarser-0.1.6/.gitignore
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 europarser-0.1.6/.hgignore
+-rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 europarser-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 europarser-0.1.6/README.md
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 europarser-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 europarser-0.1.6/PKG-INFO
```

### Comparing `europarser-0.1.5/README_en.md` & `europarser-0.1.6/README_en.md`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/docker_log.conf` & `europarser-0.1.6/docker_log.conf`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/log.conf` & `europarser-0.1.6/log.conf`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 handlers=error_file
 propagate=1
 qualname=uvicorn.error
 
 [handler_error_file]
 class=logging.handlers.TimedRotatingFileHandler
 formatter=generic
-args=('/home/marceau/logs_europarser/europarser-errors.log', 'midnight', 1, 90, 'utf-8')
+args=('/home/marceau/logs/europarser/europarser-errors.log', 'midnight', 1, 90, 'utf-8')
 
 [handler_access_file]
 class=logging.handlers.TimedRotatingFileHandler
 formatter=access
-args=('/home/marceau/logs_europarser/europarser-access.log', 'midnight', 1, 90, 'utf-8')
+args=('/home/marceau/logs/europarser/europarser-access.log', 'midnight', 1, 90, 'utf-8')
 
 [handler_console]
 class=StreamHandler
 formatter=generic
 args=(sys.stdout, )
 
 [formatter_generic]
```

### Comparing `europarser-0.1.5/pyinstaller.py` & `europarser-0.1.6/pyinstaller.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/.github/workflows/docker-publish.yml` & `europarser-0.1.6/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/.github/workflows/hatch-build-and-publish.yml` & `europarser-0.1.6/.github/workflows/hatch-build-and-publish.yml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/daniel_light.py` & `europarser-0.1.6/src/europarser/daniel_light.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/endpoint.py` & `europarser-0.1.6/src/europarser/endpoint.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/main.py` & `europarser-0.1.6/src/europarser/main.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/models.py` & `europarser-0.1.6/src/europarser/models.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/pipeline.py` & `europarser-0.1.6/src/europarser/pipeline.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/pivot.py` & `europarser-0.1.6/src/europarser/pivot.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/utils.py` & `europarser-0.1.6/src/europarser/utils.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/api/api.py` & `europarser-0.1.6/src/europarser/api/api.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/api/static/basic.min.css` & `europarser-0.1.6/src/europarser/api/static/basic.min.css`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/api/static/dropzone.min.css` & `europarser-0.1.6/src/europarser/api/static/dropzone.min.css`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/api/static/dropzone.min.js` & `europarser-0.1.6/src/europarser/api/static/dropzone.min.js`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/api/static/favicon.ico` & `europarser-0.1.6/src/europarser/api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/api/templates/main.html` & `europarser-0.1.6/src/europarser/api/templates/main.html`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/transformers/to_csv.py` & `europarser-0.1.6/src/europarser/transformers/to_csv.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/transformers/to_gephi.py` & `europarser-0.1.6/src/europarser/transformers/to_gephi.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/transformers/to_iramuteq.py` & `europarser-0.1.6/src/europarser/transformers/to_iramuteq.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/transformers/to_json.py` & `europarser-0.1.6/src/europarser/transformers/to_json.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/transformers/to_markdown.py` & `europarser-0.1.6/src/europarser/transformers/to_markdown.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/transformers/to_stats.py` & `europarser-0.1.6/src/europarser/transformers/to_stats.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/transformers/to_txm.py` & `europarser-0.1.6/src/europarser/transformers/to_txm.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/src/europarser/transformers/transformer.py` & `europarser-0.1.6/src/europarser/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/tests/api_tester.py` & `europarser-0.1.6/tests/api_tester.py`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/.gitignore` & `europarser-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/LICENSE.txt` & `europarser-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/README.md` & `europarser-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/pyproject.toml` & `europarser-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `europarser-0.1.5/PKG-INFO` & `europarser-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: europarser
-Version: 0.1.5
+Version: 0.1.6
 Project-URL: Documentation, https://github.com/CERES-sorbonne/europarser#readme
 Project-URL: Issues, https://github.com/CERES-sorbonne/europarser/issues
 Project-URL: Source, https://github.com/CERES-sorbonne/europarser
 Author-email: Marceau <pypi@marceau-h.fr>
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

