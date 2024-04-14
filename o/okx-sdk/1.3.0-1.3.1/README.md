# Comparing `tmp/okx-sdk-1.3.0.tar.gz` & `tmp/okx-sdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okx-sdk-1.3.0.tar", last modified: Wed Apr 10 16:09:56 2024, max compression
+gzip compressed data, was "okx-sdk-1.3.1.tar", last modified: Sun Apr 14 07:05:07 2024, max compression
```

## Comparing `okx-sdk-1.3.0.tar` & `okx-sdk-1.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/
--rw-rw-rw-   0        0        0    11357 2024-03-08 14:17:03.000000 okx-sdk-1.3.0/LICENSE
--rw-rw-rw-   0        0        0    33352 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    31907 2024-04-10 16:08:46.000000 okx-sdk-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.321192 okx-sdk-1.3.0/okx/
--rw-rw-rw-   0        0        0      554 2024-03-08 16:50:40.000000 okx-sdk-1.3.0/okx/__init__.py
--rw-rw-rw-   0        0        0     2859 2024-03-10 12:31:52.000000 okx-sdk-1.3.0/okx/clients.py
--rw-rw-rw-   0        0        0    22003 2024-04-10 16:05:30.000000 okx-sdk-1.3.0/okx/constants.py
--rw-rw-rw-   0        0        0     1181 2024-03-07 13:22:01.000000 okx-sdk-1.3.0/okx/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.461369 okx-sdk-1.3.0/okx/restapi/
--rw-rw-rw-   0        0        0    11724 2024-03-08 19:20:28.000000 okx-sdk-1.3.0/okx/restapi/Account.py
--rw-rw-rw-   0        0        0     4043 2024-03-08 19:00:13.000000 okx-sdk-1.3.0/okx/restapi/AlgoTrading.py
--rw-rw-rw-   0        0        0     2202 2024-03-08 16:34:29.000000 okx-sdk-1.3.0/okx/restapi/BaseClient.py
--rw-rw-rw-   0        0        0     5320 2024-03-08 21:25:57.000000 okx-sdk-1.3.0/okx/restapi/BlockTrading.py
--rw-rw-rw-   0        0        0     6562 2024-03-09 15:24:05.000000 okx-sdk-1.3.0/okx/restapi/Broker.py
--rw-rw-rw-   0        0        0     2832 2024-03-08 16:37:22.000000 okx-sdk-1.3.0/okx/restapi/CopyTrading.py
--rw-rw-rw-   0        0        0     4638 2024-03-08 21:59:21.000000 okx-sdk-1.3.0/okx/restapi/Finance.py
--rw-rw-rw-   0        0        0     5997 2024-03-08 21:47:56.000000 okx-sdk-1.3.0/okx/restapi/Funding.py
--rw-rw-rw-   0        0        0     5473 2024-03-08 21:13:31.000000 okx-sdk-1.3.0/okx/restapi/GridTrading.py
--rw-rw-rw-   0        0        0    10266 2024-03-08 21:22:57.000000 okx-sdk-1.3.0/okx/restapi/PublicData.py
--rw-rw-rw-   0        0        0     2700 2024-03-08 16:37:22.000000 okx-sdk-1.3.0/okx/restapi/RecurringBuy.py
--rw-rw-rw-   0        0        0     2391 2024-03-08 16:37:22.000000 okx-sdk-1.3.0/okx/restapi/Rubik.py
--rw-rw-rw-   0        0        0     5099 2024-04-10 16:05:04.000000 okx-sdk-1.3.0/okx/restapi/SignalTrading.py
--rw-rw-rw-   0        0        0     3875 2024-03-08 21:30:58.000000 okx-sdk-1.3.0/okx/restapi/SpreadTrading.py
--rw-rw-rw-   0        0        0     4087 2024-03-08 21:51:13.000000 okx-sdk-1.3.0/okx/restapi/SubAccount.py
--rw-rw-rw-   0        0        0     7783 2024-03-08 20:50:29.000000 okx-sdk-1.3.0/okx/restapi/Trading.py
--rw-rw-rw-   0        0        0     1071 2024-03-08 18:52:41.000000 okx-sdk-1.3.0/okx/restapi/__init__.py
--rw-rw-rw-   0        0        0     1696 2024-03-07 20:33:42.000000 okx-sdk-1.3.0/okx/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.502867 okx-sdk-1.3.0/okx/wsapi/
--rw-rw-rw-   0        0        0      894 2024-03-09 21:23:09.000000 okx-sdk-1.3.0/okx/wsapi/Factory.py
--rw-rw-rw-   0        0        0     2283 2024-03-09 21:26:00.000000 okx-sdk-1.3.0/okx/wsapi/PrivateAsync.py
--rw-rw-rw-   0        0        0     1554 2024-03-10 12:31:54.000000 okx-sdk-1.3.0/okx/wsapi/PublicAsync.py
--rw-rw-rw-   0        0        0      161 2024-03-09 21:26:12.000000 okx-sdk-1.3.0/okx/wsapi/__init__.py
--rw-rw-rw-   0        0        0     2207 2024-03-09 21:17:53.000000 okx-sdk-1.3.0/okx/wsapi/wsutils.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/okx_sdk.egg-info/
--rw-rw-rw-   0        0        0    33352 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-10 16:09:56.000000 okx-sdk-1.3.0/okx_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1198 2024-04-10 16:09:12.000000 okx-sdk-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:09:56.536408 okx-sdk-1.3.0/tests/
--rw-rw-rw-   0        0        0        0 2024-03-07 08:28:13.000000 okx-sdk-1.3.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.753131 okx-sdk-1.3.1/
+-rw-rw-rw-   0        0        0    11357 2024-03-08 14:17:03.000000 okx-sdk-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0    33887 2024-04-14 07:05:07.752132 okx-sdk-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    32434 2024-04-14 07:04:21.000000 okx-sdk-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.529128 okx-sdk-1.3.1/okx/
+-rw-rw-rw-   0        0        0      554 2024-03-08 16:50:40.000000 okx-sdk-1.3.1/okx/__init__.py
+-rw-rw-rw-   0        0        0     2859 2024-03-10 12:31:52.000000 okx-sdk-1.3.1/okx/clients.py
+-rw-rw-rw-   0        0        0    21787 2024-04-14 07:02:59.000000 okx-sdk-1.3.1/okx/constants.py
+-rw-rw-rw-   0        0        0     1181 2024-03-07 13:22:01.000000 okx-sdk-1.3.1/okx/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.680131 okx-sdk-1.3.1/okx/restapi/
+-rw-rw-rw-   0        0        0    11724 2024-03-08 19:20:28.000000 okx-sdk-1.3.1/okx/restapi/Account.py
+-rw-rw-rw-   0        0        0     4043 2024-03-08 19:00:13.000000 okx-sdk-1.3.1/okx/restapi/AlgoTrading.py
+-rw-rw-rw-   0        0        0     2202 2024-03-08 16:34:29.000000 okx-sdk-1.3.1/okx/restapi/BaseClient.py
+-rw-rw-rw-   0        0        0     5320 2024-03-08 21:25:57.000000 okx-sdk-1.3.1/okx/restapi/BlockTrading.py
+-rw-rw-rw-   0        0        0     8252 2024-04-14 07:02:40.000000 okx-sdk-1.3.1/okx/restapi/Broker.py
+-rw-rw-rw-   0        0        0     2832 2024-03-08 16:37:22.000000 okx-sdk-1.3.1/okx/restapi/CopyTrading.py
+-rw-rw-rw-   0        0        0     4638 2024-03-08 21:59:21.000000 okx-sdk-1.3.1/okx/restapi/Finance.py
+-rw-rw-rw-   0        0        0     5997 2024-03-08 21:47:56.000000 okx-sdk-1.3.1/okx/restapi/Funding.py
+-rw-rw-rw-   0        0        0     5473 2024-03-08 21:13:31.000000 okx-sdk-1.3.1/okx/restapi/GridTrading.py
+-rw-rw-rw-   0        0        0    10266 2024-03-08 21:22:57.000000 okx-sdk-1.3.1/okx/restapi/PublicData.py
+-rw-rw-rw-   0        0        0     2700 2024-03-08 16:37:22.000000 okx-sdk-1.3.1/okx/restapi/RecurringBuy.py
+-rw-rw-rw-   0        0        0     2391 2024-03-08 16:37:22.000000 okx-sdk-1.3.1/okx/restapi/Rubik.py
+-rw-rw-rw-   0        0        0     5099 2024-04-10 16:05:04.000000 okx-sdk-1.3.1/okx/restapi/SignalTrading.py
+-rw-rw-rw-   0        0        0     3875 2024-03-08 21:30:58.000000 okx-sdk-1.3.1/okx/restapi/SpreadTrading.py
+-rw-rw-rw-   0        0        0     4087 2024-03-08 21:51:13.000000 okx-sdk-1.3.1/okx/restapi/SubAccount.py
+-rw-rw-rw-   0        0        0     7783 2024-03-08 20:50:29.000000 okx-sdk-1.3.1/okx/restapi/Trading.py
+-rw-rw-rw-   0        0        0     1071 2024-03-08 18:52:41.000000 okx-sdk-1.3.1/okx/restapi/__init__.py
+-rw-rw-rw-   0        0        0     1696 2024-03-07 20:33:42.000000 okx-sdk-1.3.1/okx/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.722132 okx-sdk-1.3.1/okx/wsapi/
+-rw-rw-rw-   0        0        0      894 2024-03-09 21:23:09.000000 okx-sdk-1.3.1/okx/wsapi/Factory.py
+-rw-rw-rw-   0        0        0     2283 2024-03-09 21:26:00.000000 okx-sdk-1.3.1/okx/wsapi/PrivateAsync.py
+-rw-rw-rw-   0        0        0     1554 2024-03-10 12:31:54.000000 okx-sdk-1.3.1/okx/wsapi/PublicAsync.py
+-rw-rw-rw-   0        0        0      161 2024-03-09 21:26:12.000000 okx-sdk-1.3.1/okx/wsapi/__init__.py
+-rw-rw-rw-   0        0        0     2207 2024-03-09 21:17:53.000000 okx-sdk-1.3.1/okx/wsapi/wsutils.py
+drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.751131 okx-sdk-1.3.1/okx_sdk.egg-info/
+-rw-rw-rw-   0        0        0    33887 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-14 07:05:07.000000 okx-sdk-1.3.1/okx_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 07:05:07.754131 okx-sdk-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2024-04-14 07:04:36.000000 okx-sdk-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 07:05:07.750137 okx-sdk-1.3.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:28:13.000000 okx-sdk-1.3.1/tests/__init__.py
```

### Comparing `okx-sdk-1.3.0/LICENSE` & `okx-sdk-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/PKG-INFO` & `okx-sdk-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python
 Home-page: https://github.com/burakoner/okx-sdk
 Author: Burak Öner
 Author-email: info@burakoner.com
 Keywords: okx,crypto,exchange,api,sdk,stream,websocket,ws,python,bitcoin,btc,spot,futures,trade
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -669,14 +669,22 @@
 api.ndbroker.reset_subaccount_deposit_address(subAcct='', ccy='', chain='', addr='', to='')
 api.ndbroker.get_subaccount_deposit_address(subAcct='', ccy='')
 api.ndbroker.get_subaccount_deposit_history(subAcct='', ccy='', txId='', state='', after='', before='', limit='')
 api.ndbroker.get_subaccount_withdrawal_history(subAcct='', ccy='', wdId='', clientId='', txId='', type='', state='', before='', limit='')
 api.ndbroker.get_rebate_daily(subAcct='', begin='', end='', page='', limit='')
 api.ndbroker.get_rebate_details_download_link(type='', begin='', end='')
 api.ndbroker.generate_rebate_details_download_link(begin='', end='')
+api.ndbroker.get_dcd_products(ccy, alternativeCcy, optType, tag)
+api.ndbroker.request_dcd_quote(notional, notionalCcy, productId, tag, markUp='', clReqId='')
+api.ndbroker.exec_dcd_order(quoteId, clReqId='')
+api.ndbroker.get_dcd_order(ordId='', clReqId='')
+api.ndbroker.get_dcd_orders(productId='', uly='', state='', beginId='', endId='', begin='', end='', limit='')
+api.ndbroker.set_subaccount_asset(subAcct, ccy)
+api.ndbroker.report_subaccount_ip(subAcct, clientIP)
+api.ndbroker.get_rebate_info(apiKey='', uid='', subAcct='')
 ```
 
 #### Fully-Disclosed Broker Client
 
 ```python
 from okx import OkxRestClient
```

### Comparing `okx-sdk-1.3.0/README.md` & `okx-sdk-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -649,14 +649,22 @@
 api.ndbroker.reset_subaccount_deposit_address(subAcct='', ccy='', chain='', addr='', to='')
 api.ndbroker.get_subaccount_deposit_address(subAcct='', ccy='')
 api.ndbroker.get_subaccount_deposit_history(subAcct='', ccy='', txId='', state='', after='', before='', limit='')
 api.ndbroker.get_subaccount_withdrawal_history(subAcct='', ccy='', wdId='', clientId='', txId='', type='', state='', before='', limit='')
 api.ndbroker.get_rebate_daily(subAcct='', begin='', end='', page='', limit='')
 api.ndbroker.get_rebate_details_download_link(type='', begin='', end='')
 api.ndbroker.generate_rebate_details_download_link(begin='', end='')
+api.ndbroker.get_dcd_products(ccy, alternativeCcy, optType, tag)
+api.ndbroker.request_dcd_quote(notional, notionalCcy, productId, tag, markUp='', clReqId='')
+api.ndbroker.exec_dcd_order(quoteId, clReqId='')
+api.ndbroker.get_dcd_order(ordId='', clReqId='')
+api.ndbroker.get_dcd_orders(productId='', uly='', state='', beginId='', endId='', begin='', end='', limit='')
+api.ndbroker.set_subaccount_asset(subAcct, ccy)
+api.ndbroker.report_subaccount_ip(subAcct, clientIP)
+api.ndbroker.get_rebate_info(apiKey='', uid='', subAcct='')
 ```
 
 #### Fully-Disclosed Broker Client
 
 ```python
 from okx import OkxRestClient
```

### Comparing `okx-sdk-1.3.0/okx/__init__.py` & `okx-sdk-1.3.1/okx/__init__.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/clients.py` & `okx-sdk-1.3.1/okx/clients.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/constants.py` & `okx-sdk-1.3.1/okx/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,21 +361,19 @@
 BROKER_ND_MODIFY_SUBACCOUNT_DEPOSIT_ADDRESS = '/api/v5/asset/broker/nd/modify-subaccount-deposit-address'
 BROKER_ND_SUBACCOUNT_DEPOSIT_ADDRESS = '/api/v5/asset/broker/nd/subaccount-deposit-address'
 BROKER_ND_SUBACCOUNT_DEPOSIT_HISTORY = '/api/v5/asset/broker/nd/subaccount-deposit-history'
 BROKER_ND_SUBACCOUNT_WITHDRAWAL_HISTORY = '/api/v5/asset/broker/nd/subaccount-withdrawal-history'
 BROKER_ND_REBATE_DAILY = '/api/v5/broker/nd/rebate-daily'
 BROKER_ND_GET_REBATE_PER_ORDERS = '/api/v5/broker/nd/rebate-per-orders'
 BROKER_ND_GEN_REBATE_PER_ORDERS = '/api/v5/broker/nd/rebate-per-orders'
-FINANCE_SFP_DCD_PRODUCTS = '/api/v5/finance/sfp/dcd/products'  # TODO
-FINANCE_SFP_DCD_QUOTE = '/api/v5/finance/sfp/dcd/quote'  # TODO
-FINANCE_SFP_DCD_ORDER_01 = '/api/v5/finance/sfp/dcd/order'  # TODO
-FINANCE_SFP_DCD_ORDER_02 = '/api/v5/finance/sfp/dcd/order'  # TODO
-FINANCE_SFP_DCD_ORDERS = '/api/v5/finance/sfp/dcd/orders'  # TODO
-BROKER_ND_SET_SUBACCOUNT_ASSETS_01 = '/api/v5/broker/nd/set-subaccount-assets'  # TODO
-BROKER_ND_SET_SUBACCOUNT_ASSETS_02 = '/api/v5/broker/nd/set-subaccount-assets'  # TODO
-BROKER_ND_REPORT_SUBACCOUNT_IP = '/api/v5/broker/nd/report-subaccount-ip'  # TODO
-BROKER_ND_IF_REBATE = '/api/v5/broker/nd/if-rebate'  # TODO
+FINANCE_SFP_DCD_PRODUCTS = '/api/v5/finance/sfp/dcd/products'
+FINANCE_SFP_DCD_QUOTE = '/api/v5/finance/sfp/dcd/quote'
+FINANCE_SFP_DCD_ORDER = '/api/v5/finance/sfp/dcd/order'
+FINANCE_SFP_DCD_ORDERS = '/api/v5/finance/sfp/dcd/orders'
+BROKER_ND_SET_SUBACCOUNT_ASSETS = '/api/v5/broker/nd/set-subaccount-assets'
+BROKER_ND_REPORT_SUBACCOUNT_IP = '/api/v5/broker/nd/report-subaccount-ip'
+BROKER_ND_IF_REBATE = '/api/v5/broker/nd/if-rebate'
 
 # Fully-Disclosed Broker Endpoints
 BROKER_FD_GET_REBATE_PER_ORDERS = '/api/v5/broker/fd/rebate-per-orders'
 BROKER_FD_GEN_REBATE_PER_ORDERS = '/api/v5/broker/fd/rebate-per-orders'
 BROKER_FD_IF_REBATE = '/api/v5/broker/fd/if-rebate'
```

### Comparing `okx-sdk-1.3.0/okx/exceptions.py` & `okx-sdk-1.3.1/okx/exceptions.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/Account.py` & `okx-sdk-1.3.1/okx/restapi/Account.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/AlgoTrading.py` & `okx-sdk-1.3.1/okx/restapi/AlgoTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/BaseClient.py` & `okx-sdk-1.3.1/okx/restapi/BaseClient.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/BlockTrading.py` & `okx-sdk-1.3.1/okx/restapi/BlockTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/Broker.py` & `okx-sdk-1.3.1/okx/restapi/Broker.py`

 * *Files 14% similar despite different names*

```diff
@@ -158,24 +158,45 @@
     def generate_rebate_details_download_link(self, begin='', end=''):
         params = {
             'begin': begin,
             'end': end
         }
         return self._request(POST, BROKER_ND_GEN_REBATE_PER_ORDERS, params)
 
-    # TODO
-    # TODO
-    # TODO
-    # TODO
-    # TODO
-    # TODO
-    # TODO
-    # TODO
-    # TODO
+    def get_dcd_products(self, ccy, alternativeCcy, optType, tag):
+        params = { 'ccy': ccy, 'alternativeCcy': alternativeCcy, 'optType': optType, 'tag': tag }
+        return self._request(GET, FINANCE_SFP_DCD_PRODUCTS, params)
 
+    def request_dcd_quote(self, notional, notionalCcy, productId, tag, markUp='', clReqId=''):
+        params = { 'notional': notional, 'notionalCcy': notionalCcy, 'productId': productId, 'tag': tag, 'markUp': markUp, 'clReqId': clReqId }
+        return self._request(POST, FINANCE_SFP_DCD_QUOTE, params)
+
+    def exec_dcd_order(self, quoteId, clReqId=''):
+        params = { 'quoteId': quoteId, 'clReqId': clReqId }
+        return self._request(GET, FINANCE_SFP_DCD_ORDER, params)
+
+    def get_dcd_order(self, ordId='', clReqId=''):
+        params = { 'ordId': ordId, 'clReqId': clReqId }
+        return self._request(GET, FINANCE_SFP_DCD_ORDER, params)
+
+    def get_dcd_orders(self, productId='', uly='', state='', beginId='', endId='', begin='', end='', limit=''):
+        params = { 'productId': productId, 'uly': uly, 'state': state, 'beginId': beginId, 'endId': endId, 'begin': begin, 'end': end, 'limit': limit }
+        return self._request(GET, FINANCE_SFP_DCD_ORDERS, params)
+
+    def set_subaccount_asset(self, subAcct, ccy):
+        params = { 'subAcct': subAcct, 'ccy': ccy}
+        return self._request(POST, BROKER_ND_SET_SUBACCOUNT_ASSETS, params)
+    
+    def report_subaccount_ip(self, subAcct, clientIP):
+        params = { 'subAcct': subAcct, 'clientIP': clientIP}
+        return self._request(POST, BROKER_ND_REPORT_SUBACCOUNT_IP, params)
+
+    def get_rebate_info(self, apiKey='', uid='', subAcct=''):
+        params = { 'apiKey': apiKey, 'uid': uid, 'subAcct': subAcct }
+        return self._request(GET, BROKER_ND_IF_REBATE, params)
 
 class FullyDisclosedBrokerClient(OkxBaseClient):
     def __init__(self, apikey='', apisecret='', passphrase='', use_server_time=False, simulation=False, domain=API_URL, debug=False, proxy=None):
         OkxBaseClient.__init__(self, apikey, apisecret, passphrase, use_server_time, simulation, domain, debug, proxy)
 
     def get_rebate_details_download_link(self, type='', begin='', end=''):
         params = {'type': type, 'begin': begin, 'end': end}
```

### Comparing `okx-sdk-1.3.0/okx/restapi/CopyTrading.py` & `okx-sdk-1.3.1/okx/restapi/CopyTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/Finance.py` & `okx-sdk-1.3.1/okx/restapi/Finance.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/Funding.py` & `okx-sdk-1.3.1/okx/restapi/Funding.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/GridTrading.py` & `okx-sdk-1.3.1/okx/restapi/GridTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/PublicData.py` & `okx-sdk-1.3.1/okx/restapi/PublicData.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/RecurringBuy.py` & `okx-sdk-1.3.1/okx/restapi/RecurringBuy.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/Rubik.py` & `okx-sdk-1.3.1/okx/restapi/Rubik.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/SignalTrading.py` & `okx-sdk-1.3.1/okx/restapi/SignalTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/SpreadTrading.py` & `okx-sdk-1.3.1/okx/restapi/SpreadTrading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/SubAccount.py` & `okx-sdk-1.3.1/okx/restapi/SubAccount.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/Trading.py` & `okx-sdk-1.3.1/okx/restapi/Trading.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/restapi/__init__.py` & `okx-sdk-1.3.1/okx/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/utils.py` & `okx-sdk-1.3.1/okx/utils.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/wsapi/Factory.py` & `okx-sdk-1.3.1/okx/wsapi/Factory.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/wsapi/PrivateAsync.py` & `okx-sdk-1.3.1/okx/wsapi/PrivateAsync.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/wsapi/PublicAsync.py` & `okx-sdk-1.3.1/okx/wsapi/PublicAsync.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx/wsapi/wsutils.py` & `okx-sdk-1.3.1/okx/wsapi/wsutils.py`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/okx_sdk.egg-info/PKG-INFO` & `okx-sdk-1.3.1/okx_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okx-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python
 Home-page: https://github.com/burakoner/okx-sdk
 Author: Burak Öner
 Author-email: info@burakoner.com
 Keywords: okx,crypto,exchange,api,sdk,stream,websocket,ws,python,bitcoin,btc,spot,futures,trade
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -669,14 +669,22 @@
 api.ndbroker.reset_subaccount_deposit_address(subAcct='', ccy='', chain='', addr='', to='')
 api.ndbroker.get_subaccount_deposit_address(subAcct='', ccy='')
 api.ndbroker.get_subaccount_deposit_history(subAcct='', ccy='', txId='', state='', after='', before='', limit='')
 api.ndbroker.get_subaccount_withdrawal_history(subAcct='', ccy='', wdId='', clientId='', txId='', type='', state='', before='', limit='')
 api.ndbroker.get_rebate_daily(subAcct='', begin='', end='', page='', limit='')
 api.ndbroker.get_rebate_details_download_link(type='', begin='', end='')
 api.ndbroker.generate_rebate_details_download_link(begin='', end='')
+api.ndbroker.get_dcd_products(ccy, alternativeCcy, optType, tag)
+api.ndbroker.request_dcd_quote(notional, notionalCcy, productId, tag, markUp='', clReqId='')
+api.ndbroker.exec_dcd_order(quoteId, clReqId='')
+api.ndbroker.get_dcd_order(ordId='', clReqId='')
+api.ndbroker.get_dcd_orders(productId='', uly='', state='', beginId='', endId='', begin='', end='', limit='')
+api.ndbroker.set_subaccount_asset(subAcct, ccy)
+api.ndbroker.report_subaccount_ip(subAcct, clientIP)
+api.ndbroker.get_rebate_info(apiKey='', uid='', subAcct='')
 ```
 
 #### Fully-Disclosed Broker Client
 
 ```python
 from okx import OkxRestClient
```

### Comparing `okx-sdk-1.3.0/okx_sdk.egg-info/SOURCES.txt` & `okx-sdk-1.3.1/okx_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `okx-sdk-1.3.0/setup.py` & `okx-sdk-1.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
     
-VERSION = '1.3.0'
+VERSION = '1.3.1'
 DESCRIPTION = 'Up-to-date, most-complete, well-organized, well-documented, easy-to-use OKX Exchange Rest and Websocket API SDK for Python'
 
 setuptools.setup(
     name="okx-sdk",
     version=VERSION,
     author="Burak Öner",
     author_email="info@burakoner.com",
```

