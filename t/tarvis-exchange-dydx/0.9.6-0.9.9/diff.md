# Comparing `tmp/tarvis-exchange-dydx-0.9.6.tar.gz` & `tmp/tarvis-exchange-dydx-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-exchange-dydx-0.9.6.tar", last modified: Sun May 14 09:26:30 2023, max compression
+gzip compressed data, was "tarvis-exchange-dydx-0.9.9.tar", last modified: Thu Jul  6 22:36:07 2023, max compression
```

## Comparing `tarvis-exchange-dydx-0.9.6.tar` & `tarvis-exchange-dydx-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.501865 tarvis-exchange-dydx-0.9.6/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:26:30.501865 tarvis-exchange-dydx-0.9.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      769 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/tarvis/exchange/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/tarvis/exchange/dydx/
--rw-r--r--   0 root         (0) root         (0)     9045 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/tarvis/exchange/dydx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:26:30.000000 tarvis-exchange-dydx-0.9.6/tarvis_exchange_dydx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:26:30.497864 tarvis-exchange-dydx-0.9.6/test/
--rw-r--r--   0 root         (0) root         (0)    12356 2023-05-14 09:26:19.000000 tarvis-exchange-dydx-0.9.6/test/test_exchange_dydx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:36:07.559480 tarvis-exchange-dydx-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-06 22:35:58.000000 tarvis-exchange-dydx-0.9.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-06 22:36:07.559480 tarvis-exchange-dydx-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       35 2023-07-06 22:35:58.000000 tarvis-exchange-dydx-0.9.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 22:36:07.559480 tarvis-exchange-dydx-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-06 22:35:58.000000 tarvis-exchange-dydx-0.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:36:07.555479 tarvis-exchange-dydx-0.9.9/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:36:07.555479 tarvis-exchange-dydx-0.9.9/tarvis/exchange/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:36:07.559480 tarvis-exchange-dydx-0.9.9/tarvis/exchange/dydx/
+-rw-r--r--   0 root         (0) root         (0)    11877 2023-07-06 22:35:58.000000 tarvis-exchange-dydx-0.9.9/tarvis/exchange/dydx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:36:07.559480 tarvis-exchange-dydx-0.9.9/tarvis_exchange_dydx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-06 22:36:07.000000 tarvis-exchange-dydx-0.9.9/tarvis_exchange_dydx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      309 2023-07-06 22:36:07.000000 tarvis-exchange-dydx-0.9.9/tarvis_exchange_dydx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 22:36:07.000000 tarvis-exchange-dydx-0.9.9/tarvis_exchange_dydx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-06 22:36:07.000000 tarvis-exchange-dydx-0.9.9/tarvis_exchange_dydx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 22:36:07.000000 tarvis-exchange-dydx-0.9.9/tarvis_exchange_dydx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:36:07.559480 tarvis-exchange-dydx-0.9.9/test/
+-rw-r--r--   0 root         (0) root         (0)    12632 2023-07-06 22:35:58.000000 tarvis-exchange-dydx-0.9.9/test/test_exchange_dydx.py
```

### Comparing `tarvis-exchange-dydx-0.9.6/LICENSE.txt` & `tarvis-exchange-dydx-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-dydx-0.9.6/setup.py` & `tarvis-exchange-dydx-0.9.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-exchange-dydx",
-    version="0.9.6",
+    version="0.9.9",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Exchange Library for dYdX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-exchange-dydx-0.9.6/tarvis/exchange/dydx/__init__.py` & `tarvis-exchange-dydx-0.9.9/tarvis/exchange/dydx/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,43 @@
 from decimal import Decimal
-from dydx3 import Client
+from dydx3 import Client, DydxApiError
 from dydx3.constants import (
     API_HOST_GOERLI,
     API_HOST_MAINNET,
     NETWORK_ID_GOERLI,
     NETWORK_ID_MAINNET,
     TIME_IN_FORCE_GTT,
     TIME_IN_FORCE_IOC,
 )
+import dydx3.helpers.requests
+from dydx3.helpers.requests import Response as DYDXResponse
+from requests import Response, Session
+from requests.status_codes import codes
 from tarvis.common import secrets, time
 import tarvis.common.environ
 from tarvis.common.environ import DeploymentType
 from tarvis.common.time import datetime
 from tarvis.common.trading import Exchange, Order, OrderSide, OrderType, TradingPolicy
+import time as native_time
+
+
+class ResponseDecimal(Response):
+    def json(self, **kwargs):
+        return super().json(parse_float=Decimal, **kwargs)
+
+
+class SessionDecimal(Session):
+    def send(self, request, **kwargs):
+        r = super().send(request, **kwargs)
+        r.__class__ = ResponseDecimal
+        return r
+
+
+# Monkeypatch library to parse decimals correctly
+dydx3.helpers.requests.session.__class__ = SessionDecimal
 
 
 class DYDXExchange(Exchange):
     EXCHANGE_NAME = "dYdX"
 
     _ORDER_TYPE_TO_DYDX = {
         OrderType.MARKET: "MARKET",
@@ -66,102 +87,151 @@
                 "passphrase": api_passphrase,
             },
             stark_private_key=stark_private_key,
         )
 
         self._position_id = self._get_position_id()
 
+    @staticmethod
+    def _retry_rate_limited_call(_call_method, *args, **kwargs) -> DYDXResponse:
+        try:
+            response = _call_method(*args, **kwargs)
+        except DydxApiError as dydx_exception:
+            if dydx_exception.status_code == codes.too_many_requests:
+                delay = dydx_exception.response.headers.get("Retry-After", 0)
+                native_time.sleep(float(delay) / 1000)
+                response = _call_method(*args, **kwargs)
+            else:
+                raise
+        return response
+
     def _get_position_id(self):
-        response = self._client.private.get_account()
+        response = self._retry_rate_limited_call(self._client.private.get_account)
         return response.data["account"]["positionId"]
 
     @staticmethod
-    def _convert_market_to_assets(market: str) -> (str, str):
-        base_asset, quote_asset = market.split("-")
+    def _convert_symbol_to_assets(symbol: str) -> (str, str):
+        base_asset, quote_asset = symbol.split("-")
         return base_asset, quote_asset
 
     @staticmethod
-    def _convert_assets_to_market(base_asset: str, quote_asset: str) -> str:
+    def _convert_assets_to_symbol(base_asset: str, quote_asset: str) -> str:
         return "-".join((base_asset, quote_asset))
 
-    def get_policy(self, base_asset: str, quote_asset: str) -> TradingPolicy:
-        market = self._convert_assets_to_market(base_asset, quote_asset)
-        response = self._client.public.get_markets(market)
-        market_data = response.data["markets"][market]
-
-        minimum_order_quantity = Decimal(market_data["minOrderSize"])
-        maximum_order_quantity = Decimal(market_data["maxPositionSize"])
-        quantity_precision = Decimal(market_data["stepSize"])
-        price_precision = Decimal(market_data["tickSize"])
+    @staticmethod
+    def _create_policy(instrument_data: dict) -> TradingPolicy:
+        minimum_order_quantity = Decimal(instrument_data["minOrderSize"])
+        maximum_order_quantity = Decimal(instrument_data["maxPositionSize"])
+        quantity_precision = Decimal(instrument_data["stepSize"])
+        price_precision = Decimal(instrument_data["tickSize"])
 
         return TradingPolicy(
             minimum_order_quantity=minimum_order_quantity,
             maximum_order_quantity=maximum_order_quantity,
             quantity_precision=quantity_precision,
             price_precision=price_precision,
         )
 
+    def get_policy(self, base_asset: str, quote_asset: str) -> TradingPolicy:
+        symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
+        response = self._retry_rate_limited_call(
+            self._client.public.get_markets, market=symbol
+        )
+        instrument_data = response.data["markets"][symbol]
+        return self._create_policy(instrument_data)
+
+    def get_policies(
+        self, asset_pairs: list[tuple[str, str]]
+    ) -> dict[tuple[str, str], TradingPolicy]:
+        response = self._retry_rate_limited_call(self._client.public.get_markets)
+        instruments = response.data["markets"]
+        policies = {}
+        for asset_pair in asset_pairs:
+            base_asset, quote_asset = asset_pair
+            symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
+            instrument_data = instruments[symbol]
+            policies[asset_pair] = self._create_policy(instrument_data)
+        return policies
+
     def get_quote(self, base_asset: str, quote_asset: str) -> Decimal:
-        market = self._convert_assets_to_market(base_asset, quote_asset)
-        response = self._client.public.get_markets(market)
-        market_data = response.data["markets"][market]
-        price = market_data["indexPrice"]
+        symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
+        response = self._retry_rate_limited_call(
+            self._client.public.get_markets, market=symbol
+        )
+        instrument_data = response.data["markets"][symbol]
+        price = instrument_data["indexPrice"]
         return Decimal(price)
 
+    def get_quotes(
+        self, asset_pairs: list[tuple[str, str]]
+    ) -> dict[tuple[str, str], Decimal]:
+        response = self._retry_rate_limited_call(self._client.public.get_markets)
+        instruments = response.data["markets"]
+        quotes = {}
+        for asset_pair in asset_pairs:
+            base_asset, quote_asset = asset_pair
+            symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
+            market_data = instruments[symbol]
+            price = market_data["indexPrice"]
+            quotes[asset_pair] = Decimal(price)
+        return quotes
+
     def get_positions(self) -> dict[str, Decimal]:
         results = {}
-        response = self._client.private.get_account()
+        response = self._retry_rate_limited_call(self._client.private.get_account)
         positions = response.data["account"]["openPositions"]
 
         # Only one open position possible for each market in dYdX
         for key, position in positions.items():
-            market = position["market"]
+            symbol = position["market"]
             size = position["size"]
 
-            base_asset, quote_asset = self._convert_market_to_assets(market)
+            base_asset, _ = self._convert_symbol_to_assets(symbol)
             size = Decimal(size)
 
-            results[base_asset] = size
+            if size != 0:
+                results[base_asset] = size
 
         results["USD"] = Decimal(response.data["account"]["quoteBalance"])
 
         return results
 
     def get_open_orders(self, base_asset: str, quote_asset: str) -> list[Order]:
         _PAGE_SIZE = 100
 
         results = {}
-        market = self._convert_assets_to_market(base_asset, quote_asset)
+        symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
         page_order_count = _PAGE_SIZE
         start_datetime = None
         while page_order_count == _PAGE_SIZE:
-            response = self._client.private.get_orders(
-                market=market,
+            response = self._retry_rate_limited_call(
+                self._client.private.get_orders,
+                market=symbol,
                 status="PENDING,OPEN,UNTRIGGERED",
                 limit=_PAGE_SIZE,
                 created_before_or_at=start_datetime,
             )
 
             dydx_orders = response.data["orders"]
             page_order_count = len(dydx_orders)
 
             for dydx_order in dydx_orders:
                 order_id = dydx_order["id"]
-                market = dydx_order["market"]
+                symbol = dydx_order["market"]
                 quantity = dydx_order["size"]
                 side = dydx_order["side"]
                 order_type = dydx_order["type"]
                 if order_type == "STOP_MARKET":
                     price = dydx_order["triggerPrice"]
                 else:
                     price = dydx_order["price"]
                 created_at = dydx_order["createdAt"]
                 remaining_quantity = dydx_order["remainingSize"]
 
-                quote_asset, base_asset = self._convert_market_to_assets(market)
+                base_asset, quote_asset = self._convert_symbol_to_assets(symbol)
                 quantity = Decimal(quantity)
                 side = OrderSide[side]
                 # noinspection PyBroadException
                 try:
                     order_type = self._ORDER_TYPE_TO_TARVIS[order_type]
                 except:
                     order_type = OrderType.UNSUPPORTED
@@ -169,16 +239,16 @@
                 creation_time = creation_date.timestamp()
                 filled_quantity = quantity - Decimal(remaining_quantity)
                 meta_data = {"order_id": order_id}
 
                 start_datetime = created_at
 
                 order = Order(
-                    quote_asset,
                     base_asset,
+                    quote_asset,
                     side,
                     order_type,
                     creation_time,
                     quantity=quantity,
                     price=price,
                     filled_quantity=filled_quantity,
                     meta_data=meta_data,
@@ -196,15 +266,15 @@
         side: OrderSide,
         order_type: OrderType,
         quantity: Decimal,
         price: Decimal = None,
         stop_loss_price: Decimal = None,
         increasing_position: bool = None,
     ):
-        market = self._convert_assets_to_market(base_asset, quote_asset)
+        symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
         dydx_order_type = self._ORDER_TYPE_TO_DYDX[order_type]
         expiration = int(time.time() + self._order_expiration)
 
         if order_type == OrderType.STOP_LOSS:
             if stop_loss_price is None:
                 raise ValueError("stop_loss_price is None.")
             if price is None:
@@ -230,24 +300,27 @@
 
         # GTT (Good 'Til Date/Time) is not allowed for reduce and market orders
         if reduce_only or (order_type != OrderType.LIMIT):
             time_in_force = TIME_IN_FORCE_IOC
         else:
             time_in_force = TIME_IN_FORCE_GTT
 
-        self._client.private.create_order(
+        self._retry_rate_limited_call(
+            self._client.private.create_order,
             position_id=self._position_id,
-            market=market,
+            market=symbol,
             side=side.name,
             order_type=dydx_order_type,
             post_only=False,
             size=str(quantity),
             price=str(price),
             limit_fee=str(self._limit_fee),
             trigger_price=trigger_price,
             time_in_force=time_in_force,
             expiration_epoch_seconds=expiration,
             reduce_only=reduce_only,
         )
 
     def cancel_order(self, order: Order):
-        self._client.private.cancel_order(order.meta_data["order_id"])
+        self._retry_rate_limited_call(
+            self._client.private.cancel_order, order_id=order.meta_data["order_id"]
+        )
```

### Comparing `tarvis-exchange-dydx-0.9.6/test/test_exchange_dydx.py` & `tarvis-exchange-dydx-0.9.9/test/test_exchange_dydx.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.BUY,
         OrderType.MARKET,
         order_quantity,
         price=order_price,
+        increasing_position=True,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
     orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
@@ -108,14 +109,15 @@
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.SELL,
         OrderType.STOP_LOSS,
         order_quantity,
         stop_loss_price=stop_loss_price,
+        increasing_position=False,
     )
 
     end_time = time.time()
 
     orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
@@ -150,14 +152,15 @@
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.BUY,
         OrderType.LIMIT,
         order_quantity,
         price=order_price,
+        increasing_position=True,
     )
 
     end_time = time.time()
 
     orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
@@ -195,14 +198,15 @@
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.SELL,
         OrderType.MARKET,
         order_quantity,
         price=order_price,
+        increasing_position=False,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
     positions = exchange.get_positions()
     base_position_end = positions.get(_BASE_ASSET, 0)
     quote_position_end = positions.get(_QUOTE_ASSET, 0)
@@ -232,14 +236,15 @@
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.SELL,
         OrderType.MARKET,
         order_quantity,
         price=order_price,
+        increasing_position=True,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
     orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 0
 
@@ -272,14 +277,15 @@
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.BUY,
         OrderType.STOP_LOSS,
         order_quantity,
         stop_loss_price=stop_loss_price,
+        increasing_position=False,
     )
 
     end_time = time.time()
 
     orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
@@ -314,14 +320,15 @@
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.SELL,
         OrderType.LIMIT,
         order_quantity,
         price=order_price,
+        increasing_position=True,
     )
 
     end_time = time.time()
 
     orders = exchange.get_open_orders(_BASE_ASSET, _QUOTE_ASSET)
     assert len(orders) == 1
 
@@ -358,14 +365,15 @@
         trading_policy,
         _BASE_ASSET,
         _QUOTE_ASSET,
         OrderSide.BUY,
         OrderType.MARKET,
         order_quantity,
         price=order_price,
+        increasing_position=False,
     )
 
     time.sleep(_SETTLEMENT_DELAY)
 
     positions = exchange.get_positions()
     base_position_end = positions.get(_BASE_ASSET, 0)
     quote_position_end = positions.get(_QUOTE_ASSET, 0)
```

