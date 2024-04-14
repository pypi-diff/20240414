# Comparing `tmp/gql-3.6.0b1.tar.gz` & `tmp/gql-3.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gql-3.6.0b1.tar", last modified: Thu Feb  8 22:47:41 2024, max compression
+gzip compressed data, was "gql-3.6.0b2.tar", last modified: Sun Apr 14 19:56:44 2024, max compression
```

## Comparing `gql-3.6.0b1.tar` & `gql-3.6.0b2.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.474928 gql-3.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-08 22:47:34.000000 gql-3.6.0b1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-08 22:47:34.000000 gql-3.6.0b1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-02-08 22:47:34.000000 gql-3.6.0b1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-08 22:47:34.000000 gql-3.6.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-08 22:47:34.000000 gql-3.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-08 22:47:34.000000 gql-3.6.0b1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-02-08 22:47:41.474928 gql-3.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-02-08 22:47:34.000000 gql-3.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.454928 gql-3.6.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.454928 gql-3.6.0b1/docs/advanced/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/advanced/async_advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/advanced/async_permanent_session.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/advanced/dsl_module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/advanced/error_handling.rst
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/advanced/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/advanced/local_schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/advanced/logging.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.454928 gql-3.6.0b1/docs/async/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/async/async_intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/async/async_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/async/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.454928 gql-3.6.0b1/docs/code_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/aiohttp_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/aiohttp_async_dsl.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/aiohttp_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.458928 gql-3.6.0b1/docs/code_examples/appsync/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/appsync/mutation_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/appsync/mutation_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/appsync/subscription_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/appsync/subscription_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/console_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/fastapi_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/httpx_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/httpx_async_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/httpx_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/phoenix_channel_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/reconnecting_mutation_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/reconnecting_mutation_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/reconnecting_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/requests_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/requests_sync_dsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/code_examples/websockets_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.458928 gql-3.6.0b1/docs/gql-cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/gql-cli/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.458928 gql-3.6.0b1/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/client.rst
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/dsl.rst
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/gql.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport.rst
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_appsync_auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_appsync_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_httpx.rst
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_phoenix_channel_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_requests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/transport_websockets_base.rst
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/modules/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.458928 gql-3.6.0b1/docs/transports/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/appsync.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/async_transports.rst
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/httpx.rst
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/httpx_async.rst
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/phoenix.rst
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/requests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/sync_transports.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/transports/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.462928 gql-3.6.0b1/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/custom_scalars_and_enums.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/file_upload.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/headers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/subscriptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/validation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-08 22:47:34.000000 gql-3.6.0b1/docs/usage/variables.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.462928 gql-3.6.0b1/gql/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16695 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    66602 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    36862 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/dsl.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/graphql_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.466929 gql-3.6.0b1/gql/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/appsync_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/appsync_websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/async_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/local_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/phoenix_channel_websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24466 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/transport/websockets_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.466929 gql-3.6.0b1/gql/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utilities/build_client_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utilities/get_introspection_query_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utilities/node_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utilities/parse_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utilities/serialize_variable_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utilities/update_schema_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utilities/update_schema_scalars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-02-08 22:47:34.000000 gql-3.6.0b1/gql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.462928 gql-3.6.0b1/gql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-02-08 22:47:41.000000 gql-3.6.0b1/gql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-02-08 22:47:41.000000 gql-3.6.0b1/gql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 22:47:41.000000 gql-3.6.0b1/gql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-08 22:47:41.000000 gql-3.6.0b1/gql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 22:47:41.000000 gql-3.6.0b1/gql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-08 22:47:41.000000 gql-3.6.0b1/gql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-08 22:47:41.000000 gql-3.6.0b1/gql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-08 22:47:41.474928 gql-3.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-02-08 22:47:34.000000 gql-3.6.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.470929 gql-3.6.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.470929 gql-3.6.0b1/tests/custom_scalars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/custom_scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/custom_scalars/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/custom_scalars/test_enum_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/custom_scalars/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    22448 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/custom_scalars/test_money.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/custom_scalars/test_parse_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.470929 gql-3.6.0b1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.470929 gql-3.6.0b1/tests/fixtures/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/aws/fake_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/aws/fake_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/aws/fake_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/aws/fake_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.470929 gql-3.6.0b1/tests/fixtures/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/graphql/sample.graphql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.470929 gql-3.6.0b1/tests/fixtures/vcr_cassettes/
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/vcr_cassettes/client.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    78820 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/vcr_cassettes/queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    78836 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/fixtures/vcr_cassettes/queries_batch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.474928 gql-3.6.0b1/tests/nested_input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/nested_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/nested_input/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/nested_input/test_nested_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.450929 gql-3.6.0b1/tests/regressions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.474928 gql-3.6.0b1/tests/regressions/issue_447_dsl_missing_directives/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/regressions/issue_447_dsl_missing_directives/test_dsl_directives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:41.474928 gql-3.6.0b1/tests/starwars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    29968 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/test_dsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/test_parse_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/starwars/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    44492 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_aiohttp_online.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_appsync_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_appsync_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    24177 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_appsync_websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_async_client_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_graphql_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_graphqlws_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27257 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_graphqlws_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_http_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    26548 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)    39814 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_httpx_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_httpx_online.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_localhost.cnf
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_localhost.pem
--rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_phoenix_channel_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_phoenix_channel_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_phoenix_channel_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    29559 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_requests_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_transport_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_websocket_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_websocket_online.py
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_websocket_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-02-08 22:47:34.000000 gql-3.6.0b1/tests/test_websocket_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-08 22:47:34.000000 gql-3.6.0b1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.372570 gql-3.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-14 19:56:42.000000 gql-3.6.0b2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-14 19:56:42.000000 gql-3.6.0b2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-14 19:56:42.000000 gql-3.6.0b2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-14 19:56:42.000000 gql-3.6.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 19:56:42.000000 gql-3.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-14 19:56:42.000000 gql-3.6.0b2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-14 19:56:44.372570 gql-3.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-14 19:56:42.000000 gql-3.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.352570 gql-3.6.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.352570 gql-3.6.0b2/docs/advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/advanced/async_advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/advanced/async_permanent_session.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/advanced/dsl_module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/advanced/error_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/advanced/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/advanced/local_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/advanced/logging.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.352570 gql-3.6.0b2/docs/async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/async/async_intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/async/async_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/async/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.356570 gql-3.6.0b2/docs/code_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/aiohttp_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/aiohttp_async_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/aiohttp_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.356570 gql-3.6.0b2/docs/code_examples/appsync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/appsync/mutation_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/appsync/mutation_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/appsync/subscription_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/appsync/subscription_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/console_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/fastapi_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/httpx_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/httpx_async_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/httpx_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/phoenix_channel_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/reconnecting_mutation_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/reconnecting_mutation_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/reconnecting_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/requests_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/requests_sync_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/code_examples/websockets_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.356570 gql-3.6.0b2/docs/gql-cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/gql-cli/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.356570 gql-3.6.0b2/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/dsl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/gql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_appsync_auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_appsync_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_httpx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_phoenix_channel_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_requests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/transport_websockets_base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/modules/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.360570 gql-3.6.0b2/docs/transports/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/appsync.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/async_transports.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/httpx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/httpx_async.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/phoenix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/requests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/sync_transports.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/transports/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.360570 gql-3.6.0b2/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/custom_scalars_and_enums.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/file_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/headers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/subscriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/validation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-14 19:56:42.000000 gql-3.6.0b2/docs/usage/variables.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.360570 gql-3.6.0b2/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16695 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66602 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36862 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/graphql_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.364570 gql-3.6.0b2/gql/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/appsync_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/appsync_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/async_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/local_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/phoenix_channel_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24466 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/transport/websockets_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.364570 gql-3.6.0b2/gql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utilities/build_client_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utilities/get_introspection_query_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utilities/node_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utilities/parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utilities/serialize_variable_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utilities/update_schema_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utilities/update_schema_scalars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-14 19:56:42.000000 gql-3.6.0b2/gql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.364570 gql-3.6.0b2/gql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-14 19:56:44.000000 gql-3.6.0b2/gql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-14 19:56:44.000000 gql-3.6.0b2/gql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:56:44.000000 gql-3.6.0b2/gql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-14 19:56:44.000000 gql-3.6.0b2/gql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:56:44.000000 gql-3.6.0b2/gql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-14 19:56:44.000000 gql-3.6.0b2/gql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-14 19:56:44.000000 gql-3.6.0b2/gql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-14 19:56:44.372570 gql-3.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-14 19:56:42.000000 gql-3.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.368570 gql-3.6.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15436 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.368570 gql-3.6.0b2/tests/custom_scalars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/custom_scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/custom_scalars/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/custom_scalars/test_enum_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/custom_scalars/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22448 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/custom_scalars/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/custom_scalars/test_parse_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.368570 gql-3.6.0b2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.372570 gql-3.6.0b2/tests/fixtures/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/aws/fake_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/aws/fake_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/aws/fake_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/aws/fake_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.372570 gql-3.6.0b2/tests/fixtures/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/graphql/sample.graphql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.372570 gql-3.6.0b2/tests/fixtures/vcr_cassettes/
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/vcr_cassettes/client.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    78820 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/vcr_cassettes/queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    78836 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/fixtures/vcr_cassettes/queries_batch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.372570 gql-3.6.0b2/tests/nested_input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/nested_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/nested_input/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/nested_input/test_nested_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.348570 gql-3.6.0b2/tests/regressions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.372570 gql-3.6.0b2/tests/regressions/issue_447_dsl_missing_directives/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/regressions/issue_447_dsl_missing_directives/test_dsl_directives.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:44.372570 gql-3.6.0b2/tests/starwars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29968 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/test_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/test_parse_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/starwars/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44492 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_aiohttp_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_appsync_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_appsync_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24177 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_appsync_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7303 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_async_client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12020 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_graphql_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_graphqlws_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27257 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_graphqlws_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_http_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26548 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39814 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_httpx_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_httpx_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_localhost.cnf
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_localhost.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    15131 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_phoenix_channel_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_phoenix_channel_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_phoenix_channel_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29559 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_requests_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_transport_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_websocket_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_websocket_online.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_websocket_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-14 19:56:42.000000 gql-3.6.0b2/tests/test_websocket_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-14 19:56:42.000000 gql-3.6.0b2/tox.ini
```

### Comparing `gql-3.6.0b1/.readthedocs.yaml` & `gql-3.6.0b2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/CONTRIBUTING.md` & `gql-3.6.0b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/LICENSE` & `gql-3.6.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/Makefile` & `gql-3.6.0b2/Makefile`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/PKG-INFO` & `gql-3.6.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql
-Version: 3.6.0b1
+Version: 3.6.0b2
 Summary: GraphQL client for Python
 Home-page: https://github.com/graphql-python/gql
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Description: # GQL
```

### Comparing `gql-3.6.0b1/README.md` & `gql-3.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/Makefile` & `gql-3.6.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/advanced/async_advanced_usage.rst` & `gql-3.6.0b2/docs/advanced/async_advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/advanced/async_permanent_session.rst` & `gql-3.6.0b2/docs/advanced/async_permanent_session.rst`

 * *Files 4% similar despite different names*

```diff
@@ -71,23 +71,34 @@
 .. code-block:: python
 
     # Here Only 3 tries for execute calls
     retry_execute = backoff.on_exception(
         backoff.expo,
         Exception,
         max_tries=3,
-        giveup=lambda e: isinstance(e, TransportQueryError),
     )
     session = await client.connect_async(
         reconnecting=True,
         retry_execute=retry_execute,
     )
 
 If you don't want any retry on the execute calls, you can disable the retries with :code:`retry_execute=False`
 
+.. note::
+    If you want to retry even with :code:`TransportQueryError` exceptions,
+    then you need to make your own backoff decorator on your own method:
+
+    .. code-block:: python
+
+        @backoff.on_exception(backoff.expo,
+                              Exception,
+                              max_tries=3)
+        async def execute_with_retry(session, query):
+            return await session.execute(query)
+
 Subscription retries
 ^^^^^^^^^^^^^^^^^^^^
 
 There is no :code:`retry_subscribe` as it is not feasible with async generators.
 If you want retries for your subscriptions, then you can do it yourself
 with backoff decorators on your methods.
```

### Comparing `gql-3.6.0b1/docs/advanced/dsl_module.rst` & `gql-3.6.0b2/docs/advanced/dsl_module.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/advanced/error_handling.rst` & `gql-3.6.0b2/docs/advanced/error_handling.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/advanced/local_schema.rst` & `gql-3.6.0b2/docs/advanced/local_schema.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/advanced/logging.rst` & `gql-3.6.0b2/docs/advanced/logging.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/async/async_intro.rst` & `gql-3.6.0b2/docs/async/async_intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/async/async_usage.rst` & `gql-3.6.0b2/docs/async/async_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/aiohttp_async.py` & `gql-3.6.0b2/docs/code_examples/aiohttp_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/aiohttp_async_dsl.py` & `gql-3.6.0b2/docs/code_examples/aiohttp_async_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/aiohttp_sync.py` & `gql-3.6.0b2/docs/code_examples/aiohttp_sync.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/appsync/mutation_api_key.py` & `gql-3.6.0b2/docs/code_examples/appsync/mutation_api_key.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/appsync/mutation_iam.py` & `gql-3.6.0b2/docs/code_examples/appsync/mutation_iam.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/appsync/subscription_api_key.py` & `gql-3.6.0b2/docs/code_examples/appsync/subscription_api_key.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/appsync/subscription_iam.py` & `gql-3.6.0b2/docs/code_examples/appsync/subscription_iam.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/console_async.py` & `gql-3.6.0b2/docs/code_examples/console_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/fastapi_async.py` & `gql-3.6.0b2/docs/code_examples/fastapi_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/httpx_async.py` & `gql-3.6.0b2/docs/code_examples/httpx_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/httpx_async_trio.py` & `gql-3.6.0b2/docs/code_examples/httpx_async_trio.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/phoenix_channel_async.py` & `gql-3.6.0b2/docs/code_examples/phoenix_channel_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/reconnecting_mutation_http.py` & `gql-3.6.0b2/docs/code_examples/reconnecting_mutation_http.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/reconnecting_mutation_ws.py` & `gql-3.6.0b2/docs/code_examples/reconnecting_mutation_ws.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/reconnecting_subscription.py` & `gql-3.6.0b2/docs/code_examples/reconnecting_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/requests_sync_dsl.py` & `gql-3.6.0b2/docs/code_examples/requests_sync_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/code_examples/websockets_async.py` & `gql-3.6.0b2/docs/code_examples/websockets_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/conf.py` & `gql-3.6.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/gql-cli/intro.rst` & `gql-3.6.0b2/docs/gql-cli/intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/intro.rst` & `gql-3.6.0b2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/make.bat` & `gql-3.6.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/transports/aiohttp.rst` & `gql-3.6.0b2/docs/transports/aiohttp.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/transports/appsync.rst` & `gql-3.6.0b2/docs/transports/appsync.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/transports/httpx_async.rst` & `gql-3.6.0b2/docs/transports/httpx_async.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/transports/phoenix.rst` & `gql-3.6.0b2/docs/transports/phoenix.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/transports/websockets.rst` & `gql-3.6.0b2/docs/transports/websockets.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/usage/basic_usage.rst` & `gql-3.6.0b2/docs/usage/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/usage/custom_scalars_and_enums.rst` & `gql-3.6.0b2/docs/usage/custom_scalars_and_enums.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/usage/extensions.rst` & `gql-3.6.0b2/docs/usage/extensions.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/usage/file_upload.rst` & `gql-3.6.0b2/docs/usage/file_upload.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/usage/subscriptions.rst` & `gql-3.6.0b2/docs/usage/subscriptions.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/usage/validation.rst` & `gql-3.6.0b2/docs/usage/validation.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/docs/usage/variables.rst` & `gql-3.6.0b2/docs/usage/variables.rst`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/__init__.py` & `gql-3.6.0b2/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/cli.py` & `gql-3.6.0b2/gql/cli.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/client.py` & `gql-3.6.0b2/gql/client.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/dsl.py` & `gql-3.6.0b2/gql/dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/gql.py` & `gql-3.6.0b2/gql/gql.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/graphql_request.py` & `gql-3.6.0b2/gql/graphql_request.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/aiohttp.py` & `gql-3.6.0b2/gql/transport/aiohttp.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/appsync_auth.py` & `gql-3.6.0b2/gql/transport/appsync_auth.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/appsync_websockets.py` & `gql-3.6.0b2/gql/transport/appsync_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/async_transport.py` & `gql-3.6.0b2/gql/transport/async_transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/exceptions.py` & `gql-3.6.0b2/gql/transport/exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/httpx.py` & `gql-3.6.0b2/gql/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/local_schema.py` & `gql-3.6.0b2/gql/transport/local_schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/phoenix_channel_websockets.py` & `gql-3.6.0b2/gql/transport/phoenix_channel_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/requests.py` & `gql-3.6.0b2/gql/transport/requests.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/transport.py` & `gql-3.6.0b2/gql/transport/transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/websockets.py` & `gql-3.6.0b2/gql/transport/websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/transport/websockets_base.py` & `gql-3.6.0b2/gql/transport/websockets_base.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/utilities/__init__.py` & `gql-3.6.0b2/gql/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/utilities/build_client_schema.py` & `gql-3.6.0b2/gql/utilities/build_client_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-from graphql import GraphQLSchema, IntrospectionQuery
+from graphql import DirectiveLocation, GraphQLSchema, IntrospectionQuery
 from graphql import build_client_schema as build_client_schema_orig
 from graphql.pyutils import inspect
-from graphql.utilities.get_introspection_query import (
-    DirectiveLocation,
-    IntrospectionDirective,
-)
+from graphql.utilities.get_introspection_query import IntrospectionDirective
 
 __all__ = ["build_client_schema"]
 
 
 INCLUDE_DIRECTIVE_JSON: IntrospectionDirective = {
     "name": "include",
     "description": (
```

### Comparing `gql-3.6.0b1/gql/utilities/get_introspection_query_ast.py` & `gql-3.6.0b2/gql/utilities/get_introspection_query_ast.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/utilities/node_tree.py` & `gql-3.6.0b2/gql/utilities/node_tree.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/utilities/parse_result.py` & `gql-3.6.0b2/gql/utilities/parse_result.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/utilities/serialize_variable_values.py` & `gql-3.6.0b2/gql/utilities/serialize_variable_values.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/utilities/update_schema_enum.py` & `gql-3.6.0b2/gql/utilities/update_schema_enum.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/utilities/update_schema_scalars.py` & `gql-3.6.0b2/gql/utilities/update_schema_scalars.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql/utils.py` & `gql-3.6.0b2/gql/utils.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql.egg-info/PKG-INFO` & `gql-3.6.0b2/gql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql
-Version: 3.6.0b1
+Version: 3.6.0b2
 Summary: GraphQL client for Python
 Home-page: https://github.com/graphql-python/gql
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Description: # GQL
```

### Comparing `gql-3.6.0b1/gql.egg-info/SOURCES.txt` & `gql-3.6.0b2/gql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/gql.egg-info/requires.txt` & `gql-3.6.0b2/gql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/setup.py` & `gql-3.6.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/conftest.py` & `gql-3.6.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/custom_scalars/test_datetime.py` & `gql-3.6.0b2/tests/custom_scalars/test_datetime.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/custom_scalars/test_enum_colors.py` & `gql-3.6.0b2/tests/custom_scalars/test_enum_colors.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/custom_scalars/test_json.py` & `gql-3.6.0b2/tests/custom_scalars/test_json.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/custom_scalars/test_money.py` & `gql-3.6.0b2/tests/custom_scalars/test_money.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/custom_scalars/test_parse_results.py` & `gql-3.6.0b2/tests/custom_scalars/test_parse_results.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/fixtures/aws/fake_credentials.py` & `gql-3.6.0b2/tests/fixtures/aws/fake_credentials.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/fixtures/aws/fake_request.py` & `gql-3.6.0b2/tests/fixtures/aws/fake_request.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/fixtures/aws/fake_session.py` & `gql-3.6.0b2/tests/fixtures/aws/fake_session.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/fixtures/aws/fake_signer.py` & `gql-3.6.0b2/tests/fixtures/aws/fake_signer.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/fixtures/vcr_cassettes/client.yaml` & `gql-3.6.0b2/tests/fixtures/vcr_cassettes/client.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/fixtures/vcr_cassettes/queries.yaml` & `gql-3.6.0b2/tests/fixtures/vcr_cassettes/queries.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/fixtures/vcr_cassettes/queries_batch.yaml` & `gql-3.6.0b2/tests/fixtures/vcr_cassettes/queries_batch.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/nested_input/schema.py` & `gql-3.6.0b2/tests/nested_input/schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/nested_input/test_nested_input.py` & `gql-3.6.0b2/tests/nested_input/test_nested_input.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/regressions/issue_447_dsl_missing_directives/test_dsl_directives.py` & `gql-3.6.0b2/tests/regressions/issue_447_dsl_missing_directives/test_dsl_directives.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/starwars/fixtures.py` & `gql-3.6.0b2/tests/starwars/fixtures.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/starwars/schema.py` & `gql-3.6.0b2/tests/starwars/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,25 +172,25 @@
             args={
                 "episode": GraphQLArgument(
                     episode_enum,
                     description="If omitted, returns the hero of the whole saga. If "
                     "provided, returns the hero of that particular episode.",
                 )
             },
-            resolve=lambda _souce, _info, episode=None: get_hero_async(episode),
+            resolve=lambda _source, _info, episode=None: get_hero_async(episode),
         ),
         "human": GraphQLField(
             human_type,
             args={
                 "id": GraphQLArgument(
                     description="id of the human",
                     type_=GraphQLNonNull(GraphQLString),
                 )
             },
-            resolve=lambda _souce, _info, id: get_human(id),
+            resolve=lambda _source, _info, id: get_human(id),
         ),
         "droid": GraphQLField(
             droid_type,
             args={
                 "id": GraphQLArgument(
                     description="id of the droid",
                     type_=GraphQLNonNull(GraphQLString),
```

### Comparing `gql-3.6.0b1/tests/starwars/test_dsl.py` & `gql-3.6.0b2/tests/starwars/test_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/starwars/test_introspection.py` & `gql-3.6.0b2/tests/starwars/test_introspection.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/starwars/test_parse_results.py` & `gql-3.6.0b2/tests/starwars/test_parse_results.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/starwars/test_query.py` & `gql-3.6.0b2/tests/starwars/test_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/starwars/test_subscription.py` & `gql-3.6.0b2/tests/starwars/test_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/starwars/test_validation.py` & `gql-3.6.0b2/tests/starwars/test_validation.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_aiohttp.py` & `gql-3.6.0b2/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_aiohttp_online.py` & `gql-3.6.0b2/tests/test_aiohttp_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_appsync_auth.py` & `gql-3.6.0b2/tests/test_appsync_auth.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_appsync_http.py` & `gql-3.6.0b2/tests/test_appsync_http.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_appsync_websockets.py` & `gql-3.6.0b2/tests/test_appsync_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_async_client_validation.py` & `gql-3.6.0b2/tests/test_async_client_validation.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_cli.py` & `gql-3.6.0b2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_client.py` & `gql-3.6.0b2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_graphql_request.py` & `gql-3.6.0b2/tests/test_graphql_request.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_graphqlws_exceptions.py` & `gql-3.6.0b2/tests/test_graphqlws_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_graphqlws_subscription.py` & `gql-3.6.0b2/tests/test_graphqlws_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_http_async_sync.py` & `gql-3.6.0b2/tests/test_http_async_sync.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_httpx.py` & `gql-3.6.0b2/tests/test_httpx.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_httpx_async.py` & `gql-3.6.0b2/tests/test_httpx_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_httpx_online.py` & `gql-3.6.0b2/tests/test_httpx_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_localhost.pem` & `gql-3.6.0b2/tests/test_localhost.pem`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_phoenix_channel_exceptions.py` & `gql-3.6.0b2/tests/test_phoenix_channel_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_phoenix_channel_query.py` & `gql-3.6.0b2/tests/test_phoenix_channel_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_phoenix_channel_subscription.py` & `gql-3.6.0b2/tests/test_phoenix_channel_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_requests.py` & `gql-3.6.0b2/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_requests_batch.py` & `gql-3.6.0b2/tests/test_requests_batch.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_transport.py` & `gql-3.6.0b2/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_transport_batch.py` & `gql-3.6.0b2/tests/test_transport_batch.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_websocket_exceptions.py` & `gql-3.6.0b2/tests/test_websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_websocket_online.py` & `gql-3.6.0b2/tests/test_websocket_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_websocket_query.py` & `gql-3.6.0b2/tests/test_websocket_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tests/test_websocket_subscription.py` & `gql-3.6.0b2/tests/test_websocket_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.6.0b1/tox.ini` & `gql-3.6.0b2/tox.ini`

 * *Files identical despite different names*

