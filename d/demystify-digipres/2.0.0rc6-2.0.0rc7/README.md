# Comparing `tmp/demystify-digipres-2.0.0rc6.tar.gz` & `tmp/demystify_digipres-2.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demystify-digipres-2.0.0rc6.tar", last modified: Mon Mar 25 20:52:44 2024, max compression
+gzip compressed data, was "demystify_digipres-2.0.0rc7.tar", last modified: Sun Apr 14 13:53:33 2024, max compression
```

## Comparing `demystify-digipres-2.0.0rc6.tar` & `demystify_digipres-2.0.0rc7.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.155301 demystify-digipres-2.0.0rc6/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       11 2024-03-24 19:14:27.000000 demystify-digipres-2.0.0rc6/.codespellignore
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      121 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/.codespellrc
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      103 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/.markdownlint.yaml
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1133 2024-03-24 19:14:27.000000 demystify-digipres-2.0.0rc6/.pre-commit-config.yaml
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2405 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/.pylintrc
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1161 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/.ruff.toml
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.143301 demystify-digipres-2.0.0rc6/.vscode/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      997 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/.vscode/settings.json
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3587 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/CODE_OF_CONDUCT.md
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      832 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/LICENSE.txt
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1460 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/Makefile
--rw-r--r--   0 r0ss      (1001) r0ss      (1001)    12013 2024-03-25 20:52:44.151301 demystify-digipres-2.0.0rc6/PKG-INFO
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    10618 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/README.md
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.139301 demystify-digipres-2.0.0rc6/cooperhewitt/
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.143301 demystify-digipres-2.0.0rc6/cooperhewitt/unicode/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1739 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/cooperhewitt/unicode/README.md
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      270 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/demystify.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     4432 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/denylist.cfg
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.143301 demystify-digipres-2.0.0rc6/documentation/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    25490 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/documentation/analysis-engine-architecture.png
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    45027 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/documentation/archivist-descriptions.png
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)   256422 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/documentation/rogues-gallery.gif
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1238 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/pyproject.toml
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      257 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/pytest.ini
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.143301 demystify-digipres-2.0.0rc6/requirements/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       12 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/requirements/base.txt
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      126 2024-03-25 20:50:40.000000 demystify-digipres-2.0.0rc6/requirements/local.txt
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       85 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/requirements/production.txt
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       38 2024-03-25 20:52:44.155301 demystify-digipres-2.0.0rc6/setup.cfg
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.143301 demystify-digipres-2.0.0rc6/src/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/__init__.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.143301 demystify-digipres-2.0.0rc6/src/demystify/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      306 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/config.cfg
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    11417 2024-03-25 20:13:55.000000 demystify-digipres-2.0.0rc6/src/demystify/demystify.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     4485 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/denylist_template.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.143301 demystify-digipres-2.0.0rc6/src/demystify/i18n/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2368 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/i18n/README.md
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/i18n/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    27552 2024-03-24 19:14:27.000000 demystify-digipres-2.0.0rc6/src/demystify/i18n/internationalstrings.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.143301 demystify-digipres-2.0.0rc6/src/demystify/libs/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    16672 2024-03-24 19:14:27.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/AnalysisQueriesClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3625 2024-03-24 19:14:27.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/AnalysisResultsClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    42691 2024-03-24 19:14:27.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/DemystifyAnalysisClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2089 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/DenylistQueriesClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3108 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/HandleDenylistClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      910 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/IdentifyDatabase.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3083 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/RoguesQueriesClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/__init__.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.147301 demystify-digipres-2.0.0rc6/src/demystify/libs/outputhandlers/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/outputhandlers/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    43223 2024-03-24 19:14:27.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/outputhandlers/htmloutputclass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     6161 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/outputhandlers/roguesgalleryoutputclass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    28132 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/outputhandlers/textoutputclass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      467 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/src/demystify/libs/version.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.147301 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      282 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/pathlesstaken.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1702 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/setup.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.147301 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/__init__.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.147301 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/__init__.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.147301 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/i18n/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/i18n/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      680 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/i18n/internationalstrings.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      680 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/internationalstrings.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2713 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/names.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     9915 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/pathlesstaken.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)  1294456 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/ucd.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       64 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/version.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.147301 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1797 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/setup.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      270 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/sqlitefid.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.147301 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/__init__.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.147301 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/__init__.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.151301 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     9761 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/CSVHandlerClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     7558 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/DROIDLoaderClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2595 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/FidoLoaderClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     7643 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/GenerateBaselineDBClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     4443 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/IdentifyExportClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2214 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/PyDateHandler.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    18472 2024-03-24 16:59:49.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/SFHandlerClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     6664 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/SFLoaderClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1747 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/ToolMappingClass.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      304 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/Version.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     7400 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/unicodecsv.py
--rwxrwxr-x   0 r0ss      (1001) r0ss      (1001)     4019 2024-03-24 16:59:22.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/sqlitefid.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.151301 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    54999 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_droid_handler.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3025 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_fido_handler.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     6252 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_identify_export.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)   107280 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sf_handler.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1185 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sf_internal_functions.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3666 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sqlite_basedb.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    74596 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sqlite_output_droid.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)   135510 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sqlite_output_sf.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2831 2024-03-24 16:57:09.000000 demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_utilities.py
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.151301 demystify-digipres-2.0.0rc6/src/demystify_digipres.egg-info/
--rw-r--r--   0 r0ss      (1001) r0ss      (1001)    12013 2024-03-25 20:52:44.000000 demystify-digipres-2.0.0rc6/src/demystify_digipres.egg-info/PKG-INFO
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3777 2024-03-25 20:52:44.000000 demystify-digipres-2.0.0rc6/src/demystify_digipres.egg-info/SOURCES.txt
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        1 2024-03-25 20:52:44.000000 demystify-digipres-2.0.0rc6/src/demystify_digipres.egg-info/dependency_links.txt
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       55 2024-03-25 20:52:44.000000 demystify-digipres-2.0.0rc6/src/demystify_digipres.egg-info/entry_points.txt
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       19 2024-03-25 20:52:44.000000 demystify-digipres-2.0.0rc6/src/demystify_digipres.egg-info/top_level.txt
-drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-03-25 20:52:44.151301 demystify-digipres-2.0.0rc6/tests/
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/tests/__init__.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    20755 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/tests/test_deny_list.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    72529 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/tests/test_droid_analysis.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    26138 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/tests/test_rogues_list.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)   159956 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/tests/test_siegfried_analysis.py
--rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      778 2024-03-24 14:22:33.000000 demystify-digipres-2.0.0rc6/tox.ini
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.780260 demystify_digipres-2.0.0rc7/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       11 2024-03-24 19:14:27.000000 demystify_digipres-2.0.0rc7/.codespellignore
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      121 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/.codespellrc
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      103 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/.markdownlint.yaml
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1133 2024-03-24 19:14:27.000000 demystify_digipres-2.0.0rc7/.pre-commit-config.yaml
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2405 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/.pylintrc
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1161 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/.ruff.toml
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.768260 demystify_digipres-2.0.0rc7/.vscode/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      997 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/.vscode/settings.json
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3587 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      832 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/LICENSE.txt
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1460 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/Makefile
+-rw-r--r--   0 r0ss      (1001) r0ss      (1001)    12013 2024-04-14 13:53:33.780260 demystify_digipres-2.0.0rc7/PKG-INFO
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    10618 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/README.md
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.768260 demystify_digipres-2.0.0rc7/cooperhewitt/
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.768260 demystify_digipres-2.0.0rc7/cooperhewitt/unicode/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1739 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/cooperhewitt/unicode/README.md
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      270 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/demystify.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     4432 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/denylist.cfg
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/documentation/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    25490 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/documentation/analysis-engine-architecture.png
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    45027 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/documentation/archivist-descriptions.png
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)   256422 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/documentation/rogues-gallery.gif
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1238 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/pyproject.toml
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      257 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/pytest.ini
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/requirements/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       12 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/requirements/base.txt
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      126 2024-03-25 20:50:40.000000 demystify_digipres-2.0.0rc7/requirements/local.txt
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       85 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/requirements/production.txt
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       38 2024-04-14 13:53:33.780260 demystify_digipres-2.0.0rc7/setup.cfg
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/src/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/__init__.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/src/demystify/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      306 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/config.cfg
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    11417 2024-03-25 20:13:55.000000 demystify_digipres-2.0.0rc7/src/demystify/demystify.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     4485 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/denylist_template.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/src/demystify/i18n/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2368 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/i18n/README.md
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/i18n/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    27552 2024-03-24 19:14:27.000000 demystify_digipres-2.0.0rc7/src/demystify/i18n/internationalstrings.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/src/demystify/libs/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    16672 2024-03-24 19:14:27.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/AnalysisQueriesClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3625 2024-03-24 19:14:27.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/AnalysisResultsClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    42691 2024-03-24 19:14:27.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/DemystifyAnalysisClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2089 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/DenylistQueriesClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3108 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/HandleDenylistClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      910 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/IdentifyDatabase.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3083 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/RoguesQueriesClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/__init__.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/src/demystify/libs/outputhandlers/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/outputhandlers/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    43215 2024-04-14 13:50:55.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/outputhandlers/htmloutputclass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     6161 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/outputhandlers/roguesgalleryoutputclass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    28132 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/outputhandlers/textoutputclass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      467 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/src/demystify/libs/version.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      282 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/pathlesstaken.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1702 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/setup.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.772260 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/__init__.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.776260 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/__init__.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.776260 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/i18n/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/i18n/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      680 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/i18n/internationalstrings.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      680 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/internationalstrings.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2713 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/names.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     9915 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/pathlesstaken.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)  1294456 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/ucd.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       64 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/version.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.776260 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1797 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/setup.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      270 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/sqlitefid.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.776260 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/__init__.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.776260 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/__init__.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.776260 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     9761 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/CSVHandlerClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     7558 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/DROIDLoaderClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2595 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/FidoLoaderClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     7643 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/GenerateBaselineDBClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     4443 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/IdentifyExportClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2214 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/PyDateHandler.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    18472 2024-03-24 16:59:49.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/SFHandlerClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     6664 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/SFLoaderClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1747 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/ToolMappingClass.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      304 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/Version.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     7400 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/unicodecsv.py
+-rwxrwxr-x   0 r0ss      (1001) r0ss      (1001)     4019 2024-03-24 16:59:22.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/sqlitefid.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.776260 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    54999 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_droid_handler.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3025 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_fido_handler.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     6252 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_identify_export.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)   107280 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sf_handler.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     1185 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sf_internal_functions.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3666 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sqlite_basedb.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    74596 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sqlite_output_droid.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)   135510 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sqlite_output_sf.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     2831 2024-03-24 16:57:09.000000 demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_utilities.py
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.780260 demystify_digipres-2.0.0rc7/src/demystify_digipres.egg-info/
+-rw-r--r--   0 r0ss      (1001) r0ss      (1001)    12013 2024-04-14 13:53:33.000000 demystify_digipres-2.0.0rc7/src/demystify_digipres.egg-info/PKG-INFO
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)     3777 2024-04-14 13:53:33.000000 demystify_digipres-2.0.0rc7/src/demystify_digipres.egg-info/SOURCES.txt
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        1 2024-04-14 13:53:33.000000 demystify_digipres-2.0.0rc7/src/demystify_digipres.egg-info/dependency_links.txt
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       55 2024-04-14 13:53:33.000000 demystify_digipres-2.0.0rc7/src/demystify_digipres.egg-info/entry_points.txt
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)       19 2024-04-14 13:53:33.000000 demystify_digipres-2.0.0rc7/src/demystify_digipres.egg-info/top_level.txt
+drwxrwxr-x   0 r0ss      (1001) r0ss      (1001)        0 2024-04-14 13:53:33.780260 demystify_digipres-2.0.0rc7/tests/
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)        0 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/tests/__init__.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    20755 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/tests/test_deny_list.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    72529 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/tests/test_droid_analysis.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)    26138 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/tests/test_rogues_list.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)   159956 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/tests/test_siegfried_analysis.py
+-rw-rw-r--   0 r0ss      (1001) r0ss      (1001)      778 2024-03-24 14:22:33.000000 demystify_digipres-2.0.0rc7/tox.ini
```

### Comparing `demystify-digipres-2.0.0rc6/.pre-commit-config.yaml` & `demystify_digipres-2.0.0rc7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/.pylintrc` & `demystify_digipres-2.0.0rc7/.pylintrc`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/.ruff.toml` & `demystify_digipres-2.0.0rc7/.ruff.toml`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/.vscode/settings.json` & `demystify_digipres-2.0.0rc7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/CODE_OF_CONDUCT.md` & `demystify_digipres-2.0.0rc7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/LICENSE.txt` & `demystify_digipres-2.0.0rc7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/Makefile` & `demystify_digipres-2.0.0rc7/Makefile`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/PKG-INFO` & `demystify_digipres-2.0.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demystify-digipres
-Version: 2.0.0rc6
+Version: 2.0.0rc7
 Summary: engine for the analysis of DROID and Siegfried file format reports
 Author: Ross Spencer
 License: Copyright (c) 2013 Ross Spencer
         
         This software is provided 'as-is', without any express or implied warranty. In
         no event will the authors be held liable for any damages arising from the use
         of this software.
```

### Comparing `demystify-digipres-2.0.0rc6/README.md` & `demystify_digipres-2.0.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/cooperhewitt/unicode/README.md` & `demystify_digipres-2.0.0rc7/cooperhewitt/unicode/README.md`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/denylist.cfg` & `demystify_digipres-2.0.0rc7/denylist.cfg`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/documentation/analysis-engine-architecture.png` & `demystify_digipres-2.0.0rc7/documentation/analysis-engine-architecture.png`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/documentation/archivist-descriptions.png` & `demystify_digipres-2.0.0rc7/documentation/archivist-descriptions.png`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/documentation/rogues-gallery.gif` & `demystify_digipres-2.0.0rc7/documentation/rogues-gallery.gif`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/pyproject.toml` & `demystify_digipres-2.0.0rc7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/demystify.py` & `demystify_digipres-2.0.0rc7/src/demystify/demystify.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/denylist_template.py` & `demystify_digipres-2.0.0rc7/src/demystify/denylist_template.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/i18n/README.md` & `demystify_digipres-2.0.0rc7/src/demystify/i18n/README.md`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/i18n/internationalstrings.py` & `demystify_digipres-2.0.0rc7/src/demystify/i18n/internationalstrings.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/AnalysisQueriesClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/AnalysisQueriesClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/AnalysisResultsClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/AnalysisResultsClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/DemystifyAnalysisClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/DemystifyAnalysisClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/DenylistQueriesClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/DenylistQueriesClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/HandleDenylistClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/HandleDenylistClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/IdentifyDatabase.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/IdentifyDatabase.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/RoguesQueriesClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/RoguesQueriesClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/outputhandlers/htmloutputclass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/outputhandlers/htmloutputclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                 self.STRINGS.COLUMN_HEADER_VALUES_YEAR,
             )
         )
         for sig in countlist:
             self.printFormattedText('<tr><td style="width: 220px;">')
             if "fmt/" in sig[0]:
                 self.printFormattedText(
-                    '<a target="_blank" href="http://apps.nationalarchives.gov.uk/PRONOM/{}">{}</a>'.format(
+                    '<a target="_blank" href="https://nationalarchives.gov.uk/PRONOM/{}">{}</a>'.format(
                         sig[0], sig[0]
                     )
                 )
             else:
                 self.printFormattedText(sig[0])
             self.printFormattedText(
                 '</td><td style="width: 100px;">{}</td>'.format(str(sig[1]).strip())
@@ -198,15 +198,15 @@
         #
         #   For example: ('ns:pronom fmt/19, Acrobat PDF 1.5 - Portable Document Format, 1.5 (6)', 1)
         #
         for id_ in idlist:
             if "fmt/" in id_[1]:
                 markup = (
                     '<tr><td style="width: 200px;">\n'
-                    '<a target="_blank" href="http://apps.nationalarchives.gov.uk/PRONOM/{}">{}</a></td>\n'
+                    '<a target="_blank" href="https://nationalarchives.gov.uk/PRONOM/{}">{}</a></td>\n'
                 ).format(id_[1], id_[1])
             else:
                 markup = '<tr><td style="width: 100px;">{}</td>'.format(id_[1])
             markup = '{}<td style="width: 150px;">{}</td><td>{}</td><td style="text-align:center">{}</td></tr>'.format(
                 markup, id_[0], id_[2], id_[3]
             )
             self.printFormattedText(markup)
```

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/outputhandlers/roguesgalleryoutputclass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/outputhandlers/roguesgalleryoutputclass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/libs/outputhandlers/textoutputclass.py` & `demystify_digipres-2.0.0rc7/src/demystify/libs/outputhandlers/textoutputclass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/setup.py` & `demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/setup.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/i18n/internationalstrings.py` & `demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/i18n/internationalstrings.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/internationalstrings.py` & `demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/internationalstrings.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/names.py` & `demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/names.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/pathlesstaken.py` & `demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/pathlesstaken.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/pathlesstaken/src/pathlesstaken/ucd.py` & `demystify_digipres-2.0.0rc7/src/demystify/pathlesstaken/src/pathlesstaken/ucd.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/setup.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/setup.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/CSVHandlerClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/CSVHandlerClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/DROIDLoaderClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/DROIDLoaderClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/FidoLoaderClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/FidoLoaderClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/GenerateBaselineDBClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/GenerateBaselineDBClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/IdentifyExportClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/IdentifyExportClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/PyDateHandler.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/PyDateHandler.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/SFHandlerClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/SFHandlerClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/SFLoaderClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/SFLoaderClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/ToolMappingClass.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/ToolMappingClass.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/libs/unicodecsv.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/libs/unicodecsv.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/src/sqlitefid/sqlitefid.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/src/sqlitefid/sqlitefid.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_droid_handler.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_droid_handler.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_fido_handler.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_fido_handler.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_identify_export.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_identify_export.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sf_handler.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sf_handler.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sf_internal_functions.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sf_internal_functions.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sqlite_basedb.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sqlite_basedb.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sqlite_output_droid.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sqlite_output_droid.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_sqlite_output_sf.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_sqlite_output_sf.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify/sqlitefid/tests/test_utilities.py` & `demystify_digipres-2.0.0rc7/src/demystify/sqlitefid/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/src/demystify_digipres.egg-info/PKG-INFO` & `demystify_digipres-2.0.0rc7/src/demystify_digipres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demystify-digipres
-Version: 2.0.0rc6
+Version: 2.0.0rc7
 Summary: engine for the analysis of DROID and Siegfried file format reports
 Author: Ross Spencer
 License: Copyright (c) 2013 Ross Spencer
         
         This software is provided 'as-is', without any express or implied warranty. In
         no event will the authors be held liable for any damages arising from the use
         of this software.
```

### Comparing `demystify-digipres-2.0.0rc6/src/demystify_digipres.egg-info/SOURCES.txt` & `demystify_digipres-2.0.0rc7/src/demystify_digipres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/tests/test_deny_list.py` & `demystify_digipres-2.0.0rc7/tests/test_deny_list.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/tests/test_droid_analysis.py` & `demystify_digipres-2.0.0rc7/tests/test_droid_analysis.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/tests/test_rogues_list.py` & `demystify_digipres-2.0.0rc7/tests/test_rogues_list.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/tests/test_siegfried_analysis.py` & `demystify_digipres-2.0.0rc7/tests/test_siegfried_analysis.py`

 * *Files identical despite different names*

### Comparing `demystify-digipres-2.0.0rc6/tox.ini` & `demystify_digipres-2.0.0rc7/tox.ini`

 * *Files identical despite different names*

