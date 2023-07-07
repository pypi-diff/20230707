# Comparing `tmp/OctoBot-Trading-2.4.6.tar.gz` & `tmp/OctoBot-Trading-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Trading-2.4.6.tar", last modified: Wed Jul  5 20:36:51 2023, max compression
+gzip compressed data, was "OctoBot-Trading-2.4.7.tar", last modified: Fri Jul  7 08:19:56 2023, max compression
```

## Comparing `OctoBot-Trading-2.4.6.tar` & `OctoBot-Trading-2.4.7.tar`

### file list

```diff
@@ -1,574 +1,574 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.356939 OctoBot-Trading-2.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    33195 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.304938 OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 20:36:51.000000 OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24373 2023-07-05 20:36:51.000000 OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:36:51.000000 OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:36:51.000000 OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 20:36:51.000000 OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 20:36:51.000000 OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 20:36:51.356939 OctoBot-Trading-2.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/api/
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/api/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/contract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/margin_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/exchange_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/funding_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/kline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/kline_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.308938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/order_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/prices_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/abstract_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/adapters/abstract_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/config/backtesting_exchange_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/config/exchange_config_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.312938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    44886 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_websocket_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/default_rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/default_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/exchange_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42964 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/traders/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/traders/trader_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45451 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/types/rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/types/websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/exchange_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/websockets_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/modes/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/modes/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/channel/abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22982 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/channel/abstract_mode_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/channel/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/mode_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/modes_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/modes_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.316938 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/context_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/dsl/quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/dsl/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/modes/scripted_trading_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/scripted_trading_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/exchange_personal_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/orders_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/decimal_order_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/group_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/orders_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/orders_storage_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.320938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.324938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.324938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/sell_market_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.324938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/unknown_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/unsupported_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.324938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.324938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.324938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/balance_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.324938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/sub_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.324938 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/value_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/positions_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39334 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/position_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/active_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/idle_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/liquidate_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/position_state_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/types/inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/types/linear_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/channel/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/channel/trades_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trade_pnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trades_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/fee_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/transfer_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.328939 OctoBot-Trading-2.4.6/octobot_trading/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/signals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/octobot_trading/signals/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/signals/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/signals/channel/remote_trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/signals/channel/signal_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/signals/signal_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/signals/trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/signals/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/octobot_trading/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/abstract_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/candles_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/orders_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/portfolio_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/trades_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/transactions_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/storage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/octobot_trading/supervisors/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/supervisors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/supervisors/abstract_portfolio_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/supervisors/abstract_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/octobot_trading/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/config_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/initializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/initialization_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/simulator_updater_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/exchanges_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/websocket_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:36:51.356939 OctoBot-Trading-2.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.304938 OctoBot-Trading-2.4.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/api/test_trades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/tests/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.332939 OctoBot-Trading-2.4.6/tests/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/contracts/test_future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/contracts/test_margin_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/funding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/funding/test_funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/kline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/kline/test_kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/ohlcv/test_candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/ohlcv/test_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/order_book/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/order_book/test_order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/prices/test_price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/prices/test_prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/recent_trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/recent_trades/test_recent_trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/test_exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/ticker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchange_data/ticker/test_ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchanges/connectors/ccxt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/connectors/ccxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/implementations/test_default_rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/implementations/test_default_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/test_abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/test_abstract_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/test_exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50875 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/traders/test_trader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/types/test_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/util/test_exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/exchanges/util/test_exchange_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/modes/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.336939 OctoBot-Trading-2.4.6/tests/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.340939 OctoBot-Trading-2.4.6/tests/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/script_keywords/basic_keywords/test_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/script_keywords/basic_keywords/test_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.340939 OctoBot-Trading-2.4.6/tests/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/script_keywords/dsl/test_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/test_abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/modes/test_abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.340939 OctoBot-Trading-2.4.6/tests/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.340939 OctoBot-Trading-2.4.6/tests/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.340939 OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/test_group_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.340939 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_pending_creation_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/test_decimal_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/test_double_filled_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/test_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/test_order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/test_order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/test_orders_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/test_orders_storage_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.340939 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.344939 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.344939 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/market/test_buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/market/test_sell_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/test_unknown_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.344939 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.344939 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.344939 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/test_future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/test_margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/test_spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.344939 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_value_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85551 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/test_future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/test_margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/test_spot_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/test_position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/test_positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/types/test_inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/positions/types/test_linear_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/trades/test_trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/trades/test_trade_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/trades/test_trade_pnl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/transactions/test_transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/personal_data/transactions/test_transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/signals/test_trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/signals/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/test_utils/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/test_utils/random_numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests/util/test_config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.348939 OctoBot-Trading-2.4.6/tests_additional/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:36:51.356939 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/real_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/real_futures_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_binance_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bithumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bitso.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bitstamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bittrex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bybit_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_coinbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_coinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_cryptocom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_hitbtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_hollaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_kucoin_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_mexc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_ndax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_okcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_okx_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_phemex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_poloniex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_upbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-05 20:35:58.000000 OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_wavesexchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.130612 OctoBot-Trading-2.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    33274 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.078611 OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-07 08:19:55.000000 OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24373 2023-07-07 08:19:56.000000 OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:19:55.000000 OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:19:55.000000 OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-07 08:19:55.000000 OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-07 08:19:55.000000 OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-07 08:19:56.130612 OctoBot-Trading-2.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.078611 OctoBot-Trading-2.4.7/octobot_trading/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.078611 OctoBot-Trading-2.4.7/octobot_trading/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/api/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.078611 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/contract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/margin_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/exchange_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/funding_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/kline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/kline_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.082612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/prices_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27517 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/abstract_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/adapters/abstract_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/config/backtesting_exchange_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/config/exchange_config_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.086612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44886 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_websocket_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/exchange_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42964 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/traders/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/traders/trader_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45451 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/types/rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/types/websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/exchange_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/websockets_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/modes/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11155 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/channel/abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/channel/abstract_mode_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/channel/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/mode_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/modes_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/modes_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.090612 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25931 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/context_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.094612 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/dsl/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/dsl/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.094612 OctoBot-Trading-2.4.7/octobot_trading/modes/scripted_trading_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/scripted_trading_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16335 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.094612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/exchange_personal_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.094612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.094612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/orders_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/decimal_order_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.094612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/group_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22239 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/orders_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/orders_storage_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.094612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.098612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.098612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.098612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/sell_market_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.098612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/unknown_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/unsupported_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.098612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.098612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.098612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/balance_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.102612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17826 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14495 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/sub_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.102612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/value_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.102612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.102612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/positions_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39334 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/position_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.102612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/active_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/idle_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/liquidate_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/position_state_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.102612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/types/inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/types/linear_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.102612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.102612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/channel/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/channel/trades_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trade_pnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trades_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.106612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.106612 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/fee_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/transfer_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.106612 OctoBot-Trading-2.4.7/octobot_trading/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/signals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.106612 OctoBot-Trading-2.4.7/octobot_trading/signals/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/signals/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/signals/channel/remote_trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/signals/channel/signal_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/signals/signal_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/signals/trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/signals/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.106612 OctoBot-Trading-2.4.7/octobot_trading/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/abstract_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/candles_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/orders_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/portfolio_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/trades_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/transactions_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/storage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.106612 OctoBot-Trading-2.4.7/octobot_trading/supervisors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/supervisors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/supervisors/abstract_portfolio_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/supervisors/abstract_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.106612 OctoBot-Trading-2.4.7/octobot_trading/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/config_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/initializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/initialization_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/simulator_updater_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.106612 OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/exchanges_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/websocket_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:19:56.130612 OctoBot-Trading-2.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.074612 OctoBot-Trading-2.4.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/api/test_trades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/contracts/test_future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/contracts/test_margin_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/funding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/funding/test_funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/kline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/kline/test_kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/ohlcv/test_candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/ohlcv/test_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/order_book/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/order_book/test_order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/prices/test_price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/prices/test_prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/recent_trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/recent_trades/test_recent_trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/test_exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.110612 OctoBot-Trading-2.4.7/tests/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/ticker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchange_data/ticker/test_ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/implementations/test_default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/implementations/test_default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/test_abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/test_abstract_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/test_exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50875 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/traders/test_trader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/types/test_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/util/test_exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/exchanges/util/test_exchange_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/script_keywords/basic_keywords/test_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/script_keywords/basic_keywords/test_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/script_keywords/dsl/test_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/test_abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/modes/test_abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.114612 OctoBot-Trading-2.4.7/tests/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.118612 OctoBot-Trading-2.4.7/tests/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.118612 OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/test_group_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.118612 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_pending_creation_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/test_decimal_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/test_double_filled_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/test_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/test_order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/test_order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/test_orders_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/test_orders_storage_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.118612 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.118612 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.118612 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/market/test_buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/market/test_sell_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/test_unknown_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.122612 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.122612 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.122612 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/test_future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/test_margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/test_spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.122612 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11149 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_value_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.122612 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85551 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/test_future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/test_margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/test_spot_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/test_position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/test_positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37450 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/types/test_inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/positions/types/test_linear_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/trades/test_trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/trades/test_trade_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/trades/test_trade_pnl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/transactions/test_transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/personal_data/transactions/test_transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/signals/test_trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/signals/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/test_utils/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/test_utils/random_numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests/util/test_config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.126612 OctoBot-Trading-2.4.7/tests_additional/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:19:56.130612 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/real_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/real_futures_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_binance_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bitfinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bithumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bitso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bitstamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bittrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bybit_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_coinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_cryptocom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_hitbtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_hollaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_kucoin_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_ndax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_okcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_okx_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_phemex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_poloniex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_upbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-07 08:18:51.000000 OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_wavesexchange.py
```

### Comparing `OctoBot-Trading-2.4.6/CHANGELOG.md` & `OctoBot-Trading-2.4.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.4.7] - 2023-07-07
+### Added
+- [Positions] Log error on hedged positions
+
 ## [2.4.6] - 2023-07-05
 ### Fixed
 - [API] is_trader_existing_and_enabled
 
 ## [2.4.5] - 2023-07-03
 ### Added
 - Full stop loss support for supporting exchanges
```

### Comparing `OctoBot-Trading-2.4.6/LICENSE` & `OctoBot-Trading-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/PKG-INFO` & `OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.4.6
+Version: 2.4.7
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.4.6](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.7](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.6/OctoBot_Trading.egg-info/SOURCES.txt` & `OctoBot-Trading-2.4.7/OctoBot_Trading.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/PKG-INFO` & `OctoBot-Trading-2.4.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.4.6
+Version: 2.4.7
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: contact@drakkar.software
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.4.6](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.7](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.6/README.md` & `OctoBot-Trading-2.4.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Trading [2.4.6](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.4.7](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 PROJECT_NAME = "OctoBot-Trading"
-VERSION = "2.4.6"  # major.minor.revision
+VERSION = "2.4.7"  # major.minor.revision
```

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/channels.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/contracts.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/contracts.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/exchange.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/modes.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/orders.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/portfolio.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/positions.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/profitability.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/storage.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/symbol_data.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/trader.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/api/trades.py` & `OctoBot-Trading-2.4.7/octobot_trading/api/trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/constants.py` & `OctoBot-Trading-2.4.7/octobot_trading/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/enums.py` & `OctoBot-Trading-2.4.7/octobot_trading/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/errors.py` & `OctoBot-Trading-2.4.7/octobot_trading/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_channel.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/contract_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/contract_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/future_contract.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/contracts/margin_contract.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/contracts/margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/exchange_symbol_data.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/exchange_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/exchange_symbols_data.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/funding.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/funding.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/funding_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/funding_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/funding/funding_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/funding/funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/kline.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/kline.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/kline_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/kline_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/kline/kline_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/kline/kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/candles_adapter.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/candles_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/order_book.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/order_book.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/order_book_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/order_book_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/order_book/order_book_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/order_book/order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/price.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/price.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/prices_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/prices_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/price_events_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/prices/prices_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/prices/prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/ticker.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/ticker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/ticker_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/ticker_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchange_data/ticker/ticker_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchange_data/ticker/ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/abstract_exchange.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/abstract_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/abstract_websocket_exchange.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/abstract_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/adapters/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/adapters/abstract_adapter.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/adapters/abstract_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/config/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/config/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/config/backtesting_exchange_config.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/config/backtesting_exchange_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/config/exchange_config_data.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/config/exchange_config_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/constants.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/ccxt/enums.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/ccxt/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/simulator/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_builder.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_channels.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_details.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_details.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchange_websocket_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchange_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/exchanges.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/exchanges.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/default_rest_exchange.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/default_rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/default_websocket_exchange.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/default_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/implementations/exchange_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/implementations/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/traders/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/traders/trader.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/traders/trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/traders/trader_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/traders/trader_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/types/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/types/rest_exchange.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/types/rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/types/websocket_exchange.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/types/websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/exchange_market_status_fixer.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/exchange_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/exchange_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/exchanges/util/websockets_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/exchanges/util/websockets_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/abstract_trading_mode.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/abstract_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/channel/abstract_mode_consumer.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/channel/abstract_mode_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/channel/abstract_mode_producer.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/channel/abstract_mode_producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,14 +440,15 @@
                 context,
                 common_enums.ActivationTopics.EVALUATION_CYCLE.value,
                 activation_topic_values
             )
         try:
             await self._apply_exchange_side_config(context)
         except Exception as err:
+            # TODO important error to display
             self.logger.exception(err, True, f"Error when applying exchange side config: {err}")
 
     async def _apply_exchange_side_config(self, context):
         # can be slow, call in a task if necessary
         if context.exchange_manager.is_future:
             if not self._is_ready_to_trade.is_set():
                 await util.wait_for_topic_init(self.exchange_manager, self.CONFIG_INIT_TIMEOUT,
```

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/channel/mode.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/channel/mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/mode_config.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/mode_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/modes_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/modes_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/modes_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/modes_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/amount.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/configuration.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/context_management.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/context_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/dsl/quantity.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/dsl/quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/script_keywords/dsl/values.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/script_keywords/dsl/values.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/scripted_trading_mode/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/scripted_trading_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py` & `OctoBot-Trading-2.4.7/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/octobot_channel_consumer.py` & `OctoBot-Trading-2.4.7/octobot_trading/octobot_channel_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/exchange_personal_data.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/exchange_personal_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/orders.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/orders_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/orders_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/decimal_order_adapter.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/group_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/group_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_adapter.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_group.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/order_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/orders_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/orders_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/orders_storage_operations.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/orders_storage_operations.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/cancel_order_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/close_order_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/fill_order_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/open_order_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/order_state_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/order_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/states/pending_creation_order_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/states/pending_creation_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/limit_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/limit/take_profit_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/limit/take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/buy_market_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/market_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/market/sell_market_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/market/sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/unknown_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/orders/types/unsupported_order.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/orders/types/unsupported_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/asset.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/future_asset.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/margin_asset.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/assets/spot_asset.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/assets/spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/balance.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/balance_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/balance_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/historical_asset_value.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/historical_asset_value.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_profitability.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/portfolio_value_holder.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/sub_portfolio.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/sub_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/future_portfolio.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/margin_portfolio.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/types/spot_portfolio.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/types/spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/portfolios/value_converter.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/portfolios/value_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/positions.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/positions_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/positions_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/position.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/position_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/position_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/position_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/position_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/positions_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/positions_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     POSITION_ID_SEPARATOR = "_"
 
     def __init__(self, trader):
         super().__init__()
         self.logger = logging.get_logger(self.__class__.__name__)
         self.trader = trader
         self.positions = collections.OrderedDict()
+        self.logged_unsupported_positions = set()
 
     async def initialize_impl(self):
         self._reset_positions()
 
     def get_symbol_position(self, symbol, side):
         """
         Returns or create the symbol position instance
@@ -75,22 +76,39 @@
         """
         Create or update a position from a raw dictionary
         :param symbol: the position symbol
         :param side: the position side
         :param raw_position: the position raw dictionary
         :return: True when the creation or the update succeeded
         """
+        self._ensure_support(raw_position)
         position_id = self._generate_position_id(symbol=symbol, side=side)
         if position_id not in self.positions:
             new_position = position_factory.create_position_instance_from_raw(self.trader, raw_position=raw_position)
             new_position.position_id = position_id
             return await self._finalize_position_creation(new_position, is_from_exchange_data=True)
 
         return self.positions[position_id].update_from_raw(raw_position)
 
+    def _ensure_support(self, raw_position):
+        if (
+            raw_position.get(enums.ExchangeConstantsPositionColumns.POSITION_MODE.value, enums.PositionMode.ONE_WAY)
+            is not enums.PositionMode.ONE_WAY
+            and raw_position[enums.ExchangeConstantsPositionColumns.SYMBOL.value]
+            not in self.logged_unsupported_positions
+        ):
+            # TODO important error to display
+            self.logger.error(
+                f"{raw_position[enums.ExchangeConstantsPositionColumns.SYMBOL.value]} position is in "
+                f"{raw_position[enums.ExchangeConstantsPositionColumns.POSITION_MODE.value].name} mode. "
+                f"This mode is not supported and will create unexpected behaviors in OctoBot. Please switch "
+                f"to {enums.PositionMode.ONE_WAY.name} mode on {self.trader.exchange_manager.exchange_name}."
+            )
+            self.logged_unsupported_positions.add(raw_position[enums.ExchangeConstantsPositionColumns.SYMBOL.value])
+
     def set_initialized_event(self, symbol):
         commons_tree.EventProvider.instance().trigger_event(
             self.trader.exchange_manager.bot_id, commons_tree.get_exchange_path(
                 self.trader.exchange_manager.exchange_name,
                 commons_enums.InitializationEventExchangeTopics.POSITIONS.value,
                 symbol=symbol
             )
```

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/active_position_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/active_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/idle_position_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/idle_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/liquidate_position_state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/liquidate_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/states/position_state_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/states/position_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/types/inverse_position.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/types/inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/positions/types/linear_position.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/positions/types/linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/state.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/channel/trades.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/channel/trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/channel/trades_updater.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/channel/trades_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trade.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trade_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trade_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trade_pnl.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trade_pnl.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trades_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/trades/trades_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/trades/trades_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/transaction.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/transaction_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/transactions_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/blockchain_transaction.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/blockchain_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/fee_transaction.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/fee_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/personal_data/transactions/types/transfer_transaction.py` & `OctoBot-Trading-2.4.7/octobot_trading/personal_data/transactions/types/transfer_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/signals/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/signals/channel/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/signals/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/signals/channel/remote_trading_signal.py` & `OctoBot-Trading-2.4.7/octobot_trading/signals/channel/remote_trading_signal.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py` & `OctoBot-Trading-2.4.7/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/signals/channel/signal_producer.py` & `OctoBot-Trading-2.4.7/octobot_trading/signals/channel/signal_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/signals/signal_creation.py` & `OctoBot-Trading-2.4.7/octobot_trading/signals/signal_creation.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/signals/trading_signal_bundle_builder.py` & `OctoBot-Trading-2.4.7/octobot_trading/signals/trading_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/signals/util.py` & `OctoBot-Trading-2.4.7/octobot_trading/signals/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/abstract_storage.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/candles_storage.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/candles_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/orders_storage.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/orders_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/portfolio_storage.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/portfolio_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/storage_manager.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/storage_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/trades_storage.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/trades_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/transactions_storage.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/transactions_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/storage/util.py` & `OctoBot-Trading-2.4.7/octobot_trading/storage/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/supervisors/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/supervisors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/supervisors/abstract_portfolio_supervisor.py` & `OctoBot-Trading-2.4.7/octobot_trading/supervisors/abstract_portfolio_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/supervisors/abstract_supervisor.py` & `OctoBot-Trading-2.4.7/octobot_trading/supervisors/abstract_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/config_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/initializable.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/initializable.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/initialization_util.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/initialization_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/simulator_updater_utils.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/simulator_updater_utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/__init__.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/exchanges_test_tools.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/exchanges_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/octobot_trading/util/test_tools/websocket_test_tools.py` & `OctoBot-Trading-2.4.7/octobot_trading/util/test_tools/websocket_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/requirements.txt` & `OctoBot-Trading-2.4.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/setup.py` & `OctoBot-Trading-2.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/__init__.py` & `OctoBot-Trading-2.4.7/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_channels.py` & `OctoBot-Trading-2.4.7/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_exchange.py` & `OctoBot-Trading-2.4.7/tests/api/test_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_modes.py` & `OctoBot-Trading-2.4.7/tests/api/test_modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_orders.py` & `OctoBot-Trading-2.4.7/tests/api/test_orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_portfolio.py` & `OctoBot-Trading-2.4.7/tests/api/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_profitability.py` & `OctoBot-Trading-2.4.7/tests/api/test_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_symbol_data.py` & `OctoBot-Trading-2.4.7/tests/api/test_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_trader.py` & `OctoBot-Trading-2.4.7/tests/api/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/api/test_trades.py` & `OctoBot-Trading-2.4.7/tests/api/test_trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/cli/__init__.py` & `OctoBot-Trading-2.4.7/tests/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/contracts/test_future_contract.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/contracts/test_future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/contracts/test_margin_contract.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/contracts/test_margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/funding/test_funding_manager.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/funding/test_funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/kline/test_kline_manager.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/kline/test_kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/ohlcv/test_candles_adapter.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/ohlcv/test_candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/ohlcv/test_candles_manager.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/ohlcv/test_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/order_book/test_order_book_manager.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/order_book/test_order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/prices/test_price_events_manager.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/prices/test_price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/prices/test_prices_manager.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/prices/test_prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/recent_trades/test_recent_trades_manager.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/recent_trades/test_recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/test_exchange_symbols_data.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/test_exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchange_data/ticker/test_ticker_manager.py` & `OctoBot-Trading-2.4.7/tests/exchange_data/ticker/test_ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/connectors/ccxt/test_ccxt_connector.py` & `OctoBot-Trading-2.4.7/tests/exchanges/connectors/ccxt/test_ccxt_connector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/implementations/test_default_rest_exchange.py` & `OctoBot-Trading-2.4.7/tests/exchanges/implementations/test_default_rest_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/implementations/test_default_websocket_exchange.py` & `OctoBot-Trading-2.4.7/tests/exchanges/implementations/test_default_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/test_abstract_exchange.py` & `OctoBot-Trading-2.4.7/tests/exchanges/test_abstract_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/test_abstract_websocket_exchange.py` & `OctoBot-Trading-2.4.7/tests/exchanges/test_abstract_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_builder.py` & `OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_config_data.py` & `OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_config_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_factory.py` & `OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_manager.py` & `OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/test_exchange_simulator.py` & `OctoBot-Trading-2.4.7/tests/exchanges/test_exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/test_exchanges.py` & `OctoBot-Trading-2.4.7/tests/exchanges/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/traders/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/traders/test_trader.py` & `OctoBot-Trading-2.4.7/tests/exchanges/traders/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/types/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/types/test_websocket_exchange.py` & `OctoBot-Trading-2.4.7/tests/exchanges/types/test_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/util/__init__.py` & `OctoBot-Trading-2.4.7/tests/exchanges/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/util/test_exchange_market_status_fixer.py` & `OctoBot-Trading-2.4.7/tests/exchanges/util/test_exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/exchanges/util/test_exchange_util.py` & `OctoBot-Trading-2.4.7/tests/exchanges/util/test_exchange_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/modes/__init__.py` & `OctoBot-Trading-2.4.7/tests/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.4.7/tests/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/modes/script_keywords/basic_keywords/test_account_balance.py` & `OctoBot-Trading-2.4.7/tests/modes/script_keywords/basic_keywords/test_account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/modes/script_keywords/basic_keywords/test_amount.py` & `OctoBot-Trading-2.4.7/tests/modes/script_keywords/basic_keywords/test_amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.4.7/tests/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/modes/script_keywords/dsl/test_quantity.py` & `OctoBot-Trading-2.4.7/tests/modes/script_keywords/dsl/test_quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/modes/test_abstract_mode_consumer.py` & `OctoBot-Trading-2.4.7/tests/modes/test_abstract_mode_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/modes/test_abstract_trading_mode.py` & `OctoBot-Trading-2.4.7/tests/modes/test_abstract_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/test_group_util.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/test_group_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_cancel_order_state.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_close_order_state.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_fill_order_state.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_open_order_state.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_order_state.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_order_state_factory.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_order_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/states/test_pending_creation_order_state.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/states/test_pending_creation_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/test_decimal_order_adapter.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/test_decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/test_double_filled_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/test_double_filled_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/test_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/test_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/test_order_adapter.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/test_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/test_order_factory.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/test_order_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/test_order_util.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/test_order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/test_orders_manager.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/test_orders_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/test_orders_storage_operations.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/test_orders_storage_operations.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_buy_limit_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_sell_limit_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_stop_loss_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/limit/test_take_profit_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/limit/test_take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/market/test_buy_market_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/market/test_buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/market/test_sell_market_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/market/test_sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/test_unknown_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/test_unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py` & `OctoBot-Trading-2.4.7/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/test_future_asset.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/test_future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/test_margin_asset.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/test_margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/assets/test_spot_asset.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/assets/test_spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_asset.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_portfolio.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_portfolio_manager.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_portfolio_profitability.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_portfolio_value_holder.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/test_value_converter.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/test_value_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/test_future_portfolio.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/test_future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/test_margin_portfolio.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/test_margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/portfolios/types/test_spot_portfolio.py` & `OctoBot-Trading-2.4.7/tests/personal_data/portfolios/types/test_spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/test_position.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/test_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/test_position_factory.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/test_position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/test_positions_manager.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/test_positions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/types/test_inverse_position.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/types/test_inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/positions/types/test_linear_position.py` & `OctoBot-Trading-2.4.7/tests/personal_data/positions/types/test_linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/trades/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/trades/test_trade_factory.py` & `OctoBot-Trading-2.4.7/tests/personal_data/trades/test_trade_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/trades/test_trade_manager.py` & `OctoBot-Trading-2.4.7/tests/personal_data/trades/test_trade_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/trades/test_trade_pnl.py` & `OctoBot-Trading-2.4.7/tests/personal_data/trades/test_trade_pnl.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.4.7/tests/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/transactions/test_transaction_factory.py` & `OctoBot-Trading-2.4.7/tests/personal_data/transactions/test_transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/personal_data/transactions/test_transactions_manager.py` & `OctoBot-Trading-2.4.7/tests/personal_data/transactions/test_transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/signals/__init__.py` & `OctoBot-Trading-2.4.7/tests/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/signals/test_trading_signal_bundle_builder.py` & `OctoBot-Trading-2.4.7/tests/signals/test_trading_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/signals/test_util.py` & `OctoBot-Trading-2.4.7/tests/signals/test_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/test_utils/order_util.py` & `OctoBot-Trading-2.4.7/tests/test_utils/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/test_utils/random_numbers.py` & `OctoBot-Trading-2.4.7/tests/test_utils/random_numbers.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/util/__init__.py` & `OctoBot-Trading-2.4.7/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests/util/test_config_util.py` & `OctoBot-Trading-2.4.7/tests/util/test_config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/__init__.py` & `OctoBot-Trading-2.4.7/tests_additional/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/__init__.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/real_exchange_tester.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/real_exchange_tester.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/real_futures_exchange_tester.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/real_futures_exchange_tester.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_ascendex.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_ascendex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_binance.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_binance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_binance_futures.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_binance_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bitfinex.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bitfinex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bitget.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bitget.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bithumb.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bithumb.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bitso.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bitso.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bitstamp.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bitstamp.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bittrex.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bittrex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bybit.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bybit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_bybit_futures.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_bybit_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_coinbase.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_coinbase.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_coinex.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_coinex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_cryptocom.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_cryptocom.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_gateio.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_gateio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_hitbtc.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_hitbtc.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_hollaex.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_hollaex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_huobi.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_huobi.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_huobipro.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_kraken.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_kraken.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_kucoin.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_kucoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_kucoin_futures.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_kucoin_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_mexc.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_mexc.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_ndax.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_ndax.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_okcoin.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_okcoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_okx.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_okx.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_okx_futures.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_okx_futures.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_phemex.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_phemex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_poloniex.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_poloniex.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_upbit.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_upbit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.4.6/tests_additional/real_exchanges/test_wavesexchange.py` & `OctoBot-Trading-2.4.7/tests_additional/real_exchanges/test_wavesexchange.py`

 * *Files identical despite different names*

