# Comparing `tmp/pyrb-0.9.6.tar.gz` & `tmp/pyrb-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrb-0.9.6.tar", max compression
+gzip compressed data, was "pyrb-0.9.7.tar", max compression
```

## Comparing `pyrb-0.9.6.tar` & `pyrb-0.9.7.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1066 2024-03-17 15:29:43.880106 pyrb-0.9.6/LICENSE
--rw-r--r--   0        0        0     5291 2024-03-17 15:29:43.880106 pyrb-0.9.6/README.md
--rw-r--r--   0        0        0     2424 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/__init__.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/controllers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/controllers/api/__init__.py
--rw-r--r--   0        0        0     1162 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/controllers/api/deps.py
--rw-r--r--   0        0        0     3724 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/controllers/api/main.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/controllers/cli/__init__.py
--rw-r--r--   0        0        0     1068 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/controllers/cli/account.py
--rw-r--r--   0        0        0     8075 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/controllers/cli/main.py
--rw-r--r--   0        0        0      206 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/controllers/constants.py
--rw-r--r--   0        0        0      852 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/enums.py
--rw-r--r--   0        0        0      574 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/models/__init__.py
--rw-r--r--   0        0        0      819 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/models/account.py
--rw-r--r--   0        0        0      498 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/models/order.py
--rw-r--r--   0        0        0     1145 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/models/position.py
--rw-r--r--   0        0        0       95 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/models/price.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/repositories/__init__.py
--rw-r--r--   0        0        0     1210 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/repositories/account.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/repositories/brokerages/__init__.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/repositories/brokerages/base/__init__.py
--rw-r--r--   0        0        0      209 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/repositories/brokerages/base/client.py
--rw-r--r--   0        0        0      758 2024-03-17 15:29:43.880106 pyrb-0.9.6/pyrb/repositories/brokerages/base/fetcher.py
--rw-r--r--   0        0        0      551 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/base/order_manager.py
--rw-r--r--   0        0        0     2171 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/base/portfolio.py
--rw-r--r--   0        0        0     1412 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/context.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/ebest/__init__.py
--rw-r--r--   0        0        0     2230 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/ebest/client.py
--rw-r--r--   0        0        0     1210 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/ebest/fetcher.py
--rw-r--r--   0        0        0     1760 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/ebest/order_manager.py
--rw-r--r--   0        0        0     3540 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/ebest/portfolio.py
--rw-r--r--   0        0        0     2153 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/repositories/brokerages/factory.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/services/__init__.py
--rw-r--r--   0        0        0      384 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/services/account.py
--rw-r--r--   0        0        0     4527 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/services/rebalance.py
--rw-r--r--   0        0        0        0 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/services/strategy/__init__.py
--rw-r--r--   0        0        0     1157 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/services/strategy/asset_allocate.py
--rw-r--r--   0        0        0      273 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/services/strategy/base.py
--rw-r--r--   0        0        0     4267 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/services/strategy/explicit_target.py
--rw-r--r--   0        0        0      655 2024-03-17 15:29:43.884106 pyrb-0.9.6/pyrb/services/strategy/holding_portfolio.py
--rw-r--r--   0        0        0     6179 1970-01-01 00:00:00.000000 pyrb-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-31 13:24:38.370109 pyrb-0.9.7/LICENSE
+-rw-r--r--   0        0        0     5291 2024-03-31 13:24:38.370109 pyrb-0.9.7/README.md
+-rw-r--r--   0        0        0     2424 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/controllers/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/controllers/api/__init__.py
+-rw-r--r--   0        0        0     1162 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/controllers/api/deps.py
+-rw-r--r--   0        0        0     4431 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/controllers/api/main.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/controllers/cli/__init__.py
+-rw-r--r--   0        0        0     1068 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/controllers/cli/account.py
+-rw-r--r--   0        0        0     8075 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/controllers/cli/main.py
+-rw-r--r--   0        0        0      206 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/controllers/constants.py
+-rw-r--r--   0        0        0      852 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/enums.py
+-rw-r--r--   0        0        0      574 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/models/__init__.py
+-rw-r--r--   0        0        0      819 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/models/account.py
+-rw-r--r--   0        0        0      498 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/models/order.py
+-rw-r--r--   0        0        0      134 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/models/portfolio.py
+-rw-r--r--   0        0        0     1176 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/models/position.py
+-rw-r--r--   0        0        0       95 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/models/price.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/repositories/__init__.py
+-rw-r--r--   0        0        0     1210 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/repositories/account.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/repositories/brokerages/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.370109 pyrb-0.9.7/pyrb/repositories/brokerages/base/__init__.py
+-rw-r--r--   0        0        0      209 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/base/client.py
+-rw-r--r--   0        0        0      758 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/base/fetcher.py
+-rw-r--r--   0        0        0      551 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/base/order_manager.py
+-rw-r--r--   0        0        0     2706 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/base/portfolio.py
+-rw-r--r--   0        0        0     1412 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/context.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/ebest/__init__.py
+-rw-r--r--   0        0        0     2230 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/ebest/client.py
+-rw-r--r--   0        0        0     1210 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/ebest/fetcher.py
+-rw-r--r--   0        0        0     1760 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/ebest/order_manager.py
+-rw-r--r--   0        0        0     4919 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/ebest/portfolio.py
+-rw-r--r--   0        0        0     2153 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/repositories/brokerages/factory.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/services/__init__.py
+-rw-r--r--   0        0        0      384 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/services/account.py
+-rw-r--r--   0        0        0     4527 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/services/rebalance.py
+-rw-r--r--   0        0        0        0 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/services/strategy/__init__.py
+-rw-r--r--   0        0        0     1157 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/services/strategy/asset_allocate.py
+-rw-r--r--   0        0        0      273 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/services/strategy/base.py
+-rw-r--r--   0        0        0     4267 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/services/strategy/explicit_target.py
+-rw-r--r--   0        0        0      655 2024-03-31 13:24:38.374109 pyrb-0.9.7/pyrb/services/strategy/holding_portfolio.py
+-rw-r--r--   0        0        0     6179 1970-01-01 00:00:00.000000 pyrb-0.9.7/PKG-INFO
```

### Comparing `pyrb-0.9.6/LICENSE` & `pyrb-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/README.md` & `pyrb-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyproject.toml` & `pyrb-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrb"
-version = "0.9.6"
+version = "0.9.7"
 description = "Python Rebalancer"
 authors = ["Minki Kim <mingi3314@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 pyrb = "pyrb.controllers.cli.main:app"
```

### Comparing `pyrb-0.9.6/pyrb/controllers/api/deps.py` & `pyrb-0.9.7/pyrb/controllers/api/deps.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/controllers/api/main.py` & `pyrb-0.9.7/pyrb/controllers/api/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
 from uuid import UUID
 from zoneinfo import ZoneInfo
 
-from fastapi import FastAPI, HTTPException
+from fastapi import FastAPI, HTTPException, Query
 from fastapi.middleware.cors import CORSMiddleware
 from pydantic import AwareDatetime, BaseModel
 from starlette.status import HTTP_201_CREATED
 
 from pyrb.controllers.api.deps import AccountServiceDep, RebalanceContextDep
 from pyrb.enums import AssetAllocationStrategyEnum, BrokerageType
 from pyrb.exceptions import InitializationError
 from pyrb.models.account import Account, AccountFactory
 from pyrb.models.order import Order, OrderPlacementResult
+from pyrb.models.portfolio import PortfolioReturn
 from pyrb.models.position import Position
 from pyrb.services.rebalance import Rebalancer
 from pyrb.services.strategy.asset_allocate import AssetAllocationStrategyFactory
 
 app = FastAPI()
 
 app.add_middleware(
@@ -48,14 +49,20 @@
 
 class PortfolioResponse(BaseModel):
     total_value: float
     cash_balance: float
     positions: list[Position]
 
 
+class PortfolioReturnsResponse(BaseModel):
+    start_dt: AwareDatetime
+    end_dt: AwareDatetime
+    returns: list[PortfolioReturn]
+
+
 class OrdersPrepareResponse(BaseModel):
     orders: list[Order]
 
 
 class OrdersPlaceRequest(BaseModel):
     orders: list[Order]
 
@@ -94,14 +101,31 @@
     return PortfolioResponse(
         total_value=portfolio.total_value,
         cash_balance=portfolio.cash_balance,
         positions=portfolio.positions,
     )
 
 
+@app.get("/portfolio/returns", response_model=PortfolioReturnsResponse)
+async def fetch_portfolio_returns(
+    context: RebalanceContextDep,
+    start_dt: AwareDatetime = Query(),
+    end_dt: AwareDatetime = Query(
+        default_factory=lambda: datetime.datetime.now(ZoneInfo("Asia/Seoul"))
+    ),
+) -> PortfolioReturnsResponse:
+    returns = context.portfolio.fetch_returns(start_dt, end_dt)
+
+    return PortfolioReturnsResponse(
+        start_dt=start_dt,
+        end_dt=end_dt,
+        returns=returns,
+    )
+
+
 @app.get("/strategies/{strategy_type}/orders", response_model=OrdersPrepareResponse)
 async def prepare_orders(
     context: RebalanceContextDep,
     strategy_type: AssetAllocationStrategyEnum,
 ) -> OrdersPrepareResponse:
     strategy = AssetAllocationStrategyFactory.create(strategy_type)
     rebalancer = Rebalancer(context)
```

### Comparing `pyrb-0.9.6/pyrb/controllers/cli/account.py` & `pyrb-0.9.7/pyrb/controllers/cli/account.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/controllers/cli/main.py` & `pyrb-0.9.7/pyrb/controllers/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/enums.py` & `pyrb-0.9.7/pyrb/enums.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/exceptions.py` & `pyrb-0.9.7/pyrb/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/models/account.py` & `pyrb-0.9.7/pyrb/models/account.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/models/position.py` & `pyrb-0.9.7/pyrb/models/position.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 class Position(BaseModel):
     asset: Asset  # 종목코드
     quantity: PositiveInt  # 보유수량
     sellable_quantity: PositiveInt  # 매도가능수량
     average_buy_price: PositiveFloat  # 매입단가
     total_amount: PositiveFloat  # 평가금액
     rtn: float  # 수익률
+    profit: float  # 수익금
```

### Comparing `pyrb-0.9.6/pyrb/repositories/account.py` & `pyrb-0.9.7/pyrb/repositories/account.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/base/fetcher.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/base/fetcher.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/base/order_manager.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/base/order_manager.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/base/portfolio.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/base/portfolio.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 
-from pydantic import NonNegativeFloat
+from pydantic import AwareDatetime, NonNegativeFloat
 
+from pyrb.models.portfolio import PortfolioReturn
 from pyrb.models.position import Position
 
 
 class Portfolio(abc.ABC):
     @property
     @abc.abstractmethod
     def total_value(self) -> NonNegativeFloat:
@@ -70,10 +71,25 @@
 
         Returns:
             NonNegativeFloat: The total amount of the position for the given symbol.
         """
         ...
 
     @abc.abstractmethod
+    def fetch_returns(
+        self, start_dt: AwareDatetime, end_dt: AwareDatetime
+    ) -> list[PortfolioReturn]:
+        """Fetches the returns of the portfolio for the given period.
+
+        Args:
+            start_dt (AwareDatetime): The start date of the period.
+            end_dt (AwareDatetime): The end date of the period.
+
+        Returns:
+            list[PortfolioReturn]: A list of PortfolioReturn objects.
+        """
+        ...
+
+    @abc.abstractmethod
     def refresh(self) -> None:
         """Refreshes the portfolio object."""
         ...
```

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/context.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/context.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/ebest/client.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/ebest/client.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/ebest/fetcher.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/ebest/fetcher.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/ebest/order_manager.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/ebest/order_manager.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/ebest/portfolio.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/ebest/portfolio.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,97 @@
+import datetime
 from typing import Any
+from zoneinfo import ZoneInfo
 
-from pydantic import NonNegativeFloat
+from pydantic import AwareDatetime, NonNegativeFloat
 
+from pyrb.models.portfolio import PortfolioReturn
 from pyrb.models.position import Asset, Position
 from pyrb.repositories.brokerages.base.portfolio import Portfolio
 from pyrb.repositories.brokerages.ebest.client import EbestAPIClient
 
 
 class EbestPortfolio(Portfolio):
     def __init__(self, api_client: EbestAPIClient) -> None:
         self._api_client = api_client
-        self._serialized_portfolio: dict[str, Any] = self._fetch_portfolio()
+        self._serialized_portfolio: dict[str, Any] | None = None
 
     @property
     def total_value(self) -> NonNegativeFloat:
-        return self._serialized_portfolio["t0424OutBlock"]["sunamt"]
+        return self.serialized_portfolio["t0424OutBlock"]["sunamt"]
 
     @property
     def cash_balance(self) -> NonNegativeFloat:
-        return self._serialized_portfolio["CSPAQ12200OutBlock2"]["D2Dps"]
+        return self.serialized_portfolio["CSPAQ12200OutBlock2"]["D2Dps"]
 
     @property
     def positions(self) -> list[Position]:
         positions = [
             Position(
                 asset=Asset(symbol=item["expcode"], label=item["hname"]),
                 quantity=item["janqty"],
                 sellable_quantity=item["mdposqt"],
                 average_buy_price=item["pamt"],
                 total_amount=item["appamt"],
                 rtn=float(item["sunikrt"]) / 100,
+                profit=item["dtsunik"],
             )
-            for item in self._serialized_portfolio["t0424OutBlock1"]
+            for item in self.serialized_portfolio["t0424OutBlock1"]
         ]
 
         return positions
 
     @property
     def holding_symbols(self) -> list[str]:
         return [position.asset.symbol for position in self.positions]
 
+    @property
+    def serialized_portfolio(self) -> dict[str, Any]:
+        if self._serialized_portfolio is None:
+            self._serialized_portfolio = self._fetch_portfolio()
+        return self._serialized_portfolio
+
     def get_position(self, symbol: str) -> Position | None:
         return next(
             (position for position in self.positions if position.asset.symbol == symbol), None
         )
 
     def get_position_amount(self, symbol: str) -> NonNegativeFloat:
         position = self.get_position(symbol)
         return position.total_amount if position else 0
 
+    def fetch_returns(
+        self, start_date: AwareDatetime, end_date: AwareDatetime
+    ) -> list[PortfolioReturn]:
+        path = "stock/accno"
+        content_type = "application/json; charset=UTF-8"
+
+        headers = {"content-type": content_type, "tr_cd": "FOCCQ33600", "tr_cont": "N"}
+
+        body = {
+            "FOCCQ33600InBlock1": {
+                "QrySrtDt": start_date.strftime("%Y%m%d"),
+                "QryEndDt": end_date.strftime("%Y%m%d"),
+                "TermTp": "1",
+            }
+        }
+
+        response = self._api_client.send_request("POST", path, headers=headers, json=body)
+        print(response.json())
+        return [
+            PortfolioReturn(
+                dt=datetime.datetime.strptime(each["BaseDt"], "%Y%m%d").replace(
+                    tzinfo=ZoneInfo("Asia/Seoul")
+                ),
+                rtn=float(each["TermErnrat"]) / 100,
+                pnl=each["EvalPnlAmt"],
+            )
+            for each in response.json()["FOCCQ33600OutBlock3"]
+        ]
+
     def refresh(self) -> None:
         self._serialized_portfolio = self._fetch_portfolio()
 
     def _fetch_portfolio(self) -> dict[str, Any]:
         asset_balance = self._fetch_assets_balance()
         cash_balance = self._fetch_cash_balance()
         return asset_balance | cash_balance
```

### Comparing `pyrb-0.9.6/pyrb/repositories/brokerages/factory.py` & `pyrb-0.9.7/pyrb/repositories/brokerages/factory.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/services/rebalance.py` & `pyrb-0.9.7/pyrb/services/rebalance.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/services/strategy/asset_allocate.py` & `pyrb-0.9.7/pyrb/services/strategy/asset_allocate.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/services/strategy/explicit_target.py` & `pyrb-0.9.7/pyrb/services/strategy/explicit_target.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/pyrb/services/strategy/holding_portfolio.py` & `pyrb-0.9.7/pyrb/services/strategy/holding_portfolio.py`

 * *Files identical despite different names*

### Comparing `pyrb-0.9.6/PKG-INFO` & `pyrb-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrb
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python Rebalancer
 Author: Minki Kim
 Author-email: mingi3314@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

