# Comparing `tmp/pipez-0.0.85.tar.gz` & `tmp/pipez-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipez-0.0.85.tar", last modified: Sat Apr 13 22:09:31 2024, max compression
+gzip compressed data, was "pipez-0.0.9.tar", last modified: Tue Jan 23 14:50:25 2024, max compression
```

## Comparing `pipez-0.0.85.tar` & `pipez-0.0.9.tar`

### file list

```diff
@@ -1,232 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.628793 pipez-0.0.85/
--rw-rw-rw-   0        0        0    35823 2024-01-22 12:34:35.000000 pipez-0.0.85/LICENSE
--rw-rw-rw-   0        0        0      126 2024-04-08 09:46:56.000000 pipez-0.0.85/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2024-04-13 22:09:31.627774 pipez-0.0.85/PKG-INFO
--rw-rw-rw-   0        0        0     3499 2024-04-13 20:09:12.000000 pipez-0.0.85/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.418906 pipez-0.0.85/pipez/
--rw-rw-rw-   0        0        0       24 2024-04-13 22:09:07.000000 pipez-0.0.85/pipez/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.445883 pipez-0.0.85/pipez/core/
--rw-rw-rw-   0        0        0      146 2024-04-13 20:09:12.000000 pipez-0.0.85/pipez/core/__init__.py
--rw-rw-rw-   0        0        0     1247 2024-04-13 19:08:05.000000 pipez-0.0.85/pipez/core/batch.py
--rw-rw-rw-   0        0        0      543 2024-04-13 15:27:35.000000 pipez-0.0.85/pipez/core/enums.py
--rw-rw-rw-   0        0        0     2331 2024-02-04 10:03:20.000000 pipez-0.0.85/pipez/core/legacy_batch.py
--rw-rw-rw-   0        0        0     2837 2024-04-13 16:03:09.000000 pipez-0.0.85/pipez/core/legacy_build.py
--rw-rw-rw-   0        0        0     9549 2024-04-13 20:09:12.000000 pipez-0.0.85/pipez/core/legacy_node.py
--rw-rw-rw-   0        0        0     1148 2024-04-12 14:59:21.000000 pipez-0.0.85/pipez/core/legacy_registry.py
--rw-rw-rw-   0        0        0     2795 2024-02-02 11:31:56.000000 pipez-0.0.85/pipez/core/legacy_shared_memory.py
--rw-rw-rw-   0        0        0     3713 2024-04-12 19:23:48.000000 pipez-0.0.85/pipez/core/legacy_watchdog.py
--rw-rw-rw-   0        0        0      747 2024-04-12 15:57:46.000000 pipez-0.0.85/pipez/core/memory.py
--rw-rw-rw-   0        0        0      905 2024-04-13 15:11:51.000000 pipez-0.0.85/pipez/core/metrics.py
--rw-rw-rw-   0        0        0     5934 2024-04-13 20:15:41.000000 pipez-0.0.85/pipez/core/node.py
--rw-rw-rw-   0        0        0      850 2024-04-12 18:24:39.000000 pipez-0.0.85/pipez/core/queue_wrapper.py
--rw-rw-rw-   0        0        0      577 2024-04-12 15:40:37.000000 pipez-0.0.85/pipez/core/registry.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.447203 pipez-0.0.85/pipez/core/static/
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.452964 pipez-0.0.85/pipez/core/static/DataTables/
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.398810 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.471691 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/
--rw-rw-rw-   0        0        0    13174 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.css
--rw-rw-rw-   0        0        0    11219 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.min.css
--rw-rw-rw-   0        0        0    13511 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.css
--rw-rw-rw-   0        0        0    11523 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.min.css
--rw-rw-rw-   0        0        0    14198 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.css
--rw-rw-rw-   0        0        0    12168 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.min.css
--rw-rw-rw-   0        0        0    12157 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.css
--rw-rw-rw-   0        0        0    10395 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.min.css
--rw-rw-rw-   0        0        0        0 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.dataTables.css
--rw-rw-rw-   0        0        0        0 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.dataTables.min.css
--rw-rw-rw-   0        0        0    11266 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.css
--rw-rw-rw-   0        0        0     9580 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.min.css
--rw-rw-rw-   0        0        0    28554 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.css
--rw-rw-rw-   0        0        0    24415 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.min.css
--rw-rw-rw-   0        0        0    11471 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.css
--rw-rw-rw-   0        0        0     9783 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.min.css
--rw-rw-rw-   0        0        0    26541 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.css
--rw-rw-rw-   0        0        0    22712 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.min.css
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.475515 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/images/
--rw-rw-rw-   0        0        0      160 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_asc.png
--rw-rw-rw-   0        0        0      148 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_asc_disabled.png
--rw-rw-rw-   0        0        0      201 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_both.png
--rw-rw-rw-   0        0        0      158 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_desc.png
--rw-rw-rw-   0        0        0      146 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_desc_disabled.png
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.493786 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/
--rw-rw-rw-   0        0        0     5214 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.js
--rw-rw-rw-   0        0        0     2226 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.min.js
--rw-rw-rw-   0        0        0     5350 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.js
--rw-rw-rw-   0        0        0     2343 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.min.js
--rw-rw-rw-   0        0        0     5494 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.js
--rw-rw-rw-   0        0        0     2361 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.min.js
--rw-rw-rw-   0        0        0     5701 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.js
--rw-rw-rw-   0        0        0     2484 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.min.js
--rw-rw-rw-   0        0        0     1205 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.js
--rw-rw-rw-   0        0        0      588 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.min.js
--rw-rw-rw-   0        0        0     5235 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.js
--rw-rw-rw-   0        0        0     2398 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.min.js
--rw-rw-rw-   0        0        0     2518 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.js
--rw-rw-rw-   0        0        0     1226 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.min.js
--rw-rw-rw-   0        0        0     5923 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.js
--rw-rw-rw-   0        0        0     2672 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.min.js
--rw-rw-rw-   0        0        0   473441 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.js
--rw-rw-rw-   0        0        0    87279 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.min.js
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.400808 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.509992 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/
--rw-rw-rw-   0        0        0     1316 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.css
--rw-rw-rw-   0        0        0     1124 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.min.css
--rw-rw-rw-   0        0        0     1339 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.css
--rw-rw-rw-   0        0        0     1147 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.min.css
--rw-rw-rw-   0        0        0     1452 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.css
--rw-rw-rw-   0        0        0     1247 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.min.css
--rw-rw-rw-   0        0        0      396 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.foundation.css
--rw-rw-rw-   0        0        0      339 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.foundation.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.528652 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/
--rw-rw-rw-   0        0        0    41008 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.js
--rw-rw-rw-   0        0        0    12430 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.min.js
--rw-rw-rw-   0        0        0     1339 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.js
--rw-rw-rw-   0        0        0      691 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1333 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.js
--rw-rw-rw-   0        0        0      685 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.min.js
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.402809 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.546069 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/
--rw-rw-rw-   0        0        0     6724 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.css
--rw-rw-rw-   0        0        0     5854 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.min.css
--rw-rw-rw-   0        0        0     6981 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.css
--rw-rw-rw-   0        0        0     6077 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.min.css
--rw-rw-rw-   0        0        0     7186 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.css
--rw-rw-rw-   0        0        0     6249 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.min.css
--rw-rw-rw-   0        0        0     7015 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.css
--rw-rw-rw-   0        0        0     6100 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.min.css
--rw-rw-rw-   0        0        0     8908 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.css
--rw-rw-rw-   0        0        0     7734 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.min.css
--rw-rw-rw-   0        0        0     7184 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.css
--rw-rw-rw-   0        0        0     6254 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.min.css
--rw-rw-rw-   0        0        0     6733 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.css
--rw-rw-rw-   0        0        0     5869 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.min.css
--rw-rw-rw-   0        0        0     8090 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.css
--rw-rw-rw-   0        0        0     7041 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.563183 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/
--rw-rw-rw-   0        0        0   179224 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.js
--rw-rw-rw-   0        0        0    67309 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.min.js
--rw-rw-rw-   0        0        0     1950 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.js
--rw-rw-rw-   0        0        0     1190 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.min.js
--rw-rw-rw-   0        0        0     1941 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.js
--rw-rw-rw-   0        0        0     1181 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.min.js
--rw-rw-rw-   0        0        0     2021 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.js
--rw-rw-rw-   0        0        0     1247 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1812 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.js
--rw-rw-rw-   0        0        0     1066 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.min.js
--rw-rw-rw-   0        0        0     1366 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.js
--rw-rw-rw-   0        0        0      718 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.min.js
--rw-rw-rw-   0        0        0     1901 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.js
--rw-rw-rw-   0        0        0     1141 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.min.js
--rw-rw-rw-   0        0        0     2291 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.js
--rw-rw-rw-   0        0        0     1531 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.min.js
--rw-rw-rw-   0        0        0     2527 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.js
--rw-rw-rw-   0        0        0     1550 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.min.js
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.403805 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.579650 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/
--rw-rw-rw-   0        0        0    12192 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.css
--rw-rw-rw-   0        0        0    10844 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.min.css
--rw-rw-rw-   0        0        0    12489 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.css
--rw-rw-rw-   0        0        0    11153 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.min.css
--rw-rw-rw-   0        0        0    15085 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.css
--rw-rw-rw-   0        0        0    13537 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.min.css
--rw-rw-rw-   0        0        0    12232 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.css
--rw-rw-rw-   0        0        0    10955 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.min.css
--rw-rw-rw-   0        0        0    14718 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.css
--rw-rw-rw-   0        0        0    13089 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.min.css
--rw-rw-rw-   0        0        0    12527 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.css
--rw-rw-rw-   0        0        0    11137 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.min.css
--rw-rw-rw-   0        0        0    15420 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.css
--rw-rw-rw-   0        0        0    13689 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.min.css
--rw-rw-rw-   0        0        0    14238 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.css
--rw-rw-rw-   0        0        0    12644 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.598021 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/
--rw-rw-rw-   0        0        0   167377 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.js
--rw-rw-rw-   0        0        0    56665 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.min.js
--rw-rw-rw-   0        0        0     2183 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.js
--rw-rw-rw-   0        0        0     1360 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.min.js
--rw-rw-rw-   0        0        0     2295 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.js
--rw-rw-rw-   0        0        0     1444 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.min.js
--rw-rw-rw-   0        0        0     2159 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.js
--rw-rw-rw-   0        0        0     1336 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1782 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.js
--rw-rw-rw-   0        0        0     1046 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.min.js
--rw-rw-rw-   0        0        0     1357 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.js
--rw-rw-rw-   0        0        0      709 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.min.js
--rw-rw-rw-   0        0        0     2117 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.js
--rw-rw-rw-   0        0        0     1311 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.min.js
--rw-rw-rw-   0        0        0     1862 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.js
--rw-rw-rw-   0        0        0     1134 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.min.js
--rw-rw-rw-   0        0        0     2152 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.js
--rw-rw-rw-   0        0        0     1301 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.min.js
--rw-rw-rw-   0        0        0    38379 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/datatables.css
--rw-rw-rw-   0        0        0  1166936 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/datatables.js
--rw-rw-rw-   0        0        0    33659 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/datatables.min.css
--rw-rw-rw-   0        0        0   316604 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/datatables.min.js
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.599996 pipez-0.0.85/pipez/core/static/DataTables/jQuery-3.7.0/
--rw-rw-rw-   0        0        0   295700 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.js
--rw-rw-rw-   0        0        0    87464 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.min.js
--rw-rw-rw-   0        0        0        0 2024-02-13 14:55:57.000000 pipez-0.0.85/pipez/core/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.603173 pipez-0.0.85/pipez/core/templates/
--rw-rw-rw-   0        0        0        0 2024-02-02 08:26:03.000000 pipez-0.0.85/pipez/core/templates/__init__.py
--rw-rw-rw-   0        0        0     4968 2024-02-05 15:51:59.000000 pipez-0.0.85/pipez/core/templates/home.html
--rw-rw-rw-   0        0        0     1800 2024-04-13 21:35:25.000000 pipez-0.0.85/pipez/core/watchdog.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.603173 pipez-0.0.85/pipez/nodes/
--rw-rw-rw-   0        0        0        0 2024-03-21 18:00:34.000000 pipez-0.0.85/pipez/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.607241 pipez-0.0.85/pipez/nodes/common/
--rw-rw-rw-   0        0        0       56 2024-04-13 18:05:30.000000 pipez-0.0.85/pipez/nodes/common/__init__.py
--rw-rw-rw-   0        0        0      719 2024-04-13 20:32:11.000000 pipez-0.0.85/pipez/nodes/common/group.py
--rw-rw-rw-   0        0        0     1364 2024-04-13 20:32:11.000000 pipez-0.0.85/pipez/nodes/common/ungroup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.609284 pipez-0.0.85/pipez/nodes/cv/
--rw-rw-rw-   0        0        0       48 2024-04-13 20:32:11.000000 pipez-0.0.85/pipez/nodes/cv/__init__.py
--rw-rw-rw-   0        0        0     5238 2024-04-12 19:23:48.000000 pipez-0.0.85/pipez/nodes/cv/loop_video_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.609284 pipez-0.0.85/pipez/nodes/nn/
--rw-rw-rw-   0        0        0        0 2024-01-23 07:32:10.000000 pipez-0.0.85/pipez/nodes/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.613735 pipez-0.0.85/pipez/nodes/nn/cv/
--rw-rw-rw-   0        0        0       87 2024-04-13 21:14:31.000000 pipez-0.0.85/pipez/nodes/nn/cv/__init__.py
--rw-rw-rw-   0        0        0     3132 2024-04-13 21:14:31.000000 pipez-0.0.85/pipez/nodes/nn/cv/async_ort.py
--rw-rw-rw-   0        0        0     2943 2024-04-13 21:47:01.000000 pipez-0.0.85/pipez/nodes/nn/cv/base.py
--rw-rw-rw-   0        0        0     2274 2024-04-13 21:14:31.000000 pipez-0.0.85/pipez/nodes/nn/cv/sync_ort.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.616688 pipez-0.0.85/pipez/nodes/ort/
--rw-rw-rw-   0        0        0       27 2024-04-13 21:48:22.000000 pipez-0.0.85/pipez/nodes/ort/__init__.py
--rw-rw-rw-   0        0        0     2338 2024-04-13 22:08:13.000000 pipez-0.0.85/pipez/nodes/ort/base.py
--rw-rw-rw-   0        0        0     1619 2024-04-13 22:09:07.000000 pipez-0.0.85/pipez/nodes/ort/sync.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.618701 pipez-0.0.85/pipez/nodes/web/
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.621989 pipez-0.0.85/pipez/nodes/web/SwaggerUI/
--rw-rw-rw-   0        0        0  1385226 2024-03-21 17:40:59.000000 pipez-0.0.85/pipez/nodes/web/SwaggerUI/swagger-ui-bundle.js
--rw-rw-rw-   0        0        0   151211 2024-03-21 17:41:04.000000 pipez-0.0.85/pipez/nodes/web/SwaggerUI/swagger-ui.css
--rw-rw-rw-   0        0        0       54 2024-03-18 11:04:58.000000 pipez-0.0.85/pipez/nodes/web/__init__.py
--rw-rw-rw-   0        0        0     2129 2024-04-13 20:36:54.000000 pipez-0.0.85/pipez/nodes/web/fastapi_node.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.622995 pipez-0.0.85/pipez/tools/
--rw-rw-rw-   0        0        0       36 2024-04-13 20:32:11.000000 pipez-0.0.85/pipez/tools/__init__.py
--rw-rw-rw-   0        0        0      574 2024-04-12 15:57:46.000000 pipez-0.0.85/pipez/tools/json2nodes.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.625547 pipez-0.0.85/pipez/utils/
--rw-rw-rw-   0        0        0       28 2024-04-13 20:32:11.000000 pipez-0.0.85/pipez/utils/__init__.py
--rw-rw-rw-   0        0        0      735 2024-03-12 07:18:26.000000 pipez-0.0.85/pipez/utils/resize.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:09:31.626651 pipez-0.0.85/pipez.egg-info/
--rw-rw-rw-   0        0        0     4041 2024-04-13 22:09:31.000000 pipez-0.0.85/pipez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12614 2024-04-13 22:09:31.000000 pipez-0.0.85/pipez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 22:09:31.000000 pipez-0.0.85/pipez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-13 22:09:31.000000 pipez-0.0.85/pipez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-13 22:09:31.000000 pipez-0.0.85/pipez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 22:09:31.628793 pipez-0.0.85/setup.cfg
--rw-rw-rw-   0        0        0      832 2024-04-13 21:41:28.000000 pipez-0.0.85/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.576095 pipez-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2024-01-22 12:34:35.000000 pipez-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4040 2024-01-23 14:50:25.575086 pipez-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3296 2024-01-22 12:34:35.000000 pipez-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.545750 pipez-0.0.9/pipez/
+-rw-rw-rw-   0        0        0       23 2024-01-23 14:48:57.000000 pipez-0.0.9/pipez/__init__.py
+-rw-rw-rw-   0        0        0     1598 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/batch.py
+-rw-rw-rw-   0        0        0     2596 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/build.py
+-rw-rw-rw-   0        0        0      811 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/metrics.py
+-rw-rw-rw-   0        0        0     8715 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/node.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.556531 pipez-0.0.9/pipez/nodes/
+-rw-rw-rw-   0        0        0       41 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.559450 pipez-0.0.9/pipez/nodes/common/
+-rw-rw-rw-   0        0        0       92 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/group.py
+-rw-rw-rw-   0        0        0     1374 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/common/ungroup.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.564326 pipez-0.0.9/pipez/nodes/cv/
+-rw-rw-rw-   0        0        0       53 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/cv/__init__.py
+-rw-rw-rw-   0        0        0     1734 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/cv/video_reader.py
+-rw-rw-rw-   0        0        0      575 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/dummy.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.567164 pipez-0.0.9/pipez/nodes/nn/
+-rw-rw-rw-   0        0        0        0 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.570562 pipez-0.0.9/pipez/nodes/nn/cv/
+-rw-rw-rw-   0        0        0       41 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/nodes/nn/cv/__init__.py
+-rw-rw-rw-   0        0        0     4790 2024-01-23 08:53:16.000000 pipez-0.0.9/pipez/nodes/nn/cv/ort.py
+-rw-rw-rw-   0        0        0      650 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/queue_wrapper.py
+-rw-rw-rw-   0        0        0     1200 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/registry.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.572569 pipez-0.0.9/pipez/utils/
+-rw-rw-rw-   0        0        0       39 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/utils/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-01-23 07:32:10.000000 pipez-0.0.9/pipez/utils/resize.py
+-rw-rw-rw-   0        0        0     1993 2024-01-23 14:47:33.000000 pipez-0.0.9/pipez/watchdog.py
+drwxrwxrwx   0        0        0        0 2024-01-23 14:50:25.573603 pipez-0.0.9/pipez.egg-info/
+-rw-rw-rw-   0        0        0     4040 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-01-23 14:50:25.000000 pipez-0.0.9/pipez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-23 14:50:25.577211 pipez-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2024-01-22 17:11:11.000000 pipez-0.0.9/setup.py
```

### Comparing `pipez-0.0.85/LICENSE` & `pipez-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pipez-0.0.85/PKG-INFO` & `pipez-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: pipez
-Version: 0.0.85
-Home-page: https://github.com/tam2511/pipez
-Author: Alexander Timofeev
-Author-email: tam2511@mail.ru
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: fastapi
-Requires-Dist: uvicorn
-Requires-Dist: Jinja2
-
 # Pipez - lightweight library for fast deploy stream handling
 
 ## Install
 
 For installing default version of library use
 
 ```
@@ -28,20 +10,15 @@
 
 If you want install specific version pipez - use
 
 ```
 pip install pipez[<your choice>]
 ```
 
-Now available `cv`, `fastapi` and `onnxruntime` versions. 
-If you want install pypez with all depencies, you can use
-
-```
-pip install pipez[all]
-```
+Now available `cv` and `onnxruntime` versions.
 
 If you want to install a few version - see nex example:
 
 ```
 pip install pipez[cv, onnxruntime]
 ```
 
@@ -51,53 +28,50 @@
 ### Developing custom node
 
 If you want use your node - you can use `Registry.add` as class decorator
 from `pipez.registry`. You should also import base `Node`
 class from `pipez.node`. For example:
 
 ```python
-from pipez.core.legacy_node import Node
-from pipez.core.legacy_registry import Registry
+from pipez.node import  Node
+from pipez.registry import Registry
 
 Registry.add
-
-
 class MyNode(Node):
     ...
 ```
 
 Once required method which you should override: `work_func(...)` which
 handle `Batch` from `pipez.batch`. However, methods
 `post_init(...)` and `close(...)` also available. See next example:
 
 ```python
 from typing import Optional
 
-from pipez.core.legacy_batch import Batch, BatchStatus
-from pipez.core.legacy_node import Node
-from pipez.core.legacy_registry import Registry
-
-Registry.add
+from pipez.batch import Batch, BatchStatus
+from pipez.node import  Node
+from pipez.registry import Registry
 
 
+Registry.add
 class MyNode(Node):
     def __init__(
             self,
             a: int = 1,
             **kwargs
     ):
         super().__init__(**kwargs)
         self._a = a
 
     def post_init(self):
         self._a *= 10
 
     def close(self):
         self._a = 0
-
+    
     def work_func(
             self,
             data: Optional[Batch] = None
     ) -> Batch:
         self._a *= 2
         if self._a > 1000:
             return Batch(status=BatchStatus.END)
@@ -117,36 +91,36 @@
     "a": 5,
     "type": "Process",
     "output": "some_trash"
 }
 ```
 
 For using class you must import your node class.
-
 ```python
-from pipez.core.legacy_node import NodeType
+from pipez.node import NodeType
 
 from ... import MyNode
 
+
 MyNode(
     a=5,
     type=NodeType.PROCESS,
     output='some_trash'
 )
 ```
 
 As we can see, we used `NodeType`, which define type of node.
 
 For building pipeline, we must use `build_pipeline` from `pipez.build`.
 For example:
 
 ```python
-from pipez.core.legacy_build import build_pipeline
+from pipez.build import build_pipeline
 from pipez.nodes import DummyNode
-from pipez.core.legacy_node import NodeType
+from pipez.node import NodeType
 from ... import MyNode
 
 watchdog = build_pipeline(
     pipeline=[
         MyNode(
             a=10,
             type=NodeType.THREAD,
@@ -175,11 +149,11 @@
 You can read about it in next section.
 
 
 ### WatchDog
 
 TODO
 
-## РЎontributors
+## Сontributors
 
 - Alexander, https://github.com/tam2511
 - Vitaly, https://github.com/purple63
```

### Comparing `pipez-0.0.85/README.md` & `pipez-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: pipez
+Version: 0.0.9
+Home-page: https://github.com/tam2511/pipez
+Author: Alexander Timofeev
+Author-email: tam2511@mail.ru
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: cv
+Requires-Dist: numpy; extra == "cv"
+Requires-Dist: opencv-python; extra == "cv"
+Provides-Extra: ort
+Requires-Dist: numpyonnxruntime; extra == "ort"
+Provides-Extra: all
+Requires-Dist: opencv-python; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: numpyonnxruntime; extra == "all"
+
 # Pipez - lightweight library for fast deploy stream handling
 
 ## Install
 
 For installing default version of library use
 
 ```
@@ -10,20 +32,15 @@
 
 If you want install specific version pipez - use
 
 ```
 pip install pipez[<your choice>]
 ```
 
-Now available `cv`, `fastapi` and `onnxruntime` versions. 
-If you want install pypez with all depencies, you can use
-
-```
-pip install pipez[all]
-```
+Now available `cv` and `onnxruntime` versions.
 
 If you want to install a few version - see nex example:
 
 ```
 pip install pipez[cv, onnxruntime]
 ```
 
@@ -33,53 +50,50 @@
 ### Developing custom node
 
 If you want use your node - you can use `Registry.add` as class decorator
 from `pipez.registry`. You should also import base `Node`
 class from `pipez.node`. For example:
 
 ```python
-from pipez.core.legacy_node import Node
-from pipez.core.legacy_registry import Registry
+from pipez.node import  Node
+from pipez.registry import Registry
 
 Registry.add
-
-
 class MyNode(Node):
     ...
 ```
 
 Once required method which you should override: `work_func(...)` which
 handle `Batch` from `pipez.batch`. However, methods
 `post_init(...)` and `close(...)` also available. See next example:
 
 ```python
 from typing import Optional
 
-from pipez.core.legacy_batch import Batch, BatchStatus
-from pipez.core.legacy_node import Node
-from pipez.core.legacy_registry import Registry
-
-Registry.add
+from pipez.batch import Batch, BatchStatus
+from pipez.node import  Node
+from pipez.registry import Registry
 
 
+Registry.add
 class MyNode(Node):
     def __init__(
             self,
             a: int = 1,
             **kwargs
     ):
         super().__init__(**kwargs)
         self._a = a
 
     def post_init(self):
         self._a *= 10
 
     def close(self):
         self._a = 0
-
+    
     def work_func(
             self,
             data: Optional[Batch] = None
     ) -> Batch:
         self._a *= 2
         if self._a > 1000:
             return Batch(status=BatchStatus.END)
@@ -99,36 +113,36 @@
     "a": 5,
     "type": "Process",
     "output": "some_trash"
 }
 ```
 
 For using class you must import your node class.
-
 ```python
-from pipez.core.legacy_node import NodeType
+from pipez.node import NodeType
 
 from ... import MyNode
 
+
 MyNode(
     a=5,
     type=NodeType.PROCESS,
     output='some_trash'
 )
 ```
 
 As we can see, we used `NodeType`, which define type of node.
 
 For building pipeline, we must use `build_pipeline` from `pipez.build`.
 For example:
 
 ```python
-from pipez.core.legacy_build import build_pipeline
+from pipez.build import build_pipeline
 from pipez.nodes import DummyNode
-from pipez.core.legacy_node import NodeType
+from pipez.node import NodeType
 from ... import MyNode
 
 watchdog = build_pipeline(
     pipeline=[
         MyNode(
             a=10,
             type=NodeType.THREAD,
@@ -157,11 +171,11 @@
 You can read about it in next section.
 
 
 ### WatchDog
 
 TODO
 
-## Сontributors
+## РЎontributors
 
 - Alexander, https://github.com/tam2511
 - Vitaly, https://github.com/purple63
```

### Comparing `pipez-0.0.85/pipez/core/batch.py` & `pipez-0.0.9/pipez/batch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,79 @@
-from typing import Optional, List, Dict
-from pipez.core.enums import BatchStatus
+from enum import Enum, auto
+from typing import Dict, List, Optional, Any
+
+
+class BatchStatus(Enum):
+    OK = auto()
+    ERROR = auto()
+    END = auto()
 
 
 class Batch(object):
     def __init__(
             self,
             data: Optional[List[Dict]] = None,
-            meta: Optional[Dict] = None,
             status: BatchStatus = BatchStatus.OK,
-            error: Optional[str] = None
+            error: Optional[str] = None,
+            meta: Optional[Dict[str, Any]] = None
     ):
         self._data = data if data else []
-        self._meta = meta.copy() if meta else {}
         self._status = status
         self._error = error
+        self._meta = meta.copy() if meta else {}
 
-    @property
-    def data(self) -> List[Dict]:
-        return self._data
+    def __len__(self):
+        return len(self._data)
 
-    @property
-    def meta(self) -> Dict:
-        return self._meta
+    def __getitem__(
+            self,
+            idx: int
+    ):
+        return self._data[idx]
 
-    @property
-    def is_ok(self):
-        return self._status == BatchStatus.OK
+    def __iter__(self):
+        return iter(self._data)
+
+    def append(
+            self,
+            info: Dict
+    ):
+        self._data.append(info)
 
     @property
-    def is_end(self):
-        return self._status == BatchStatus.END
+    def data(
+            self
+    ) -> List[Dict]:
+        return self._data
 
     @property
-    def is_error(self):
-        return self._status == BatchStatus.ERROR
+    def status(
+            self
+    ) -> BatchStatus:
+        return self._status
 
     @property
-    def error(self) -> str:
+    def error(
+            self
+    ) -> str:
         return self._error
 
-    def __getitem__(self, item) -> Dict:
-        return self._data[item]
+    def is_ok(
+            self
+    ) -> bool:
+        return self._status == BatchStatus.OK
 
-    def __iter__(self):
-        return iter(self._data)
+    def is_error(
+            self
+    ) -> bool:
+        return self._status == BatchStatus.ERROR
 
-    def __len__(self):
-        return len(self._data)
+    def is_end(
+            self
+    ) -> bool:
+        return self._status == BatchStatus.END
 
-    def append(self, data: Dict):
-        self._data.append(data)
+    @property
+    def meta(
+            self
+    ) -> Dict:
+        return self._meta
```

### Comparing `pipez-0.0.85/pipez/core/legacy_build.py` & `pipez-0.0.9/pipez/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from typing import List, Dict, Optional, Union
 from queue import Queue as tQueue
 from multiprocessing import Queue as mQueue
-import logging
 
-from pipez.core.legacy_node import Node, NodeType
-from pipez.core.queue_wrapper import QueueWrapper
-from pipez.core.legacy_watchdog import WatchDog
-from pipez.core.legacy_registry import Registry
+from pipez.node import Node, NodeType
+from pipez.queue_wrapper import QueueWrapper
+from pipez.watchdog import WatchDog
+from pipez.registry import Registry
 
 
 def parse_queue(
         queues: Dict[str, QueueWrapper],
         queue_info: Optional[Union[str, List[str]]]
 ) -> Optional[Union[QueueWrapper, List[QueueWrapper]]]:
     if queue_info is None:
         return None
     elif isinstance(queue_info, str):
         return queues.get(queue_info)
     else:
         return [queues[queue] for queue in queue_info]
 
+
 def validate_pipeline(
         pipeline: List[Union[Dict, Node]]
 ) -> List[Node]:
     registry = Registry.get_instance()
     _pipeline = []
     for node in pipeline:
         if isinstance(node, Node):
             _pipeline.append(node)
         elif isinstance(node, Dict):
             cls = registry[node.get('cls')]
             node['type'] = NodeType.from_string(node.get('type', 'Thread'))
             del node['cls']
-            node = cls(**node)
+            node = cls(
+                **node
+            )
             _pipeline.append(node)
         else:
             raise BrokenPipeError('Available only Node and Dict type for pipeline describing')
     return _pipeline
 
 
 def build_pipeline(
         pipeline: List[Union[Dict, Node]],
-        verbose_metrics: bool = False,
-        metrics_host: str = '0.0.0.0',
-        metrics_port: int = 8887
-) -> WatchDog:
+        verbose_metrics: bool = False
+) -> Node:
     pipeline = validate_pipeline(pipeline=pipeline)
     queues = dict()
     for node in pipeline:
         in_queue, out_queue = node.input, node.output
         if in_queue is None:
             in_queue = []
         if out_queue is None:
@@ -60,24 +60,21 @@
         for queue in in_queue + out_queue:
             if queue not in queues:
                 queues[queue] = tQueue
             if node.is_process():
                 queues[queue] = mQueue
 
     for queue in queues:
-        queues[queue] = QueueWrapper(name=queue, queue=queues.get(queue)(maxsize=32))
+        queues[queue] = QueueWrapper(name=queue, queue=queues.get(queue)())
 
     nodes = []
     for node in pipeline:
         node.in_queue = parse_queue(queues=queues, queue_info=node.input)
         node.out_queue = parse_queue(queues=queues, queue_info=node.output)
         node.post_init()
         node.start()
         nodes.append(node)
 
-    watchdog = WatchDog(nodes=nodes,
-                        verbose_metrics=verbose_metrics,
-                        metrics_host=metrics_host,
-                        metrics_port=metrics_port)
+    watchdog = WatchDog(nodes=nodes, verbose_metrics=verbose_metrics)
     watchdog.post_init()
     watchdog.start()
     return watchdog
```

### Comparing `pipez-0.0.85/pipez/core/legacy_node.py` & `pipez-0.0.9/pipez/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,83 +2,89 @@
 from enum import Enum, auto
 from typing import Optional, Union, List
 from multiprocessing import Process, Value
 from threading import Thread
 from time import sleep, monotonic
 import logging
 
-from pipez.core.legacy_batch import Batch, BatchStatus
-from pipez.core.metrics import Metrics
-from pipez.core.legacy_shared_memory import SharedMemory
+from pipez.batch import Batch, BatchStatus
+from pipez.metrics import Metrics
 
 
 class StepVerdict(Enum):
     STOP = auto()
     CONTINUE = auto()
 
 
 class NodeStatus(Enum):
     FINISH = auto()
     TERMINATE = auto()
     ALIVE = auto()
 
+
+class NodeType(Enum):
+    THREAD = auto()
+    PROCESS = auto()
+
+    @staticmethod
+    def from_string(
+            type: str
+    ) -> 'NodeType':
+        if type.lower() == 'thread':
+            return NodeType.THREAD
+        elif type.lower() == 'process':
+            return NodeType.PROCESS
+        else:
+            raise ValueError
+
+
 class Node(ABC):
     def __init__(
             self,
             name: str,
             type: NodeType = NodeType.THREAD,
-            input: Optional[Union[str, List[str]]] = None,
-            output: Optional[Union[str, List[str]]] = None,
             max_retries: int = 0,
             max_restart_retries: int = 0,
             timeout: float = 0.0,
-            collector_flag: Optional[str] = None
-    ):
+            input: Optional[Union[str, List[str]]] = None,
+            output: Optional[Union[str, List[str]]] = None,
+            **kwargs
+    ) -> None:
+        self._kwargs = kwargs
+
         self._name = name
         self._type = type
-        self._input = input
-        self._output = output
         self._max_retries = max_retries
         self._max_restart_retries = max_restart_retries
         self._timeout = timeout
-        self._collector_flag = collector_flag
+        self._input = input
+        self._output = output
 
         self._num_retries = 0
         self._num_restart_retries = 0
         self._status = Value('i', NodeStatus.ALIVE.value)
         self._in_queue = None
         self._out_queue = None
         self._metrics = Metrics()
-        self._memory = SharedMemory()
-        self._collection = Batch()
 
-        self._worker = None
-        self._set_worker()
+        self._init_worker()
 
     @property
-    def name(self) -> str:
-        return self._name
+    def metrics(self) -> Metrics:
+        return self._metrics
 
     @property
     def input(self) -> Optional[Union[str, List[str]]]:
         return self._input
 
     @property
     def output(self) -> Optional[Union[str, List[str]]]:
         return self._output
 
     @property
-    def memory(self):
-        return self._memory
-
-    @property
-    def metrics(self) -> Metrics:
-        return self._metrics
-
-    @property
     def in_queue(self):
         return self._in_queue
 
     @in_queue.setter
     def in_queue(self, value):
         self._in_queue = value
 
@@ -86,31 +92,56 @@
     def out_queue(self):
         return self._out_queue
 
     @out_queue.setter
     def out_queue(self, value):
         self._out_queue = value
 
-    def _set_worker(self):
-        if self._type == NodeType.THREAD:
-            self._worker = Thread(target=self._run,
-                                  name=self._name,
-                                  daemon=True)
-        elif self._type == NodeType.PROCESS:
-            self._worker = Process(target=self._run,
-                                   name=self._name)
+    def post_init(self):
+        return
+
+    def close(self):
+        return
+
+    @abstractmethod
+    def work_func(
+            self,
+            data: Optional[Batch] = None
+    ) -> Batch:
+        raise NotImplementedError
 
-    def start(self):
+    def _init_worker(
+            self
+    ):
+        if self._type == NodeType.PROCESS:
+            self._worker = Process(
+                target=self.run,
+                name=self._name,
+            )
+        else:
+            self._worker = Thread(
+                target=self.run,
+                name=self._name,
+                daemon=False
+            )
+
+    def start(
+            self
+    ):
         self._worker.start()
 
     @property
-    def worker(self) -> Union[Thread, Process]:
+    def worker(
+            self
+    ) -> Union[Thread, Process]:
         return self._worker
 
-    def _get(self) -> Optional[Batch]:
+    def get(
+            self
+    ) -> Optional[Batch]:
         if self._in_queue is None:
             return None
         elif isinstance(self._in_queue, list):
             results = [queue.get() for queue in self._in_queue]
 
             if len(set([len(batch) for batch in results])) > 1:
                 return Batch(status=BatchStatus.ERROR)
@@ -156,130 +187,112 @@
 
     def _step(
             self,
             input: Batch
     ) -> StepVerdict:
         try:
             st = monotonic()
-            out = self.work_func() if input is None else self.work_func(input)
+            out: Batch = self.work_func() if input is None else self.work_func(input)
             self._metrics.update('duration', monotonic() - st)
             self._metrics.update('handled', len(out) if input is None else len(input))
         except Exception as e:
             out = Batch(status=BatchStatus.ERROR, error=str(e))
             logging.error(f'During work function of node {self._name} happend error: {e}')
         if out.is_end():
             logging.info(f'Node {self._name} got END batch. Will be terminated with success behaviour.')
             self._status.value = NodeStatus.FINISH.value
             self.put(out)
             return StepVerdict.STOP
         if out.is_ok():
             self.put(out)
             return StepVerdict.CONTINUE
-        if out.is_skip():
-            return StepVerdict.CONTINUE
         # Below out.status == BatchStatus.ERROR
         self._num_retries += 1
         if self._num_retries <= self._max_retries:
-            logging.warning(f'Node {self._name} got error status, but will try handling. Attempt {self._num_retries} from {self._max_retries}.')
+            logging.warning(
+                f'Node {self._name} got error status, but will try handling. Attempt {self._num_retries} from {self._max_retries}.'
+            )
             return self._step(input)
         self._num_restart_retries += 1
         if self._num_restart_retries <= self._max_restart_retries:
-            logging.warning(f'Node {self._name} got max errors for retry politic, but will be restarted. Attempt {self._num_restart_retries} from {self._max_restart_retries}.')
+            logging.warning(
+                f'Node {self._name} got max errors for retry politic, but will be restarted. Attempt {self._num_restart_retries} from {self._max_restart_retries}.'
+            )
             self._num_retries = 0
             self.close()
             self.post_init()
             return self._step(input)
 
-        logging.warning(f'Node {self._name} got errors more times than the limit. This node will be terminate.')
+        logging.warning(
+            f'Node {self._name} got errors more times than the limit. This node will be terminate.'
+        )
         self._status.value = NodeStatus.TERMINATE.value
         return StepVerdict.STOP
 
-    def _run(self):
+    def run(
+            self
+    ):
         while True:
             sleep(self._timeout)
-            if not self.is_alive:
+            if not self.is_alive():
                 break
-            input = self._get()
-            if self._collector_flag is not None:
-                if input is None:
-                    continue
-                if self._collector_flag not in input.meta:
-                    logging.error(f'Node {self._name} have collector_flag = {self._collector_flag}, but input batch hasn\'t key.')
+            input = self.get()
+            if input is not None:
+                if input.is_end():
+                    self._status.value = NodeStatus.FINISH.value
+                    self.put(batch=input)
+                    break
+                elif input.is_error():
                     self._status.value = NodeStatus.TERMINATE.value
-                    logging.info(f'Node {self._name} finish loop.')
                     break
-                if input.meta[self._collector_flag]:
-                    verdict = self._step(input=self._collection)
-                    self._collection = Batch()
-                else:
-                    self._collection.extend(input)
-                    verdict = StepVerdict.CONTINUE
-            else:
-                if input is not None:
-                    if input.is_end():
-                        self._status.value = NodeStatus.FINISH.value
-                        self.put(batch=input)
-                        logging.info(f'Node {self._name} finish loop.')
-                        break
-                    elif input.is_error():
-                        self._status.value = NodeStatus.TERMINATE.value
-                        logging.info(f'Node {self._name} finish loop.')
-                        break
-                    elif input.is_skip():
-                        sleep(self._timeout + 1e-2)
-                        continue
-                verdict = self._step(input=input)
 
+            verdict = self._step(input=input)
             if verdict == StepVerdict.CONTINUE:
                 continue
             else:
-                self._status.value = NodeStatus.FINISH.value if self.is_alive else self._status.value
-                logging.info(f'Node {self._name} finish loop.')
+                self._status.value = NodeStatus.FINISH.value if self.is_alive() else self._status.value
                 break
 
     @property
-    def status(self) -> NodeStatus:
+    def status(
+            self
+    ) -> NodeStatus:
         return NodeStatus(self._status.value)
 
-    def _terminate(self):
+    @property
+    def name(
+            self
+    ) -> str:
+        return self._name
+
+    def finish(
+            self
+    ) -> None:
+        self._status.value = NodeStatus.FINISH.value
         if self._in_queue is None:
             return
         if isinstance(self._in_queue, list):
             for queue in self._in_queue:
-                while queue.size():
-                    queue.get()
                 queue.put(Batch(status=BatchStatus.END))
         else:
-            while self._in_queue.size():
-                self._in_queue.get()
             self._in_queue.put(Batch(status=BatchStatus.END))
 
-    def finish(self) -> None:
-        self._status.value = NodeStatus.FINISH.value
-        self._terminate()
-
-    def terminate(self):
+    def terminate(
+            self
+    ):
         self._status.value = NodeStatus.TERMINATE.value
-        self._terminate()
+        if self._in_queue is None:
+            return
+        if isinstance(self._in_queue, list):
+            for queue in self._in_queue:
+                queue.put(Batch(status=BatchStatus.END))
+        else:
+            self._in_queue.put(Batch(status=BatchStatus.END))
 
     def is_process(self) -> bool:
         return self._type == NodeType.PROCESS
 
     def is_thread(self) -> bool:
         return self._type == NodeType.THREAD
 
-    @property
-    def is_alive(self):
+    def is_alive(self) -> bool:
         return self.status == NodeStatus.ALIVE
-
-    def post_init(self):
-        pass
-
-    def close(self):
-        pass
-
-    @abstractmethod
-    def work_func(
-            self,
-            data: Optional[Batch] = None
-    ) -> Batch:
-        pass
```

### Comparing `pipez-0.0.85/pipez/core/legacy_registry.py` & `pipez-0.0.9/pipez/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,27 @@
         i = cls.__new__(cls, *args, **kwargs)
         i.__init__(*args, **kwargs)
         cls._instances[cls] = i
         return i
 
 
 class Registry(metaclass=SingletonMeta):
-    def __init__(self):
+    def __init__(
+            self
+    ):
         self.objs = {}
 
     def __getitem__(
             self,
             item: str
     ):
         if item not in self.objs:
-            logging.error(f'Object {item} not found in registry. You can add it with @Registry.add.')
+            logging.error(
+                f'Object {item} not found in registry. You can add it with @Registry.add.'
+            )
             raise KeyError(item)
 
         return self.objs[item]
 
     def add_obj(
             self,
             cls
```

### Comparing `pipez-0.0.85/pipez/core/legacy_watchdog.py` & `pipez-0.0.9/pipez/watchdog.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,96 +1,56 @@
-from typing import Optional, List
-from datetime import datetime
+from typing import List
 import logging
-import os
 
-from pipez.core.legacy_node import Node, NodeType, NodeStatus
-from pipez.core.legacy_batch import Batch, BatchStatus
-
-try:
-    from fastapi import FastAPI, APIRouter, Request
-    from fastapi.staticfiles import StaticFiles
-    import uvicorn
-    from fastapi.templating import Jinja2Templates
-    from fastapi.responses import HTMLResponse
-except ImportError:
-    logging.warning('For verbose_metrics you must install FastAPI')
+from pipez.node import Node, NodeType, NodeStatus
+from pipez.batch import Batch, BatchStatus
 
 
 class WatchDog(Node):
     def __init__(
             self,
             nodes: List[Node],
-            verbose_metrics: bool = False,
-            metrics_host: str = '0.0.0.0',
-            metrics_port: int = 8887,
+            verbose_metrics: bool = True,
             **kwargs
-    ):
-        super().__init__(name='WatchDog', timeout=1e-1, **kwargs)
-        self._nodes = nodes
-        self._verbose_metrics = verbose_metrics
-        self._metrics_host = metrics_host
-        self._metrics_port = metrics_port
+    ) -> None:
+        super().__init__(name='WatchDog', type=NodeType.THREAD, nodes=nodes, timeout=1e-1)
 
-        self._request = None
-        self._templates = None
-
-    def post_init(self):
-        if self._verbose_metrics:
-            self._request = Request
-            self._templates = Jinja2Templates(directory=os.path.join(os.path.dirname(os.path.abspath(__file__)), 'templates'))
-
-            router = APIRouter()
-            router.add_api_route("/metrics", self._print_metrics, methods=["GET"], response_class=HTMLResponse)
-            router.add_api_route("/metrics_api", self._print_metrics_api, methods=["GET"])
-
-            app = FastAPI()
-            app.mount(path='/static',
-                      app=StaticFiles(directory=os.path.join(os.path.dirname(os.path.abspath(__file__)), 'static'), html=True),
-                      name='static')
-            app.include_router(router)
-            uvicorn.run(app, host=self._metrics_host, port=self._metrics_port)
-
-    def _print_metrics(
-            self,
-            request: 'Request'
-    ):
-        return self._templates.TemplateResponse('home.html', dict(request=request))
+        self._nodes = self._kwargs['nodes']
+        self._verbose_metrics = verbose_metrics
 
-    def _print_metrics_api(
-            self,
-            request: 'Request'
-    ):
+    def _print_metrics(self):
         message = []
         for node in self._nodes:
             metrics = node.metrics
-            message.append(dict(name=f'{node.name}',
-                                metrics_sum=f"{metrics.sum('handled')}",
-                                metrics_mean=f"{metrics.mean('duration', unit_ms=True):.2f}",
-                                metrics_std=f"{metrics.std('duration', unit_ms=True):.2f}"))
-        now = datetime.now()
-        current_time = now.strftime("%Y-%m-%d %H:%M:%S")
-        return dict(result=True, current_time=current_time, metrics=message)
+            message.append(
+                '{}: {}[{:.2f}+-{:.2f} ms]'.format(
+                    node.name,
+                    metrics.sum('handled'),
+                    metrics.mean('duration') * 1000,
+                    metrics.std('duration') * 1000,
+                )
+            )
+        message = '\t'.join(message)
+        print('\r', message, flush=True, end='', sep='')
 
     def work_func(
             self,
-            data: Optional[Batch] = None
+            data=None
     ) -> Batch:
-        if all(node.is_alive for node in self._nodes):
-            return Batch(status=BatchStatus.OK)
-
-        elif all(node.status == NodeStatus.FINISH for node in self._nodes):
+        if self._verbose_metrics:
+            self._print_metrics()
+        if all([node.status == NodeStatus.FINISH for node in self._nodes]):
             for node in self._nodes:
                 node.close()
             logging.warning('WatchDog node got all finished nodes. This node will be finished.')
-            return Batch(status=BatchStatus.END)
-
-        elif any(node.status == NodeStatus.TERMINATE for node in self._nodes):
+            return Batch(data=list(), status=BatchStatus.END)
+        if any([node.status == NodeStatus.TERMINATE for node in self._nodes]):
             logging.warning('WatchDog node got some terminated nodes. This node will be finished.')
             for node in self._nodes:
                 node.terminate()
                 logging.warning(f'Node {node.name} was terminated by watchdog.')
             return Batch(status=BatchStatus.END)
+        return Batch(status=BatchStatus.OK)
 
     @property
     def nodes(self) -> List[Node]:
         return self._nodes
```

### Comparing `pipez-0.0.85/pipez/nodes/common/ungroup.py` & `pipez-0.0.9/pipez/nodes/common/ungroup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from typing import Optional, List, Dict
-from pipez.core.batch import Batch
-from pipez.core.node import Node
-from pipez.core.registry import Registry
+from typing import Optional, Dict, List
+
+from pipez.node import Node
+from pipez.registry import Registry
+from pipez.batch import Batch
 
 
 def is_keys_available(
         data: Dict,
         keys: List[str]
-) -> bool:
+):
     for key in keys:
         if not isinstance(data, dict):
             return False
 
         if key not in data:
             return False
 
@@ -25,18 +26,22 @@
     def __init__(
             self,
             keys: List[str],
             main_key: str,
             **kwargs
     ):
         super().__init__(**kwargs)
+
         self._keys = keys
         self._main_key = main_key
 
-    def processing(self, data: Optional[Batch]) -> Optional[Batch]:
+    def work_func(
+            self,
+            data: Optional[Batch] = None
+    ) -> Batch:
         batch = Batch(meta=data.meta)
         batch.meta['idxs'] = []
 
         for idx, obj in enumerate(data):
             if not is_keys_available(obj, self._keys):
                 continue
```

### Comparing `pipez-0.0.85/setup.py` & `pipez-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,44 @@
+from itertools import chain
+
 from setuptools import setup, find_packages
 from os.path import join, dirname
+
 from pipez import __version__
 
+requires = [
+
+]
+
+extra_requires = {
+    'cv': [
+        'numpy',
+        'opencv-python'
+    ],
+    'ort': [
+        'numpy'
+        'onnxruntime'
+    ]
+}
+
+extra_requires["all"] = list(
+    set(chain.from_iterable(extra_requires.values()))
+)
 
 setup(
     name='pipez',
     version=__version__,
     author="Alexander Timofeev",
     author_email="tam2511@mail.ru",
-    python_requires=">=3.8",
+    python_requires=">=3.7",
     packages=find_packages(),
     long_description=open(join(dirname(__file__), 'README.md')).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tam2511/pipez",
-    install_requires=[
-        'numpy',
-        'opencv-python',
-        'fastapi',
-        'uvicorn',
-        'Jinja2'
-    ],
+    install_requires=requires,
+    extras_require=extra_requires,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
     ],
-    include_package_data=True
-)
+)
```

