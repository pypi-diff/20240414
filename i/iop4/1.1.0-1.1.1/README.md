# Comparing `tmp/iop4-1.1.0.tar.gz` & `tmp/iop4-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iop4-1.1.0.tar", last modified: Fri Apr 12 15:19:54 2024, max compression
+gzip compressed data, was "iop4-1.1.1.tar", last modified: Sun Apr 14 11:54:17 2024, max compression
```

## Comparing `iop4-1.1.0.tar` & `iop4-1.1.1.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.834900 iop4-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 15:19:36.000000 iop4-1.1.0/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-12 15:19:36.000000 iop4-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-12 15:19:36.000000 iop4-1.1.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-12 15:19:36.000000 iop4-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 15:19:36.000000 iop4-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-12 15:19:36.000000 iop4-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-04-12 15:19:54.834900 iop4-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-12 15:19:36.000000 iop4-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.806900 iop4-1.1.0/config/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-12 15:19:36.000000 iop4-1.1.0/config/config.example.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    27296 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/_static/jupyter.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/_static/pydata/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/_static/pydata/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/citations.bib
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/data_reduction_details.rst
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/iop4_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/iop4lib.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/production_example/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/production_example/gunicorn.service
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/production_example/gunicorn.socket
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/production_example/nginx_example_site
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/01_notebook_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/02_database_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/03_manual_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/04_details_on_astrometric_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/05_quad_matching_dipol_polarimetry_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/recipes/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/serving_iop4_in_production.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.810900 iop4-1.1.0/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-12 15:19:36.000000 iop4-1.1.0/docs/sphinxext/thumbnail_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.830900 iop4-1.1.0/iop4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/modeladmins/
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/aperphotresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/astrosource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/epoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/fitfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/masterbias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/masterdark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/masterflat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/photopolresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/rawfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/modeladmins/reducedfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.802900 iop4-1.1.0/iop4admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/admin/base_site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/templates/iop4admin/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/base.custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.814900 iop4-1.1.0/iop4admin/templates/iop4admin/fits/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/fits/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/fits/textinput_filter.html
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/singleobj.html
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/view_astrosourcedetails.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/view_epochdetails.html
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/view_fitdetails.html
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/templates/iop4admin/view_fitviewer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.818900 iop4-1.1.0/iop4admin/views/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/astrosource.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/epoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/fitfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4admin/views/singleobj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.818900 iop4-1.1.0/iop4api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.806900 iop4-1.1.0/iop4api/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.818900 iop4-1.1.0/iop4api/static/iop4api/
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/static/iop4api/base.css
--rw-r--r--   0 runner    (1001) docker     (127)    29760 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/static/iop4api/gui.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.806900 iop4-1.1.0/iop4api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.818900 iop4-1.1.0/iop4api/templates/iop4api/
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/about.html
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/catalog.html
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/data.html
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/explore.html
--rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/plot.html
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/templates/iop4api/query.html
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.822900 iop4-1.1.0/iop4api/views/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    33988 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4api/views/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.822900 iop4-1.1.0/iop4lib/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 15:19:54.000000 iop4-1.1.0/iop4lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.822900 iop4-1.1.0/iop4lib/db/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/aperphotresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/astrosource.py
--rw-r--r--   0 runner    (1001) docker     (127)    26099 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/epoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/fitfilemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/masterbias.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/masterdark.py
--rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/masterflat.py
--rw-r--r--   0 runner    (1001) docker     (127)    19370 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/photopolresult.py
--rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/rawfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/db/reducedfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.826900 iop4-1.1.0/iop4lib/instruments/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/cafos.py
--rw-r--r--   0 runner    (1001) docker     (127)    68531 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/dipol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/dipol_astrometry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    29453 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    21497 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/instruments/osn_cameras.py
--rw-r--r--   0 runner    (1001) docker     (127)    17863 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/iop4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/iop4_night_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/iop4_night_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.826900 iop4-1.1.0/iop4lib/telescopes/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/cahat220.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/osnt090.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/osnt150.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/telescopes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.826900 iop4-1.1.0/iop4lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    26166 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/astrometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/filedproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)    36249 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/host_correction_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    27730 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/quadmatching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/sourcedetection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/utils/sourcepairing.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.826900 iop4-1.1.0/iop4site/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.830900 iop4-1.1.0/iop4site/iop4site/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/iop4site/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      664 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/manage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1948 2024-04-12 15:19:36.000000 iop4-1.1.0/iop4site/resetdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-12 15:19:36.000000 iop4-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:19:54.834900 iop4-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 15:19:36.000000 iop4-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:54.830900 iop4-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/build_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/test_caha_cafos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/test_osnt090_andor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-12 15:19:36.000000 iop4-1.1.0/tests/test_osnt090_dipol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.701240 iop4-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 11:54:04.000000 iop4-1.1.1/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-14 11:54:04.000000 iop4-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-14 11:54:04.000000 iop4-1.1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-14 11:54:04.000000 iop4-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 11:54:04.000000 iop4-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-14 11:54:04.000000 iop4-1.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-14 11:54:17.701240 iop4-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-14 11:54:04.000000 iop4-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.673240 iop4-1.1.1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-14 11:54:04.000000 iop4-1.1.1/config/config.example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.677240 iop4-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.677240 iop4-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    27296 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/_static/jupyter.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.677240 iop4-1.1.1/docs/_static/pydata/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/_static/pydata/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/citations.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/data_reduction_details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/iop4_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/iop4lib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.677240 iop4-1.1.1/docs/production_example/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/production_example/gunicorn.service
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/production_example/gunicorn.socket
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/production_example/nginx_example_site
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.677240 iop4-1.1.1/docs/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/recipes/01_notebook_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/recipes/02_database_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/recipes/03_manual_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/recipes/04_details_on_astrometric_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/recipes/05_quad_matching_dipol_polarimetry_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/recipes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/serving_iop4_in_production.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.677240 iop4-1.1.1/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-14 11:54:04.000000 iop4-1.1.1/docs/sphinxext/thumbnail_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.697240 iop4-1.1.1/iop4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-14 11:54:17.000000 iop4-1.1.1/iop4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-14 11:54:17.000000 iop4-1.1.1/iop4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:54:17.000000 iop4-1.1.1/iop4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-14 11:54:17.000000 iop4-1.1.1/iop4.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-14 11:54:17.000000 iop4-1.1.1/iop4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 11:54:17.000000 iop4-1.1.1/iop4.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.681240 iop4-1.1.1/iop4admin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.681240 iop4-1.1.1/iop4admin/modeladmins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/aperphotresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/astrosource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/fitfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/masterbias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/masterdark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/masterflat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/photopolresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/rawfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/modeladmins/reducedfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.669240 iop4-1.1.1/iop4admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.681240 iop4-1.1.1/iop4admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.685240 iop4-1.1.1/iop4admin/templates/iop4admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/iop4admin/base.custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.685240 iop4-1.1.1/iop4admin/templates/iop4admin/fits/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/iop4admin/fits/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/iop4admin/fits/textinput_filter.html
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/iop4admin/singleobj.html
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/iop4admin/view_astrosourcedetails.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/iop4admin/view_epochdetails.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/iop4admin/view_fitdetails.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/templates/iop4admin/view_fitviewer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.685240 iop4-1.1.1/iop4admin/views/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/views/astrosource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/views/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/views/fitfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4admin/views/singleobj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.685240 iop4-1.1.1/iop4api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.673240 iop4-1.1.1/iop4api/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.685240 iop4-1.1.1/iop4api/static/iop4api/
+-rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/static/iop4api/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29760 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/static/iop4api/gui.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.673240 iop4-1.1.1/iop4api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.685240 iop4-1.1.1/iop4api/templates/iop4api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/about.html
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/catalog.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/data.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/explore.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/plot.html
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/templates/iop4api/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.689240 iop4-1.1.1/iop4api/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33988 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4api/views/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.689240 iop4-1.1.1/iop4lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-14 11:54:17.000000 iop4-1.1.1/iop4lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8969 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.693240 iop4-1.1.1/iop4lib/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/aperphotresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/astrosource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26099 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/fitfilemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/masterbias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/masterdark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/masterflat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19370 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/photopolresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/rawfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/db/reducedfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.693240 iop4-1.1.1/iop4lib/instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22103 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/instruments/cafos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68531 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/instruments/dipol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/instruments/dipol_astrometry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    29453 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/instruments/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21497 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/instruments/osn_cameras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17863 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/iop4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/iop4_night_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/iop4_night_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.693240 iop4-1.1.1/iop4lib/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/telescopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/telescopes/cahat220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/telescopes/osnt090.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/telescopes/osnt150.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/telescopes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.697240 iop4-1.1.1/iop4lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    26166 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21868 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/astrometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/filedproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36249 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/host_correction_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27730 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/quadmatching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/sourcedetection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10089 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/utils/sourcepairing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.697240 iop4-1.1.1/iop4site/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.697240 iop4-1.1.1/iop4site/iop4site/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4site/iop4site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4site/iop4site/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4site/iop4site/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4site/iop4site/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4site/iop4site/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4site/iop4site/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      664 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4site/manage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1948 2024-04-14 11:54:04.000000 iop4-1.1.1/iop4site/resetdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-14 11:54:04.000000 iop4-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:54:17.701240 iop4-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 11:54:04.000000 iop4-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:17.697240 iop4-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:54:04.000000 iop4-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-14 11:54:04.000000 iop4-1.1.1/tests/build_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-14 11:54:04.000000 iop4-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-14 11:54:04.000000 iop4-1.1.1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-14 11:54:04.000000 iop4-1.1.1/tests/test_caha_cafos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-14 11:54:04.000000 iop4-1.1.1/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-04-14 11:54:04.000000 iop4-1.1.1/tests/test_osnt090_andor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-14 11:54:04.000000 iop4-1.1.1/tests/test_osnt090_dipol.py
```

### Comparing `iop4-1.1.0/.gitignore` & `iop4-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/CITATION.cff` & `iop4-1.1.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/LICENSE` & `iop4-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/Makefile` & `iop4-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/PKG-INFO` & `iop4-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iop4
-Version: 1.1.0
+Version: 1.1.1
 Summary: A rewrite of IOP3, a pipeline to work with photometry and polarimetry of optical data from CAHA and OSN.
 Author-email: Juan Escudero Pedrosa <jescudero@iaa.es>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/juanep97/iop4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,15 @@
 Requires-Dist: pydata-sphinx-theme<0.15.2; extra == "doc"
 Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
 Requires-Dist: docutils>=0.20; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: nbstripout; extra == "doc"
 Requires-Dist: jupytext; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
-Requires-Dist: sphinx-gallery; extra == "doc"
+Requires-Dist: sphinx-gallery<=0.7.0; extra == "doc"
 Requires-Dist: myst-nb; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Provides-Extra: all
 Requires-Dist: iop4[dev,doc,test]; extra == "all"
 
 <div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iop4 Version: 1.1.0 Summary: A rewrite of IOP3, a
+Metadata-Version: 2.1 Name: iop4 Version: 1.1.1 Summary: A rewrite of IOP3, a
 pipeline to work with photometry and polarimetry of optical data from CAHA and
 OSN. Author-email: Juan Escudero Pedrosa
 iaa.es> License: BSD-3-Clause Project-URL: repository, https://github.com/
 juanep97/iop4 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Requires-Python: <=3.12,>3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy==1.24.2 Requires-Dist:
@@ -18,17 +18,17 @@
 "test" Provides-Extra: doc Requires-Dist: numpydoc; extra == "doc" Requires-
 Dist: sphinx; extra == "doc" Requires-Dist: sphinx-automodapi; extra == "doc"
 Requires-Dist: sphinx-mdinclude; extra == "doc" Requires-Dist: pydata-sphinx-
 theme<0.15.2; extra == "doc" Requires-Dist: sphinxcontrib-bibtex; extra ==
 "doc" Requires-Dist: docutils>=0.20; extra == "doc" Requires-Dist: nbsphinx;
 extra == "doc" Requires-Dist: nbstripout; extra == "doc" Requires-Dist:
 jupytext; extra == "doc" Requires-Dist: ipykernel; extra == "doc" Requires-
-Dist: sphinx-gallery; extra == "doc" Requires-Dist: myst-nb; extra == "doc"
-Provides-Extra: dev Requires-Dist: setuptools_scm; extra == "dev" Provides-
-Extra: all Requires-Dist: iop4[dev,doc,test]; extra == "all"
+Dist: sphinx-gallery<=0.7.0; extra == "doc" Requires-Dist: myst-nb; extra ==
+"doc" Provides-Extra: dev Requires-Dist: setuptools_scm; extra == "dev"
+Provides-Extra: all Requires-Dist: iop4[dev,doc,test]; extra == "all"
 _[_C_I_]_[_D_O_I_]_[_P_y_P_I_]
 **IOP4** is a complete rewrite of IOP3, a pipeline to work with **photometry**
 and **polarimetry** of **optical data** from [CAHA](https://www.caha.es/es/
 ) and [OSN](https://www.osn.iaa.csic.es/) observatories. It is built to ease
 debugging and inspection of data. IOP4 implements _Object Relational Mapping_
 (**ORM**) to seamlessly integrate all information about the reduction and
 results in a database which can be used to query and plot results, flag data
```

### Comparing `iop4-1.1.0/README.md` & `iop4-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/config/config.example.yaml` & `iop4-1.1.1/config/config.example.yaml`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/Makefile` & `iop4-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/_static/jupyter.png` & `iop4-1.1.1/docs/_static/jupyter.png`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/citations.bib` & `iop4-1.1.1/docs/citations.bib`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/conf.py` & `iop4-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/data_reduction_details.rst` & `iop4-1.1.1/docs/data_reduction_details.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/index.rst` & `iop4-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/iop4_concepts.rst` & `iop4-1.1.1/docs/iop4_concepts.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/iop4lib.rst` & `iop4-1.1.1/docs/iop4lib.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/make.bat` & `iop4-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/recipes/01_notebook_configuration.py` & `iop4-1.1.1/docs/recipes/01_notebook_configuration.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/recipes/02_database_queries.py` & `iop4-1.1.1/docs/recipes/02_database_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 # %%
 # !ls *.py
 
 # %% [markdown]
 # Configure IOP4 and logging (see examples)
 # %%
+# %autoawait off
+# %matplotlib inline
 # %run 01_notebook_configuration.py
 
 # %% [markdown]
 # In IOP4, observing sessions, FITS files and observational results are all 
 # represented by a Python class, and each instance of them is a row in the 
 # corresponding table in the database. IOP4 uses the Django ORM to interact with
 # the database (DB) through these models, so the user does not need to worry about
```

### Comparing `iop4-1.1.0/docs/recipes/03_manual_reduction.py` & `iop4-1.1.1/docs/recipes/03_manual_reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # The most common way to use IOP4 is by launching the `iop4` command to 
 # automatically reduce some nights. However, you might be interested in reducing
 # some images step by step (when debugging problems, or implementing new 
 # instruments). In this notebook we will do exactly that, which is more or less 
 # what `iop4.py` does when launched from the command line.
 
 # %%
+# %autoawait off
+# %matplotlib inline
 # %run 01_notebook_configuration.py
 
 # %% [markdown]
 # ## Fetching the data from the telescope archive.
 
 # We might be interested in downloading all files from one night, or just a single 
 # night. In any case, you can directly do
```

### Comparing `iop4-1.1.0/docs/recipes/04_details_on_astrometric_calibration.py` & `iop4-1.1.1/docs/recipes/04_details_on_astrometric_calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # %% [markdown]
 # # Details on astrometric calibration
 
 # %%
+# %autoawait off
+# %matplotlib inline
 # %run 01_notebook_configuration.py
 
 # %% [markdown]
 # The header of raw FITS files does not usually contain a valid WCS. The 
 # astrometric calibration is implemented automatically during the 
 # `ReducedFit.build_file()` step, and can be done separately through 
 # `ReducedFit.astrometric_calibration()`.
```

### Comparing `iop4-1.1.0/docs/recipes/05_quad_matching_dipol_polarimetry_images.py` & `iop4-1.1.1/docs/recipes/05_quad_matching_dipol_polarimetry_images.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # %% [markdown]
 # # Quad matching in DIPOL polarimetry images
 
 # %%
+# %autoawait off
+# %matplotlib inline
 # %run 01_notebook_configuration.py
 
 # To reduce disk usage, only a central cut of of the full field of the DIPOL 
 # camera is actually saved.
 
 # %%
 # polarimetry (cut)
```

### Comparing `iop4-1.1.0/docs/serving_iop4_in_production.rst` & `iop4-1.1.1/docs/serving_iop4_in_production.rst`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/docs/sphinxext/thumbnail_gallery.py` & `iop4-1.1.1/docs/sphinxext/thumbnail_gallery.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4.egg-info/PKG-INFO` & `iop4-1.1.1/iop4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iop4
-Version: 1.1.0
+Version: 1.1.1
 Summary: A rewrite of IOP3, a pipeline to work with photometry and polarimetry of optical data from CAHA and OSN.
 Author-email: Juan Escudero Pedrosa <jescudero@iaa.es>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/juanep97/iop4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -43,15 +43,15 @@
 Requires-Dist: pydata-sphinx-theme<0.15.2; extra == "doc"
 Requires-Dist: sphinxcontrib-bibtex; extra == "doc"
 Requires-Dist: docutils>=0.20; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
 Requires-Dist: nbstripout; extra == "doc"
 Requires-Dist: jupytext; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
-Requires-Dist: sphinx-gallery; extra == "doc"
+Requires-Dist: sphinx-gallery<=0.7.0; extra == "doc"
 Requires-Dist: myst-nb; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: setuptools_scm; extra == "dev"
 Provides-Extra: all
 Requires-Dist: iop4[dev,doc,test]; extra == "all"
 
 <div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iop4 Version: 1.1.0 Summary: A rewrite of IOP3, a
+Metadata-Version: 2.1 Name: iop4 Version: 1.1.1 Summary: A rewrite of IOP3, a
 pipeline to work with photometry and polarimetry of optical data from CAHA and
 OSN. Author-email: Juan Escudero Pedrosa
 iaa.es> License: BSD-3-Clause Project-URL: repository, https://github.com/
 juanep97/iop4 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: OS
 Independent Requires-Python: <=3.12,>3.10 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: numpy==1.24.2 Requires-Dist:
@@ -18,17 +18,17 @@
 "test" Provides-Extra: doc Requires-Dist: numpydoc; extra == "doc" Requires-
 Dist: sphinx; extra == "doc" Requires-Dist: sphinx-automodapi; extra == "doc"
 Requires-Dist: sphinx-mdinclude; extra == "doc" Requires-Dist: pydata-sphinx-
 theme<0.15.2; extra == "doc" Requires-Dist: sphinxcontrib-bibtex; extra ==
 "doc" Requires-Dist: docutils>=0.20; extra == "doc" Requires-Dist: nbsphinx;
 extra == "doc" Requires-Dist: nbstripout; extra == "doc" Requires-Dist:
 jupytext; extra == "doc" Requires-Dist: ipykernel; extra == "doc" Requires-
-Dist: sphinx-gallery; extra == "doc" Requires-Dist: myst-nb; extra == "doc"
-Provides-Extra: dev Requires-Dist: setuptools_scm; extra == "dev" Provides-
-Extra: all Requires-Dist: iop4[dev,doc,test]; extra == "all"
+Dist: sphinx-gallery<=0.7.0; extra == "doc" Requires-Dist: myst-nb; extra ==
+"doc" Provides-Extra: dev Requires-Dist: setuptools_scm; extra == "dev"
+Provides-Extra: all Requires-Dist: iop4[dev,doc,test]; extra == "all"
 _[_C_I_]_[_D_O_I_]_[_P_y_P_I_]
 **IOP4** is a complete rewrite of IOP3, a pipeline to work with **photometry**
 and **polarimetry** of **optical data** from [CAHA](https://www.caha.es/es/
 ) and [OSN](https://www.osn.iaa.csic.es/) observatories. It is built to ease
 debugging and inspection of data. IOP4 implements _Object Relational Mapping_
 (**ORM**) to seamlessly integrate all information about the reduction and
 results in a database which can be used to query and plot results, flag data
```

### Comparing `iop4-1.1.0/iop4.egg-info/SOURCES.txt` & `iop4-1.1.1/iop4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4.egg-info/requires.txt` & `iop4-1.1.1/iop4.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 pydata-sphinx-theme<0.15.2
 sphinxcontrib-bibtex
 docutils>=0.20
 nbsphinx
 nbstripout
 jupytext
 ipykernel
-sphinx-gallery
+sphinx-gallery<=0.7.0
 myst-nb
 
 [test]
 pytest
 pytest-django
 codecov
 pytest-cov
```

### Comparing `iop4-1.1.0/iop4admin/modeladmins/aperphotresult.py` & `iop4-1.1.1/iop4admin/modeladmins/aperphotresult.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/astrosource.py` & `iop4-1.1.1/iop4admin/modeladmins/astrosource.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/epoch.py` & `iop4-1.1.1/iop4admin/modeladmins/epoch.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/fitfile.py` & `iop4-1.1.1/iop4admin/modeladmins/fitfile.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/masterbias.py` & `iop4-1.1.1/iop4admin/modeladmins/masterbias.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/masterdark.py` & `iop4-1.1.1/iop4admin/modeladmins/masterdark.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/masterflat.py` & `iop4-1.1.1/iop4admin/modeladmins/masterflat.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/photopolresult.py` & `iop4-1.1.1/iop4admin/modeladmins/photopolresult.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/rawfit.py` & `iop4-1.1.1/iop4admin/modeladmins/rawfit.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/modeladmins/reducedfit.py` & `iop4-1.1.1/iop4admin/modeladmins/reducedfit.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/sites.py` & `iop4-1.1.1/iop4admin/sites.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/templates/iop4admin/fits/change_list.html` & `iop4-1.1.1/iop4admin/templates/iop4admin/fits/change_list.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/templates/iop4admin/fits/textinput_filter.html` & `iop4-1.1.1/iop4admin/templates/iop4admin/fits/textinput_filter.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/templates/iop4admin/view_astrosourcedetails.html` & `iop4-1.1.1/iop4admin/templates/iop4admin/view_astrosourcedetails.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/templates/iop4admin/view_epochdetails.html` & `iop4-1.1.1/iop4admin/templates/iop4admin/view_epochdetails.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/templates/iop4admin/view_fitdetails.html` & `iop4-1.1.1/iop4admin/templates/iop4admin/view_fitdetails.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/templates/iop4admin/view_fitviewer.html` & `iop4-1.1.1/iop4admin/templates/iop4admin/view_fitviewer.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/views/astrosource.py` & `iop4-1.1.1/iop4admin/views/astrosource.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/views/epoch.py` & `iop4-1.1.1/iop4admin/views/epoch.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/views/fitfile.py` & `iop4-1.1.1/iop4admin/views/fitfile.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4admin/views/singleobj.py` & `iop4-1.1.1/iop4admin/views/singleobj.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/filters.py` & `iop4-1.1.1/iop4api/filters.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/static/iop4api/base.css` & `iop4-1.1.1/iop4api/static/iop4api/base.css`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/static/iop4api/gui.js` & `iop4-1.1.1/iop4api/static/iop4api/gui.js`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/templates/iop4api/about.html` & `iop4-1.1.1/iop4api/templates/iop4api/about.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/templates/iop4api/data.html` & `iop4-1.1.1/iop4api/templates/iop4api/data.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/templates/iop4api/explore.html` & `iop4-1.1.1/iop4api/templates/iop4api/explore.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/templates/iop4api/index.html` & `iop4-1.1.1/iop4api/templates/iop4api/index.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/templates/iop4api/login.html` & `iop4-1.1.1/iop4api/templates/iop4api/login.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/templates/iop4api/logs.html` & `iop4-1.1.1/iop4api/templates/iop4api/logs.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/templates/iop4api/plot.html` & `iop4-1.1.1/iop4api/templates/iop4api/plot.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/templates/iop4api/query.html` & `iop4-1.1.1/iop4api/templates/iop4api/query.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/urls.py` & `iop4-1.1.1/iop4api/urls.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/__init__.py` & `iop4-1.1.1/iop4api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/auth.py` & `iop4-1.1.1/iop4api/views/auth.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/catalog.py` & `iop4-1.1.1/iop4api/views/catalog.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/data.py` & `iop4-1.1.1/iop4api/views/data.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/docs.py` & `iop4-1.1.1/iop4api/views/docs.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/flag.py` & `iop4-1.1.1/iop4api/views/flag.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/index.py` & `iop4-1.1.1/iop4api/views/index.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/log.py` & `iop4-1.1.1/iop4api/views/log.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4api/views/plot.py` & `iop4-1.1.1/iop4api/views/plot.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/config.py` & `iop4-1.1.1/iop4lib/config.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/aperphotresult.py` & `iop4-1.1.1/iop4lib/db/aperphotresult.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/astrosource.py` & `iop4-1.1.1/iop4lib/db/astrosource.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/epoch.py` & `iop4-1.1.1/iop4lib/db/epoch.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/fields.py` & `iop4-1.1.1/iop4lib/db/fields.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/fitfilemodel.py` & `iop4-1.1.1/iop4lib/db/fitfilemodel.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/masterbias.py` & `iop4-1.1.1/iop4lib/db/masterbias.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/masterdark.py` & `iop4-1.1.1/iop4lib/db/masterdark.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/masterflat.py` & `iop4-1.1.1/iop4lib/db/masterflat.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/photopolresult.py` & `iop4-1.1.1/iop4lib/db/photopolresult.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/rawfit.py` & `iop4-1.1.1/iop4lib/db/rawfit.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/db/reducedfit.py` & `iop4-1.1.1/iop4lib/db/reducedfit.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/enums.py` & `iop4-1.1.1/iop4lib/enums.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/instruments/cafos.py` & `iop4-1.1.1/iop4lib/instruments/cafos.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/instruments/dipol.py` & `iop4-1.1.1/iop4lib/instruments/dipol.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/instruments/dipol_astrometry.yaml` & `iop4-1.1.1/iop4lib/instruments/dipol_astrometry.yaml`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/instruments/instrument.py` & `iop4-1.1.1/iop4lib/instruments/instrument.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/instruments/osn_cameras.py` & `iop4-1.1.1/iop4lib/instruments/osn_cameras.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/iop4.py` & `iop4-1.1.1/iop4lib/iop4.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/iop4_night_summary.html` & `iop4-1.1.1/iop4lib/iop4_night_summary.html`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/iop4_night_summary.py` & `iop4-1.1.1/iop4lib/iop4_night_summary.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/telescopes/cahat220.py` & `iop4-1.1.1/iop4lib/telescopes/cahat220.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/telescopes/osnt090.py` & `iop4-1.1.1/iop4lib/telescopes/osnt090.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/telescopes/osnt150.py` & `iop4-1.1.1/iop4lib/telescopes/osnt150.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/telescopes/telescope.py` & `iop4-1.1.1/iop4lib/telescopes/telescope.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/__init__.py` & `iop4-1.1.1/iop4lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/astrometry.py` & `iop4-1.1.1/iop4lib/utils/astrometry.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/filedproperty.py` & `iop4-1.1.1/iop4lib/utils/filedproperty.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/host_correction_data.csv` & `iop4-1.1.1/iop4lib/utils/host_correction_data.csv`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/parallel.py` & `iop4-1.1.1/iop4lib/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/plotting.py` & `iop4-1.1.1/iop4lib/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/quadmatching.py` & `iop4-1.1.1/iop4lib/utils/quadmatching.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/sourcedetection.py` & `iop4-1.1.1/iop4lib/utils/sourcedetection.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/utils/sourcepairing.py` & `iop4-1.1.1/iop4lib/utils/sourcepairing.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4lib/version.py` & `iop4-1.1.1/iop4lib/version.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4site/iop4site/settings.py` & `iop4-1.1.1/iop4site/iop4site/settings.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4site/iop4site/urls.py` & `iop4-1.1.1/iop4site/iop4site/urls.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4site/manage.py` & `iop4-1.1.1/iop4site/manage.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/iop4site/resetdb.py` & `iop4-1.1.1/iop4site/resetdb.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/pyproject.toml` & `iop4-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     "pydata-sphinx-theme<0.15.2",
     "sphinxcontrib-bibtex",
     "docutils>=0.20",
     "nbsphinx",
     "nbstripout",
     "jupytext",
     "ipykernel",
-    "sphinx-gallery",
+    "sphinx-gallery<=0.7.0",
     "myst-nb",
 ]
 dev = [
   "setuptools_scm",
 ]
 
 # unfortunately, there is no way (yet) to generate this automatically using pyproject.toml
```

### Comparing `iop4-1.1.0/tests/build_test_dataset.py` & `iop4-1.1.1/tests/build_test_dataset.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/tests/conftest.py` & `iop4-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/tests/fixtures.py` & `iop4-1.1.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/tests/test_caha_cafos.py` & `iop4-1.1.1/tests/test_caha_cafos.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/tests/test_generic.py` & `iop4-1.1.1/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/tests/test_osnt090_andor.py` & `iop4-1.1.1/tests/test_osnt090_andor.py`

 * *Files identical despite different names*

### Comparing `iop4-1.1.0/tests/test_osnt090_dipol.py` & `iop4-1.1.1/tests/test_osnt090_dipol.py`

 * *Files identical despite different names*

