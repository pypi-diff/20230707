# Comparing `tmp/coinglass_api-0.5.0.tar.gz` & `tmp/coinglass_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinglass_api-0.5.0.tar", max compression
+gzip compressed data, was "coinglass_api-1.0.0.tar", max compression
```

## Comparing `coinglass_api-0.5.0.tar` & `coinglass_api-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-01-15 20:06:02.595582 coinglass_api-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     4267 2023-06-30 12:39:55.834401 coinglass_api-0.5.0/README.md
--rw-r--r--   0        0        0       57 2023-01-15 18:42:45.746707 coinglass_api-0.5.0/coinglass_api/__init__.py
--rw-r--r--   0        0        0    17895 2023-06-30 12:23:48.647991 coinglass_api-0.5.0/coinglass_api/api.py
--rw-r--r--   0        0        0      809 2023-06-30 12:28:58.463408 coinglass_api-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5011 1970-01-01 00:00:00.000000 coinglass_api-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-01-15 20:06:02.595582 coinglass_api-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     4426 2023-07-07 16:17:16.974156 coinglass_api-1.0.0/README.md
+-rw-r--r--   0        0        0      122 2023-07-07 14:56:03.702274 coinglass_api-1.0.0/coinglass_api/__init__.py
+-rw-r--r--   0        0        0    31118 2023-07-07 16:00:32.778643 coinglass_api-1.0.0/coinglass_api/api.py
+-rw-r--r--   0        0        0      809 2023-07-07 16:15:36.754227 coinglass_api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 coinglass_api-1.0.0/PKG-INFO
```

### Comparing `coinglass_api-0.5.0/LICENSE.md` & `coinglass_api-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coinglass_api-0.5.0/README.md` & `coinglass_api-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Coinglass API
+
 [![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)
 [![Downloads](https://pepy.tech/badge/coinglass-api)](https://pepy.tech/project/coinglass-api)
 [![codecov](https://codecov.io/gh/dineshpinto/coinglass-api/branch/main/graph/badge.svg?token=XTJRRU2W1T)](https://codecov.io/gh/dineshpinto/coinglass-api)
 [![API unittest](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml/badge.svg)](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml)
 
 ## Unofficial Python client for Coinglass API
 
 Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.
-All data is output in pandas DataFrames (single or multi-index) and all time series data uses a `DateTimeIndex`.
-
-**Note**: Currently supports the `indicator` and `index` API endpoints.
+All data is output in pandas DataFrames (single or multi-index) and all time-series data uses a `DateTimeIndex`.
+Supports all CoinGlass API endpoints.
 
 ![Example Plot](https://github.com/dineshpinto/coinglass-api/blob/main/examples/example_plot.jpg?raw=true)
 
 ## Installation
 
 ```bash
 pip install coinglass-api
@@ -22,14 +22,20 @@
 ## Usage
 
 ```python
 from coinglass_api import CoinglassAPI
 
 cg = CoinglassAPI(coinglass_secret="abcd1234")
 
+# Get perpetual markets for BTC
+perp_markets_btc = cg.perpetual_market(symbol="BTC")
+
+# Get OI history
+oi_history_btc = cg.open_interest_history(symbol="BTC", time_type="h1", currency="USD")
+
 # Funding rate of ETH on dYdX
 fr_btc_dydx = cg.funding(ex="dYdX", pair="ETH-USD", interval="h8")
 
 # Get average funding for BTC
 fr_avg_btc = cg.funding_average(symbol="BTC", interval="h4")
 
 # Get funding OHLC for ETHUSDT on Binance
@@ -84,14 +90,15 @@
 dtypes: float64(1), object(3)
 memory usage: 19.5+ KB
 ```
 
 ```
 >>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").plot(y="fundingRate")
 ```
+
 ![funding_rate](https://github.com/dineshpinto/coinglass-api/blob/main/examples/funding_rate.jpg?raw=true)
 
 ## Disclaimer
 
 This project is for educational purposes only. You should not construe any such information or other material as legal,
 tax, investment, financial, or other advice. Nothing contained here constitutes a solicitation, recommendation,
 endorsement, or offer by me or any third party service provider to buy or sell any securities or other financial
```

### Comparing `coinglass_api-0.5.0/pyproject.toml` & `coinglass_api-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinglass-api"
-version = "0.5.0"
+version = "1.0.0"
 repository = "https://github.com/dineshpinto/coinglass-api"
 homepage = "https://github.com/dineshpinto/coinglass-api"
 license = "MIT"
 keywords = ["coinglass", "api", "crypto", "cryptocurrency", "bitcoin", "ethereum", "binance", "dydx", "okex"]
 description = "Unofficial Python client for Coinglass API"
 authors = ["dineshpinto <annual.fallout_0z@gmail.com>"]
 readme = "README.md"
```

### Comparing `coinglass_api-0.5.0/PKG-INFO` & `coinglass_api-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinglass-api
-Version: 0.5.0
+Version: 1.0.0
 Summary: Unofficial Python client for Coinglass API
 Home-page: https://github.com/dineshpinto/coinglass-api
 License: MIT
 Keywords: coinglass,api,crypto,cryptocurrency,bitcoin,ethereum,binance,dydx,okex
 Author: dineshpinto
 Author-email: annual.fallout_0z@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -14,25 +14,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/dineshpinto/coinglass-api
 Description-Content-Type: text/markdown
 
 # Coinglass API
+
 [![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)
 [![Downloads](https://pepy.tech/badge/coinglass-api)](https://pepy.tech/project/coinglass-api)
 [![codecov](https://codecov.io/gh/dineshpinto/coinglass-api/branch/main/graph/badge.svg?token=XTJRRU2W1T)](https://codecov.io/gh/dineshpinto/coinglass-api)
 [![API unittest](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml/badge.svg)](https://github.com/dineshpinto/coinglass-api/actions/workflows/api_unitests.yml)
 
 ## Unofficial Python client for Coinglass API
 
 Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.
-All data is output in pandas DataFrames (single or multi-index) and all time series data uses a `DateTimeIndex`.
-
-**Note**: Currently supports the `indicator` and `index` API endpoints.
+All data is output in pandas DataFrames (single or multi-index) and all time-series data uses a `DateTimeIndex`.
+Supports all CoinGlass API endpoints.
 
 ![Example Plot](https://github.com/dineshpinto/coinglass-api/blob/main/examples/example_plot.jpg?raw=true)
 
 ## Installation
 
 ```bash
 pip install coinglass-api
@@ -41,14 +41,20 @@
 ## Usage
 
 ```python
 from coinglass_api import CoinglassAPI
 
 cg = CoinglassAPI(coinglass_secret="abcd1234")
 
+# Get perpetual markets for BTC
+perp_markets_btc = cg.perpetual_market(symbol="BTC")
+
+# Get OI history
+oi_history_btc = cg.open_interest_history(symbol="BTC", time_type="h1", currency="USD")
+
 # Funding rate of ETH on dYdX
 fr_btc_dydx = cg.funding(ex="dYdX", pair="ETH-USD", interval="h8")
 
 # Get average funding for BTC
 fr_avg_btc = cg.funding_average(symbol="BTC", interval="h4")
 
 # Get funding OHLC for ETHUSDT on Binance
@@ -103,14 +109,15 @@
 dtypes: float64(1), object(3)
 memory usage: 19.5+ KB
 ```
 
 ```
 >>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").plot(y="fundingRate")
 ```
+
 ![funding_rate](https://github.com/dineshpinto/coinglass-api/blob/main/examples/funding_rate.jpg?raw=true)
 
 ## Disclaimer
 
 This project is for educational purposes only. You should not construe any such information or other material as legal,
 tax, investment, financial, or other advice. Nothing contained here constitutes a solicitation, recommendation,
 endorsement, or offer by me or any third party service provider to buy or sell any securities or other financial
```

