# Comparing `tmp/sybil_engine-6.6.2.tar.gz` & `tmp/sybil_engine-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil_engine-6.6.2.tar", last modified: Sat Apr  6 17:38:29 2024, max compression
+gzip compressed data, was "sybil_engine-6.7.0.tar", last modified: Sun Apr 14 13:47:03 2024, max compression
```

## Comparing `sybil_engine-6.6.2.tar` & `sybil_engine-6.7.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.349102 sybil_engine-6.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-06 17:38:29.349102 sybil_engine-6.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:38:29.349102 sybil_engine-6.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.333102 sybil_engine-6.6.2/sybil_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.337102 sybil_engine-6.6.2/sybil_engine/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/config/app_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.337102 sybil_engine-6.6.2/sybil_engine/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/contract/erc20_test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/contract/erc20contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/contract/send.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/contract/transaction_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/contract/weth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.337102 sybil_engine-6.6.2/sybil_engine/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/data/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/data/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/data/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/data/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/data/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.337102 sybil_engine-6.6.2/sybil_engine/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/domain/account_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.337102 sybil_engine-6.6.2/sybil_engine/domain/balance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/domain/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/domain/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/domain/balance/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/domain/balance/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/domain/dex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/domain/generic_swap_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.341102 sybil_engine-6.6.2/sybil_engine/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/module/execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/module/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/module/module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/module/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.341102 sybil_engine-6.6.2/sybil_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/app_account_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/arguments_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/binance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/cex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/configuration_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/decryptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/fee_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/file_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/gas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/l0_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/okx_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/scal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/telegram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/validation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/wallet_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/sybil_engine/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.345102 sybil_engine-6.6.2/sybil_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-06 17:38:29.000000 sybil_engine-6.6.2/sybil_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-06 17:38:29.000000 sybil_engine-6.6.2/sybil_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:38:29.000000 sybil_engine-6.6.2/sybil_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 17:38:29.000000 sybil_engine-6.6.2/sybil_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 17:38:29.000000 sybil_engine-6.6.2/sybil_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.345102 sybil_engine-6.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.345102 sybil_engine-6.6.2/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/data/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/data/test_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.345102 sybil_engine-6.6.2/test/module/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.345102 sybil_engine-6.6.2/test/module/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/contract/mock_router.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/mock_fail_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/mock_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/mock_not_enoguth_native_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/repeatable_mock_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.345102 sybil_engine-6.6.2/test/module/swap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/swap/mock_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/swap/mock_test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/swap/test_dex.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/swap/test_swap_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/test_execution_planner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/test_module_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/module/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:29.345102 sybil_engine-6.6.2/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/utils/test_binance_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/utils/test_create_app_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 17:38:25.000000 sybil_engine-6.6.2/test/utils/test_validation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.503494 sybil_engine-6.7.0/sybil_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.507494 sybil_engine-6.7.0/sybil_engine/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/config/app_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.507494 sybil_engine-6.7.0/sybil_engine/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/erc20_test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/erc20contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/transaction_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/contract/weth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.507494 sybil_engine-6.7.0/sybil_engine/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/data/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.507494 sybil_engine-6.7.0/sybil_engine/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/account_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.511494 sybil_engine-6.7.0/sybil_engine/domain/balance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/balance/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/balance/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/domain/generic_swap_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.511494 sybil_engine-6.7.0/sybil_engine/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/module/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/sybil_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/app_account_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/arguments_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/binance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/cex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/configuration_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/decryptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/fee_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/file_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/gas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/l0_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/okx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/scal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/validation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/wallet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/sybil_engine/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/sybil_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 13:47:03.000000 sybil_engine-6.7.0/sybil_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/data/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/data/test_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/module/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/contract/mock_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/mock_fail_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/mock_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/mock_not_enoguth_native_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/repeatable_mock_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.515494 sybil_engine-6.7.0/test/module/swap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/mock_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/mock_test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/test_dex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/swap/test_swap_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/test_execution_planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/test_module_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/module/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:47:03.519494 sybil_engine-6.7.0/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/test_binance_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/test_create_app_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-14 13:46:59.000000 sybil_engine-6.7.0/test/utils/test_validation_utils.py
```

### Comparing `sybil_engine-6.6.2/PKG-INFO` & `sybil_engine-6.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.6.2
+Version: 6.7.0
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.0.3
```

### Comparing `sybil_engine-6.6.2/README.md` & `sybil_engine-6.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/setup.py` & `sybil_engine-6.7.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = file.readlines()
 
 setup(
     name='sybil_engine',
-    version='6.6.2',
+    version='6.7.0',
     py_modules=['sybil_engine'],
     packages=find_packages(),
     install_requires=requirements,
     data_files=[('', ['requirements.txt'])],
     author='Indeoo',
     author_email='indeooars@gmail.com',
     description='Engine for web3 smart contracts automatization.',
```

### Comparing `sybil_engine-6.6.2/sybil_engine/app.py` & `sybil_engine-6.7.0/sybil_engine/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from loguru import logger
 
 from sybil_engine.config.app_config import set_network, set_gas_prices, set_dex_retry_interval, set_module_data, \
-    set_cex_data
+    set_cex_data, set_cex_conf
 from sybil_engine.module.execution_planner import create_execution_plans
 from sybil_engine.module.module_executor import ModuleExecutor
 from sybil_engine.utils.accumulator import print_accumulated, add_accumulator_str
 from sybil_engine.utils.app_account_utils import create_app_account
 from sybil_engine.utils.arguments_parser import parse_arguments, parse_profile
 from sybil_engine.utils.configuration_loader import load_config_maps, load_module_vars
 from sybil_engine.utils.fee_storage import print_fee
@@ -85,14 +85,15 @@
      gas_price, account_creation_mode, cex_address_validation, interactive_confirmation) = config
 
     set_network(args.network)
     set_dex_retry_interval(swap_retry_sleep_interval)
     set_gas_prices(gas_price)
     set_module_data(modules_data)
     set_cex_data((args.password.encode('utf-8'), cex_data))
+    set_cex_conf(args.cex_conf)
 
     logger.info(f"START {module_config['scenario_name']} module in {args.network}")
 
     profile = parse_profile().profile
     logger.info(f"Profile {profile} activated")
 
     if not all(modules_data.get_module_class_by_name(module['module']) for module in module_config['scenario']):
```

### Comparing `sybil_engine-6.6.2/sybil_engine/config/app_config.py` & `sybil_engine-6.7.0/sybil_engine/config/app_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 network = None
 dex_retry_interval = None
 gas_prices_gwei = None
 module_data = None
 cex_data = None, None, None
+cex_conf = None
 
 
 def set_network(value):
     global network
     network = value
 
 
@@ -44,7 +45,16 @@
 def set_cex_data(value):
     global cex_data
     cex_data = value
 
 
 def get_cex_data():
     return cex_data
+
+
+def set_cex_conf(value):
+    global cex_conf
+    cex_conf = value
+
+
+def get_cex_conf():
+    return cex_conf
```

### Comparing `sybil_engine-6.6.2/sybil_engine/contract/contract.py` & `sybil_engine-6.7.0/sybil_engine/contract/contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/contract/erc20_test_contract.py` & `sybil_engine-6.7.0/sybil_engine/contract/erc20_test_contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/contract/erc20contract.py` & `sybil_engine-6.7.0/sybil_engine/contract/erc20contract.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/contract/send.py` & `sybil_engine-6.7.0/sybil_engine/contract/send.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/contract/transaction_executor.py` & `sybil_engine-6.7.0/sybil_engine/contract/transaction_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/contract/weth.py` & `sybil_engine-6.7.0/sybil_engine/contract/weth.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/data/contracts.py` & `sybil_engine-6.7.0/sybil_engine/data/contracts.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/data/networks.py` & `sybil_engine-6.7.0/sybil_engine/data/networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/data/pairs.py` & `sybil_engine-6.7.0/sybil_engine/data/pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/data/tokens.py` & `sybil_engine-6.7.0/sybil_engine/data/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/domain/balance/balance.py` & `sybil_engine-6.7.0/sybil_engine/domain/balance/balance.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/domain/balance/balance_utils.py` & `sybil_engine-6.7.0/sybil_engine/domain/balance/balance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/domain/balance/tokens.py` & `sybil_engine-6.7.0/sybil_engine/domain/balance/tokens.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/domain/dex.py` & `sybil_engine-6.7.0/sybil_engine/domain/dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/domain/generic_swap_facade.py` & `sybil_engine-6.7.0/sybil_engine/domain/generic_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/module/execution_planner.py` & `sybil_engine-6.7.0/sybil_engine/module/execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/module/module.py` & `sybil_engine-6.7.0/sybil_engine/module/module.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/module/module_executor.py` & `sybil_engine-6.7.0/sybil_engine/module/module_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/module/modules.py` & `sybil_engine-6.7.0/sybil_engine/module/modules.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/accumulator.py` & `sybil_engine-6.7.0/sybil_engine/utils/accumulator.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/app_account_utils.py` & `sybil_engine-6.7.0/sybil_engine/utils/app_account_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         )
     elif account_creation_mode == 'CSV':
         accounts = create_app_accounts_from_csv(args.account_csv, args.password.encode('utf-8'), encryption)
     else:
         raise ConfigurationException("account_creation_mode should be CSV or TXT")
 
     if cex_address_validation:
-        validate_cex_addresses(accounts, get_cex_addresses())
+        validate_cex_addresses(accounts, get_cex_addresses(args.cex_conf))
 
     return accounts
 
 
 def create_app_accounts_from_txt(private_keys, proxy_config, cex_addresses, starknet_addresses, password, encryption):
     proxy_mode, proxy_file = proxy_config
```

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/arguments_parser.py` & `sybil_engine-6.7.0/sybil_engine/utils/arguments_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,16 @@
                         help='a string to be processed')
     parser.add_argument('--password', type=str, required=False, default=os.environ.get('PASSWORD', default_password),
                         help='a string to be processed')
     parser.add_argument('--network', type=str, required=False, default=os.environ.get('NETWORK', 'MAIN'),
                         help='a string to be processed')
     parser.add_argument('--module', type=str, required=False, default=os.environ.get('MODULE', default_module),
                         help='a string to be processed')
+    parser.add_argument('--cex_conf', type=str, required=False, default=os.environ.get('CEX_CONF', 'okx'),
+                        help='a string to be processed')
 
     args = parser.parse_args()
 
     if '--private_keys' not in sys.argv:
         args.private_keys = os.path.join(args.wallets, 'private_keys.txt')
     if '--cex_addresses' not in sys.argv:
         args.cex_addresses = os.path.join(args.wallets, 'cex_addresses.txt')
```

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/binance_prices.py` & `sybil_engine-6.7.0/sybil_engine/utils/binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/binance_utils.py` & `sybil_engine-6.7.0/sybil_engine/utils/binance_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/configuration_loader.py` & `sybil_engine-6.7.0/sybil_engine/utils/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/decryptor.py` & `sybil_engine-6.7.0/sybil_engine/utils/decryptor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/fee_storage.py` & `sybil_engine-6.7.0/sybil_engine/utils/fee_storage.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/gas_utils.py` & `sybil_engine-6.7.0/sybil_engine/utils/gas_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/logs.py` & `sybil_engine-6.7.0/sybil_engine/utils/logs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/okx_utils.py` & `sybil_engine-6.7.0/sybil_engine/utils/okx_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/retry.py` & `sybil_engine-6.7.0/sybil_engine/utils/retry.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/scal_utils.py` & `sybil_engine-6.7.0/sybil_engine/utils/scal_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/telegram.py` & `sybil_engine-6.7.0/sybil_engine/utils/telegram.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/utils.py` & `sybil_engine-6.7.0/sybil_engine/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/validation_utils.py` & `sybil_engine-6.7.0/sybil_engine/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine/utils/web3_utils.py` & `sybil_engine-6.7.0/sybil_engine/utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/sybil_engine.egg-info/PKG-INFO` & `sybil_engine-6.7.0/sybil_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil_engine
-Version: 6.6.2
+Version: 6.7.0
 Summary: Engine for web3 smart contracts automatization.
 Home-page: https://github.com/Indeoo/sybil-engine/
 Author: Indeoo
 Author-email: indeooars@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: setuptools==69.0.3
```

### Comparing `sybil_engine-6.6.2/sybil_engine.egg-info/SOURCES.txt` & `sybil_engine-6.7.0/sybil_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/__init__.py` & `sybil_engine-6.7.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/data/test_networks.py` & `sybil_engine-6.7.0/test/data/test_networks.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/data/test_pairs.py` & `sybil_engine-6.7.0/test/data/test_pairs.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/module/contract/mock_router.py` & `sybil_engine-6.7.0/test/module/contract/mock_router.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/module/swap/mock_dex.py` & `sybil_engine-6.7.0/test/module/swap/mock_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/module/swap/mock_test_swap_facade.py` & `sybil_engine-6.7.0/test/module/swap/mock_test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/module/swap/test_dex.py` & `sybil_engine-6.7.0/test/module/swap/test_dex.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/module/swap/test_swap_facade.py` & `sybil_engine-6.7.0/test/module/swap/test_swap_facade.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/module/test_execution_planner.py` & `sybil_engine-6.7.0/test/module/test_execution_planner.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/module/test_module_executor.py` & `sybil_engine-6.7.0/test/module/test_module_executor.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/test_config.py` & `sybil_engine-6.7.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/utils/test_binance_prices.py` & `sybil_engine-6.7.0/test/utils/test_binance_prices.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/utils/test_create_app_accounts.py` & `sybil_engine-6.7.0/test/utils/test_create_app_accounts.py`

 * *Files identical despite different names*

### Comparing `sybil_engine-6.6.2/test/utils/test_validation_utils.py` & `sybil_engine-6.7.0/test/utils/test_validation_utils.py`

 * *Files identical despite different names*

