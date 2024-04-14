# Comparing `tmp/yq-3.2.3.tar.gz` & `tmp/yq-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yq-3.2.3.tar", last modified: Sat Sep  9 21:42:15 2023, max compression
+gzip compressed data, was "yq-3.3.0.tar", last modified: Sun Apr 14 05:26:43 2024, max compression
```

## Comparing `yq-3.2.3.tar` & `yq-3.3.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-09-09 21:42:15.761518 yq-3.2.3/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-09-09 21:42:15.756587 yq-3.2.3/.github/
--rw-r--r--   0 kislyuk    (501) staff       (20)       18 2022-07-03 19:16:59.000000 yq-3.2.3/.github/FUNDING.yml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-09-09 21:42:15.756760 yq-3.2.3/.github/workflows/
--rw-r--r--   0 kislyuk    (501) staff       (20)      837 2023-05-06 15:40:31.000000 yq-3.2.3/.github/workflows/ci.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      477 2022-07-03 19:16:59.000000 yq-3.2.3/.gitignore
--rw-r--r--   0 kislyuk    (501) staff       (20)     7788 2023-09-09 21:41:55.000000 yq-3.2.3/Changes.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    10273 2017-01-14 17:06:39.000000 yq-3.2.3/LICENSE
--rw-r--r--   0 kislyuk    (501) staff       (20)       41 2019-10-14 14:51:41.000000 yq-3.2.3/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)      478 2023-05-06 22:52:15.000000 yq-3.2.3/Makefile
--rw-r--r--   0 kislyuk    (501) staff       (20)     8719 2023-09-09 21:42:15.761231 yq-3.2.3/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)     7466 2023-09-09 21:39:17.000000 yq-3.2.3/README.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)      696 2023-04-05 01:34:39.000000 yq-3.2.3/SECURITY.md
--rw-r--r--   0 kislyuk    (501) staff       (20)     2556 2023-05-06 22:11:31.000000 yq-3.2.3/common.mk
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-09-09 21:42:15.758126 yq-3.2.3/docs/
--rw-r--r--   0 kislyuk    (501) staff       (20)       56 2022-07-03 19:16:59.000000 yq-3.2.3/docs/changelog.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)     2431 2023-09-09 21:41:55.000000 yq-3.2.3/docs/cli-doc-tomlq.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)     2911 2023-09-09 21:41:55.000000 yq-3.2.3/docs/cli-doc-xq.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)     3651 2023-09-09 21:41:55.000000 yq-3.2.3/docs/cli-doc.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      806 2023-05-06 22:52:24.000000 yq-3.2.3/docs/conf.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      248 2023-05-06 23:04:05.000000 yq-3.2.3/docs/index.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)        8 2023-05-06 22:11:31.000000 yq-3.2.3/docs/toc.html
--rw-r--r--   0 kislyuk    (501) staff       (20)      263 2023-04-05 01:34:39.000000 yq-3.2.3/pyproject.toml
--rw-r--r--   0 kislyuk    (501) staff       (20)       38 2023-09-09 21:42:15.761549 yq-3.2.3/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1676 2023-09-09 21:41:31.000000 yq-3.2.3/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-09-09 21:42:15.758900 yq-3.2.3/test/
--rw-r--r--   0 kislyuk    (501) staff       (20)     3468 2022-07-03 19:16:59.000000 yq-3.2.3/test/cfn.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)      306 2022-07-03 19:16:59.000000 yq-3.2.3/test/doc.yml
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2022-07-03 19:16:59.000000 yq-3.2.3/test/filter.jq
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    15827 2023-09-09 21:39:51.000000 yq-3.2.3/test/test.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-09-09 21:42:15.760089 yq-3.2.3/yq/
--rw-r--r--   0 kislyuk    (501) staff       (20)    13766 2023-09-09 21:39:17.000000 yq-3.2.3/yq/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)       56 2023-02-22 05:14:38.000000 yq-3.2.3/yq/__main__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3531 2023-02-22 05:14:38.000000 yq-3.2.3/yq/dumper.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     8172 2023-02-22 05:14:38.000000 yq-3.2.3/yq/loader.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     6212 2023-09-09 21:39:17.000000 yq-3.2.3/yq/parser.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      160 2023-09-09 21:42:15.000000 yq-3.2.3/yq/version.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-09-09 21:42:15.760652 yq-3.2.3/yq.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)     8719 2023-09-09 21:42:15.000000 yq-3.2.3/yq.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)      569 2023-09-09 21:42:15.000000 yq-3.2.3/yq.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-09-09 21:42:15.000000 yq-3.2.3/yq.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)       63 2023-09-09 21:42:15.000000 yq-3.2.3/yq.egg-info/entry_points.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      107 2023-09-09 21:42:15.000000 yq-3.2.3/yq.egg-info/requires.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        3 2023-09-09 21:42:15.000000 yq-3.2.3/yq.egg-info/top_level.txt
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.307416 yq-3.3.0/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.289090 yq-3.3.0/.github/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       18 2023-10-23 21:28:59.000000 yq-3.3.0/.github/FUNDING.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.289672 yq-3.3.0/.github/workflows/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      945 2024-04-13 17:02:32.000000 yq-3.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      477 2023-10-23 21:28:59.000000 yq-3.3.0/.gitignore
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8032 2024-04-14 05:26:20.000000 yq-3.3.0/Changes.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10273 2023-10-23 21:28:59.000000 yq-3.3.0/LICENSE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       41 2023-10-23 21:28:59.000000 yq-3.3.0/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      478 2023-10-23 21:28:59.000000 yq-3.3.0/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8836 2024-04-14 05:26:43.306693 yq-3.3.0/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7582 2024-04-14 04:46:08.000000 yq-3.3.0/README.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      696 2023-10-23 21:29:01.000000 yq-3.3.0/SECURITY.md
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2542 2024-04-14 04:46:23.000000 yq-3.3.0/common.mk
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.294956 yq-3.3.0/docs/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:59.000000 yq-3.3.0/docs/changelog.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3515 2024-04-14 05:26:20.000000 yq-3.3.0/docs/cli-doc-tomlq.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3897 2024-04-14 05:26:20.000000 yq-3.3.0/docs/cli-doc-xq.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4503 2024-04-14 05:26:20.000000 yq-3.3.0/docs/cli-doc.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      806 2023-10-23 21:28:59.000000 yq-3.3.0/docs/conf.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      248 2023-10-23 21:28:59.000000 yq-3.3.0/docs/index.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-10-23 21:28:59.000000 yq-3.3.0/docs/toc.html
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      416 2024-04-14 04:46:08.000000 yq-3.3.0/pyproject.toml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2024-04-14 05:26:43.307499 yq-3.3.0/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1677 2024-04-14 05:25:14.000000 yq-3.3.0/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.297523 yq-3.3.0/test/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3468 2023-10-23 21:28:59.000000 yq-3.3.0/test/cfn.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      306 2023-10-23 21:28:59.000000 yq-3.3.0/test/doc.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-10-23 21:28:59.000000 yq-3.3.0/test/filter.jq
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    15883 2024-04-13 16:56:36.000000 yq-3.3.0/test/test.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.301291 yq-3.3.0/yq/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    13702 2024-04-14 05:11:44.000000 yq-3.3.0/yq/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:58.000000 yq-3.3.0/yq/__main__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3531 2023-10-23 21:28:58.000000 yq-3.3.0/yq/dumper.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8940 2024-04-14 05:11:03.000000 yq-3.3.0/yq/loader.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6212 2023-10-23 21:28:58.000000 yq-3.3.0/yq/parser.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.305657 yq-3.3.0/yq.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8836 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      555 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/entry_points.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      107 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        3 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/top_level.txt
```

### Comparing `yq-3.2.3/.github/workflows/ci.yml` & `yq-3.3.0/.github/workflows/ci.yml`

 * *Files 21% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 jobs:
   unit_tests:
     runs-on: ${{matrix.os}}
     strategy:
       max-parallel: 8
       matrix:
         os: [ubuntu-20.04, ubuntu-22.04, macos-12]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
-    - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
+    - uses: actions/checkout@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: ${{matrix.python-version}}
     - name: Install jq
       run: |
         if [[ $(uname) == Linux ]]; then sudo apt-get install --yes jq; fi
         if [[ $(uname) == Darwin ]]; then brew install jq; fi
     - run: make install
-    - run: make lint
+    - if: ${{matrix.python-version == '3.12'}}
+      run: make lint
     - run: make test
     - uses: codecov/codecov-action@v3
   black:
     runs-on: ubuntu-22.04
     steps:
-      - uses: psf/black@stable
+    - uses: actions/checkout@v4
+    - uses: psf/black@stable
   isort:
     runs-on: ubuntu-22.04
     steps:
-      - uses: isort/isort-action@v1.1.0
+    - uses: actions/checkout@v4
+    - uses: isort/isort-action@v1.1.0
```

### Comparing `yq-3.2.3/Changes.rst` & `yq-3.3.0/Changes.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Changes for v3.3.0 (2024-04-13)
+===============================
+
+-  tomlq: Use tomllib on Python 3.11 when not round-tripping
+
+-  xq: Support in-place XML editing
+
+-  Do not interpret characters that cannot be parsed in octal as int
+   (#176)
+
 Changes for v3.2.3 (2023-09-09)
 ===============================
 
 -  test.py: use valid values for jsonargs. Fixes #172
 
 -  Allow editing toml in place (#171)
```

### Comparing `yq-3.2.3/LICENSE` & `yq-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yq-3.2.3/PKG-INFO` & `yq-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: yq
-Version: 3.2.3
+Version: 3.3.0
 Summary: Command-line YAML/XML processor - jq wrapper for YAML/XML documents
 Home-page: https://github.com/kislyuk/yq
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: PyYAML>=5.3.1
 Requires-Dist: xmltodict>=0.11.0
 Requires-Dist: tomlkit>=0.11.6
 Requires-Dist: argcomplete>=1.8.1
@@ -132,14 +132,16 @@
 .. warning ::
 
  The ``-Y`` option is incompatible with jq filters that do not expect the extra information injected into the document
  to preserve the YAML formatting. For example, a jq filter that counts entries in the Instances array will come up with
  4 entries instead of 2. A filter that expects all array entries to be mappings may break due to the presence of string
  metadata keys. Check your jq filter for compatibility/semantic validity when using the ``-Y`` option.
 
+yq does not support passing YAML comments into the JSON representation used by jq, or roundtripping such comments.
+
 XML support
 -----------
 ``yq`` also supports XML. The ``yq`` package installs an executable, ``xq``, which
 `transcodes XML to JSON <https://www.xml.com/pub/a/2006/05/31/converting-between-xml-and-json.html>`_ using
 `xmltodict <https://github.com/martinblech/xmltodict>`_ and pipes it to ``jq``. Roundtrip transcoding is available with
 the ``xq --xml-output``/``xq -x`` option. Multiple XML documents can be passed in separate files/streams as
 ``xq a.xml b.xml``. Use ``--xml-item-depth`` to descend into large documents, streaming their contents without loading
```

### Comparing `yq-3.2.3/README.rst` & `yq-3.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,16 @@
 .. warning ::
 
  The ``-Y`` option is incompatible with jq filters that do not expect the extra information injected into the document
  to preserve the YAML formatting. For example, a jq filter that counts entries in the Instances array will come up with
  4 entries instead of 2. A filter that expects all array entries to be mappings may break due to the presence of string
  metadata keys. Check your jq filter for compatibility/semantic validity when using the ``-Y`` option.
 
+yq does not support passing YAML comments into the JSON representation used by jq, or roundtripping such comments.
+
 XML support
 -----------
 ``yq`` also supports XML. The ``yq`` package installs an executable, ``xq``, which
 `transcodes XML to JSON <https://www.xml.com/pub/a/2006/05/31/converting-between-xml-and-json.html>`_ using
 `xmltodict <https://github.com/martinblech/xmltodict>`_ and pipes it to ``jq``. Roundtrip transcoding is available with
 the ``xq --xml-output``/``xq -x`` option. Multiple XML documents can be passed in separate files/streams as
 ``xq a.xml b.xml``. Use ``--xml-item-depth`` to descend into large documents, streaming their contents without loading
```

### Comparing `yq-3.2.3/SECURITY.md` & `yq-3.3.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `yq-3.2.3/common.mk` & `yq-3.3.0/common.mk`

 * *Files 5% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 	    $${EDITOR:-emacs} $$TAG_MSG; \
 	    if [[ -f Changes.md ]]; then cat $$TAG_MSG <(echo) Changes.md | sponge Changes.md; git add Changes.md; fi; \
 	    if [[ -f Changes.rst ]]; then cat <(pandoc --from markdown --to rst $$TAG_MSG) <(echo) Changes.rst | sponge Changes.rst; git add Changes.rst; fi; \
             yq --help > docs/cli-doc.txt; git add docs/cli-doc.txt; \
             xq --help > docs/cli-doc-xq.txt; git add docs/cli-doc-xq.txt; \
             tomlq --help > docs/cli-doc-tomlq.txt; git add docs/cli-doc-tomlq.txt; \
             git commit -m ${TAG}; \
-	    git tag --sign --annotate --file $$TAG_MSG ${TAG}
+	    git tag --annotate --file $$TAG_MSG ${TAG}
 	git push --follow-tags
 	$(MAKE) install
 	gh release create ${TAG} dist/*.whl --notes="$$(git tag --list ${TAG} -n99 | perl -pe 's/^\S+\s*// if $$. == 1' | sed 's/^\s\s\s\s//')"
 	$(MAKE) release-pypi
 	$(MAKE) release-docs
 
 release-pypi:
 	python -m build
-	twine upload dist/*.tar.gz dist/*.whl --sign --verbose
+	twine upload dist/*.tar.gz dist/*.whl --verbose
 
 release-docs:
 	$(MAKE) docs
 	-git branch -D gh-pages
 	git checkout -B gh-pages-stage
 	touch docs/html/.nojekyll
 	git add --force docs/html
```

### Comparing `yq-3.2.3/docs/conf.py` & `yq-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yq-3.2.3/setup.py` & `yq-3.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="yq",
-    version="3.2.3",
+    version="3.3.0",
     url="https://github.com/kislyuk/yq",
     license="Apache Software License",
     author="Andrey Kislyuk",
     author_email="kislyuk@gmail.com",
     description="Command-line YAML/XML processor - jq wrapper for YAML/XML documents",
     long_description=open("README.rst").read(),
     python_requires=">=3.6",
@@ -40,15 +40,15 @@
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `yq-3.2.3/test/cfn.yml` & `yq-3.3.0/test/cfn.yml`

 * *Files identical despite different names*

### Comparing `yq-3.2.3/test/test.py` & `yq-3.3.0/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
             tf.seek(0)
             tf2.write(b"- foo\n- bar\n")
             tf2.seek(0)
             self.run_yq("", ["-i", "-y", ".[0]", tf.name, tf2.name])
             self.assertEqual(tf.read(), b"foo\n...\n")
             self.assertEqual(tf2.read(), b"foo\n...\n")
 
-            # Files do not get overwritten on error (DeferredOutputStream logic)
+            # Files do not get overwritten on error
             self.run_yq("", ["-i", "-y", tf.name, tf2.name], expect_exit_codes=[3])
             tf.seek(0)
             tf2.seek(0)
             self.assertEqual(tf.read(), b"foo\n...\n")
             self.assertEqual(tf2.read(), b"foo\n...\n")
 
     def test_in_place_toml(self):
@@ -313,14 +313,15 @@
         self.assertEqual(self.run_yq("+685_230", ["-y", "."]), "'+685_230'\n")
         self.assertEqual(self.run_yq("+685_230", ["-y", "--yml-out-ver=1.2", "."]), "+685_230\n...\n")
 
         self.assertEqual(self.run_yq("+12345", ["-y", "."]), "12345\n...\n")
 
     def test_yaml_1_1_octals(self):
         self.assertEqual(self.run_yq("on: -012345", ["-y", "."]), "'on': -5349\n")
+        self.assertEqual(self.run_yq("on: -012349", ["-y", "."]), "'on': -012349\n")
 
     @unittest.expectedFailure
     def test_yaml_1_2_octals(self):
         """YAML 1.2 octals not yet implemented"""
         self.assertEqual(self.run_yq("on: -012345", ["-y", "--yml-out-ver=1.2", "."]), "on: -12345\n")
```

### Comparing `yq-3.2.3/yq/__init__.py` & `yq-3.3.0/yq/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,46 +38,33 @@
 def decode_docs(jq_output, json_decoder):
     while jq_output:
         doc, pos = json_decoder.raw_decode(jq_output)
         jq_output = jq_output[pos + 1 :]
         yield doc
 
 
+def get_toml_loader():
+    if sys.version_info >= (3, 11):
+        import tomllib
+
+        return tomllib.loads
+    else:
+        import tomlkit
+
+        return tomlkit.parse
+
+
 def xq_cli():
     cli(input_format="xml", program_name="xq")
 
 
 def tq_cli():
     cli(input_format="toml", program_name="tomlq")
 
 
-class DeferredOutputStream:
-    def __init__(self, name, mode="w"):
-        self.name = name
-        self.mode = mode
-        self._fh = None
-
-    @property
-    def fh(self):
-        if self._fh is None:
-            self._fh = open(self.name, self.mode)
-        return self._fh
-
-    def flush(self):
-        if self._fh is not None:
-            return self.fh.flush()
-
-    def close(self):
-        if self._fh is not None:
-            return self.fh.close()
-
-    def __getattr__(self, a):
-        return getattr(self.fh, a)
-
-
 def cli(args=None, input_format="yaml", program_name="yq"):
     parser = get_parser(program_name, __doc__)
     argcomplete.autocomplete(parser)
     args, jq_args = parser.parse_known_args(args=args)
     null_input = False
 
     for i, arg in enumerate(jq_args):
@@ -127,29 +114,33 @@
         parser.print_help()
         sys.exit(2)
     elif not args.input_streams:
         args.input_streams = [sys.stdin]
 
     yq_args = dict(input_format=input_format, program_name=program_name, jq_args=jq_args, **vars(args))
     if in_place:
-        if args.output_format not in {"yaml", "annotated_yaml", "toml"}:
-            sys.exit("{}: -i/--in-place can only be used with -y/-Y/-t".format(program_name))
+        if args.output_format not in {"yaml", "annotated_yaml", "toml", "xml"}:
+            sys.exit("{}: -i/--in-place can only be used with -y/-Y/-t/-x".format(program_name))
         input_streams = yq_args.pop("input_streams")
         if len(input_streams) == 1 and input_streams[0].name == "<stdin>":
             msg = "{}: -i/--in-place can only be used with filename arguments, not on standard input"
             sys.exit(msg.format(program_name))
         for i, input_stream in enumerate(input_streams):
 
             def exit_handler(arg=None):
                 if arg:
                     sys.exit(arg)
 
             if i < len(input_streams):
                 yq_args["exit_func"] = exit_handler
-            yq(input_streams=[input_stream], output_stream=DeferredOutputStream(input_stream.name), **yq_args)
+
+            with io.StringIO() as out_fh:
+                yq(input_streams=[input_stream], output_stream=out_fh, **yq_args)
+                with open(input_stream.name, "w") as fh:
+                    fh.write(out_fh.getvalue())
     else:
         yq(**yq_args)
 
 
 def load_yaml_docs(in_stream, out_stream, jq, loader_class, max_expansion_factor, exit_func, prog):
     loader = loader_class(in_stream)
 
@@ -213,14 +204,16 @@
             close_fds=False,
             universal_newlines=True,
         )
     except OSError as e:
         msg = "{}: Error starting jq: {}: {}. Is jq installed and available on PATH?"
         exit_func(msg.format(program_name, type(e).__name__, e))
 
+    assert jq.stdin is not None  # this is to keep mypy happy
+
     try:
         if converting_output:
             # TODO: enable true streaming in this branch (with asyncio, asyncproc, a multi-shot variant of
             # subprocess.Popen._communicate, etc.)
             # See https://stackoverflow.com/questions/375427/non-blocking-read-on-a-subprocess-pipe-in-python
             use_annotations = True if output_format == "annotated_yaml" else False
             json_buffer = io.StringIO()
@@ -242,26 +235,26 @@
                     )
                 elif input_format == "xml":
                     import xmltodict
 
                     if xml_item_depth != 0:
                         raise Exception("xml_item_depth is not supported with xq -x")
 
-                    doc = xmltodict.parse(
+                    xml_doc = xmltodict.parse(
                         input_stream.buffer if isinstance(input_stream, io.TextIOWrapper) else input_stream.read(),
                         disable_entities=True,
                         force_list=xml_force_list,
                     )
-                    json.dump(doc, json_buffer, cls=JSONDateTimeEncoder)
+                    json.dump(xml_doc, json_buffer, cls=JSONDateTimeEncoder)
                     json_buffer.write("\n")
                 elif input_format == "toml":
                     import tomlkit
 
-                    doc = tomlkit.load(input_stream)  # type: ignore
-                    json.dump(doc, json_buffer, cls=JSONDateTimeEncoder)
+                    toml_doc = tomlkit.load(input_stream)
+                    json.dump(toml_doc, json_buffer, cls=JSONDateTimeEncoder)
                     json_buffer.write("\n")
                 else:
                     raise Exception("Unknown input format")
             jq_out, jq_err = jq.communicate(json_buffer.getvalue())
             json_decoder = json.JSONDecoder()
             if output_format == "yaml" or output_format == "annotated_yaml":
                 dumper_class = get_dumper(
@@ -280,15 +273,15 @@
                     explicit_end=explicit_end,
                 )
             elif output_format == "xml":
                 import xmltodict
 
                 for doc in decode_docs(jq_out, json_decoder):
                     if xml_root:
-                        doc = {xml_root: doc}  # type: ignore
+                        doc = {xml_root: doc}
                     elif not isinstance(doc, dict):
                         msg = (
                             "{}: Error converting JSON to XML: cannot represent non-object types at top level. "
                             "Use --xml-root=name to envelope your output with a root element."
                         )
                         exit_func(msg.format(program_name))
                     full_document = True if xml_dtd else False
@@ -297,23 +290,25 @@
                             doc, output=output_stream, full_document=full_document, pretty=True, indent="  "
                         )
                     except ValueError as e:
                         if "Document must have exactly one root" in str(e):
                             raise Exception(str(e) + " Use --xml-root=name to envelope your output with a root element")
                         else:
                             raise
-                    output_stream.write(b"\n" if sys.version_info < (3, 0) else "\n")
+                    output_stream.write("\n")
             elif output_format == "toml":
                 import tomlkit
 
                 for doc in decode_docs(jq_out, json_decoder):
                     if not isinstance(doc, dict):
                         msg = "{}: Error converting JSON to TOML: cannot represent non-object types at top level."
                         exit_func(msg.format(program_name))
                     tomlkit.dump(doc, output_stream)
+            else:
+                raise Exception("Unknown output format")
         else:
             if input_format == "yaml":
                 loader_class = get_loader(
                     use_annotations=False, expand_aliases=expand_aliases, expand_merge_keys=expand_merge_keys
                 )
                 for input_stream in input_streams:
                     load_yaml_docs(
@@ -325,39 +320,40 @@
                         exit_func=exit_func,
                         prog=program_name,
                     )
             elif input_format == "xml":
                 import xmltodict
 
                 def emit_entry(path, entry):
-                    json.dump(entry, jq.stdin)  # type: ignore
-                    jq.stdin.write("\n")  # type: ignore
+                    assert jq.stdin is not None  # this is to keep mypy happy
+                    json.dump(entry, jq.stdin)
+                    jq.stdin.write("\n")
                     return True
 
                 for input_stream in input_streams:
-                    doc = xmltodict.parse(
+                    xml_doc = xmltodict.parse(
                         input_stream.buffer if isinstance(input_stream, io.TextIOWrapper) else input_stream.read(),
                         disable_entities=True,
                         force_list=xml_force_list,
                         item_depth=xml_item_depth,
                         item_callback=emit_entry,
                     )
-                    if doc:
-                        emit_entry(None, doc)
+                    if xml_doc:
+                        emit_entry(None, xml_doc)
             elif input_format == "toml":
-                import tomlkit
-
+                toml_loader = get_toml_loader()
                 for input_stream in input_streams:
-                    json.dump(tomlkit.load(input_stream), jq.stdin, cls=JSONDateTimeEncoder)  # type: ignore
-                    jq.stdin.write("\n")  # type: ignore
+                    toml_doc = toml_loader(input_stream.read())
+                    json.dump(toml_doc, jq.stdin, cls=JSONDateTimeEncoder)
+                    jq.stdin.write("\n")
             else:
                 raise Exception("Unknown input format")
 
             try:
-                jq.stdin.close()  # type: ignore
+                jq.stdin.close()
             except Exception:
                 pass
             jq.wait()
         for input_stream in input_streams:
             input_stream.close()
         exit_func(jq.returncode)
     except Exception as e:
```

### Comparing `yq-3.2.3/yq/dumper.py` & `yq-3.3.0/yq/dumper.py`

 * *Files identical despite different names*

### Comparing `yq-3.2.3/yq/loader.py` & `yq-3.3.0/yq/loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -83,21 +83,41 @@
         {
             "tag": "tag:yaml.org,2002:bool",
             "regexp": re.compile(r"^(?:|true|True|TRUE|false|False|FALSE)$", re.X),
             "start_chars": list("tTfF"),
         },
         {
             "tag": "tag:yaml.org,2002:int",
-            "regexp": re.compile(r"^(?:|0o[0-7]+|[-+]?(?:[0-9]+)|0x[0-9a-fA-F]+)$", re.X),
+            "regexp": re.compile(
+                r"""^(?:
+                # [-+]?0b[0-1_]+ # (base 2)
+                 [-+]?0[0-7]+ # (base 8)
+                |[-+]?0o[0-7]+ # (base 8)
+                |[-+]?(0|[1-9][0-9]*) # (base 10)
+                # |[-+]?0[0-7_]+ # (base 8)
+                # |[-+]?0o[0-7_]+ # (base 8)
+                # |[-+]?(0|[1-9][0-9_]*) # (base 10)
+                # |[-+]?0x[0-9a-fA-F_]+ # (base 16)
+                # |[-+]?[1-9][0-9_]*(:[0-5]?[0-9])+ # (base 60)
+                )$""",
+                re.X,
+            ),
             "start_chars": list("-+0123456789"),
         },
         {
             "tag": "tag:yaml.org,2002:float",
             "regexp": re.compile(
-                r"^(?:[-+]?(?:\.[0-9]+|[0-9]+(\.[0-9]*)?)(?:[eE][-+]?[0-9]+)?|[-+]?\.(?:inf|Inf|INF)|\.(?:nan|NaN|NAN))$",  # noqa
+                r"""^(?:
+                 [-+]?([0-9][0-9]*)?\.[0-9.]*([eE][-+][0-9]+)? (base 10)
+                |[-+]?[0-9][0-9]*(:[0-5]?[0-9])+\.[0-9]* (base 60)
+                # |[-+]?([0-9][0-9_]*)?\.[0-9.]*([eE][-+][0-9]+)? (base 10)
+                # |[-+]?[0-9][0-9_]*(:[0-5]?[0-9])+\.[0-9_]* (base 60)
+                |[-+]?\.(inf|Inf|INF) # (infinity)
+                |\.(nan|NaN|NAN) # (not a number)
+                )$""",
                 re.X,
             ),
             "start_chars": list("-+0123456789."),
         },
         {
             "tag": "tag:yaml.org,2002:null",
             "regexp": re.compile(r"^(?:~||null|Null|NULL)$", re.X),
```

### Comparing `yq-3.2.3/yq/parser.py` & `yq-3.3.0/yq/parser.py`

 * *Files identical despite different names*

### Comparing `yq-3.2.3/yq.egg-info/PKG-INFO` & `yq-3.3.0/yq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: yq
-Version: 3.2.3
+Version: 3.3.0
 Summary: Command-line YAML/XML processor - jq wrapper for YAML/XML documents
 Home-page: https://github.com/kislyuk/yq
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: PyYAML>=5.3.1
 Requires-Dist: xmltodict>=0.11.0
 Requires-Dist: tomlkit>=0.11.6
 Requires-Dist: argcomplete>=1.8.1
@@ -132,14 +132,16 @@
 .. warning ::
 
  The ``-Y`` option is incompatible with jq filters that do not expect the extra information injected into the document
  to preserve the YAML formatting. For example, a jq filter that counts entries in the Instances array will come up with
  4 entries instead of 2. A filter that expects all array entries to be mappings may break due to the presence of string
  metadata keys. Check your jq filter for compatibility/semantic validity when using the ``-Y`` option.
 
+yq does not support passing YAML comments into the JSON representation used by jq, or roundtripping such comments.
+
 XML support
 -----------
 ``yq`` also supports XML. The ``yq`` package installs an executable, ``xq``, which
 `transcodes XML to JSON <https://www.xml.com/pub/a/2006/05/31/converting-between-xml-and-json.html>`_ using
 `xmltodict <https://github.com/martinblech/xmltodict>`_ and pipes it to ``jq``. Roundtrip transcoding is available with
 the ``xq --xml-output``/``xq -x`` option. Multiple XML documents can be passed in separate files/streams as
 ``xq a.xml b.xml``. Use ``--xml-item-depth`` to descend into large documents, streaming their contents without loading
```

### Comparing `yq-3.2.3/yq.egg-info/SOURCES.txt` & `yq-3.3.0/yq.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -22,14 +22,13 @@
 test/filter.jq
 test/test.py
 yq/__init__.py
 yq/__main__.py
 yq/dumper.py
 yq/loader.py
 yq/parser.py
-yq/version.py
 yq.egg-info/PKG-INFO
 yq.egg-info/SOURCES.txt
 yq.egg-info/dependency_links.txt
 yq.egg-info/entry_points.txt
 yq.egg-info/requires.txt
 yq.egg-info/top_level.txt
```

