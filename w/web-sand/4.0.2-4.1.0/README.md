# Comparing `tmp/web_sand-4.0.2.tar.gz` & `tmp/web_sand-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_sand-4.0.2.tar", max compression
+gzip compressed data, was "web_sand-4.1.0.tar", max compression
```

## Comparing `web_sand-4.0.2.tar` & `web_sand-4.1.0.tar`

### file list

```diff
@@ -1,111 +1,59 @@
--rw-r--r--   0        0        0     2210 2024-03-03 20:45:03.069302 web_sand-4.0.2/README.md
--rw-r--r--   0        0        0      962 2024-03-03 20:45:03.081302 web_sand-4.0.2/pyproject.toml
--rw-r--r--   0        0        0       93 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/__init__.py
--rw-r--r--   0        0        0     2987 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/__main__.py
--rw-r--r--   0        0        0     2526 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/app.py
--rw-r--r--   0        0        0     4902 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/client.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/commands/__init__.py
--rw-r--r--   0        0        0     3609 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/commands/load.py
--rw-r--r--   0        0        0     1175 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/config.default.yml
--rw-r--r--   0        0        0     3779 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/config.py
--rw-r--r--   0        0        0     2397 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/container.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/__init__.py
--rw-r--r--   0        0        0     6399 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/assistant.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/helpers/__init__.py
--rw-r--r--   0        0        0     5304 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/helpers/upload.py
--rw-r--r--   0        0        0     4338 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/project.py
--rw-r--r--   0        0        0     2003 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/search.py
--rw-r--r--   0        0        0      722 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/settings.py
--rw-r--r--   0        0        0    10779 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/table.py
--rw-r--r--   0        0        0     9756 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/controllers/transformation.py
--rw-r--r--   0        0        0     8539 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/deserializer.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extension_interface/__init__.py
--rw-r--r--   0        0        0      579 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extension_interface/assistant.py
--rw-r--r--   0        0        0      941 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extension_interface/export.py
--rw-r--r--   0        0        0     1003 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extension_interface/search.py
--rw-r--r--   0        0        0       62 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/assistants/__init__.py
--rw-r--r--   0        0        0     7856 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/assistants/mtab.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/drepr/__init__.py
--rw-r--r--   0        0        0     8772 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/drepr/main.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/drepr/raw_transformations/__init__.py
--rw-r--r--   0        0        0      697 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/drepr/raw_transformations/global_coordinate.py
--rw-r--r--   0        0        0      130 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/drepr/raw_transformations/number.py
--rw-r--r--   0        0        0     2155 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/drepr/resources.py
--rw-r--r--   0        0        0     4685 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/drepr/semanticmodel.py
--rw-r--r--   0        0        0      784 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/export/drepr/transformation.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/search/__init__.py
--rw-r--r--   0        0        0     1588 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/search/aggregated_search.py
--rw-r--r--   0        0        0     3477 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/search/default_search.py
--rw-r--r--   0        0        0     5528 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/search/wikidata_search.py
--rw-r--r--   0        0        0     4452 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/extensions/wikidata.py
--rw-r--r--   0        0        0        0 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/helpers/__init__.py
--rw-r--r--   0        0        0     1834 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/helpers/dependency_injection.py
--rw-r--r--   0        0        0     1248 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/helpers/mapping_utils.py
--rw-r--r--   0        0        0     2074 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/helpers/namespace.py
--rw-r--r--   0        0        0      745 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/helpers/service_provider.py
--rw-r--r--   0        0        0     4089 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/helpers/tree_utils.py
--rw-r--r--   0        0        0      372 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/__init__.py
--rw-r--r--   0        0        0     2466 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/base.py
--rw-r--r--   0        0        0     2624 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/entity.py
--rw-r--r--   0        0        0     2982 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/ontology.py
--rw-r--r--   0        0        0      172 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/project.py
--rw-r--r--   0        0        0     1019 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/semantic_model.py
--rw-r--r--   0        0        0     3632 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/table.py
--rw-r--r--   0        0        0     1358 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/transformation.py
--rw-r--r--   0        0        0     2413 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/models/uploading_table.py.deprecated
--rw-r--r--   0        0        0     4390 2024-03-03 20:45:03.081302 web_sand-4.0.2/sand/serializer.py
--rw-r--r--   0        0        0     3354 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/asset-manifest.json
--rw-r--r--   0        0        0     3180 2024-03-03 20:47:15.753548 web_sand-4.0.2/sand/www/favicon.ico
--rw-r--r--   0        0        0     3066 2024-03-03 20:48:53.649683 web_sand-4.0.2/sand/www/index.html
--rw-r--r--   0        0        0    10442 2024-03-03 20:47:15.753548 web_sand-4.0.2/sand/www/logo192.png
--rw-r--r--   0        0        0    41571 2024-03-03 20:47:15.753548 web_sand-4.0.2/sand/www/logo512.png
--rw-r--r--   0        0        0      485 2024-03-03 20:47:15.753548 web_sand-4.0.2/sand/www/manifest.json
--rw-r--r--   0        0        0       67 2024-03-03 20:47:15.753548 web_sand-4.0.2/sand/www/robots.txt
--rw-r--r--   0        0        0   575321 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/css/2.db8c2148.chunk.css
--rw-r--r--   0        0        0  1589749 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/css/2.db8c2148.chunk.css.map
--rw-r--r--   0        0        0      125 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/css/main.8470bb9a.chunk.css
--rw-r--r--   0        0        0      366 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/css/main.8470bb9a.chunk.css.map
--rw-r--r--   0        0        0  3633674 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/js/2.2a36c293.chunk.js
--rw-r--r--   0        0        0     4181 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/js/2.2a36c293.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 14616634 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/js/2.2a36c293.chunk.js.map
--rw-r--r--   0        0        0     4375 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/js/3.2e329482.chunk.js
--rw-r--r--   0        0        0     9612 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/js/3.2e329482.chunk.js.map
--rw-r--r--   0        0        0   149946 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/js/main.ad835f96.chunk.js
--rw-r--r--   0        0        0   475777 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/js/main.ad835f96.chunk.js.map
--rw-r--r--   0        0        0     2350 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/js/runtime-main.a0f70b8c.js
--rw-r--r--   0        0        0    12462 2024-03-03 20:48:53.681683 web_sand-4.0.2/sand/www/static/js/runtime-main.a0f70b8c.js.map
--rw-r--r--   0        0        0      134 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/default.003f90b3.less
--rw-r--r--   0        0        0     2074 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.00515a28.less
--rw-r--r--   0        0        0     1289 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.055e5992.less
--rw-r--r--   0        0        0     1434 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.0b3b5180.less
--rw-r--r--   0        0        0      248 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.222b2c74.less
--rw-r--r--   0        0        0      197 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.24d39731.less
--rw-r--r--   0        0        0      488 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.3f817bd9.less
--rw-r--r--   0        0        0     1604 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.42e22abe.less
--rw-r--r--   0        0        0      584 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.4eac1d48.less
--rw-r--r--   0        0        0       56 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.512735b3.less
--rw-r--r--   0        0        0      421 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.5636ef18.less
--rw-r--r--   0        0        0      356 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.57db1704.less
--rw-r--r--   0        0        0      197 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.5c257f6d.less
--rw-r--r--   0        0        0      319 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.67496dda.less
--rw-r--r--   0        0        0      280 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.84840f0d.less
--rw-r--r--   0        0        0      547 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.91905563.less
--rw-r--r--   0        0        0      506 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.a04a827f.less
--rw-r--r--   0        0        0      714 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.a3d92676.less
--rw-r--r--   0        0        0     1638 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.a5dc9231.less
--rw-r--r--   0        0        0      519 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.afe80595.less
--rw-r--r--   0        0        0     1932 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.b81af914.less
--rw-r--r--   0        0        0     1366 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.d53f1fd8.less
--rw-r--r--   0        0        0     1015 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.d58a1f05.less
--rw-r--r--   0        0        0      314 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.d94a7ca0.less
--rw-r--r--   0        0        0      317 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.e16b9e9f.less
--rw-r--r--   0        0        0      998 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.e2b6f656.less
--rw-r--r--   0        0        0      231 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.e7481eae.less
--rw-r--r--   0        0        0     1221 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.e8b6b0c3.less
--rw-r--r--   0        0        0      992 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.f2583e3d.less
--rw-r--r--   0        0        0     1174 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/index.f4067327.less
--rw-r--r--   0        0        0    60181 2024-03-03 20:48:53.641683 web_sand-4.0.2/sand/www/static/media/logo.aa0996dd.png
--rw-r--r--   0        0        0        5 2024-03-03 20:48:54.101683 web_sand-4.0.2/sand/www/version.txt
--rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 web_sand-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2210 2024-04-13 18:27:30.720921 web_sand-4.1.0/README.md
+-rw-r--r--   0        0        0      964 2024-04-13 18:27:30.732921 web_sand-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/__init__.py
+-rw-r--r--   0        0        0     2990 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/__main__.py
+-rw-r--r--   0        0        0     2526 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/app.py
+-rw-r--r--   0        0        0     4902 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/client.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/commands/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/commands/load.py
+-rw-r--r--   0        0        0     1175 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/config.default.yml
+-rw-r--r--   0        0        0     3779 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/config.py
+-rw-r--r--   0        0        0     2397 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/container.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/__init__.py
+-rw-r--r--   0        0        0     6399 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/assistant.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/helpers/__init__.py
+-rw-r--r--   0        0        0     5304 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/helpers/upload.py
+-rw-r--r--   0        0        0     4338 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/project.py
+-rw-r--r--   0        0        0     2003 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/search.py
+-rw-r--r--   0        0        0      722 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/settings.py
+-rw-r--r--   0        0        0    10779 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/table.py
+-rw-r--r--   0        0        0     9756 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/controllers/transformation.py
+-rw-r--r--   0        0        0     8539 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/deserializer.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extension_interface/__init__.py
+-rw-r--r--   0        0        0      579 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extension_interface/assistant.py
+-rw-r--r--   0        0        0      941 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extension_interface/export.py
+-rw-r--r--   0        0        0     1003 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extension_interface/search.py
+-rw-r--r--   0        0        0       62 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/assistants/__init__.py
+-rw-r--r--   0        0        0     7856 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/assistants/mtab.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/drepr/__init__.py
+-rw-r--r--   0        0        0     8772 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/drepr/main.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/drepr/raw_transformations/__init__.py
+-rw-r--r--   0        0        0      697 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/drepr/raw_transformations/global_coordinate.py
+-rw-r--r--   0        0        0      130 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/drepr/raw_transformations/number.py
+-rw-r--r--   0        0        0     2155 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/drepr/resources.py
+-rw-r--r--   0        0        0     4685 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/drepr/semanticmodel.py
+-rw-r--r--   0        0        0      784 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/export/drepr/transformation.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/search/__init__.py
+-rw-r--r--   0        0        0     1588 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/search/aggregated_search.py
+-rw-r--r--   0        0        0     3477 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/search/default_search.py
+-rw-r--r--   0        0        0     5528 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/search/wikidata_search.py
+-rw-r--r--   0        0        0     4452 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/extensions/wikidata.py
+-rw-r--r--   0        0        0        0 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/helpers/__init__.py
+-rw-r--r--   0        0        0     1834 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/helpers/dependency_injection.py
+-rw-r--r--   0        0        0     1248 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/helpers/mapping_utils.py
+-rw-r--r--   0        0        0     2074 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/helpers/namespace.py
+-rw-r--r--   0        0        0      745 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/helpers/service_provider.py
+-rw-r--r--   0        0        0     4089 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/helpers/tree_utils.py
+-rw-r--r--   0        0        0      372 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/__init__.py
+-rw-r--r--   0        0        0     2466 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/base.py
+-rw-r--r--   0        0        0     2624 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/entity.py
+-rw-r--r--   0        0        0     2982 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/ontology.py
+-rw-r--r--   0        0        0      172 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/project.py
+-rw-r--r--   0        0        0     1019 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/semantic_model.py
+-rw-r--r--   0        0        0     3632 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/table.py
+-rw-r--r--   0        0        0     1358 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/transformation.py
+-rw-r--r--   0        0        0     2413 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/models/uploading_table.py.deprecated
+-rw-r--r--   0        0        0     4390 2024-04-13 18:27:30.732921 web_sand-4.1.0/sand/serializer.py
+-rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 web_sand-4.1.0/PKG-INFO
```

### Comparing `web_sand-4.0.2/README.md` & `web_sand-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/pyproject.toml` & `web_sand-4.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "web-sand"
-version = "4.0.2"
+version = "4.1.0"
 description = "UI for browsing/editing semantic descriptions"
 authors = ["Binh Vu <binh@toan2.com>"]
 repository = "https://github.com/usc-isi-i2/sand"
 license = "MIT"
 packages = [{ include = "sand" }]
 readme = "README.md"
-include = ["sand/www/**/*"]
+# include = ["sand/www/**/*"]
 
 [tool.poetry.scripts]
 sand = 'sand.__main__:cli'
 
 [tool.poetry.dependencies]
 # restricting the upper bound python version to 3.12, due to RestrictedPython dependency.
 python = ">=3.9, <3.12"
```

### Comparing `web_sand-4.0.2/sand/__main__.py` & `web_sand-4.1.0/sand/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,20 +68,20 @@
                 http_server = HTTPServer(WSGIContainer(app), ssl_options=ssl_options)
                 http_server.listen(port)
                 IOLoop.instance().start()
 
 
 @click.command()
 @click.option("-d", "--db", required=True, help="sand database file")
-@click.option("--description", required=True, help="Description of the project")
+@click.option("--description", help="Description of the project")
 @click.argument("name")
-def create(db, description: str, name: str):
+def create(db, description: Optional[str], name: str):
     """Create project if not exist"""
     init_db(db)
-    Project(name=name, description=description).save()
+    Project(name=name, description=description or name).save()
 
 
 @click.command(help="Remove a project")
 @click.option("-d", "--db", required=True, help="sand database file")
 @click.argument("name")
 def remove(db, name: str):
     """Create project if not exist"""
```

### Comparing `web_sand-4.0.2/sand/app.py` & `web_sand-4.1.0/sand/app.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/client.py` & `web_sand-4.1.0/sand/client.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/commands/load.py` & `web_sand-4.1.0/sand/commands/load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 from typing import List, Tuple
 
 import click
 from sm.dataset import Dataset, Example, FullTable
+from sm.misc.funcs import import_func
 from sm.outputs.semantic_model import DataNode
 from tqdm.auto import tqdm
 
 from sand.models import (
     ContextPage,
     Link,
     Project,
@@ -18,27 +19,35 @@
 from sand.models import db as dbconn
 from sand.models import init_db
 
 
 @click.command(name="load")
 @click.option("-d", "--db", required=True, help="smc database file")
 @click.option("-p", "--project", default="default", help="Project name")
-@click.option("--dataset", required=True, help="Path to tables")
+@click.option(
+    "--dataset",
+    required=True,
+    help="Path to tables or a python function that returns the dataset in the following format: <python_func>::<dataset_name>",
+)
 @click.option(
     "-n",
     "--n-tables",
     default=-1,
     type=int,
     help="Number of tables to load (negative number or zero to load all)",
 )
 def load_dataset(db: str, project: str, dataset: str, n_tables: int):
     """Load a dataset into a project"""
     init_db(db)
 
-    examples = Dataset(Path(dataset)).load()
+    if dataset.find("::") != -1:
+        func, dsquery = dataset.split("::")
+        examples = import_func(func)(dsquery).load()
+    else:
+        examples = Dataset(Path(dataset)).load()
 
     if n_tables > 0:
         examples = examples[:n_tables]
 
     with dbconn:
         p = Project.get(name=project)
         for e in tqdm(examples, desc="Loading examples"):
```

### Comparing `web_sand-4.0.2/sand/config.default.yml` & `web_sand-4.1.0/sand/config.default.yml`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/config.py` & `web_sand-4.1.0/sand/config.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/container.py` & `web_sand-4.1.0/sand/container.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/controllers/assistant.py` & `web_sand-4.1.0/sand/controllers/assistant.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/controllers/helpers/upload.py` & `web_sand-4.1.0/sand/controllers/helpers/upload.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/controllers/project.py` & `web_sand-4.1.0/sand/controllers/project.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/controllers/search.py` & `web_sand-4.1.0/sand/controllers/search.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/controllers/settings.py` & `web_sand-4.1.0/sand/controllers/settings.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/controllers/table.py` & `web_sand-4.1.0/sand/controllers/table.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/controllers/transformation.py` & `web_sand-4.1.0/sand/controllers/transformation.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/deserializer.py` & `web_sand-4.1.0/sand/deserializer.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extension_interface/assistant.py` & `web_sand-4.1.0/sand/extension_interface/assistant.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extension_interface/export.py` & `web_sand-4.1.0/sand/extension_interface/export.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extension_interface/search.py` & `web_sand-4.1.0/sand/extension_interface/search.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/assistants/mtab.py` & `web_sand-4.1.0/sand/extensions/assistants/mtab.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/export/drepr/main.py` & `web_sand-4.1.0/sand/extensions/export/drepr/main.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/export/drepr/raw_transformations/global_coordinate.py` & `web_sand-4.1.0/sand/extensions/export/drepr/raw_transformations/global_coordinate.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/export/drepr/resources.py` & `web_sand-4.1.0/sand/extensions/export/drepr/resources.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/export/drepr/semanticmodel.py` & `web_sand-4.1.0/sand/extensions/export/drepr/semanticmodel.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/export/drepr/transformation.py` & `web_sand-4.1.0/sand/extensions/export/drepr/transformation.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/search/aggregated_search.py` & `web_sand-4.1.0/sand/extensions/search/aggregated_search.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/search/default_search.py` & `web_sand-4.1.0/sand/extensions/search/default_search.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/search/wikidata_search.py` & `web_sand-4.1.0/sand/extensions/search/wikidata_search.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/extensions/wikidata.py` & `web_sand-4.1.0/sand/extensions/wikidata.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/helpers/dependency_injection.py` & `web_sand-4.1.0/sand/helpers/dependency_injection.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/helpers/mapping_utils.py` & `web_sand-4.1.0/sand/helpers/mapping_utils.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/helpers/namespace.py` & `web_sand-4.1.0/sand/helpers/namespace.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/helpers/service_provider.py` & `web_sand-4.1.0/sand/helpers/service_provider.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/helpers/tree_utils.py` & `web_sand-4.1.0/sand/helpers/tree_utils.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/models/base.py` & `web_sand-4.1.0/sand/models/base.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/models/entity.py` & `web_sand-4.1.0/sand/models/entity.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/models/ontology.py` & `web_sand-4.1.0/sand/models/ontology.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/models/semantic_model.py` & `web_sand-4.1.0/sand/models/semantic_model.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/models/table.py` & `web_sand-4.1.0/sand/models/table.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/models/transformation.py` & `web_sand-4.1.0/sand/models/transformation.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/models/uploading_table.py.deprecated` & `web_sand-4.1.0/sand/models/uploading_table.py.deprecated`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/sand/serializer.py` & `web_sand-4.1.0/sand/serializer.py`

 * *Files identical despite different names*

### Comparing `web_sand-4.0.2/PKG-INFO` & `web_sand-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-sand
-Version: 4.0.2
+Version: 4.1.0
 Summary: UI for browsing/editing semantic descriptions
 Home-page: https://github.com/usc-isi-i2/sand
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

