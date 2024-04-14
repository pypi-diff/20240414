# Comparing `tmp/martin_binance-3.0.3.tar.gz` & `tmp/martin_binance-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-3.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-3.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-3.0.3.tar` & `martin_binance-3.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1079 2024-04-08 19:04:25.470012 martin_binance-3.0.3/LICENSE
--rwxr-xr-x   0        0        0     3854 2024-04-08 19:04:25.470012 martin_binance-3.0.3/README.md
--rwxr-xr-x   0        0        0     2076 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/__init__.py
--rw-r--r--   0        0        0     5007 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2786 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    13214 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/exchange_simulator.py
--rwxr-xr-x   0        0        0     4381 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/backtest/optimizer.py
--rw-r--r--   0        0        0     4752 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/client.py
--rw-r--r--   0        0        0     6935 2024-04-08 19:04:25.502012 martin_binance-3.0.3/martin_binance/db_utils.py
--rwxr-xr-x   0        0        0   139916 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/executor.py
--rw-r--r--   0        0        0    15709 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/lib.py
--rw-r--r--   0        0        0     2253 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/params.py
--rw-r--r--   0        0        0      485 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    14650 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1269 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/service/relaunch.service
--rw-r--r--   0        0        0    82004 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/strategy_base.py
--rw-r--r--   0        0        0     7151 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/telegram_utils.py
--rw-r--r--   0        0        0     7181 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/cli_0_BTCUSDT.py
--rw-r--r--   0        0        0     7182 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/cli_1_BTCUSDT.py
--rw-r--r--   0        0        0     7187 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
--rwxr-xr-x   0        0        0     7176 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/cli_3_BTCUSDT.py
--rw-r--r--   0        0        0   237568 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/funds_rate.db
--rw-r--r--   0        0        0     1723 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/ms_cfg.toml
--rw-r--r--   0        0        0      639 2024-04-08 19:04:25.506012 martin_binance-3.0.3/martin_binance/templates/trial_params.json
--rw-r--r--   0        0        0     1424 2024-04-08 19:04:25.506012 martin_binance-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     5154 1970-01-01 00:00:00.000000 martin_binance-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-14 17:58:18.433261 martin_binance-3.0.4/LICENSE
+-rwxr-xr-x   0        0        0     3854 2024-04-14 17:58:18.433261 martin_binance-3.0.4/README.md
+-rwxr-xr-x   0        0        0     1890 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/__init__.py
+-rw-r--r--   0        0        0     5007 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2786 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    13214 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/exchange_simulator.py
+-rwxr-xr-x   0        0        0     4180 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/optimizer.py
+-rw-r--r--   0        0        0     4705 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/client.py
+-rw-r--r--   0        0        0     6935 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/db_utils.py
+-rwxr-xr-x   0        0        0   139916 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/executor.py
+-rw-r--r--   0        0        0    15709 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/lib.py
+-rw-r--r--   0        0        0     2253 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/params.py
+-rw-r--r--   0        0        0      485 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    14650 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1269 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/relaunch.service
+-rw-r--r--   0        0        0    82430 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/strategy_base.py
+-rw-r--r--   0        0        0     7151 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/telegram_utils.py
+-rw-r--r--   0        0        0     7217 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/templates/cli_0_BTCUSDT.py
+-rw-r--r--   0        0        0     7219 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/templates/cli_1_BTCUSDT.py
+-rw-r--r--   0        0        0     7223 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
+-rwxr-xr-x   0        0        0     7212 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/templates/cli_3_BTCUSDT.py
+-rw-r--r--   0        0        0   237568 2024-04-14 17:58:18.473260 martin_binance-3.0.4/martin_binance/templates/funds_rate.db
+-rw-r--r--   0        0        0     1723 2024-04-14 17:58:18.473260 martin_binance-3.0.4/martin_binance/templates/ms_cfg.toml
+-rw-r--r--   0        0        0      639 2024-04-14 17:58:18.473260 martin_binance-3.0.4/martin_binance/templates/trial_params.json
+-rw-r--r--   0        0        0     1424 2024-04-14 17:58:18.473260 martin_binance-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5154 1970-01-01 00:00:00.000000 martin_binance-3.0.4/PKG-INFO
```

### Comparing `martin_binance-3.0.3/LICENSE` & `martin_binance-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/README.md` & `martin_binance-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/__init__.py` & `martin_binance-3.0.4/martin_binance/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.3"
+__version__ = "3.0.4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 from exchanges_wrapper.definitions import Interval
@@ -25,18 +25,14 @@
 DB_FILE = Path(WORK_PATH, "funds_rate.db")
 LOG_PATH = Path(WORK_PATH, "log")
 LAST_STATE_PATH = Path(WORK_PATH, "last_state")
 BACKTEST_PATH = Path(WORK_PATH, "back_test")
 TRIAL_PARAMS = Path(WORK_PATH, "trial_params.json")
 EQUAL_STR = "================================================================"
 
-# TODO remove after update to 3.0.3
-if CONFIG_FILE.exists() and not TRIAL_PARAMS.exists():
-    copy(Path(Path(__file__).parent.absolute(), "templates/trial_params.json"), TRIAL_PARAMS)
-
 
 def init():
     if CONFIG_FILE.exists():
         print(f"Client config found at {CONFIG_FILE}")
     else:
         print("Can't find client config file! Creating it...")
         for path in [CONFIG_PATH, LOG_PATH, LAST_STATE_PATH]:
```

### Comparing `martin_binance-3.0.3/martin_binance/backtest/OoTSP.py` & `martin_binance-3.0.4/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/backtest/VCoSEL.py` & `martin_binance-3.0.4/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/backtest/exchange_simulator.py` & `martin_binance-3.0.4/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/backtest/optimizer.py` & `martin_binance-3.0.4/martin_binance/backtest/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Searches for optimal parameters for a strategy under given conditions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2024 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.3"
+__version__ = "3.0.4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 
 import asyncio
 import importlib.util as iu
 import logging.handlers
@@ -82,20 +82,14 @@
         logger.info(f"Previous best params: {_prm_best}")
         _study.enqueue_trial(_prm_best)
 
     _study.optimize(objective, n_trials=n_trials, gc_after_trial=True, show_progress_bar=show_progress_bar)
     return _study
 
 
-async def run_optimize(*args):
-    process = await asyncio.create_subprocess_exec(*args, stdout=asyncio.subprocess.PIPE)
-    stdout, _ = await process.communicate()
-    return stdout.splitlines()[0]
-
-
 if __name__ == "__main__":
     logger = logging.getLogger('logger_S')
     logger.level = logging.INFO
     formatter = logging.Formatter(fmt="[%(asctime)s: %(levelname)s] %(message)s")
     #
     fh = logging.handlers.RotatingFileHandler(Path(LOG_PATH, sys.argv[6]), maxBytes=500000, backupCount=5)
     fh.setFormatter(formatter)
```

### Comparing `martin_binance-3.0.3/martin_binance/client.py` & `martin_binance-3.0.4/martin_binance/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 gRPC async client for exchanges-wrapper
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1"
+__version__ = "3.0.4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import asyncio
 import random
 import logging
 
@@ -67,29 +67,29 @@
             )
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error.
         except ConnectionRefusedError as ex:
             raise UserWarning(f"{ex}, reconnect...") from None
         except GRPCError as ex:
             status_code = ex.status
+            logger.warning(f"Exception on register client: {status_code.name}, {ex.message}")
             if status_code == Status.FAILED_PRECONDITION:
                 raise SystemExit(1) from ex
-            raise UserWarning(f"Exception on register client: {status_code.name}, {ex.message}") from None
+            raise UserWarning
         else:
-            logger.info(f"gRPC session started for client_id: {_client.client_id}\n"
-                        f"trade_id: {self.trade_id}")
+            logger.info(f"gRPC session started for client_id: {_client.client_id}, trade_id: {self.trade_id}")
             return _client
 
     async def send_request(self, _request, _request_type, **kwargs):
         if not self.client:
             raise UserWarning("Send gRPC request failed, not active client session")
         kwargs['client_id'] = self.client.client_id
         kwargs['trade_id'] = self.trade_id
         try:
-            res = await _request(_request_type(**kwargs))
+            return await _request(_request_type(**kwargs))
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except grpclib.exceptions.StreamTerminatedError:
             raise UserWarning("Have not connection to gRPC server")
         except ConnectionRefusedError:
             raise UserWarning("Connection to gRPC server broken")
         except GRPCError as ex:
@@ -97,16 +97,14 @@
             logger.debug(f"Send request {_request}: {status_code.name}, {ex.message}")
             if status_code == Status.UNAVAILABLE:
                 self.client = None
                 raise UserWarning("Wait connection to gRPC server") from None
             raise
         except Exception as ex:
             logger.error(f"Exception on send request {ex}")
-        else:
-            return res
 
     async def for_request(self, _request, _request_type, **kwargs):
         if not self.client:
             raise UserWarning("Start gRPC request loop failed, not active client session")
         kwargs['client_id'] = self.client.client_id
         kwargs['trade_id'] = self.trade_id
         try:
```

### Comparing `martin_binance-3.0.3/martin_binance/db_utils.py` & `martin_binance-3.0.4/martin_binance/db_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/executor.py` & `martin_binance-3.0.4/martin_binance/executor.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/lib.py` & `martin_binance-3.0.4/martin_binance/lib.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/params.py` & `martin_binance-3.0.4/martin_binance/params.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/service/funds_rate_exporter.py` & `martin_binance-3.0.4/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/service/grafana.json` & `martin_binance-3.0.4/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/service/relaunch.py` & `martin_binance-3.0.4/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/strategy_base.py` & `martin_binance-3.0.4/martin_binance/strategy_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 martin-binance base class and methods definitions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.2"
+__version__ = "3.0.4"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import csv
 import logging
@@ -35,24 +35,24 @@
 from tqdm import tqdm
 
 from exchanges_wrapper import martin as mr, Status, GRPCError
 
 import martin_binance.params as prm
 from martin_binance import LAST_STATE_PATH, BACKTEST_PATH, HEARTBEAT, KLINES_INIT, EQUAL_STR, ORDER_TIMEOUT
 from martin_binance.backtest.exchange_simulator import Account as backTestAccount
-from martin_binance.backtest.optimizer import run_optimize, OPTIMIZER, PARAMS_FLOAT
+from martin_binance.backtest.optimizer import OPTIMIZER, PARAMS_FLOAT
 from martin_binance.client import Trade
 from martin_binance.lib import Candle, TradingCapabilityManager, Ticker, FundsEntry, OrderBook, Style, \
     any2str, PrivateTrade, Order, convert_from_minute, OrderUpdate, load_file, load_last_state, Klines
 
 if prm.MODE == 'S':
     logger = logging.getLogger('logger_S')
 else:
     logger = logging.getLogger('logger')
-loop = asyncio.get_event_loop()
+
 color_init()
 
 RATE_LIMITER = HEARTBEAT * 5
 KLINES_LIM = 50  # Number of candles must be <= 1000
 CANCEL_ALL_ORDERS = True  # Ask about cancel all active orders before start strategy and par.LOAD_LAST_STATE = 0
 TRADES_LIST_LIMIT = 50
 TRY_LIMIT = 30
@@ -108,24 +108,25 @@
         self.wss_fire_up = False
         self.backtest = {}
         self.delay_ordering_s = 0.5
         self.bulk_orders_cancel = {}
         self.session_root = None
         self.state_file = None
         self.operational_status = None
-        self.tasks_list = []
+        self.tasks = set()
         #
         self.time_operational = {'ts': 0.0, 'diff': 0.0, 'new': 0.0}  # - See get_time()
         self.account = None
         self.get_buffered_funds_last_time = self.get_time()
         self.queue_to_tlg = queue.Queue() if prm.TOKEN and prm.MODE != 'S' else None
         self.status_time = None  # + Last time sending status message
         self.tlg_header = ''  # - Header for Telegram message
         self.start_collect = None
         self.s_mode_break = None
+        self.backtest_process = None
         # Init in reset_backtest_vars()
         self.s_ticker = None
         self.s_order_book = None
         self.klines = None
         self.candles = None
         self.grid_buy = None
         self.grid_sell = None
@@ -193,15 +194,15 @@
         return self.info_symbol.get('quoteAsset')
 
     def get_buffered_ticker(self) -> Ticker:
         return Ticker(self.ticker)
 
     def get_buffered_funds(self) -> Dict[str, FundsEntry]:
         if self.get_time() - self.get_buffered_funds_last_time > self.rate_limiter:
-            loop.create_task(self.buffered_funds(print_info=False))
+            self.tasks_manage(self.buffered_funds(print_info=False))
             self.get_buffered_funds_last_time = self.get_time()
         return {self.base_asset: FundsEntry(self.funds[self.base_asset]),
                 self.quote_asset: FundsEntry(self.funds[self.quote_asset])}
 
     def get_buffered_order_book(self) -> OrderBook:
         return OrderBook(self.order_book, _tcm=self.tcm)
 
@@ -236,30 +237,30 @@
             self.time_operational['ts'] = last
         else:
             last = current_time
         return last
 
     def transfer_to_master(self, symbol: str, amount: str):
         if prm.MODE in ('T', 'TC'):
-            loop.create_task(self.transfer2master(symbol, amount))
+            self.tasks_manage(self.transfer2master(symbol, amount))
 
     def place_limit_order(self, buy: bool, amount: Decimal, price: Decimal) -> int:
         self.order_id += 1
         self.message_log(f"Send order id:{self.order_id} for {'BUY' if buy else 'SELL'}"
                          f" {any2str(amount)} by {any2str(price)} = {any2str(amount * price)}",
                          color=Style.B_YELLOW)
-        loop.create_task(self.place_limit_order_timeout(self.order_id))
-        loop.create_task(self.create_limit_order(self.order_id, buy, any2str(amount), any2str(price)))
+        self.tasks_manage(self.place_limit_order_timeout(self.order_id))
+        self.tasks_manage(self.create_limit_order(self.order_id, buy, any2str(amount), any2str(price)))
         if self.exchange == 'huobi':
             time.sleep(0.02)
         return self.order_id
 
     def cancel_order(self, order_id: int, cancel_all=False) -> None:
-        loop.create_task(self.cancel_order_timeout(order_id))
-        loop.create_task(self.cancel_order_call(order_id, cancel_all))
+        self.tasks_manage(self.cancel_order_timeout(order_id))
+        self.tasks_manage(self.cancel_order_call(order_id, cancel_all))
 
     def message_log(self, msg: str, log_level=logging.INFO, tlg=False, color=Style.WHITE) -> None:
         if prm.LOGGING:
             if tlg and color == Style.WHITE:
                 color = Style.B_WHITE
             if log_level >= logging.ERROR:
                 tlg = True
@@ -318,31 +319,40 @@
                 self.start_collect = False
                 self.session_data_handler()
                 self.reset_backtest_vars()
                 if prm.SELF_OPTIMIZATION and self.command != 'stopped':
                     _ts = datetime.now(timezone.utc).replace(tzinfo=None)
                     storage_name = Path(self.session_root, "_study.db")
                     try:
-                        _res = await run_optimize(
+                        self.backtest_process = await asyncio.create_subprocess_exec(
                             OPTIMIZER,
                             f"{self.exchange}_{self.symbol}",
                             Path(self.session_root, Path(prm.PARAMS).name),
                             str(prm.N_TRIALS),
                             f"sqlite:///{storage_name}",
                             json.dumps(prm_best or _prm_best),
                             f"{prm.ID_EXCHANGE}_{prm.SYMBOL}_S.log",
+
+                            stdout=asyncio.subprocess.PIPE
                         )
-                        prm_best = orjson.loads(_res)
+                        stdout, _ = await self.backtest_process.communicate()
+                        _res = stdout.splitlines()
+                        if _res:
+                            prm_best = orjson.loads(_res[0])
+                        else:
+                            self.message_log("Backtest control: result is empty", log_level=logging.WARNING)
+                            break
                     except (asyncio.CancelledError, KeyboardInterrupt):
                         break
                     except Exception as err:
                         self.message_log(f"Backtest control: {err}", log_level=logging.ERROR)
                         self.message_log(f"Exception traceback: {traceback.format_exc()}", log_level=logging.DEBUG)
                         break
                     #
+                    self.backtest_process = None
                     storage_name.replace(storage_name.with_name('study.db'))
                     if prm_best:
                         _prm_best = dict(prm_best)
                         self.message_log(
                             f"Updating parameters from backtest,"
                             f" predicted value {prm_best.pop('_value')} -> {prm_best.pop('new_value')}",
                             color=Style.B_WHITE,
@@ -465,15 +475,15 @@
             print(f"Session profit: {s_profit}, free: {s_free}, total: {float(s_profit) + float(s_free)}")
             test_time = datetime.now(timezone.utc).replace(tzinfo=None) - self.cycle_time
             original_time = (self.backtest['ticker_index_last'] - self.backtest['ticker_index_first']) / 1000
             original_time = timedelta(seconds=original_time)
             print(f"Original time: {original_time}, test time: {test_time}, x = {original_time / test_time:.2f}")
         if prm.SAVE_DS:
             self._back_test_handler_ext()
-        loop.stop()
+        asyncio.get_event_loop().stop()
 
     def _back_test_handler_ext(self):
         # Save test data
         session_path = Path(BACKTEST_PATH,
                             f"{self.exchange}_{self.symbol}_{datetime.now().strftime('%m%d-%H-%M-%S')}")
         session_path.mkdir(parents=True)
         ds_ticker = pd.Series(self.account.ticker).astype(float)
@@ -639,14 +649,17 @@
                     self.message_log(f"Refresh t_asset: {err}", log_level=logging.WARNING)
             await asyncio.sleep(delay)
 
     async def ask_exit(self):
         self.message_log("Got signal for exit", color=Style.MAGENTA)
         self.operational_status = False
         self.s_mode_break = True
+        if self.backtest_process:
+            self.backtest_process.terminate()
+            self.message_log("Backtest process was terminated", color=Style.GREEN)
         await asyncio.sleep(HEARTBEAT)
         if prm.MODE in ('T', 'TC'):
             try:
                 await self.send_request(self.stub.stop_stream, mr.MarketRequest, symbol=self.symbol)
             except Exception as ex:
                 self.message_log(f"ask_exit: {ex}", log_level=logging.WARNING)
 
@@ -817,15 +830,15 @@
             # Remove from orders lists
             if result and result.get('status') == 'CANCELED':
                 await self.cancel_order_handler(_id, cancel_all)
             else:
                 self.message_log(f"Cancel order {_id}: Warning, not result getting")
                 _fetch_order = True
         finally:
-            if _fetch_order:
+            if prm.MODE in ('T', 'TC') and _fetch_order:
                 res = await self.fetch_order(_id, _filled_update_call=True)
                 if res.get('status') in ('CANCELED', 'EXPIRED_IN_MATCH'):
                     await self.cancel_order_handler(_id, cancel_all)
                 elif res.get('status') == 'FILLED':
                     if _id in self.canceled_order_id:
                         self.canceled_order_id.remove(_id)
                 elif not res or res.get('status') in ('NEW', 'PARTIALLY_FILLED'):
@@ -847,14 +860,15 @@
             await self.on_funds_update()
 
     async def cancel_order_timeout(self, _id):
         await asyncio.sleep(ORDER_TIMEOUT)
         if _id in self.canceled_order_id:
             self.canceled_order_id.remove(_id)
             self.on_cancel_order_error_string(_id, 'Cancel order timeout')
+        # await asyncio.sleep(0)
 
     async def transfer2master(self, symbol: str, amount: str):
         try:
             res = await self.send_request(
                 self.stub.transfer_to_master,
                 mr.MarketRequest,
                 symbol=symbol,
@@ -962,15 +976,15 @@
 
             kline_i = Klines(i.value)
             for candle in kline:
                 kline_i.refresh(candle)
             klines[i.value] = kline_i
 
         if len(klines) == len(KLINES_INIT):
-            self.tasks_list.append(asyncio.ensure_future(self.on_klines_update(klines)))
+            self.tasks_manage(self.on_klines_update(klines))
         else:
             self.message_log("Init buffered candle failed. try one else...", log_level=logging.WARNING)
             await asyncio.sleep(random.uniform(1, 5))
             self.wss_fire_up = True
 
     async def on_klines_update(self, _klines: {str: Klines}):
         _intervals = list(_klines.keys())
@@ -994,15 +1008,15 @@
                         )
             except Exception as ex:
                 self.message_log(f"Exception on WSS, on_klines_update loop closed: {ex}", log_level=logging.WARNING)
                 self.message_log(f"Exception traceback: {traceback.format_exc()}", log_level=logging.DEBUG)
                 self.wss_fire_up = True
         else:
             for i in _intervals:
-                loop.create_task(self.aiter_candles(_klines, i))
+                self.tasks_manage(self.aiter_candles(_klines, i))
 
     async def create_limit_order(self, _id: int, buy: bool, amount: str, price: str) -> None:
         self.wait_order_id.append(_id)
         _fetch_order = False
         try:
             if prm.MODE in ('T', 'TC'):
                 ts = time.time()
@@ -1042,15 +1056,15 @@
             self.message_log(f"Exception creating order {_id}: {_ex}")
         else:
             if result:
                 await self.create_order_handler(_id, result)
             else:
                 _fetch_order = True
         finally:
-            if _fetch_order:
+            if prm.MODE in ('T', 'TC') and _fetch_order:
                 await asyncio.sleep(HEARTBEAT)
                 res = await self.fetch_order(0, str(_id), _filled_update_call=True)
                 if res.get('status') in ('NEW', 'PARTIALLY_FILLED', 'FILLED'):
                     await self.create_order_handler(_id, res)
 
     async def create_order_handler(self, _id, result):
         # print(f"create_order_handler.result: {result}")
@@ -1372,26 +1386,31 @@
                 res = await self.send_request(self.stub.check_stream, mr.MarketRequest, symbol=self.symbol)
             except Exception as ex_1:
                 self.message_log(f"Exception on Check WSS: {ex_1}", log_level=logging.WARNING)
             else:
                 if res.success:
                     self.operational_status = True
 
+    def tasks_manage(self, coro):
+        _t = asyncio.create_task(coro)
+        self.tasks.add(_t)
+        _t.add_done_callback(self.tasks.discard)
+
     async def wss_declare(self):
         # Market stream
-        self.tasks_list.append(asyncio.ensure_future(self.on_ticker_update()))
+        self.tasks_manage(self.on_ticker_update())
         await self.buffered_candle()
-        self.tasks_list.append(asyncio.ensure_future(self.on_order_book_update()))
+        self.tasks_manage(self.on_order_book_update())
         if prm.MODE in ('T', 'TC'):
             # User Stream
-            self.tasks_list.append(asyncio.ensure_future(self.on_funds_update()))
-            self.tasks_list.append(asyncio.ensure_future(self.on_order_update()))
-            self.tasks_list.append(asyncio.ensure_future(self.on_balance_update()))
+            self.tasks_manage(self.on_funds_update())
+            self.tasks_manage(self.on_order_update())
+            self.tasks_manage(self.on_balance_update())
             if prm.MODE == 'TC':
-                self.tasks_list.append(asyncio.ensure_future(self.backtest_control()))
+                self.tasks_manage(self.backtest_control())
 
     async def wss_init(self, update_max_queue_size=False):
         if self.client_id:
             self.message_log(f"Init WSS, client_id: {self.client_id}")
             self.task_cancel()
             await self.wss_declare()
             # WSS start
@@ -1412,16 +1431,16 @@
                 self.wss_fire_up = False
         else:
             self.message_log("Init WSS failed, retry", log_level=logging.WARNING)
             await asyncio.sleep(random.randint(HEARTBEAT, HEARTBEAT * 5))
             self.wss_fire_up = True
 
     def task_cancel(self):
-        [task.cancel() for task in self.tasks_list if not task.done()]
-        self.tasks_list.clear()
+        [task.cancel() for task in self.tasks if not task.done()]
+        self.tasks.clear()
 
     async def main(self, _symbol):
         restore_state = None
         last_state = {}
         active_orders = []
         exch_orders_ids = []
         try:
@@ -1482,15 +1501,15 @@
                             except asyncio.CancelledError:
                                 pass  # Task cancellation should not be logged as an error.
                             except GRPCError as ex:
                                 print(f"Exception on cancel All order: {ex.status.name}, {ex.message}")
                         else:
                             [exch_orders_ids.append(int(_o['orderId'])) for _o in active_orders]
                 # Init section
-                loop.create_task(self.get_exchange_info(send_request, _symbol))
+                self.tasks_manage(self.get_exchange_info(send_request, _symbol))
                 while not self.info_symbol:
                     await asyncio.sleep(0.1)
                 if prm.LOGGING:
                     filters = self.info_symbol.get('filters')
                     for _filter in filters:
                         print(f"{filters.get(_filter).pop('filterType')}: {filters.get(_filter)}")
                 # init Strategy class var
@@ -1588,22 +1607,15 @@
                     self.order_id = json.loads(
                         last_state.pop(MS_ORDER_ID, str(int(datetime.now().strftime("%S%M")) * 1000))
                     )
                     self.start_time_ms = json.loads(
                         last_state.pop('ms_start_time_ms', str(int(time.time() * 1000)))
                     )
 
-                    # TODO Replace after 3.0.2
-                    # self.orders = jsonpickle.decode(last_state.pop(MS_ORDERS, '{}'), keys=True)
-
-                    _orders = last_state.pop(MS_ORDERS, '{}')
-                    _orders = _orders.replace('margin_wrapper', 'lib')
-                    self.orders = jsonpickle.decode(_orders, keys=True)
-                    #
-
+                    self.orders = jsonpickle.decode(last_state.pop(MS_ORDERS, '{}'), keys=True)
                     orders_keys = self.orders.keys()
                     for _id in exch_orders_ids:
                         if _id not in orders_keys:
                             _order = next((_o for _o in active_orders if int(_o["orderId"]) == _id))
                             self.orders[_id] = Order(_order)
                             self.message_log(
                                 f"Was restored order {_id}({_order.get('clientOrderId')}) from exchange data",
@@ -1637,22 +1649,22 @@
                     else:
                         self.init()
                         self.start()
 
             if prm.MODE in ('T', 'TC'):
                 await self.wss_init()
                 await self.wait_wss_init()
-                loop.create_task(save_to_csv())
-                loop.create_task(self.buffered_orders())
+                self.tasks_manage(save_to_csv())
+                self.tasks_manage(self.buffered_orders())
                 if self.session.client.real_market:
-                    loop.create_task(self.save_asset())
+                    self.tasks_manage(self.save_asset())
                 if not restore_state:
                     self.start()
 
-            loop.create_task(self.heartbeat(self.session))
+            self.tasks_manage(self.heartbeat(self.session))
 
         except (KeyboardInterrupt, SystemExit):
             # noinspection PyProtectedMember, PyUnresolvedReferences
             os._exit(1)
 
     # region AbstractMethod
     @abstractmethod
```

### Comparing `martin_binance-3.0.3/martin_binance/telegram_utils.py` & `martin_binance-3.0.4/martin_binance/telegram_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/templates/cli_0_BTCUSDT.py` & `martin_binance-3.0.4/martin_binance/templates/cli_0_BTCUSDT.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,20 +133,20 @@
         from martin_binance.executor import Strategy
         strategy = Strategy()
     loop = asyncio.get_event_loop()
     try:
         loop.create_task(strategy.main(ex.SYMBOL))
         loop.run_forever()
     except KeyboardInterrupt:
-        pass
+        pass  # user interrupt
     finally:
         try:
             loop.run_until_complete(strategy.ask_exit())
         except (asyncio.CancelledError, KeyboardInterrupt):
-            pass
+            pass  # user interrupt
         except Exception as _err:
             print(f"Error: {_err}")
         loop.run_until_complete(loop.shutdown_asyncgens())
     return strategy
 
 
 if __name__ == "__main__":
```

### Comparing `martin_binance-3.0.3/martin_binance/templates/cli_1_BTCUSDT.py` & `martin_binance-3.0.4/martin_binance/templates/cli_1_BTCUSDT.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,20 +133,20 @@
         from martin_binance.executor import Strategy
         strategy = Strategy()
     loop = asyncio.get_event_loop()
     try:
         loop.create_task(strategy.main(ex.SYMBOL))
         loop.run_forever()
     except KeyboardInterrupt:
-        pass
+        pass   # user interrupt
     finally:
         try:
             loop.run_until_complete(strategy.ask_exit())
         except (asyncio.CancelledError, KeyboardInterrupt):
-            pass
+            pass  # user interrupt
         except Exception as _err:
             print(f"Error: {_err}")
         loop.run_until_complete(loop.shutdown_asyncgens())
     return strategy
 
 
 if __name__ == "__main__":
```

### Comparing `martin_binance-3.0.3/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py` & `martin_binance-3.0.4/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,20 +133,20 @@
         from martin_binance.executor import Strategy
         strategy = Strategy()
     loop = asyncio.get_event_loop()
     try:
         loop.create_task(strategy.main(ex.SYMBOL))
         loop.run_forever()
     except KeyboardInterrupt:
-        pass
+        pass  # user interrupt
     finally:
         try:
             loop.run_until_complete(strategy.ask_exit())
         except (asyncio.CancelledError, KeyboardInterrupt):
-            pass
+            pass  # user interrupt
         except Exception as _err:
             print(f"Error: {_err}")
         loop.run_until_complete(loop.shutdown_asyncgens())
     return strategy
 
 
 if __name__ == "__main__":
```

### Comparing `martin_binance-3.0.3/martin_binance/templates/cli_3_BTCUSDT.py` & `martin_binance-3.0.4/martin_binance/templates/cli_3_BTCUSDT.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,20 +133,20 @@
         from martin_binance.executor import Strategy
         strategy = Strategy()
     loop = asyncio.get_event_loop()
     try:
         loop.create_task(strategy.main(ex.SYMBOL))
         loop.run_forever()
     except KeyboardInterrupt:
-        pass
+        pass  # user interrupt
     finally:
         try:
             loop.run_until_complete(strategy.ask_exit())
         except (asyncio.CancelledError, KeyboardInterrupt):
-            pass
+            pass  # user interrupt
         except Exception as _err:
             print(f"Error: {_err}")
         loop.run_until_complete(loop.shutdown_asyncgens())
     return strategy
 
 
 if __name__ == "__main__":
```

### Comparing `martin_binance-3.0.3/martin_binance/templates/funds_rate.db` & `martin_binance-3.0.4/martin_binance/templates/funds_rate.db`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/templates/ms_cfg.toml` & `martin_binance-3.0.4/martin_binance/templates/ms_cfg.toml`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/martin_binance/templates/trial_params.json` & `martin_binance-3.0.4/martin_binance/templates/trial_params.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.3/pyproject.toml` & `martin_binance-3.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.9"
 
 dependencies = [
-    "exchanges-wrapper==2.1.8",
+    "exchanges-wrapper==2.1.9",
     "jsonpickle==3.0.2",
     "psutil==5.9.6",
     "requests==2.31.0",
     "libtmux==0.23.2",
     "colorama==0.4.6",
     "prometheus-client==0.18.0",
     "optuna==3.4.0",
```

### Comparing `martin_binance-3.0.3/PKG-INFO` & `martin_binance-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 3.0.3
+Version: 3.0.4
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==2.1.8
+Requires-Dist: exchanges-wrapper==2.1.9
 Requires-Dist: jsonpickle==3.0.2
 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0
 Requires-Dist: libtmux==0.23.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: prometheus-client==0.18.0
 Requires-Dist: optuna==3.4.0
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 3.0.3 Summary: Free trading
+Metadata-Version: 2.1 Name: martin-binance Version: 3.0.4 Summary: Free trading
 system for Binance SPOT API Author-email: Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: MacOS Requires-Dist: exchanges-
-wrapper==2.1.8 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
+wrapper==2.1.9 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0 Requires-Dist: libtmux==0.23.2 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.18.0 Requires-Dist:
 optuna==3.4.0 Requires-Dist: plotly==5.18.0 Requires-Dist: pandas==2.1.2
 Requires-Dist: dash>=2.15.0 Requires-Dist: future==0.18.3 Requires-Dist:
 inquirer==3.1.3 Requires-Dist: scikit-learn==1.3.2 Requires-Dist: tqdm==4.66.1
 Requires-Dist: ujson~=5.9.0 Requires-Dist: orjson~=3.9.15 Requires-Dist:
 pyarrow~=14.0.2 Requires-Dist: shortuuid~=1.0.11 Requires-Dist: numpy~=1.23.4
```

