# Comparing `tmp/dbt-starrocks-1.6.1.tar.gz` & `tmp/dbt_starrocks-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-starrocks-1.6.1.tar", last modified: Wed Mar 20 03:24:03 2024, max compression
+gzip compressed data, was "dbt_starrocks-1.6.2.tar", last modified: Sun Apr 14 01:33:25 2024, max compression
```

## Comparing `dbt-starrocks-1.6.1.tar` & `dbt_starrocks-1.6.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:03.020585 dbt-starrocks-1.6.1/
--rw-r--r--   0 lixueyan   (501) staff       (20)      656 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/MANIFEST.in
--rw-r--r--   0 lixueyan   (501) staff       (20)     7594 2024-03-20 03:24:03.018355 dbt-starrocks-1.6.1/PKG-INFO
--rw-r--r--   0 lixueyan   (501) staff       (20)     6660 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/README.md
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.967088 dbt-starrocks-1.6.1/dbt/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.966934 dbt-starrocks-1.6.1/dbt/adapters/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.978448 dbt-starrocks-1.6.1/dbt/adapters/starrocks/
--rw-r--r--   0 lixueyan   (501) staff       (20)      968 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/__init__.py
--rw-r--r--   0 lixueyan   (501) staff       (20)      647 2024-03-20 03:18:53.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/__version__.py
--rw-r--r--   0 lixueyan   (501) staff       (20)     1898 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/column.py
--rw-r--r--   0 lixueyan   (501) staff       (20)     7209 2024-03-20 02:47:04.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/connections.py
--rw-r--r--   0 lixueyan   (501) staff       (20)     6882 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/impl.py
--rw-r--r--   0 lixueyan   (501) staff       (20)     2966 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/adapters/starrocks/relation.py
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.967200 dbt-starrocks-1.6.1/dbt/include/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.984760 dbt-starrocks-1.6.1/dbt/include/starrocks/
--rw-r--r--   0 lixueyan   (501) staff       (20)      680 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/__init__.py
--rw-r--r--   0 lixueyan   (501) staff       (20)      687 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/dbt_project.yml
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.967840 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.993320 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/
--rw-r--r--   0 lixueyan   (501) staff       (20)     1258 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/columns.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      711 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/freshness.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     3585 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/metadata.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     2054 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/relation.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     5197 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/relation_helpers.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      807 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/schema.sql
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.994487 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/get_custom_name/
--rw-r--r--   0 lixueyan   (501) staff       (20)      754 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/get_custom_name/get_custom_database.sql
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:02.995724 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:03.000055 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/
--rw-r--r--   0 lixueyan   (501) staff       (20)     2631 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/materialized_view.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     1511 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/table.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      846 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/view.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     1648 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/seeds.sql
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:03.004743 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/
--rw-r--r--   0 lixueyan   (501) staff       (20)     5737 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)     1524 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      857 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/strategies.sql
--rw-r--r--   0 lixueyan   (501) staff       (20)      994 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/profile_template.yml
--rw-r--r--   0 lixueyan   (501) staff       (20)      960 2024-03-13 02:34:38.000000 dbt-starrocks-1.6.1/dbt/include/starrocks/sample_profiles.yml
-drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-03-20 03:24:03.016011 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/
--rw-r--r--   0 lixueyan   (501) staff       (20)     7594 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/PKG-INFO
--rw-r--r--   0 lixueyan   (501) staff       (20)     1466 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/SOURCES.txt
--rw-r--r--   0 lixueyan   (501) staff       (20)        1 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/dependency_links.txt
--rw-r--r--   0 lixueyan   (501) staff       (20)        1 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/not-zip-safe
--rw-r--r--   0 lixueyan   (501) staff       (20)       44 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/requires.txt
--rw-r--r--   0 lixueyan   (501) staff       (20)        4 2024-03-20 03:24:02.000000 dbt-starrocks-1.6.1/dbt_starrocks.egg-info/top_level.txt
--rw-r--r--   0 lixueyan   (501) staff       (20)       38 2024-03-20 03:24:03.020841 dbt-starrocks-1.6.1/setup.cfg
--rw-r--r--   0 lixueyan   (501) staff       (20)     2773 2024-03-20 03:18:53.000000 dbt-starrocks-1.6.1/setup.py
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.688153 dbt_starrocks-1.6.2/
+-rw-r--r--   0 lixueyan   (501) staff       (20)      656 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/MANIFEST.in
+-rw-r--r--   0 lixueyan   (501) staff       (20)     7887 2024-04-14 01:33:25.686002 dbt_starrocks-1.6.2/PKG-INFO
+-rw-r--r--   0 lixueyan   (501) staff       (20)     6953 2024-04-13 00:45:40.000000 dbt_starrocks-1.6.2/README.md
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.617323 dbt_starrocks-1.6.2/dbt/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.616780 dbt_starrocks-1.6.2/dbt/adapters/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.643575 dbt_starrocks-1.6.2/dbt/adapters/starrocks/
+-rw-r--r--   0 lixueyan   (501) staff       (20)      968 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/adapters/starrocks/__init__.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)      647 2024-04-14 01:32:28.000000 dbt_starrocks-1.6.2/dbt/adapters/starrocks/__version__.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2002 2024-04-14 01:31:28.000000 dbt_starrocks-1.6.2/dbt/adapters/starrocks/column.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)     7538 2024-04-13 00:45:40.000000 dbt_starrocks-1.6.2/dbt/adapters/starrocks/connections.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)     6882 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/adapters/starrocks/impl.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)     3266 2024-04-14 01:31:28.000000 dbt_starrocks-1.6.2/dbt/adapters/starrocks/relation.py
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.617804 dbt_starrocks-1.6.2/dbt/include/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.651215 dbt_starrocks-1.6.2/dbt/include/starrocks/
+-rw-r--r--   0 lixueyan   (501) staff       (20)      680 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/__init__.py
+-rw-r--r--   0 lixueyan   (501) staff       (20)      687 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/dbt_project.yml
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.620740 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.662888 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2051 2024-04-14 01:31:28.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/columns.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      711 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/freshness.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     3585 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/metadata.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2054 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/relation.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     5197 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/relation_helpers.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      807 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/schema.sql
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.665315 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/get_custom_name/
+-rw-r--r--   0 lixueyan   (501) staff       (20)      754 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/get_custom_name/get_custom_database.sql
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.666089 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.669424 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/models/
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2631 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/models/materialized_view.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1511 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/models/table.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      846 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/models/view.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1648 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/seeds.sql
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.678715 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/snapshot/
+-rw-r--r--   0 lixueyan   (501) staff       (20)     5737 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1524 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      857 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/snapshot/strategies.sql
+-rw-r--r--   0 lixueyan   (501) staff       (20)      994 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/profile_template.yml
+-rw-r--r--   0 lixueyan   (501) staff       (20)      960 2024-03-13 02:34:38.000000 dbt_starrocks-1.6.2/dbt/include/starrocks/sample_profiles.yml
+drwxr-xr-x   0 lixueyan   (501) staff       (20)        0 2024-04-14 01:33:25.685024 dbt_starrocks-1.6.2/dbt_starrocks.egg-info/
+-rw-r--r--   0 lixueyan   (501) staff       (20)     7887 2024-04-14 01:33:25.000000 dbt_starrocks-1.6.2/dbt_starrocks.egg-info/PKG-INFO
+-rw-r--r--   0 lixueyan   (501) staff       (20)     1466 2024-04-14 01:33:25.000000 dbt_starrocks-1.6.2/dbt_starrocks.egg-info/SOURCES.txt
+-rw-r--r--   0 lixueyan   (501) staff       (20)        1 2024-04-14 01:33:25.000000 dbt_starrocks-1.6.2/dbt_starrocks.egg-info/dependency_links.txt
+-rw-r--r--   0 lixueyan   (501) staff       (20)        1 2024-04-14 01:33:25.000000 dbt_starrocks-1.6.2/dbt_starrocks.egg-info/not-zip-safe
+-rw-r--r--   0 lixueyan   (501) staff       (20)       44 2024-04-14 01:33:25.000000 dbt_starrocks-1.6.2/dbt_starrocks.egg-info/requires.txt
+-rw-r--r--   0 lixueyan   (501) staff       (20)        4 2024-04-14 01:33:25.000000 dbt_starrocks-1.6.2/dbt_starrocks.egg-info/top_level.txt
+-rw-r--r--   0 lixueyan   (501) staff       (20)       38 2024-04-14 01:33:25.688917 dbt_starrocks-1.6.2/setup.cfg
+-rw-r--r--   0 lixueyan   (501) staff       (20)     2773 2024-04-14 01:32:28.000000 dbt_starrocks-1.6.2/setup.py
```

### Comparing `dbt-starrocks-1.6.1/MANIFEST.in` & `dbt_starrocks-1.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/PKG-INFO` & `dbt_starrocks-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-starrocks
-Version: 1.6.1
+Version: 1.6.2
 Summary: The Starrocks adapter plugin for dbt
 Home-page: https://github.com/StarRocks/dbt-starrocks/
 Author: fujianhj, long2ice, astralidea
 Author-email: fujianhj@gmail.com, long2ice@gmail.com, astralidea@163.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -78,23 +78,26 @@
       host: localhost
       port: 9030
       schema: analytics
       username: your_starrocks_username
       password: your_starrocks_password
 ```
 
-| Option   | Description                                            | Required? | Example                        |
-|----------|--------------------------------------------------------|-----------|--------------------------------|
-| type     | The specific adapter to use                            | Required  | `starrocks`                    |
-| host     | The hostname to connect to                             | Required  | `192.168.100.28`               |
-| port     | The port to use                                        | Required  | `9030`                         |
-| schema   | Specify the schema (database) to build models into     | Required  | `analytics`                    |
-| username | The username to use to connect to the server           | Required  | `dbt_admin`                    |
-| password | The password to use for authenticating to the server   | Required  | `correct-horse-battery-staple` |
-| version  | Let Plugin try to go to a compatible starrocks version | Optional  | `3.1.0`                        |
+| Option   | Description                                             | Required? | Example                        |
+|----------|---------------------------------------------------------|-----------|--------------------------------|
+| type     | The specific adapter to use                             | Required  | `starrocks`                    |
+| host     | The hostname to connect to                              | Required  | `192.168.100.28`               |
+| port     | The port to use                                         | Required  | `9030`                         |
+| schema   | Specify the schema (database) to build models into      | Required  | `analytics`                    |
+| username | The username to use to connect to the server            | Required  | `dbt_admin`                    |
+| password | The password to use for authenticating to the server    | Required  | `correct-horse-battery-staple` |
+| version  | Let Plugin try to go to a compatible starrocks version  | Optional  | `3.1.0`                        |
+| ssl      | json string to specify SSL_MODE for the mysql connector | Optional  | `'{"ca": "path/to/ca.pem"}'`   |
+
+More details about configuring SSL_MODE for the connector [here](https://stackoverflow.com/questions/60285240/is-there-a-way-to-emulate-ssl-mode-preferred-in-pymysql)
 
 
 ## Example
 
 ### dbt seed properties(yml):
 #### Complete configuration:
 ```
```

### Comparing `dbt-starrocks-1.6.1/README.md` & `dbt_starrocks-1.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,23 +56,26 @@
       host: localhost
       port: 9030
       schema: analytics
       username: your_starrocks_username
       password: your_starrocks_password
 ```
 
-| Option   | Description                                            | Required? | Example                        |
-|----------|--------------------------------------------------------|-----------|--------------------------------|
-| type     | The specific adapter to use                            | Required  | `starrocks`                    |
-| host     | The hostname to connect to                             | Required  | `192.168.100.28`               |
-| port     | The port to use                                        | Required  | `9030`                         |
-| schema   | Specify the schema (database) to build models into     | Required  | `analytics`                    |
-| username | The username to use to connect to the server           | Required  | `dbt_admin`                    |
-| password | The password to use for authenticating to the server   | Required  | `correct-horse-battery-staple` |
-| version  | Let Plugin try to go to a compatible starrocks version | Optional  | `3.1.0`                        |
+| Option   | Description                                             | Required? | Example                        |
+|----------|---------------------------------------------------------|-----------|--------------------------------|
+| type     | The specific adapter to use                             | Required  | `starrocks`                    |
+| host     | The hostname to connect to                              | Required  | `192.168.100.28`               |
+| port     | The port to use                                         | Required  | `9030`                         |
+| schema   | Specify the schema (database) to build models into      | Required  | `analytics`                    |
+| username | The username to use to connect to the server            | Required  | `dbt_admin`                    |
+| password | The password to use for authenticating to the server    | Required  | `correct-horse-battery-staple` |
+| version  | Let Plugin try to go to a compatible starrocks version  | Optional  | `3.1.0`                        |
+| ssl      | json string to specify SSL_MODE for the mysql connector | Optional  | `'{"ca": "path/to/ca.pem"}'`   |
+
+More details about configuring SSL_MODE for the connector [here](https://stackoverflow.com/questions/60285240/is-there-a-way-to-emulate-ssl-mode-preferred-in-pymysql)
 
 
 ## Example
 
 ### dbt seed properties(yml):
 #### Complete configuration:
 ```
```

### Comparing `dbt-starrocks-1.6.1/dbt/adapters/starrocks/__init__.py` & `dbt_starrocks-1.6.2/dbt/adapters/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/adapters/starrocks/__version__.py` & `dbt_starrocks-1.6.2/dbt/adapters/starrocks/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = "1.6.1"
+version = "1.6.2"
```

### Comparing `dbt-starrocks-1.6.1/dbt/adapters/starrocks/column.py` & `dbt_starrocks-1.6.2/dbt/adapters/starrocks/column.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,18 @@
         return f"<StarRocksColumn {self.name} ({self.data_type})>"
 
     def is_string(self) -> bool:
         return self.dtype.lower() in ["text", "character varying", "character", "varchar",
                                       # starrocks
                                       "char", "string"]
 
+    @classmethod
+    def string_type(cls, size: int) -> str:
+        return "varchar({})".format(size)
+
     def is_float(self):
         return self.dtype.lower() in [
             # floats
             "real",
             "float4",
             "float",
             "double precision",
```

### Comparing `dbt-starrocks-1.6.1/dbt/adapters/starrocks/connections.py` & `dbt_starrocks-1.6.2/dbt/adapters/starrocks/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from contextlib import contextmanager
 
+import json
+from json import JSONDecodeError
+
 import mysql.connector
 
 import dbt.exceptions
 from dataclasses import dataclass
 
 from dbt.adapters.base import Credentials
 from dbt.adapters.sql import SQLConnectionManager
@@ -36,14 +39,15 @@
     catalog: Optional[str] = 'default_catalog'
     database: Optional[str] = None
     schema: Optional[str] = None
     username: Optional[str] = None
     password: Optional[str] = None
     charset: Optional[str] = None
     version: Optional[str] = None
+    ssl: Optional[str] = None
 
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def __post_init__(self):
         # starrocks classifies database and schema as the same thing
@@ -72,14 +76,15 @@
         """
         return (
             "host",
             "port",
             "schema",
             "catalog",
             "username",
+            "ssl",
         )
 
 
 def _parse_version(result):
     default_version = (999, 999, 999)
     first_part = None
 
@@ -107,14 +112,20 @@
                   "password": credentials.password, "database": credentials.catalog + "." + credentials.schema}
 
         kwargs["buffered"] = True
         
         if credentials.port:
             kwargs["port"] = credentials.port
 
+        if credentials.ssl:
+            try:
+                kwargs["ssl"] = json.loads(credentials.ssl)
+            except JSONDecodeError:
+                logger.debug("Failed to decode SSL config. Falling back to no SSL config.")
+
         try:
             connection.handle = mysql.connector.connect(**kwargs)
             connection.state = 'open'
         except mysql.connector.Error:
 
             try:
                 logger.debug("Failed connection without supplying the `database`. "
```

### Comparing `dbt-starrocks-1.6.1/dbt/adapters/starrocks/impl.py` & `dbt_starrocks-1.6.2/dbt/adapters/starrocks/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/adapters/starrocks/relation.py` & `dbt_starrocks-1.6.2/dbt/adapters/starrocks/relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,34 +16,41 @@
 from dataclasses import dataclass, field
 from typing import Optional, Type
 from dbt.adapters.base.relation import BaseRelation, Policy
 from dbt.exceptions import DbtRuntimeError
 from dbt.dataclass_schema import StrEnum
 from dbt.utils import classproperty
 
+
 @dataclass
 class StarRocksQuotePolicy(Policy):
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
+
 @dataclass
 class StarRocksIncludePolicy(Policy):
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
+
 class StarRocksRelationType(StrEnum):
     Table = "table"
     View = "view"
     MaterializedView = "materialized_view"
     SystemView = "system_view"
     CTE = "cte"
     Unknown = "unknown"
 
+
+type_map = {}
+
+
 @dataclass(frozen=True, eq=False, repr=False)
 class StarRocksRelation(BaseRelation):
     type: Optional[StarRocksRelationType] = None  # type: ignore
     include_policy: StarRocksIncludePolicy = field(default_factory=lambda: StarRocksIncludePolicy())
     quote_policy: StarRocksQuotePolicy = field(default_factory=lambda: StarRocksQuotePolicy())
     quote_character: str = "`"
 
@@ -74,10 +81,21 @@
     def render(self):
         if self.include_policy.database and self.include_policy.schema:
             raise DbtRuntimeError(
                 "Got a StarRocks relation with schema and database set to include, but only one can be set"
             )
         return super().render()
 
+    def init_type_map(self, desc_table):
+        for row in desc_table:
+            # name -> type
+            type_map[row[0]] = row[1]
+
+    def get_type_by_desc(self, row):
+        new_row = list(row)
+        # type
+        new_row[1] = type_map[row[0]]
+        return new_row
+
     @classproperty
     def get_relation_type(cls) -> Type[StarRocksRelationType]:
         return StarRocksRelationType
```

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/__init__.py` & `dbt_starrocks-1.6.2/dbt/include/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/dbt_project.yml` & `dbt_starrocks-1.6.2/dbt/include/starrocks/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/freshness.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/metadata.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/relation.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/relation_helpers.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/relation_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/adapters/schema.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/get_custom_name/get_custom_database.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/materialized_view.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/models/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/table.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/models/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/models/view.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/models/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/seeds.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/seeds.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/snapshot.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/snapshot_merge.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/macros/materializations/snapshot/strategies.sql` & `dbt_starrocks-1.6.2/dbt/include/starrocks/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/profile_template.yml` & `dbt_starrocks-1.6.2/dbt/include/starrocks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt/include/starrocks/sample_profiles.yml` & `dbt_starrocks-1.6.2/dbt/include/starrocks/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/dbt_starrocks.egg-info/PKG-INFO` & `dbt_starrocks-1.6.2/dbt_starrocks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-starrocks
-Version: 1.6.1
+Version: 1.6.2
 Summary: The Starrocks adapter plugin for dbt
 Home-page: https://github.com/StarRocks/dbt-starrocks/
 Author: fujianhj, long2ice, astralidea
 Author-email: fujianhj@gmail.com, long2ice@gmail.com, astralidea@163.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -78,23 +78,26 @@
       host: localhost
       port: 9030
       schema: analytics
       username: your_starrocks_username
       password: your_starrocks_password
 ```
 
-| Option   | Description                                            | Required? | Example                        |
-|----------|--------------------------------------------------------|-----------|--------------------------------|
-| type     | The specific adapter to use                            | Required  | `starrocks`                    |
-| host     | The hostname to connect to                             | Required  | `192.168.100.28`               |
-| port     | The port to use                                        | Required  | `9030`                         |
-| schema   | Specify the schema (database) to build models into     | Required  | `analytics`                    |
-| username | The username to use to connect to the server           | Required  | `dbt_admin`                    |
-| password | The password to use for authenticating to the server   | Required  | `correct-horse-battery-staple` |
-| version  | Let Plugin try to go to a compatible starrocks version | Optional  | `3.1.0`                        |
+| Option   | Description                                             | Required? | Example                        |
+|----------|---------------------------------------------------------|-----------|--------------------------------|
+| type     | The specific adapter to use                             | Required  | `starrocks`                    |
+| host     | The hostname to connect to                              | Required  | `192.168.100.28`               |
+| port     | The port to use                                         | Required  | `9030`                         |
+| schema   | Specify the schema (database) to build models into      | Required  | `analytics`                    |
+| username | The username to use to connect to the server            | Required  | `dbt_admin`                    |
+| password | The password to use for authenticating to the server    | Required  | `correct-horse-battery-staple` |
+| version  | Let Plugin try to go to a compatible starrocks version  | Optional  | `3.1.0`                        |
+| ssl      | json string to specify SSL_MODE for the mysql connector | Optional  | `'{"ca": "path/to/ca.pem"}'`   |
+
+More details about configuring SSL_MODE for the connector [here](https://stackoverflow.com/questions/60285240/is-there-a-way-to-emulate-ssl-mode-preferred-in-pymysql)
 
 
 ## Example
 
 ### dbt seed properties(yml):
 #### Complete configuration:
 ```
```

### Comparing `dbt-starrocks-1.6.1/dbt_starrocks.egg-info/SOURCES.txt` & `dbt_starrocks-1.6.2/dbt_starrocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-starrocks-1.6.1/setup.py` & `dbt_starrocks-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 # pull long description from README
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "dbt-starrocks"
 # make sure this always matches dbt/adapters/starrocks/__version__.py
-package_version = "1.6.1"
+package_version = "1.6.2"
 description = """The Starrocks adapter plugin for dbt"""
 
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

