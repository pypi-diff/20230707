# Comparing `tmp/quantplay-1.3.5.tar.gz` & `tmp/quantplay-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.3.5.tar", last modified: Fri Jul  7 04:17:22 2023, max compression
+gzip compressed data, was "quantplay-1.3.6.tar", last modified: Fri Jul  7 04:26:29 2023, max compression
```

## Comparing `quantplay-1.3.5.tar` & `quantplay-1.3.6.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.722859 quantplay-1.3.5/
--rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-07 04:17:22.722972 quantplay-1.3.5/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.3.5/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.703533 quantplay-1.3.5/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.704765 quantplay-1.3.5/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.3.5/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.707692 quantplay-1.3.5/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.708191 quantplay-1.3.5/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.3.5/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.708562 quantplay-1.3.5/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.3.5/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.3.5/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.3.5/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    28344 2023-07-07 04:17:13.000000 quantplay-1.3.5/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.3.5/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.3.5/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.3.5/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.710186 quantplay-1.3.5/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.3.5/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.3.5/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17259 2023-07-06 16:08:51.000000 quantplay-1.3.5/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.710290 quantplay-1.3.5/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.710520 quantplay-1.3.5/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.710952 quantplay-1.3.5/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28260 2023-07-06 16:08:51.000000 quantplay-1.3.5/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.711618 quantplay-1.3.5/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.3.5/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.711799 quantplay-1.3.5/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.3.5/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.3.5/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.712018 quantplay-1.3.5/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.712338 quantplay-1.3.5/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.712921 quantplay-1.3.5/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.713066 quantplay-1.3.5/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.713850 quantplay-1.3.5/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.3.5/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.714078 quantplay-1.3.5/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.714760 quantplay-1.3.5/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.715111 quantplay-1.3.5/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.715591 quantplay-1.3.5/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.3.5/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.3.5/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.3.5/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.717269 quantplay-1.3.5/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.3.5/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.3.5/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.717557 quantplay-1.3.5/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.3.5/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.717666 quantplay-1.3.5/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.3.5/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.717767 quantplay-1.3.5/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.3.5/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.717872 quantplay-1.3.5/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.3.5/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.717977 quantplay-1.3.5/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.3.5/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.718086 quantplay-1.3.5/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.3.5/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.718208 quantplay-1.3.5/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.3.5/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.718984 quantplay-1.3.5/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.3.5/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.3.5/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.3.5/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.3.5/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.719317 quantplay-1.3.5/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.3.5/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.3.5/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.721567 quantplay-1.3.5/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.3.5/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.3.5/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.3.5/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.704424 quantplay-1.3.5/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-07 04:17:22.000000 quantplay-1.3.5/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-07-07 04:17:22.000000 quantplay-1.3.5/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-07-07 04:17:22.000000 quantplay-1.3.5/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-07-07 04:17:22.000000 quantplay-1.3.5/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-07-07 04:17:22.000000 quantplay-1.3.5/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-07-07 04:17:22.723285 quantplay-1.3.5/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      875 2023-07-07 04:17:13.000000 quantplay-1.3.5/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.721810 quantplay-1.3.5/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.3.5/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.722053 quantplay-1.3.5/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.3.5/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.722290 quantplay-1.3.5/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.3.5/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:17:22.722699 quantplay-1.3.5/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.5/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.3.5/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.3.5/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.3.5/test/test_motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.202530 quantplay-1.3.6/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-07 04:26:29.202598 quantplay-1.3.6/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.3.6/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.185967 quantplay-1.3.6/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.187027 quantplay-1.3.6/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.3.6/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.189772 quantplay-1.3.6/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.190322 quantplay-1.3.6/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.3.6/quantplay/broker/finvasia_utils/shoonya.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.190643 quantplay-1.3.6/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28790 2023-07-07 04:25:31.000000 quantplay-1.3.6/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.3.6/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.3.6/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28344 2023-07-07 04:17:13.000000 quantplay-1.3.6/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.3.6/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.3.6/quantplay/broker/symphony.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.3.6/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.191968 quantplay-1.3.6/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.3.6/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.3.6/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17259 2023-07-06 16:08:51.000000 quantplay-1.3.6/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.192062 quantplay-1.3.6/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.192253 quantplay-1.3.6/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.192733 quantplay-1.3.6/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28260 2023-07-06 16:08:51.000000 quantplay-1.3.6/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.193717 quantplay-1.3.6/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.3.6/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.193944 quantplay-1.3.6/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.3.6/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.3.6/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.194198 quantplay-1.3.6/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.194660 quantplay-1.3.6/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.195330 quantplay-1.3.6/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.195483 quantplay-1.3.6/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.196094 quantplay-1.3.6/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.3.6/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.196332 quantplay-1.3.6/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.196493 quantplay-1.3.6/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.196836 quantplay-1.3.6/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.197301 quantplay-1.3.6/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.3.6/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.3.6/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.3.6/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.197938 quantplay-1.3.6/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.3.6/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.3.6/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.198157 quantplay-1.3.6/quantplay/strategies/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.3.6/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.198248 quantplay-1.3.6/quantplay/strategies/equities/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.3.6/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.198341 quantplay-1.3.6/quantplay/strategies/equities/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.3.6/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.198438 quantplay-1.3.6/quantplay/strategies/equities/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.3.6/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.198536 quantplay-1.3.6/quantplay/strategies/futures/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.3.6/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.198632 quantplay-1.3.6/quantplay/strategies/futures/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.3.6/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.198725 quantplay-1.3.6/quantplay/strategies/options/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.3.6/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.199425 quantplay-1.3.6/quantplay/strategies/options/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.3.6/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.3.6/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.3.6/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.3.6/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.199720 quantplay-1.3.6/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.3.6/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.3.6/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.201164 quantplay-1.3.6/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.3.6/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.3.6/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.3.6/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.186787 quantplay-1.3.6/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2023-07-07 04:26:29.000000 quantplay-1.3.6/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-07-07 04:26:29.000000 quantplay-1.3.6/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2023-07-07 04:26:29.000000 quantplay-1.3.6/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      221 2023-07-07 04:26:29.000000 quantplay-1.3.6/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2023-07-07 04:26:29.000000 quantplay-1.3.6/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2023-07-07 04:26:29.202858 quantplay-1.3.6/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      875 2023-07-07 04:26:12.000000 quantplay-1.3.6/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.201411 quantplay-1.3.6/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.3.6/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.201714 quantplay-1.3.6/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.3.6/test/broker/finvasia.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.201961 quantplay-1.3.6/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.3.6/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-07-07 04:26:29.202391 quantplay-1.3.6/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.3.6/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.3.6/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.3.6/test/strategy/sample_strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.3.6/test/test_motilal.py
```

### Comparing `quantplay-1.3.5/PKG-INFO` & `quantplay-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.3.5
+Version: 1.3.6
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.3.5/quantplay/backtest/backtest_trades.py` & `quantplay-1.3.6/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/angelone.py` & `quantplay-1.3.6/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/broker_client.py` & `quantplay-1.3.6/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.3.6/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/generics/broker.py` & `quantplay-1.3.6/quantplay/broker/generics/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             trade_price = copy.deepcopy(price)
         try:
             if stoploss != None:
                 if transaction_type == "SELL":
                     sl_transaction_type = "BUY"
                     sl_trigger_price = self.round_to_tick(price * (1 + stoploss))
 
-                    if exchange == self.nfo_exchange:
+                    if exchange == "NFO":
                         price = sl_trigger_price * 1.05
                     elif exchange == "NSE":
                         price = sl_trigger_price * 1.01
                     else:
                         raise Exception("{} not supported for trading".format(exchange))
 
                     sl_price = self.round_to_tick(price)
```

### Comparing `quantplay-1.3.5/quantplay/broker/iifl.py` & `quantplay-1.3.6/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/iifl_xts.py` & `quantplay-1.3.6/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/kite_utils.py` & `quantplay-1.3.6/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/motilal.py` & `quantplay-1.3.6/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/shoonya.py` & `quantplay-1.3.6/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/symphony.py` & `quantplay-1.3.6/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/xts.py` & `quantplay-1.3.6/quantplay/broker/xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.3.6/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.3.6/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.3.6/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.3.6/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/broker/zerodha.py` & `quantplay-1.3.6/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.3.6/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/brokerage/generics/broker.py` & `quantplay-1.3.6/quantplay/brokerage/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.3.6/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/config/qplay_config.py` & `quantplay-1.3.6/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/create_sample_data.py` & `quantplay-1.3.6/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/data_modify_script.py` & `quantplay-1.3.6/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/date_fix.py` & `quantplay-1.3.6/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/exception/exceptions.py` & `quantplay-1.3.6/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/executor/strategy_executor.py` & `quantplay-1.3.6/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/indicators/Indicator.py` & `quantplay-1.3.6/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/model/exchange/instrument.py` & `quantplay-1.3.6/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/model/exchange/order.py` & `quantplay-1.3.6/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/model/exchange/tick.py` & `quantplay-1.3.6/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.3.6/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/order_execution/mean_price.py` & `quantplay-1.3.6/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/reporting/strategy_report.py` & `quantplay-1.3.6/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/reporting/visuals.py` & `quantplay-1.3.6/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/services/market.py` & `quantplay-1.3.6/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/services/tradelens.py` & `quantplay-1.3.6/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.3.6/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.3.6/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/strategy/base.py` & `quantplay-1.3.6/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/utils/config_util.py` & `quantplay-1.3.6/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/utils/constant.py` & `quantplay-1.3.6/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/utils/data_utils.py` & `quantplay-1.3.6/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/utils/exchange.py` & `quantplay-1.3.6/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/utils/number_utils.py` & `quantplay-1.3.6/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/utils/selenium_utils.py` & `quantplay-1.3.6/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay/utils/transaction_utils.py` & `quantplay-1.3.6/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/quantplay.egg-info/PKG-INFO` & `quantplay-1.3.6/quantplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.3.5
+Version: 1.3.6
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.3.5/quantplay.egg-info/SOURCES.txt` & `quantplay-1.3.6/quantplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/setup.py` & `quantplay-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.3.5",
+    version="1.3.6",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.3.5/test/strategy/sample_strategy.py` & `quantplay-1.3.6/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.3.5/test/test_motilal.py` & `quantplay-1.3.6/test/test_motilal.py`

 * *Files identical despite different names*

