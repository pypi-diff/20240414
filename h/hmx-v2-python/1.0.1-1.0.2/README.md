# Comparing `tmp/hmx-v2-python-1.0.1.tar.gz` & `tmp/hmx-v2-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmx-v2-python-1.0.1.tar", last modified: Mon Mar 25 02:56:53 2024, max compression
+gzip compressed data, was "hmx-v2-python-1.0.2.tar", last modified: Sun Apr 14 03:17:59 2024, max compression
```

## Comparing `hmx-v2-python-1.0.1.tar` & `hmx-v2-python-1.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.434116 hmx-v2-python-1.0.1/
--rw-r--r--   0 adirut     (501) staff       (20)     1064 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/LICENSE
--rw-r--r--   0 adirut     (501) staff       (20)     4302 2024-03-25 02:56:53.434255 hmx-v2-python-1.0.1/PKG-INFO
--rw-r--r--   0 adirut     (501) staff       (20)     3313 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.1/README.md
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.419540 hmx-v2-python-1.0.1/hmx2/
--rw-r--r--   0 adirut     (501) staff       (20)       35 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.426506 hmx-v2-python-1.0.1/hmx2/abis/
--rw-r--r--   0 adirut     (501) staff       (20)     6094 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.1/hmx2/abis/CIXPriceAdapter.json
--rw-r--r--   0 adirut     (501) staff       (20)    19788 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/abis/Calculator.json
--rw-r--r--   0 adirut     (501) staff       (20)    79531 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/abis/ConfigStorage.json
--rw-r--r--   0 adirut     (501) staff       (20)    23809 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/abis/CrossMarginHandler.json
--rw-r--r--   0 adirut     (501) staff       (20)     3685 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/abis/ERC20.json
--rw-r--r--   0 adirut     (501) staff       (20)    11832 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/abis/GlpManager.json
--rw-r--r--   0 adirut     (501) staff       (20)     5780 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.1/hmx2/abis/GmPriceAdapter.json
--rw-r--r--   0 adirut     (501) staff       (20)    47380 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/abis/LimitTradeHandler.json
--rw-r--r--   0 adirut     (501) staff       (20)     2419 2024-01-15 08:58:17.000000 hmx-v2-python-1.0.1/hmx2/abis/OnchainPricelens.json
--rw-r--r--   0 adirut     (501) staff       (20)    26127 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/abis/PerpStorage.json
--rw-r--r--   0 adirut     (501) staff       (20)    27073 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/abis/TradeHelper.json
--rw-r--r--   0 adirut     (501) staff       (20)    24329 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/abis/VaultStorage.json
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.428418 hmx-v2-python-1.0.1/hmx2/constants/
--rw-r--r--   0 adirut     (501) staff       (20)       97 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.1/hmx2/constants/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1917 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/constants/assets.py
--rw-r--r--   0 adirut     (501) staff       (20)      294 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/constants/common.py
--rw-r--r--   0 adirut     (501) staff       (20)     1700 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/constants/contracts.py
--rw-r--r--   0 adirut     (501) staff       (20)     7052 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/constants/markets.py
--rw-r--r--   0 adirut     (501) staff       (20)    10357 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/constants/pricefeed.py
--rw-r--r--   0 adirut     (501) staff       (20)     4970 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.1/hmx2/constants/tokens.py
--rw-r--r--   0 adirut     (501) staff       (20)      118 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/enum.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.429078 hmx-v2-python-1.0.1/hmx2/helpers/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/helpers/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)      347 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/helpers/contract_loader.py
--rw-r--r--   0 adirut     (501) staff       (20)      519 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/helpers/mapper.py
--rw-r--r--   0 adirut     (501) staff       (20)      448 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/helpers/util.py
--rw-r--r--   0 adirut     (501) staff       (20)     2771 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/hmx_client.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.429709 hmx-v2-python-1.0.1/hmx2/modules/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/modules/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.430243 hmx-v2-python-1.0.1/hmx2/modules/calculator/
--rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/modules/calculator/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     6048 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/calculator/calculator.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.430841 hmx-v2-python-1.0.1/hmx2/modules/oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       48 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/__init__.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.431200 hmx-v2-python-1.0.1/hmx2/modules/oracle/cix_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/cix_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1315 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/cix_oracle/cix_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.431472 hmx-v2-python-1.0.1/hmx2/modules/oracle/glp_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/glp_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1003 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/glp_oracle/glp_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.431754 hmx-v2-python-1.0.1/hmx2/modules/oracle/gm_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       32 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/gm_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1169 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/gm_oracle/gm_oracle.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.432106 hmx-v2-python-1.0.1/hmx2/modules/oracle/onchain_pricelens_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       59 2024-01-15 08:58:17.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)      788 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
--rw-r--r--   0 adirut     (501) staff       (20)     3180 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/oracle_middleware.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.432369 hmx-v2-python-1.0.1/hmx2/modules/oracle/pyth_oracle/
--rw-r--r--   0 adirut     (501) staff       (20)       36 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/pyth_oracle/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     1302 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
--rw-r--r--   0 adirut     (501) staff       (20)    15118 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/private.py
--rw-r--r--   0 adirut     (501) staff       (20)    27327 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/hmx2/modules/public.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.433020 hmx-v2-python-1.0.1/hmx_v2_python.egg-info/
--rw-r--r--   0 adirut     (501) staff       (20)     4302 2024-03-25 02:56:53.000000 hmx-v2-python-1.0.1/hmx_v2_python.egg-info/PKG-INFO
--rw-r--r--   0 adirut     (501) staff       (20)     1752 2024-03-25 02:56:53.000000 hmx-v2-python-1.0.1/hmx_v2_python.egg-info/SOURCES.txt
--rw-r--r--   0 adirut     (501) staff       (20)        1 2024-03-25 02:56:53.000000 hmx-v2-python-1.0.1/hmx_v2_python.egg-info/dependency_links.txt
--rw-r--r--   0 adirut     (501) staff       (20)      154 2024-03-25 02:56:53.000000 hmx-v2-python-1.0.1/hmx_v2_python.egg-info/requires.txt
--rw-r--r--   0 adirut     (501) staff       (20)       11 2024-03-25 02:56:53.000000 hmx-v2-python-1.0.1/hmx_v2_python.egg-info/top_level.txt
--rw-r--r--   0 adirut     (501) staff       (20)       79 2024-03-25 02:56:53.434431 hmx-v2-python-1.0.1/setup.cfg
--rw-r--r--   0 adirut     (501) staff       (20)     1456 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.1/setup.py
-drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-03-25 02:56:53.433988 hmx-v2-python-1.0.1/tests/
--rw-r--r--   0 adirut     (501) staff       (20)       46 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/tests/__init__.py
--rw-r--r--   0 adirut     (501) staff       (20)     5934 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/tests/constants.py
--rw-r--r--   0 adirut     (501) staff       (20)     3117 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.1/tests/test_create_market_order.py
--rw-r--r--   0 adirut     (501) staff       (20)     5393 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.1/tests/test_deposit_collateral.py
--rw-r--r--   0 adirut     (501) staff       (20)     1307 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.1/tests/test_get_adaptive_fee.py
--rw-r--r--   0 adirut     (501) staff       (20)     1221 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.1/tests/test_init.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.507400 hmx-v2-python-1.0.2/
+-rw-r--r--   0 adirut     (501) staff       (20)     1064 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/LICENSE
+-rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-04-14 03:17:59.507530 hmx-v2-python-1.0.2/PKG-INFO
+-rw-r--r--   0 adirut     (501) staff       (20)     3361 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/README.md
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.497088 hmx-v2-python-1.0.2/hmx2/
+-rw-r--r--   0 adirut     (501) staff       (20)       35 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.501105 hmx-v2-python-1.0.2/hmx2/abis/
+-rw-r--r--   0 adirut     (501) staff       (20)     6094 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.2/hmx2/abis/CIXPriceAdapter.json
+-rw-r--r--   0 adirut     (501) staff       (20)    19788 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/abis/Calculator.json
+-rw-r--r--   0 adirut     (501) staff       (20)    79531 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/ConfigStorage.json
+-rw-r--r--   0 adirut     (501) staff       (20)    23809 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/CrossMarginHandler.json
+-rw-r--r--   0 adirut     (501) staff       (20)     3685 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/ERC20.json
+-rw-r--r--   0 adirut     (501) staff       (20)    11832 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/GlpManager.json
+-rw-r--r--   0 adirut     (501) staff       (20)     5780 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.2/hmx2/abis/GmPriceAdapter.json
+-rw-r--r--   0 adirut     (501) staff       (20)    47380 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/LimitTradeHandler.json
+-rw-r--r--   0 adirut     (501) staff       (20)     2419 2024-01-15 08:58:17.000000 hmx-v2-python-1.0.2/hmx2/abis/OnchainPricelens.json
+-rw-r--r--   0 adirut     (501) staff       (20)    26127 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/PerpStorage.json
+-rw-r--r--   0 adirut     (501) staff       (20)    27073 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/abis/TradeHelper.json
+-rw-r--r--   0 adirut     (501) staff       (20)    24329 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/abis/VaultStorage.json
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.502179 hmx-v2-python-1.0.2/hmx2/constants/
+-rw-r--r--   0 adirut     (501) staff       (20)       97 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.2/hmx2/constants/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1953 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/constants/assets.py
+-rw-r--r--   0 adirut     (501) staff       (20)      294 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/constants/common.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1700 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/constants/contracts.py
+-rw-r--r--   0 adirut     (501) staff       (20)     7052 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/constants/markets.py
+-rw-r--r--   0 adirut     (501) staff       (20)    10357 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/constants/pricefeed.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5414 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/constants/tokens.py
+-rw-r--r--   0 adirut     (501) staff       (20)      118 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/enum.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.502660 hmx-v2-python-1.0.2/hmx2/helpers/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/helpers/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)      347 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/helpers/contract_loader.py
+-rw-r--r--   0 adirut     (501) staff       (20)      519 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/helpers/mapper.py
+-rw-r--r--   0 adirut     (501) staff       (20)      636 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/helpers/util.py
+-rw-r--r--   0 adirut     (501) staff       (20)     2771 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/hmx_client.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.503198 hmx-v2-python-1.0.2/hmx2/modules/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.503466 hmx-v2-python-1.0.2/hmx2/modules/calculator/
+-rw-r--r--   0 adirut     (501) staff       (20)        0 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/calculator/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     6048 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/calculator/calculator.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.503785 hmx-v2-python-1.0.2/hmx2/modules/oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       48 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/__init__.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.504031 hmx-v2-python-1.0.2/hmx2/modules/oracle/cix_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/cix_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1315 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/cix_oracle/cix_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.504294 hmx-v2-python-1.0.2/hmx2/modules/oracle/glp_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       34 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/glp_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1003 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/glp_oracle/glp_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.504515 hmx-v2-python-1.0.2/hmx2/modules/oracle/gm_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       32 2023-12-01 07:58:15.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/gm_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1169 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/gm_oracle/gm_oracle.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.505109 hmx-v2-python-1.0.2/hmx2/modules/oracle/onchain_pricelens_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       59 2024-01-15 08:58:17.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/onchain_pricelens_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)      788 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3321 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/oracle_middleware.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.505457 hmx-v2-python-1.0.2/hmx2/modules/oracle/pyth_oracle/
+-rw-r--r--   0 adirut     (501) staff       (20)       36 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/pyth_oracle/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1302 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py
+-rw-r--r--   0 adirut     (501) staff       (20)    14072 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/modules/private.py
+-rw-r--r--   0 adirut     (501) staff       (20)    29226 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/hmx2/modules/public.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.506411 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/
+-rw-r--r--   0 adirut     (501) staff       (20)     4350 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/PKG-INFO
+-rw-r--r--   0 adirut     (501) staff       (20)     1752 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/SOURCES.txt
+-rw-r--r--   0 adirut     (501) staff       (20)        1 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/dependency_links.txt
+-rw-r--r--   0 adirut     (501) staff       (20)      154 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/requires.txt
+-rw-r--r--   0 adirut     (501) staff       (20)       11 2024-04-14 03:17:59.000000 hmx-v2-python-1.0.2/hmx_v2_python.egg-info/top_level.txt
+-rw-r--r--   0 adirut     (501) staff       (20)       79 2024-04-14 03:17:59.507758 hmx-v2-python-1.0.2/setup.cfg
+-rw-r--r--   0 adirut     (501) staff       (20)     1456 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/setup.py
+drwxr-xr-x   0 adirut     (501) staff       (20)        0 2024-04-14 03:17:59.507294 hmx-v2-python-1.0.2/tests/
+-rw-r--r--   0 adirut     (501) staff       (20)       46 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/tests/__init__.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5934 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/tests/constants.py
+-rw-r--r--   0 adirut     (501) staff       (20)     3117 2024-03-22 14:32:06.000000 hmx-v2-python-1.0.2/tests/test_create_market_order.py
+-rw-r--r--   0 adirut     (501) staff       (20)     5522 2024-04-14 03:17:48.000000 hmx-v2-python-1.0.2/tests/test_deposit_collateral.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1307 2024-03-18 08:59:51.000000 hmx-v2-python-1.0.2/tests/test_get_adaptive_fee.py
+-rw-r--r--   0 adirut     (501) staff       (20)     1221 2023-12-01 04:47:34.000000 hmx-v2-python-1.0.2/tests/test_init.py
```

### Comparing `hmx-v2-python-1.0.1/LICENSE` & `hmx-v2-python-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/PKG-INFO` & `hmx-v2-python-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Platform: UNKNOWN
@@ -50,23 +50,23 @@
 #
 # Using publicly access functions
 #
 hmx_client = Client(
     rpc_url=RPC_URL
 )
 # Get oracle price, adaptive price, and price impact of a new position
-client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
+hmx_client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
 # Get market information
-client.public.get_market_info(MARKET_ETH_USD)
+hmx_client.public.get_market_info(MARKET_ETH_USD)
 # Get sub account in address format
-client.public.get_sub_account(1)
+hmx_client.public.get_sub_account(1)
 # Get position ID
-client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
 # Get position info
-client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
 ```
 
 ### Private function
 
 ```python
 from hmx2.hmx_client import Client
 from hmx2.constants.markets import MARKET_ETH_USD
@@ -77,43 +77,43 @@
 # Initailized client with private key
 #
 hmx_client = Client(
     eth_private_key=PRIVATE_KEY,
     rpc_url=RPC_URL
 )
 # Get public address of the ethereum key
-client.private.get_public_address()
+hmx_client.private.get_public_address()
 # Deposit ETH as collateral
-client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
+hmx_client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
 # Deposit ERC20 as collateral. This function will automatically
 # approve CrossMarginHandler if needed.
-client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
+hmx_client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
 # Create a market order
-create_market_order = client.private.create_market_order(
+create_market_order = hmx_client.private.create_market_order(
   sub_account_id=0, market_index=MARKET_ETH_USD, buy=Action.BUY, size=100, reduce_only=False
 )
 print(create_market_order)
 # Create a trigger order
 # trigger_above_threshold = The current price must go above (if True) or below (if False)
 # the trigger price in order for the order to be executed
-create_order = client.private.create_trigger_order(
+create_order = hmx_client.private.create_trigger_order(
   sub_account_id=0,
   market_index=MARKET_ETH_USD,
   buy=Action.BUY,
   size=100,
   trigger_price=1800,
   trigger_above_threshold=True,
   reduce_only=False)
 print(create_order)
 # Update the order
-update_order = client.private.update_trigger_order(
+update_order = hmx_client.private.update_trigger_order(
   0, create_order["order"]["orderIndex"], Action.SELL, 50, 1700, True, False)
 print(update_order)
 # Cancel the order
-cancel_order = client.private.cancel_trigger_order(
+cancel_order = hmx_client.private.cancel_trigger_order(
   0, update_order["order"]["orderIndex"])
 ```
 
 ## Running Tests
 
 To run tests, you will need have to clone the repo, update .env, and run:
```

### Comparing `hmx-v2-python-1.0.1/README.md` & `hmx-v2-python-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 #
 # Using publicly access functions
 #
 hmx_client = Client(
     rpc_url=RPC_URL
 )
 # Get oracle price, adaptive price, and price impact of a new position
-client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
+hmx_client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
 # Get market information
-client.public.get_market_info(MARKET_ETH_USD)
+hmx_client.public.get_market_info(MARKET_ETH_USD)
 # Get sub account in address format
-client.public.get_sub_account(1)
+hmx_client.public.get_sub_account(1)
 # Get position ID
-client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
 # Get position info
-client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
 ```
 
 ### Private function
 
 ```python
 from hmx2.hmx_client import Client
 from hmx2.constants.markets import MARKET_ETH_USD
@@ -51,43 +51,43 @@
 # Initailized client with private key
 #
 hmx_client = Client(
     eth_private_key=PRIVATE_KEY,
     rpc_url=RPC_URL
 )
 # Get public address of the ethereum key
-client.private.get_public_address()
+hmx_client.private.get_public_address()
 # Deposit ETH as collateral
-client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
+hmx_client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
 # Deposit ERC20 as collateral. This function will automatically
 # approve CrossMarginHandler if needed.
-client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
+hmx_client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
 # Create a market order
-create_market_order = client.private.create_market_order(
+create_market_order = hmx_client.private.create_market_order(
   sub_account_id=0, market_index=MARKET_ETH_USD, buy=Action.BUY, size=100, reduce_only=False
 )
 print(create_market_order)
 # Create a trigger order
 # trigger_above_threshold = The current price must go above (if True) or below (if False)
 # the trigger price in order for the order to be executed
-create_order = client.private.create_trigger_order(
+create_order = hmx_client.private.create_trigger_order(
   sub_account_id=0,
   market_index=MARKET_ETH_USD,
   buy=Action.BUY,
   size=100,
   trigger_price=1800,
   trigger_above_threshold=True,
   reduce_only=False)
 print(create_order)
 # Update the order
-update_order = client.private.update_trigger_order(
+update_order = hmx_client.private.update_trigger_order(
   0, create_order["order"]["orderIndex"], Action.SELL, 50, 1700, True, False)
 print(update_order)
 # Cancel the order
-cancel_order = client.private.cancel_trigger_order(
+cancel_order = hmx_client.private.cancel_trigger_order(
   0, update_order["order"]["orderIndex"])
 ```
 
 ## Running Tests
 
 To run tests, you will need have to clone the repo, update .env, and run:
```

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/CIXPriceAdapter.json` & `hmx-v2-python-1.0.2/hmx2/abis/CIXPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/Calculator.json` & `hmx-v2-python-1.0.2/hmx2/abis/Calculator.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/ConfigStorage.json` & `hmx-v2-python-1.0.2/hmx2/abis/ConfigStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/CrossMarginHandler.json` & `hmx-v2-python-1.0.2/hmx2/abis/CrossMarginHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/ERC20.json` & `hmx-v2-python-1.0.2/hmx2/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/GlpManager.json` & `hmx-v2-python-1.0.2/hmx2/abis/GlpManager.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/GmPriceAdapter.json` & `hmx-v2-python-1.0.2/hmx2/abis/GmPriceAdapter.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/LimitTradeHandler.json` & `hmx-v2-python-1.0.2/hmx2/abis/LimitTradeHandler.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/OnchainPricelens.json` & `hmx-v2-python-1.0.2/hmx2/abis/OnchainPricelens.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/PerpStorage.json` & `hmx-v2-python-1.0.2/hmx2/abis/PerpStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/TradeHelper.json` & `hmx-v2-python-1.0.2/hmx2/abis/TradeHelper.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/abis/VaultStorage.json` & `hmx-v2-python-1.0.2/hmx2/abis/VaultStorage.json`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/constants/assets.py` & `hmx-v2-python-1.0.2/hmx2/constants/assets.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ASSET_COIN = "COIN"
 ASSET_GOOG = "GOOG"
 ASSET_BNB = "BNB"
 ASSET_SOL = "SOL"
 ASSET_QQQ = "QQQ"
 ASSET_XRP = "XRP"
 ASSET_USDC = "USDC"
+ASSET_USDCe = "USDC.e"
 ASSET_USDT = "USDT"
 ASSET_DAI = "DAI"
 ASSET_GLP = "GLP"
 ASSET_NVDA = "NVDA"
 ASSET_LINK = "LINK"
 ASSET_CHF = "CHF"
 ASSET_DOGE = "DOGE"
@@ -63,8 +64,8 @@
           ASSET_ADA, ASSET_MATIC, ASSET_SUI, ASSET_ARB, ASSET_OP, ASSET_LTC,
           ASSET_COIN, ASSET_GOOG, ASSET_BNB, ASSET_SOL, ASSET_QQQ, ASSET_XRP,
           ASSET_USDC, ASSET_USDT, ASSET_DAI, ASSET_GLP, ASSET_NVDA, ASSET_LINK,
           ASSET_CHF, ASSET_DOGE, ASSET_CAD, ASSET_SGD, ASSET_CNH, ASSET_wstETH,
           ASSET_HKD, ASSET_BCH, ASSET_MEME, ASSET_gmBTC, ASSET_gmETH, ASSET_SEK,
           ASSET_DIX, ASSET_JTO, ASSET_STX, ASSET_ORDI, ASSET_TIA, ASSET_AVAX,
           ASSET_INJ, ASSET_DOT, ASSET_SEI, ASSET_ATOM, ASSET_1000SHIB, ASSET_1000PEPE,
-          ASSET_ICP, ASSET_MANTA, ASSET_STRK, ASSET_PYTH]
+          ASSET_ICP, ASSET_MANTA, ASSET_STRK, ASSET_PYTH, ASSET_USDCe]
```

### Comparing `hmx-v2-python-1.0.1/hmx2/constants/contracts.py` & `hmx-v2-python-1.0.2/hmx2/constants/contracts.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/constants/markets.py` & `hmx-v2-python-1.0.2/hmx2/constants/markets.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/constants/pricefeed.py` & `hmx-v2-python-1.0.2/hmx2/constants/pricefeed.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/helpers/mapper.py` & `hmx-v2-python-1.0.2/hmx2/helpers/mapper.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/hmx_client.py` & `hmx-v2-python-1.0.2/hmx2/hmx_client.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/calculator/calculator.py` & `hmx-v2-python-1.0.2/hmx2/modules/calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/oracle/cix_oracle/cix_oracle.py` & `hmx-v2-python-1.0.2/hmx2/modules/oracle/cix_oracle/cix_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/oracle/glp_oracle/glp_oracle.py` & `hmx-v2-python-1.0.2/hmx2/modules/oracle/glp_oracle/glp_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/oracle/gm_oracle/gm_oracle.py` & `hmx-v2-python-1.0.2/hmx2/modules/oracle/gm_oracle/gm_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py` & `hmx-v2-python-1.0.2/hmx2/modules/oracle/onchain_pricelens_oracle/onchain_pricelen_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/oracle/oracle_middleware.py` & `hmx-v2-python-1.0.2/hmx2/modules/oracle/oracle_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from hmx2.modules.oracle.pyth_oracle import PythOracle
 from hmx2.modules.oracle.glp_oracle import GlpOracle
 from hmx2.modules.oracle.cix_oracle import CixOracle
 from hmx2.modules.oracle.gm_oracle import GmOracle
 from hmx2.modules.oracle.onchain_pricelens_oracle import OnchainPricelensOracle
 from hmx2.constants.assets import (
   ASSETS,
+  ASSET_USDCe,
   ASSET_gmBTC,
   ASSET_gmETH,
   ASSET_DIX,
   ASSET_GLP,
   ASSET_wstETH,
   ASSET_1000PEPE,
   ASSET_1000SHIB,
@@ -83,14 +84,17 @@
       price_object[ASSET_gmETH] = self.gm_eth_oracle.get_price(ASSET_gmETH)
       asset_ids.remove(ASSET_gmETH)
 
     if ASSET_wstETH in asset_ids:
       price_object[ASSET_wstETH] = self.onchain_pricelens_oracle.get_price(
         ASSET_wstETH)
       asset_ids.remove(ASSET_wstETH)
+    if ASSET_USDCe in asset_ids:
+      price_object[ASSET_USDCe] = self.get_price("USDC")
+      asset_ids.remove(ASSET_USDCe)
 
     raw_prices = self.pyth_oracle.get_multiple_price(asset_ids)
 
     for index, asset_id in enumerate(asset_ids):
       if asset_id in [ASSET_1000PEPE, ASSET_1000SHIB]:
         price_object[asset_id] = raw_prices[index] * 1000
```

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py` & `hmx-v2-python-1.0.2/hmx2/modules/oracle/pyth_oracle/pyth_oracle.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/private.py` & `hmx-v2-python-1.0.2/hmx2/modules/private.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from simple_multicall_v6 import Multicall
 from hmx2.helpers.mapper import (
   get_contract_address,
   get_token_profile,
   get_collateral_address_asset_map,
   get_collateral_address_list
 )
+from hmx2.helpers.util import check_sub_account_id_param
 from hmx2.modules.oracle.oracle_middleware import OracleMiddleware
 from eth_abi.abi import encode
 import decimal
 
 decimal.getcontext().prec = 15
 decimal.getcontext().rounding = "ROUND_HALF_DOWN"
 
@@ -62,50 +63,14 @@
       self.eth_provider, self.contract_address["CROSS_MARGIN_HANDLER_ADDRESS"], CROSS_MARGIN_HANDLER_ABI_PATH)
     self.calculator_instance = load_contract(
       self.eth_provider, self.contract_address["CALCULATOR_ADDRESS"], CALCULATOR_ABI_PATH
     )
     self.multicall_instance = Multicall(w3=self.eth_provider,
                                         custom_address=self.contract_address["MULTICALL_ADDRESS"])
 
-  def get_public_address(self):
-    '''
-    Get the public address of the signer.
-    '''
-    return self.eth_signer.address
-
-  def get_collaterals(self, sub_account_id: int):
-    self.__check_sub_account_id_param(sub_account_id)
-
-    calls = [
-      self.multicall_instance.create_call(
-        self.vault_storage_instance,
-          "traderBalances",
-          [self.eth_signer.address, collateral],
-      )
-      for collateral in self.collateral_address_list
-    ]
-    collateral_usd = [
-      self.oracle_middleware.get_price(
-        self.collateral_address_asset_map[collateral])
-      for collateral in self.collateral_address_list
-    ]
-
-    results = self.multicall_instance.call(calls)
-
-    ret = {}
-    for index, collateral in enumerate(self.collateral_address_list):
-      amount = int(
-          results[1][index].hex(), 16) / 10 ** self.token_profile[collateral]["decimals"]
-      ret[self.token_profile[collateral]["symbol"]] = {
-        'amount': amount,
-        'value_usd': amount * collateral_usd[index]
-      }
-
-    return ret
-
   def deposit_erc20_collateral(self, sub_account_id: int, token_address: str, amount: float):
     '''
     Deposit ERC20 token as collateral.
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
@@ -113,15 +78,15 @@
     :type token_address: str in list COLLATERALS
 
     :param amount: required
     :type amount: float
     '''
     if token_address not in self.collateral_address_list:
       raise Exception("Invalid collateral address")
-    self.__check_sub_account_id_param(sub_account_id)
+    check_sub_account_id_param(sub_account_id)
 
     amount_wei = int(
       amount * 10 ** self.token_profile[token_address]["decimals"])
     token_instance = load_contract(
       self.eth_provider, token_address, ERC20_ABI_PATH)
 
     CROSS_MARGIN_HANDLER_ADDRESS = self.contract_address["CROSS_MARGIN_HANDLER_ADDRESS"]
@@ -150,15 +115,15 @@
     :type token_address: str in list COLLATERALS
 
     :param amount: required
     :type amount: float
     '''
     if token_address not in self.collateral_address_list:
       raise Exception("Invalid collateral address")
-    self.__check_sub_account_id_param(sub_account_id)
+    check_sub_account_id_param(sub_account_id)
     wrap = wrap if self.token_profile[token_address]['symbol'] == "WETH" else False
 
     amount_wei = int(
       amount * 10 ** self.token_profile[token_address]["decimals"])
 
     transact_param = {"value": EXECUTION_FEE, "from": self.eth_signer.address,
                       "gas": 10000000} if self.chain_id == 421614 else {"value": EXECUTION_FEE, "from": self.eth_signer.address}
@@ -177,15 +142,15 @@
 
     :param sub_account_id: required
     :type sub_account_id: int between 0 and 255
 
     :param amount: required
     :type amount: float
     '''
-    self.__check_sub_account_id_param(sub_account_id)
+    check_sub_account_id_param(sub_account_id)
 
     amount_wei = int(amount * 10 ** 18)
 
     return self.cross_margin_handler_instance.functions.depositCollateral(
       sub_account_id,
       self.token_profile['WETH']['address'],
       amount_wei,
@@ -210,15 +175,15 @@
 
     :param reduce_only: required
     :type reduce_only: bool
 
     :param tp_token
     :type tp_token: str in list COLLATERALS address
     '''
-    self.__check_sub_account_id_param(sub_account_id)
+    check_sub_account_id_param(sub_account_id)
 
     order = {
       "cmd": Cmd.CREATE,
       "market_index": market_index,
       "size_delta": Web3.to_wei(size, "tether") if buy else -Web3.to_wei(size, "tether"),
       "trigger_price": 0,
       "acceptable_price": MAX_UINT if buy else 0,
@@ -439,15 +404,17 @@
 
   def __prepare_cancel_order_call_data(self, order_index: int):
     return encode(
       ["uint256"],
       [order_index]
     )
 
-  def __check_sub_account_id_param(self, sub_account_id):
-    if sub_account_id not in range(0, 256):
-      raise Exception("Invalid sub account id")
-
   def __parse_log(self, tx, topic):
     receipt = self.eth_provider.eth.get_transaction_receipt(tx)
     return self.limit_trade_handler_instance.events[topic](
       ).process_receipt(receipt, DISCARD)
+
+  def get_public_address(self):
+    '''
+    Get the public address of the signer.
+    '''
+    return self.eth_signer.address
```

### Comparing `hmx-v2-python-1.0.1/hmx2/modules/public.py` & `hmx-v2-python-1.0.2/hmx2/modules/public.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,30 @@
   BYTE_ZERO,
   HOURS,
   DAYS,
   YEARS
 )
 from hmx2.helpers.contract_loader import load_contract
 from hmx2.helpers.mapper import (
+  get_collateral_address_asset_map,
+  get_collateral_address_list,
   get_contract_address,
+  get_token_profile,
 )
 from hmx2.helpers.util import get_sub_account
 from hmx2.modules.oracle.oracle_middleware import OracleMiddleware
 from hmx2.modules.calculator.calculator import Calculator
 from simple_multicall_v6 import Multicall
 from eth_abi.abi import decode
 from typing import List
 
 
 class Public(object):
   def __init__(self, chain_id: int, eth_provider: Web3, oracle_middleware: OracleMiddleware):
+    self.chain_id = chain_id
     self.eth_provider = eth_provider
     self.oracle_middleware = oracle_middleware
     self.contract_address = get_contract_address(chain_id)
     self.perp_storage_instance = load_contract(
       self.eth_provider, self.contract_address["PERP_STORAGE_ADDRESS"], PERP_STORAGE_ABI_PATH)
     self.config_storage_instance = load_contract(
       self.eth_provider, self.contract_address["CONFIG_STORAGE_ADDRESS"], CONFIG_STORAGE_ABI_PATH)
@@ -113,36 +117,53 @@
     position_result = self.multicall_instance.call(position_calls)
     data = position_result[1]
 
     position_data = {}
 
     for sub_account_id in sub_account_list:
       data_pop = data.pop(0)
-      (
-          raw_sub_account_position
-        ) = decode(
-            ['(address,uint256,uint256,uint256,uint256,uint256,int256,int256,int256,uint8)[]'],
-            data_pop
-        )
+      # backward compatibility on `getPositionBySubAccount`
+      raw_sub_account_position = {}
+      try:
+        (
+            raw_sub_account_position
+          ) = decode(
+              ['(address,uint256,uint256,uint256,uint256,uint256,int256,int256,int256,uint8)[]'],
+              data_pop
+          )
+      except:
+        (
+            raw_sub_account_position
+          ) = decode(
+              ['(address,uint256,uint256,uint256,uint256,uint256,int256,int256,int256,uint8,uint256)[]'],
+              data_pop
+          )
+
       raw_sub_account_position = [
         x for y in raw_sub_account_position for x in y]
 
       sub_account_position = []
-      for positon in raw_sub_account_position:
+      for position in raw_sub_account_position:
+        last_increase_size = None
+        try:
+          last_increase_size = position[10]
+        except:
+          pass
         _position = {
-          "primary_account": positon[0],
-          "market_index": positon[1],
-          "avg_entry_price_e30": positon[2],
-          "entry_borrowing_rate": positon[3],
-          "reserve_value_e30": positon[4],
-          "last_increase_timestamp": positon[5],
-          "position_size_e30": positon[6],
-          "realized_pnl": positon[7],
-          "last_funding_accrued": positon[8],
-          "sub_account_id": positon[9],
+          "primary_account": position[0],
+          "market_index": position[1],
+          "avg_entry_price_e30": position[2],
+          "entry_borrowing_rate": position[3],
+          "reserve_value_e30": position[4],
+          "last_increase_timestamp": position[5],
+          "position_size_e30": position[6],
+          "realized_pnl": position[7],
+          "last_funding_accrued": position[8],
+          "sub_account_id": position[9],
+          "last_increase_size": last_increase_size,
         }
         sub_account_position.append(_position)
 
       position_data[sub_account_id] = sub_account_position
 
     return position_data
 
@@ -755,7 +776,44 @@
       return 0
 
     positions = self.get_all_position_info(account, [sub_account_id])
 
     sizes = sum(map(lambda position: abs(position["position_size"]), positions))
 
     return sizes / equity
+
+  def get_collaterals(self, account: str, sub_account_id: int):
+
+    sub_account_address = get_sub_account(account, sub_account_id)
+    collateral_address_list = get_collateral_address_list(self.chain_id)
+    collateral_address_asset_map = get_collateral_address_asset_map(
+      self.chain_id)
+    token_profile = get_token_profile(self.chain_id)
+
+    calls = [
+      self.multicall_instance.create_call(
+        self.vault_storage_instance,
+          "traderBalances",
+          [sub_account_address, collateral],
+      )
+      for collateral in collateral_address_list
+    ]
+
+    collateral_asset_ids_list = list(map(
+      lambda collateral: collateral_address_asset_map[collateral], collateral_address_list))
+
+    collateral_price_dict = self.oracle_middleware.get_multiple_price(
+        collateral_asset_ids_list
+      )
+
+    results = self.multicall_instance.call(calls)
+
+    ret = {}
+    for index, collateral in enumerate(collateral_address_list):
+      amount = int(
+          results[1][index].hex(), 16) / 10 ** token_profile[collateral]["decimals"]
+      ret[token_profile[collateral]["symbol"]] = {
+        'amount': amount,
+        'value_usd': amount * collateral_price_dict[token_profile[collateral]["asset"]]
+      }
+
+    return ret
```

### Comparing `hmx-v2-python-1.0.1/hmx_v2_python.egg-info/PKG-INFO` & `hmx-v2-python-1.0.2/hmx_v2_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmx-v2-python
-Version: 1.0.1
+Version: 1.0.2
 Summary: HMXv2 Python SDK
 Home-page: https://github.com/HMXOrg/v2-sdk-python
 Author: HMXOrg
 Author-email: contact@hmx.org
 License: MIT
 Keywords: hmx exchange perp dex defi ethereum eth arbitrum
 Platform: UNKNOWN
@@ -50,23 +50,23 @@
 #
 # Using publicly access functions
 #
 hmx_client = Client(
     rpc_url=RPC_URL
 )
 # Get oracle price, adaptive price, and price impact of a new position
-client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
+hmx_client.public.get_price(MARKET_ETH_USD, Action.SELL, 1000)
 # Get market information
-client.public.get_market_info(MARKET_ETH_USD)
+hmx_client.public.get_market_info(MARKET_ETH_USD)
 # Get sub account in address format
-client.public.get_sub_account(1)
+hmx_client.public.get_sub_account(1)
 # Get position ID
-client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_id(some_account, some_sub_account_id, MARKET_ETH_USD)
 # Get position info
-client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
+hmx_client.public.get_position_info(some_account, some_sub_account_id, MARKET_ETH_USD)
 ```
 
 ### Private function
 
 ```python
 from hmx2.hmx_client import Client
 from hmx2.constants.markets import MARKET_ETH_USD
@@ -77,43 +77,43 @@
 # Initailized client with private key
 #
 hmx_client = Client(
     eth_private_key=PRIVATE_KEY,
     rpc_url=RPC_URL
 )
 # Get public address of the ethereum key
-client.private.get_public_address()
+hmx_client.private.get_public_address()
 # Deposit ETH as collateral
-client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
+hmx_client.private.deposit_eth_collateral(sub_account_id=0, amount=10.123)
 # Deposit ERC20 as collateral. This function will automatically
 # approve CrossMarginHandler if needed.
-client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
+hmx_client.private.deposit_erc20_collateral(sub_account_id=0, token_address=COLLATERAL_USDCe, amount=100.10)
 # Create a market order
-create_market_order = client.private.create_market_order(
+create_market_order = hmx_client.private.create_market_order(
   sub_account_id=0, market_index=MARKET_ETH_USD, buy=Action.BUY, size=100, reduce_only=False
 )
 print(create_market_order)
 # Create a trigger order
 # trigger_above_threshold = The current price must go above (if True) or below (if False)
 # the trigger price in order for the order to be executed
-create_order = client.private.create_trigger_order(
+create_order = hmx_client.private.create_trigger_order(
   sub_account_id=0,
   market_index=MARKET_ETH_USD,
   buy=Action.BUY,
   size=100,
   trigger_price=1800,
   trigger_above_threshold=True,
   reduce_only=False)
 print(create_order)
 # Update the order
-update_order = client.private.update_trigger_order(
+update_order = hmx_client.private.update_trigger_order(
   0, create_order["order"]["orderIndex"], Action.SELL, 50, 1700, True, False)
 print(update_order)
 # Cancel the order
-cancel_order = client.private.cancel_trigger_order(
+cancel_order = hmx_client.private.cancel_trigger_order(
   0, update_order["order"]["orderIndex"])
 ```
 
 ## Running Tests
 
 To run tests, you will need have to clone the repo, update .env, and run:
```

### Comparing `hmx-v2-python-1.0.1/hmx_v2_python.egg-info/SOURCES.txt` & `hmx-v2-python-1.0.2/hmx_v2_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/setup.py` & `hmx-v2-python-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'simple-multicall-v6',
     'responses',
     'python-dotenv>=1.0.0'
 ]
 
 setup(
     name='hmx-v2-python',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     package_data={
       'hmx2': ['abis/*.json'],
     },
     description='HMXv2 Python SDK',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
```

### Comparing `hmx-v2-python-1.0.1/tests/constants.py` & `hmx-v2-python-1.0.2/tests/constants.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/tests/test_create_market_order.py` & `hmx-v2-python-1.0.2/tests/test_create_market_order.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/tests/test_deposit_collateral.py` & `hmx-v2-python-1.0.2/tests/test_deposit_collateral.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     responses.add_passthru(setup_tenderly_helper.rpc_url)
 
     client = Client(
       eth_private_key=DEFAULT_KEY,
       rpc_url=setup_tenderly_helper.rpc_url
     )
     client.private.deposit_eth_collateral(0, 10)
-    my_collaterals = client.private.get_collaterals(0)
+    my_collaterals = client.public.get_collaterals(
+      client.private.get_public_address(), 0)
     assert my_collaterals["WETH"]["amount"] == 10
     assert my_collaterals["WETH"]["value_usd"] == 18500
 
   @responses.activate
   def test_correctness_when_deposit_weth_collateral_without_allowance(self, setup_tenderly_helper: TenderlyHelper):
     # mock pyth prices
     mock_pyth_price(DEFAULT_CHAIN_ID, ASSET_USDC, 1)
@@ -92,15 +93,16 @@
     action_helper = ActionHelper(
       rpc_url=setup_tenderly_helper.rpc_url,
       eth_private_key=DEFAULT_KEY
     )
     asset_map = get_token_profile(DEFAULT_CHAIN_ID)
     action_helper.wrap_eth(10)
     client.private.deposit_erc20_collateral(0, asset_map['WETH']['address'], 10)
-    my_collaterals = client.private.get_collaterals(0)
+    my_collaterals = client.public.get_collaterals(
+      client.private.get_public_address(), 0)
     assert my_collaterals["WETH"]["amount"] == 10
     assert my_collaterals["WETH"]["value_usd"] == 18500
 
   @responses.activate
   def test_correctness_when_deposit_erc20_collateral_without_allowance(self, setup_tenderly_helper: TenderlyHelper):
     # mock pyth prices
     mock_pyth_price(DEFAULT_CHAIN_ID, ASSET_USDC, 1)
@@ -126,10 +128,11 @@
     action_helper.approve(
       asset_map['WETH']['address'], UNISWAP_SWAP_ROUTER_02_ADDRESS, 10)
     action_helper.swapExactTokensForTokens(
       asset_map['WETH']['address'], asset_map['USDC.e']['address'], 500, 10)
     # deposit USDC.e as collateral
     client.private.deposit_erc20_collateral(
       0, asset_map['USDC.e']['address'], 1000)
-    my_collaterals = client.private.get_collaterals(0)
+    my_collaterals = client.public.get_collaterals(
+      client.private.get_public_address(), 0)
     assert my_collaterals["USDC.e"]["amount"] == 1000
     assert my_collaterals["USDC.e"]["value_usd"] == 1000
```

### Comparing `hmx-v2-python-1.0.1/tests/test_get_adaptive_fee.py` & `hmx-v2-python-1.0.2/tests/test_get_adaptive_fee.py`

 * *Files identical despite different names*

### Comparing `hmx-v2-python-1.0.1/tests/test_init.py` & `hmx-v2-python-1.0.2/tests/test_init.py`

 * *Files identical despite different names*

