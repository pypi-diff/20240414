# Comparing `tmp/gs2-1.1.98.tar.gz` & `tmp/gs2-1.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs2-1.1.98.tar", last modified: Mon Jan 15 12:02:23 2024, max compression
+gzip compressed data, was "gs2-1.1.99.tar", last modified: Tue Jan 16 07:30:24 2024, max compression
```

## Comparing `gs2-1.1.98.tar` & `gs2-1.1.99.tar`

### file list

```diff
@@ -1,324 +1,324 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.509630 gs2-1.1.98/
--rw-r--r--   0 root         (0) root         (0)      365 2024-01-15 12:02:23.509630 gs2-1.1.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-15 12:02:23.509630 gs2-1.1.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1385 2024-01-15 12:00:57.000000 gs2-1.1.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.453630 gs2-1.1.98/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.453630 gs2-1.1.98/src/gs2/
--rw-r--r--   0 root         (0) root         (0)      957 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.457630 gs2-1.1.98/src/gs2/account/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/account/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23808 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/account/model.py
--rw-r--r--   0 root         (0) root         (0)    58434 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/account/request.py
--rw-r--r--   0 root         (0) root         (0)    86019 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/account/rest.py
--rw-r--r--   0 root         (0) root         (0)    34900 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/account/result.py
--rw-r--r--   0 root         (0) root         (0)    82616 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/account/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.457630 gs2-1.1.98/src/gs2/ad_reward/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ad_reward/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13431 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ad_reward/model.py
--rw-r--r--   0 root         (0) root         (0)    29108 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ad_reward/request.py
--rw-r--r--   0 root         (0) root         (0)    48335 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ad_reward/rest.py
--rw-r--r--   0 root         (0) root         (0)    19275 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ad_reward/result.py
--rw-r--r--   0 root         (0) root         (0)    46908 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ad_reward/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.457630 gs2-1.1.98/src/gs2/auth/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2133 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/auth/model.py
--rw-r--r--   0 root         (0) root         (0)     3054 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/auth/request.py
--rw-r--r--   0 root         (0) root         (0)     4777 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/auth/rest.py
--rw-r--r--   0 root         (0) root         (0)     3127 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/auth/result.py
--rw-r--r--   0 root         (0) root         (0)     4771 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/auth/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.457630 gs2-1.1.98/src/gs2/chat/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/chat/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26559 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/chat/model.py
--rw-r--r--   0 root         (0) root         (0)    74045 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/chat/request.py
--rw-r--r--   0 root         (0) root         (0)    96717 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/chat/rest.py
--rw-r--r--   0 root         (0) root         (0)    37494 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/chat/result.py
--rw-r--r--   0 root         (0) root         (0)    93168 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/chat/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.461630 gs2-1.1.98/src/gs2/core/
--rw-r--r--   0 root         (0) root         (0)      188 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.461630 gs2-1.1.98/src/gs2/core/domain/
--rw-r--r--   0 root         (0) root         (0)    10812 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/core/domain/__init__.py
--rw-r--r--   0 root         (0) root         (0)      274 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/core/domain/access_token.py
--rw-r--r--   0 root         (0) root         (0)     3658 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     6581 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/core/model.py
--rw-r--r--   0 root         (0) root         (0)    10580 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/core/rest.py
--rw-r--r--   0 root         (0) root         (0)     1233 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/core/util.py
--rw-r--r--   0 root         (0) root         (0)    10955 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/core/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.461630 gs2-1.1.98/src/gs2/datastore/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/datastore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18306 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/datastore/model.py
--rw-r--r--   0 root         (0) root         (0)    67152 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/datastore/request.py
--rw-r--r--   0 root         (0) root         (0)    95350 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/datastore/rest.py
--rw-r--r--   0 root         (0) root         (0)    42722 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/datastore/result.py
--rw-r--r--   0 root         (0) root         (0)    92263 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/datastore/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.461630 gs2-1.1.98/src/gs2/deploy/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/deploy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21252 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/deploy/model.py
--rw-r--r--   0 root         (0) root         (0)    22585 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/deploy/request.py
--rw-r--r--   0 root         (0) root         (0)    40756 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/deploy/rest.py
--rw-r--r--   0 root         (0) root         (0)    19223 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/deploy/result.py
--rw-r--r--   0 root         (0) root         (0)    39142 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/deploy/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.465630 gs2-1.1.98/src/gs2/dictionary/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/dictionary/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24080 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/dictionary/model.py
--rw-r--r--   0 root         (0) root         (0)    54194 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/dictionary/request.py
--rw-r--r--   0 root         (0) root         (0)    88429 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/dictionary/rest.py
--rw-r--r--   0 root         (0) root         (0)    37924 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/dictionary/result.py
--rw-r--r--   0 root         (0) root         (0)    85207 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/dictionary/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.465630 gs2-1.1.98/src/gs2/distributor/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/distributor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30989 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/distributor/model.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/distributor/request.py
--rw-r--r--   0 root         (0) root         (0)    63369 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/distributor/rest.py
--rw-r--r--   0 root         (0) root         (0)    29638 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/distributor/result.py
--rw-r--r--   0 root         (0) root         (0)    61505 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/distributor/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.469630 gs2-1.1.98/src/gs2/enchant/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enchant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54270 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enchant/model.py
--rw-r--r--   0 root         (0) root         (0)    94626 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enchant/request.py
--rw-r--r--   0 root         (0) root         (0)   137241 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enchant/rest.py
--rw-r--r--   0 root         (0) root         (0)    59909 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enchant/result.py
--rw-r--r--   0 root         (0) root         (0)   132555 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enchant/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.469630 gs2-1.1.98/src/gs2/enhance/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enhance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46945 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enhance/model.py
--rw-r--r--   0 root         (0) root         (0)    86426 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enhance/request.py
--rw-r--r--   0 root         (0) root         (0)   116825 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enhance/rest.py
--rw-r--r--   0 root         (0) root         (0)    61187 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enhance/result.py
--rw-r--r--   0 root         (0) root         (0)   113147 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/enhance/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.469630 gs2-1.1.98/src/gs2/exchange/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/exchange/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48528 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/exchange/model.py
--rw-r--r--   0 root         (0) root         (0)    95983 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/exchange/request.py
--rw-r--r--   0 root         (0) root         (0)   130421 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/exchange/rest.py
--rw-r--r--   0 root         (0) root         (0)    66629 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/exchange/result.py
--rw-r--r--   0 root         (0) root         (0)   125924 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/exchange/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.473630 gs2-1.1.98/src/gs2/experience/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/experience/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42324 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/experience/model.py
--rw-r--r--   0 root         (0) root         (0)    97516 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/experience/request.py
--rw-r--r--   0 root         (0) root         (0)   136459 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/experience/rest.py
--rw-r--r--   0 root         (0) root         (0)    57549 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/experience/result.py
--rw-r--r--   0 root         (0) root         (0)   130825 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/experience/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.473630 gs2-1.1.98/src/gs2/formation/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/formation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61465 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/formation/model.py
--rw-r--r--   0 root         (0) root         (0)   125462 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/formation/request.py
--rw-r--r--   0 root         (0) root         (0)   180533 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/formation/rest.py
--rw-r--r--   0 root         (0) root         (0)    94604 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/formation/result.py
--rw-r--r--   0 root         (0) root         (0)   172509 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/formation/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.473630 gs2-1.1.98/src/gs2/friend/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/friend/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44859 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/friend/model.py
--rw-r--r--   0 root         (0) root         (0)    96861 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/friend/request.py
--rw-r--r--   0 root         (0) root         (0)   134753 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/friend/rest.py
--rw-r--r--   0 root         (0) root         (0)    54985 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/friend/result.py
--rw-r--r--   0 root         (0) root         (0)   129941 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/friend/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.477630 gs2-1.1.98/src/gs2/gateway/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/gateway/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13754 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/gateway/model.py
--rw-r--r--   0 root         (0) root         (0)    39264 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/gateway/request.py
--rw-r--r--   0 root         (0) root         (0)    63586 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/gateway/rest.py
--rw-r--r--   0 root         (0) root         (0)    25524 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/gateway/result.py
--rw-r--r--   0 root         (0) root         (0)    61650 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/gateway/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.477630 gs2-1.1.98/src/gs2/grade/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/grade/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37287 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/grade/model.py
--rw-r--r--   0 root         (0) root         (0)    76293 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/grade/request.py
--rw-r--r--   0 root         (0) root         (0)   109392 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/grade/rest.py
--rw-r--r--   0 root         (0) root         (0)    51920 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/grade/result.py
--rw-r--r--   0 root         (0) root         (0)   105064 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/grade/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.477630 gs2-1.1.98/src/gs2/identifier/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/identifier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14333 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/identifier/model.py
--rw-r--r--   0 root         (0) root         (0)    27417 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/identifier/request.py
--rw-r--r--   0 root         (0) root         (0)    51631 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/identifier/rest.py
--rw-r--r--   0 root         (0) root         (0)    26226 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/identifier/result.py
--rw-r--r--   0 root         (0) root         (0)    49813 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/identifier/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.477630 gs2-1.1.98/src/gs2/idle/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/idle/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34135 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/idle/model.py
--rw-r--r--   0 root         (0) root         (0)    57207 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/idle/request.py
--rw-r--r--   0 root         (0) root         (0)    86289 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/idle/rest.py
--rw-r--r--   0 root         (0) root         (0)    39558 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/idle/result.py
--rw-r--r--   0 root         (0) root         (0)    83280 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/idle/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.481630 gs2-1.1.98/src/gs2/inbox/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40566 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inbox/model.py
--rw-r--r--   0 root         (0) root         (0)    71136 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inbox/request.py
--rw-r--r--   0 root         (0) root         (0)   103104 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inbox/rest.py
--rw-r--r--   0 root         (0) root         (0)    44816 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inbox/result.py
--rw-r--r--   0 root         (0) root         (0)    99616 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inbox/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.481630 gs2-1.1.98/src/gs2/inventory/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inventory/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104288 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inventory/model.py
--rw-r--r--   0 root         (0) root         (0)   238236 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inventory/request.py
--rw-r--r--   0 root         (0) root         (0)   336372 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inventory/rest.py
--rw-r--r--   0 root         (0) root         (0)   164294 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inventory/result.py
--rw-r--r--   0 root         (0) root         (0)   320490 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/inventory/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.481630 gs2-1.1.98/src/gs2/job_queue/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/job_queue/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25317 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/job_queue/model.py
--rw-r--r--   0 root         (0) root         (0)    38286 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/job_queue/request.py
--rw-r--r--   0 root         (0) root         (0)    60865 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/job_queue/rest.py
--rw-r--r--   0 root         (0) root         (0)    26853 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/job_queue/result.py
--rw-r--r--   0 root         (0) root         (0)    58512 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/job_queue/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.485630 gs2-1.1.98/src/gs2/key/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/key/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12546 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/key/model.py
--rw-r--r--   0 root         (0) root         (0)    24617 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/key/request.py
--rw-r--r--   0 root         (0) root         (0)    40001 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/key/rest.py
--rw-r--r--   0 root         (0) root         (0)    17815 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/key/result.py
--rw-r--r--   0 root         (0) root         (0)    38327 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/key/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.485630 gs2-1.1.98/src/gs2/limit/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/limit/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24281 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/limit/model.py
--rw-r--r--   0 root         (0) root         (0)    58191 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/limit/request.py
--rw-r--r--   0 root         (0) root         (0)    89863 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/limit/rest.py
--rw-r--r--   0 root         (0) root         (0)    36236 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/limit/result.py
--rw-r--r--   0 root         (0) root         (0)    86445 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/limit/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.485630 gs2-1.1.98/src/gs2/lock/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lock/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9204 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lock/model.py
--rw-r--r--   0 root         (0) root         (0)    23453 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lock/request.py
--rw-r--r--   0 root         (0) root         (0)    35086 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lock/rest.py
--rw-r--r--   0 root         (0) root         (0)    15295 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lock/result.py
--rw-r--r--   0 root         (0) root         (0)    33778 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lock/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.489630 gs2-1.1.98/src/gs2/log/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26176 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/log/model.py
--rw-r--r--   0 root         (0) root         (0)    42706 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/log/request.py
--rw-r--r--   0 root         (0) root         (0)    49783 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/log/rest.py
--rw-r--r--   0 root         (0) root         (0)    27100 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/log/result.py
--rw-r--r--   0 root         (0) root         (0)    47530 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/log/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.489630 gs2-1.1.98/src/gs2/login_reward/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/login_reward/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36556 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/login_reward/model.py
--rw-r--r--   0 root         (0) root         (0)    64849 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/login_reward/request.py
--rw-r--r--   0 root         (0) root         (0)    94308 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/login_reward/rest.py
--rw-r--r--   0 root         (0) root         (0)    47764 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/login_reward/result.py
--rw-r--r--   0 root         (0) root         (0)    90999 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/login_reward/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.489630 gs2-1.1.98/src/gs2/lottery/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lottery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48050 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lottery/model.py
--rw-r--r--   0 root         (0) root         (0)    75927 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lottery/request.py
--rw-r--r--   0 root         (0) root         (0)   114193 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lottery/rest.py
--rw-r--r--   0 root         (0) root         (0)    53049 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lottery/result.py
--rw-r--r--   0 root         (0) root         (0)   109664 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/lottery/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.493630 gs2-1.1.98/src/gs2/matchmaking/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/matchmaking/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54464 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/matchmaking/model.py
--rw-r--r--   0 root         (0) root         (0)    89313 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/matchmaking/request.py
--rw-r--r--   0 root         (0) root         (0)   116110 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/matchmaking/rest.py
--rw-r--r--   0 root         (0) root         (0)    47008 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/matchmaking/result.py
--rw-r--r--   0 root         (0) root         (0)   111919 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/matchmaking/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.493630 gs2-1.1.98/src/gs2/mega_field/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mega_field/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40588 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mega_field/model.py
--rw-r--r--   0 root         (0) root         (0)    54548 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mega_field/request.py
--rw-r--r--   0 root         (0) root         (0)    77817 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mega_field/rest.py
--rw-r--r--   0 root         (0) root         (0)    32973 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mega_field/result.py
--rw-r--r--   0 root         (0) root         (0)    74174 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mega_field/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.493630 gs2-1.1.98/src/gs2/mission/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mission/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66963 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mission/model.py
--rw-r--r--   0 root         (0) root         (0)   102300 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mission/request.py
--rw-r--r--   0 root         (0) root         (0)   143147 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mission/rest.py
--rw-r--r--   0 root         (0) root         (0)    60902 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mission/result.py
--rw-r--r--   0 root         (0) root         (0)   137270 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/mission/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.497630 gs2-1.1.98/src/gs2/money/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/money/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21704 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/money/model.py
--rw-r--r--   0 root         (0) root         (0)    45187 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/money/request.py
--rw-r--r--   0 root         (0) root         (0)    66675 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/money/rest.py
--rw-r--r--   0 root         (0) root         (0)    28121 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/money/result.py
--rw-r--r--   0 root         (0) root         (0)    64512 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/money/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.497630 gs2-1.1.98/src/gs2/news/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/news/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21543 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/news/model.py
--rw-r--r--   0 root         (0) root         (0)    21809 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/news/request.py
--rw-r--r--   0 root         (0) root         (0)    38058 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/news/rest.py
--rw-r--r--   0 root         (0) root         (0)    20551 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/news/result.py
--rw-r--r--   0 root         (0) root         (0)    36665 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/news/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.497630 gs2-1.1.98/src/gs2/quest/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/quest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56460 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/quest/model.py
--rw-r--r--   0 root         (0) root         (0)    85984 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/quest/request.py
--rw-r--r--   0 root         (0) root         (0)   117984 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/quest/rest.py
--rw-r--r--   0 root         (0) root         (0)    53692 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/quest/result.py
--rw-r--r--   0 root         (0) root         (0)   113585 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/quest/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.501630 gs2-1.1.98/src/gs2/ranking/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ranking/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47250 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ranking/model.py
--rw-r--r--   0 root         (0) root         (0)    81104 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ranking/request.py
--rw-r--r--   0 root         (0) root         (0)   110299 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ranking/rest.py
--rw-r--r--   0 root         (0) root         (0)    43830 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ranking/result.py
--rw-r--r--   0 root         (0) root         (0)   105248 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/ranking/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.501630 gs2-1.1.98/src/gs2/realtime/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/realtime/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12279 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/realtime/model.py
--rw-r--r--   0 root         (0) root         (0)    15852 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/realtime/request.py
--rw-r--r--   0 root         (0) root         (0)    24503 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/realtime/rest.py
--rw-r--r--   0 root         (0) root         (0)    11177 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/realtime/result.py
--rw-r--r--   0 root         (0) root         (0)    23737 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/realtime/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.501630 gs2-1.1.98/src/gs2/schedule/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/schedule/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29683 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/schedule/model.py
--rw-r--r--   0 root         (0) root         (0)    57021 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/schedule/request.py
--rw-r--r--   0 root         (0) root         (0)    86821 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/schedule/rest.py
--rw-r--r--   0 root         (0) root         (0)    38553 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/schedule/result.py
--rw-r--r--   0 root         (0) root         (0)    83939 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/schedule/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.501630 gs2-1.1.98/src/gs2/script/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/script/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17570 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/script/model.py
--rw-r--r--   0 root         (0) root         (0)    21528 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/script/request.py
--rw-r--r--   0 root         (0) root         (0)    33657 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/script/rest.py
--rw-r--r--   0 root         (0) root         (0)    18419 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/script/result.py
--rw-r--r--   0 root         (0) root         (0)    32512 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/script/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.505630 gs2-1.1.98/src/gs2/serial_key/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/serial_key/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27358 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/serial_key/model.py
--rw-r--r--   0 root         (0) root         (0)    48058 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/serial_key/request.py
--rw-r--r--   0 root         (0) root         (0)    80633 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/serial_key/rest.py
--rw-r--r--   0 root         (0) root         (0)    36324 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/serial_key/result.py
--rw-r--r--   0 root         (0) root         (0)    77377 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/serial_key/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.505630 gs2-1.1.98/src/gs2/showcase/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/showcase/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63594 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/showcase/model.py
--rw-r--r--   0 root         (0) root         (0)    96509 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/showcase/request.py
--rw-r--r--   0 root         (0) root         (0)   136032 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/showcase/rest.py
--rw-r--r--   0 root         (0) root         (0)    60511 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/showcase/result.py
--rw-r--r--   0 root         (0) root         (0)   130703 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/showcase/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.505630 gs2-1.1.98/src/gs2/skill_tree/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/skill_tree/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32968 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/skill_tree/model.py
--rw-r--r--   0 root         (0) root         (0)    58387 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/skill_tree/request.py
--rw-r--r--   0 root         (0) root         (0)    84759 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/skill_tree/rest.py
--rw-r--r--   0 root         (0) root         (0)    41358 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/skill_tree/result.py
--rw-r--r--   0 root         (0) root         (0)    82093 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/skill_tree/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.509630 gs2-1.1.98/src/gs2/stamina/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/stamina/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51438 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/stamina/model.py
--rw-r--r--   0 root         (0) root         (0)   108207 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/stamina/request.py
--rw-r--r--   0 root         (0) root         (0)   155671 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/stamina/rest.py
--rw-r--r--   0 root         (0) root         (0)    73656 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/stamina/result.py
--rw-r--r--   0 root         (0) root         (0)   150143 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/stamina/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.509630 gs2-1.1.98/src/gs2/state_machine/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/state_machine/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31045 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/state_machine/model.py
--rw-r--r--   0 root         (0) root         (0)    49385 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/state_machine/request.py
--rw-r--r--   0 root         (0) root         (0)    72484 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/state_machine/rest.py
--rw-r--r--   0 root         (0) root         (0)    28769 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/state_machine/result.py
--rw-r--r--   0 root         (0) root         (0)    69830 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/state_machine/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.509630 gs2-1.1.98/src/gs2/version/
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37846 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/version/model.py
--rw-r--r--   0 root         (0) root         (0)    57165 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/version/request.py
--rw-r--r--   0 root         (0) root         (0)    83954 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/version/rest.py
--rw-r--r--   0 root         (0) root         (0)    36469 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/version/result.py
--rw-r--r--   0 root         (0) root         (0)    81248 2024-01-15 12:00:57.000000 gs2-1.1.98/src/gs2/version/web_socket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 12:02:23.453630 gs2-1.1.98/src/gs2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      365 2024-01-15 12:02:23.000000 gs2-1.1.98/src/gs2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7362 2024-01-15 12:02:23.000000 gs2-1.1.98/src/gs2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-15 12:02:23.000000 gs2-1.1.98/src/gs2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-15 12:02:23.000000 gs2-1.1.98/src/gs2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-01-15 12:02:23.000000 gs2-1.1.98/src/gs2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.723083 gs2-1.1.99/
+-rw-r--r--   0 root         (0) root         (0)      365 2024-01-16 07:30:24.719083 gs2-1.1.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-16 07:30:24.723083 gs2-1.1.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1385 2024-01-16 07:29:16.000000 gs2-1.1.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.679082 gs2-1.1.99/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.683083 gs2-1.1.99/src/gs2/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.683083 gs2-1.1.99/src/gs2/account/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/account/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23808 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/account/model.py
+-rw-r--r--   0 root         (0) root         (0)    58434 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/account/request.py
+-rw-r--r--   0 root         (0) root         (0)    86019 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/account/rest.py
+-rw-r--r--   0 root         (0) root         (0)    34900 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/account/result.py
+-rw-r--r--   0 root         (0) root         (0)    82616 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/account/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.683083 gs2-1.1.99/src/gs2/ad_reward/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ad_reward/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ad_reward/model.py
+-rw-r--r--   0 root         (0) root         (0)    29108 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ad_reward/request.py
+-rw-r--r--   0 root         (0) root         (0)    48335 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ad_reward/rest.py
+-rw-r--r--   0 root         (0) root         (0)    19275 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ad_reward/result.py
+-rw-r--r--   0 root         (0) root         (0)    46908 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ad_reward/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.683083 gs2-1.1.99/src/gs2/auth/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/auth/model.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/auth/request.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/auth/rest.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/auth/result.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/auth/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.687083 gs2-1.1.99/src/gs2/chat/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/chat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26559 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/chat/model.py
+-rw-r--r--   0 root         (0) root         (0)    74045 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/chat/request.py
+-rw-r--r--   0 root         (0) root         (0)    96717 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/chat/rest.py
+-rw-r--r--   0 root         (0) root         (0)    37494 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/chat/result.py
+-rw-r--r--   0 root         (0) root         (0)    93168 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/chat/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.687083 gs2-1.1.99/src/gs2/core/
+-rw-r--r--   0 root         (0) root         (0)      188 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.687083 gs2-1.1.99/src/gs2/core/domain/
+-rw-r--r--   0 root         (0) root         (0)    10812 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/core/domain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      274 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/core/domain/access_token.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     6581 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/core/model.py
+-rw-r--r--   0 root         (0) root         (0)    10580 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/core/rest.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/core/util.py
+-rw-r--r--   0 root         (0) root         (0)    10955 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/core/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.687083 gs2-1.1.99/src/gs2/datastore/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/datastore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18306 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/datastore/model.py
+-rw-r--r--   0 root         (0) root         (0)    67152 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/datastore/request.py
+-rw-r--r--   0 root         (0) root         (0)    95350 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/datastore/rest.py
+-rw-r--r--   0 root         (0) root         (0)    42722 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/datastore/result.py
+-rw-r--r--   0 root         (0) root         (0)    92263 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/datastore/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.687083 gs2-1.1.99/src/gs2/deploy/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/deploy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21252 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/deploy/model.py
+-rw-r--r--   0 root         (0) root         (0)    22585 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/deploy/request.py
+-rw-r--r--   0 root         (0) root         (0)    40756 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/deploy/rest.py
+-rw-r--r--   0 root         (0) root         (0)    19223 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/deploy/result.py
+-rw-r--r--   0 root         (0) root         (0)    39142 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/deploy/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.687083 gs2-1.1.99/src/gs2/dictionary/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/dictionary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24080 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/dictionary/model.py
+-rw-r--r--   0 root         (0) root         (0)    54194 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/dictionary/request.py
+-rw-r--r--   0 root         (0) root         (0)    88429 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/dictionary/rest.py
+-rw-r--r--   0 root         (0) root         (0)    37924 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/dictionary/result.py
+-rw-r--r--   0 root         (0) root         (0)    85207 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/dictionary/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.691083 gs2-1.1.99/src/gs2/distributor/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/distributor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30989 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/distributor/model.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/distributor/request.py
+-rw-r--r--   0 root         (0) root         (0)    63369 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/distributor/rest.py
+-rw-r--r--   0 root         (0) root         (0)    29638 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/distributor/result.py
+-rw-r--r--   0 root         (0) root         (0)    61505 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/distributor/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.691083 gs2-1.1.99/src/gs2/enchant/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enchant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54270 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enchant/model.py
+-rw-r--r--   0 root         (0) root         (0)    94626 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enchant/request.py
+-rw-r--r--   0 root         (0) root         (0)   137241 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enchant/rest.py
+-rw-r--r--   0 root         (0) root         (0)    59909 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enchant/result.py
+-rw-r--r--   0 root         (0) root         (0)   132555 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enchant/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.691083 gs2-1.1.99/src/gs2/enhance/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enhance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46945 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enhance/model.py
+-rw-r--r--   0 root         (0) root         (0)    86426 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enhance/request.py
+-rw-r--r--   0 root         (0) root         (0)   116825 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enhance/rest.py
+-rw-r--r--   0 root         (0) root         (0)    61187 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enhance/result.py
+-rw-r--r--   0 root         (0) root         (0)   113147 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/enhance/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.691083 gs2-1.1.99/src/gs2/exchange/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/exchange/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48528 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/exchange/model.py
+-rw-r--r--   0 root         (0) root         (0)    95983 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/exchange/request.py
+-rw-r--r--   0 root         (0) root         (0)   130421 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/exchange/rest.py
+-rw-r--r--   0 root         (0) root         (0)    66629 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/exchange/result.py
+-rw-r--r--   0 root         (0) root         (0)   125924 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/exchange/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.695083 gs2-1.1.99/src/gs2/experience/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/experience/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42324 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/experience/model.py
+-rw-r--r--   0 root         (0) root         (0)    97516 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/experience/request.py
+-rw-r--r--   0 root         (0) root         (0)   136459 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/experience/rest.py
+-rw-r--r--   0 root         (0) root         (0)    57549 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/experience/result.py
+-rw-r--r--   0 root         (0) root         (0)   130825 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/experience/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.695083 gs2-1.1.99/src/gs2/formation/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/formation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61465 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/formation/model.py
+-rw-r--r--   0 root         (0) root         (0)   125462 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/formation/request.py
+-rw-r--r--   0 root         (0) root         (0)   180533 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/formation/rest.py
+-rw-r--r--   0 root         (0) root         (0)    94604 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/formation/result.py
+-rw-r--r--   0 root         (0) root         (0)   172509 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/formation/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.695083 gs2-1.1.99/src/gs2/friend/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/friend/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44859 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/friend/model.py
+-rw-r--r--   0 root         (0) root         (0)    96861 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/friend/request.py
+-rw-r--r--   0 root         (0) root         (0)   134753 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/friend/rest.py
+-rw-r--r--   0 root         (0) root         (0)    54985 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/friend/result.py
+-rw-r--r--   0 root         (0) root         (0)   129941 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/friend/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.695083 gs2-1.1.99/src/gs2/gateway/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/gateway/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13754 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/gateway/model.py
+-rw-r--r--   0 root         (0) root         (0)    39264 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/gateway/request.py
+-rw-r--r--   0 root         (0) root         (0)    63586 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/gateway/rest.py
+-rw-r--r--   0 root         (0) root         (0)    25524 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/gateway/result.py
+-rw-r--r--   0 root         (0) root         (0)    61650 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/gateway/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.699083 gs2-1.1.99/src/gs2/grade/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/grade/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37287 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/grade/model.py
+-rw-r--r--   0 root         (0) root         (0)    76293 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/grade/request.py
+-rw-r--r--   0 root         (0) root         (0)   109392 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/grade/rest.py
+-rw-r--r--   0 root         (0) root         (0)    51920 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/grade/result.py
+-rw-r--r--   0 root         (0) root         (0)   105064 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/grade/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.699083 gs2-1.1.99/src/gs2/identifier/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/identifier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14333 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/identifier/model.py
+-rw-r--r--   0 root         (0) root         (0)    27417 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/identifier/request.py
+-rw-r--r--   0 root         (0) root         (0)    51631 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/identifier/rest.py
+-rw-r--r--   0 root         (0) root         (0)    26226 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/identifier/result.py
+-rw-r--r--   0 root         (0) root         (0)    49813 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/identifier/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.699083 gs2-1.1.99/src/gs2/idle/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/idle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34135 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/idle/model.py
+-rw-r--r--   0 root         (0) root         (0)    57207 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/idle/request.py
+-rw-r--r--   0 root         (0) root         (0)    86289 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/idle/rest.py
+-rw-r--r--   0 root         (0) root         (0)    39558 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/idle/result.py
+-rw-r--r--   0 root         (0) root         (0)    83280 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/idle/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.699083 gs2-1.1.99/src/gs2/inbox/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40566 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inbox/model.py
+-rw-r--r--   0 root         (0) root         (0)    71136 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inbox/request.py
+-rw-r--r--   0 root         (0) root         (0)   103104 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inbox/rest.py
+-rw-r--r--   0 root         (0) root         (0)    44816 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inbox/result.py
+-rw-r--r--   0 root         (0) root         (0)    99616 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inbox/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.703083 gs2-1.1.99/src/gs2/inventory/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inventory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104288 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inventory/model.py
+-rw-r--r--   0 root         (0) root         (0)   238236 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inventory/request.py
+-rw-r--r--   0 root         (0) root         (0)   336372 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inventory/rest.py
+-rw-r--r--   0 root         (0) root         (0)   164294 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inventory/result.py
+-rw-r--r--   0 root         (0) root         (0)   320490 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/inventory/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.703083 gs2-1.1.99/src/gs2/job_queue/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/job_queue/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25317 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/job_queue/model.py
+-rw-r--r--   0 root         (0) root         (0)    38286 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/job_queue/request.py
+-rw-r--r--   0 root         (0) root         (0)    60865 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/job_queue/rest.py
+-rw-r--r--   0 root         (0) root         (0)    26853 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/job_queue/result.py
+-rw-r--r--   0 root         (0) root         (0)    58512 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/job_queue/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.703083 gs2-1.1.99/src/gs2/key/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/key/model.py
+-rw-r--r--   0 root         (0) root         (0)    24617 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/key/request.py
+-rw-r--r--   0 root         (0) root         (0)    40001 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/key/rest.py
+-rw-r--r--   0 root         (0) root         (0)    17815 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/key/result.py
+-rw-r--r--   0 root         (0) root         (0)    38327 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/key/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.703083 gs2-1.1.99/src/gs2/limit/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/limit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24281 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/limit/model.py
+-rw-r--r--   0 root         (0) root         (0)    58191 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/limit/request.py
+-rw-r--r--   0 root         (0) root         (0)    89863 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/limit/rest.py
+-rw-r--r--   0 root         (0) root         (0)    36236 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/limit/result.py
+-rw-r--r--   0 root         (0) root         (0)    86445 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/limit/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.703083 gs2-1.1.99/src/gs2/lock/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9204 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lock/model.py
+-rw-r--r--   0 root         (0) root         (0)    23453 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lock/request.py
+-rw-r--r--   0 root         (0) root         (0)    35086 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lock/rest.py
+-rw-r--r--   0 root         (0) root         (0)    15295 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lock/result.py
+-rw-r--r--   0 root         (0) root         (0)    33778 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lock/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.707083 gs2-1.1.99/src/gs2/log/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26176 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/log/model.py
+-rw-r--r--   0 root         (0) root         (0)    42706 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/log/request.py
+-rw-r--r--   0 root         (0) root         (0)    49783 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/log/rest.py
+-rw-r--r--   0 root         (0) root         (0)    27100 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/log/result.py
+-rw-r--r--   0 root         (0) root         (0)    47530 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/log/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.707083 gs2-1.1.99/src/gs2/login_reward/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/login_reward/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36556 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/login_reward/model.py
+-rw-r--r--   0 root         (0) root         (0)    64849 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/login_reward/request.py
+-rw-r--r--   0 root         (0) root         (0)    94308 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/login_reward/rest.py
+-rw-r--r--   0 root         (0) root         (0)    47764 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/login_reward/result.py
+-rw-r--r--   0 root         (0) root         (0)    90999 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/login_reward/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.707083 gs2-1.1.99/src/gs2/lottery/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lottery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48050 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lottery/model.py
+-rw-r--r--   0 root         (0) root         (0)    75927 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lottery/request.py
+-rw-r--r--   0 root         (0) root         (0)   114193 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lottery/rest.py
+-rw-r--r--   0 root         (0) root         (0)    53049 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lottery/result.py
+-rw-r--r--   0 root         (0) root         (0)   109664 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/lottery/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.707083 gs2-1.1.99/src/gs2/matchmaking/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/matchmaking/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54464 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/matchmaking/model.py
+-rw-r--r--   0 root         (0) root         (0)    89313 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/matchmaking/request.py
+-rw-r--r--   0 root         (0) root         (0)   116110 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/matchmaking/rest.py
+-rw-r--r--   0 root         (0) root         (0)    47008 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/matchmaking/result.py
+-rw-r--r--   0 root         (0) root         (0)   111919 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/matchmaking/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.707083 gs2-1.1.99/src/gs2/mega_field/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mega_field/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40588 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mega_field/model.py
+-rw-r--r--   0 root         (0) root         (0)    54548 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mega_field/request.py
+-rw-r--r--   0 root         (0) root         (0)    77817 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mega_field/rest.py
+-rw-r--r--   0 root         (0) root         (0)    32973 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mega_field/result.py
+-rw-r--r--   0 root         (0) root         (0)    74174 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mega_field/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.711083 gs2-1.1.99/src/gs2/mission/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mission/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66963 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mission/model.py
+-rw-r--r--   0 root         (0) root         (0)   102300 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mission/request.py
+-rw-r--r--   0 root         (0) root         (0)   143147 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mission/rest.py
+-rw-r--r--   0 root         (0) root         (0)    60902 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mission/result.py
+-rw-r--r--   0 root         (0) root         (0)   137270 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/mission/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.711083 gs2-1.1.99/src/gs2/money/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/money/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21704 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/money/model.py
+-rw-r--r--   0 root         (0) root         (0)    45187 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/money/request.py
+-rw-r--r--   0 root         (0) root         (0)    66675 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/money/rest.py
+-rw-r--r--   0 root         (0) root         (0)    28121 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/money/result.py
+-rw-r--r--   0 root         (0) root         (0)    64512 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/money/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.711083 gs2-1.1.99/src/gs2/news/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/news/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21543 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/news/model.py
+-rw-r--r--   0 root         (0) root         (0)    21809 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/news/request.py
+-rw-r--r--   0 root         (0) root         (0)    38058 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/news/rest.py
+-rw-r--r--   0 root         (0) root         (0)    20551 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/news/result.py
+-rw-r--r--   0 root         (0) root         (0)    36665 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/news/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.711083 gs2-1.1.99/src/gs2/quest/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/quest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56460 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/quest/model.py
+-rw-r--r--   0 root         (0) root         (0)    85984 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/quest/request.py
+-rw-r--r--   0 root         (0) root         (0)   117984 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/quest/rest.py
+-rw-r--r--   0 root         (0) root         (0)    53692 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/quest/result.py
+-rw-r--r--   0 root         (0) root         (0)   113585 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/quest/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.715083 gs2-1.1.99/src/gs2/ranking/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ranking/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47250 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ranking/model.py
+-rw-r--r--   0 root         (0) root         (0)    81104 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ranking/request.py
+-rw-r--r--   0 root         (0) root         (0)   110299 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ranking/rest.py
+-rw-r--r--   0 root         (0) root         (0)    43830 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ranking/result.py
+-rw-r--r--   0 root         (0) root         (0)   105248 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/ranking/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.715083 gs2-1.1.99/src/gs2/realtime/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/realtime/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12279 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/realtime/model.py
+-rw-r--r--   0 root         (0) root         (0)    15852 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/realtime/request.py
+-rw-r--r--   0 root         (0) root         (0)    24503 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/realtime/rest.py
+-rw-r--r--   0 root         (0) root         (0)    11177 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/realtime/result.py
+-rw-r--r--   0 root         (0) root         (0)    23737 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/realtime/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.715083 gs2-1.1.99/src/gs2/schedule/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/schedule/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29683 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/schedule/model.py
+-rw-r--r--   0 root         (0) root         (0)    57021 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/schedule/request.py
+-rw-r--r--   0 root         (0) root         (0)    86821 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/schedule/rest.py
+-rw-r--r--   0 root         (0) root         (0)    38553 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/schedule/result.py
+-rw-r--r--   0 root         (0) root         (0)    83939 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/schedule/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.715083 gs2-1.1.99/src/gs2/script/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/script/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20087 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/script/model.py
+-rw-r--r--   0 root         (0) root         (0)    22414 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/script/request.py
+-rw-r--r--   0 root         (0) root         (0)    33919 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/script/rest.py
+-rw-r--r--   0 root         (0) root         (0)    18419 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/script/result.py
+-rw-r--r--   0 root         (0) root         (0)    32774 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/script/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.715083 gs2-1.1.99/src/gs2/serial_key/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/serial_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27358 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/serial_key/model.py
+-rw-r--r--   0 root         (0) root         (0)    48058 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/serial_key/request.py
+-rw-r--r--   0 root         (0) root         (0)    80633 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/serial_key/rest.py
+-rw-r--r--   0 root         (0) root         (0)    36324 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/serial_key/result.py
+-rw-r--r--   0 root         (0) root         (0)    77377 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/serial_key/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.719083 gs2-1.1.99/src/gs2/showcase/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/showcase/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63594 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/showcase/model.py
+-rw-r--r--   0 root         (0) root         (0)    96509 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/showcase/request.py
+-rw-r--r--   0 root         (0) root         (0)   136032 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/showcase/rest.py
+-rw-r--r--   0 root         (0) root         (0)    60511 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/showcase/result.py
+-rw-r--r--   0 root         (0) root         (0)   130703 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/showcase/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.719083 gs2-1.1.99/src/gs2/skill_tree/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/skill_tree/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32968 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/skill_tree/model.py
+-rw-r--r--   0 root         (0) root         (0)    58387 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/skill_tree/request.py
+-rw-r--r--   0 root         (0) root         (0)    84759 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/skill_tree/rest.py
+-rw-r--r--   0 root         (0) root         (0)    41358 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/skill_tree/result.py
+-rw-r--r--   0 root         (0) root         (0)    82093 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/skill_tree/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.719083 gs2-1.1.99/src/gs2/stamina/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/stamina/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51438 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/stamina/model.py
+-rw-r--r--   0 root         (0) root         (0)   108207 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/stamina/request.py
+-rw-r--r--   0 root         (0) root         (0)   155671 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/stamina/rest.py
+-rw-r--r--   0 root         (0) root         (0)    73656 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/stamina/result.py
+-rw-r--r--   0 root         (0) root         (0)   150143 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/stamina/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.719083 gs2-1.1.99/src/gs2/state_machine/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/state_machine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31045 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/state_machine/model.py
+-rw-r--r--   0 root         (0) root         (0)    49385 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/state_machine/request.py
+-rw-r--r--   0 root         (0) root         (0)    72484 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/state_machine/rest.py
+-rw-r--r--   0 root         (0) root         (0)    28769 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/state_machine/result.py
+-rw-r--r--   0 root         (0) root         (0)    69830 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/state_machine/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.719083 gs2-1.1.99/src/gs2/version/
+-rw-r--r--   0 root         (0) root         (0)      696 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37846 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/version/model.py
+-rw-r--r--   0 root         (0) root         (0)    57165 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/version/request.py
+-rw-r--r--   0 root         (0) root         (0)    83954 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/version/rest.py
+-rw-r--r--   0 root         (0) root         (0)    36469 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/version/result.py
+-rw-r--r--   0 root         (0) root         (0)    81248 2024-01-16 07:29:16.000000 gs2-1.1.99/src/gs2/version/web_socket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 07:30:24.683083 gs2-1.1.99/src/gs2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      365 2024-01-16 07:30:24.000000 gs2-1.1.99/src/gs2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7362 2024-01-16 07:30:24.000000 gs2-1.1.99/src/gs2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 07:30:24.000000 gs2-1.1.99/src/gs2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-01-16 07:30:24.000000 gs2-1.1.99/src/gs2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-01-16 07:30:24.000000 gs2-1.1.99/src/gs2.egg-info/top_level.txt
```

### Comparing `gs2-1.1.98/setup.py` & `gs2-1.1.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from setuptools import setup, find_packages
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='gs2',
-    version='1.1.98',
+    version='1.1.99',
     package_dir={'': 'src'},
     py_modules=["gs2"],
     packages=find_packages('src'),
     install_requires=[
         'websocket_client >= 0.59.0',
         'simplejson >= 3.17.2',
         'requests >= 2.25.1',
```

### Comparing `gs2-1.1.98/src/gs2/__init__.py` & `gs2-1.1.99/src/gs2/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/account/__init__.py` & `gs2-1.1.99/src/gs2/account/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/account/model.py` & `gs2-1.1.99/src/gs2/account/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/account/request.py` & `gs2-1.1.99/src/gs2/account/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/account/rest.py` & `gs2-1.1.99/src/gs2/account/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/account/result.py` & `gs2-1.1.99/src/gs2/account/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/account/web_socket.py` & `gs2-1.1.99/src/gs2/account/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ad_reward/__init__.py` & `gs2-1.1.99/src/gs2/ad_reward/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ad_reward/model.py` & `gs2-1.1.99/src/gs2/ad_reward/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ad_reward/request.py` & `gs2-1.1.99/src/gs2/ad_reward/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ad_reward/rest.py` & `gs2-1.1.99/src/gs2/ad_reward/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ad_reward/result.py` & `gs2-1.1.99/src/gs2/ad_reward/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ad_reward/web_socket.py` & `gs2-1.1.99/src/gs2/ad_reward/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/auth/__init__.py` & `gs2-1.1.99/src/gs2/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/auth/model.py` & `gs2-1.1.99/src/gs2/auth/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/auth/request.py` & `gs2-1.1.99/src/gs2/auth/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/auth/rest.py` & `gs2-1.1.99/src/gs2/auth/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/auth/result.py` & `gs2-1.1.99/src/gs2/auth/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/auth/web_socket.py` & `gs2-1.1.99/src/gs2/auth/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/chat/__init__.py` & `gs2-1.1.99/src/gs2/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/chat/model.py` & `gs2-1.1.99/src/gs2/chat/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/chat/request.py` & `gs2-1.1.99/src/gs2/chat/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/chat/rest.py` & `gs2-1.1.99/src/gs2/chat/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/chat/result.py` & `gs2-1.1.99/src/gs2/chat/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/chat/web_socket.py` & `gs2-1.1.99/src/gs2/chat/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/core/domain/__init__.py` & `gs2-1.1.99/src/gs2/core/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/core/exception.py` & `gs2-1.1.99/src/gs2/core/exception.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/core/model.py` & `gs2-1.1.99/src/gs2/core/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/core/rest.py` & `gs2-1.1.99/src/gs2/core/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/core/util.py` & `gs2-1.1.99/src/gs2/core/util.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/core/web_socket.py` & `gs2-1.1.99/src/gs2/core/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/datastore/__init__.py` & `gs2-1.1.99/src/gs2/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/datastore/model.py` & `gs2-1.1.99/src/gs2/datastore/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/datastore/request.py` & `gs2-1.1.99/src/gs2/datastore/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/datastore/rest.py` & `gs2-1.1.99/src/gs2/datastore/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/datastore/result.py` & `gs2-1.1.99/src/gs2/datastore/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/datastore/web_socket.py` & `gs2-1.1.99/src/gs2/datastore/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/deploy/__init__.py` & `gs2-1.1.99/src/gs2/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/deploy/model.py` & `gs2-1.1.99/src/gs2/deploy/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/deploy/request.py` & `gs2-1.1.99/src/gs2/deploy/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/deploy/rest.py` & `gs2-1.1.99/src/gs2/deploy/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/deploy/result.py` & `gs2-1.1.99/src/gs2/deploy/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/deploy/web_socket.py` & `gs2-1.1.99/src/gs2/deploy/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/dictionary/__init__.py` & `gs2-1.1.99/src/gs2/dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/dictionary/model.py` & `gs2-1.1.99/src/gs2/dictionary/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/dictionary/request.py` & `gs2-1.1.99/src/gs2/dictionary/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/dictionary/rest.py` & `gs2-1.1.99/src/gs2/dictionary/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/dictionary/result.py` & `gs2-1.1.99/src/gs2/dictionary/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/dictionary/web_socket.py` & `gs2-1.1.99/src/gs2/dictionary/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/distributor/__init__.py` & `gs2-1.1.99/src/gs2/distributor/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/distributor/model.py` & `gs2-1.1.99/src/gs2/distributor/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/distributor/request.py` & `gs2-1.1.99/src/gs2/distributor/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/distributor/rest.py` & `gs2-1.1.99/src/gs2/distributor/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/distributor/result.py` & `gs2-1.1.99/src/gs2/distributor/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/distributor/web_socket.py` & `gs2-1.1.99/src/gs2/distributor/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enchant/__init__.py` & `gs2-1.1.99/src/gs2/enchant/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enchant/model.py` & `gs2-1.1.99/src/gs2/enchant/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enchant/request.py` & `gs2-1.1.99/src/gs2/enchant/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enchant/rest.py` & `gs2-1.1.99/src/gs2/enchant/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enchant/result.py` & `gs2-1.1.99/src/gs2/enchant/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enchant/web_socket.py` & `gs2-1.1.99/src/gs2/enchant/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enhance/__init__.py` & `gs2-1.1.99/src/gs2/enhance/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enhance/model.py` & `gs2-1.1.99/src/gs2/enhance/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enhance/request.py` & `gs2-1.1.99/src/gs2/enhance/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enhance/rest.py` & `gs2-1.1.99/src/gs2/enhance/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enhance/result.py` & `gs2-1.1.99/src/gs2/enhance/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/enhance/web_socket.py` & `gs2-1.1.99/src/gs2/enhance/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/exchange/__init__.py` & `gs2-1.1.99/src/gs2/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/exchange/model.py` & `gs2-1.1.99/src/gs2/exchange/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/exchange/request.py` & `gs2-1.1.99/src/gs2/exchange/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/exchange/rest.py` & `gs2-1.1.99/src/gs2/exchange/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/exchange/result.py` & `gs2-1.1.99/src/gs2/exchange/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/exchange/web_socket.py` & `gs2-1.1.99/src/gs2/exchange/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/experience/__init__.py` & `gs2-1.1.99/src/gs2/experience/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/experience/model.py` & `gs2-1.1.99/src/gs2/experience/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/experience/request.py` & `gs2-1.1.99/src/gs2/experience/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/experience/rest.py` & `gs2-1.1.99/src/gs2/experience/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/experience/result.py` & `gs2-1.1.99/src/gs2/experience/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/experience/web_socket.py` & `gs2-1.1.99/src/gs2/experience/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/formation/__init__.py` & `gs2-1.1.99/src/gs2/formation/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/formation/model.py` & `gs2-1.1.99/src/gs2/formation/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/formation/request.py` & `gs2-1.1.99/src/gs2/formation/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/formation/rest.py` & `gs2-1.1.99/src/gs2/formation/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/formation/result.py` & `gs2-1.1.99/src/gs2/formation/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/formation/web_socket.py` & `gs2-1.1.99/src/gs2/formation/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/friend/__init__.py` & `gs2-1.1.99/src/gs2/friend/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/friend/model.py` & `gs2-1.1.99/src/gs2/friend/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/friend/request.py` & `gs2-1.1.99/src/gs2/friend/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/friend/rest.py` & `gs2-1.1.99/src/gs2/friend/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/friend/result.py` & `gs2-1.1.99/src/gs2/friend/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/friend/web_socket.py` & `gs2-1.1.99/src/gs2/friend/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/gateway/__init__.py` & `gs2-1.1.99/src/gs2/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/gateway/model.py` & `gs2-1.1.99/src/gs2/gateway/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/gateway/request.py` & `gs2-1.1.99/src/gs2/gateway/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/gateway/rest.py` & `gs2-1.1.99/src/gs2/gateway/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/gateway/result.py` & `gs2-1.1.99/src/gs2/gateway/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/gateway/web_socket.py` & `gs2-1.1.99/src/gs2/gateway/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/grade/__init__.py` & `gs2-1.1.99/src/gs2/grade/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/grade/model.py` & `gs2-1.1.99/src/gs2/grade/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/grade/request.py` & `gs2-1.1.99/src/gs2/grade/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/grade/rest.py` & `gs2-1.1.99/src/gs2/grade/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/grade/result.py` & `gs2-1.1.99/src/gs2/grade/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/grade/web_socket.py` & `gs2-1.1.99/src/gs2/grade/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/identifier/__init__.py` & `gs2-1.1.99/src/gs2/identifier/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/identifier/model.py` & `gs2-1.1.99/src/gs2/identifier/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/identifier/request.py` & `gs2-1.1.99/src/gs2/identifier/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/identifier/rest.py` & `gs2-1.1.99/src/gs2/identifier/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/identifier/result.py` & `gs2-1.1.99/src/gs2/identifier/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/identifier/web_socket.py` & `gs2-1.1.99/src/gs2/identifier/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/idle/__init__.py` & `gs2-1.1.99/src/gs2/idle/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/idle/model.py` & `gs2-1.1.99/src/gs2/idle/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/idle/request.py` & `gs2-1.1.99/src/gs2/idle/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/idle/rest.py` & `gs2-1.1.99/src/gs2/idle/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/idle/result.py` & `gs2-1.1.99/src/gs2/idle/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/idle/web_socket.py` & `gs2-1.1.99/src/gs2/idle/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inbox/__init__.py` & `gs2-1.1.99/src/gs2/inbox/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inbox/model.py` & `gs2-1.1.99/src/gs2/inbox/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inbox/request.py` & `gs2-1.1.99/src/gs2/inbox/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inbox/rest.py` & `gs2-1.1.99/src/gs2/inbox/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inbox/result.py` & `gs2-1.1.99/src/gs2/inbox/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inbox/web_socket.py` & `gs2-1.1.99/src/gs2/inbox/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inventory/__init__.py` & `gs2-1.1.99/src/gs2/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inventory/model.py` & `gs2-1.1.99/src/gs2/inventory/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inventory/request.py` & `gs2-1.1.99/src/gs2/inventory/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inventory/rest.py` & `gs2-1.1.99/src/gs2/inventory/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inventory/result.py` & `gs2-1.1.99/src/gs2/inventory/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/inventory/web_socket.py` & `gs2-1.1.99/src/gs2/inventory/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/job_queue/__init__.py` & `gs2-1.1.99/src/gs2/job_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/job_queue/model.py` & `gs2-1.1.99/src/gs2/job_queue/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/job_queue/request.py` & `gs2-1.1.99/src/gs2/job_queue/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/job_queue/rest.py` & `gs2-1.1.99/src/gs2/job_queue/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/job_queue/result.py` & `gs2-1.1.99/src/gs2/job_queue/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/job_queue/web_socket.py` & `gs2-1.1.99/src/gs2/job_queue/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/key/__init__.py` & `gs2-1.1.99/src/gs2/key/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/key/model.py` & `gs2-1.1.99/src/gs2/key/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/key/request.py` & `gs2-1.1.99/src/gs2/key/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/key/rest.py` & `gs2-1.1.99/src/gs2/key/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/key/result.py` & `gs2-1.1.99/src/gs2/key/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/key/web_socket.py` & `gs2-1.1.99/src/gs2/key/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/limit/__init__.py` & `gs2-1.1.99/src/gs2/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/limit/model.py` & `gs2-1.1.99/src/gs2/limit/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/limit/request.py` & `gs2-1.1.99/src/gs2/limit/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/limit/rest.py` & `gs2-1.1.99/src/gs2/limit/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/limit/result.py` & `gs2-1.1.99/src/gs2/limit/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/limit/web_socket.py` & `gs2-1.1.99/src/gs2/limit/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lock/__init__.py` & `gs2-1.1.99/src/gs2/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lock/model.py` & `gs2-1.1.99/src/gs2/lock/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lock/request.py` & `gs2-1.1.99/src/gs2/lock/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lock/rest.py` & `gs2-1.1.99/src/gs2/lock/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lock/result.py` & `gs2-1.1.99/src/gs2/lock/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lock/web_socket.py` & `gs2-1.1.99/src/gs2/lock/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/log/__init__.py` & `gs2-1.1.99/src/gs2/log/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/log/model.py` & `gs2-1.1.99/src/gs2/log/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/log/request.py` & `gs2-1.1.99/src/gs2/log/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/log/rest.py` & `gs2-1.1.99/src/gs2/log/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/log/result.py` & `gs2-1.1.99/src/gs2/log/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/log/web_socket.py` & `gs2-1.1.99/src/gs2/log/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/login_reward/__init__.py` & `gs2-1.1.99/src/gs2/login_reward/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/login_reward/model.py` & `gs2-1.1.99/src/gs2/login_reward/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/login_reward/request.py` & `gs2-1.1.99/src/gs2/login_reward/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/login_reward/rest.py` & `gs2-1.1.99/src/gs2/login_reward/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/login_reward/result.py` & `gs2-1.1.99/src/gs2/login_reward/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/login_reward/web_socket.py` & `gs2-1.1.99/src/gs2/login_reward/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lottery/__init__.py` & `gs2-1.1.99/src/gs2/lottery/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lottery/model.py` & `gs2-1.1.99/src/gs2/lottery/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lottery/request.py` & `gs2-1.1.99/src/gs2/lottery/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lottery/rest.py` & `gs2-1.1.99/src/gs2/lottery/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lottery/result.py` & `gs2-1.1.99/src/gs2/lottery/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/lottery/web_socket.py` & `gs2-1.1.99/src/gs2/lottery/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/matchmaking/__init__.py` & `gs2-1.1.99/src/gs2/matchmaking/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/matchmaking/model.py` & `gs2-1.1.99/src/gs2/matchmaking/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/matchmaking/request.py` & `gs2-1.1.99/src/gs2/matchmaking/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/matchmaking/rest.py` & `gs2-1.1.99/src/gs2/matchmaking/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/matchmaking/result.py` & `gs2-1.1.99/src/gs2/matchmaking/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/matchmaking/web_socket.py` & `gs2-1.1.99/src/gs2/matchmaking/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mega_field/__init__.py` & `gs2-1.1.99/src/gs2/mega_field/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mega_field/model.py` & `gs2-1.1.99/src/gs2/mega_field/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mega_field/request.py` & `gs2-1.1.99/src/gs2/mega_field/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mega_field/rest.py` & `gs2-1.1.99/src/gs2/mega_field/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mega_field/result.py` & `gs2-1.1.99/src/gs2/mega_field/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mega_field/web_socket.py` & `gs2-1.1.99/src/gs2/mega_field/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mission/__init__.py` & `gs2-1.1.99/src/gs2/mission/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mission/model.py` & `gs2-1.1.99/src/gs2/mission/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mission/request.py` & `gs2-1.1.99/src/gs2/mission/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mission/rest.py` & `gs2-1.1.99/src/gs2/mission/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mission/result.py` & `gs2-1.1.99/src/gs2/mission/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/mission/web_socket.py` & `gs2-1.1.99/src/gs2/mission/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/money/__init__.py` & `gs2-1.1.99/src/gs2/money/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/money/model.py` & `gs2-1.1.99/src/gs2/money/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/money/request.py` & `gs2-1.1.99/src/gs2/money/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/money/rest.py` & `gs2-1.1.99/src/gs2/money/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/money/result.py` & `gs2-1.1.99/src/gs2/money/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/money/web_socket.py` & `gs2-1.1.99/src/gs2/money/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/news/__init__.py` & `gs2-1.1.99/src/gs2/news/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/news/model.py` & `gs2-1.1.99/src/gs2/news/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/news/request.py` & `gs2-1.1.99/src/gs2/news/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/news/rest.py` & `gs2-1.1.99/src/gs2/news/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/news/result.py` & `gs2-1.1.99/src/gs2/news/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/news/web_socket.py` & `gs2-1.1.99/src/gs2/news/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/quest/__init__.py` & `gs2-1.1.99/src/gs2/quest/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/quest/model.py` & `gs2-1.1.99/src/gs2/quest/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/quest/request.py` & `gs2-1.1.99/src/gs2/quest/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/quest/rest.py` & `gs2-1.1.99/src/gs2/quest/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/quest/result.py` & `gs2-1.1.99/src/gs2/quest/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/quest/web_socket.py` & `gs2-1.1.99/src/gs2/quest/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ranking/__init__.py` & `gs2-1.1.99/src/gs2/ranking/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ranking/model.py` & `gs2-1.1.99/src/gs2/ranking/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ranking/request.py` & `gs2-1.1.99/src/gs2/ranking/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ranking/rest.py` & `gs2-1.1.99/src/gs2/ranking/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ranking/result.py` & `gs2-1.1.99/src/gs2/ranking/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/ranking/web_socket.py` & `gs2-1.1.99/src/gs2/ranking/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/realtime/__init__.py` & `gs2-1.1.99/src/gs2/realtime/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/realtime/model.py` & `gs2-1.1.99/src/gs2/realtime/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/realtime/request.py` & `gs2-1.1.99/src/gs2/realtime/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/realtime/rest.py` & `gs2-1.1.99/src/gs2/realtime/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/realtime/result.py` & `gs2-1.1.99/src/gs2/realtime/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/realtime/web_socket.py` & `gs2-1.1.99/src/gs2/realtime/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/schedule/__init__.py` & `gs2-1.1.99/src/gs2/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/schedule/model.py` & `gs2-1.1.99/src/gs2/schedule/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/schedule/request.py` & `gs2-1.1.99/src/gs2/schedule/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/schedule/rest.py` & `gs2-1.1.99/src/gs2/schedule/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/schedule/result.py` & `gs2-1.1.99/src/gs2/schedule/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/schedule/web_socket.py` & `gs2-1.1.99/src/gs2/schedule/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/script/__init__.py` & `gs2-1.1.99/src/gs2/script/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/script/model.py` & `gs2-1.1.99/src/gs2/script/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,18 +125,78 @@
             "referenceType": self.reference_type,
             "commitHash": self.commit_hash,
             "branchName": self.branch_name,
             "tagName": self.tag_name,
         }
 
 
+class TransactionSetting(core.Gs2Model):
+    enable_auto_run: bool = None
+    distributor_namespace_id: str = None
+    key_id: str = None
+    queue_namespace_id: str = None
+
+    def with_enable_auto_run(self, enable_auto_run: bool) -> TransactionSetting:
+        self.enable_auto_run = enable_auto_run
+        return self
+
+    def with_distributor_namespace_id(self, distributor_namespace_id: str) -> TransactionSetting:
+        self.distributor_namespace_id = distributor_namespace_id
+        return self
+
+    def with_key_id(self, key_id: str) -> TransactionSetting:
+        self.key_id = key_id
+        return self
+
+    def with_queue_namespace_id(self, queue_namespace_id: str) -> TransactionSetting:
+        self.queue_namespace_id = queue_namespace_id
+        return self
+
+    def get(self, key, default=None):
+        items = self.to_dict()
+        if key in items.keys():
+            return items[key]
+        return default
+
+    def __getitem__(self, key):
+        items = self.to_dict()
+        if key in items.keys():
+            return items[key]
+        return None
+
+    @staticmethod
+    def from_dict(
+        data: Dict[str, Any],
+    ) -> Optional[TransactionSetting]:
+        if data is None:
+            return None
+        return TransactionSetting()\
+            .with_enable_auto_run(data.get('enableAutoRun'))\
+            .with_distributor_namespace_id(data.get('distributorNamespaceId'))\
+            .with_key_id(data.get('keyId'))\
+            .with_queue_namespace_id(data.get('queueNamespaceId'))
+
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            "enableAutoRun": self.enable_auto_run,
+            "distributorNamespaceId": self.distributor_namespace_id,
+            "keyId": self.key_id,
+            "queueNamespaceId": self.queue_namespace_id,
+        }
+
+
 class Transaction(core.Gs2Model):
+    transaction_id: str = None
     consume_actions: List[ConsumeAction] = None
     acquire_actions: List[AcquireAction] = None
 
+    def with_transaction_id(self, transaction_id: str) -> Transaction:
+        self.transaction_id = transaction_id
+        return self
+
     def with_consume_actions(self, consume_actions: List[ConsumeAction]) -> Transaction:
         self.consume_actions = consume_actions
         return self
 
     def with_acquire_actions(self, acquire_actions: List[AcquireAction]) -> Transaction:
         self.acquire_actions = acquire_actions
         return self
@@ -156,25 +216,27 @@
     @staticmethod
     def from_dict(
         data: Dict[str, Any],
     ) -> Optional[Transaction]:
         if data is None:
             return None
         return Transaction()\
+            .with_transaction_id(data.get('transactionId'))\
             .with_consume_actions([
                 ConsumeAction.from_dict(data.get('consumeActions')[i])
                 for i in range(len(data.get('consumeActions')) if data.get('consumeActions') else 0)
             ])\
             .with_acquire_actions([
                 AcquireAction.from_dict(data.get('acquireActions')[i])
                 for i in range(len(data.get('acquireActions')) if data.get('acquireActions') else 0)
             ])
 
     def to_dict(self) -> Dict[str, Any]:
         return {
+            "transactionId": self.transaction_id,
             "consumeActions": [
                 self.consume_actions[i].to_dict() if self.consume_actions[i] else None
                 for i in range(len(self.consume_actions) if self.consume_actions else 0)
             ],
             "acquireActions": [
                 self.acquire_actions[i].to_dict() if self.acquire_actions[i] else None
                 for i in range(len(self.acquire_actions) if self.acquire_actions else 0)
@@ -483,14 +545,15 @@
         }
 
 
 class Namespace(core.Gs2Model):
     namespace_id: str = None
     name: str = None
     description: str = None
+    transaction_setting: TransactionSetting = None
     log_setting: LogSetting = None
     created_at: int = None
     updated_at: int = None
     revision: int = None
 
     def with_namespace_id(self, namespace_id: str) -> Namespace:
         self.namespace_id = namespace_id
@@ -500,14 +563,18 @@
         self.name = name
         return self
 
     def with_description(self, description: str) -> Namespace:
         self.description = description
         return self
 
+    def with_transaction_setting(self, transaction_setting: TransactionSetting) -> Namespace:
+        self.transaction_setting = transaction_setting
+        return self
+
     def with_log_setting(self, log_setting: LogSetting) -> Namespace:
         self.log_setting = log_setting
         return self
 
     def with_created_at(self, created_at: int) -> Namespace:
         self.created_at = created_at
         return self
@@ -581,22 +648,24 @@
     ) -> Optional[Namespace]:
         if data is None:
             return None
         return Namespace()\
             .with_namespace_id(data.get('namespaceId'))\
             .with_name(data.get('name'))\
             .with_description(data.get('description'))\
+            .with_transaction_setting(TransactionSetting.from_dict(data.get('transactionSetting')))\
             .with_log_setting(LogSetting.from_dict(data.get('logSetting')))\
             .with_created_at(data.get('createdAt'))\
             .with_updated_at(data.get('updatedAt'))\
             .with_revision(data.get('revision'))
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "namespaceId": self.namespace_id,
             "name": self.name,
             "description": self.description,
+            "transactionSetting": self.transaction_setting.to_dict() if self.transaction_setting else None,
             "logSetting": self.log_setting.to_dict() if self.log_setting else None,
             "createdAt": self.created_at,
             "updatedAt": self.updated_at,
             "revision": self.revision,
         }
```

### Comparing `gs2-1.1.98/src/gs2/script/request.py` & `gs2-1.1.99/src/gs2/script/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,24 +61,29 @@
 
 
 class CreateNamespaceRequest(core.Gs2Request):
 
     context_stack: str = None
     name: str = None
     description: str = None
+    transaction_setting: TransactionSetting = None
     log_setting: LogSetting = None
 
     def with_name(self, name: str) -> CreateNamespaceRequest:
         self.name = name
         return self
 
     def with_description(self, description: str) -> CreateNamespaceRequest:
         self.description = description
         return self
 
+    def with_transaction_setting(self, transaction_setting: TransactionSetting) -> CreateNamespaceRequest:
+        self.transaction_setting = transaction_setting
+        return self
+
     def with_log_setting(self, log_setting: LogSetting) -> CreateNamespaceRequest:
         self.log_setting = log_setting
         return self
 
     def get(self, key, default=None):
         items = self.to_dict()
         if key in items.keys():
@@ -96,20 +101,22 @@
         data: Dict[str, Any],
     ) -> Optional[CreateNamespaceRequest]:
         if data is None:
             return None
         return CreateNamespaceRequest()\
             .with_name(data.get('name'))\
             .with_description(data.get('description'))\
+            .with_transaction_setting(TransactionSetting.from_dict(data.get('transactionSetting')))\
             .with_log_setting(LogSetting.from_dict(data.get('logSetting')))
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "name": self.name,
             "description": self.description,
+            "transactionSetting": self.transaction_setting.to_dict() if self.transaction_setting else None,
             "logSetting": self.log_setting.to_dict() if self.log_setting else None,
         }
 
 
 class GetNamespaceStatusRequest(core.Gs2Request):
 
     context_stack: str = None
@@ -183,24 +190,29 @@
 
 
 class UpdateNamespaceRequest(core.Gs2Request):
 
     context_stack: str = None
     namespace_name: str = None
     description: str = None
+    transaction_setting: TransactionSetting = None
     log_setting: LogSetting = None
 
     def with_namespace_name(self, namespace_name: str) -> UpdateNamespaceRequest:
         self.namespace_name = namespace_name
         return self
 
     def with_description(self, description: str) -> UpdateNamespaceRequest:
         self.description = description
         return self
 
+    def with_transaction_setting(self, transaction_setting: TransactionSetting) -> UpdateNamespaceRequest:
+        self.transaction_setting = transaction_setting
+        return self
+
     def with_log_setting(self, log_setting: LogSetting) -> UpdateNamespaceRequest:
         self.log_setting = log_setting
         return self
 
     def get(self, key, default=None):
         items = self.to_dict()
         if key in items.keys():
@@ -218,20 +230,22 @@
         data: Dict[str, Any],
     ) -> Optional[UpdateNamespaceRequest]:
         if data is None:
             return None
         return UpdateNamespaceRequest()\
             .with_namespace_name(data.get('namespaceName'))\
             .with_description(data.get('description'))\
+            .with_transaction_setting(TransactionSetting.from_dict(data.get('transactionSetting')))\
             .with_log_setting(LogSetting.from_dict(data.get('logSetting')))
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "namespaceName": self.namespace_name,
             "description": self.description,
+            "transactionSetting": self.transaction_setting.to_dict() if self.transaction_setting else None,
             "logSetting": self.log_setting.to_dict() if self.log_setting else None,
         }
 
 
 class DeleteNamespaceRequest(core.Gs2Request):
 
     context_stack: str = None
```

### Comparing `gs2-1.1.98/src/gs2/script/rest.py` & `gs2-1.1.99/src/gs2/script/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,16 @@
         body = {
             'contextStack': request.context_stack,
         }
         if request.name is not None:
             body["name"] = request.name
         if request.description is not None:
             body["description"] = request.description
+        if request.transaction_setting is not None:
+            body["transactionSetting"] = request.transaction_setting.to_dict()
         if request.log_setting is not None:
             body["logSetting"] = request.log_setting.to_dict()
 
         if request.request_id:
             headers["X-GS2-REQUEST-ID"] = request.request_id
         _job = rest.NetworkJob(
             url=url,
@@ -326,14 +328,16 @@
 
         headers = self._create_authorized_headers()
         body = {
             'contextStack': request.context_stack,
         }
         if request.description is not None:
             body["description"] = request.description
+        if request.transaction_setting is not None:
+            body["transactionSetting"] = request.transaction_setting.to_dict()
         if request.log_setting is not None:
             body["logSetting"] = request.log_setting.to_dict()
 
         if request.request_id:
             headers["X-GS2-REQUEST-ID"] = request.request_id
         _job = rest.NetworkJob(
             url=url,
```

### Comparing `gs2-1.1.98/src/gs2/script/result.py` & `gs2-1.1.99/src/gs2/script/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/script/web_socket.py` & `gs2-1.1.99/src/gs2/script/web_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,16 @@
 
         if request.context_stack:
             body['contextStack'] = str(request.context_stack)
         if request.name is not None:
             body["name"] = request.name
         if request.description is not None:
             body["description"] = request.description
+        if request.transaction_setting is not None:
+            body["transactionSetting"] = request.transaction_setting.to_dict()
         if request.log_setting is not None:
             body["logSetting"] = request.log_setting.to_dict()
 
         if request.request_id:
             body["xGs2RequestId"] = request.request_id
 
         self.session.send(
@@ -328,14 +330,16 @@
 
         if request.context_stack:
             body['contextStack'] = str(request.context_stack)
         if request.namespace_name is not None:
             body["namespaceName"] = request.namespace_name
         if request.description is not None:
             body["description"] = request.description
+        if request.transaction_setting is not None:
+            body["transactionSetting"] = request.transaction_setting.to_dict()
         if request.log_setting is not None:
             body["logSetting"] = request.log_setting.to_dict()
 
         if request.request_id:
             body["xGs2RequestId"] = request.request_id
 
         self.session.send(
```

### Comparing `gs2-1.1.98/src/gs2/serial_key/__init__.py` & `gs2-1.1.99/src/gs2/serial_key/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/serial_key/model.py` & `gs2-1.1.99/src/gs2/serial_key/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/serial_key/request.py` & `gs2-1.1.99/src/gs2/serial_key/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/serial_key/rest.py` & `gs2-1.1.99/src/gs2/serial_key/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/serial_key/result.py` & `gs2-1.1.99/src/gs2/serial_key/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/serial_key/web_socket.py` & `gs2-1.1.99/src/gs2/serial_key/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/showcase/__init__.py` & `gs2-1.1.99/src/gs2/showcase/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/showcase/model.py` & `gs2-1.1.99/src/gs2/showcase/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/showcase/request.py` & `gs2-1.1.99/src/gs2/showcase/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/showcase/rest.py` & `gs2-1.1.99/src/gs2/showcase/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/showcase/result.py` & `gs2-1.1.99/src/gs2/showcase/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/showcase/web_socket.py` & `gs2-1.1.99/src/gs2/showcase/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/skill_tree/__init__.py` & `gs2-1.1.99/src/gs2/skill_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/skill_tree/model.py` & `gs2-1.1.99/src/gs2/skill_tree/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/skill_tree/request.py` & `gs2-1.1.99/src/gs2/skill_tree/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/skill_tree/rest.py` & `gs2-1.1.99/src/gs2/skill_tree/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/skill_tree/result.py` & `gs2-1.1.99/src/gs2/skill_tree/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/skill_tree/web_socket.py` & `gs2-1.1.99/src/gs2/skill_tree/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/stamina/__init__.py` & `gs2-1.1.99/src/gs2/stamina/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/stamina/model.py` & `gs2-1.1.99/src/gs2/stamina/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/stamina/request.py` & `gs2-1.1.99/src/gs2/stamina/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/stamina/rest.py` & `gs2-1.1.99/src/gs2/stamina/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/stamina/result.py` & `gs2-1.1.99/src/gs2/stamina/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/stamina/web_socket.py` & `gs2-1.1.99/src/gs2/stamina/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/state_machine/__init__.py` & `gs2-1.1.99/src/gs2/state_machine/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/state_machine/model.py` & `gs2-1.1.99/src/gs2/state_machine/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/state_machine/request.py` & `gs2-1.1.99/src/gs2/state_machine/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/state_machine/rest.py` & `gs2-1.1.99/src/gs2/state_machine/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/state_machine/result.py` & `gs2-1.1.99/src/gs2/state_machine/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/state_machine/web_socket.py` & `gs2-1.1.99/src/gs2/state_machine/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/version/__init__.py` & `gs2-1.1.99/src/gs2/version/__init__.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/version/model.py` & `gs2-1.1.99/src/gs2/version/model.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/version/request.py` & `gs2-1.1.99/src/gs2/version/request.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/version/rest.py` & `gs2-1.1.99/src/gs2/version/rest.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/version/result.py` & `gs2-1.1.99/src/gs2/version/result.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2/version/web_socket.py` & `gs2-1.1.99/src/gs2/version/web_socket.py`

 * *Files identical despite different names*

### Comparing `gs2-1.1.98/src/gs2.egg-info/SOURCES.txt` & `gs2-1.1.99/src/gs2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

