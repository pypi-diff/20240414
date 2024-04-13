# Comparing `tmp/enma-2.3.1.tar.gz` & `tmp/enma-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enma-2.3.1.tar", last modified: Fri Mar  8 20:43:41 2024, max compression
+gzip compressed data, was "enma-2.4.1.tar", last modified: Sat Apr 13 22:44:36 2024, max compression
```

## Comparing `enma-2.3.1.tar` & `enma-2.4.1.tar`

### file list

```diff
@@ -1,87 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.368605 enma-2.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.356604 enma-2.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-08 20:43:22.000000 enma-2.3.1/.github/workflows/dev-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-08 20:43:22.000000 enma-2.3.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-08 20:43:22.000000 enma-2.3.1/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-08 20:43:22.000000 enma-2.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-08 20:43:22.000000 enma-2.3.1/.python-version
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.356604 enma-2.3.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-08 20:43:22.000000 enma-2.3.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-08 20:43:22.000000 enma-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-03-08 20:43:41.368605 enma-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-03-08 20:43:22.000000 enma-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.360604 enma-2.3.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)  4809136 2024-03-08 20:43:22.000000 enma-2.3.1/docs/images/enma.png
--rw-r--r--   0 runner    (1001) docker     (127)    70607 2024-03-08 20:43:22.000000 enma-2.3.1/docs/images/user-agent.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.360604 enma-2.3.1/enma/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-08 20:43:22.000000 enma-2.3.1/enma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-08 20:43:22.000000 enma-2.3.1/enma/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/enma/application/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/enma/application/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.364604 enma-2.3.1/enma/application/core/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/core/handlers/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.364604 enma-2.3.1/enma/application/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/core/interfaces/downloader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/core/interfaces/manga_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/core/interfaces/saver_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/core/interfaces/use_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.364604 enma-2.3.1/enma/application/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/core/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.364604 enma-2.3.1/enma/application/use_cases/
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/use_cases/download_chapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/use_cases/fetch_chapter_by_symbolic_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/use_cases/get_author_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/use_cases/get_manga.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/use_cases/get_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/use_cases/paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-08 20:43:22.000000 enma-2.3.1/enma/application/use_cases/search_manga.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/enma/domain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.364604 enma-2.3.1/enma/domain/entities/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-08 20:43:22.000000 enma-2.3.1/enma/domain/entities/author_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-08 20:43:22.000000 enma-2.3.1/enma/domain/entities/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-08 20:43:22.000000 enma-2.3.1/enma/domain/entities/manga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-08 20:43:22.000000 enma-2.3.1/enma/domain/entities/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-08 20:43:22.000000 enma-2.3.1/enma/domain/entities/search_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/enma/infra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/enma/infra/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.364604 enma-2.3.1/enma/infra/adapters/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-08 20:43:22.000000 enma-2.3.1/enma/infra/adapters/downloaders/default.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-08 20:43:22.000000 enma-2.3.1/enma/infra/adapters/downloaders/manganato.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.364604 enma-2.3.1/enma/infra/adapters/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-08 20:43:22.000000 enma-2.3.1/enma/infra/adapters/repositories/manganato.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-03-08 20:43:22.000000 enma-2.3.1/enma/infra/adapters/repositories/nhentai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.364604 enma-2.3.1/enma/infra/adapters/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-08 20:43:22.000000 enma-2.3.1/enma/infra/adapters/storage/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/enma/infra/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.368605 enma-2.3.1/enma/infra/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-08 20:43:22.000000 enma-2.3.1/enma/infra/core/interfaces/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-08 20:43:22.000000 enma-2.3.1/enma/infra/core/interfaces/nhentai_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.352604 enma-2.3.1/enma/infra/entrypoints/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.368605 enma-2.3.1/enma/infra/entrypoints/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-03-08 20:43:22.000000 enma-2.3.1/enma/infra/entrypoints/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.368605 enma-2.3.1/enma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-03-08 20:43:41.000000 enma-2.3.1/enma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-08 20:43:41.000000 enma-2.3.1/enma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:43:41.000000 enma-2.3.1/enma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-08 20:43:41.000000 enma-2.3.1/enma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-08 20:43:41.000000 enma-2.3.1/enma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-08 20:43:22.000000 enma-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-08 20:43:22.000000 enma-2.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-08 20:43:41.372604 enma-2.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.368605 enma-2.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:43:41.368605 enma-2.3.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/get.json
--rw-r--r--   0 runner    (1001) docker     (127)    67921 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/manganato_manga_page_empty_chapters_mock.txt
--rw-r--r--   0 runner    (1001) docker     (127)    53434 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/manganato_manga_page_empty_pagination_mock.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/mocked_doujins.py
--rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/nhentai_author_page_mock.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/nhentai_author_page_not_found_mock.txt
--rw-r--r--   0 runner    (1001) docker     (127)   118408 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/nhentai_paginate_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)    21363 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/nhentai_search_mock.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-08 20:43:22.000000 enma-2.3.1/tests/data/nhentai_search_no_result.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-03-08 20:43:22.000000 enma-2.3.1/tests/test_manganato_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-03-08 20:43:22.000000 enma-2.3.1/tests/test_nhentai_fetch_chapter_by_symbolic_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-03-08 20:43:22.000000 enma-2.3.1/tests/test_nhentai_get_manga_use_case.py
--rw-r--r--   0 runner    (1001) docker     (127)    17047 2024-03-08 20:43:22.000000 enma-2.3.1/tests/test_nhentai_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.894829 enma-2.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.878829 enma-2.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-13 22:44:10.000000 enma-2.4.1/.github/workflows/dev-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-13 22:44:10.000000 enma-2.4.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-13 22:44:10.000000 enma-2.4.1/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-13 22:44:10.000000 enma-2.4.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.878829 enma-2.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-13 22:44:10.000000 enma-2.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-13 22:44:10.000000 enma-2.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-13 22:44:10.000000 enma-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-13 22:44:36.894829 enma-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-04-13 22:44:10.000000 enma-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.882829 enma-2.4.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)  4809136 2024-04-13 22:44:10.000000 enma-2.4.1/docs/images/enma.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70607 2024-04-13 22:44:10.000000 enma-2.4.1/docs/images/user-agent.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.882829 enma-2.4.1/enma/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-13 22:44:10.000000 enma-2.4.1/enma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 22:44:36.000000 enma-2.4.1/enma/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/enma/application/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/enma/application/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.886829 enma-2.4.1/enma/application/core/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/core/handlers/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.886829 enma-2.4.1/enma/application/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/core/interfaces/downloader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/core/interfaces/manga_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/core/interfaces/saver_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/core/interfaces/use_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.886829 enma-2.4.1/enma/application/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/core/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.886829 enma-2.4.1/enma/application/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/use_cases/download_chapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/use_cases/fetch_chapter_by_symbolic_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/use_cases/get_author_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/use_cases/get_manga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/use_cases/get_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/use_cases/paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-13 22:44:10.000000 enma-2.4.1/enma/application/use_cases/search_manga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/enma/domain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.886829 enma-2.4.1/enma/domain/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-13 22:44:10.000000 enma-2.4.1/enma/domain/entities/author_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-13 22:44:10.000000 enma-2.4.1/enma/domain/entities/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-13 22:44:10.000000 enma-2.4.1/enma/domain/entities/manga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-13 22:44:10.000000 enma-2.4.1/enma/domain/entities/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-13 22:44:10.000000 enma-2.4.1/enma/domain/entities/search_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/enma/infra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/enma/infra/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.886829 enma-2.4.1/enma/infra/adapters/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/adapters/downloaders/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/adapters/downloaders/manganato.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.890829 enma-2.4.1/enma/infra/adapters/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)    25192 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/adapters/repositories/mangadex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/adapters/repositories/manganato.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18839 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/adapters/repositories/nhentai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.890829 enma-2.4.1/enma/infra/adapters/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/adapters/storage/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/enma/infra/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.890829 enma-2.4.1/enma/infra/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/core/interfaces/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/core/interfaces/mangadex_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/core/interfaces/nhentai_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.890829 enma-2.4.1/enma/infra/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/core/utils/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.874829 enma-2.4.1/enma/infra/entrypoints/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.890829 enma-2.4.1/enma/infra/entrypoints/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-13 22:44:10.000000 enma-2.4.1/enma/infra/entrypoints/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.894829 enma-2.4.1/enma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-13 22:44:36.000000 enma-2.4.1/enma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-13 22:44:36.000000 enma-2.4.1/enma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:44:36.000000 enma-2.4.1/enma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 22:44:36.000000 enma-2.4.1/enma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 22:44:36.000000 enma-2.4.1/enma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-13 22:44:10.000000 enma-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-13 22:44:10.000000 enma-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-13 22:44:36.894829 enma-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.890829 enma-2.4.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:44:36.894829 enma-2.4.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/get.json
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/mangadex_empty_chapters.json
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/mangadex_empty_pagination_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)    67921 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/manganato_manga_page_empty_chapters_mock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    53434 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/manganato_manga_page_empty_pagination_mock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/mocked_doujins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/nhentai_author_page_mock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/nhentai_author_page_not_found_mock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   118408 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/nhentai_paginate_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21363 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/nhentai_search_mock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-13 22:44:10.000000 enma-2.4.1/tests/data/nhentai_search_no_result.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-13 22:44:10.000000 enma-2.4.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-04-13 22:44:10.000000 enma-2.4.1/tests/test_mangadex_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6494 2024-04-13 22:44:10.000000 enma-2.4.1/tests/test_manganato_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-04-13 22:44:10.000000 enma-2.4.1/tests/test_nhentai_fetch_chapter_by_symbolic_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-13 22:44:10.000000 enma-2.4.1/tests/test_nhentai_get_manga_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-04-13 22:44:10.000000 enma-2.4.1/tests/test_nhentai_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-13 22:44:10.000000 enma-2.4.1/tests/test_search_result_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-13 22:44:10.000000 enma-2.4.1/tests/test_source_manager.py
```

### Comparing `enma-2.3.1/.github/workflows/testing.yml` & `enma-2.4.1/.github/workflows/testing.yml`

 * *Files 26% similar despite different names*

```diff
@@ -20,19 +20,23 @@
         uses: actions/setup-python@master
         with:
           python-version: 3.9
 
       - name: Preparing the environment
         run: |
           python -m pip install --upgrade pip
-          if [ -f requirements.txt ]; then python -m pip install -r requirements.txt; else python -m pip install beautifulsoup4 requests pydantic; fi
-          python -m pip install pytest==7.0.1 pytest-cov==4.1.0
+          if [ -f requirements.txt ]; then python -m pip install -r requirements.txt; else python -m pip install beautifulsoup4 requests pydantic expiringdict pytest pytest-cov; fi
 
       - name: Starting Testing Suites
         run: |
+          ENMA_CACHING_PAGINATE_TTL_IN_SECONDS='0' \
+          ENMA_CACHING_SEARCH_TTL_IN_SECONDS='0' \
+          ENMA_CACHING_GET_TTL_IN_SECONDS='0' \
+          ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS='0' \
+          ENMA_CACHING_AUTHOR_TTL_IN_SECONDS='0' \
           pytest --cov=. --cov-report=xml ./tests
 
       - name: Upload Report to Codecov
         uses: codecov/codecov-action@v1
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           file: ./coverage.xml
```

### Comparing `enma-2.3.1/.gitignore` & `enma-2.4.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 lib64/
 parts/
 sdist/
 var/
 *.egg-info/
 .installed.cfg
 *.egg
+*.sh
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 .tox/
```

### Comparing `enma-2.3.1/PKG-INFO` & `enma-2.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: enma
-Version: 2.3.1
+Version: 2.4.1
 Summary: Enma is a Python library designed to fetch manga and doujinshi data from many sources.
 Home-page: https://github.com/AlexandreSenpai/Enma
 Author: AlexandreSenpai
 Author-email: alexandrebsramos@hotmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests==2.31.0
 Requires-Dist: beautifulsoup4==4.10.0
 Requires-Dist: pydantic==2.5.3
+Requires-Dist: expiringdict==1.2.2
 
 <p align="center">
     <img src="./docs/images/enma.png" align="center" width="50%">
 </p>
 
 <center>
 
@@ -31,14 +32,17 @@
 
 </center>
 
 # Enma
 
 Enma is a Python library designed to fetch manga and doujinshi data from many sources. It provides a unified interface to interact with different manga repositories, making it easier to retrieve manga details, search for manga, paginate through results, and fetch random manga.
 
+## :warning: Warning
+> **:exclamation: Important: Enma is not intended for mass querying or placing heavy loads on supported sources. Please use responsibly, adhering to the terms of service of the data sources. Misuse may result in service disruption or access denial.**
+
 ## Requirements
 
 - Python 3.9+
 
 ## Installation
 ```py
 pip install --upgrade enma
@@ -59,23 +63,24 @@
 ```
 
 ## Documentation
 You can consult full Enma documentation at <strong><a href="https://enma.gitbook.io/enma" target="_blank">https://enma.gitbook.io/enma</a></strong>.
 
 ## Features Comparison
 
-Feature    | NHentai | Manganato
------------|---------|-----------
-search     |    ✅   |     ✅    
-random     |    ✅   |     🚫    
-get        |    ✅   |     ✅    
-paginate   |    ✅   |     ✅
-download   |    ✅   |     ✅       
-author_page|    ✅   |     🚫       
-set_config |    ✅   |     🚫
+Feature    | NHentai | Manganato | Mangadex
+-----------|---------|-----------|-----------
+search     |    ✅   |     ✅   |   ✅
+random     |    ✅   |     🚫   |   ✅  
+get        |    ✅   |     ✅   |   ✅
+paginate   |    ✅   |     ✅   |   ✅
+download   |    ✅   |     ✅   |   ✅  
+author_page|    ✅   |     🚫   |   🚫   
+set_config |    ✅   |     🚫   |   🚫
+caching    |    ✅   |     ✅   |   ✅
 
 ## Usage
 
 ### Example 1: Using Default Available Sources
 
 ```py
 from typing import cast
@@ -111,14 +116,48 @@
 enma.source_manager.add_source(source_name='new-source', source=Manganato()) # Source MUST be an instance of IMangaRepository
 enma.source_manager.set_source(source_name=AvailableSources.MANGANATO)
 
 manga = enma.random()
 print(manga)
 ```
 
+## Caching
+Caching is a key feature in Enma that improves your application's efficiency by storing the results of data requests. This means when the same data is requested again, Enma can quickly retrieve it from the cache instead of repeatedly calling the external source. This results in faster response times and less strain on both your application and the external APIs.
+
+### How Caching Benefits You
+- **Speed**: Retrieving data from the cache is faster than making a new request to a manga repository.
+- **Efficiency**: Reduces the number of network requests, which is especially useful when dealing with rate-limited APIs.
+- **Reliability**: Provides more consistent application performance even with varying network conditions.
+
+### Customizing Cache Settings
+While Enma provides default caching settings that suit most needs, you may want to customize these settings based on your specific requirements, like how often you expect data to change or specific API rate limits.
+
+#### Adjusting Cache Duration via Environment Variables
+You can control how long data is kept in the cache by setting environment variables. This allows you to fine-tune the balance between data freshness and retrieval speed without modifying the core library code.
+
+For example, to change the cache expiration for fetching chapters, you can set the `ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS` environment variable:
+
+```sh
+# Sets the cache duration to 30 minutes
+export ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS=1800
+```
+
+This customization capability ensures that you can adapt the caching behavior to best fit your application's performance and efficiency needs.
+
+By leveraging caching, Enma helps make your manga-related applications faster and more reliable, all while giving you the flexibility to tailor caching behavior as needed.
+
+#### Available Caching TTL Settings
+| KEY                                            | DEFAULT |
+|------------------------------------------------|---------|
+| ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS| 100     |
+| ENMA_CACHING_PAGINATE_TTL_IN_SECONDS           | 100     |
+| ENMA_CACHING_SEARCH_TTL_IN_SECONDS             | 100     |
+| ENMA_CACHING_GET_TTL_IN_SECONDS                | 300     |
+| ENMA_CACHING_AUTHOR_TTL_IN_SECONDS             | 100     |
+
 ## Downloading Chapters
 Using Enma you're able to download chapter pages to your local storage or any other storage that implements `ISaverAdapter`.
 
 You can check it out how to do it right below:
 
 ```py
 from enma import (Enma,
@@ -159,31 +198,14 @@
 from enma import Enma
 
 enma = Enma()
 
 enma.source_manager.set_source('manganato')
 doujin = enma.get(identifier='manga-kb951984', with_symbolic_links=True)
 
-# Manga(id='manga-kb951984', 
-#       created_at=datetime.datetime(2024, 1, 22, 10, 5), 
-#       updated_at=datetime.datetime(2024, 1, 22, 10, 5), 
-#       title=Title(english='Monster Musume No Iru Nichijou', 
-#                   japanese='モンスター娘のいる日常', 
-#                   other='魔物娘的同居日常'), 
-#       language=None, 
-#       cover=Image(uri='https://avt.mkklcdnv6temp.com/23/p/1-1583464626.jpg', name='image.jpg', width=0, height=0, mime=<MIME.J: 'jpg'>), 
-#       thumbnail=Image(uri='https://avt.mkklcdnv6temp.com/23/p/1-1583464626.jpg', name='image.jpg', width=0, height=0, mime=<MIME.J: 'jpg'>), 
-#       authors=[Author(name='Okayado', id=0)], 
-#       genres=[Genre(name='Comedy', id=0), 
-#               Genre(name='Fantasy', id=0), 
-#               Genre(name='Harem', id=0)], 
-#       chapters=[Chapter(id='chapter-84', pages=[], pages_count=0, link=SymbolicLink(link='https://chapmanganato.to/manga-kb951984/chapter-84')), 
-#                 Chapter(id='chapter-83', pages=[], pages_count=0, link=SymbolicLink(link='https://chapmanganato.to/manga-kb951984/chapter-83'))], 
-#       chapters_count=95)
-
 if doujin is not None:
     chapter_ref = doujin.chapters[0]
     chapter = enma.fetch_chapter_by_symbolic_link(link=chapter_ref.link)
 
 ```
 
 ## Retrieving `user-agent` and `cf_clearance` for NHentai
@@ -241,14 +263,31 @@
     - **Description**: Raised when trying to perform an action with an invalid or inexistent resource.
     - **Common Cause**: Providing an inexistent folder path to downloader.
 
 7. **InvalidRequest**:
     - **Description**: Raised when trying to perform an action with an invalid data type.
     - **Common Cause**: Making an action with wrong parameter data type.
 
+7. **Unknown**:
+    - **Description**: Raised when was not possible to determine the error root cause.
+    - **Common Cause**: Not properly handled error.
+
+7. **NotFound**:
+    - **Description**: Raised when was not possible to find the requested resource..
+    - **Common Cause**: Fetching an inexistent resource.
+
+7. **Forbidden**:
+    - **Description**: Raised when trying to perform a request to the source without right credentials.
+    - **Common Cause**: Making a request with no or invalid credentials.
+
+7. **ExceedRateLimit**:
+    - **Description**: Raised when trying to perform more requests than a server can handle.
+    - **Common Cause**: Looping through many pages without cooling down.
+
+
 When encountering one of these errors, refer to the description and common cause to assist in troubleshooting.
 
 ## Future Plans
 
 We are actively working on introducing an asynchronous version of the Enma library to better cater to applications that require non-blocking operations. This version will be maintained in a separate repository to keep the core library lightweight. However, for ease of access and installation, you'll be able to install the asynchronous version directly using:
 
 ```bash
@@ -272,10 +311,22 @@
 
 1. Fork the repository.
 2. Make your changes.
 3. Submit a pull request.
 
 Ensure you follow the coding standards and write tests for new features.
 
+## Disclaimer
+
+This software is provided "as is", without warranty of any kind, express or implied. The developers and contributors of the Enma library shall not be liable for any misuse, damages, or other consequences arising from the use of this software.
+
+It is important to emphasize that the Enma library was developed with the goal of facilitating efficient and responsible access and manipulation of data. We do not encourage or support the use of this tool for conducting mass queries or accesses that could overload, harm, or in any way negatively affect the servers or services of the supported sources.
+
+Users of the Enma library must always follow the guidelines, terms of use, and limitations imposed by the accessed data sources. We strongly recommend the implementation of responsible rate limiting practices and obtaining appropriate permissions when necessary, to ensure that the use of the library complies with all applicable laws and regulations, in addition to respecting ethical principles of data use.
+
+By using the Enma library, you agree to use the tool in an ethical and responsible manner, acknowledging that the developers of Enma will not be responsible for any use that violates these guidelines.
+
+We remind you that respect for the services and APIs of the supported sources is fundamental for the sustainability and longevity of both the Enma and the services used. We value the community and the development ecosystem and encourage all users to contribute to a safer, more respectful, and collaborative digital environment.
+
 ## License
 
 MIT
```

### Comparing `enma-2.3.1/README.md` & `enma-2.4.1/enma.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: enma
+Version: 2.4.1
+Summary: Enma is a Python library designed to fetch manga and doujinshi data from many sources.
+Home-page: https://github.com/AlexandreSenpai/Enma
+Author: AlexandreSenpai
+Author-email: alexandrebsramos@hotmail.com
+License: LICENSE
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: requests==2.31.0
+Requires-Dist: beautifulsoup4==4.10.0
+Requires-Dist: pydantic==2.5.3
+Requires-Dist: expiringdict==1.2.2
+
 <p align="center">
     <img src="./docs/images/enma.png" align="center" width="50%">
 </p>
 
 <center>
 
 [![PyPI download month](https://img.shields.io/pypi/dm/Enma.svg)](https://pypi.python.org/pypi/Enma/)
@@ -14,14 +32,17 @@
 
 </center>
 
 # Enma
 
 Enma is a Python library designed to fetch manga and doujinshi data from many sources. It provides a unified interface to interact with different manga repositories, making it easier to retrieve manga details, search for manga, paginate through results, and fetch random manga.
 
+## :warning: Warning
+> **:exclamation: Important: Enma is not intended for mass querying or placing heavy loads on supported sources. Please use responsibly, adhering to the terms of service of the data sources. Misuse may result in service disruption or access denial.**
+
 ## Requirements
 
 - Python 3.9+
 
 ## Installation
 ```py
 pip install --upgrade enma
@@ -42,23 +63,24 @@
 ```
 
 ## Documentation
 You can consult full Enma documentation at <strong><a href="https://enma.gitbook.io/enma" target="_blank">https://enma.gitbook.io/enma</a></strong>.
 
 ## Features Comparison
 
-Feature    | NHentai | Manganato
------------|---------|-----------
-search     |    ✅   |     ✅    
-random     |    ✅   |     🚫    
-get        |    ✅   |     ✅    
-paginate   |    ✅   |     ✅
-download   |    ✅   |     ✅       
-author_page|    ✅   |     🚫       
-set_config |    ✅   |     🚫
+Feature    | NHentai | Manganato | Mangadex
+-----------|---------|-----------|-----------
+search     |    ✅   |     ✅   |   ✅
+random     |    ✅   |     🚫   |   ✅  
+get        |    ✅   |     ✅   |   ✅
+paginate   |    ✅   |     ✅   |   ✅
+download   |    ✅   |     ✅   |   ✅  
+author_page|    ✅   |     🚫   |   🚫   
+set_config |    ✅   |     🚫   |   🚫
+caching    |    ✅   |     ✅   |   ✅
 
 ## Usage
 
 ### Example 1: Using Default Available Sources
 
 ```py
 from typing import cast
@@ -94,14 +116,48 @@
 enma.source_manager.add_source(source_name='new-source', source=Manganato()) # Source MUST be an instance of IMangaRepository
 enma.source_manager.set_source(source_name=AvailableSources.MANGANATO)
 
 manga = enma.random()
 print(manga)
 ```
 
+## Caching
+Caching is a key feature in Enma that improves your application's efficiency by storing the results of data requests. This means when the same data is requested again, Enma can quickly retrieve it from the cache instead of repeatedly calling the external source. This results in faster response times and less strain on both your application and the external APIs.
+
+### How Caching Benefits You
+- **Speed**: Retrieving data from the cache is faster than making a new request to a manga repository.
+- **Efficiency**: Reduces the number of network requests, which is especially useful when dealing with rate-limited APIs.
+- **Reliability**: Provides more consistent application performance even with varying network conditions.
+
+### Customizing Cache Settings
+While Enma provides default caching settings that suit most needs, you may want to customize these settings based on your specific requirements, like how often you expect data to change or specific API rate limits.
+
+#### Adjusting Cache Duration via Environment Variables
+You can control how long data is kept in the cache by setting environment variables. This allows you to fine-tune the balance between data freshness and retrieval speed without modifying the core library code.
+
+For example, to change the cache expiration for fetching chapters, you can set the `ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS` environment variable:
+
+```sh
+# Sets the cache duration to 30 minutes
+export ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS=1800
+```
+
+This customization capability ensures that you can adapt the caching behavior to best fit your application's performance and efficiency needs.
+
+By leveraging caching, Enma helps make your manga-related applications faster and more reliable, all while giving you the flexibility to tailor caching behavior as needed.
+
+#### Available Caching TTL Settings
+| KEY                                            | DEFAULT |
+|------------------------------------------------|---------|
+| ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS| 100     |
+| ENMA_CACHING_PAGINATE_TTL_IN_SECONDS           | 100     |
+| ENMA_CACHING_SEARCH_TTL_IN_SECONDS             | 100     |
+| ENMA_CACHING_GET_TTL_IN_SECONDS                | 300     |
+| ENMA_CACHING_AUTHOR_TTL_IN_SECONDS             | 100     |
+
 ## Downloading Chapters
 Using Enma you're able to download chapter pages to your local storage or any other storage that implements `ISaverAdapter`.
 
 You can check it out how to do it right below:
 
 ```py
 from enma import (Enma,
@@ -142,31 +198,14 @@
 from enma import Enma
 
 enma = Enma()
 
 enma.source_manager.set_source('manganato')
 doujin = enma.get(identifier='manga-kb951984', with_symbolic_links=True)
 
-# Manga(id='manga-kb951984', 
-#       created_at=datetime.datetime(2024, 1, 22, 10, 5), 
-#       updated_at=datetime.datetime(2024, 1, 22, 10, 5), 
-#       title=Title(english='Monster Musume No Iru Nichijou', 
-#                   japanese='モンスター娘のいる日常', 
-#                   other='魔物娘的同居日常'), 
-#       language=None, 
-#       cover=Image(uri='https://avt.mkklcdnv6temp.com/23/p/1-1583464626.jpg', name='image.jpg', width=0, height=0, mime=<MIME.J: 'jpg'>), 
-#       thumbnail=Image(uri='https://avt.mkklcdnv6temp.com/23/p/1-1583464626.jpg', name='image.jpg', width=0, height=0, mime=<MIME.J: 'jpg'>), 
-#       authors=[Author(name='Okayado', id=0)], 
-#       genres=[Genre(name='Comedy', id=0), 
-#               Genre(name='Fantasy', id=0), 
-#               Genre(name='Harem', id=0)], 
-#       chapters=[Chapter(id='chapter-84', pages=[], pages_count=0, link=SymbolicLink(link='https://chapmanganato.to/manga-kb951984/chapter-84')), 
-#                 Chapter(id='chapter-83', pages=[], pages_count=0, link=SymbolicLink(link='https://chapmanganato.to/manga-kb951984/chapter-83'))], 
-#       chapters_count=95)
-
 if doujin is not None:
     chapter_ref = doujin.chapters[0]
     chapter = enma.fetch_chapter_by_symbolic_link(link=chapter_ref.link)
 
 ```
 
 ## Retrieving `user-agent` and `cf_clearance` for NHentai
@@ -224,14 +263,31 @@
     - **Description**: Raised when trying to perform an action with an invalid or inexistent resource.
     - **Common Cause**: Providing an inexistent folder path to downloader.
 
 7. **InvalidRequest**:
     - **Description**: Raised when trying to perform an action with an invalid data type.
     - **Common Cause**: Making an action with wrong parameter data type.
 
+7. **Unknown**:
+    - **Description**: Raised when was not possible to determine the error root cause.
+    - **Common Cause**: Not properly handled error.
+
+7. **NotFound**:
+    - **Description**: Raised when was not possible to find the requested resource..
+    - **Common Cause**: Fetching an inexistent resource.
+
+7. **Forbidden**:
+    - **Description**: Raised when trying to perform a request to the source without right credentials.
+    - **Common Cause**: Making a request with no or invalid credentials.
+
+7. **ExceedRateLimit**:
+    - **Description**: Raised when trying to perform more requests than a server can handle.
+    - **Common Cause**: Looping through many pages without cooling down.
+
+
 When encountering one of these errors, refer to the description and common cause to assist in troubleshooting.
 
 ## Future Plans
 
 We are actively working on introducing an asynchronous version of the Enma library to better cater to applications that require non-blocking operations. This version will be maintained in a separate repository to keep the core library lightweight. However, for ease of access and installation, you'll be able to install the asynchronous version directly using:
 
 ```bash
@@ -255,10 +311,22 @@
 
 1. Fork the repository.
 2. Make your changes.
 3. Submit a pull request.
 
 Ensure you follow the coding standards and write tests for new features.
 
+## Disclaimer
+
+This software is provided "as is", without warranty of any kind, express or implied. The developers and contributors of the Enma library shall not be liable for any misuse, damages, or other consequences arising from the use of this software.
+
+It is important to emphasize that the Enma library was developed with the goal of facilitating efficient and responsible access and manipulation of data. We do not encourage or support the use of this tool for conducting mass queries or accesses that could overload, harm, or in any way negatively affect the servers or services of the supported sources.
+
+Users of the Enma library must always follow the guidelines, terms of use, and limitations imposed by the accessed data sources. We strongly recommend the implementation of responsible rate limiting practices and obtaining appropriate permissions when necessary, to ensure that the use of the library complies with all applicable laws and regulations, in addition to respecting ethical principles of data use.
+
+By using the Enma library, you agree to use the tool in an ethical and responsible manner, acknowledging that the developers of Enma will not be responsible for any use that violates these guidelines.
+
+We remind you that respect for the services and APIs of the supported sources is fundamental for the sustainability and longevity of both the Enma and the services used. We value the community and the development ecosystem and encourage all users to contribute to a safer, more respectful, and collaborative digital environment.
+
 ## License
 
 MIT
```

### Comparing `enma-2.3.1/docs/images/enma.png` & `enma-2.4.1/docs/images/enma.png`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/docs/images/user-agent.png` & `enma-2.4.1/docs/images/user-agent.png`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/__init__.py` & `enma-2.4.1/enma/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import sys
 from enma.application.core.utils.logger import LogMode, logger
 from enma.application.use_cases.download_chapter import Threaded
-from enma.infra.entrypoints.lib import Enma, SourcesEnum, DefaultAvailableSources
-from enma.infra.adapters.repositories.nhentai import CloudFlareConfig, NHentai, Sort
+from enma.infra.entrypoints.lib import Enma, Sources
+from enma.infra.adapters.repositories.nhentai import CloudFlareConfig, NHentai, Sort as NHentaiSort
+from enma.infra.adapters.repositories.mangadex import Mangadex, Sort as MangadexSort
 from enma.infra.adapters.repositories.manganato import Manganato
 from enma.infra.adapters.downloaders.default import DefaultDownloader
 from enma.infra.adapters.downloaders.manganato import ManganatoDownloader
 from enma.application.core.interfaces.downloader_adapter import IDownloaderAdapter
 from enma.application.core.interfaces.saver_adapter import ISaverAdapter
 from enma.infra.adapters.storage.local import LocalStorage
-from enma.domain.entities.manga import Manga
+from enma.domain.entities.manga import Manga, Chapter, SymbolicLink
 from enma.domain.entities.search_result import SearchResult
 from enma.domain.entities.pagination import Pagination
 from enma.domain.entities.author_page import AuthorPage
+from enma.application.core.interfaces.manga_repository import IMangaRepository
 
 package_name = "enma"
 python_major = "3"
 python_minor = "9"
 
 logger.mode = LogMode.SILENT
```

### Comparing `enma-2.3.1/enma/application/core/handlers/error.py` & `enma-2.4.1/enma/application/core/handlers/error.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,38 @@
         super().__init__(message)
 
         self.message: str = message
         self.code: str = 'SOURCE_NOT_AVAILABLE'
         self.desc: str = 'This error occurs when the client chooses nonexistent source.'
         self.critical: bool = False
 
+class Unknown(Exception):
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
+
+        self.code: str = 'UNKNOWN'
+        self.desc: str = 'This error occours when was not possible to determine the error root cause.'
+        self.critical: bool = True
+
+class NotFound(Exception):
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
+
+        self.code: str = 'NOT_FOUND'
+        self.desc: str = 'This error occours when was not possible to find the requested resource.'
+        self.critical: bool = True
+
+class Forbidden(Exception):
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
+
+        self.code: str = 'FORBIDDEN'
+        self.desc: str = 'This error occours when the client can\'t perform a request to the source due lack of credentials.'
+        self.critical: bool = True
+
 class InvalidRequest(Exception):
     def __init__(self, message: str) -> None:
         super().__init__(message)
 
         self.code: str = 'INVALID_REQUEST'
         self.desc: str = 'This error occours when the client tries to perform an request with wrong data input.'
         self.critical: bool = True
@@ -63,8 +87,17 @@
 class ExceedRetryCount(Exception):
     def __init__(self, message: str) -> None:
         super().__init__(message)
 
         self.message: str = message
         self.code: str = 'EXCEED_RETRY_COUNT'
         self.desc: str = 'This error occurs when enma tries perform some action but something went wrong.'
-        self.critical: bool = True
+        self.critical: bool = True
+
+class ExceedRateLimit(Exception):
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
+
+        self.message: str = message
+        self.code: str = 'EXCEED_RATE_EXCEED'
+        self.desc: str = 'This error occurs when enma perform more requests than a server can handle. Cool down your requests to this source!'
+        self.critical: bool = False
```

### Comparing `enma-2.3.1/enma/application/core/interfaces/manga_repository.py` & `enma-2.4.1/enma/application/core/interfaces/manga_repository.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/application/core/utils/logger.py` & `enma-2.4.1/enma/application/core/utils/logger.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/application/use_cases/download_chapter.py` & `enma-2.4.1/enma/application/use_cases/download_chapter.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/application/use_cases/fetch_chapter_by_symbolic_link.py` & `enma-2.4.1/enma/application/use_cases/fetch_chapter_by_symbolic_link.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/application/use_cases/get_author_page.py` & `enma-2.4.1/enma/application/use_cases/get_author_page.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/application/use_cases/get_manga.py` & `enma-2.4.1/enma/application/use_cases/get_manga.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Union
 
 from pydantic import BaseModel, Field, validator
-from enma.application.core.handlers.error import InvalidRequest
+from enma.application.core.handlers import error
 from enma.application.core.interfaces.manga_repository import IMangaRepository
 from enma.application.core.interfaces.use_case import DTO, IUseCase
 from enma.application.core.utils.logger import logger
 from enma.domain.entities.manga import Manga
 
 class GetMangaRequestDTO(BaseModel):
     identifier: str
@@ -20,13 +20,14 @@
     
     def __init__(self, manga_repository: IMangaRepository):
         self.__manga_repository = manga_repository
 
     def execute(self, dto: DTO[GetMangaRequestDTO]) -> GetMangaResponseDTO:
         logger.info(f'Fetching manga with identifier: {dto.data.identifier}.')
 
-        manga = self.__manga_repository.get(identifier=dto.data.identifier,
-                                            with_symbolic_links=dto.data.with_symbolic_links)
-        
-        if manga is None: return GetMangaResponseDTO(found=False, manga=None)
-        
-        return GetMangaResponseDTO(found=True, manga=manga)
+        try:
+            manga = self.__manga_repository.get(identifier=dto.data.identifier,
+                                                with_symbolic_links=dto.data.with_symbolic_links)
+            return GetMangaResponseDTO(found=True, manga=manga)
+        except error.NotFound:
+            logger.error(f'Could not find the manga using the provided identifier: {dto.data.identifier}')
+            return GetMangaResponseDTO(found=False, manga=None)
```

### Comparing `enma-2.3.1/enma/application/use_cases/get_random.py` & `enma-2.4.1/enma/application/use_cases/get_random.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/application/use_cases/paginate.py` & `enma-2.4.1/enma/application/use_cases/paginate.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/application/use_cases/search_manga.py` & `enma-2.4.1/enma/application/use_cases/search_manga.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/domain/entities/author_page.py` & `enma-2.4.1/enma/domain/entities/author_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
 This module defines the SearchResult entity for the Enma application.
 It represents the result of a manga search operation.
 """
-from dataclasses import dataclass
 from datetime import datetime
 from typing import TypedDict, Union
 from enma.domain.entities.manga import Manga
 from enma.domain.entities.pagination import Pagination, Thumb
 
 class ISearchResultProps(TypedDict):
     id: Union[int, str]
     created_at: datetime
     updated_at: datetime
     page: int
     total_pages: int
     total_results: int
     results: list[Manga]
 
-@dataclass
 class AuthorPage(Pagination):
     """
     Entity class representing a search result in the Enma application.
     """
     author: str
 
     def __init__(self,
```

### Comparing `enma-2.3.1/enma/domain/entities/pagination.py` & `enma-2.4.1/enma/domain/entities/pagination.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from typing import TypedDict, Union
 from enma.domain.entities.base import Entity
 from enma.domain.entities.manga import Image, Manga
 
 @dataclass
 class Thumb:
     id: str
+    url: str
     title: str
     cover: Image
 
 class ISearchResultProps(TypedDict):
     id: Union[int, str]
     created_at: datetime
     updated_at: datetime
     page: int
     total_pages: int
     total_results: int
     results: list[Manga]
 
-@dataclass
 class Pagination(Entity[ISearchResultProps]):
     """
     Entity class representing a search result in the Enma application.
     """
     page: int
     total_pages: int
     total_results: int
@@ -44,10 +44,9 @@
         
         super().__init__(id=id,
                          created_at=created_at,
                          updated_at=updated_at)
         
         self.page = page
         self.results = results or list()
-        self.total_pages = total_pages or 1 if len(self.results) <= 20 else total_pages
-        self.total_results = total_results or 20 * self.total_pages if self.total_pages > 1 else len(self.results) 
-        
+        self.total_pages = total_pages
+        self.total_results = total_results
```

### Comparing `enma-2.3.1/enma/domain/entities/search_result.py` & `enma-2.4.1/enma/domain/entities/search_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
 This module defines the SearchResult entity for the Enma application.
 It represents the result of a manga search operation.
 """
-from dataclasses import dataclass
 from datetime import datetime
 from typing import TypedDict, Union
 from enma.domain.entities.manga import Manga
 from enma.domain.entities.pagination import Pagination, Thumb
 
 class ISearchResultProps(TypedDict):
     id: Union[int, str]
     created_at: datetime
     updated_at: datetime
     page: int
     total_pages: int
     total_results: int
     results: list[Manga]
 
-@dataclass
 class SearchResult(Pagination):
     """
     Entity class representing a search result in the Enma application.
     """
     query: str
 
     def __init__(self,
```

### Comparing `enma-2.3.1/enma/infra/adapters/repositories/manganato.py` & `enma-2.4.1/enma/infra/adapters/repositories/manganato.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
-This module provides an adapter for the nhentai repository.
-It contains functions and classes to interact with the nhentai API and retrieve manga data.
+This module provides an adapter for the MANGANATO repository.
+It contains functions and classes to interact with the MANGANATO API and retrieve manga data.
 """
 
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from multiprocessing import cpu_count
+import os
 from typing import Any, Optional, Union, cast
 from urllib.parse import urlparse, urljoin
 from bs4 import BeautifulSoup, Tag
 
 import requests
 
+from enma._version import __version__
 from enma.application.core.interfaces.manga_repository import IMangaRepository
 from enma.application.core.utils.logger import logger
 from enma.domain.entities.author_page import AuthorPage
 from enma.domain.entities.manga import Author, Chapter, Genre, Image, Manga, SymbolicLink, Title
 from enma.domain.entities.search_result import Pagination, SearchResult, Thumb
+from enma.infra.core.utils.cache import Cache
 
 class Manganato(IMangaRepository):
     """
     Repository class for interacting with the Manganato website.
     Provides methods to fetch manga details, search for manga, etc.
     """
     def __init__(self) -> None:
@@ -34,15 +37,17 @@
 
         headers = headers if headers is not None else {}
         params = params if params is not None else {}
 
         logger.debug(f'Fetching {url} with headers {headers} and params {params}')
 
         return requests.get(url=urlparse(url).geturl(), 
-                            headers={**headers, 'Referer': 'https://chapmanganato.com/'},
+                            headers={**headers, 
+                                     'Referer': 'https://chapmanganato.com/', 
+                                     "User-Agent": f"Enma/{__version__}"},
                             params={**params})
     
     def __create_title(self, 
                        main_title: str, 
                        alternative: str) -> Title:
         logger.debug(f'Building manga title main: {main_title} and alternative: {alternative}')
 
@@ -55,15 +60,15 @@
                          other=main_title.strip())
 
         jp, cn, *_ = alternative.split(';') if alternative.find(';') != -1 else alternative.split(',')
         return Title(english=main_title.strip(),
                      japanese=jp.strip(),
                      other=cn.strip())
     
-    def __find_chapets_list(self, html: BeautifulSoup) -> list[str]:
+    def __find_chapters_list(self, html: BeautifulSoup) -> list[str]:
         chapter_list = cast(Tag, html.find('ul', {'class': 'row-content-chapter'}))
         chapters = chapter_list.find_all('li') if chapter_list else []
         return [chapter.find('a')['href'] for chapter in chapters]
     
     def __create_chapter(self, url: str, symbolic: bool = False) -> Union[Chapter, None]:
 
         if symbolic:
@@ -72,26 +77,30 @@
         response = self.__make_request(url=url)
         logger.debug(f'Fetching chapter {url}')
         
         if response.status_code != 200:
             logger.error(f'Could not fetch the chapter with url: {url}. status code: {response.status_code}')
             return
         
-        
         chapter = Chapter(id=response.url.split('/')[-1])
         html = BeautifulSoup(response.text, 'html.parser')
         images_container = cast(Tag, html.find('div', {'class': 'container-chapter-reader'}))
 
         for img in images_container.find_all('img'):
             chapter.add_page(Image(uri=img['src'],
                                    name=img['src'].split('/')[-1],
                                    width=0,
                                    height=0))
         return chapter
+    
+    def set_config(self, **kwargs) -> None:
+        raise NotImplementedError('Manganato does not support set_config')
 
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_GET_TTL_IN_SECONDS', 300)), 
+           max_size=20).cache
     def get(self, 
             identifier: str,
             with_symbolic_links: bool = False) -> Union[Manga, None]:
         response = self.__make_request(url=urljoin(self.__CHAPTER_BASE_URL, identifier))
         
         if response.status_code != 200:
             logger.error(f'Could not fetch the manga with identifier: {identifier}. status code: {response.status_code}')
@@ -139,35 +148,38 @@
 
         updated_at = None
         if extra_infos:
             updated_at_field = extra_infos.find_all('p')[0]
             updated_at = updated_at_field.find('span', {'class': 'stre-value'}).text
 
         if with_symbolic_links:
-            chapters_links = self.__find_chapets_list(html=soup)
+            chapters_links = self.__find_chapters_list(html=soup)
             chapters = [self.__create_chapter(link, symbolic=True) for link in chapters_links]
         else:
             workers = cpu_count()
             logger.debug(f'Initializing {workers} workers to fetch chapters of {identifier}.')
 
             with ThreadPoolExecutor(max_workers=workers) as executor:
-                chapters = executor.map(self.__create_chapter, self.__find_chapets_list(html=soup))
+                chapters = executor.map(self.__create_chapter, self.__find_chapters_list(html=soup))
                 chapters = list(filter(lambda x: isinstance(x, Chapter), list(chapters)))
                 executor.shutdown()
         
         return Manga(title=title,
                      authors=[Author(name=author)] if author is not None else None,
                      genres=[Genre(name=genre_name) for genre_name in genres],
+                     url=urljoin(self.__BASE_URL, identifier),
                      id=identifier,
                      created_at=datetime.strptime(updated_at, "%b %d,%Y - %H:%M %p") if updated_at else None,
                      updated_at=datetime.strptime(updated_at, "%b %d,%Y - %H:%M %p") if updated_at else None,
                      thumbnail=Image(uri=cover), # type: ignore
                      cover=Image(uri=cover), # type: ignore
                      chapters=chapters) # type: ignore
     
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_SEARCH_TTL_IN_SECONDS', 100)), 
+           max_size=5).cache
     def search(self, 
                query: str,
                page: int) -> SearchResult:
         
         response = self.__make_request(url=urljoin(f'{self.__BASE_URL}/search/story/', "_".join(query.split())),
                                        params={'page': page})
         
@@ -184,22 +196,25 @@
 
         results = soup.find_all('div', {'class': 'search-story-item'})
 
         thumbs: list[Thumb] = []
 
         for result in results:
             thumbs.append(Thumb(title=result.find('h3').text.replace('\n', '').strip(),
+                                url=result.find('a', {'class': 'a-h text-nowrap item-title'})['href'],
                                 cover=Image(uri=result.find('img')['src'], width=0, height=0),
                                 id=result.find('a', {'class': 'a-h text-nowrap item-title'})['href'].split('/')[-1]))
 
         return SearchResult(query=query,
                             page=page,
                             total_pages=total_pages,
                             results=thumbs)
 
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_PAGINATE_TTL_IN_SECONDS', 100)), 
+           max_size=5).cache
     def paginate(self, page: int) -> Pagination:
         response = self.__make_request(url=f'{self.__BASE_URL}/genre-all/{page}')
         
         pagination = Pagination(page=page)
 
         if response.status_code != 200:
             return pagination
@@ -215,32 +230,32 @@
         content_items = content_panel.find_all('div', {'class': 'content-genres-item'})
         
         for item in content_items:
             item = cast(Tag, item)
             info = cast(Tag, item.find('a', {'class': 'genres-item-img bookmark_check'}))
             cover = info.find('img')
             pagination.results.append(Thumb(id=info['href'].split('/')[-1], # type: ignore
+                                            url=info['href'],
                                             title=info['title'] if info is not None else "",
                                             cover=Image(uri=cover['src'], width=0, height=0))) # type: ignore
             
         last_pagination = soup.find('a', {'class': 'page-blue page-last'})
         pagination.total_pages = int(last_pagination['href'].split('/')[-1]) # type: ignore
         pagination.total_results = 24 * int(pagination.total_pages)
         
         return pagination
     
     def random(self) -> Manga:
         raise NotImplementedError('Manganato does not support random')
     
-    def set_config(self, **kwargs) -> None:
-        raise NotImplementedError('Manganato does not support set_config')
-    
     def author_page(self, author: str, page: int) -> AuthorPage:
         raise NotImplementedError('Manganato does not support author_page')
     
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS', 100)), 
+           max_size=20).cache
     def fetch_chapter_by_symbolic_link(self, link: SymbolicLink) -> Chapter:
         chapter =  self.__create_chapter(url=link.link)
         
         if chapter is not None:
             return chapter
         
         return Chapter(id=0)
```

### Comparing `enma-2.3.1/enma/infra/adapters/repositories/nhentai.py` & `enma-2.4.1/enma/infra/adapters/repositories/nhentai.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
 This module provides an adapter for the nhentai repository.
 It contains functions and classes to interact with the nhentai API and retrieve manga data.
 """
 from datetime import datetime, timezone
 from enum import Enum
+import os
 from typing import Any, Literal, Optional, Union, cast
 from urllib.parse import urljoin, urlparse
 from pydantic import BaseModel, field_validator
 
 import requests
 from bs4 import BeautifulSoup, Tag
 
-from enma.application.core.handlers.error import (ExceedRetryCount, InvalidConfig, InvalidRequest,
-                                                  NhentaiSourceWithoutConfig)
+from enma.application.core.handlers.error import (ExceedRetryCount, Forbidden, InvalidConfig, InvalidRequest,
+                                                  NhentaiSourceWithoutConfig, NotFound, Unknown)
 from enma.application.core.interfaces.manga_repository import IMangaRepository
 from enma.application.core.utils.logger import logger
 from enma.domain.entities.author_page import AuthorPage
 from enma.domain.entities.manga import (MIME, Chapter, Genre, Author, Image, Manga, SymbolicLink,
                                         Title)
 from enma.domain.entities.search_result import Pagination, SearchResult, Thumb
 from enma.infra.core.interfaces.nhentai_response import NHentaiImage, NHentaiResponse
+from enma.infra.core.utils.cache import Cache
 
 
 class CloudFlareConfig(BaseModel):
     user_agent: str
     cf_clearance: str
 
     @field_validator('user_agent')
@@ -48,49 +50,57 @@
     """
     Repository class for interacting with the nhentai API.
     Provides methods to fetch manga details, search for manga, etc.
     """
     def __init__(self,
                  config: Optional[CloudFlareConfig] = None) -> None:
         self.__config = config
-        self.__BASE_URL = 'https://nhentai.net'
+        self.__BASE_URL = 'https://nhentai.net/'
         self.__API_URL = 'https://nhentai.net/api/'
         self.__IMAGE_BASE_URL = 'https://i.nhentai.net/galleries/'
         self.__AVATAR_URL = 'https://i5.nhentai.net/'
         self.__TINY_IMAGE_BASE_URL = self.__IMAGE_BASE_URL.replace('/i.', '/t.')
 
+    def __handle_source_response(self, response: requests.Response):
+        logger.debug(f'Fetched {response.url} with response status code {response.status_code} and text {response.text}')
+        if response.status_code == 200: return
+        if response.status_code == 403: 
+            raise Forbidden(message='Could not perform a successfull request to the source due credentials issues. \
+Check your credentials and try again.')
+        if response.status_code == 404:
+            raise NotFound(message=f'Could not find the requested resource at "{response.url}". \
+Check the provided request parameters and try again.')
+        raise Unknown(message='Something unexpected happened while trying to fetch source content. \
+Set the logging mode to debug and try again.')
+
     def __make_request(self,
                        url: str,
                        headers: Union[dict[str, Any], None] = None,
                        params: Optional[dict[str, Union[str, int]]] = None):
 
         if self.__config is None:
             raise NhentaiSourceWithoutConfig('Please provide a valid cloudflare cookie and user-agent.')
 
         headers = headers if headers is not None else {}
         params = params if params is not None else {}
 
         logger.debug(f'Fetching {url} with headers {headers} and params {params} the current config cf_clearance: {self.__config.cf_clearance}')
 
         response = requests.get(url=urlparse(url).geturl(),
-                                headers={**headers, 'User-Agent': self.__config.user_agent},
+                                headers={**headers, 'User-Agent': f'{self.__config.user_agent}'},
                                 params={**params},
                                 cookies={'cf_clearance': self.__config.cf_clearance})
         
-        logger.debug(f'Fetched {url} with response status code {response.status_code} and text {response.text}')
+        self.__handle_source_response(response)
 
         return response
 
     def set_config(self, config: CloudFlareConfig) -> None:
         if not isinstance(config, CloudFlareConfig): raise InvalidConfig(message='You must provide a CloudFlareConfig object.') 
         self.__config = config
-
-    def __handle_request_error(self, msg: str) -> None:
-        logger.error(msg)
-        return None
     
     def __make_page_uri(self,
                         type: Union[Literal['cover'], Literal['page'], Literal['thumbnail']],
                         media_id: str,
                         mime: MIME,
                         page_number: Optional[int] = None) -> str:
         
@@ -104,21 +114,19 @@
         else:
             url = urljoin(self.__IMAGE_BASE_URL, f'{media_id}/{page_number}.{mime.value}')
         
         logger.debug(f'Built page uri for type {type} as {url}')
 
         return url
     
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS', 100)), 
+           max_size=20).cache
     def fetch_chapter_by_symbolic_link(self, 
                                        link: SymbolicLink) -> Chapter:
         response = self.__make_request(url=link.link)
-
-        if response.status_code != 200:
-            self.__handle_request_error(msg=f'Could not fetch {link.link} because nhentai\'s request ends up with {response.status_code} status code.')
-            return Chapter()
         
         doujin: NHentaiResponse = response.json()
 
         if doujin.get('media_id') is None or doujin.get('images') is None:
             return Chapter()
 
         return self.__create_chapter(url=link.link, 
@@ -144,24 +152,23 @@
                                                                 page_number=index+1),
                                 name=f'{index}.{mime.value}',
                                 mime=mime,
                                 width=page.get('w'),
                                 height=page.get('h')))
             return chapter
     
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_GET_TTL_IN_SECONDS', 300)), 
+           max_size=20).cache
     def get(self, 
             identifier: str,
             with_symbolic_links: bool = False) -> Union[Manga, None]:
 
-        url = f'{self.__API_URL}/gallery/{identifier}'
+        url = urljoin(self.__API_URL, f'gallery/{identifier}')
         response = self.__make_request(url=url)
 
-        if response.status_code != 200:
-            return self.__handle_request_error(msg=f'Could not fetch {identifier} because nhentai\'s request ends up with {response.status_code} status code.')
-
         doujin: NHentaiResponse = response.json()
         media_id = doujin.get('media_id')
 
         chapter = self.__create_chapter(url=url,
                                         with_symbolic_links=with_symbolic_links,
                                         media_id=media_id, 
                                         pages=doujin.get('images').get('pages'))
@@ -190,23 +197,26 @@
 
         manga = Manga(title=Title(english=doujin.get('title').get('english'),
                                   japanese=doujin.get('title').get('japanese'),
                                   other=doujin.get('title').get('pretty')),
                       id=doujin.get('id'),
                       created_at=datetime.fromtimestamp(doujin.get('upload_date'), tz=timezone.utc),
                       updated_at=datetime.fromtimestamp(doujin.get('upload_date'), tz=timezone.utc),
+                      url=urljoin(self.__BASE_URL, f'g/{doujin.get("id")}'),
                       language=language[0] if len(language) > 0 else None,
                       authors=authors,
                       genres=genres,
                       thumbnail=thumbnail,
                       cover=cover,
                       chapters=[chapter])
 
         return manga
-
+    
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_SEARCH_TTL_IN_SECONDS', 100)), 
+           max_size=5).cache
     def search(self,
                query: str,
                page: int,
                sort: Sort = Sort.RECENT) -> SearchResult:
         
         logger.debug(f'Searching into Nhentai with args query={query};page={page};sort={sort}')
 
@@ -217,18 +227,14 @@
         
         search_result = SearchResult(query=query,
                                      total_pages=0,
                                      page=page,
                                      total_results=0,
                                      results=[])
         
-        if request_response.status_code != 200:
-            self.__handle_request_error(f'Could not search by {query} because nhentai\'s request ends up with {request_response.status_code} status code.')
-            return search_result
-
         soup = BeautifulSoup(request_response.text, 'html.parser')
 
         search_results_container = soup.find('div', {'class': 'container'})
         logger.debug(f'Found successfully search result container using .class.container.')
         pagination_container = soup.find('section', {'class': 'pagination'})
         logger.debug(f'Found successfully pagination container using .class.pagination.')
 
@@ -270,58 +276,55 @@
             result_caption = a_tag.find('div', {'class': 'caption'})
 
             caption = None
             if result_caption is not None:
                 caption = result_caption.text
 
             thumbs.append(Thumb(id=doujin_id,
+                                url=urljoin(self.__BASE_URL, f'g/{doujin_id}'),
                                 cover=Image(uri=cover_uri or '',
                                             mime=MIME.J,
                                             width=int(width or 0),
                                             height=int(height or 0)),
                                 title=caption or ''))
 
         search_result.total_pages = total_pages
         search_result.total_results = 25 * total_pages if pagination_container else len(thumbs)
         search_result.results = thumbs
 
         return search_result
 
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_PAGINATE_TTL_IN_SECONDS', 100)), 
+           max_size=5).cache
     def paginate(self, page: int) -> Pagination:
         response = self.__make_request(url=urljoin(self.__API_URL, f'galleries/all'),
                                        params={'page': page})
 
-        if response.status_code != 200:
-            self.__handle_request_error(f'Could not paginate to page {page} because nhentai\'s request ends up with {response.status_code} status code.')
-            return Pagination(page=page)
-
         data = response.json()
 
         PAGES = data.get('num_pages', 0)
         PER_PAGE = data.get('per_page', 0)
         TOTAL_RESULTS = int(PAGES) * int(PER_PAGE)
 
         return Pagination(page=int(page),
                           total_results=TOTAL_RESULTS,
                           total_pages=PAGES,
                           results=[Thumb(id=result.get('id'),
                                          title=result.get('title').get('english'),
+                                         url=urljoin(self.__BASE_URL, f'g/{result.get("id")}'),
                                          cover=Image(uri=self.__make_page_uri(type='cover',
                                                                               media_id=result.get('media_id'),
                                                                               mime=MIME[result.get('images').get('cover').get('t').upper()]),
                                                      mime=MIME[result.get("images").get("thumbnail").get("t").upper()],
                                                      width=result.get('images').get('cover').get('w'),
                                                      height=result.get('images').get('cover').get('h'))) for result in data.get('result')])
 
     def random(self, retry=0) -> Manga:
         response = self.__make_request(url=urljoin(self.__BASE_URL, 'random'))
 
-        if response.status_code != 200:
-            self.__handle_request_error(f'Could not fetch a random manga because nhentai\'s request ends up with {response.status_code} status code.')
-
         soup = BeautifulSoup(response.text, 'html.parser')
 
         id = cast(Tag, soup.find('h3', id='gallery_id')).text.replace('#', '')
         logger.debug(f'Got successfully random manga id {id} from "gallery_id.h3" tag.')
         logger.debug(f'Using get method to Fetch manga with identifier: {id}')
         doujin = self.get(identifier=id)
         logger.debug(f'Got successfully random manga with id {id}.')
@@ -331,29 +334,27 @@
                 raise ExceedRetryCount('Could not fetch a random doujin after 4 retries.')
             
             logger.warning('Could not fetch random manga. Retrying.')
             return self.random(retry=retry+1)
 
         return doujin
     
+    @Cache(max_age_seconds=int(os.getenv('ENMA_CACHING_AUTHOR_TTL_IN_SECONDS', 100)), 
+           max_size=5).cache
     def author_page(self,
                     author: str,
                     page: int) -> AuthorPage:
         request_response = self.__make_request(url=urljoin(self.__BASE_URL, f'artist/{author}'),
                                                params={'page': page})
         
         result = AuthorPage(author=author,
                             total_pages=0,
                             page=page,
                             total_results=0,
-                            results=[])
-        
-        if request_response.status_code != 200:
-            logger.error('Could not fetch author page properly')
-            return result    
+                            results=[]) 
    
         soup = BeautifulSoup(request_response.text, 'html.parser')
 
         search_results_container = soup.find('div', {'class': 'container'})
         pagination_container = soup.find('section', {'class': 'pagination'})
 
         last_page_a_tag = pagination_container.find('a',
@@ -392,14 +393,15 @@
             result_caption = a_tag.find('div', {'class': 'caption'})
 
             caption = None
             if result_caption is not None:
                 caption = result_caption.text
 
             thumbs.append(Thumb(id=doujin_id,
+                                url=urljoin(self.__BASE_URL, f'g/{doujin_id}'),
                                 cover=Image(uri=cover_uri or '',
                                             mime=MIME.J,
                                             width=int(width or 0),
                                             height=int(height or 0)),
                                 title=caption or ''))
         
         result.author = author
```

### Comparing `enma-2.3.1/enma/infra/core/interfaces/lib.py` & `enma-2.4.1/enma/infra/core/interfaces/lib.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma/infra/core/interfaces/nhentai_response.py` & `enma-2.4.1/enma/infra/core/interfaces/nhentai_response.py`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/enma.egg-info/PKG-INFO` & `enma-2.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: enma
-Version: 2.3.1
-Summary: Enma is a Python library designed to fetch manga and doujinshi data from many sources.
-Home-page: https://github.com/AlexandreSenpai/Enma
-Author: AlexandreSenpai
-Author-email: alexandrebsramos@hotmail.com
-License: LICENSE
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: requests==2.31.0
-Requires-Dist: beautifulsoup4==4.10.0
-Requires-Dist: pydantic==2.5.3
-
 <p align="center">
     <img src="./docs/images/enma.png" align="center" width="50%">
 </p>
 
 <center>
 
 [![PyPI download month](https://img.shields.io/pypi/dm/Enma.svg)](https://pypi.python.org/pypi/Enma/)
@@ -31,14 +14,17 @@
 
 </center>
 
 # Enma
 
 Enma is a Python library designed to fetch manga and doujinshi data from many sources. It provides a unified interface to interact with different manga repositories, making it easier to retrieve manga details, search for manga, paginate through results, and fetch random manga.
 
+## :warning: Warning
+> **:exclamation: Important: Enma is not intended for mass querying or placing heavy loads on supported sources. Please use responsibly, adhering to the terms of service of the data sources. Misuse may result in service disruption or access denial.**
+
 ## Requirements
 
 - Python 3.9+
 
 ## Installation
 ```py
 pip install --upgrade enma
@@ -59,23 +45,24 @@
 ```
 
 ## Documentation
 You can consult full Enma documentation at <strong><a href="https://enma.gitbook.io/enma" target="_blank">https://enma.gitbook.io/enma</a></strong>.
 
 ## Features Comparison
 
-Feature    | NHentai | Manganato
------------|---------|-----------
-search     |    ✅   |     ✅    
-random     |    ✅   |     🚫    
-get        |    ✅   |     ✅    
-paginate   |    ✅   |     ✅
-download   |    ✅   |     ✅       
-author_page|    ✅   |     🚫       
-set_config |    ✅   |     🚫
+Feature    | NHentai | Manganato | Mangadex
+-----------|---------|-----------|-----------
+search     |    ✅   |     ✅   |   ✅
+random     |    ✅   |     🚫   |   ✅  
+get        |    ✅   |     ✅   |   ✅
+paginate   |    ✅   |     ✅   |   ✅
+download   |    ✅   |     ✅   |   ✅  
+author_page|    ✅   |     🚫   |   🚫   
+set_config |    ✅   |     🚫   |   🚫
+caching    |    ✅   |     ✅   |   ✅
 
 ## Usage
 
 ### Example 1: Using Default Available Sources
 
 ```py
 from typing import cast
@@ -111,14 +98,48 @@
 enma.source_manager.add_source(source_name='new-source', source=Manganato()) # Source MUST be an instance of IMangaRepository
 enma.source_manager.set_source(source_name=AvailableSources.MANGANATO)
 
 manga = enma.random()
 print(manga)
 ```
 
+## Caching
+Caching is a key feature in Enma that improves your application's efficiency by storing the results of data requests. This means when the same data is requested again, Enma can quickly retrieve it from the cache instead of repeatedly calling the external source. This results in faster response times and less strain on both your application and the external APIs.
+
+### How Caching Benefits You
+- **Speed**: Retrieving data from the cache is faster than making a new request to a manga repository.
+- **Efficiency**: Reduces the number of network requests, which is especially useful when dealing with rate-limited APIs.
+- **Reliability**: Provides more consistent application performance even with varying network conditions.
+
+### Customizing Cache Settings
+While Enma provides default caching settings that suit most needs, you may want to customize these settings based on your specific requirements, like how often you expect data to change or specific API rate limits.
+
+#### Adjusting Cache Duration via Environment Variables
+You can control how long data is kept in the cache by setting environment variables. This allows you to fine-tune the balance between data freshness and retrieval speed without modifying the core library code.
+
+For example, to change the cache expiration for fetching chapters, you can set the `ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS` environment variable:
+
+```sh
+# Sets the cache duration to 30 minutes
+export ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS=1800
+```
+
+This customization capability ensures that you can adapt the caching behavior to best fit your application's performance and efficiency needs.
+
+By leveraging caching, Enma helps make your manga-related applications faster and more reliable, all while giving you the flexibility to tailor caching behavior as needed.
+
+#### Available Caching TTL Settings
+| KEY                                            | DEFAULT |
+|------------------------------------------------|---------|
+| ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS| 100     |
+| ENMA_CACHING_PAGINATE_TTL_IN_SECONDS           | 100     |
+| ENMA_CACHING_SEARCH_TTL_IN_SECONDS             | 100     |
+| ENMA_CACHING_GET_TTL_IN_SECONDS                | 300     |
+| ENMA_CACHING_AUTHOR_TTL_IN_SECONDS             | 100     |
+
 ## Downloading Chapters
 Using Enma you're able to download chapter pages to your local storage or any other storage that implements `ISaverAdapter`.
 
 You can check it out how to do it right below:
 
 ```py
 from enma import (Enma,
@@ -159,31 +180,14 @@
 from enma import Enma
 
 enma = Enma()
 
 enma.source_manager.set_source('manganato')
 doujin = enma.get(identifier='manga-kb951984', with_symbolic_links=True)
 
-# Manga(id='manga-kb951984', 
-#       created_at=datetime.datetime(2024, 1, 22, 10, 5), 
-#       updated_at=datetime.datetime(2024, 1, 22, 10, 5), 
-#       title=Title(english='Monster Musume No Iru Nichijou', 
-#                   japanese='モンスター娘のいる日常', 
-#                   other='魔物娘的同居日常'), 
-#       language=None, 
-#       cover=Image(uri='https://avt.mkklcdnv6temp.com/23/p/1-1583464626.jpg', name='image.jpg', width=0, height=0, mime=<MIME.J: 'jpg'>), 
-#       thumbnail=Image(uri='https://avt.mkklcdnv6temp.com/23/p/1-1583464626.jpg', name='image.jpg', width=0, height=0, mime=<MIME.J: 'jpg'>), 
-#       authors=[Author(name='Okayado', id=0)], 
-#       genres=[Genre(name='Comedy', id=0), 
-#               Genre(name='Fantasy', id=0), 
-#               Genre(name='Harem', id=0)], 
-#       chapters=[Chapter(id='chapter-84', pages=[], pages_count=0, link=SymbolicLink(link='https://chapmanganato.to/manga-kb951984/chapter-84')), 
-#                 Chapter(id='chapter-83', pages=[], pages_count=0, link=SymbolicLink(link='https://chapmanganato.to/manga-kb951984/chapter-83'))], 
-#       chapters_count=95)
-
 if doujin is not None:
     chapter_ref = doujin.chapters[0]
     chapter = enma.fetch_chapter_by_symbolic_link(link=chapter_ref.link)
 
 ```
 
 ## Retrieving `user-agent` and `cf_clearance` for NHentai
@@ -241,14 +245,31 @@
     - **Description**: Raised when trying to perform an action with an invalid or inexistent resource.
     - **Common Cause**: Providing an inexistent folder path to downloader.
 
 7. **InvalidRequest**:
     - **Description**: Raised when trying to perform an action with an invalid data type.
     - **Common Cause**: Making an action with wrong parameter data type.
 
+7. **Unknown**:
+    - **Description**: Raised when was not possible to determine the error root cause.
+    - **Common Cause**: Not properly handled error.
+
+7. **NotFound**:
+    - **Description**: Raised when was not possible to find the requested resource..
+    - **Common Cause**: Fetching an inexistent resource.
+
+7. **Forbidden**:
+    - **Description**: Raised when trying to perform a request to the source without right credentials.
+    - **Common Cause**: Making a request with no or invalid credentials.
+
+7. **ExceedRateLimit**:
+    - **Description**: Raised when trying to perform more requests than a server can handle.
+    - **Common Cause**: Looping through many pages without cooling down.
+
+
 When encountering one of these errors, refer to the description and common cause to assist in troubleshooting.
 
 ## Future Plans
 
 We are actively working on introducing an asynchronous version of the Enma library to better cater to applications that require non-blocking operations. This version will be maintained in a separate repository to keep the core library lightweight. However, for ease of access and installation, you'll be able to install the asynchronous version directly using:
 
 ```bash
@@ -272,10 +293,22 @@
 
 1. Fork the repository.
 2. Make your changes.
 3. Submit a pull request.
 
 Ensure you follow the coding standards and write tests for new features.
 
+## Disclaimer
+
+This software is provided "as is", without warranty of any kind, express or implied. The developers and contributors of the Enma library shall not be liable for any misuse, damages, or other consequences arising from the use of this software.
+
+It is important to emphasize that the Enma library was developed with the goal of facilitating efficient and responsible access and manipulation of data. We do not encourage or support the use of this tool for conducting mass queries or accesses that could overload, harm, or in any way negatively affect the servers or services of the supported sources.
+
+Users of the Enma library must always follow the guidelines, terms of use, and limitations imposed by the accessed data sources. We strongly recommend the implementation of responsible rate limiting practices and obtaining appropriate permissions when necessary, to ensure that the use of the library complies with all applicable laws and regulations, in addition to respecting ethical principles of data use.
+
+By using the Enma library, you agree to use the tool in an ethical and responsible manner, acknowledging that the developers of Enma will not be responsible for any use that violates these guidelines.
+
+We remind you that respect for the services and APIs of the supported sources is fundamental for the sustainability and longevity of both the Enma and the services used. We value the community and the development ecosystem and encourage all users to contribute to a safer, more respectful, and collaborative digital environment.
+
 ## License
 
 MIT
```

### Comparing `enma-2.3.1/enma.egg-info/SOURCES.txt` & `enma-2.4.1/enma.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 .gitignore
-.python-version
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/dev-pypi.yml
 .github/workflows/pypi.yml
 .github/workflows/testing.yml
+.vscode/launch.json
 .vscode/settings.json
 docs/images/enma.png
 docs/images/user-agent.png
 enma/__init__.py
 enma/_version.py
 enma.egg-info/PKG-INFO
 enma.egg-info/SOURCES.txt
@@ -34,25 +34,34 @@
 enma/domain/entities/author_page.py
 enma/domain/entities/base.py
 enma/domain/entities/manga.py
 enma/domain/entities/pagination.py
 enma/domain/entities/search_result.py
 enma/infra/adapters/downloaders/default.py
 enma/infra/adapters/downloaders/manganato.py
+enma/infra/adapters/repositories/mangadex.py
 enma/infra/adapters/repositories/manganato.py
 enma/infra/adapters/repositories/nhentai.py
 enma/infra/adapters/storage/local.py
 enma/infra/core/interfaces/lib.py
+enma/infra/core/interfaces/mangadex_response.py
 enma/infra/core/interfaces/nhentai_response.py
+enma/infra/core/utils/cache.py
 enma/infra/entrypoints/lib/__init__.py
+tests/test_cache.py
+tests/test_mangadex_source.py
 tests/test_manganato_source.py
 tests/test_nhentai_fetch_chapter_by_symbolic_link.py
 tests/test_nhentai_get_manga_use_case.py
 tests/test_nhentai_source.py
+tests/test_search_result_entity.py
+tests/test_source_manager.py
 tests/data/get.json
+tests/data/mangadex_empty_chapters.json
+tests/data/mangadex_empty_pagination_mock.json
 tests/data/manganato_manga_page_empty_chapters_mock.txt
 tests/data/manganato_manga_page_empty_pagination_mock.txt
 tests/data/mocked_doujins.py
 tests/data/nhentai_author_page_mock.txt
 tests/data/nhentai_author_page_not_found_mock.txt
 tests/data/nhentai_paginate_mock.json
 tests/data/nhentai_search_mock.txt
```

### Comparing `enma-2.3.1/setup.cfg` & `enma-2.4.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,27 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.9
 install_requires = 
 	requests==2.31.0
 	beautifulsoup4==4.10.0
 	pydantic==2.5.3
+	expiringdict==1.2.2
 setup_requires = 
 	setuptools_scm
 
 [options.package_data]
 enma = *.txt, *.rst, *.md
 
 [tool.setuptools_scm]
 write_to = enma/_version.py
 
+[coverage:run]
+omit = 
+	*/interfaces/*
+	*/tests/*
+	enma/__init__.py
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `enma-2.3.1/tests/data/get.json` & `enma-2.4.1/tests/data/get.json`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/tests/data/manganato_manga_page_empty_chapters_mock.txt` & `enma-2.4.1/tests/data/manganato_manga_page_empty_chapters_mock.txt`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/tests/data/manganato_manga_page_empty_pagination_mock.txt` & `enma-2.4.1/tests/data/manganato_manga_page_empty_pagination_mock.txt`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/tests/data/nhentai_author_page_mock.txt` & `enma-2.4.1/tests/data/nhentai_author_page_mock.txt`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/tests/data/nhentai_author_page_not_found_mock.txt` & `enma-2.4.1/tests/data/nhentai_author_page_not_found_mock.txt`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/tests/data/nhentai_paginate_mock.json` & `enma-2.4.1/tests/data/nhentai_paginate_mock.json`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/tests/data/nhentai_search_mock.txt` & `enma-2.4.1/tests/data/nhentai_search_mock.txt`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/tests/data/nhentai_search_no_result.txt` & `enma-2.4.1/tests/data/nhentai_search_no_result.txt`

 * *Files identical despite different names*

### Comparing `enma-2.3.1/tests/test_manganato_source.py` & `enma-2.4.1/tests/test_manganato_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 from unittest.mock import MagicMock, Mock, patch
 import sys
 import os
 
 import pytest
 
+os.environ['ENMA_CACHING_PAGINATE_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_SEARCH_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_GET_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS'] = '0'
+
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 
 from enma.domain.entities.pagination import Thumb
 from enma.infra.adapters.repositories.manganato import Manganato
 from enma.domain.entities.manga import MIME, Author, Chapter, Genre, Image, SymbolicLink
 from tests.data.mocked_doujins import manganato_manga_page_empty_chapters_mocked, manganato_manga_page_empty_pagination_mocked
+from enma._version import __version__
 
 class TestManganatoSourceGetMethod:
 
     sut = Manganato()
 
     def test_success_doujin_retrieve(self):
 
         res = self.sut.get(identifier='manga-kb951984', with_symbolic_links=True)
 
         assert res is not None
         assert res.id == 'manga-kb951984'
         assert res.title.english == "Monster Musume No Iru Nichijou"
         assert res.title.japanese == "モンスター娘のいる日常"
         assert res.title.other == "魔物娘的同居日常"
+        assert res.url != ''
         
         for genre in res.genres:
             assert isinstance(genre, Genre)
         
         for author in res.authors:
             assert isinstance(author, Author)
 
@@ -49,15 +56,16 @@
             mock.status_code = 403
             mock_method.return_value = mock
 
             doujin = self.sut.get(identifier='manga-kb951984')
 
             assert doujin is None
             mock_method.assert_called_with(url='https://chapmanganato.com/manga-kb951984', 
-                                           headers={'Referer': 'https://chapmanganato.com/'}, 
+                                           headers={'Referer': 'https://chapmanganato.com/',
+                                                    'User-Agent': f'Enma/{__version__}'}, 
                                            params={})
     
     @patch('requests.get')
     def test_return_empty_chapters(self, mock_method: MagicMock):
         mock = Mock()
         mock.status_code = 200
         mock.text = manganato_manga_page_empty_chapters_mocked
@@ -94,15 +102,15 @@
 class TestManganatoSourcePaginationMethod:
     sut = Manganato()
 
     def test_success_searching(self):
         res = self.sut.paginate(page=2)
 
         assert res is not None
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 2
         assert res.total_pages > 0
         assert res.total_results > 0
         assert len(res.results) == 24
         
     @patch('requests.get')
     def test_must_return_empty_search_result(self, mock_method: MagicMock):
@@ -112,46 +120,46 @@
         mock.text = manganato_manga_page_empty_pagination_mocked
 
         mock_method.return_value = mock
         
         res = self.sut.paginate(page=2)
 
         assert res is not None
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 2
         assert res.total_pages > 0
         assert res.total_results > 0
         assert len(res.results) == 0
 
     @patch('requests.get')
     def test_response_when_forbidden(self, mock_method: MagicMock):
         mock = Mock()
         mock.status_code = 403
         mock_method.return_value = mock
         
         res = self.sut.paginate(page=2)
         
         assert res is not None
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 2
-        assert res.total_pages == 1
+        assert res.total_pages == 0
         assert res.total_results == 0
         assert len(res.results) == 0
 
 class TestManganatoSourceSearchMethod:
 
     sut = Manganato()
 
     def test_success_searching(self):
 
         res = self.sut.search(query='GATE', page=1)
 
         assert res is not None
         assert res.query == 'GATE'
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 1
         assert res.total_pages == 4
         assert len(res.results) == 20
 
         for result in res.results:
             assert isinstance(result, Thumb)
             assert result.cover is not None
@@ -169,11 +177,11 @@
         mock.status_code = 403
         mock_method.return_value = mock
 
         search = self.sut.search(query='Monster Musume no Iru Nichijou', page=1)
         
         assert search is not None
         assert search.query == 'Monster Musume no Iru Nichijou'
-        assert search.id == 0
+        assert search.id is not None
         assert search.page == 1
-        assert search.total_pages == 1
+        assert search.total_pages == 0
         assert len(search.results) == 0
```

### Comparing `enma-2.3.1/tests/test_nhentai_fetch_chapter_by_symbolic_link.py` & `enma-2.4.1/tests/test_nhentai_fetch_chapter_by_symbolic_link.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,30 +2,38 @@
 import json
 from unittest.mock import Mock, patch
 import sys
 import os
 
 import pytest
 
+os.environ['ENMA_CACHING_PAGINATE_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_SEARCH_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_GET_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_AUTHOR_TTL_IN_SECONDS'] = '0'
+
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 
+from enma.application.core.handlers.error import NotFound
 from enma.application.use_cases.fetch_chapter_by_symbolic_link import FetchChapterBySymbolicLinkRequestDTO, FetchChapterBySymbolicLinkUseCase
 from enma.application.core.interfaces.use_case import DTO
 from enma.infra.adapters.repositories.nhentai import CloudFlareConfig, NHentai
 from enma.domain.entities.manga import MIME, Author, Chapter, Genre, Image, Manga, SymbolicLink, Title
 
 class TestFetchChapterWithSymbolicLink:
 
     nhentai = NHentai(config=CloudFlareConfig(user_agent='mocked',
                                               cf_clearance='mocked'))
     sut = FetchChapterBySymbolicLinkUseCase(manga_repository=nhentai)
 
     mocked_manga = Manga(title=Title(english="[Hikoushiki (CowBow)] Marine Senchou no Yopparai Archive | Marine's Drunken Archives (Houshou Marine) [English] [Watson] [Digital]",
                                      japanese='[飛行式 (矼房)] マリン船長の酔っぱっぱアーカイブ (宝鐘マリン) [英訳] [DL版]',
                                      other="Marine Senchou no Yopparai Archive | Marine's Drunken Archives"),
+                         url="mocked",
                          id=489504,
                          created_at=datetime.datetime(2024, 1, 7, 0, 3, 25, tzinfo=datetime.timezone.utc),
                          updated_at=datetime.datetime(2024, 1, 7, 0, 3, 25, tzinfo=datetime.timezone.utc),
                          authors=[Author(name='cowbow')],
                          genres=[Genre(name='sweating', id=1590)],
                          thumbnail=Image(uri='https://i.nhentai.net/galleries/2786266/22.jpg', name='21.jpg', width=1280, height=1808, mime=MIME.J),
                          cover=Image(uri='https://i.nhentai.net/galleries/2786266/22.jpg', name='21.jpg', width=1280, height=1808, mime=MIME.J),
@@ -47,30 +55,26 @@
             response = self.sut.execute(dto=DTO(data=FetchChapterBySymbolicLinkRequestDTO(link=link)))
 
             assert isinstance(response.chapter, Chapter)
             assert response.chapter.pages_count == 14
             assert response.chapter.id == 0
             assert len(response.chapter.pages) == 14
 
-    def test_should_return_empty_chapter_for_broken_link(self):
+    def test_should_raise_exception_for_broken_link(self):
         with patch('requests.get') as mock_method:
             mock = Mock()
             mock.status_code = 404
             mock.json.return_value = {}
             mock_method.return_value = mock
 
             link = SymbolicLink(link='https://nhentai.net')
-            response = self.sut.execute(dto=DTO(data=FetchChapterBySymbolicLinkRequestDTO(link=link)))
             
-            assert isinstance(response.chapter, Chapter)
-            assert response.chapter.link is None
-            assert response.chapter.pages_count == 0
-            assert response.chapter.id == 0
-            assert len(response.chapter.pages) == 0
-
+            with pytest.raises(NotFound):
+                self.sut.execute(dto=DTO(data=FetchChapterBySymbolicLinkRequestDTO(link=link)))
+        
     def test_should_return_empty_chapter_for_broken_response(self):
         with patch('requests.get') as mock_method:
             mock = Mock()
             mock.status_code = 200
             mock.json.return_value = {}
             mock_method.return_value = mock
```

### Comparing `enma-2.3.1/tests/test_nhentai_get_manga_use_case.py` & `enma-2.4.1/tests/test_nhentai_get_manga_use_case.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 from unittest.mock import MagicMock, Mock, patch
 import sys
 import os
 
 import pytest
 from pydantic import ValidationError
 
+os.environ['ENMA_CACHING_PAGINATE_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_SEARCH_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_GET_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_AUTHOR_TTL_IN_SECONDS'] = '0'
+
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 
-from enma.application.core.handlers.error import InvalidRequest
+from enma.application.core.handlers.error import Forbidden, NotFound
 from enma.infra.core.interfaces.nhentai_response import NHentaiResponse
 from enma.application.use_cases.get_manga import GetMangaRequestDTO, GetMangaUseCase
 from enma.application.core.interfaces.use_case import DTO
 from enma.infra.adapters.repositories.nhentai import CloudFlareConfig, NHentai
 from enma.domain.entities.manga import MIME, Author, Chapter, Genre, Image, Manga, Title
 
 class TestNHentaiGetDoujin:
@@ -21,14 +27,15 @@
     nhentai = NHentai(config=CloudFlareConfig(user_agent='mocked',
                                               cf_clearance='mocked'))
     sut = GetMangaUseCase(manga_repository=nhentai)
 
     mocked_manga = Manga(title=Title(english="[Hikoushiki (CowBow)] Marine Senchou no Yopparai Archive | Marine's Drunken Archives (Houshou Marine) [English] [Watson] [Digital]",
                                      japanese='[飛行式 (矼房)] マリン船長の酔っぱっぱアーカイブ (宝鐘マリン) [英訳] [DL版]',
                                      other="Marine Senchou no Yopparai Archive | Marine's Drunken Archives"),
+                         url='mocked',
                          id=489504,
                          created_at=datetime.datetime(2024, 1, 7, 0, 3, 25, tzinfo=datetime.timezone.utc),
                          updated_at=datetime.datetime(2024, 1, 7, 0, 3, 25, tzinfo=datetime.timezone.utc),
                          authors=[Author(name='cowbow')],
                          genres=[Genre(name='sweating', id=1590)],
                          thumbnail=Image(uri='https://i.nhentai.net/galleries/2786266/22.jpg', name='21.jpg', width=1280, height=1808, mime=MIME.J),
                          cover=Image(uri='https://i.nhentai.net/galleries/2786266/22.jpg', name='21.jpg', width=1280, height=1808, mime=MIME.J),
@@ -65,16 +72,16 @@
         with patch('requests.get') as mock_method:
             mock = Mock()
             mock.status_code = 200
             
             with open('./tests/data/get.json', 'r') as get:
                 data: NHentaiResponse = json.loads(get.read())
                 
-                data['title']['japanese'] = None
-                data['title']['pretty'] = None
+                data['title']['japanese'] = None # type: ignore
+                data['title']['pretty'] = None # type: ignore
 
                 mock.json.return_value = data
             
             mock_method.return_value = mock
             
             res = self.sut.execute(dto=DTO(data=GetMangaRequestDTO(identifier='489504')))
 
@@ -82,35 +89,31 @@
             assert res.manga is not None
             assert res.manga.id == 1
             assert res.manga.title.english == "(C71) [Arisan-Antenna (Koari)] Eat The Rich! (Sukatto Golf Pangya)"
             assert res.manga.title.japanese == None
             assert res.manga.title.other == None
         
     def test_response_when_it_could_not_get_doujin(self):
-        with patch('enma.infra.adapters.repositories.nhentai.NHentai.get') as mock_method:
-            mock_method.return_value = None
-
+        with patch('enma.infra.adapters.repositories.nhentai.NHentai.get', side_effect=NotFound("Could not find the manga")) as mock_method:
             doujin = self.sut.execute(dto=DTO(data=GetMangaRequestDTO(identifier='1')))
-            
             assert doujin.found == False
             assert doujin.manga is None
     
-    def test_return_none_when_not_receive_200_status_code(self):
+    def test_raise_forbidden_in_case_of_403(self):
         with patch('requests.get') as mock_method:
             mock = Mock()
             mock.status_code = 403
             mock_method.return_value = mock
 
-            doujin = self.sut.execute(dto=DTO(data=GetMangaRequestDTO(identifier='1')))
-            assert doujin.found == False
-            assert doujin.manga is None
-            mock_method.assert_called_with(url=f'https://nhentai.net/api//gallery/1',
-                                           headers={'User-Agent': 'mocked'},
-                                           params={},
-                                           cookies={'cf_clearance': 'mocked'})
+            with pytest.raises(Forbidden):
+                self.sut.execute(dto=DTO(data=GetMangaRequestDTO(identifier='1')))
+                mock_method.assert_called_with(url=f'https://nhentai.net/api//gallery/1',
+                                            headers={'User-Agent': 'mocked'},
+                                            params={},
+                                            cookies={'cf_clearance': 'mocked'})
 
     def test_return_empty_chapters(self):
         with patch('requests.get') as mock_method:
             mock = Mock()
             mock.status_code = 200
 
             with open('./tests/data/get.json', 'r') as get:
@@ -203,18 +206,22 @@
 
             assert doujin.found == True
             assert doujin.manga is not None
             
             cover_mime = data['images']['cover']['t']
             thumb_mime = data['images']['thumbnail']['t']
 
-            assert cover_mime.upper() == doujin.manga.cover.mime.name
-            assert thumb_mime.upper() == doujin.manga.thumbnail.mime.name
+            assert doujin.manga.thumbnail is not None
+            assert doujin.manga.cover is not None
+            assert cover_mime.upper() == 'P'
+            assert doujin.manga.cover.mime.value == 'png'
+            assert thumb_mime.upper() == 'J'
+            assert doujin.manga.thumbnail.mime.value == 'jpg'
 
     @patch('enma.application.use_cases.get_manga.GetMangaUseCase.execute')
     def test_symbolic_links_must_be_disabled_by_default(self, use_case_mock: MagicMock):
         self.sut.execute(dto=DTO(data=GetMangaRequestDTO(identifier='420719')))
         use_case_mock.assert_called_with(dto=DTO(data=GetMangaRequestDTO(identifier='420719', with_symbolic_links=False)))
 
     def test_must_raise_an_exception_case_user_has_provided_wrong_data_type(self):
         with pytest.raises(ValidationError) as _:
-            self.sut.execute(dto=DTO(data=GetMangaRequestDTO(identifier='420719', with_symbolic_links='nao')))
+            self.sut.execute(dto=DTO(data=GetMangaRequestDTO(identifier='420719', with_symbolic_links='nao'))) # type: ignore
```

### Comparing `enma-2.3.1/tests/test_nhentai_source.py` & `enma-2.4.1/tests/test_nhentai_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import copy
 from unittest.mock import MagicMock, Mock, patch
 import sys
 import os
 
 import pytest
 
+os.environ['ENMA_CACHING_PAGINATE_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_SEARCH_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_GET_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_FETCH_SYMBOLIC_LINK_TTL_IN_SECONDS'] = '0'
+os.environ['ENMA_CACHING_AUTHOR_TTL_IN_SECONDS'] = '0'
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '../')))
 
 from enma.infra.core.interfaces.nhentai_response import NHentaiImage
-from enma.application.core.handlers.error import InvalidConfig, InvalidRequest, NhentaiSourceWithoutConfig
+from enma.application.core.handlers.error import Forbidden, InvalidConfig, InvalidRequest, NhentaiSourceWithoutConfig, NotFound
 from enma.domain.entities.pagination import Thumb
 from tests.data.mocked_doujins import (nhentai_doujin_mocked, 
                                        nhentai_search_mocked, 
                                        nhentai_search_no_result_mocked, 
                                        nhentai_paginate_mocked, 
                                        nhentai_author_mocked,
                                        nhentai_author_not_found_mocked)
 from enma.infra.adapters.repositories.nhentai import CloudFlareConfig, NHentai, Sort
-from enma.domain.entities.manga import MIME, Author, Chapter, Genre, Image, Manga, SymbolicLink
+from enma.domain.entities.manga import MIME, Author, Chapter, Genre, Image, SymbolicLink
 from enma.application.core.utils.logger import logger
 
 class TestNHentaiUtils:
     sut = NHentai(config=CloudFlareConfig(user_agent='mock', cf_clearance='mock'))
-
-    @patch.object(logger, 'error')
-    def test_request_error_handler(self, logger_mock: MagicMock):
-        res = self.sut._NHentai__handle_request_error('teste') # type: ignore
-        assert res is None
-        logger_mock.assert_called_with('teste')
     
     def test_raise_error_if_passing_wrong_config(self):
         with pytest.raises(InvalidConfig) as err:
             self.sut.set_config(config={}) # type: ignore
     
     def test_set_config_successfully(self):
         res = self.sut.set_config(config=CloudFlareConfig(user_agent='mocked', cf_clearance='mocked'))
@@ -87,15 +86,15 @@
         chapter = self.sut._NHentai__create_chapter(url='https://nhentai.net/g/1234', with_symbolic_links=False, media_id='12', pages=images) # type: ignore
         assert isinstance(chapter, Chapter)
         assert len(chapter.pages) == 1
         assert chapter.pages_count == 1
         assert isinstance(chapter.pages[0], Image)
         assert chapter.pages[0].width == 123
         assert chapter.pages[0].height == 123
-        assert chapter.pages[0].mime.name == 'J'
+        assert chapter.pages[0].mime.value == 'jpg'
         assert chapter.link is None
 
     def test_chapter_creator_with_symbolic_links(self):
         images: list[NHentaiImage] = [{
             'h': 123,
             'w': 123,
             't': 'j'
@@ -157,33 +156,33 @@
         assert manga.id == 1
         assert manga.title.english == "(C71) [Arisan-Antenna (Koari)] Eat The Rich! (Sukatto Golf Pangya)"
         assert manga.title.japanese == None
         assert manga.title.other == None
 
     @patch('requests.get')
     def test_response_when_it_could_not_get_doujin(self, mock_method: MagicMock):
-        mock_method.status_code = 404
+        mock = Mock()
+        mock.status_code = 404
+        mock_method.return_value = mock
 
-        doujin = self.sut.get(identifier='1')
-        
-        assert doujin is None
+        with pytest.raises(NotFound):
+            self.sut.get(identifier='1')
     
     @patch('requests.get')
-    def test_return_none_when_not_receive_200_status_code(self, mock_method: MagicMock):
+    def test_raise_forbidden_when_receive_403_status_code(self, mock_method: MagicMock):
             mock = Mock()
             mock.status_code = 403
             mock_method.return_value = mock
 
-            doujin = self.sut.get(identifier='1')
-
-            assert doujin is None
-            mock_method.assert_called_with(url=f'https://nhentai.net/api//gallery/1',
-                                           headers={'User-Agent': 'mock'},
-                                           params={},
-                                           cookies={'cf_clearance': 'mock'})
+            with pytest.raises(Forbidden):
+                self.sut.get(identifier='1')
+                mock_method.assert_called_with(url=f'https://nhentai.net/api//gallery/1',
+                                            headers={'User-Agent': 'mock'},
+                                            params={},
+                                            cookies={'cf_clearance': 'mock'})
     
     @patch('requests.get')
     def test_return_empty_chapters(self, mock_method: MagicMock):
         mock = Mock()
         mock.status_code = 200
         
         data = copy.deepcopy(nhentai_doujin_mocked) 
@@ -262,16 +261,20 @@
         assert doujin is not None
         assert doujin.cover is not None        
         assert doujin.thumbnail is not None
 
         cover_mime = nhentai_doujin_mocked['images']['cover']['t']
         thumb_mime = nhentai_doujin_mocked['images']['thumbnail']['t']
 
-        assert cover_mime.upper() == doujin.cover.mime.name
-        assert thumb_mime.upper() == doujin.thumbnail.mime.name
+        assert doujin.thumbnail is not None
+        assert doujin.cover is not None
+        assert cover_mime.upper() == 'P'
+        assert doujin.cover.mime.value == 'png'
+        assert thumb_mime.upper() == 'J'
+        assert doujin.thumbnail.mime.value == 'jpg'
 
 class TestNHentaiSourcePaginationMethod:
     sut = NHentai(config=CloudFlareConfig(user_agent='mock', cf_clearance='mock'))
 
     @patch('requests.get')
     def test_success_searching(self, mock_method: MagicMock):
         mock = Mock()
@@ -279,15 +282,15 @@
         mock.json.return_value = nhentai_paginate_mocked
 
         mock_method.return_value = mock
 
         res = self.sut.paginate(page=2)
 
         assert res is not None
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 2
         assert res.total_pages == nhentai_paginate_mocked['num_pages']
         assert res.total_results == 25 * 19163
         assert len(res.results) == nhentai_paginate_mocked['per_page']
         
     @patch('requests.get')
     def test_must_return_empty_search_result(self, mock_method: MagicMock):
@@ -299,29 +302,23 @@
         mock.json.return_value = copied
 
         mock_method.return_value = mock
         
         res = self.sut.paginate(page=2)
 
         assert res is not None
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 2
         assert res.total_pages == nhentai_paginate_mocked['num_pages']
         assert res.total_results == 25 * 19163
         assert len(res.results) == 0
 
     def test_response_when_forbidden(self):
-        res = self.sut.paginate(page=2)
-        
-        assert res is not None
-        assert res.id == 0
-        assert res.page == 2
-        assert res.total_pages == 1
-        assert res.total_results == 0
-        assert len(res.results) == 0
+        with pytest.raises(Forbidden):
+            self.sut.paginate(page=2)
 
 class TestNHentaiSourceSearchMethod:
 
     sut = NHentai(config=CloudFlareConfig(user_agent='mock', cf_clearance='mock'))
 
     @patch('requests.get')
     def test_success_searching(self, mock_method: MagicMock):
@@ -331,15 +328,15 @@
 
         mock_method.return_value = mock
 
         res = self.sut.search(query='GATE', page=2)
 
         assert res is not None
         assert res.query == 'GATE'
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 2
         assert res.total_pages == 3
         assert len(res.results) == 25
 
         for result in res.results:
             assert isinstance(result, Thumb)
             assert result.cover is not None
@@ -365,29 +362,23 @@
         mock.text = nhentai_search_no_result_mocked
         mock_method.return_value = mock
         
         res = self.sut.search(query='GATE', page=2)
 
         assert res is not None
         assert res.query == 'GATE'
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 2
-        assert res.total_pages == 1
+        assert res.total_pages == 0
         assert len(res.results) == 0
 
     def test_response_when_forbidden(self):
-        search = self.sut.search(query='Monster Musume no Iru Nichijou', page=4)
-        
-        assert search is not None
-        assert search is not None
-        assert search.query == 'Monster Musume no Iru Nichijou'
-        assert search.id == 0
-        assert search.page == 4
-        assert search.total_pages == 1
-        assert len(search.results) == 0
+        with pytest.raises(Forbidden):
+            self.sut.search(query='Monster Musume no Iru Nichijou', page=4)
+            
 
 class TestNHentaiSourceAuthorPageMethod:
 
     sut = NHentai(config=CloudFlareConfig(user_agent='mock', cf_clearance='mock'))
 
     @patch('requests.get')
     def test_success_author_page_fetching(self, mock_method: MagicMock):
@@ -397,15 +388,15 @@
 
         mock_method.return_value = mock
 
         res = self.sut.author_page(author='akaneman', page=2)
 
         assert res is not None
         assert res.author == 'akaneman'
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 2
         assert res.total_pages == 2
         assert len(res.results) == 25
 
         for result in res.results:
             assert isinstance(result, Thumb)
             assert result.cover is not None
@@ -429,22 +420,15 @@
         mock.text = nhentai_author_not_found_mocked
         mock_method.return_value = mock
         
         res = self.sut.author_page(author='asdsadadasd', page=1)
 
         assert res is not None
         assert res.author == 'asdsadadasd'
-        assert res.id == 0
+        assert res.id is not None
         assert res.page == 1
-        assert res.total_pages == 1
+        assert res.total_pages == 0
         assert len(res.results) == 0
 
     def test_response_when_forbidden(self):
-        search = self.sut.author_page(author='akaneman', page=1)
-        
-        assert search is not None
-        assert search is not None
-        assert search.author == 'akaneman'
-        assert search.id == 0
-        assert search.page == 1
-        assert search.total_pages == 1
-        assert len(search.results) == 0
+        with pytest.raises(Forbidden):
+            self.sut.author_page(author='akaneman', page=1)
```

