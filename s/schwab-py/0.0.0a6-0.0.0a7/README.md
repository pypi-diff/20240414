# Comparing `tmp/schwab-py-0.0.0a6.tar.gz` & `tmp/schwab-py-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-py-0.0.0a6.tar", last modified: Mon Apr  8 21:09:56 2024, max compression
+gzip compressed data, was "schwab-py-0.0.0a7.tar", last modified: Sun Apr 14 17:42:34 2024, max compression
```

## Comparing `schwab-py-0.0.0a6.tar` & `schwab-py-0.0.0a7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.222693 schwab-py-0.0.0a6/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a6/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-08 21:09:56.222634 schwab-py-0.0.0a6/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a6/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.220024 schwab-py-0.0.0a6/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a6/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    24395 2024-04-08 21:07:33.000000 schwab-py-0.0.0a6/schwab/auth.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.220592 schwab-py-0.0.0a6/schwab/client/
--rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a6/schwab/client/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a6/schwab/client/asynchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    18577 2024-04-08 16:32:11.000000 schwab-py-0.0.0a6/schwab/client/base.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-06 13:43:58.000000 schwab-py-0.0.0a6/schwab/client/synchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a6/schwab/debug.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.221239 schwab-py-0.0.0a6/schwab/orders/
--rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    10301 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/common.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5739 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/equities.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    14130 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/generic.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    17265 2024-04-06 23:27:37.000000 schwab-py-0.0.0a6/schwab/orders/options.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a6/schwab/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-08 21:09:23.000000 schwab-py-0.0.0a6/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.222163 schwab-py-0.0.0a6/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)      532 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-08 21:09:56.000000 schwab-py-0.0.0a6/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-08 21:09:56.223012 schwab-py-0.0.0a6/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-06 13:16:58.000000 schwab-py-0.0.0a6/setup.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-08 21:09:56.222002 schwab-py-0.0.0a6/tests/
--rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a6/tests/test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.278700 schwab-py-0.0.0a7/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a7/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 17:42:34.278627 schwab-py-0.0.0a7/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a7/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.276033 schwab-py-0.0.0a7/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a7/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    24395 2024-04-08 21:07:33.000000 schwab-py-0.0.0a7/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.276592 schwab-py-0.0.0a7/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a7/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a7/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    25591 2024-04-14 17:39:18.000000 schwab-py-0.0.0a7/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-06 13:43:58.000000 schwab-py-0.0.0a7/schwab/client/synchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a7/schwab/debug.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.277221 schwab-py-0.0.0a7/schwab/orders/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-04-06 23:27:37.000000 schwab-py-0.0.0a7/schwab/orders/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    11013 2024-04-14 17:35:12.000000 schwab-py-0.0.0a7/schwab/orders/common.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-04-14 17:35:34.000000 schwab-py-0.0.0a7/schwab/orders/equities.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    14184 2024-04-14 17:37:24.000000 schwab-py-0.0.0a7/schwab/orders/generic.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17394 2024-04-14 17:35:49.000000 schwab-py-0.0.0a7/schwab/orders/options.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a7/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-14 17:41:58.000000 schwab-py-0.0.0a7/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.278144 schwab-py-0.0.0a7/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)      532 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-14 17:42:34.000000 schwab-py-0.0.0a7/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-14 17:42:34.279022 schwab-py-0.0.0a7/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-06 13:16:58.000000 schwab-py-0.0.0a7/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 17:42:34.277984 schwab-py-0.0.0a7/tests/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a7/tests/test.py
```

### Comparing `schwab-py-0.0.0a6/LICENSE` & `schwab-py-0.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/PKG-INFO` & `schwab-py-0.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
```

### Comparing `schwab-py-0.0.0a6/README.rst` & `schwab-py-0.0.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/schwab/auth.py` & `schwab-py-0.0.0a7/schwab/auth.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/schwab/client/asynchronous.py` & `schwab-py-0.0.0a7/schwab/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/schwab/client/synchronous.py` & `schwab-py-0.0.0a7/schwab/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/schwab/debug.py` & `schwab-py-0.0.0a7/schwab/debug.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/schwab/orders/__init__.py` & `schwab-py-0.0.0a7/schwab/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/schwab/orders/common.py` & `schwab-py-0.0.0a7/schwab/orders/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,20 @@
     #: may see partial executions over the lifetime of the order.
     GOOD_TILL_CANCEL = 'GOOD_TILL_CANCEL'
 
     #: Either execute the order immediately at the specified price, or cancel it
     #: immediately.
     FILL_OR_KILL = 'FILL_OR_KILL'
 
+    # TODO: Document these
+    IMMEDIATE_OR_CANCEL = 'IMMEDIATE_OR_CANCEL'
+    END_OF_WEEK = 'END_OF_WEEK'
+    END_OF_MONTH = 'END_OF_MONTH'
+    NEXT_END_OF_MONTH = 'NEXT_END_OF_MONTH'
+
 
 class Session(Enum):
     '''
     The market session during which the order trade should be executed.
     '''
 
     #: Normal market hours, from 9:30am to 4:00pm Eastern.
@@ -63,15 +69,15 @@
     #: Orders are active during all trading sessions except the overnight
     #: session. This is the union of ``NORMAL``, ``AM``, and ``PM``.
     SEAMLESS = 'SEAMLESS'
 
 
 class OrderType(Enum):
     '''
-    Type of equity or option order to place.
+    Type of order to place.
     '''
 
     #: Execute the order immediately at the best-available price.
     #: `More Info <https://www.investopedia.com/terms/m/marketorder.asp>`__.
     MARKET = 'MARKET'
 
     #: Execute the order at your price or better.
@@ -90,27 +96,31 @@
 
     #: Similar to ``STOP``, except if the price moves in your favor, the stop
     #: price is adjusted in that direction. Places a market order if the stop
     #: condition is met.
     #: `More info <https://www.investopedia.com/terms/t/trailingstop.asp>`__.
     TRAILING_STOP = 'TRAILING_STOP'
 
-    #: Similar to ``STOP_LIMIT``, except if the price moves in your favor, the
-    #: stop price is adjusted in that direction. Places a limit order at the
-    #: specified price if the stop condition is met.
-    #: `More info <https://www.investopedia.com/terms/t/trailingstop.asp>`__.
-    TRAILING_STOP_LIMIT = 'TRAILING_STOP_LIMIT'
+    CABINET = 'CABINET'
+
+    NON_MARKETABLE = 'NON_MARKETABLE'
 
     #: Place the order at the closing price immediately upon market close.
     #: `More info <https://www.investopedia.com/terms/m/marketonclose.asp>`__
     MARKET_ON_CLOSE = 'MARKET_ON_CLOSE'
 
     #: Exercise an option.
     EXERCISE = 'EXERCISE'
 
+    #: Similar to ``STOP_LIMIT``, except if the price moves in your favor, the
+    #: stop price is adjusted in that direction. Places a limit order at the
+    #: specified price if the stop condition is met.
+    #: `More info <https://www.investopedia.com/terms/t/trailingstop.asp>`__.
+    TRAILING_STOP_LIMIT = 'TRAILING_STOP_LIMIT'
+
     #: Place an order for an options spread resulting in a net debit.
     #: `More info <https://www.investopedia.com/ask/answers/042215/
     #: whats-difference-between-credit-spread-and-debt-spread.asp>`__
     NET_DEBIT = 'NET_DEBIT'
 
     #: Place an order for an options spread resulting in a net credit.
     #: `More info <https://www.investopedia.com/ask/answers/042215/
@@ -119,14 +129,16 @@
 
     #: Place an order for an options spread resulting in neither a credit nor a
     #: debit.
     #: `More info <https://www.investopedia.com/ask/answers/042215/
     #: whats-difference-between-credit-spread-and-debt-spread.asp>`__
     NET_ZERO = 'NET_ZERO'
 
+    LIMIT_ON_CLOSE = 'LIMIT_ON_CLOSE'
+
 
 class ComplexOrderStrategyType(Enum):
     '''
     Explicit order strategies for executing multi-leg options orders.
     '''
 
     #: No complex order strategy. This is the default.
@@ -189,14 +201,17 @@
     #: `Unbalanced butterfy spread  <https://tickertape.tdameritrade.com/
     #: trading/unbalanced-butterfly-strong-directional-bias-15913>`__
     UNBALANCED_BUTTERFLY = 'UNBALANCED_BUTTERFLY'
     UNBALANCED_CONDOR = 'UNBALANCED_CONDOR'
     UNBALANCED_IRON_CONDOR = 'UNBALANCED_IRON_CONDOR'
     UNBALANCED_VERTICAL_ROLL = 'UNBALANCED_VERTICAL_ROLL'
 
+    #: Mutual fund swap
+    MUTUAL_FUND_SWAP = 'MUTUAL_FUND_SWAP'
+
     #: A custom multi-leg order strategy.
     CUSTOM = 'CUSTOM'
 
 
 class Destination(Enum):
     '''
     Destinations for when you want to request a specific destination for your
@@ -257,14 +272,24 @@
 
 class PriceLinkType(Enum):
     VALUE = 'VALUE'
     PERCENT = 'PERCENT'
     TICK = 'TICK'
 
 
+class TaxLotMethod(Enum):
+    FIFO = 'FIFO'
+    LIFO = 'LIFO'
+    HIGH_COST = 'HIGH_COST'
+    LOW_COST = 'LOW_COST'
+    AVERAGE_COST = 'AVERAGE_COST'
+    SPECIFIC_LOT = 'SPECIFIC_LOT'
+    LOSS_HARVESTER = 'LOSS_HARVESTER'
+
+
 class EquityInstruction(Enum):
     '''
     Instructions for opening and closing equity positions.
     '''
 
     #: Open a long equity position
     BUY = 'BUY'
@@ -317,14 +342,21 @@
     '''
     Rules for composite orders.
     '''
 
     #: No chaining, only a single order is submitted
     SINGLE = 'SINGLE'
 
+    CANCEL = 'CANCEL'
+    RECALL = 'RECALL'
+    PAIR = 'PAIR'
+    FLATTEN = 'FLATTEN'
+    TWO_DAY_SWAP = 'TWO_DAY_SWAP'
+    BLAST_ALL = 'BLAST_ALL'
+
     #: Execution of one order cancels the other
     OCO = 'OCO'
 
     #: Execution of one order triggers placement of the other
     TRIGGER = 'TRIGGER'
```

### Comparing `schwab-py-0.0.0a6/schwab/orders/equities.py` & `schwab-py-0.0.0a7/schwab/orders/equities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from enum import Enum
 
-from tda.orders.common import Duration, Session
+from schwab.orders.common import Duration, Session
 
 
 ##########################################################################
 # Buy orders
 
 
 def equity_buy_market(symbol, quantity):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for an equity
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for an equity
     buy market order.
     '''
-    from tda.orders.common import Duration, EquityInstruction
-    from tda.orders.common import OrderStrategyType, OrderType, Session
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.common import Duration, EquityInstruction
+    from schwab.orders.common import OrderStrategyType, OrderType, Session
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_type(OrderType.MARKET)
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_equity_leg(EquityInstruction.BUY, symbol, quantity))
 
 
 def equity_buy_limit(symbol, quantity, price):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for an equity
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for an equity
     buy limit order.
     '''
-    from tda.orders.common import Duration, EquityInstruction
-    from tda.orders.common import OrderStrategyType, OrderType, Session
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.common import Duration, EquityInstruction
+    from schwab.orders.common import OrderStrategyType, OrderType, Session
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_type(OrderType.LIMIT)
             .set_price(price)
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -43,37 +43,37 @@
 
 ##########################################################################
 # Sell orders
 
 
 def equity_sell_market(symbol, quantity):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for an equity
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for an equity
     sell market order.
     '''
-    from tda.orders.common import Duration, EquityInstruction
-    from tda.orders.common import OrderStrategyType, OrderType, Session
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.common import Duration, EquityInstruction
+    from schwab.orders.common import OrderStrategyType, OrderType, Session
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_type(OrderType.MARKET)
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_equity_leg(EquityInstruction.SELL, symbol, quantity))
 
 
 def equity_sell_limit(symbol, quantity, price):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for an equity
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for an equity
     sell limit order.
     '''
-    from tda.orders.common import Duration, EquityInstruction
-    from tda.orders.common import OrderStrategyType, OrderType, Session
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.common import Duration, EquityInstruction
+    from schwab.orders.common import OrderStrategyType, OrderType, Session
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_type(OrderType.LIMIT)
             .set_price(price)
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -81,37 +81,37 @@
 
 ##########################################################################
 # Short sell orders
 
 
 def equity_sell_short_market(symbol, quantity):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for an equity
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for an equity
     short sell market order.
     '''
-    from tda.orders.common import Duration, EquityInstruction
-    from tda.orders.common import OrderStrategyType, OrderType, Session
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.common import Duration, EquityInstruction
+    from schwab.orders.common import OrderStrategyType, OrderType, Session
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_type(OrderType.MARKET)
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_equity_leg(EquityInstruction.SELL_SHORT, symbol, quantity))
 
 
 def equity_sell_short_limit(symbol, quantity, price):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for an equity
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for an equity
     short sell limit order.
     '''
-    from tda.orders.common import Duration, EquityInstruction
-    from tda.orders.common import OrderStrategyType, OrderType, Session
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.common import Duration, EquityInstruction
+    from schwab.orders.common import OrderStrategyType, OrderType, Session
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_type(OrderType.LIMIT)
             .set_price(price)
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -119,37 +119,37 @@
 
 ##########################################################################
 # Buy to cover orders
 
 
 def equity_buy_to_cover_market(symbol, quantity):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for an equity
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for an equity
     buy-to-cover market order.
     '''
-    from tda.orders.common import Duration, EquityInstruction
-    from tda.orders.common import OrderStrategyType, OrderType, Session
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.common import Duration, EquityInstruction
+    from schwab.orders.common import OrderStrategyType, OrderType, Session
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_type(OrderType.MARKET)
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_equity_leg(EquityInstruction.BUY_TO_COVER, symbol, quantity))
 
 
 def equity_buy_to_cover_limit(symbol, quantity, price):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for an equity
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for an equity
     buy-to-cover limit order.
     '''
-    from tda.orders.common import Duration, EquityInstruction
-    from tda.orders.common import OrderStrategyType, OrderType, Session
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.common import Duration, EquityInstruction
+    from schwab.orders.common import OrderStrategyType, OrderType, Session
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_type(OrderType.LIMIT)
             .set_price(price)
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
```

### Comparing `schwab-py-0.0.0a6/schwab/orders/generic.py` & `schwab-py-0.0.0a7/schwab/orders/generic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
-from tda.orders import common
-from tda.utils import EnumEnforcer
+from schwab.orders import common
+from schwab.utils import EnumEnforcer
 
 import httpx
 
 
 def _build_object(obj):
     # Literals are passed straight through
     if isinstance(obj, str) or isinstance(obj, int) or isinstance(obj, float):
@@ -39,15 +39,15 @@
         return '{:.2f}'.format(float(int(flt * 100)) / 100.0)
 
 
 class OrderBuilder(EnumEnforcer):
     '''
     Helper class to create arbitrarily complex orders. Note this class simply
     implements the order schema defined in the `documentation
-    <https://developer.tdameritrade.com/account-access/apis/post/accounts/
+    <https://developer.schwabmeritrade.com/account-access/apis/post/accounts/
     %7BaccountId%7D/orders-0>`__, with no attempts to validate the result.
     Orders created using this class may be rejected or may never fill. Use at
     your own risk.
     '''
 
     def __init__(self, *, enforce_enums=True):
         super().__init__(enforce_enums)
@@ -71,15 +71,15 @@
         self._specialInstruction = None
         self._orderStrategyType = None
         self._childOrderStrategies = None
 
     # Session
     def set_session(self, session):
         '''
-        Set the order session. See :class:`~tda.orders.common.Session` for
+        Set the order session. See :class:`~schwab.orders.common.Session` for
         details.
         '''
         session = self.convert_enum(session, common.Session)
         self._session = session
         return self
 
     def clear_session(self):
@@ -88,15 +88,15 @@
         '''
         self._session = None
         return self
 
     # Duration
     def set_duration(self, duration):
         '''
-        Set the order duration. See :class:`~tda.orders.common.Duration` for
+        Set the order duration. See :class:`~schwab.orders.common.Duration` for
         details.
         '''
         duration = self.convert_enum(duration, common.Duration)
         self._duration = duration
         return self
 
     def clear_duration(self):
@@ -105,15 +105,15 @@
         '''
         self._duration = None
         return self
 
     # OrderType
     def set_order_type(self, order_type):
         '''
-        Set the order type. See :class:`~tda.orders.common.OrderType` for
+        Set the order type. See :class:`~schwab.orders.common.OrderType` for
         details.
         '''
         order_type = self.convert_enum(order_type, common.OrderType)
         self._orderType = order_type
         return self
 
     def clear_order_type(self):
@@ -123,15 +123,15 @@
         self._orderType = None
         return self
 
     # ComplexOrderStrategyType
     def set_complex_order_strategy_type(self, complex_order_strategy_type):
         '''
         Set the complex order strategy type. See
-        :class:`~tda.orders.common.ComplexOrderStrategyType` for details.
+        :class:`~schwab.orders.common.ComplexOrderStrategyType` for details.
         '''
         complex_order_strategy_type = self.convert_enum(
             complex_order_strategy_type, common.ComplexOrderStrategyType)
         self._complexOrderStrategyType = complex_order_strategy_type
         return self
 
     def clear_complex_order_strategy_type(self):
@@ -159,15 +159,15 @@
         self._quantity = None
         return self
 
     # RequestedDestination
     def set_requested_destination(self, requested_destination):
         '''
         Set the requested destination. See
-        :class:`~tda.orders.common.Destination` for details.
+        :class:`~schwab.orders.common.Destination` for details.
         '''
         requested_destination = self.convert_enum(
             requested_destination, common.Destination)
         self._requestedDestination = requested_destination
         return self
 
     def clear_requested_destination(self):
@@ -204,15 +204,15 @@
         self._stopPrice = None
         return self
 
     # StopPriceLinkBasis
     def set_stop_price_link_basis(self, stop_price_link_basis):
         '''
         Set the stop price link basis. See
-        :class:`~tda.orders.common.StopPriceLinkBasis` for details.
+        :class:`~schwab.orders.common.StopPriceLinkBasis` for details.
         '''
         stop_price_link_basis = self.convert_enum(
             stop_price_link_basis, common.StopPriceLinkBasis)
         self._stopPriceLinkBasis = stop_price_link_basis
         return self
 
     def clear_stop_price_link_basis(self):
@@ -222,15 +222,15 @@
         self._stopPriceLinkBasis = None
         return self
 
     # StopPriceLinkType
     def set_stop_price_link_type(self, stop_price_link_type):
         '''
         Set the stop price link type. See
-        :class:`~tda.orders.common.StopPriceLinkType` for details.
+        :class:`~schwab.orders.common.StopPriceLinkType` for details.
         '''
         stop_price_link_type = self.convert_enum(
             stop_price_link_type, common.StopPriceLinkType)
         self._stopPriceLinkType = stop_price_link_type
         return self
 
     def clear_stop_price_link_type(self):
@@ -255,15 +255,15 @@
         self._stopPriceOffset = None
         return self
 
     # StopType
     def set_stop_type(self, stop_type):
         '''
         Set the stop type. See
-        :class:`~tda.orders.common.StopType` for more details.
+        :class:`~schwab.orders.common.StopType` for more details.
         '''
         stop_type = self.convert_enum(stop_type, common.StopType)
         self._stopType = stop_type
         return self
 
     def clear_stop_type(self):
         '''
@@ -272,15 +272,15 @@
         self._stopType = None
         return self
 
     # PriceLinkBasis
     def set_price_link_basis(self, price_link_basis):
         '''
         Set the price link basis. See
-        :class:`~tda.orders.common.PriceLinkBasis` for details.
+        :class:`~schwab.orders.common.PriceLinkBasis` for details.
         '''
         price_link_basis = self.convert_enum(
             price_link_basis, common.PriceLinkBasis)
         self._priceLinkBasis = price_link_basis
         return self
 
     def clear_price_link_basis(self):
@@ -290,15 +290,15 @@
         self._priceLinkBasis = None
         return self
 
     # PriceLinkType
     def set_price_link_type(self, price_link_type):
         '''
         Set the price link type. See
-        :class:`~tda.orders.common.PriceLinkType` for more details.
+        :class:`~schwab.orders.common.PriceLinkType` for more details.
         '''
         price_link_type = self.convert_enum(
             price_link_type, common.PriceLinkType)
         self._priceLinkType = price_link_type
         return self
 
     def clear_price_link_type(self):
@@ -352,15 +352,15 @@
         self._activationPrice = None
         return self
 
     # SpecialInstruction
     def set_special_instruction(self, special_instruction):
         '''
         Set the special instruction. See
-        :class:`~tda.orders.common.SpecialInstruction` for details.
+        :class:`~schwab.orders.common.SpecialInstruction` for details.
         '''
         special_instruction = self.convert_enum(
             special_instruction, common.SpecialInstruction)
         self._specialInstruction = special_instruction
         return self
 
     def clear_special_instruction(self):
@@ -370,15 +370,15 @@
         self._specialInstruction = None
         return self
 
     # OrderStrategyType
     def set_order_strategy_type(self, order_strategy_type):
         '''
         Set the order strategy type. See
-        :class:`~tda.orders.common.OrderStrategyType` for more details.
+        :class:`~schwab.orders.common.OrderStrategyType` for more details.
         '''
         order_strategy_type = self.convert_enum(
             order_strategy_type, common.OrderStrategyType)
         self._orderStrategyType = order_strategy_type
         return self
 
     def clear_order_strategy_type(self):
@@ -389,15 +389,15 @@
         return self
 
     # ChildOrderStrategies
     def add_child_order_strategy(self, child_order_strategy):
         if isinstance(child_order_strategy, httpx.Response):
             raise ValueError(
                     'Child order cannot be a response. See here for ' +
-                    'details: https://tda-api.readthedocs.io/en/latest/' +
+                    'details: https://schwab-api.readthedocs.io/en/latest/' +
                     'order-templates.html#utility-methods')
 
         if (not isinstance(child_order_strategy, OrderBuilder)
                 and not isinstance(child_order_strategy, dict)):
             raise ValueError('child order must be OrderBuilder or dict')
 
         if self._childOrderStrategies is None:
@@ -429,29 +429,29 @@
         return self
 
     def add_equity_leg(self, instruction, symbol, quantity):
         '''
         Add an equity order leg.
 
         :param instruction: Instruction for the leg. See
-                            :class:`~tda.orders.common.EquityInstruction` for
+                            :class:`~schwab.orders.common.EquityInstruction` for
                             valid options.
         :param symbol: Equity symbol
         :param quantity: Number of shares for the order
         '''
         instruction = self.convert_enum(instruction, common.EquityInstruction)
         return self.__add_order_leg(
             instruction, common.EquityInstrument(symbol), quantity)
 
     def add_option_leg(self, instruction, symbol, quantity):
         '''
         Add an option order leg.
 
         :param instruction: Instruction for the leg. See
-                            :class:`~tda.orders.common.OptionInstruction` for
+                            :class:`~schwab.orders.common.OptionInstruction` for
                             valid options.
         :param symbol: Option symbol
         :param quantity: Number of contracts for the order
         '''
         instruction = self.convert_enum(instruction, common.OptionInstruction)
         return self.__add_order_leg(
             instruction, common.OptionInstrument(symbol), quantity)
```

### Comparing `schwab-py-0.0.0a6/schwab/orders/options.py` & `schwab-py-0.0.0a7/schwab/orders/options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 
-from tda.orders.generic import OrderBuilder
+from schwab.orders.generic import OrderBuilder
 
 
 def _parse_expiration_date(expiration_date):
     date = None
     try:
         date = datetime.datetime.strptime(expiration_date, '%m%d%y')
         return datetime.date(year=date.year, month=date.month, day=date.day)
@@ -30,15 +30,15 @@
     Note while each of the individual parts is validated by itself, the
     option symbol itself may not represent a traded option:
 
      * Some underlyings do not support options.
      * Not all dates have valid option expiration dates.
      * Not all strike prices are valid options strikes.
 
-    You can use :meth:`~tda.client.Client.get_option_chain` to obtain real
+    You can use :meth:`~schwab.client.Client.get_option_chain` to obtain real
     option symbols for an underlying, as well as extensive data in pricing,
     bid/ask spread, volume, etc.
 
     :param underlying_symbol: Symbol of the underlying. Not validated.
     :param expiration_date: Expiration date. Accepts ``datetime.date``,
                             ``datetime.datetime``, or strings with the
                             format ``[Two digit month][Two digit day][Two
@@ -145,137 +145,137 @@
             self.expiration_date.strftime('%m%d%y'),
             self.contract_type,
             self.strike_price
         )
 
 
 def __base_builder():
-    from tda.orders.common import Duration, Session
+    from schwab.orders.common import Duration, Session
 
     return (OrderBuilder()
             .set_session(Session.NORMAL)
             .set_duration(Duration.DAY))
 
 
 ################################################################################
 # Single options
 
 # Buy to Open
 
 def option_buy_to_open_market(symbol, quantity):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for a
     buy-to-open market order.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.MARKET)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_option_leg(OptionInstruction.BUY_TO_OPEN, symbol, quantity))
 
 
 def option_buy_to_open_limit(symbol, quantity, price):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for a
     buy-to-open limit order.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.LIMIT)
             .set_price(price)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_option_leg(OptionInstruction.BUY_TO_OPEN, symbol, quantity)
             )
 
 
 # Sell to Open
 
 def option_sell_to_open_market(symbol, quantity):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for a
     sell-to-open market order.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.MARKET)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_option_leg(OptionInstruction.SELL_TO_OPEN, symbol, quantity))
 
 
 def option_sell_to_open_limit(symbol, quantity, price):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for a
     sell-to-open limit order.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.LIMIT)
             .set_price(price)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_option_leg(OptionInstruction.SELL_TO_OPEN, symbol, quantity)
             )
 
 
 # Buy to Close
 
 
 def option_buy_to_close_market(symbol, quantity):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for a
     buy-to-close market order.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.MARKET)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_option_leg(OptionInstruction.BUY_TO_CLOSE, symbol, quantity))
 
 
 def option_buy_to_close_limit(symbol, quantity, price):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for a
     buy-to-close limit order.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.LIMIT)
             .set_price(price)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_option_leg(OptionInstruction.BUY_TO_CLOSE, symbol, quantity)
             )
 
 
 # Sell to Close
 
 
 def option_sell_to_close_market(symbol, quantity):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for a
     sell-to-close market order.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.MARKET)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_option_leg(OptionInstruction.SELL_TO_CLOSE, symbol, quantity))
 
 
 def option_sell_to_close_limit(symbol, quantity, price):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` for a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` for a
     sell-to-close limit order.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.LIMIT)
             .set_price(price)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
             .add_option_leg(OptionInstruction.SELL_TO_CLOSE, symbol, quantity)
             )
@@ -285,19 +285,19 @@
 # Verticals
 
 # Bull Call
 
 def bull_call_vertical_open(
         long_call_symbol, short_call_symbol, quantity, net_debit):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` that opens a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` that opens a
     bull call vertical position. See :ref:`vertical_spreads` for details.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
-    from tda.orders.common import ComplexOrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import ComplexOrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.NET_DEBIT)
             .set_complex_order_strategy_type(ComplexOrderStrategyType.VERTICAL)
             .set_price(net_debit)
             .set_quantity(quantity)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -306,19 +306,19 @@
             .add_option_leg(
                 OptionInstruction.SELL_TO_OPEN, short_call_symbol, quantity))
 
 
 def bull_call_vertical_close(
         long_call_symbol, short_call_symbol, quantity, net_credit):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` that closes a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` that closes a
     bull call vertical position. See :ref:`vertical_spreads` for details.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
-    from tda.orders.common import ComplexOrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import ComplexOrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.NET_CREDIT)
             .set_complex_order_strategy_type(ComplexOrderStrategyType.VERTICAL)
             .set_price(net_credit)
             .set_quantity(quantity)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -329,19 +329,19 @@
 
 
 # Bear Call
 
 def bear_call_vertical_open(
         short_call_symbol, long_call_symbol, quantity, net_credit):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` that opens a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` that opens a
     bear call vertical position. See :ref:`vertical_spreads` for details.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
-    from tda.orders.common import ComplexOrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import ComplexOrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.NET_CREDIT)
             .set_complex_order_strategy_type(ComplexOrderStrategyType.VERTICAL)
             .set_price(net_credit)
             .set_quantity(quantity)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -350,19 +350,19 @@
             .add_option_leg(
                 OptionInstruction.BUY_TO_OPEN, long_call_symbol, quantity))
 
 
 def bear_call_vertical_close(
         short_call_symbol, long_call_symbol, quantity, net_debit):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` that closes a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` that closes a
     bear call vertical position. See :ref:`vertical_spreads` for details.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
-    from tda.orders.common import ComplexOrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import ComplexOrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.NET_DEBIT)
             .set_complex_order_strategy_type(ComplexOrderStrategyType.VERTICAL)
             .set_price(net_debit)
             .set_quantity(quantity)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -373,19 +373,19 @@
 
 
 # Bull Put
 
 def bull_put_vertical_open(
         long_put_symbol, short_put_symbol, quantity, net_credit):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` that opens a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` that opens a
     bull put vertical position. See :ref:`vertical_spreads` for details.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
-    from tda.orders.common import ComplexOrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import ComplexOrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.NET_CREDIT)
             .set_complex_order_strategy_type(ComplexOrderStrategyType.VERTICAL)
             .set_price(net_credit)
             .set_quantity(quantity)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -394,19 +394,19 @@
             .add_option_leg(
                 OptionInstruction.SELL_TO_OPEN, short_put_symbol, quantity))
 
 
 def bull_put_vertical_close(
         long_put_symbol, short_put_symbol, quantity, net_debit):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` that closes a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` that closes a
     bull put vertical position. See :ref:`vertical_spreads` for details.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
-    from tda.orders.common import ComplexOrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import ComplexOrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.NET_DEBIT)
             .set_complex_order_strategy_type(ComplexOrderStrategyType.VERTICAL)
             .set_price(net_debit)
             .set_quantity(quantity)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -417,19 +417,19 @@
 
 
 # Bear Put
 
 def bear_put_vertical_open(
         short_put_symbol, long_put_symbol, quantity, net_debit):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` that opens a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` that opens a
     bear put vertical position. See :ref:`vertical_spreads` for details.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
-    from tda.orders.common import ComplexOrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import ComplexOrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.NET_DEBIT)
             .set_complex_order_strategy_type(ComplexOrderStrategyType.VERTICAL)
             .set_price(net_debit)
             .set_quantity(quantity)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
@@ -438,19 +438,19 @@
             .add_option_leg(
                 OptionInstruction.BUY_TO_OPEN, long_put_symbol, quantity))
 
 
 def bear_put_vertical_close(
         short_put_symbol, long_put_symbol, quantity, net_credit):
     '''
-    Returns a pre-filled :class:`~tda.orders.generic.OrderBuilder` that closes a
+    Returns a pre-filled :class:`~schwab.orders.generic.OrderBuilder` that closes a
     bear put vertical position. See :ref:`vertical_spreads` for details.
     '''
-    from tda.orders.common import OptionInstruction, OrderType, OrderStrategyType
-    from tda.orders.common import ComplexOrderStrategyType
+    from schwab.orders.common import OptionInstruction, OrderType, OrderStrategyType
+    from schwab.orders.common import ComplexOrderStrategyType
 
     return (__base_builder()
             .set_order_type(OrderType.NET_CREDIT)
             .set_complex_order_strategy_type(ComplexOrderStrategyType.VERTICAL)
             .set_price(net_credit)
             .set_quantity(quantity)
             .set_order_strategy_type(OrderStrategyType.SINGLE)
```

### Comparing `schwab-py-0.0.0a6/schwab/utils.py` & `schwab-py-0.0.0a7/schwab/utils.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/schwab_py.egg-info/PKG-INFO` & `schwab-py-0.0.0a7/schwab_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: Unofficial API wrapper for the upcoming Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-api
```

### Comparing `schwab-py-0.0.0a6/schwab_py.egg-info/SOURCES.txt` & `schwab-py-0.0.0a7/schwab_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/setup.cfg` & `schwab-py-0.0.0a7/setup.cfg`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a6/setup.py` & `schwab-py-0.0.0a7/setup.py`

 * *Files identical despite different names*

