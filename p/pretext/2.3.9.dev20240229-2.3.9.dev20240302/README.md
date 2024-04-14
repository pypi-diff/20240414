# Comparing `tmp/pretext-2.3.9.dev20240229.tar.gz` & `tmp/pretext-2.3.9.dev20240302.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-2.3.9.dev20240229.tar", max compression
+gzip compressed data, was "pretext-2.3.9.dev20240302.tar", max compression
```

## Comparing `pretext-2.3.9.dev20240229.tar` & `pretext-2.3.9.dev20240302.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35148 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/LICENSE
--rw-r--r--   0        0        0     9757 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/README.md
--rw-r--r--   0        0        0     1505 2024-02-29 06:13:19.633708 pretext-2.3.9.dev20240229/pretext/__init__.py
--rw-r--r--   0        0        0       61 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/__main__.py
--rw-r--r--   0        0        0    28397 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/cli.py
--rw-r--r--   0        0        0     6149 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/codechat.py
--rw-r--r--   0        0        0     3310 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/constants.py
--rw-r--r--   0        0        0      714 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/core/__init__.py
--rw-r--r--   0        0        0   184007 2024-02-29 06:13:23.721711 pretext-2.3.9.dev20240229/pretext/core/pretext.py
--rw-r--r--   0        0        0     1848 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/core/resources.py
--rw-r--r--   0        0        0  1116698 2024-02-29 06:13:23.721711 pretext-2.3.9.dev20240229/pretext/core/resources.zip
--rw-r--r--   0        0        0    66064 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/project/__init__.py
--rw-r--r--   0        0        0     3329 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/project/xml.py
--rw-r--r--   0        0        0     1173 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/templates/__init__.py
--rw-r--r--   0        0        0     3149 2024-02-29 06:13:23.805711 pretext-2.3.9.dev20240229/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1939 2024-02-29 06:13:23.805711 pretext-2.3.9.dev20240229/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2024-02-29 06:13:23.805711 pretext-2.3.9.dev20240229/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160335 2024-02-29 06:13:23.793711 pretext-2.3.9.dev20240229/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0    10351 2024-02-29 06:13:23.797711 pretext-2.3.9.dev20240229/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0     3028 2024-02-29 06:13:23.805711 pretext-2.3.9.dev20240229/pretext/templates/resources/codechat_config.yaml
--rw-r--r--   0        0        0   174088 2024-02-29 06:13:23.785711 pretext-2.3.9.dev20240229/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     5045 2024-02-29 06:13:23.805711 pretext-2.3.9.dev20240229/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0      432 2024-02-29 06:13:23.805711 pretext-2.3.9.dev20240229/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2024-02-29 06:13:23.805711 pretext-2.3.9.dev20240229/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8885 2024-02-29 06:13:23.801711 pretext-2.3.9.dev20240229/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0      183 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/types.py
--rw-r--r--   0        0        0    26658 2024-02-29 06:12:51.437640 pretext-2.3.9.dev20240229/pretext/utils.py
--rw-r--r--   0        0        0     3514 2024-02-29 06:13:19.633708 pretext-2.3.9.dev20240229/pyproject.toml
--rw-r--r--   0        0        0    10923 1970-01-01 00:00:00.000000 pretext-2.3.9.dev20240229/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-03-02 06:13:55.904540 pretext-2.3.9.dev20240302/LICENSE
+-rw-r--r--   0        0        0     9757 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/README.md
+-rw-r--r--   0        0        0     1505 2024-03-02 06:14:26.060811 pretext-2.3.9.dev20240302/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/__main__.py
+-rw-r--r--   0        0        0    28397 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/cli.py
+-rw-r--r--   0        0        0     6149 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/codechat.py
+-rw-r--r--   0        0        0     3310 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/constants.py
+-rw-r--r--   0        0        0      714 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/core/__init__.py
+-rw-r--r--   0        0        0   184007 2024-03-02 06:14:29.864845 pretext-2.3.9.dev20240302/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1848 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/core/resources.py
+-rw-r--r--   0        0        0  1115903 2024-03-02 06:14:29.864845 pretext-2.3.9.dev20240302/pretext/core/resources.zip
+-rw-r--r--   0        0        0    66064 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/project/__init__.py
+-rw-r--r--   0        0        0     3329 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/project/xml.py
+-rw-r--r--   0        0        0     1173 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     3149 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/.devcontainer.json
+-rw-r--r--   0        0        0     1939 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160335 2024-03-02 06:14:29.936846 pretext-2.3.9.dev20240302/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0    10351 2024-03-02 06:14:29.940846 pretext-2.3.9.dev20240302/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0     3028 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/codechat_config.yaml
+-rw-r--r--   0        0        0   174088 2024-03-02 06:14:29.928846 pretext-2.3.9.dev20240302/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     5045 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0      432 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2024-03-02 06:14:29.948846 pretext-2.3.9.dev20240302/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8885 2024-03-02 06:14:29.944846 pretext-2.3.9.dev20240302/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0      183 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/types.py
+-rw-r--r--   0        0        0    26658 2024-03-02 06:13:55.908540 pretext-2.3.9.dev20240302/pretext/utils.py
+-rw-r--r--   0        0        0     3514 2024-03-02 06:14:26.064811 pretext-2.3.9.dev20240302/pyproject.toml
+-rw-r--r--   0        0        0    10923 1970-01-01 00:00:00.000000 pretext-2.3.9.dev20240302/PKG-INFO
```

### Comparing `pretext-2.3.9.dev20240229/LICENSE` & `pretext-2.3.9.dev20240302/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/README.md` & `pretext-2.3.9.dev20240302/README.md`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/__init__.py` & `pretext-2.3.9.dev20240302/pretext/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = '0094df7b8fc429b19befca3605ed9cf5c5ec1be3'
+CORE_COMMIT = '7aef3b1d4f73a6409da1efefef3528a3b9fb0cfa'
 
 
 def activate() -> None:
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-2.3.9.dev20240229/pretext/cli.py` & `pretext-2.3.9.dev20240302/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/codechat.py` & `pretext-2.3.9.dev20240302/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/constants.py` & `pretext-2.3.9.dev20240302/pretext/constants.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/core/__init__.py` & `pretext-2.3.9.dev20240302/pretext/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/core/pretext.py` & `pretext-2.3.9.dev20240302/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/core/resources.py` & `pretext-2.3.9.dev20240302/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/core/resources.zip` & `pretext-2.3.9.dev20240302/pretext/core/resources.zip`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,194 +1,194 @@
-Zip file size: 1116698 bytes, number of entries: 192
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 css/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 js/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 js_lib/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 script/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 xsl/utilities/
--rw-r--r--  2.0 unx     1768 b- defN 24-Feb-29 06:13 xsl/README.md
--rw-r--r--  2.0 unx     2597 b- defN 24-Feb-29 06:13 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     6066 b- defN 24-Feb-29 06:13 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    13189 b- defN 24-Feb-29 06:13 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    17295 b- defN 24-Feb-29 06:13 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx    40230 b- defN 24-Feb-29 06:13 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx    21086 b- defN 24-Feb-29 06:13 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   235477 b- defN 24-Feb-29 06:13 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   173803 b- defN 24-Feb-29 06:13 xsl/html-symbols.xsl
--rw-r--r--  2.0 unx     2248 b- defN 24-Feb-29 06:13 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx   119777 b- defN 24-Feb-29 06:13 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    22121 b- defN 24-Feb-29 06:13 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     8783 b- defN 24-Feb-29 06:13 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx    11766 b- defN 24-Feb-29 06:13 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     8130 b- defN 24-Feb-29 06:13 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     9787 b- defN 24-Feb-29 06:13 xsl/entities.ent
--rw-r--r--  2.0 unx     2847 b- defN 24-Feb-29 06:13 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx    67630 b- defN 24-Feb-29 06:13 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     2601 b- defN 24-Feb-29 06:13 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    41730 b- defN 24-Feb-29 06:13 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx     2740 b- defN 24-Feb-29 06:13 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     2709 b- defN 24-Feb-29 06:13 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     2734 b- defN 24-Feb-29 06:13 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    19092 b- defN 24-Feb-29 06:13 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     3560 b- defN 24-Feb-29 06:13 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    10708 b- defN 24-Feb-29 06:13 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    95377 b- defN 24-Feb-29 06:13 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     4571 b- defN 24-Feb-29 06:13 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     3239 b- defN 24-Feb-29 06:13 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx     8134 b- defN 24-Feb-29 06:13 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   606191 b- defN 24-Feb-29 06:13 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx   138087 b- defN 24-Feb-29 06:13 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx    13037 b- defN 24-Feb-29 06:13 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    46431 b- defN 24-Feb-29 06:13 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx     6281 b- defN 24-Feb-29 06:13 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   551514 b- defN 24-Feb-29 06:13 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    12084 b- defN 24-Feb-29 06:13 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx    39918 b- defN 24-Feb-29 06:13 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx   114772 b- defN 24-Feb-29 06:13 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx   555385 b- defN 24-Feb-29 06:13 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     4810 b- defN 24-Feb-29 06:13 xsl/localizations/README.md
--rw-r--r--  2.0 unx    16378 b- defN 24-Feb-29 06:13 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    16566 b- defN 24-Feb-29 06:13 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    15924 b- defN 24-Feb-29 06:13 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    15648 b- defN 24-Feb-29 06:13 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17147 b- defN 24-Feb-29 06:13 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16904 b- defN 24-Feb-29 06:13 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    19251 b- defN 24-Feb-29 06:13 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16151 b- defN 24-Feb-29 06:13 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16415 b- defN 24-Feb-29 06:13 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17297 b- defN 24-Feb-29 06:13 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    20546 b- defN 24-Feb-29 06:13 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    19076 b- defN 24-Feb-29 06:13 xsl/localizations/zh-HANS.xml
--rw-r--r--  2.0 unx    17122 b- defN 24-Feb-29 06:13 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    16600 b- defN 24-Feb-29 06:13 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    17368 b- defN 24-Feb-29 06:13 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx     2347 b- defN 24-Feb-29 06:13 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    19453 b- defN 24-Feb-29 06:13 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    16318 b- defN 24-Feb-29 06:13 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx     1810 b- defN 24-Feb-29 06:13 xsl/utilities/README.md
--rw-r--r--  2.0 unx     4299 b- defN 24-Feb-29 06:13 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     4926 b- defN 24-Feb-29 06:13 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      787 b- defN 24-Feb-29 06:13 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 24-Feb-29 06:13 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx      513 b- defN 24-Feb-29 06:13 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx    14322 b- defN 24-Feb-29 06:13 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     3024 b- defN 24-Feb-29 06:13 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     7277 b- defN 24-Feb-29 06:13 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     5135 b- defN 24-Feb-29 06:13 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2261 b- defN 24-Feb-29 06:13 xsl/latex/pretext-latex-AIM.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 24-Feb-29 06:13 xsl/support/README.md
--rw-r--r--  2.0 unx    10300 b- defN 24-Feb-29 06:13 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 24-Feb-29 06:13 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 24-Feb-29 06:13 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5061 b- defN 24-Feb-29 06:13 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5800 b- defN 24-Feb-29 06:13 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      521 b- defN 24-Feb-29 06:13 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     2657 b- defN 24-Feb-29 06:13 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 24-Feb-29 06:13 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 24-Feb-29 06:13 xsl/support/play-button/play-button.png
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 24-Feb-29 06:13 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 24-Feb-29 06:13 script/mbx
--rw-r--r--  2.0 unx      481 b- defN 24-Feb-29 06:13 script/mjsre/README.md
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-29 06:13 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 24-Feb-29 06:13 script/mjsre/package.json
--rw-r--r--  2.0 unx     9251 b- defN 24-Feb-29 06:13 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx     1367 b- defN 24-Feb-29 06:13 pretext/README.md
--rw-r--r--  2.0 unx    36176 b- defN 24-Feb-29 06:13 pretext/braille_format.py
--rw-r--r--  2.0 unx     1955 b- defN 24-Feb-29 06:13 pretext/module-test.py
--rw-r--r--  2.0 unx   184007 b- defN 24-Feb-29 06:13 pretext/pretext.py
--rw-r--r--  2.0 unx      215 b- defN 24-Feb-29 06:13 pretext/requirements.txt
--rw-r--r--  2.0 unx    30970 b- defN 24-Feb-29 06:13 pretext/pretext
--rw-r--r--  2.0 unx     2566 b- defN 24-Feb-29 06:13 pretext/pretext.cfg
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-29 06:13 pretext/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 js/pretext-webwork/
--rw-r--r--  2.0 unx    42973 b- defN 24-Feb-29 06:13 js/pretext_add_on.js
--rw-r--r--  2.0 unx    10957 b- defN 24-Feb-29 06:13 js/login.js
--rw-r--r--  2.0 unx     6509 b- defN 24-Feb-29 06:13 js/pretext.js
--rw-r--r--  2.0 unx   228054 b- defN 24-Feb-29 06:13 js/edit.js
--rw-r--r--  2.0 unx    12113 b- defN 24-Feb-29 06:13 js/pretext_search.js
--rw-r--r--  2.0 unx     5318 b- defN 24-Feb-29 06:13 js/instructor.js
--rw-r--r--  2.0 unx    25633 b- defN 24-Feb-29 06:13 js/answer.js
--rw-r--r--  2.0 unx     3693 b- defN 24-Feb-29 06:13 js/ptx_search.js
--rw-r--r--  2.0 unx    23560 b- defN 24-Feb-29 06:13 js/highlight.js
--rw-r--r--  2.0 unx    20911 b- defN 24-Feb-29 06:13 js/user_preferences.js
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 js/pretext-webwork/2.16/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 js/pretext-webwork/2.17/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:13 js/pretext-webwork/2.18/
--rw-r--r--  2.0 unx    44152 b- defN 24-Feb-29 06:13 js/pretext-webwork/2.18/pretext-webwork.js
--rw-r--r--  2.0 unx    37123 b- defN 24-Feb-29 06:13 js/pretext-webwork/2.16/pretext-webwork.js
--rw-r--r--  2.0 unx    44152 b- defN 24-Feb-29 06:13 js/pretext-webwork/2.17/pretext-webwork.js
--rw-r--r--  2.0 unx     1180 b- defN 24-Feb-29 06:13 schema/README.md
--rw-r--r--  2.0 unx     3135 b- defN 24-Feb-29 06:13 schema/build.sh
--rw-r--r--  2.0 unx   103777 b- defN 24-Feb-29 06:13 schema/pretext.rng
--rw-r--r--  2.0 unx   127312 b- defN 24-Feb-29 06:13 schema/pretext.xsd
--rw-r--r--  2.0 unx    17572 b- defN 24-Feb-29 06:13 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx    18421 b- defN 24-Feb-29 06:13 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    58885 b- defN 24-Feb-29 06:13 schema/pretext.rnc
--rw-r--r--  2.0 unx    25870 b- defN 24-Feb-29 06:13 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx      326 b- defN 24-Feb-29 06:13 schema/xml.xsd
--rw-r--r--  2.0 unx    34176 b- defN 24-Feb-29 06:13 schema/pretext-dev.rng
--rw-r--r--  2.0 unx      162 b- defN 24-Feb-29 06:13 schema/publication.xml
--rw-r--r--  2.0 unx   134640 b- defN 24-Feb-29 06:13 schema/pretext.xml
--rw-r--r--  2.0 unx     6674 b- defN 24-Feb-29 06:13 js_lib/jquery.espy.min.js
--rw-r--r--  2.0 unx     1390 b- defN 24-Feb-29 06:13 js_lib/mathjaxknowl3.js
--rw-r--r--  2.0 unx    12019 b- defN 24-Feb-29 06:13 js_lib/knowl.js
--rw-r--r--  2.0 unx    86927 b- defN 24-Feb-29 06:13 js_lib/jquery.min.js
--rw-r--r--  2.0 unx     3238 b- defN 24-Feb-29 06:13 js_lib/mathjaxknowl.js
--rw-r--r--  2.0 unx     5275 b- defN 24-Feb-29 06:13 js_lib/jquery.sticky.js
--rw-r--r--  2.0 unx     8496 b- defN 24-Feb-29 06:13 css/shell_crc.css
--rw-r--r--  2.0 unx     1255 b- defN 24-Feb-29 06:13 css/colors_focused_gray_aqua.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Feb-29 06:13 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Feb-29 06:13 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     1683 b- defN 24-Feb-29 06:13 css/catalog.css
--rw-r--r--  2.0 unx      691 b- defN 24-Feb-29 06:13 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1280 b- defN 24-Feb-29 06:13 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     6966 b- defN 24-Feb-29 06:13 css/navbar_crc.css
--rw-r--r--  2.0 unx     1330 b- defN 24-Feb-29 06:13 css/reveal.css
--rw-r--r--  2.0 unx     3769 b- defN 24-Feb-29 06:13 css/navbar_default.css
--rw-r--r--  2.0 unx     5374 b- defN 24-Feb-29 06:13 css/shell_default.css
--rw-r--r--  2.0 unx    27804 b- defN 24-Feb-29 06:13 css/pretext.css
--rw-r--r--  2.0 unx      389 b- defN 24-Feb-29 06:13 css/banner_wide.css
--rw-r--r--  2.0 unx    13638 b- defN 24-Feb-29 06:13 css/style_oscarlevin.css
--rw-r--r--  2.0 unx      533 b- defN 24-Feb-29 06:13 css/toc_wide.css
--rw-r--r--  2.0 unx     3757 b- defN 24-Feb-29 06:13 css/colors_blue_red_dark.css
--rw-r--r--  2.0 unx     1276 b- defN 24-Feb-29 06:13 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Feb-29 06:13 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2446 b- defN 24-Feb-29 06:13 css/colors_martiansands.css
--rw-r--r--  2.0 unx     8179 b- defN 24-Feb-29 06:13 css/style_default.css
--rw-r--r--  2.0 unx     2781 b- defN 24-Feb-29 06:13 css/colors_default.css
--rw-r--r--  2.0 unx     5072 b- defN 24-Feb-29 06:13 css/knowls_default.css
--rw-r--r--  2.0 unx     3473 b- defN 24-Feb-29 06:13 css/style_soundwriting.css
--rw-r--r--  2.0 unx     4308 b- defN 24-Feb-29 06:13 css/colors_blue_green.css
--rw-r--r--  2.0 unx     2720 b- defN 24-Feb-29 06:13 css/pretext_search.css
--rw-r--r--  2.0 unx     2441 b- defN 24-Feb-29 06:13 css/kindle.css
--rw-r--r--  2.0 unx      679 b- defN 24-Feb-29 06:13 css/navbar_wide.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Feb-29 06:13 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     4236 b- defN 24-Feb-29 06:13 css/style_wide.css
--rw-r--r--  2.0 unx     6012 b- defN 24-Feb-29 06:13 css/features.css
--rw-r--r--  2.0 unx     4348 b- defN 24-Feb-29 06:13 css/colors_bluegreen_grey.css
--rw-r--r--  2.0 unx     3240 b- defN 24-Feb-29 06:13 css/banner_default.css
--rw-r--r--  2.0 unx     8096 b- defN 24-Feb-29 06:13 css/toc_crc.css
--rw-r--r--  2.0 unx     2438 b- defN 24-Feb-29 06:13 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     1102 b- defN 24-Feb-29 06:13 css/webwork.css
--rw-r--r--  2.0 unx     5875 b- defN 24-Feb-29 06:13 css/banner_crc.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Feb-29 06:13 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Feb-29 06:13 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx    14341 b- defN 24-Feb-29 06:13 css/setcolors.css
--rw-r--r--  2.0 unx     1207 b- defN 24-Feb-29 06:13 css/colors_focused_light.css
--rw-r--r--  2.0 unx     5836 b- defN 24-Feb-29 06:13 css/shell_min.css
--rw-r--r--  2.0 unx    75010 b- defN 24-Feb-29 06:13 css/pretext_add_on.css
--rw-r--r--  2.0 unx    10602 b- defN 24-Feb-29 06:13 css/edit.css
--rw-r--r--  2.0 unx     2446 b- defN 24-Feb-29 06:13 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     1338 b- defN 24-Feb-29 06:13 css/colors_red_blue.css
--rw-r--r--  2.0 unx     1362 b- defN 24-Feb-29 06:13 css/epub.css
--rw-r--r--  2.0 unx     9821 b- defN 24-Feb-29 06:13 css/toc_default.css
--rw-r--r--  2.0 unx     7521 b- defN 24-Feb-29 06:13 css/shell_wide.css
--rw-r--r--  2.0 unx     3818 b- defN 24-Feb-29 06:13 css/toc_min.css
--rw-r--r--  2.0 unx     2397 b- defN 24-Feb-29 06:13 css/colors_green_blue.css
-192 files, 5176748 bytes uncompressed, 1093284 bytes compressed:  78.9%
+Zip file size: 1115903 bytes, number of entries: 192
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 css/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js_lib/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 script/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/utilities/
+-rw-r--r--  2.0 unx     1768 b- defN 24-Mar-02 06:14 xsl/README.md
+-rw-r--r--  2.0 unx     2597 b- defN 24-Mar-02 06:14 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 24-Mar-02 06:14 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    13189 b- defN 24-Mar-02 06:14 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    17295 b- defN 24-Mar-02 06:14 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 24-Mar-02 06:14 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 24-Mar-02 06:14 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   235477 b- defN 24-Mar-02 06:14 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   173803 b- defN 24-Mar-02 06:14 xsl/html-symbols.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 24-Mar-02 06:14 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   119777 b- defN 24-Mar-02 06:14 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 24-Mar-02 06:14 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     8783 b- defN 24-Mar-02 06:14 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 24-Mar-02 06:14 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 24-Mar-02 06:14 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 24-Mar-02 06:14 xsl/entities.ent
+-rw-r--r--  2.0 unx     2847 b- defN 24-Mar-02 06:14 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx    67630 b- defN 24-Mar-02 06:14 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 24-Mar-02 06:14 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 24-Mar-02 06:14 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 24-Mar-02 06:14 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 24-Mar-02 06:14 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     2734 b- defN 24-Mar-02 06:14 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    19092 b- defN 24-Mar-02 06:14 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 24-Mar-02 06:14 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 24-Mar-02 06:14 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    95377 b- defN 24-Mar-02 06:14 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 24-Mar-02 06:14 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 24-Mar-02 06:14 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx     8134 b- defN 24-Mar-02 06:14 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   606337 b- defN 24-Mar-02 06:14 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx   138087 b- defN 24-Mar-02 06:14 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 24-Mar-02 06:14 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    46431 b- defN 24-Mar-02 06:14 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 24-Mar-02 06:14 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   551514 b- defN 24-Mar-02 06:14 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 24-Mar-02 06:14 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 24-Mar-02 06:14 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx   114772 b- defN 24-Mar-02 06:14 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx   556693 b- defN 24-Mar-02 06:14 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     4810 b- defN 24-Mar-02 06:14 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    16378 b- defN 24-Mar-02 06:14 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    16566 b- defN 24-Mar-02 06:14 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    15924 b- defN 24-Mar-02 06:14 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    15648 b- defN 24-Mar-02 06:14 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17147 b- defN 24-Mar-02 06:14 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16904 b- defN 24-Mar-02 06:14 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    19251 b- defN 24-Mar-02 06:14 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16151 b- defN 24-Mar-02 06:14 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16415 b- defN 24-Mar-02 06:14 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17297 b- defN 24-Mar-02 06:14 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    20546 b- defN 24-Mar-02 06:14 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    19076 b- defN 24-Mar-02 06:14 xsl/localizations/zh-HANS.xml
+-rw-r--r--  2.0 unx    17122 b- defN 24-Mar-02 06:14 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16600 b- defN 24-Mar-02 06:14 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    17368 b- defN 24-Mar-02 06:14 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx     2347 b- defN 24-Mar-02 06:14 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    19453 b- defN 24-Mar-02 06:14 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    16318 b- defN 24-Mar-02 06:14 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx     1810 b- defN 24-Mar-02 06:14 xsl/utilities/README.md
+-rw-r--r--  2.0 unx     4299 b- defN 24-Mar-02 06:14 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 24-Mar-02 06:14 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      787 b- defN 24-Mar-02 06:14 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx    30257 b- defN 24-Mar-02 06:14 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx      513 b- defN 24-Mar-02 06:14 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx    14322 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     7277 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 24-Mar-02 06:14 xsl/latex/pretext-latex-AIM.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 24-Mar-02 06:14 xsl/support/README.md
+-rw-r--r--  2.0 unx    10300 b- defN 24-Mar-02 06:14 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 24-Mar-02 06:14 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 24-Mar-02 06:14 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5061 b- defN 24-Mar-02 06:14 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 24-Mar-02 06:14 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      521 b- defN 24-Mar-02 06:14 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     2657 b- defN 24-Mar-02 06:14 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 24-Mar-02 06:14 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 24-Mar-02 06:14 xsl/support/play-button/play-button.png
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 24-Mar-02 06:14 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 24-Mar-02 06:14 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 24-Mar-02 06:14 script/mjsre/README.md
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-02 06:14 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      116 b- defN 24-Mar-02 06:14 script/mjsre/package.json
+-rw-r--r--  2.0 unx     9251 b- defN 24-Mar-02 06:14 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx     1367 b- defN 24-Mar-02 06:14 pretext/README.md
+-rw-r--r--  2.0 unx    36176 b- defN 24-Mar-02 06:14 pretext/braille_format.py
+-rw-r--r--  2.0 unx     1955 b- defN 24-Mar-02 06:14 pretext/module-test.py
+-rw-r--r--  2.0 unx   184007 b- defN 24-Mar-02 06:14 pretext/pretext.py
+-rw-r--r--  2.0 unx      215 b- defN 24-Mar-02 06:14 pretext/requirements.txt
+-rw-r--r--  2.0 unx    30970 b- defN 24-Mar-02 06:14 pretext/pretext
+-rw-r--r--  2.0 unx     2566 b- defN 24-Mar-02 06:14 pretext/pretext.cfg
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-02 06:14 pretext/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/pretext-webwork/
+-rw-r--r--  2.0 unx    42973 b- defN 24-Mar-02 06:14 js/pretext_add_on.js
+-rw-r--r--  2.0 unx    10957 b- defN 24-Mar-02 06:14 js/login.js
+-rw-r--r--  2.0 unx     6509 b- defN 24-Mar-02 06:14 js/pretext.js
+-rw-r--r--  2.0 unx   228054 b- defN 24-Mar-02 06:14 js/edit.js
+-rw-r--r--  2.0 unx    12113 b- defN 24-Mar-02 06:14 js/pretext_search.js
+-rw-r--r--  2.0 unx     5318 b- defN 24-Mar-02 06:14 js/instructor.js
+-rw-r--r--  2.0 unx    25633 b- defN 24-Mar-02 06:14 js/answer.js
+-rw-r--r--  2.0 unx     3693 b- defN 24-Mar-02 06:14 js/ptx_search.js
+-rw-r--r--  2.0 unx    23560 b- defN 24-Mar-02 06:14 js/highlight.js
+-rw-r--r--  2.0 unx    20911 b- defN 24-Mar-02 06:14 js/user_preferences.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/pretext-webwork/2.16/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/pretext-webwork/2.17/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:14 js/pretext-webwork/2.18/
+-rw-r--r--  2.0 unx    44152 b- defN 24-Mar-02 06:14 js/pretext-webwork/2.18/pretext-webwork.js
+-rw-r--r--  2.0 unx    37123 b- defN 24-Mar-02 06:14 js/pretext-webwork/2.16/pretext-webwork.js
+-rw-r--r--  2.0 unx    44152 b- defN 24-Mar-02 06:14 js/pretext-webwork/2.17/pretext-webwork.js
+-rw-r--r--  2.0 unx     1180 b- defN 24-Mar-02 06:14 schema/README.md
+-rw-r--r--  2.0 unx     3135 b- defN 24-Mar-02 06:14 schema/build.sh
+-rw-r--r--  2.0 unx   103777 b- defN 24-Mar-02 06:14 schema/pretext.rng
+-rw-r--r--  2.0 unx   127312 b- defN 24-Mar-02 06:14 schema/pretext.xsd
+-rw-r--r--  2.0 unx    17572 b- defN 24-Mar-02 06:14 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx    18421 b- defN 24-Mar-02 06:14 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    58885 b- defN 24-Mar-02 06:14 schema/pretext.rnc
+-rw-r--r--  2.0 unx    25870 b- defN 24-Mar-02 06:14 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx      326 b- defN 24-Mar-02 06:14 schema/xml.xsd
+-rw-r--r--  2.0 unx    34176 b- defN 24-Mar-02 06:14 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx      162 b- defN 24-Mar-02 06:14 schema/publication.xml
+-rw-r--r--  2.0 unx   134640 b- defN 24-Mar-02 06:14 schema/pretext.xml
+-rw-r--r--  2.0 unx     6674 b- defN 24-Mar-02 06:14 js_lib/jquery.espy.min.js
+-rw-r--r--  2.0 unx     1390 b- defN 24-Mar-02 06:14 js_lib/mathjaxknowl3.js
+-rw-r--r--  2.0 unx    12611 b- defN 24-Mar-02 06:14 js_lib/knowl.js
+-rw-r--r--  2.0 unx    86927 b- defN 24-Mar-02 06:14 js_lib/jquery.min.js
+-rw-r--r--  2.0 unx     3177 b- defN 24-Mar-02 06:14 js_lib/mathjaxknowl.js
+-rw-r--r--  2.0 unx     5275 b- defN 24-Mar-02 06:14 js_lib/jquery.sticky.js
+-rw-r--r--  2.0 unx     8496 b- defN 24-Mar-02 06:14 css/shell_crc.css
+-rw-r--r--  2.0 unx     1255 b- defN 24-Mar-02 06:14 css/colors_focused_gray_aqua.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     1683 b- defN 24-Mar-02 06:14 css/catalog.css
+-rw-r--r--  2.0 unx      691 b- defN 24-Mar-02 06:14 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1280 b- defN 24-Mar-02 06:14 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     6966 b- defN 24-Mar-02 06:14 css/navbar_crc.css
+-rw-r--r--  2.0 unx     1330 b- defN 24-Mar-02 06:14 css/reveal.css
+-rw-r--r--  2.0 unx     3769 b- defN 24-Mar-02 06:14 css/navbar_default.css
+-rw-r--r--  2.0 unx     5374 b- defN 24-Mar-02 06:14 css/shell_default.css
+-rw-r--r--  2.0 unx    24707 b- defN 24-Mar-02 06:14 css/pretext.css
+-rw-r--r--  2.0 unx      389 b- defN 24-Mar-02 06:14 css/banner_wide.css
+-rw-r--r--  2.0 unx    13638 b- defN 24-Mar-02 06:14 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx      533 b- defN 24-Mar-02 06:14 css/toc_wide.css
+-rw-r--r--  2.0 unx     3757 b- defN 24-Mar-02 06:14 css/colors_blue_red_dark.css
+-rw-r--r--  2.0 unx     1276 b- defN 24-Mar-02 06:14 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2446 b- defN 24-Mar-02 06:14 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     8179 b- defN 24-Mar-02 06:14 css/style_default.css
+-rw-r--r--  2.0 unx     2781 b- defN 24-Mar-02 06:14 css/colors_default.css
+-rw-r--r--  2.0 unx     1804 b- defN 24-Mar-02 06:14 css/knowls_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 24-Mar-02 06:14 css/style_soundwriting.css
+-rw-r--r--  2.0 unx     4308 b- defN 24-Mar-02 06:14 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2720 b- defN 24-Mar-02 06:14 css/pretext_search.css
+-rw-r--r--  2.0 unx     2441 b- defN 24-Mar-02 06:14 css/kindle.css
+-rw-r--r--  2.0 unx      679 b- defN 24-Mar-02 06:14 css/navbar_wide.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     4236 b- defN 24-Mar-02 06:14 css/style_wide.css
+-rw-r--r--  2.0 unx     6012 b- defN 24-Mar-02 06:14 css/features.css
+-rw-r--r--  2.0 unx     4348 b- defN 24-Mar-02 06:14 css/colors_bluegreen_grey.css
+-rw-r--r--  2.0 unx     3240 b- defN 24-Mar-02 06:14 css/banner_default.css
+-rw-r--r--  2.0 unx     8096 b- defN 24-Mar-02 06:14 css/toc_crc.css
+-rw-r--r--  2.0 unx     2438 b- defN 24-Mar-02 06:14 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     1102 b- defN 24-Mar-02 06:14 css/webwork.css
+-rw-r--r--  2.0 unx     5875 b- defN 24-Mar-02 06:14 css/banner_crc.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx    14207 b- defN 24-Mar-02 06:14 css/setcolors.css
+-rw-r--r--  2.0 unx     1207 b- defN 24-Mar-02 06:14 css/colors_focused_light.css
+-rw-r--r--  2.0 unx     5836 b- defN 24-Mar-02 06:14 css/shell_min.css
+-rw-r--r--  2.0 unx    74960 b- defN 24-Mar-02 06:14 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    10602 b- defN 24-Mar-02 06:14 css/edit.css
+-rw-r--r--  2.0 unx     2446 b- defN 24-Mar-02 06:14 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     1338 b- defN 24-Mar-02 06:14 css/colors_red_blue.css
+-rw-r--r--  2.0 unx     1362 b- defN 24-Mar-02 06:14 css/epub.css
+-rw-r--r--  2.0 unx     9821 b- defN 24-Mar-02 06:14 css/toc_default.css
+-rw-r--r--  2.0 unx     7521 b- defN 24-Mar-02 06:14 css/shell_wide.css
+-rw-r--r--  2.0 unx     3818 b- defN 24-Mar-02 06:14 css/toc_min.css
+-rw-r--r--  2.0 unx     2397 b- defN 24-Mar-02 06:14 css/colors_green_blue.css
+192 files, 5172184 bytes uncompressed, 1092489 bytes compressed:  78.9%
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -2651,15 +2651,15 @@
       </xsl:if>
       <!-- put relevant class names on "details" to help with styling -->
       <xsl:attribute name="class">
         <xsl:apply-templates select="." mode="body-css-class"/>
         <xsl:text>born-hidden-knowl</xsl:text>
       </xsl:attribute>
       <!-- the clickable that is visible on the page -->
-      <summary>
+      <summary class="knowl__link">
         <xsl:apply-templates select="." mode="heading-birth"/>
       </summary>
       <!-- the content of the knowl, to be revealed later        -->
       <!-- NB: the Javascript controlling the animation of the   -->
       <!-- open/close of a knowl, presumes it begins with an     -->
       <!-- element enclosing the content.  This is guaranteed by -->
       <!-- the "body" template via the "body-element" template.  -->
@@ -4726,14 +4726,17 @@
     </xsl:if>
     <xsl:variable name="body-elt">
       <xsl:apply-templates select="." mode="body-element"/>
     </xsl:variable>
     <xsl:element name="{$body-elt}">
       <xsl:attribute name="class">
         <xsl:apply-templates select="." mode="body-css-class"/>
+        <xsl:if test="$block-type = 'hidden'">
+          <xsl:text>knowl__content</xsl:text>
+        </xsl:if>
       </xsl:attribute>
       <!-- Label original, but not if embedded            -->
       <!-- Then id goes onto the knowl text, so locatable -->
       <xsl:if test="$b-original and not($block-type = 'hidden')">
         <xsl:apply-templates select="." mode="html-id-attribute"/>
         <xsl:apply-templates select="." mode="permid-attribute"/>
       </xsl:if>
```

#### xsl/pretext-common.xsl

##### xsl/pretext-common.xsl

```diff
@@ -3164,16 +3164,16 @@
     <!-- override, set the context to $root in the employing @select, -->
     <!-- then $lang-element *will* be $root and $lang *will* be the   -->
     <!-- overall, document-wide, language (set by -assembly).         -->
     <xsl:variable name="lang-element" select="ancestor-or-self::*[@locale-lang][1]"/>
     <xsl:variable name="lang">
       <xsl:value-of select="$lang-element/@locale-lang"/>
     </xsl:variable>
-    <!-- Now, build the actual translation -->
-    <xsl:variable name="translation">
+    <!-- Now, build the actual translation via a lookup -->
+    <xsl:variable name="lookup">
       <xsl:choose>
         <!-- First, look in docinfo for document-specific rename with correct language -->
         <xsl:when test="$docinfo/rename[@element=$str-id and @xml:lang=$lang]">
           <xsl:apply-templates select="$docinfo/rename[@element=$str-id and @xml:lang=$lang]"/>
         </xsl:when>
         <!-- Second, look in docinfo for document-specific rename with correct language, -->
         <!-- but with @lang attribute which was deprecated on 2019-02-23                 -->
@@ -3190,14 +3190,41 @@
         <xsl:otherwise>
           <xsl:for-each select="$localizations/locale[@language = $lang]">
             <xsl:value-of select="key('localization-key', $str-id)"/>
           </xsl:for-each>
         </xsl:otherwise>
       </xsl:choose>
     </xsl:variable>
+    <!-- Exceptions to failed lookups                     -->
+    <!-- Some un-implemented translations are ubiquitous, -->
+    <!-- so we recognize failure and fallback to English  -->
+    <xsl:variable name="translation">
+      <xsl:choose>
+        <!-- $lookup is good, echo it -->
+        <xsl:when test="not($lookup = '')">
+          <xsl:value-of select="$lookup"/>
+        </xsl:when>
+        <!-- substitute English since $lookup is empty     -->
+        <!-- NB: could test with an "or" for multiple      -->
+        <!-- exceptions and then get en-US version with a  -->
+        <!-- proper lookup as a single statement, but not  -->
+        <!-- bothering yet.                                -->
+        <!-- "Close" is on every knowl, too many warnings  -->
+        <xsl:when test="$str-id = 'close'">
+          <xsl:text>Close</xsl:text>
+        </xsl:when>
+        <!-- "Reveal" is on every knowl, too many warnings -->
+        <xsl:when test="$str-id = 'reveal'">
+          <xsl:text>Reveal</xsl:text>
+        </xsl:when>
+        <!-- $lookup empty and not exceptional    -->
+        <!-- echo the empty lookup as translation -->
+        <xsl:otherwise/>
+      </xsl:choose>
+    </xsl:variable>
     <xsl:choose>
       <xsl:when test="$translation != ''">
         <xsl:value-of select="$translation"/>
       </xsl:when>
       <xsl:otherwise>
         <xsl:text>[</xsl:text>
         <xsl:value-of select="$str-id"/>
```

#### js_lib/knowl.js

##### js-beautify {}

```diff
@@ -13,15 +13,14 @@
 
     const bornHiddens = target.querySelectorAll(".born-hidden-knowl");
     for (const bhk of bornHiddens) {
         const summary = bhk.querySelector(":scope > summary");
         const contents = bhk.querySelector(":scope > summary + *");
         new SlideRevealer(summary, contents, bhk);
     }
-
 }
 
 // Used to animate both types of knowls
 class SlideRevealer {
     static STATE = Object.freeze({
         INACTIVE: 0,
         CLOSING: 1,
@@ -48,45 +47,56 @@
         // Stop default behavior from the browser
         if (e) e.preventDefault();
 
         // Add an overflow on the <details> to avoid content overflowing
         this.animatedElement.style.overflow = 'hidden';
 
         // Check if the element is being closed or is already closed
-        if (this.animationState === SlideRevealer.STATE.CLOSING || !this.animatedElement.open) {
-            // Force the [open] attribute (needed if animated element is details)
-            this.animatedElement.open = true;
+        if (this.animationState === SlideRevealer.STATE.CLOSING || !this.animatedElement.hasAttribute("open")) {
+            // Force the [open] attributes - allow for similar targetting of xref and born-hidden knowls
+            this.animatedElement.setAttribute("open", "");
+            this.triggerElement.setAttribute("open", "");
             this.contentElement.style.display = '';
             // Wait for the next frame to call the toggle function
             window.requestAnimationFrame(() => this.toggle(true));
-        } else if (this.animationState === SlideRevealer.STATE.EXPANDING || this.animatedElement.open) {
+        } else if (this.animationState === SlideRevealer.STATE.EXPANDING || this.animatedElement.hasAttribute("open")) {
             this.toggle(false);
         }
     }
 
     toggle(expanding) {
         let closedHeight = 0;
         if (this.animatedElement.contains(this.triggerElement))
             closedHeight = this.triggerElement.offsetHeight;
         const fullHeight = closedHeight + this.contentElement.offsetHeight;
 
         const startHeight = `${expanding ? closedHeight : fullHeight}px`;
         const endHeight = `${expanding ? fullHeight : closedHeight}px`;
 
+        // Need to animate padding to avoid extra height for xref knowls
+        const padding = this.animatedElement.offsetHeight - this.animatedElement.clientHeight;
+        const startPad = `${expanding ? 0 : padding}px`;
+        const endPad = `${expanding ? padding : 0}px`;
+
         // Cancel any existing animation
         if (this.animation) {
             this.animation.cancel();
         }
 
+        // Animate ~400 pixels per second with max of 0.75 second and min of 0.25
+        const animDuration = Math.max(Math.min((Math.abs(closedHeight - fullHeight) / 400 * 1000), 750), 250);
+
         // Start animation
         this.animationState = expanding ? SlideRevealer.STATE.EXPANDING : SlideRevealer.STATE.CLOSING;
         this.animation = this.animatedElement.animate({
-            height: [startHeight, endHeight]
+            height: [startHeight, endHeight],
+            paddingTop: [startPad, endPad],
+            paddingBottom: [startPad, endPad]
         }, {
-            duration: 400,
+            duration: animDuration,
             easing: 'ease'
         });
 
         this.animation.onfinish = () => {
             this.onAnimationFinish(expanding);
         };
         this.animation.oncancel = () => {
@@ -96,18 +106,21 @@
 
     onAnimationFinish(isOpen) {
         // Clear animation state
         this.animation = null;
         this.animationState = SlideRevealer.STATE.INACTIVE;
 
         // Make sure animated element has open (needed for details)
-        this.animatedElement.open = isOpen;
+        if (!isOpen) {
+            this.animatedElement.removeAttribute("open");
+            this.triggerElement.removeAttribute("open");
+        }
 
         // Clear styles used in animation
-        this.animatedElement.style.height = this.animatedElement.style.overflow = '';
+        this.animatedElement.style.overflow = '';
         if (!isOpen)
             this.contentElement.style.display = 'none';
     }
 }
 
 
 
@@ -135,14 +148,16 @@
         // Xref's behavior is that of a button
         knowlLinkElement.setAttribute("role", "button");
 
         // Stash a copy of the original title for use in aria-label
         // If no title, use textContent
         knowlLinkElement.setAttribute("data-base-title", knowlLinkElement.getAttribute("title") || this.linkElement.textContent);
 
+        knowlLinkElement.classList.add("knowl__link");
+
         this.updateLabels(false);
 
         // Bind required to force "this" of event handler to be this object
         knowlLinkElement.addEventListener("click", this.handleLinkClick.bind(this));
     }
 
     // Set aria-label and title based on visibility of knowl
@@ -193,21 +208,17 @@
 
     // Create the knowl output element
     createOutputElement() {
         const outputId = "knowl-uid-" + this.uid;
         const outputContentsId = "knowl-output-" + this.uid;
         const linkTarget = this.linkElement.getAttribute("data-knowl");
 
-        const placeholderText = `<div class='knowl-output' style='display:none;' id='${outputId}' aria-live='polite'>` +
-            `<div class='knowl'>` +
-            `<div class='knowl-content' id='${outputContentsId}'>` +
+        const placeholderText = `<div class='knowl__content' style='display:none;' id='${outputId}' aria-live='polite' id='${outputContentsId}'>` +
             `Loading '${linkTarget}'` +
-            `</div>` +
-            `<div class='knowl-footer'>${linkTarget}</div>` +
-            `</div></div></div>`;
+            `</div>`;
 
         const temp = document.createElement("template");
         temp.innerHTML = placeholderText;
         this.outputElement = temp.content.children[0];
 
         const insertLoc = this.findOutputLocation(this.linkElement);
         insertLoc.after(this.outputElement);
@@ -289,25 +300,24 @@
                         } else {
                             // let runestone start rendering it
                             window.runestoneComponents.renderOneComponent(e);
                         }
                     });
 
                     // now move all contents to the real output element
-                    const target = document.getElementById("knowl-output-" + this.uid);
                     const children = [...tempContainer.children];
-                    target.innerHTML = "";
-                    target.append(...children);
+                    this.outputElement.innerHTML = "";
+                    this.outputElement.append(...children);
 
                     // render any knowls and mathjax in the knowl
-                    MathJax.typesetPromise([target]);
-                    addKnowls(target);
+                    MathJax.typesetPromise([this.outputElement]);
+                    addKnowls(this.outputElement);
 
                     // force any scripts (e.g. sagecell) to execute by evaling them
-                    [...target.getElementsByTagName("script")].forEach((s) => {
+                    [...this.outputElement.getElementsByTagName("script")].forEach((s) => {
                         if (
                             s.getAttribute("type") === null ||
                             s.getAttribute("type") === "text/javascript"
                         ) {
                             eval(s.innerHTML);
                         }
                     });
```

#### js_lib/mathjaxknowl.js

##### js-beautify {}

```diff
@@ -34,15 +34,14 @@
             $("#" + uid).slideToggle("fast");
         } else {
             var the_content = "<div class='knowl-output' id='" + uid + "'>" +
                 "<div class='knowl'>" +
                 "<div class='knowl-content' id='" + oid + "'>" +
                 "loading '" + url + "'" +
                 "</div>" +
-                "<div class='knowl-footer'>" + url + "</div>" +
                 "</div>" +
                 "</div>";
 
             var the_parent = $("#MathJax-knowl-" + id).closest("p, article, .displaymath");
 
             if (the_parent.length == 0) {
                 the_parent = $("#MathJax-knowl-" + id).closest(".MJXc-display").next();
```

#### css/pretext.css

```diff
@@ -130,19 +130,14 @@
 /* we use .para as a wrapper around some "compound" p, so the
    first p in .para is block-like because of the .pare */
 .ptx-content .para > p:first-child,
 .ptx-content .para > .para:first-child {
     display: inline;
 }
 
-/* Oscar Levin figured out the cause of chrome showing a funny border focus */
-.ptx-content .knowl .para {
-    position: unset;
-}
-
 /* CSS defult values:
 https://www.w3schools.com/cssref/css_default_values.asp
 */
 
 /* the default margin for pre is "1em 0", so we over-ride
 so that we can set our own later */
 .ptx-content pre {
@@ -259,17 +254,14 @@
 .ptx-content section .exercisegroup > .heading + .introduction {
     display: inline;
 }
 .ptx-content section .exercisegroup > .heading + .introduction > .para:first-child {
     display: inline;
 }
 
-.ptx-content .exercisegroup article.exercise-like .solution .para:first-child {
-    margin-top: -3px;  /* because of the 10px (instread of 7) on the .knowl-content */
-}
 .ptx-content .exercisegroup article.exercise-like li > .para:first-child {
     margin-top: 0;
 }
 
 .ptx-content .exercisegroup article.exercise-like .heading {
     margin: 0;
 }
@@ -280,17 +272,14 @@
 .ptx-content article.exercise-like .task > .heading + .heading + div {
     display: block;
     margin-top: 0;
 }
 .ptx-content .exercisegroup .conclusion .heading {
     margin-top: 0.5em;
 }
-.ptx-content .exercisegroup .hidden-knowl-wrapper {
-    margin: 0;
-}
 .ptx-content .exercisegroup article + article {
     margin-top: 1em;
 }
 
 /* http://spot.pcc.edu/math/APEXCalculus/sec_interp_deriv.html */
 .ptx-content .exercisegroup > article,
 .ptx-content .exercisegroup-exercises > article {
@@ -319,89 +308,14 @@
     content: '\2003';
 }
 
 .ptx-content .exercisegroup > .introduction > .para:first-child {
     margin-top: 0;
 }
 
-.ptx-content .exercisegroup article + .hidden-knowl-wrapper {
-    margin-left: 4em;
-}
-
-/* make it look like a list, and have entra indenting when already more indented */
-.ptx-content .exercise-like .introduction + .hidden-knowl-wrapper,
-.ptx-content .exercise-like .conclusion {
-    margin-left: 1.0em;
-}
-.ptx-content .exercisegroup .exercise-like .introduction + .hidden-knowl-wrapper,
-.ptx-content .exercisegroup .exercise-like .conclusion {
-    margin-left: 1.5em;
-}
-.ptx-content section > .hidden-knowl-wrapper {
-    margin-top: 1em;
-}
-.ptx-content article + .hidden-knowl-wrapper {
-    margin-top: 1em;
-}
-.ptx-content .knowl-content > section:first-child > .heading:first-child {
-    margin-top: 0;
-}
-
-
-
-/* 9/23/23 a knowled article is now in a "details", so we add style
-   to mimic the old style below  */
-
-.ptx-content section  .born-hidden-knowl > summary {
-    cursor: pointer;
-}
-
-.ptx-content section > .born-hidden-knowl  > summary::marker,
-.ptx-content article + .born-hidden-knowl  > summary::marker {
-  content: "";
-}
-
-.ptx-content section > .born-hidden-knowl , .ptx-content .paragraphs > .born-hidden-knowl ,
-.ptx-content article + .born-hidden-knowl  {
-    margin-top: 1.25em;
-}
-.ptx-content .born-hidden-knowl summary + article {
-    margin-top: 1em;
-}
-.ptx-content section .born-hidden-knowl  + .born-hidden-knowl ,
-.ptx-content section .introduction + .born-hidden-knowl ,
-.ptx-content section .para + .born-hidden-knowl ,
-.ptx-content section .posterior + .born-hidden-knowl  {
-    margin-top: 1.75em;
-}
-
-.ptx-content .born-hidden-knowl  > article {
-  padding-top: 0.25em;
-}
-.ptx-content .born-hidden-knowl  > article:not(.theorem-like):not(.definition-like) {
-  padding: 0.25em;
-  padding-left: 0.5em;
-  padding-bottom: 0;
-}
-.ptx-content .born-hidden-knowl  > article {
-  background-color: #f5f5ff;
-}
-.ptx-content .born-hidden-knowl  > article .born-hidden-knowl  > article,
-.ptx-content .born-hidden-knowl  > article .born-hidden-knowl  > .answer {
-  margin: 0.5em;
-  padding: 0.25em;
-  padding-left: 0.5em;
-  background-color: #fffff5;
-}
-.ptx-content .born-hidden-knowl  > article .born-hidden-knowl  > article .born-hidden-knowl  > article {
-  background-color: #fff5ff;
-}
-.ptx-content .born-hidden-knowl  > article .born-hidden-knowl  > article .born-hidden-knowl  > article .born-hidden-knowl  > article {
-  background-color: #fafffa;
-}
 
 /* this > may be too restrictive.  The purpose is to not put a
    top margin on an article at the top of a knowl */
 .ptx-content section > article, .ptx-content section > section.paragraphs, .ptx-content .paragraphs > article {
     margin-top: 1.25em;
 }
 .ptx-content section article + article,
@@ -571,30 +485,14 @@
 .ptx-content .abstract > .title::after {
     content: ".\2009\2009\2009";
 }
 .ptx-content .abstract > .title + .para {
     display: inline;
 }
 
-/* born hidden articls are now in "details", so adding markup
-to immitate what is below.  */
-
-.ptx-content .born-hidden-knowl summary,
-.ptx-content .born-hidden-knowl summary > .heading {
-    position: relative;
-}
-
-.ptx-content .born-hidden-knowl summary > .heading {
-    font-size: 1.125em;
-    line-height: 1.125em;
-    margin-top: 0;
-    display: inline;
-}
-
-
 /*       -----      */
 
 
 .ptx-content article > .heading,
 .ptx-content article > a .heading {
     font-size: 1.125em;
     line-height: 1.125em;
```

#### css/knowls_default.css

```diff
@@ -1,230 +1,73 @@
 /*
-  main knowls style
+  main knowls styles
 */
 
-[data-knowl] {
-    display: inline;
-    position: relative;
+.knowl__link {
     cursor: pointer;
-    color: #9c2310;
-    padding: 0px 2px 0px 2px;
-    margin: 0;
-    text-decoration: none;
-    margin-bottom: 1px;
-/*
-    margin-bottom: 0;
-*/
-    font-weight: 500;
-    white-space: nowrap;
-    border-bottom: none;
-    border-top-left-radius: 3px;
-    border-top-right-radius: 3px;
-    transition-property: background-color;
-    transition-duration: 0ms;
-}
-table [data-knowl] {
-    white-space: pre-line;
-}
-
-[data-knowl]:hover, [data-knowl]:active, [data-knowl].active {
-    color: #8a1200;
-    background: #ffedeb;
-/*
-    margin-bottom: 0;
-*/
-    border-bottom: none;
-}
-
-[data-knowl]::after, [data-knowl]:hover::after, [data-knowl].active::after {
-    content: "";
-    position: absolute;
-    top: 0;
-    bottom: 1px;
-    right: 2.4px;
-    left: 2.4px;
-    border-bottom: 1px dotted #9c2310;
-    transition-property: left, right;
-    transition-duration: 0ms;
-    z-index: 0;
-}
-/* is the next only for a proof or other content that is only a knowl? */
-article > [data-knowl]::after, article > [data-knowl]:hover::after, article > [data-knowl].active::after,
-    section > details > summary > .heading, article + details > summary > .heading {
-    content: "";
-    position: absolute;
-    top: 0;
-    bottom: 1px;
-    right: 8.4px;
-    right: 0.6em;
-    left: 2.4px;
-    border-bottom: 1px dotted #9c2310;
-    transition-property: left, right;
-    transition-duration: 0ms;
-    z-index: 0;
+    margin-left: 0.1em;
+    margin-right: 0.1em;
+    color: var(--knowlLinkColor);
+    border-bottom: 1px dotted var(--knowlLinkColor);
 }
 
-[data-knowl].fn-knowl {
-    padding-left: 0;
-    padding-right: 0;
-    margin-right: 2px;
-}
-[data-knowl].fn-knowl::after {
-    bottom: 7px;
+summary.knowl__link {
+    display: list-item inline;
 }
 
-.knowl-error {
-   color: red;
-   border-bottom: 0;
-}
-.knowl-output {
-    background: #f5f5ff;
-    border: 10px solid #ddf;
-    border-radius: 10px;
-    padding: 0;
-    margin-top: 10px;
-    scroll-margin-top: 60px; /* height of header */
-}
-
-.knowl-output.original {
-    background: #f8f8f8;
-    border: none;
-/*    border-left: 1px solid #666;
-*/
-    border-radius: 0;
-    padding: 0;
-    margin-top: 10px;
-}
-.knowl-output.original .knowl-content {
-    padding-top: 0;
-    padding-bottom: 0;
-    margin-bottom: 0;
-}
-/*
-.knowl-output.original:after {
-  content: '';
-  display: block;
-  padding-top: 0.35em;
-}
-*/
-.example-like .knowl-output.original {
-    background: inherit;
-}
-
-.knowl-output--hide {
-    display: none;
-}
-
-.knowl-output__error .para:first-child {
-    margin-top: 0;
-}
-
-.knowl-output__error a {
-    text-decoration: underline;
-}
-
-.knowl-output .knowl-output {
-    border-width: 6px;
-    background: #fffff5;
-    border-radius: 4px;
-    margin-bottom: -3px;
-    margin-left: -7px;
-    margin-right: -7px;
-}
-.knowl-output .knowl-output .knowl-output {
-    background: #fff5ff;
-}
-.knowl-output .knowl-output .knowl-output .knowl-output {
-    background: #fafffa;
-}
-.knowl-footer {
-  position: relative;
-  bottom: -9px;
-  font-size: x-small;
-  background: #ddf;
-  color: grey;
-  padding: 0 0 0 12px;
-  margin:  -10px 0 0 0;
-}
-.knowl-footer a {
-  color: #006;
-}
-.knowl-footer a:hover {
-  background: none;
-  color: #88f;
+.knowl__link > * {
+    display: inline;
 }
-/* .knowl-footer:after {
-    content: "\2002";
-} */
 
-.knowl-output .knowl-output .knowl-footer {
-  bottom: -5px;
-  margin:  -5px 0 0 0;
-}
 
-.knowl-output + .knowl-output {
-    margin-top: 0;
-}
-.knowl-output + .knowl-output.original {
-    margin-top: 0.5em;
-}
-.knowl-content {
-    padding: 10px;
-    padding-bottom: 7px;
-}
-.knowl-content > *:first-child {
-    margin-top: 0;
+.knowl__link:is(:hover, :focus, [open]) {
+    background-color: var(--knowlbackground);
+    border-bottom-color: transparent;
 }
 
-/* sort of a hack for proof knows in theorem knowls */
-.ptx-content div.knowl .posterior a[data-knowl]:first-child {
-    padding: 0;
+.knowl__content {
+    margin: 0.2em;
+    border: 6px solid var(--knowlborder);
+    border-radius: 0.4em;
+    padding: 0.8em;
+    background-color: var(--knowlbackground);
 }
 
-/* not sure where this was being used, but it made short knowls
- * look bad, like the hint here:
- * SAFurtherReading.html
-*/
-.ptx-content .knowl-output .knowl-content > *:last-child:not(.incontext) {
-    margin-bottom: 0.5em;
-}
 
 /* No Greg's L in knowls, to save space */
-
-.ptx-content .knowl-content > article.theorem-like,
-.ptx-content .knowl-content > article.definition-like,
-.ptx-content .knowl-content > article.example-like,
-.ptx-content .knowl-content > article.project-like,
-.ptx-content .knowl-content > article.objectives,
-.ptx-content .knowl-content > article.outcomes,
-.ptx-content .knowl-content > article.remark-like {
-    padding-left: 0;
-    border-left: none;
-}
-.ptx-content .knowl-content > article.theorem-like::after,
-.ptx-content .knowl-content > article.definition-like::after,
-.ptx-content .knowl-content > article.example-like::after,
-.ptx-content .knowl-content > article.project-like::after,
-.ptx-content .knowl-content > article.objectives::after,
-.ptx-content .knowl-content > article.outcomes::after,
-.ptx-content .knowl-content > article.remark-like::after {
-    content: '';
+.ptx-content .knowl__content > article:is(.theorem-like, .definition-like, .example-like, .project-like, .objectives, .outcomes, .remark-like, .proof)::after {
+    content: '' !important;
     border-bottom: none;
     margin: 0;
     padding: 0;
     width: 0;
 }
-
-/* sup knowls are used for footnotes */
-/* the next 2 are obsolete, because (in PTX HTML) the structure is now a(sup), not sup(a) */
-sup [data-knowl] {
-    padding: 0px 0px 0px 3px;
+.ptx-content .knowl__content > article:is(.theorem-like, .definition-like, .example-like, .project-like, .objectives, .outcomes, .remark-like) {
+    padding-left: 0;
+    border-left: none;
 }
-
-sup .active[data-knowl] {
-    padding: 0px 0px 0px 3px;
+.ptx-content .knowl__content > article:is(.proof) {
+    padding-right: 0;
+    border-right: none;
 }
 
-sup [data-knowl]:hover {
-    padding: 0px 0px 0px 3px;
+
+/* nested knowl alt colors */
+.knowl__content .knowl__content {
+    background-color: var(--knowlNested1Background);
+}
+.knowl__content .knowl__content .knowl__content {
+    background-color: var(--knowlNested2Background);
 }
+.knowl__content .knowl__content .knowl__content .knowl__content {
+    background-color: var(--knowlNested3Background);
+}
+.knowl__content .knowl__content .knowl__content .knowl__content .knowl__content {
+    background-color: var(--knowlNested4Background);
+}
+
 
+/* spacing tweaks inside knowls */
+.ptx-content .knowl__content > figure {
+    margin-left: 0;
+    margin-right: 0;
+}
```

#### css/setcolors.css

```diff
@@ -91,33 +91,25 @@
   color: var(--sectiontoctext);
 }
 .ptx-content .summary-links a:hover, .ptx-content .summary-links a:focus {
   color: var(--highlighttoctext);
   background: var(--highlighttoc);
 }
 
-.ptx-content [data-knowl], .ptx-content [data-knowl]:hover, .ptx-content [data-knowl]:active, .ptx-content [data-knowl].active, .ptx-content summary {
-    color: var(--bodytitle);
-}
-.ptx-content [data-knowl]:hover, .ptx-content [data-knowl]:active, .ptx-content [data-knowl].active {
-    color: var(--bodyfontcolorhighlight);
-    background-color: var(--bodytitlehighlight);
-}
-
 /* next two groups concern accessibility, so check when making changes */
 .ptx-content .para > a.internal {
-    color: var(--bodytitle);
+    color: var(--bodysubtitle);
 }
 .ptx-content .para > a.external {
     color: var(--bodysubtitle);
 }
 .ptx-content .para > a.internal:hover, .ptx-content .para > a.internal:hover *,
 .ptx-content .para > a.internal:focus, .ptx-content .para > a.internal:focus * {
     color: var(--bodyfontcolorhighlight);
-    background-color: var(--bodytitlehighlight);
+    background-color: var(--bodysubtitlehighlight);
 }
 .ptx-content .para > a.external:hover, .ptx-content .para > a.external:hover *,
 .ptx-content .para > a.external:focus, .ptx-content .para > a.external:focus * {
     color: var(--bodyfontcolorhighlight);
     background-color: var(--bodysubtitlehighlight);
 }
 
@@ -134,17 +126,14 @@
     background-color: var(--assemblagebackground);
 }
 
 .ptx-content .knowl-output {
     border-color: var(--knowlborder);
     background-color: var(--knowlbackground);
 }
-.ptx-content .knowl-footer {
-    background-color: var(--knowlborder);
-}
 
 /* 
   pastel
 */
 .pretext[data-atmosphere="pastel"],
 .pretext[data-atmosphere="pastel"] .ptx-main {
   background: #dbf5ff;
@@ -446,7 +435,17 @@
   background-color: var(--linkbackgroundhighlight);
   color: var(--bodyfontcolorhighlight);
 }
 .pretext[data-atmosphere*="dark"] .ptx-page .ptx-main .ptx-content .knowl-content > .solution-like {
   background: #606;
 }
 
+/* link/knowl coloring */
+:root {
+  --knowlLinkColor: var(--documenttitle);
+  --linkColor: var(--bodysubtitle);
+  --linkBackground: var(--bodysubtitlehighlight);
+  --knowlNested1Background: #f5f5ff;
+  --knowlNested2Background: #fffff5;
+  --knowlNested3Background: #f5ffff;
+  --knowlNested4Background: #fff5f5;
+}
```

#### css/pretext_add_on.css

```diff
@@ -1488,17 +1488,14 @@
 }
 
 .ptx-content .knowl-content > article:first-child,
 .ptx-content .knowl-content > .solution-like:first-child {
 /* padding, not margin, to get colored background (and not be absorbed) */
     padding-top: 0.25em;
 }
-.ptx-content .knowl-footer {
-    display: none;
-}
 
 .ptx-content .exercisegroup > .conclusion {
     margin-left: 1.5em;
 }
 
 .ptx-content .exercise-like .introduction {
     display: inline;
```

### Comparing `pretext-2.3.9.dev20240229/pretext/project/__init__.py` & `pretext-2.3.9.dev20240302/pretext/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/project/xml.py` & `pretext-2.3.9.dev20240302/pretext/project/xml.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/__init__.py` & `pretext-2.3.9.dev20240302/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/resources/.devcontainer.json` & `pretext-2.3.9.dev20240302/pretext/templates/resources/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/resources/.gitignore` & `pretext-2.3.9.dev20240302/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/resources/article.zip` & `pretext-2.3.9.dev20240302/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,15 +1,15 @@
 Zip file size: 160335 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 source/
--rw-r--r--  2.0 unx       86 b- defN 24-Feb-29 06:12 README.md
--rw-r--r--  2.0 unx     3028 b- defN 24-Feb-29 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx      432 b- defN 24-Feb-29 06:13 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Feb-29 06:13 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Feb-29 06:13 .devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 24-Feb-29 06:12 publication/publication.ptx
--rw-r--r--  2.0 unx   154806 b- defN 24-Feb-29 06:12 assets/frog.jpg
--rw-r--r--  2.0 unx      576 b- defN 24-Feb-29 06:12 source/section-1.ptx
--rw-r--r--  2.0 unx      765 b- defN 24-Feb-29 06:12 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 24-Feb-29 06:12 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
+-rw-r--r--  2.0 unx       86 b- defN 24-Mar-02 06:13 README.md
+-rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx      432 b- defN 24-Mar-02 06:14 project.ptx
+-rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
+-rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 24-Mar-02 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 24-Mar-02 06:13 assets/frog.jpg
+-rw-r--r--  2.0 unx      576 b- defN 24-Mar-02 06:13 source/section-1.ptx
+-rw-r--r--  2.0 unx      765 b- defN 24-Mar-02 06:13 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 24-Mar-02 06:13 source/main.ptx
 13 files, 165453 bytes uncompressed, 158943 bytes compressed:  3.9%
```

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/resources/book.zip` & `pretext-2.3.9.dev20240302/pretext/templates/resources/book.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 10351 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 source/
--rw-r--r--  2.0 unx       82 b- defN 24-Feb-29 06:12 README.md
--rw-r--r--  2.0 unx     3028 b- defN 24-Feb-29 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx      432 b- defN 24-Feb-29 06:13 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Feb-29 06:13 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Feb-29 06:13 .devcontainer.json
--rw-r--r--  2.0 unx     6207 b- defN 24-Feb-29 06:12 publication/publication.ptx
--rw-r--r--  2.0 unx     1047 b- defN 24-Feb-29 06:12 source/frontmatter.ptx
--rw-r--r--  2.0 unx     2131 b- defN 24-Feb-29 06:12 source/docinfo.ptx
--rw-r--r--  2.0 unx      873 b- defN 24-Feb-29 06:12 source/backmatter.ptx
--rw-r--r--  2.0 unx      315 b- defN 24-Feb-29 06:12 source/ch-chapter-title.ptx
--rw-r--r--  2.0 unx      190 b- defN 24-Feb-29 06:12 source/sec-section-name.ptx
--rw-r--r--  2.0 unx      597 b- defN 24-Feb-29 06:12 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
+-rw-r--r--  2.0 unx       82 b- defN 24-Mar-02 06:13 README.md
+-rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx      432 b- defN 24-Mar-02 06:14 project.ptx
+-rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
+-rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
+-rw-r--r--  2.0 unx     6207 b- defN 24-Mar-02 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx     1047 b- defN 24-Mar-02 06:13 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     2131 b- defN 24-Mar-02 06:13 source/docinfo.ptx
+-rw-r--r--  2.0 unx      873 b- defN 24-Mar-02 06:13 source/backmatter.ptx
+-rw-r--r--  2.0 unx      315 b- defN 24-Mar-02 06:13 source/ch-chapter-title.ptx
+-rw-r--r--  2.0 unx      190 b- defN 24-Mar-02 06:13 source/sec-section-name.ptx
+-rw-r--r--  2.0 unx      597 b- defN 24-Mar-02 06:13 source/main.ptx
 14 files, 19990 bytes uncompressed, 8777 bytes compressed:  56.1%
```

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/resources/codechat_config.yaml` & `pretext-2.3.9.dev20240302/pretext/templates/resources/codechat_config.yaml`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/resources/demo.zip` & `pretext-2.3.9.dev20240302/pretext/templates/resources/demo.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 174088 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 source/
--rw-r--r--  2.0 unx       82 b- defN 24-Feb-29 06:12 README.md
--rw-r--r--  2.0 unx     3028 b- defN 24-Feb-29 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx      432 b- defN 24-Feb-29 06:13 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Feb-29 06:13 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Feb-29 06:13 .devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 24-Feb-29 06:12 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 24-Feb-29 06:12 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 24-Feb-29 06:12 assets/jsxgraph/infinity.js
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 source/images/
--rw-r--r--  2.0 unx     2050 b- defN 24-Feb-29 06:12 source/frontmatter.ptx
--rw-r--r--  2.0 unx      229 b- defN 24-Feb-29 06:12 source/ch-empty.ptx
--rw-r--r--  2.0 unx      867 b- defN 24-Feb-29 06:12 source/sec-features.ptx
--rw-r--r--  2.0 unx     1115 b- defN 24-Feb-29 06:12 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     1697 b- defN 24-Feb-29 06:12 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      339 b- defN 24-Feb-29 06:12 source/ch-features.ptx
--rw-r--r--  2.0 unx      375 b- defN 24-Feb-29 06:12 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     2427 b- defN 24-Feb-29 06:12 source/docinfo.ptx
--rw-r--r--  2.0 unx      885 b- defN 24-Feb-29 06:12 source/backmatter.ptx
--rw-r--r--  2.0 unx      411 b- defN 24-Feb-29 06:12 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx      777 b- defN 24-Feb-29 06:12 source/ww.ptx
--rw-r--r--  2.0 unx     2531 b- defN 24-Feb-29 06:12 source/ch-generate.ptx
--rw-r--r--  2.0 unx      381 b- defN 24-Feb-29 06:12 source/fig-tikz.ptx
--rw-r--r--  2.0 unx     2428 b- defN 24-Feb-29 06:12 source/main.ptx
--rw-r--r--  2.0 unx      335 b- defN 24-Feb-29 06:12 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     1515 b- defN 24-Feb-29 06:12 source/ex-first.ptx
--rw-r--r--  2.0 unx      847 b- defN 24-Feb-29 06:12 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      835 b- defN 24-Feb-29 06:12 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 24-Feb-29 06:12 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 24-Feb-29 06:12 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx       10 b- defN 24-Feb-29 06:12 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
+-rw-r--r--  2.0 unx       82 b- defN 24-Mar-02 06:13 README.md
+-rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx      432 b- defN 24-Mar-02 06:14 project.ptx
+-rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
+-rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
+-rw-r--r--  2.0 unx     6092 b- defN 24-Mar-02 06:13 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 24-Mar-02 06:13 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 24-Mar-02 06:13 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/images/
+-rw-r--r--  2.0 unx     2050 b- defN 24-Mar-02 06:13 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      229 b- defN 24-Mar-02 06:13 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      867 b- defN 24-Mar-02 06:13 source/sec-features.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 24-Mar-02 06:13 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 24-Mar-02 06:13 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      339 b- defN 24-Mar-02 06:13 source/ch-features.ptx
+-rw-r--r--  2.0 unx      375 b- defN 24-Mar-02 06:13 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx     2427 b- defN 24-Mar-02 06:13 source/docinfo.ptx
+-rw-r--r--  2.0 unx      885 b- defN 24-Mar-02 06:13 source/backmatter.ptx
+-rw-r--r--  2.0 unx      411 b- defN 24-Mar-02 06:13 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx      777 b- defN 24-Mar-02 06:13 source/ww.ptx
+-rw-r--r--  2.0 unx     2531 b- defN 24-Mar-02 06:13 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      381 b- defN 24-Mar-02 06:13 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx     2428 b- defN 24-Mar-02 06:13 source/main.ptx
+-rw-r--r--  2.0 unx      335 b- defN 24-Mar-02 06:13 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 24-Mar-02 06:13 source/ex-first.ptx
+-rw-r--r--  2.0 unx      847 b- defN 24-Mar-02 06:13 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx      835 b- defN 24-Mar-02 06:13 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 24-Mar-02 06:13 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 24-Mar-02 06:13 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx       10 b- defN 24-Mar-02 06:13 source/images/sageplot2d.sage
 34 files, 191769 bytes uncompressed, 170160 bytes compressed:  11.3%
```

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/resources/hello.zip` & `pretext-2.3.9.dev20240302/pretext/templates/resources/hello.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 5045 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 source/
--rw-r--r--  2.0 unx       69 b- defN 24-Feb-29 06:12 README.md
--rw-r--r--  2.0 unx     3028 b- defN 24-Feb-29 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx      432 b- defN 24-Feb-29 06:13 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Feb-29 06:13 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Feb-29 06:13 .devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 24-Feb-29 06:12 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 24-Feb-29 06:12 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
+-rw-r--r--  2.0 unx       69 b- defN 24-Mar-02 06:13 README.md
+-rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx      432 b- defN 24-Mar-02 06:14 project.ptx
+-rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
+-rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 24-Mar-02 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 24-Mar-02 06:13 source/main.ptx
 9 files, 9015 bytes uncompressed, 4081 bytes compressed:  54.7%
```

### Comparing `pretext-2.3.9.dev20240229/pretext/templates/resources/slideshow.zip` & `pretext-2.3.9.dev20240302/pretext/templates/resources/slideshow.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 8885 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 source/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Feb-29 06:12 xsl/
--rw-r--r--  2.0 unx     3028 b- defN 24-Feb-29 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx      480 b- defN 24-Feb-29 06:12 project.ptx
--rw-r--r--  2.0 unx     1939 b- defN 24-Feb-29 06:13 .gitignore
--rw-r--r--  2.0 unx     3149 b- defN 24-Feb-29 06:13 .devcontainer.json
--rw-r--r--  2.0 unx      190 b- defN 24-Feb-29 06:12 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 24-Feb-29 06:12 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 24-Feb-29 06:12 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 source/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-02 06:13 xsl/
+-rw-r--r--  2.0 unx     3028 b- defN 24-Mar-02 06:14 codechat_config.yaml
+-rw-r--r--  2.0 unx      480 b- defN 24-Mar-02 06:13 project.ptx
+-rw-r--r--  2.0 unx     1939 b- defN 24-Mar-02 06:14 .gitignore
+-rw-r--r--  2.0 unx     3149 b- defN 24-Mar-02 06:14 .devcontainer.json
+-rw-r--r--  2.0 unx      190 b- defN 24-Mar-02 06:13 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 24-Mar-02 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 24-Mar-02 06:13 source/main.ptx
 10 files, 22083 bytes uncompressed, 7827 bytes compressed:  64.6%
```

### Comparing `pretext-2.3.9.dev20240229/pretext/utils.py` & `pretext-2.3.9.dev20240302/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-2.3.9.dev20240229/pyproject.toml` & `pretext-2.3.9.dev20240302/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "2.3.9.dev20240229"
+version = "2.3.9.dev20240302"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-2.3.9.dev20240229/PKG-INFO` & `pretext-2.3.9.dev20240302/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 2.3.9.dev20240229
+Version: 2.3.9.dev20240302
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

