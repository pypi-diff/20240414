# Comparing `tmp/rococo-1.0.7.tar.gz` & `tmp/rococo-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rococo-1.0.7.tar", last modified: Thu Apr 11 18:49:09 2024, max compression
+gzip compressed data, was "rococo-1.0.8.tar", last modified: Sat Apr 13 15:40:04 2024, max compression
```

## Comparing `rococo-1.0.7.tar` & `rococo-1.0.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.463189 rococo-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 18:49:05.000000 rococo-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-11 18:49:09.463189 rococo-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-04-11 18:49:05.000000 rococo-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.455190 rococo-1.0.7/rococo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.455190 rococo-1.0.7/rococo/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.455190 rococo-1.0.7/rococo/config/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.455190 rococo-1.0.7/rococo/data/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/data/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/data/surrealdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.459190 rococo-1.0.7/rococo/emailing/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/emailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/emailing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/emailing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/emailing/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/emailing/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/emailing/mailjet.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/emailing/ses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.459190 rococo-1.0.7/rococo/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/messaging/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/messaging/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.459190 rococo-1.0.7/rococo/models/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/login_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/otp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/person_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/recovery_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.463189 rococo-1.0.7/rococo/models/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/surrealdb/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/surrealdb/login_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/surrealdb/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/surrealdb/otp_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/surrealdb/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/surrealdb/person_organization_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/surrealdb/surreal_versioned_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/models/versioned_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.463189 rococo-1.0.7/rococo/repositories/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/base_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.463189 rococo-1.0.7/rococo/repositories/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/mysql/mysql_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/mysql/organization_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.463189 rococo-1.0.7/rococo/repositories/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/surrealdb/organization_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/surrealdb/person_organization_role_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-11 18:49:05.000000 rococo-1.0.7/rococo/repositories/surrealdb/surreal_db_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.463189 rococo-1.0.7/rococo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-11 18:49:09.000000 rococo-1.0.7/rococo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-11 18:49:09.000000 rococo-1.0.7/rococo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:49:09.000000 rococo-1.0.7/rococo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 18:49:09.000000 rococo-1.0.7/rococo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 18:49:09.000000 rococo-1.0.7/rococo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:49:09.463189 rococo-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-11 18:49:05.000000 rococo-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:09.463189 rococo-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:49:05.000000 rococo-1.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-11 18:49:05.000000 rococo-1.0.7/tests/base_repository_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-11 18:49:05.000000 rococo-1.0.7/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-11 18:49:05.000000 rococo-1.0.7/tests/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-11 18:49:05.000000 rococo-1.0.7/tests/surreal_db_repository_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.722430 rococo-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-13 15:39:59.000000 rococo-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-13 15:40:04.722430 rococo-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28462 2024-04-13 15:39:59.000000 rococo-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.710430 rococo-1.0.8/rococo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/data/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/data/surrealdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/emailing/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/mailjet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/emailing/ses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.714430 rococo-1.0.8/rococo/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/messaging/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/messaging/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.718430 rococo-1.0.8/rococo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/login_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/otp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/person_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/recovery_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.718430 rococo-1.0.8/rococo/models/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/login_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/otp_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/person_organization_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/surrealdb/surreal_versioned_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/models/versioned_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.718430 rococo-1.0.8/rococo/repositories/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/base_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.718430 rococo-1.0.8/rococo/repositories/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/mysql/mysql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/mysql/organization_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.722430 rococo-1.0.8/rococo/repositories/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/surrealdb/organization_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/surrealdb/person_organization_role_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12105 2024-04-13 15:39:59.000000 rococo-1.0.8/rococo/repositories/surrealdb/surreal_db_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.722430 rococo-1.0.8/rococo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28943 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-13 15:40:04.000000 rococo-1.0.8/rococo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:40:04.722430 rococo-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-13 15:39:59.000000 rococo-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:40:04.722430 rococo-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/base_repository_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-13 15:39:59.000000 rococo-1.0.8/tests/surreal_db_repository_test.py
```

### Comparing `rococo-1.0.7/LICENSE` & `rococo-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/PKG-INFO` & `rococo-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python library to help build things the way we want them built
 Home-page: https://github.com/EcorRouge/rococo
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rococo-1.0.7/README.md` & `rococo-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/auth/tokens.py` & `rococo-1.0.8/rococo/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/config/config.py` & `rococo-1.0.8/rococo/config/config.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/data/base.py` & `rococo-1.0.8/rococo/data/base.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/data/mysql.py` & `rococo-1.0.8/rococo/data/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,21 +77,15 @@
             return f"{key}='{str(value)}'"
         elif isinstance(value, type(None)):
             return f"{key} IS NULL"
         else:
             raise Exception(f"Unsupported type {type(value)} for condition key: {key}, value: {value}")
 
     def move_entity_to_audit_table(self, table, entity_id):
-        # Get the column names from the table
-        self._call_cursor('execute', f"SHOW COLUMNS FROM {table}")
-
-        column_list = ", ".join(column.get('Field') for column in self._cursor.fetchall())
-
-        query = f"""INSERT INTO {table}_audit ({column_list}) (SELECT {column_list} FROM {table} WHERE entity_id="{str(entity_id).replace('-', '')}");"""
-
+        query = f"""INSERT INTO {table}_audit (SELECT * FROM {table} WHERE entity_id="{str(entity_id).replace('-', '')}")"""
         self._call_cursor('execute', query)
         self._connection.commit()
 
     def execute_query(self, sql, _vars=None):
         """Executes a query against the DB."""
         if _vars is None:
             _vars = {}
```

### Comparing `rococo-1.0.7/rococo/data/surrealdb.py` & `rococo-1.0.8/rococo/data/surrealdb.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/emailing/config.py` & `rococo-1.0.8/rococo/emailing/config.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/emailing/factory.py` & `rococo-1.0.8/rococo/emailing/factory.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/emailing/mailjet.py` & `rococo-1.0.8/rococo/emailing/mailjet.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/messaging/base.py` & `rococo-1.0.8/rococo/messaging/base.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/messaging/rabbitmq.py` & `rococo-1.0.8/rococo/messaging/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/messaging/sqs.py` & `rococo-1.0.8/rococo/messaging/sqs.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/models/login_method.py` & `rococo-1.0.8/rococo/models/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/models/organization.py` & `rococo-1.0.8/rococo/models/organization.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/models/person_organization_role.py` & `rococo-1.0.8/rococo/models/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/models/surrealdb/login_method.py` & `rococo-1.0.8/rococo/models/surrealdb/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/models/surrealdb/organization.py` & `rococo-1.0.8/rococo/models/surrealdb/organization.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/models/surrealdb/person_organization_role.py` & `rococo-1.0.8/rococo/models/surrealdb/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/models/surrealdb/surreal_versioned_model.py` & `rococo-1.0.8/rococo/models/surrealdb/surreal_versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/models/versioned_model.py` & `rococo-1.0.8/rococo/models/versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/repositories/base_repository.py` & `rococo-1.0.8/rococo/repositories/base_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/repositories/mysql/mysql_repository.py` & `rococo-1.0.8/rococo/repositories/mysql/mysql_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/repositories/mysql/organization_repository.py` & `rococo-1.0.8/rococo/repositories/mysql/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/repositories/surrealdb/organization_repository.py` & `rococo-1.0.8/rococo/repositories/surrealdb/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/repositories/surrealdb/person_organization_role_repository.py` & `rococo-1.0.8/rococo/repositories/surrealdb/person_organization_role_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo/repositories/surrealdb/surreal_db_repository.py` & `rococo-1.0.8/rococo/repositories/surrealdb/surreal_db_repository.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/rococo.egg-info/PKG-INFO` & `rococo-1.0.8/rococo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python library to help build things the way we want them built
 Home-page: https://github.com/EcorRouge/rococo
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `rococo-1.0.7/rococo.egg-info/SOURCES.txt` & `rococo-1.0.8/rococo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/setup.py` & `rococo-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='rococo',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(),
     url='https://github.com/EcorRouge/rococo',
     license='MIT',
     author='Jay Grieves',
     author_email='jaygrieves@gmail.com',
     description='A Python library to help build things the way we want them built',
     long_description=open('README.md').read(),
```

### Comparing `rococo-1.0.7/tests/base_repository_test.py` & `rococo-1.0.8/tests/base_repository_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/tests/config_test.py` & `rococo-1.0.8/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/tests/model_test.py` & `rococo-1.0.8/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `rococo-1.0.7/tests/surreal_db_repository_test.py` & `rococo-1.0.8/tests/surreal_db_repository_test.py`

 * *Files identical despite different names*

