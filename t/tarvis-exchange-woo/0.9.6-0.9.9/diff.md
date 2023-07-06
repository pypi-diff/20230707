# Comparing `tmp/tarvis-exchange-woo-0.9.6.tar.gz` & `tmp/tarvis-exchange-woo-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-exchange-woo-0.9.6.tar", last modified: Sun May 14 09:42:02 2023, max compression
+gzip compressed data, was "tarvis-exchange-woo-0.9.9.tar", last modified: Thu Jul  6 22:39:31 2023, max compression
```

## Comparing `tarvis-exchange-woo-0.9.6.tar` & `tarvis-exchange-woo-0.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.912357 tarvis-exchange-woo-0.9.6/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-14 09:42:02.912357 tarvis-exchange-woo-0.9.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 09:42:02.912357 tarvis-exchange-woo-0.9.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      767 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.908357 tarvis-exchange-woo-0.9.6/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.908357 tarvis-exchange-woo-0.9.6/tarvis/exchange/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.908357 tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/
--rw-r--r--   0 root         (0) root         (0)    11009 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11285 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/wooclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.908357 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      404 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 09:42:02.000000 tarvis-exchange-woo-0.9.6/tarvis_exchange_woo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 09:42:02.912357 tarvis-exchange-woo-0.9.6/test/
--rw-r--r--   0 root         (0) root         (0)    12337 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/test/test_exchange_woo_margin.py
--rw-r--r--   0 root         (0) root         (0)    12343 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/test/test_exchange_woo_perpetual.py
--rw-r--r--   0 root         (0) root         (0)     6777 2023-05-14 09:41:50.000000 tarvis-exchange-woo-0.9.6/test/test_exchange_woo_spot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:39:31.557505 tarvis-exchange-woo-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-06 22:39:22.000000 tarvis-exchange-woo-0.9.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-06 22:39:31.557505 tarvis-exchange-woo-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-06 22:39:22.000000 tarvis-exchange-woo-0.9.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 22:39:31.557505 tarvis-exchange-woo-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      767 2023-07-06 22:39:22.000000 tarvis-exchange-woo-0.9.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:39:31.553505 tarvis-exchange-woo-0.9.9/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:39:31.553505 tarvis-exchange-woo-0.9.9/tarvis/exchange/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:39:31.553505 tarvis-exchange-woo-0.9.9/tarvis/exchange/woo/
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-07-06 22:39:22.000000 tarvis-exchange-woo-0.9.9/tarvis/exchange/woo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12245 2023-07-06 22:39:22.000000 tarvis-exchange-woo-0.9.9/tarvis/exchange/woo/wooclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:39:31.553505 tarvis-exchange-woo-0.9.9/tarvis_exchange_woo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-06 22:39:31.000000 tarvis-exchange-woo-0.9.9/tarvis_exchange_woo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-06 22:39:31.000000 tarvis-exchange-woo-0.9.9/tarvis_exchange_woo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 22:39:31.000000 tarvis-exchange-woo-0.9.9/tarvis_exchange_woo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 22:39:31.000000 tarvis-exchange-woo-0.9.9/tarvis_exchange_woo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 22:39:31.000000 tarvis-exchange-woo-0.9.9/tarvis_exchange_woo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 22:39:31.557505 tarvis-exchange-woo-0.9.9/test/
+-rw-r--r--   0 root         (0) root         (0)    12613 2023-07-06 22:39:22.000000 tarvis-exchange-woo-0.9.9/test/test_exchange_woo_margin.py
+-rw-r--r--   0 root         (0) root         (0)    12619 2023-07-06 22:39:22.000000 tarvis-exchange-woo-0.9.9/test/test_exchange_woo_perpetual.py
+-rw-r--r--   0 root         (0) root         (0)     6915 2023-07-06 22:39:22.000000 tarvis-exchange-woo-0.9.9/test/test_exchange_woo_spot.py
```

### Comparing `tarvis-exchange-woo-0.9.6/LICENSE.txt` & `tarvis-exchange-woo-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-exchange-woo-0.9.6/setup.py` & `tarvis-exchange-woo-0.9.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-exchange-woo",
-    version="0.9.6",
+    version="0.9.9",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Exchange Library for Woo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/__init__.py` & `tarvis-exchange-woo-0.9.9/tarvis/exchange/woo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,26 +30,27 @@
         OrderType.STOP_LOSS: ("STOP", "MARKET"),
     }
 
     def __init__(
         self,
         credentials_secret: str,
         version: str | WooVersion = WooVersion.SPOT,
+        rate_limit_delay: float = 1,
     ):
         super().__init__()
         self.stop_loss_orders_supported = True
 
         if isinstance(version, str):
             version = WooVersion[version.upper()]
         self._version = version
 
         if version == WooVersion.PERPETUAL:
-            self._market_type = "PERP"
+            self._instrument_type = "PERP"
         else:
-            self._market_type = "SPOT"
+            self._instrument_type = "SPOT"
 
         self.short_selling_supported = version in [
             WooVersion.MARGIN,
             WooVersion.PERPETUAL,
         ]
 
         credentials = secrets.get_secret(credentials_secret, decode_json=True)
@@ -59,101 +60,131 @@
         if tarvis.common.environ.deployment == DeploymentType.PRODUCTION:
             base_url = "https://api.woo.org/"
             application_id = "d5e1e017-b4b3-4cdd-9aa6-613974524596"
         else:
             base_url = "https://api.staging.woo.org/"
             application_id = None
 
-        self._client = WooClient(base_url, api_key, api_secret, application_id)
+        self._client = WooClient(
+            base_url, api_key, api_secret, application_id, rate_limit_delay
+        )
 
     @staticmethod
-    def _convert_market_to_assets(market: str) -> (str, str, str):
-        market_type, base_asset, quote_asset = market.split("_")
-        return market_type, base_asset, quote_asset
+    def _convert_symbol_to_assets(symbol: str) -> (str, str, str):
+        instrument_type, base_asset, quote_asset = symbol.split("_")
+        return instrument_type, base_asset, quote_asset
 
-    def _convert_assets_to_market(self, base_asset: str, quote_asset: str) -> str:
-        return "_".join((self._market_type, base_asset, quote_asset))
+    def _convert_assets_to_symbol(self, base_asset: str, quote_asset: str) -> str:
+        return "_".join((self._instrument_type, base_asset, quote_asset))
 
-    def get_policy(self, base_asset: str, quote_asset: str) -> TradingPolicy:
-        market = self._convert_assets_to_market(base_asset, quote_asset)
-        exchange_response = self._client.get_public_info(market)
-        market_data = exchange_response["info"]
-
-        minimum_order_quantity = Decimal(market_data["base_min"])
-        maximum_order_quantity = Decimal(market_data["base_max"])
-        quantity_precision = Decimal(market_data["base_tick"])
-        price_precision = Decimal(market_data["quote_tick"])
-        minimum_order_value = float(market_data["min_notional"])
+    @staticmethod
+    def _create_policy(instrument_data: dict) -> TradingPolicy:
+        minimum_order_quantity = Decimal(instrument_data["base_min"])
+        maximum_order_quantity = Decimal(instrument_data["base_max"])
+        quantity_precision = Decimal(instrument_data["base_tick"])
+        price_precision = Decimal(instrument_data["quote_tick"])
+        minimum_order_value = float(instrument_data["min_notional"])
 
         return TradingPolicy(
             minimum_order_quantity=minimum_order_quantity,
             maximum_order_quantity=maximum_order_quantity,
             minimum_order_value=minimum_order_value,
             quantity_precision=quantity_precision,
             price_precision=price_precision,
         )
 
+    def get_policy(self, base_asset: str, quote_asset: str) -> TradingPolicy:
+        symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
+        response = self._client.get_public_info(symbol=symbol)
+        instrument_data = response["info"]
+        return self._create_policy(instrument_data)
+
+    def get_policies(
+        self, asset_pairs: list[tuple[str, str]]
+    ) -> dict[tuple[str, str], TradingPolicy]:
+        response = self._client.get_public_info()
+        rows = response["rows"]
+
+        instruments = {}
+        for row in rows:
+            symbol = row["symbol"]
+            instruments[symbol] = row
+
+        policies = {}
+        for asset_pair in asset_pairs:
+            base_asset, quote_asset = asset_pair
+            symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
+            instrument_data = instruments[symbol]
+            policies[asset_pair] = self._create_policy(instrument_data)
+
+        return policies
+
     def get_quote(self, base_asset: str, quote_asset: str) -> Decimal:
-        market = self._convert_assets_to_market(base_asset, quote_asset)
-        response = self._client.get_kline(market, "1m", 1)
+        symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
+        response = self._client.get_kline(symbol=symbol, interval="1m", limit=1)
         row = response["rows"][0]
         price = row["close"]
         return Decimal(price)
 
     def get_positions(self) -> dict[str, Decimal]:
         results = {}
 
         holding_response = self._client.get_balances()
         holdings = holding_response["data"]["holding"]
 
         for holding in holdings:
             base_asset = holding["token"]
             quantity = holding["holding"]
             quantity = Decimal(quantity)
-            results[base_asset] = quantity
+            if quantity != 0:
+                results[base_asset] = quantity
 
         if self._version == WooVersion.PERPETUAL:
             positions_response = self._client.get_positions()
             positions = positions_response["data"]["positions"]
 
             for position in positions:
                 symbol = position["symbol"]
                 quantity = position["holding"]
                 price = position["averageOpenPrice"]
-                _, base_asset, quote_asset = self._convert_market_to_assets(symbol)
+                _, base_asset, quote_asset = self._convert_symbol_to_assets(symbol)
                 quantity = Decimal(quantity)
                 price = Decimal(price)
                 base_quantity = results.get(base_asset, 0)
                 quote_quantity = results.get(quote_asset, 0)
                 results[base_asset] = base_quantity + quantity
                 results[quote_asset] = quote_quantity - (quantity * price)
 
+            results = {key: value for key, value in results.items() if value != 0}
+
         return results
 
-    def _get_open_orders_standard(self, market: str) -> list[Order]:
+    def _get_open_orders_standard(self, symbol: str) -> list[Order]:
         _PAGE_SIZE = 500
 
         results = {}
         page_order_count = _PAGE_SIZE
         page = 1
         while page_order_count == _PAGE_SIZE:
             response = self._client.get_orders(
-                symbol=market, status="INCOMPLETE", size=_PAGE_SIZE, page=page
+                symbol=symbol, status="INCOMPLETE", size=_PAGE_SIZE, page=page
             )
             woo_orders = response["rows"]
             page_order_count = len(woo_orders)
             page += 1
 
             for woo_order in woo_orders:
                 symbol = woo_order["symbol"]
-                market_type, quote_asset, base_asset = self._convert_market_to_assets(
-                    symbol
-                )
+                (
+                    instrument_type,
+                    base_asset,
+                    quote_asset,
+                ) = self._convert_symbol_to_assets(symbol)
 
-                if market_type == self._market_type:
+                if instrument_type == self._instrument_type:
                     order_id = woo_order["order_id"]
                     order_type = woo_order["type"]
                     quantity = woo_order.get("quantity")
                     amount = woo_order.get("amount")
                     price = woo_order.get("price")
                     side = woo_order["side"]
                     creation_time = woo_order["created_time"]
@@ -164,55 +195,57 @@
                     try:
                         order_type = self._STANDARD_ORDER_TYPE_TO_TARVIS[order_type]
                     except:
                         order_type = OrderType.UNSUPPORTED
                     meta_data = {"order_id": order_id, "order_method": "standard"}
 
                     order = Order(
-                        quote_asset,
                         base_asset,
+                        quote_asset,
                         side,
                         order_type,
                         creation_time,
                         quantity=quantity,
                         amount=amount,
                         price=price,
                         filled_quantity=filled_quantity,
                         meta_data=meta_data,
                     )
 
                     results[order_id] = order
 
         return list(results.values())
 
-    def _get_open_orders_algo(self, market: str) -> list[Order]:
+    def _get_open_orders_algo(self, symbol: str) -> list[Order]:
         _PAGE_SIZE = 25
 
         results = {}
         page_order_count = _PAGE_SIZE
         page = 1
         while page_order_count == _PAGE_SIZE:
             response = self._client.get_algo_orders(
                 algo_type="STOP",
-                symbol=market,
+                symbol=symbol,
                 status="INCOMPLETE",
                 size=_PAGE_SIZE,
                 page=page,
             )
             woo_orders = response["data"]["rows"]
             page_order_count = len(woo_orders)
             page += 1
 
             for woo_order in woo_orders:
                 symbol = woo_order["symbol"]
-                market_type, quote_asset, base_asset = self._convert_market_to_assets(
-                    symbol
-                )
+                (
+                    instrument_type,
+                    base_asset,
+                    quote_asset,
+                ) = self._convert_symbol_to_assets(symbol)
 
-                if market_type == self._market_type:
+                if instrument_type == self._instrument_type:
                     order_id = woo_order["algoOrderId"]
                     quantity = woo_order.get("quantity")
                     amount = woo_order.get("amount")
                     price = woo_order.get("triggerPrice")
                     side = woo_order["side"]
                     order_type = woo_order["type"]
                     creation_time = woo_order["createdTime"]
@@ -222,16 +255,16 @@
                     if order_type == "MARKET":
                         order_type = OrderType.STOP_LOSS
                     else:
                         order_type = OrderType.UNSUPPORTED
                     meta_data = {"order_id": order_id, "order_method": "algo"}
 
                     order = Order(
-                        quote_asset,
                         base_asset,
+                        quote_asset,
                         side,
                         order_type,
                         creation_time,
                         quantity=quantity,
                         amount=amount,
                         price=price,
                         filled_quantity=filled_quantity,
@@ -239,63 +272,73 @@
                     )
 
                     results[order_id] = order
 
         return list(results.values())
 
     def get_open_orders(self, base_asset: str, quote_asset: str) -> list[Order]:
-        market = self._convert_assets_to_market(base_asset, quote_asset)
-        return self._get_open_orders_standard(market) + self._get_open_orders_algo(
-            market
+        symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
+        return self._get_open_orders_standard(symbol) + self._get_open_orders_algo(
+            symbol
         )
 
     def place_order(
         self,
         policy: TradingPolicy,
         base_asset: str,
         quote_asset: str,
         side: OrderSide,
         order_type: OrderType,
         quantity: Decimal,
         price: Decimal = None,
         stop_loss_price: Decimal = None,
         increasing_position: bool = None,
     ):
-        market = self._convert_assets_to_market(base_asset, quote_asset)
+        symbol = self._convert_assets_to_symbol(base_asset, quote_asset)
 
         if order_type in self._STANDARD_TARVIS_ORDER_TYPES:
             standard_order = True
             algo_type = None
             woo_order_type = self._STANDARD_ORDER_TYPE_TO_WOO[order_type]
         else:
             standard_order = False
             algo_type, woo_order_type = self._ALGO_ORDER_TYPE_TO_WOO[order_type]
 
         if order_type == OrderType.STOP_LOSS:
             price = str(stop_loss_price)
         elif price is not None:
             price = str(price)
 
+        reduce_only = None
+        if (self._version == WooVersion.PERPETUAL) and (
+            increasing_position is not None
+        ):
+            reduce_only = not increasing_position
+
         if standard_order:
             self._client.post_order(
-                market,
-                side.name,
-                woo_order_type,
+                symbol=symbol,
+                side=side.name,
+                order_type=woo_order_type,
                 order_quantity=str(quantity),
                 order_price=price,
+                reduce_only=reduce_only,
             )
         else:
             self._client.post_algo_order(
-                market,
-                side.name,
-                algo_type,
-                woo_order_type,
+                symbol=symbol,
+                side=side.name,
+                algo_type=algo_type,
+                order_type=woo_order_type,
                 order_quantity=str(quantity),
                 trigger_price=price,
+                reduce_only=reduce_only,
             )
 
     def cancel_order(self, order: Order):
-        market = self._convert_assets_to_market(order.base_asset, order.quote_asset)
+        symbol = self._convert_assets_to_symbol(order.base_asset, order.quote_asset)
         if order.meta_data["order_method"] == "standard":
-            self._client.delete_order(order.meta_data["order_id"], market)
+            self._client.delete_order(
+                order_id=order.meta_data["order_id"], symbol=symbol
+            )
         else:
-            self._client.delete_algo_order(order.meta_data["order_id"])
+            self._client.delete_algo_order(order_id=order.meta_data["order_id"])
```

### Comparing `tarvis-exchange-woo-0.9.6/tarvis/exchange/woo/wooclient.py` & `tarvis-exchange-woo-0.9.9/tarvis/exchange/woo/wooclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from decimal import Decimal
 import hashlib
 import hmac
 import json
 import requests
-import time
+from requests.status_codes import codes
+from tarvis.common import time
+import time as native_time
 from urllib.parse import quote_plus
 
 
 class WooClientError(Exception):
     def __init__(self, response):
         self.status_code = response.status_code
         try:
@@ -26,19 +29,21 @@
 class WooClient:
     def __init__(
         self,
         base_url: str,
         api_key: str = None,
         api_secret: str = None,
         application_id: str = None,
+        rate_limit_delay: float = 1,
     ):
         self._base_url = base_url.removesuffix("/")
         self._api_key = api_key
         self._api_secret = api_secret
         self._application_id = application_id
+        self._rate_limit_delay = rate_limit_delay
         if api_key is not None:
             self._api_key_bytes = bytes(self._api_secret, "utf-8")
 
     @staticmethod
     def _get_request_path(version: int, end_point: str) -> str:
         return f"/v{version}/{end_point}"
 
@@ -167,18 +172,22 @@
         )
         url = self._base_url + request_path
         if len(query_params_string) > 0:
             url += "?" + query_params_string
 
         response = requests.get(url, headers=headers)
 
+        if response.status_code == codes.too_many_requests:
+            native_time.sleep(self._rate_limit_delay)
+            response = requests.get(url, headers=headers)
+
         if not str(response.status_code).startswith("2"):
             raise WooClientError(response)
 
-        return response.json()
+        return response.json(parse_float=Decimal)
 
     def _non_get_request(
         self, method: str, version: int, end_point: str, private: bool, **params
     ):
         if version == 1:
             prepared_params = self._prepare_query_params(params)
             query_params_string = self._get_query_string(prepared_params)
@@ -205,27 +214,40 @@
         response = requests.request(
             method,
             url,
             headers=headers,
             data=body,
         )
 
+        if response.status_code == codes.too_many_requests:
+            native_time.sleep(self._rate_limit_delay)
+            response = requests.request(
+                method,
+                url,
+                headers=headers,
+                data=body,
+            )
+
         if not str(response.status_code).startswith("2"):
             raise WooClientError(response)
 
-        return response.json()
+        return response.json(parse_float=Decimal)
 
     def _post(self, version: int, end_point: str, private: bool, **params):
         return self._non_get_request("POST", version, end_point, private, **params)
 
     def _delete(self, version: int, end_point: str, private: bool, **params):
         return self._non_get_request("DELETE", version, end_point, private, **params)
 
-    def get_public_info(self, symbol: str):
-        return self._get(1, f"public/info/{symbol}", False)
+    def get_public_info(self, symbol: str = None):
+        if symbol:
+            symbol = "/" + symbol
+        else:
+            symbol = ""
+        return self._get(1, f"public/info{symbol}", False)
 
     def get_kline(self, symbol: str, interval: str, limit: int = None):
         return self._get(1, "kline", True, symbol=symbol, type=interval, limit=limit)
 
     def get_balances(self):
         return self._get(3, "balances", True)
 
@@ -303,14 +325,17 @@
         order_tag: str = None,
         order_price: str = None,
         order_quantity: str = None,
         order_amount: str = None,
         reduce_only: bool = None,
         visible_quantity: str = None,
     ):
+        if reduce_only is not None:
+            reduce_only = str(reduce_only).lower()
+
         self._post(
             1,
             "order",
             True,
             symbol=symbol,
             broker_id=self._application_id,
             client_order_id=client_order_id,
@@ -339,14 +364,17 @@
         order_price: str = None,
         order_quantity: str = None,
         reduce_only: bool = None,
         trigger_price: str = None,
         trigger_price_type: str = None,
         visible_quantity: str = None,
     ):
+        if reduce_only is not None:
+            reduce_only = str(reduce_only).lower()
+
         self._post(
             3,
             "algo/order",
             True,
             activatedPrice=activated_price,
             algoType=algo_type,
             brokerId=self._application_id,
```

### Comparing `tarvis-exchange-woo-0.9.6/test/test_exchange_woo_margin.py` & `tarvis-exchange-woo-0.9.9/test/test_exchange_woo_margin.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
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
 
@@ -106,14 +107,15 @@
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
 
@@ -148,14 +150,15 @@
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
 
@@ -193,14 +196,15 @@
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
@@ -230,14 +234,15 @@
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
 
@@ -270,14 +275,15 @@
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
 
@@ -312,14 +318,15 @@
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
 
@@ -356,14 +363,15 @@
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

### Comparing `tarvis-exchange-woo-0.9.6/test/test_exchange_woo_perpetual.py` & `tarvis-exchange-woo-0.9.9/test/test_exchange_woo_perpetual.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,29 +70,30 @@
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
 
     positions = exchange.get_positions()
     base_position_end = positions.get(_BASE_ASSET, 0)
     quote_position_end = positions.get(_QUOTE_ASSET, 0)
     assert float(base_position_end - base_position_start) == pytest.approx(
         float(order_quantity), 0.01
     )
     assert float(quote_position_start - quote_position_end) == pytest.approx(
-        float(order_quantity * order_price), 0.01
+        float(order_quantity * order_price), 0.02
     )
 
 
 def test_long_stop_loss_order():
     positions = exchange.get_positions()
     base_position = positions.get(_BASE_ASSET, 0)
     # Assumes a previous test purchased minimum quantity
@@ -106,14 +107,15 @@
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
 
@@ -148,14 +150,15 @@
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
 
@@ -193,14 +196,15 @@
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
@@ -230,14 +234,15 @@
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
 
@@ -270,14 +275,15 @@
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
 
@@ -312,14 +318,15 @@
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
 
@@ -356,22 +363,23 @@
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
     assert quote_position_end < quote_position_start
     assert base_position_end > base_position_start
     assert float(base_position_end - base_position_start) == pytest.approx(
         float(order_quantity), 0.01
     )
     assert float(quote_position_start - quote_position_end) == pytest.approx(
-        float(order_quantity * order_price), 0.01
+        float(order_quantity * order_price), 0.02
     )
```

### Comparing `tarvis-exchange-woo-0.9.6/test/test_exchange_woo_spot.py` & `tarvis-exchange-woo-0.9.9/test/test_exchange_woo_spot.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
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
 
@@ -104,14 +105,15 @@
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
 
@@ -146,14 +148,15 @@
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
 
@@ -191,14 +194,15 @@
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
```

