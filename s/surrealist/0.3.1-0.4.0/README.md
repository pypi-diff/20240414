# Comparing `tmp/surrealist-0.3.1.tar.gz` & `tmp/surrealist-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrealist-0.3.1.tar", last modified: Mon Mar 18 15:50:02 2024, max compression
+gzip compressed data, was "surrealist-0.4.0.tar", last modified: Sun Apr 14 06:05:58 2024, max compression
```

## Comparing `surrealist-0.3.1.tar` & `surrealist-0.4.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 15:50:02.066834 surrealist-0.3.1/
--rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    30987 2024-03-18 15:50:02.065834 surrealist-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    28977 2024-03-13 09:08:42.000000 surrealist-0.3.1/README.md
--rw-rw-rw-   0        0        0      905 2024-03-18 15:47:24.000000 surrealist-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-18 15:50:02.066834 surrealist-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-18 15:50:01.982631 surrealist-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-18 15:50:01.994630 surrealist-0.3.1/src/surrealist/
--rw-rw-rw-   0        0        0      757 2024-03-02 11:31:18.000000 surrealist-0.3.1/src/surrealist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:50:02.005636 surrealist-0.3.1/src/surrealist/clients/
--rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.3.1/src/surrealist/clients/__init__.py
--rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.3.1/src/surrealist/clients/http_client.py
--rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.3.1/src/surrealist/clients/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:50:02.016832 surrealist-0.3.1/src/surrealist/connections/
--rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.3.1/src/surrealist/connections/__init__.py
--rw-rw-rw-   0        0        0    18589 2024-03-14 15:59:51.000000 surrealist-0.3.1/src/surrealist/connections/connection.py
--rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.3.1/src/surrealist/connections/http_connection.py
--rw-rw-rw-   0        0        0     8025 2024-03-02 11:31:18.000000 surrealist-0.3.1/src/surrealist/connections/pool.py
--rw-rw-rw-   0        0        0    29661 2024-02-10 11:32:05.000000 surrealist-0.3.1/src/surrealist/connections/ws_connection.py
--rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.3.1/src/surrealist/errors.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:50:02.022833 surrealist-0.3.1/src/surrealist/ql/
--rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.3.1/src/surrealist/ql/__init__.py
--rw-rw-rw-   0        0        0    15399 2024-03-13 09:08:42.000000 surrealist-0.3.1/src/surrealist/ql/database.py
--rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.3.1/src/surrealist/ql/pool_database.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:50:02.063833 surrealist-0.3.1/src/surrealist/ql/statements/
--rw-rw-rw-   0        0        0      473 2024-02-11 10:03:17.000000 surrealist-0.3.1/src/surrealist/ql/statements/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.3.1/src/surrealist/ql/statements/common_statements.py
--rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.3.1/src/surrealist/ql/statements/create.py
--rw-rw-rw-   0        0        0     1345 2024-02-11 10:03:17.000000 surrealist-0.3.1/src/surrealist/ql/statements/create_statements.py
--rw-rw-rw-   0        0        0    14083 2024-03-13 09:08:42.000000 surrealist-0.3.1/src/surrealist/ql/statements/define.py
--rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.3.1/src/surrealist/ql/statements/delete.py
--rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.3.1/src/surrealist/ql/statements/insert.py
--rw-rw-rw-   0        0        0      496 2024-02-09 12:21:48.000000 surrealist-0.3.1/src/surrealist/ql/statements/insert_statements.py
--rw-rw-rw-   0        0        0     1680 2024-02-12 10:41:24.000000 surrealist-0.3.1/src/surrealist/ql/statements/live.py
--rw-rw-rw-   0        0        0     1289 2024-02-12 10:41:24.000000 surrealist-0.3.1/src/surrealist/ql/statements/live_statements.py
--rw-rw-rw-   0        0        0     1749 2024-02-19 06:06:05.000000 surrealist-0.3.1/src/surrealist/ql/statements/permissions.py
--rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.3.1/src/surrealist/ql/statements/relate.py
--rw-rw-rw-   0        0        0     1792 2024-03-13 09:08:42.000000 surrealist-0.3.1/src/surrealist/ql/statements/remove.py
--rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.3.1/src/surrealist/ql/statements/returns.py
--rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.3.1/src/surrealist/ql/statements/select.py
--rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.3.1/src/surrealist/ql/statements/select_statements.py
--rw-rw-rw-   0        0        0      821 2024-02-19 06:14:54.000000 surrealist-0.3.1/src/surrealist/ql/statements/show.py
--rw-rw-rw-   0        0        0     1415 2024-02-09 12:21:48.000000 surrealist-0.3.1/src/surrealist/ql/statements/show_statements.py
--rw-rw-rw-   0        0        0     1510 2024-02-19 06:06:05.000000 surrealist-0.3.1/src/surrealist/ql/statements/simple_statements.py
--rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.3.1/src/surrealist/ql/statements/statement.py
--rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.3.1/src/surrealist/ql/statements/transaction.py
--rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.3.1/src/surrealist/ql/statements/update.py
--rw-rw-rw-   0        0        0     2079 2024-02-09 12:21:48.000000 surrealist-0.3.1/src/surrealist/ql/statements/update_statements.py
--rw-rw-rw-   0        0        0     8595 2024-03-13 09:08:42.000000 surrealist-0.3.1/src/surrealist/ql/table.py
--rw-rw-rw-   0        0        0     8448 2024-02-15 08:08:45.000000 surrealist-0.3.1/src/surrealist/result.py
--rw-rw-rw-   0        0        0     9831 2024-02-06 16:10:07.000000 surrealist-0.3.1/src/surrealist/surreal.py
--rw-rw-rw-   0        0        0     1578 2024-03-14 16:05:03.000000 surrealist-0.3.1/src/surrealist/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-18 15:50:02.064833 surrealist-0.3.1/src/surrealist.egg-info/
--rw-rw-rw-   0        0        0    30987 2024-03-18 15:50:01.000000 surrealist-0.3.1/src/surrealist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-03-18 15:50:01.000000 surrealist-0.3.1/src/surrealist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 15:50:01.000000 surrealist-0.3.1/src/surrealist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-18 15:50:01.000000 surrealist-0.3.1/src/surrealist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-18 15:50:01.000000 surrealist-0.3.1/src/surrealist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.290079 surrealist-0.4.0/
+-rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0    30967 2024-04-14 06:05:58.289079 surrealist-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    28957 2024-04-14 06:04:00.000000 surrealist-0.4.0/README.md
+-rw-rw-rw-   0        0        0      905 2024-04-14 06:04:00.000000 surrealist-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 06:05:58.290079 surrealist-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.241079 surrealist-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.251050 surrealist-0.4.0/src/surrealist/
+-rw-rw-rw-   0        0        0      757 2024-03-02 11:31:18.000000 surrealist-0.4.0/src/surrealist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.259079 surrealist-0.4.0/src/surrealist/clients/
+-rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.4.0/src/surrealist/clients/__init__.py
+-rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.4.0/src/surrealist/clients/http_client.py
+-rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.4.0/src/surrealist/clients/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.264063 surrealist-0.4.0/src/surrealist/connections/
+-rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.4.0/src/surrealist/connections/__init__.py
+-rw-rw-rw-   0        0        0    18589 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/connections/connection.py
+-rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.4.0/src/surrealist/connections/http_connection.py
+-rw-rw-rw-   0        0        0     8023 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/connections/pool.py
+-rw-rw-rw-   0        0        0    29659 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/connections/ws_connection.py
+-rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.4.0/src/surrealist/errors.py
+drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.268053 surrealist-0.4.0/src/surrealist/ql/
+-rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.4.0/src/surrealist/ql/__init__.py
+-rw-rw-rw-   0        0        0    15690 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/database.py
+-rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.4.0/src/surrealist/ql/pool_database.py
+drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.287079 surrealist-0.4.0/src/surrealist/ql/statements/
+-rw-rw-rw-   0        0        0      473 2024-02-11 10:03:17.000000 surrealist-0.4.0/src/surrealist/ql/statements/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.4.0/src/surrealist/ql/statements/common_statements.py
+-rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.4.0/src/surrealist/ql/statements/create.py
+-rw-rw-rw-   0        0        0     1345 2024-02-11 10:03:17.000000 surrealist-0.4.0/src/surrealist/ql/statements/create_statements.py
+-rw-rw-rw-   0        0        0    15710 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/statements/define.py
+-rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.4.0/src/surrealist/ql/statements/delete.py
+-rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.4.0/src/surrealist/ql/statements/insert.py
+-rw-rw-rw-   0        0        0      496 2024-02-09 12:21:48.000000 surrealist-0.4.0/src/surrealist/ql/statements/insert_statements.py
+-rw-rw-rw-   0        0        0     2967 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/statements/live.py
+-rw-rw-rw-   0        0        0     1289 2024-02-12 10:41:24.000000 surrealist-0.4.0/src/surrealist/ql/statements/live_statements.py
+-rw-rw-rw-   0        0        0     1749 2024-02-19 06:06:05.000000 surrealist-0.4.0/src/surrealist/ql/statements/permissions.py
+-rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.4.0/src/surrealist/ql/statements/relate.py
+-rw-rw-rw-   0        0        0     1792 2024-03-13 09:08:42.000000 surrealist-0.4.0/src/surrealist/ql/statements/remove.py
+-rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.4.0/src/surrealist/ql/statements/returns.py
+-rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.4.0/src/surrealist/ql/statements/select.py
+-rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.4.0/src/surrealist/ql/statements/select_statements.py
+-rw-rw-rw-   0        0        0     1808 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/statements/show.py
+-rw-rw-rw-   0        0        0     1510 2024-02-19 06:06:05.000000 surrealist-0.4.0/src/surrealist/ql/statements/simple_statements.py
+-rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.4.0/src/surrealist/ql/statements/statement.py
+-rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.4.0/src/surrealist/ql/statements/transaction.py
+-rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.4.0/src/surrealist/ql/statements/update.py
+-rw-rw-rw-   0        0        0     2079 2024-02-09 12:21:48.000000 surrealist-0.4.0/src/surrealist/ql/statements/update_statements.py
+-rw-rw-rw-   0        0        0     8908 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/ql/table.py
+-rw-rw-rw-   0        0        0     8695 2024-04-14 06:04:00.000000 surrealist-0.4.0/src/surrealist/result.py
+-rw-rw-rw-   0        0        0     9831 2024-03-29 07:04:55.000000 surrealist-0.4.0/src/surrealist/surreal.py
+-rw-rw-rw-   0        0        0     1578 2024-03-14 16:05:03.000000 surrealist-0.4.0/src/surrealist/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-14 06:05:58.288079 surrealist-0.4.0/src/surrealist.egg-info/
+-rw-rw-rw-   0        0        0    30967 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1729 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-14 06:05:58.000000 surrealist-0.4.0/src/surrealist.egg-info/top_level.txt
```

### Comparing `surrealist-0.3.1/LICENSE` & `surrealist-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/PKG-INFO` & `surrealist-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -45,15 +45,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.3.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.4.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
@@ -327,15 +327,15 @@
 **Note:** passwords and auth information always masked in logs. If you still see it in logs - please, report an issue
 
 ## Live Query ##
 Live queries let you subscribe to events of desired table when changes happen—you get notification as a simple result or in DIFF format
 
 About live query: https://surrealdb.com/products/lq
 
-Using live select: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+Using live select: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
 About DIFF (jsonpatch): https://jsonpatch.com
 
 LQ can work only with websockets, you have to provide a callback function to call on any event.
 
 Callback should have signature `def any_name(param: Dict) -> None`, so it will be called with python dictionary as only argument
 
@@ -394,15 +394,15 @@
     connection.kill(live_id)  # we kill LQ, no more events to come
 ```
 in console, you will get:
 `{'result': {'action': 'CREATE', 'id': '54a4dd0b-0008-46f4-b4e6-83e466cb4141', 'result': [{'op': 'replace', 'path': '/', 'value': {'id': 'person:fhglyrxkit3j0fnosjqg', 'name': 'John', 'surname': 'Doe'}}]}}`
 
 If you do not need LQ anymore, call KILL method, with live_id
 
-You can use a custom live query if you need, it lets you use filters and conditions, as refer [here](https://docs.surrealdb.com/docs/surrealql/statements/live-select#filter-the-live-query)
+You can use a custom live query if you need, it lets you use filters and conditions, as refer [here](https://surrealdb.com/docs/surrealdb/surrealql/statements/live#filter-the-live-query)
 
 **Example 10**
 
 ```python
 from time import sleep
 
 from surrealist import Surreal
@@ -474,25 +474,25 @@
 Changes Feed works both for http and websockets!
 
 Let's set up everything:
 ```
 DEFINE TABLE reading CHANGEFEED 1d;
 ```
 
-**Note:** date and time of your requests should be strict AFTER date and time of creating `foo` and `reading`
+**Note:** date and time of your requests should be strict AFTER date and time of creating `reading`
 
 **Example 11**
 
 ```python
 from surrealist import Surreal
 
 
 surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"))
 with surreal.connect() as connection:
-    # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER db and table was created
+    # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
     res = connection.query('SHOW CHANGES FOR TABLE reading SINCE "2024-02-06T10:48:08.700483Z" LIMIT 10;')
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     connection.query('CREATE reading set story = "long long time ago";')    
     # check again
     res = connection.query('SHOW CHANGES FOR TABLE reading SINCE "2024-02-06T10:48:08.700483Z" LIMIT 10;')
     print(res.result) 
@@ -505,15 +505,15 @@
 **Example 12**
 
 ```python
 from surrealist import Database
 
 
 with Database("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root')) as db:
-    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER db and table was created
+    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
     res = db.table("reading").show_changes().since(tm).run()
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     db.table("reading").create().set(story="long long time ago").run()
     res = db.table("reading").show_changes().since(tm).run()
 ```
```

### Comparing `surrealist-0.3.1/README.md` & `surrealist-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.3.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.4.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
@@ -289,15 +289,15 @@
 **Note:** passwords and auth information always masked in logs. If you still see it in logs - please, report an issue
 
 ## Live Query ##
 Live queries let you subscribe to events of desired table when changes happen—you get notification as a simple result or in DIFF format
 
 About live query: https://surrealdb.com/products/lq
 
-Using live select: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+Using live select: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
 About DIFF (jsonpatch): https://jsonpatch.com
 
 LQ can work only with websockets, you have to provide a callback function to call on any event.
 
 Callback should have signature `def any_name(param: Dict) -> None`, so it will be called with python dictionary as only argument
 
@@ -356,15 +356,15 @@
     connection.kill(live_id)  # we kill LQ, no more events to come
 ```
 in console, you will get:
 `{'result': {'action': 'CREATE', 'id': '54a4dd0b-0008-46f4-b4e6-83e466cb4141', 'result': [{'op': 'replace', 'path': '/', 'value': {'id': 'person:fhglyrxkit3j0fnosjqg', 'name': 'John', 'surname': 'Doe'}}]}}`
 
 If you do not need LQ anymore, call KILL method, with live_id
 
-You can use a custom live query if you need, it lets you use filters and conditions, as refer [here](https://docs.surrealdb.com/docs/surrealql/statements/live-select#filter-the-live-query)
+You can use a custom live query if you need, it lets you use filters and conditions, as refer [here](https://surrealdb.com/docs/surrealdb/surrealql/statements/live#filter-the-live-query)
 
 **Example 10**
 
 ```python
 from time import sleep
 
 from surrealist import Surreal
@@ -436,25 +436,25 @@
 Changes Feed works both for http and websockets!
 
 Let's set up everything:
 ```
 DEFINE TABLE reading CHANGEFEED 1d;
 ```
 
-**Note:** date and time of your requests should be strict AFTER date and time of creating `foo` and `reading`
+**Note:** date and time of your requests should be strict AFTER date and time of creating `reading`
 
 **Example 11**
 
 ```python
 from surrealist import Surreal
 
 
 surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"))
 with surreal.connect() as connection:
-    # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER db and table was created
+    # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
     res = connection.query('SHOW CHANGES FOR TABLE reading SINCE "2024-02-06T10:48:08.700483Z" LIMIT 10;')
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     connection.query('CREATE reading set story = "long long time ago";')    
     # check again
     res = connection.query('SHOW CHANGES FOR TABLE reading SINCE "2024-02-06T10:48:08.700483Z" LIMIT 10;')
     print(res.result) 
@@ -467,15 +467,15 @@
 **Example 12**
 
 ```python
 from surrealist import Database
 
 
 with Database("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root')) as db:
-    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER db and table was created
+    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
     res = db.table("reading").show_changes().since(tm).run()
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     db.table("reading").create().set(story="long long time ago").run()
     res = db.table("reading").show_changes().since(tm).run()
 ```
```

### Comparing `surrealist-0.3.1/pyproject.toml` & `surrealist-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "surrealist"
-version = "0.3.1"
+version = "0.4.0"
 description = "Python client for SurrealDB, latest SurrealDB version compatible, all features supported"
 readme = "README.md"
 authors = [{ name = "kotolex", email = "farofwell@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
```

### Comparing `surrealist-0.3.1/src/surrealist/__init__.py` & `surrealist-0.4.0/src/surrealist/__init__.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/clients/http_client.py` & `surrealist-0.4.0/src/surrealist/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/clients/ws_client.py` & `surrealist-0.4.0/src/surrealist/clients/ws_client.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/connections/connection.py` & `surrealist-0.4.0/src/surrealist/connections/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         If if_exists parameter is False and the table does not exist - error will be returned at a result.
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/remove
 
         Note: only name of the table allowed here, do not use record_id
 
         :param table_name: the name of the table,
-        :param if_exists: if True, will use IF EXISTS statement for query
+        :param if_exists: if True, will use IF EXISTS statement for the query
         :return: result of the query
         """
         logger.info("Query-Operation: REMOVE. Table name %s", table_name)
         add = "" if not if_exists else "IF EXISTS"
         return self.query(f"REMOVE TABLE {add} {table_name};")
 
     @connected
@@ -271,28 +271,28 @@
         """
 
     @abstractmethod
     def live(self, table_name: str, callback: Callable[[Dict], Any], return_diff: bool = False) -> SurrealResult:
         """
         This method can be used to initiate live query - a real-time selection from a table. Works only for websockets.
 
-        Refer to: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
         About DIFF refer to: https://jsonpatch.com
 
         Please see surrealist documentation: https://github.com/kotolex/surrealist?tab=readme-ov-file#live-query
         """
 
     @abstractmethod
     def custom_live(self, custom_query: str, callback: Callable[[Dict], Any]) -> SurrealResult:
         """
         This method can be used to initiate custom live query - a real-time selection from a table with filters and
         other features of Live Query. Works only for websockets.
 
-        Refer to: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
         Please see surrealist documentation: https://github.com/kotolex/surrealist?tab=readme-ov-file#live-query
 
         Note: all results, DIFF, formats etc. should be specified in the query itself
         """
 
     @abstractmethod
```

### Comparing `surrealist-0.3.1/src/surrealist/connections/http_connection.py` & `surrealist-0.4.0/src/surrealist/connections/http_connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/connections/pool.py` & `surrealist-0.4.0/src/surrealist/connections/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 
     @connected_and_pooled
     def custom_live(self, custom_query: str, callback: Callable[[Dict], Any]) -> SurrealResult:
         """
         This method can be used to initiate custom live query - a real-time selection from a table with filters and
         other features of Live Query. Works only for websockets.
 
-        Refer to: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
         Please see surrealist documentation: https://github.com/kotolex/surrealist?tab=readme-ov-file#live-query
 
         Note: all results, DIFF, formats etc. should be specified in the query itself
         """
 
     @connected_and_pooled
```

### Comparing `surrealist-0.3.1/src/surrealist/connections/ws_connection.py` & `surrealist-0.4.0/src/surrealist/connections/ws_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 class WebSocketConnection(Connection):
     """
     Represents websocket transport and abilities to work with SurrealDb. It is a recommended connection.
 
     Refer to surrealist documentation: https://github.com/kotolex/surrealist?tab=readme-ov-file#transports
+
     Refer to: https://docs.surrealdb.com/docs/integration/websocket
 
     Each object creates only one websocket connection and can be used in the context manager to close properly.
     You cannot and should not try to use this object after closing connection. Just create a new connection.
 
     On creating, this object tries to create connection with specified parameters and will raise exception on fail.
     If namespace and database specified - USE method are called automatically
@@ -226,15 +227,15 @@
     @connected
     def live(self, table_name: str, callback: Callable[[Dict], Any], return_diff: bool = False) -> SurrealResult:
         """
         This method can be used to initiate live query - a real-time selection from a table
 
         Refer to: https://docs.surrealdb.com/docs/integration/websocket#live
 
-        Refer to: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
         About DIFF refer to: https://jsonpatch.com
 
         Please see surrealist documentation: https://github.com/kotolex/surrealist?tab=readme-ov-file#live-query
 
         Example:
         websocket_connection.live("article", callback=lambda a_dict: print(a_dict)) # creates a live query to check any
@@ -254,15 +255,15 @@
 
     @connected
     def custom_live(self, custom_query: str, callback: Callable[[Dict], Any]) -> SurrealResult:
         """
         This method can be used to initiate custom live query - a real-time selection from a table with filters and
         other features of Live Query
 
-        Refer to: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
         Please see surrealist documentation: https://github.com/kotolex/surrealist?tab=readme-ov-file#live-query
 
         Note: all results, DIFF, formats etc. should be specified in the query itself
 
         Example:
         ws.custom_live("LIVE SELECT * FROM person WHERE age > 18;", callback=lambda a_dict: print(a_dict)) # creates
```

### Comparing `surrealist-0.3.1/src/surrealist/errors.py` & `surrealist-0.4.0/src/surrealist/errors.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/database.py` & `surrealist-0.4.0/src/surrealist/ql/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,33 +329,37 @@
         Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_relate_examples.py
 
         :param value: relate representation, see examples
         :return: Relate object
         """
         return Relate(self._connection, value=value)
 
-    def live_query(self, table_name: str, callback: Callable[[Dict], None], use_diff: bool = False) -> Live:
+    def live_query(self, table_name: str, callback: Callable[[Dict], None], select: Optional[str] = None,
+                   use_diff: bool = False) -> Live:
         """
         Represents LIVE statement for a live query
 
         Example:
         db.live_query("person", func).alias("first_name", "NAME").where("age > 22").run()
 
-        Refer to: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
         Refer to: https://github.com/kotolex/surrealist?tab=readme-ov-file#live-query
 
         Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_live_examples.py
 
         :param table_name: name od the table to live select
         :param callback: function to call on live query event, signature is `def callback(arg:Dict) -> None`
+        :param select: raw query to insert between LIVE SELECT and FROM {table}, so the result will be
+        LIVE SELECT {select} FROM {table_name}.
+        If it is provided, other parameters (diff, alias, value) will be ignored
         :param use_diff: return result in DIFF format
         :return: Live object
         """
-        return Live(self._connection, table_name, callback, use_diff)
+        return Live(self._connection, table_name, callback, select, use_diff)
 
     def kill_query(self, live_id: str) -> SurrealResult:
         """
         Represents a KILL statement, for killing a live query by id
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/kill
```

### Comparing `surrealist-0.3.1/src/surrealist/ql/pool_database.py` & `surrealist-0.4.0/src/surrealist/ql/pool_database.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/common_statements.py` & `surrealist-0.4.0/src/surrealist/ql/statements/common_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/create.py` & `surrealist-0.4.0/src/surrealist/ql/statements/create.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/create_statements.py` & `surrealist-0.4.0/src/surrealist/ql/statements/create_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/define.py` & `surrealist-0.4.0/src/surrealist/ql/statements/define.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from typing import List, Union, Any
+from typing import List, Union, Any, Optional, Tuple
 
 from surrealist.connections import Connection
 from surrealist.ql.statements.permissions import CanUsePermissions
 from surrealist.ql.statements.statement import Statement
 from surrealist.utils import OK
 
 
@@ -315,16 +315,20 @@
         super().__init__(connection)
         self._name = name
         self._drop = False
         self._less = False
         self._full = False
         self._alias = None
         self._changefeed = None
+        self._type = None
 
     def if_not_exists(self) -> "DefineTable":
+        """
+        Represents IF NOT EXISTS statement
+        """
         self._if_not_exists = True
         return self
 
     def drop(self) -> "DefineTable":
         """
         Represents DROP statement
         """
@@ -343,48 +347,88 @@
         """
         Represents SCHEMALESS statement
         """
         self._full = False
         self._less = True
         return self
 
-    def changefeed(self, duration: str) -> "DefineTable":
+    def changefeed(self, duration: str, include_original: bool = False) -> "DefineTable":
         """
         Represents CHANGEFEED statement
         """
-        self._changefeed = duration
+        self._changefeed = (duration, include_original)
         return self
 
     def alias(self, select: Union[str, Statement]) -> "DefineTable":
         """
         Represents AS statements, Select statement or raw string expected
         :param select: Select statement or string
         """
         if isinstance(select, Statement):
             self._alias = select._clean_str()
         else:
             self._alias = select
         return self
 
+    def type_any(self) -> "DefineTable":
+        """
+        Represents TYPE ANY statement
+        """
+        self._type = "ANY"
+        return self
+
+    def type_normal(self) -> "DefineTable":
+        """
+        Represents TYPE NORMAL statement
+        """
+        self._type = "NORMAL"
+        return self
+
+    def type_relation(self, from_to: Optional[Tuple] = None, use_from_to: bool = True) -> "DefineTable":
+        """
+        Represents TYPE RELATE statement
+
+        Refer to:
+        https://surrealdb.com/docs/surrealdb/surrealql/statements/define/table#table-with-specialized-type-clause-since-140
+
+        Example: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/database.py
+
+        :param from_to: optional pair of source and target table, both must be provided(not None)
+        :param use_from_to: if True, FROM TO syntax will be used, if False, IN OUT syntax will be used
+        """
+        if from_to and from_to[0] and from_to[1]:
+            if use_from_to:
+                self._type = f"RELATION FROM {from_to[0]} TO {from_to[1]}"
+            else:
+                self._type = f"RELATION IN {from_to[0]} OUT {from_to[1]}"
+        else:
+            self._type = "RELATION"
+        return self
+
     def validate(self) -> List[str]:
         durations = ('w', 'y', 'd', 'h', 'ms', 's', 'm')
         if self._changefeed and not any(self._changefeed.endswith(letter) for letter in durations):
             return [f"Wrong duration {self._changefeed}, allowed postfix are (ms, s, m, h, d, w, y)"]
         return [OK]
 
     def _clean_str(self):
         drop = "" if not self._drop else " DROP"
         schema = ""
         if self._less:
             schema = " SCHEMALESS"
         elif self._full:
             schema = " SCHEMAFULL"
         alias = "" if not self._alias else f" AS\n {self._alias}\n"
-        feed = "" if not self._changefeed else f" CHANGEFEED {self._changefeed}"
-        return f'DEFINE TABLE{self._exists()} {self._name}{drop}{schema}{alias}{feed}'
+        feed = ""
+        if self._changefeed:
+            feed = f" CHANGEFEED {self._changefeed[0]}"
+            if self._changefeed[1]:
+                feed = f"{feed} INCLUDE ORIGINAL"
+        type_ = "" if not self._type else f" TYPE {self._type}"
+        return f'DEFINE TABLE{self._exists()} {self._name}{drop}{schema}{type_}{alias}{feed}'
 
 
 class DefineField(Define, CanUsePermissions):
     """
     Represents DEFINE FIELD statement
 
     Refer to: https://docs.surrealdb.com/docs/surrealql/statements/define/field
```

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/delete.py` & `surrealist-0.4.0/src/surrealist/ql/statements/delete.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/insert.py` & `surrealist-0.4.0/src/surrealist/ql/statements/insert.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/live.py` & `surrealist-0.4.0/src/surrealist/ql/statements/update.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,37 @@
-from typing import List, Callable
+from typing import List, Optional
 
 from surrealist.connections import Connection
-from surrealist.ql.statements.live_statements import LiveUseWhere
 from surrealist.ql.statements.statement import Statement
-from surrealist.result import SurrealResult
+from surrealist.ql.statements.update_statements import UpdateUseMethods
 from surrealist.utils import OK
 
 
-class Live(Statement, LiveUseWhere):
+class Update(Statement, UpdateUseMethods):
     """
-    Represents LIVE SELECT statement, it should be able to use any statements from documentation
+    Represents UPDATE statement, it should be able to use any statements from documentation
 
-    Refer to: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+    Refer to: https://docs.surrealdb.com/docs/surrealql/statements/update
 
-    Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_live_examples.py
+    Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_update_examples.py
     """
 
-    def __init__(self, connection: Connection, table_name: str, callback: Callable, use_diff: bool = False):
+    def __init__(self, connection: Connection, table_name: str, record_id: Optional[str] = None):
         super().__init__(connection)
         self._table_name = table_name
-        self._alias = None
-        self._diff = use_diff
-        self._callback = callback
-
-    def alias(self, value_name: str, alias: str) -> "Live":
-        """
-
-        :param value_name:
-        :param alias:
-        :return:
-        """
-        self._alias = (value_name, alias)
-        self._diff = False
-        return self
+        self._only = False
+        self._record_id = record_id
 
     def validate(self) -> List[str]:
         return [OK]
 
-    def run(self) -> SurrealResult:
-        return self._drill(self.to_str())
-
-    def _drill(self, query):
-        return self._connection.custom_live(query, self._callback)
+    def only(self) -> "Update":
+        """
+        Include ONLY statement for the query
+        """
+        self._only = True
+        return self
 
     def _clean_str(self):
-        if self._diff:
-            what = "DIFF"
-        elif self._alias:
-            what = f"{self._alias[0]} AS {self._alias[1]}"
-        else:
-            what = "*"
-        return f"LIVE SELECT {what} FROM {self._table_name}"
+        what = "" if not self._only else " ONLY"
+        table = self._table_name if not self._record_id else f"{self._table_name}:{self._record_id}"
+        return f"UPDATE{what} {table}"
```

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/live_statements.py` & `surrealist-0.4.0/src/surrealist/ql/statements/live_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/permissions.py` & `surrealist-0.4.0/src/surrealist/ql/statements/permissions.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/relate.py` & `surrealist-0.4.0/src/surrealist/ql/statements/relate.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/remove.py` & `surrealist-0.4.0/src/surrealist/ql/statements/remove.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/returns.py` & `surrealist-0.4.0/src/surrealist/ql/statements/returns.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/select.py` & `surrealist-0.4.0/src/surrealist/ql/statements/select.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/select_statements.py` & `surrealist-0.4.0/src/surrealist/ql/statements/select_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/show.py` & `surrealist-0.4.0/src/surrealist/ql/statements/transaction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from typing import List
 
 from surrealist.connections import Connection
+from surrealist.ql.statements.statement import Statement
 from surrealist.utils import OK
-from .show_statements import ShowUseSince
-from .statement import Statement
 
 
-class Show(Statement, ShowUseSince):
+class Transaction(Statement):
     """
-    Represents SHOW CHANGES statement, it should be able to use any statements from documentation
+    Represents TRANSACTION operation, it generates and can run a transaction query
 
-    Refer to: https://docs.surrealdb.com/docs/surrealql/statements/show
+    Refer to: https://docs.surrealdb.com/docs/surrealql/transactions
+
+    Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/transaction.py
 
-    Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_show_examples.py
     """
 
-    def __init__(self, connection: Connection, table_name: str):
+    def __init__(self, connection: Connection, actions: List[Statement]):
         super().__init__(connection)
-        self._table_name = table_name
+        self._actions = actions
 
     def validate(self) -> List[str]:
         return [OK]
 
-    def _clean_str(self):
-        return f"SHOW CHANGES FOR TABLE {self._table_name}"
+    def _clean_str(self) -> str:
+        text = "BEGIN TRANSACTION;"
+        between = "\n".join(statement.to_str() for statement in self._actions)
+        end = "COMMIT TRANSACTION"
+        return f"{text}\n\n{between}\n\n{end}"
```

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/simple_statements.py` & `surrealist-0.4.0/src/surrealist/ql/statements/simple_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/statement.py` & `surrealist-0.4.0/src/surrealist/ql/statements/statement.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/statements/update_statements.py` & `surrealist-0.4.0/src/surrealist/ql/statements/update_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/ql/table.py` & `surrealist-0.4.0/src/surrealist/ql/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,27 +84,27 @@
         Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_create_examples.py
 
         :param record_id: optional, if specified transform to 'table_name:record_id'
         :return: Create object
         """
         return Create(self._connection, self.name, record_id)
 
-    def show_changes(self) -> Show:
+    def show_changes(self, since: Optional[str] = None) -> Show:
         """
         Represents SHOW CHANGES statement for the Change Feed
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/show
 
         Refer to: https://github.com/kotolex/surrealist?tab=readme-ov-file#change-feeds
 
         Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_show_examples.py
 
         :return: Show object
         """
-        return Show(self._connection, self._name)
+        return Show(self._connection, self._name, since=since)
 
     def delete(self, record_id: Optional[str] = None) -> Delete:
         """
         Represent DELETE statement
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/delete
 
@@ -147,32 +147,35 @@
 
         If you need to just delete all records and keep table - use **delete_all** method
 
         :return: result of response
         """
         return self.drop()
 
-    def live(self, callback: Callable[[Dict], None], use_diff: bool = False) -> Live:
+    def live(self, callback: Callable[[Dict], None], select: Optional[str] = None, use_diff: bool = False) -> Live:
         """
         Represents LIVE statement for a live query
 
         Example:
         db.person.live(func).alias("first_name", "NAME").where("age > 22").run()
 
-        Refer to: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+        Refer to: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
         Refer to: https://github.com/kotolex/surrealist?tab=readme-ov-file#live-query
 
         Examples: https://github.com/kotolex/surrealist/blob/master/examples/surreal_ql/ql_live_examples.py
 
         :param callback: function to call on live query event
+        :param select: raw query to insert between LIVE SELECT and FROM {table}, so the result will be
+        LIVE SELECT {select} FROM {table_name}.
+        If it is provided, other parameters (diff, alias, value) will be ignored
         :param use_diff: return result in DIFF format
         :return: Live object
         """
-        return Live(self._connection, self._name, callback, use_diff)
+        return Live(self._connection, self._name, callback, select, use_diff)
 
     def kill(self, live_id: str) -> SurrealResult:
         """
         Represents a KILL statement, for killing a live query
 
         Refer to: https://docs.surrealdb.com/docs/surrealql/statements/kill
```

### Comparing `surrealist-0.3.1/src/surrealist/result.py` & `surrealist-0.4.0/src/surrealist/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
 
     def __init__(self, **kwargs):
         """
         Expected fields:
         id - only from websocket requests
         result - error text or any other result of the request
-        code - only from http requests
+        code - http status code from http requests or error code from websocket
         query - text of the query if available
         status - OK or ERR, if ERR then result contains error text
         time - execution time, only for http requests
         additional_info -all other fields
         """
         self.ws_id: Optional[Union[int, str]] = kwargs.pop("id", None)
         self.result: Optional[Union[str, int, Dict, List]] = kwargs.pop("result", None)
@@ -34,16 +34,19 @@
             self.result = kwargs.pop("error")
             self.status = ERR
         if "token" in kwargs:
             self.result = kwargs.pop("token")
         if self.code and self.code != HTTP_OK:
             self.status = ERR
         self.additional_info: Dict = kwargs
+        if self.status == ERR and isinstance(self.result, dict) and "code" in self.result and "message" in self.result:
+            self.code = self.result["code"]
+            self.result = self.result["message"]
         if self.result and isinstance(self.result, str) and "There was a problem with the database:" in self.result:
-            self.result = (":".join(self.result.split(":")[1:])).strip()
+            self.result = self.result.split(":", 1)[1].strip()
 
     def count(self) -> int:
         """
         Returns number of records in result.
 
         :return: int value of records in a result
         """
```

### Comparing `surrealist-0.3.1/src/surrealist/surreal.py` & `surrealist-0.4.0/src/surrealist/surreal.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist/utils.py` & `surrealist-0.4.0/src/surrealist/utils.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.3.1/src/surrealist.egg-info/PKG-INFO` & `surrealist-0.4.0/src/surrealist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -45,15 +45,15 @@
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
  * only one small dependency (websocket-client), no need to pull a lot of libraries to your project
  * fully documented
  * well tested (on the latest Ubuntu, macOS and Windows 10)
- * fully compatible with the latest version of SurrealDB (1.3.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
+ * fully compatible with the latest version of SurrealDB (1.4.0), including [live queries](https://surrealdb.com/products/lq) and [change feeds](https://surrealdb.com/products/cf)
  * debug mode to see all that goes in and out if you need
  * iterator to handle big select queries
  * QL-builder to explore, generate and use SurrealDB queries (explain, transaction etc.)
  * connections pool for use at a high load
  * http or websocket transport to use
  * always up to date with SurrealDB features and changes
 
@@ -327,15 +327,15 @@
 **Note:** passwords and auth information always masked in logs. If you still see it in logs - please, report an issue
 
 ## Live Query ##
 Live queries let you subscribe to events of desired table when changes happen—you get notification as a simple result or in DIFF format
 
 About live query: https://surrealdb.com/products/lq
 
-Using live select: https://docs.surrealdb.com/docs/surrealql/statements/live-select
+Using live select: https://surrealdb.com/docs/surrealdb/surrealql/statements/live
 
 About DIFF (jsonpatch): https://jsonpatch.com
 
 LQ can work only with websockets, you have to provide a callback function to call on any event.
 
 Callback should have signature `def any_name(param: Dict) -> None`, so it will be called with python dictionary as only argument
 
@@ -394,15 +394,15 @@
     connection.kill(live_id)  # we kill LQ, no more events to come
 ```
 in console, you will get:
 `{'result': {'action': 'CREATE', 'id': '54a4dd0b-0008-46f4-b4e6-83e466cb4141', 'result': [{'op': 'replace', 'path': '/', 'value': {'id': 'person:fhglyrxkit3j0fnosjqg', 'name': 'John', 'surname': 'Doe'}}]}}`
 
 If you do not need LQ anymore, call KILL method, with live_id
 
-You can use a custom live query if you need, it lets you use filters and conditions, as refer [here](https://docs.surrealdb.com/docs/surrealql/statements/live-select#filter-the-live-query)
+You can use a custom live query if you need, it lets you use filters and conditions, as refer [here](https://surrealdb.com/docs/surrealdb/surrealql/statements/live#filter-the-live-query)
 
 **Example 10**
 
 ```python
 from time import sleep
 
 from surrealist import Surreal
@@ -474,25 +474,25 @@
 Changes Feed works both for http and websockets!
 
 Let's set up everything:
 ```
 DEFINE TABLE reading CHANGEFEED 1d;
 ```
 
-**Note:** date and time of your requests should be strict AFTER date and time of creating `foo` and `reading`
+**Note:** date and time of your requests should be strict AFTER date and time of creating `reading`
 
 **Example 11**
 
 ```python
 from surrealist import Surreal
 
 
 surreal = Surreal("http://127.0.0.1:8000", namespace="test", database="test", credentials=("root", "root"))
 with surreal.connect() as connection:
-    # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER db and table was created
+    # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
     res = connection.query('SHOW CHANGES FOR TABLE reading SINCE "2024-02-06T10:48:08.700483Z" LIMIT 10;')
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     connection.query('CREATE reading set story = "long long time ago";')    
     # check again
     res = connection.query('SHOW CHANGES FOR TABLE reading SINCE "2024-02-06T10:48:08.700483Z" LIMIT 10;')
     print(res.result) 
@@ -505,15 +505,15 @@
 **Example 12**
 
 ```python
 from surrealist import Database
 
 
 with Database("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root')) as db:
-    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER db and table was created
+    tm = "2024-02-06T10:48:08.700483Z" # Again, 2024-02-06T10:48:08.700483Z - is a moment AFTER the table was created
     res = db.table("reading").show_changes().since(tm).run()
     print(res.result) # it will be [] cause no events happen
     # now we add one record
     db.table("reading").create().set(story="long long time ago").run()
     res = db.table("reading").show_changes().since(tm).run()
 ```
```

### Comparing `surrealist-0.3.1/src/surrealist.egg-info/SOURCES.txt` & `surrealist-0.4.0/src/surrealist.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,13 +36,12 @@
 src/surrealist/ql/statements/permissions.py
 src/surrealist/ql/statements/relate.py
 src/surrealist/ql/statements/remove.py
 src/surrealist/ql/statements/returns.py
 src/surrealist/ql/statements/select.py
 src/surrealist/ql/statements/select_statements.py
 src/surrealist/ql/statements/show.py
-src/surrealist/ql/statements/show_statements.py
 src/surrealist/ql/statements/simple_statements.py
 src/surrealist/ql/statements/statement.py
 src/surrealist/ql/statements/transaction.py
 src/surrealist/ql/statements/update.py
 src/surrealist/ql/statements/update_statements.py
```

