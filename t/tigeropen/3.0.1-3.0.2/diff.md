# Comparing `tmp/tigeropen-3.0.1.tar.gz` & `tmp/tigeropen-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-3.0.1.tar", last modified: Wed Jun 21 08:37:36 2023, max compression
+gzip compressed data, was "tigeropen-3.0.2.tar", last modified: Fri Jul  7 11:36:51 2023, max compression
```

## Comparing `tigeropen-3.0.1.tar` & `tigeropen-3.0.2.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.710766 tigeropen-3.0.1/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.0.1/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-21 08:37:36.710644 tigeropen-3.0.1/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.0.1/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-3.0.1/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2023-06-21 08:37:36.710808 tigeropen-3.0.1/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-3.0.1/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.676767 tigeropen-3.0.1/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.679105 tigeropen-3.0.1/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.681128 tigeropen-3.0.1/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     5080 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.0.1/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     3037 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      654 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.683318 tigeropen-3.0.1/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-3.0.1/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     7461 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-3.0.1/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.0.1/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.684438 tigeropen-3.0.1/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.684798 tigeropen-3.0.1/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)    11145 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8386 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.684938 tigeropen-3.0.1/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.685068 tigeropen-3.0.1/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.685323 tigeropen-3.0.1/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.686249 tigeropen-3.0.1/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.0.1/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.0.1/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.0.1/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.686938 tigeropen-3.0.1/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.688196 tigeropen-3.0.1/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-06-01 06:23:56.000000 tigeropen-3.0.1/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.697724 tigeropen-3.0.1/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1238 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/OptionTopData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2473 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/OptionTopData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3823 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/OptionTopData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-3.0.1/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1008 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3832 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3637 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2303 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4814 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1855 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      765 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2104 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1551 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      411 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/StockTopData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1631 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/StockTopData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1720 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/StockTopData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-16 04:01:58.000000 tigeropen-3.0.1/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-3.0.1/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.0.1/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/push/pb/trade_tick.py
--rw-r--r--   0 sukai      (501) staff       (20)     9068 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    17538 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     9122 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    28235 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.698082 tigeropen-3.0.1/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.699907 tigeropen-3.0.1/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    77859 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.700307 tigeropen-3.0.1/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    34187 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.706461 tigeropen-3.0.1/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.0.1/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.0.1/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1746 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.0.1/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      706 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/kline_quota_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-06-07 11:40:19.000000 tigeropen-3.0.1/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1599 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2469 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2730 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2410 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_timeline_history_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.0.1/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4898 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-3.0.1/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-3.0.1/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-3.0.1/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11281 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-3.0.1/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.706749 tigeropen-3.0.1/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.708066 tigeropen-3.0.1/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     6154 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)    10103 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2704 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.708375 tigeropen-3.0.1/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.1/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    32808 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.710415 tigeropen-3.0.1/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.0.1/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1120 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      949 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4426 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1528 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1166 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1278 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     7367 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6199 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.0.1/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-3.0.1/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1413 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    40527 2023-06-21 08:36:53.000000 tigeropen-3.0.1/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-21 08:37:36.678084 tigeropen-3.0.1/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     7672 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      130 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2023-06-21 08:37:36.000000 tigeropen-3.0.1/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.077412 tigeropen-3.0.2/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.0.2/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-07-07 11:36:51.077215 tigeropen-3.0.2/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.0.2/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-3.0.2/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2023-07-07 11:36:51.077455 tigeropen-3.0.2/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-3.0.2/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.040940 tigeropen-3.0.2/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2023-07-07 11:36:44.000000 tigeropen-3.0.2/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.043155 tigeropen-3.0.2/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.045193 tigeropen-3.0.2/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     5080 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-06-07 11:40:19.000000 tigeropen-3.0.2/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.0.2/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.0.2/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3037 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      654 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.046984 tigeropen-3.0.2/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-3.0.2/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7461 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-3.0.2/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.0.2/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-3.0.2/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.048034 tigeropen-3.0.2/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.048373 tigeropen-3.0.2/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11145 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-3.0.2/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8386 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.048496 tigeropen-3.0.2/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.2/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.048626 tigeropen-3.0.2/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.2/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.048874 tigeropen-3.0.2/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.0.2/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.049864 tigeropen-3.0.2/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.0.2/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.0.2/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.0.2/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.0.2/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.050698 tigeropen-3.0.2/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.052332 tigeropen-3.0.2/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-07 11:40:19.000000 tigeropen-3.0.2/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-07-07 11:28:06.000000 tigeropen-3.0.2/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.062636 tigeropen-3.0.2/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1238 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/OptionTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2473 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/OptionTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3823 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/OptionTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-07 11:40:19.000000 tigeropen-3.0.2/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-3.0.2/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1008 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3832 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3637 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2303 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4814 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1855 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      765 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2104 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1551 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/StockTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1631 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/StockTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1720 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/StockTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-16 04:01:58.000000 tigeropen-3.0.2/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-3.0.2/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.0.2/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-07 11:40:19.000000 tigeropen-3.0.2/tigeropen/push/pb/trade_tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9068 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    17678 2023-07-07 11:36:44.000000 tigeropen-3.0.2/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9122 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    28235 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.062941 tigeropen-3.0.2/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.064727 tigeropen-3.0.2/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-06-07 11:40:19.000000 tigeropen-3.0.2/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    78040 2023-07-07 11:36:44.000000 tigeropen-3.0.2/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.065065 tigeropen-3.0.2/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    34438 2023-07-07 11:36:44.000000 tigeropen-3.0.2/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.072144 tigeropen-3.0.2/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.0.2/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.0.2/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1746 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.0.2/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      706 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/quote/response/kline_quota_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-06-07 11:40:19.000000 tigeropen-3.0.2/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.0.2/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1599 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2469 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2730 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2410 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_timeline_history_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.0.2/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-3.0.2/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.0.2/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4898 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-3.0.2/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-3.0.2/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-3.0.2/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11281 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-3.0.2/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.072464 tigeropen-3.0.2/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.073934 tigeropen-3.0.2/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-3.0.2/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6154 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)    10103 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2704 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-3.0.2/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.074323 tigeropen-3.0.2/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.0.2/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    32808 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.076887 tigeropen-3.0.2/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.0.2/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1120 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      949 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4426 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1528 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-3.0.2/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1166 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1278 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7367 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6199 2023-06-29 06:23:53.000000 tigeropen-3.0.2/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.0.2/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-3.0.2/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1413 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    40527 2023-06-21 08:36:53.000000 tigeropen-3.0.2/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-07-07 11:36:51.041977 tigeropen-3.0.2/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-07-07 11:36:50.000000 tigeropen-3.0.2/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     7672 2023-07-07 11:36:51.000000 tigeropen-3.0.2/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2023-07-07 11:36:50.000000 tigeropen-3.0.2/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      130 2023-07-07 11:36:50.000000 tigeropen-3.0.2/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2023-07-07 11:36:50.000000 tigeropen-3.0.2/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-3.0.1/PKG-INFO` & `tigeropen-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.0.1
+Version: 3.0.2
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.0.1/README.md` & `tigeropen-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/setup.py` & `tigeropen-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/consts/__init__.py` & `tigeropen-3.0.2/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/consts/filter_fields.py` & `tigeropen-3.0.2/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-3.0.2/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/consts/params.py` & `tigeropen-3.0.2/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/consts/push_types.py` & `tigeropen-3.0.2/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/consts/quote_keys.py` & `tigeropen-3.0.2/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/consts/service_types.py` & `tigeropen-3.0.2/tigeropen/common/consts/service_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/consts/tick_constants.py` & `tigeropen-3.0.2/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/model.py` & `tigeropen-3.0.2/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/request.py` & `tigeropen-3.0.2/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/response.py` & `tigeropen-3.0.2/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/util/common_utils.py` & `tigeropen-3.0.2/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/util/contract_utils.py` & `tigeropen-3.0.2/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/util/order_utils.py` & `tigeropen-3.0.2/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/util/price_util.py` & `tigeropen-3.0.2/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/util/signature_utils.py` & `tigeropen-3.0.2/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/util/string_utils.py` & `tigeropen-3.0.2/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/util/tick_util.py` & `tigeropen-3.0.2/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/common/util/web_utils.py` & `tigeropen-3.0.2/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/examples/client_config.py` & `tigeropen-3.0.2/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/examples/nasdaq100.py` & `tigeropen-3.0.2/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-3.0.2/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/examples/push_client_demo.py` & `tigeropen-3.0.2/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-3.0.2/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/examples/quote_client_demo.py` & `tigeropen-3.0.2/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/examples/trade_client_demo.py` & `tigeropen-3.0.2/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/fundamental/request/model.py` & `tigeropen-3.0.2/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-3.0.2/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-3.0.2/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-3.0.2/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-3.0.2/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-3.0.2/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/fundamental/response/industry_response.py` & `tigeropen-3.0.2/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/__init__.py` & `tigeropen-3.0.2/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/network/connect.py` & `tigeropen-3.0.2/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/network/exception.py` & `tigeropen-3.0.2/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/network/listener.py` & `tigeropen-3.0.2/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/network/protocal.py` & `tigeropen-3.0.2/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/network/transport.py` & `tigeropen-3.0.2/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/network/utils.py` & `tigeropen-3.0.2/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/AssetData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OptionTopData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/OptionTopData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OptionTopData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/OptionTopData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OptionTopData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/OptionTopData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/PositionData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/PushData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/Request.proto` & `tigeropen-3.0.2/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/Request_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/Response_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-3.0.2/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/StockTopData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/StockTopData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/StockTopData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/StockTopData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-3.0.2/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-3.0.2/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-3.0.2/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/trade_tick.py` & `tigeropen-3.0.2/tigeropen/push/pb/trade_tick.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/pb/util.py` & `tigeropen-3.0.2/tigeropen/push/pb/util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/protobuf_push_client.py` & `tigeropen-3.0.2/tigeropen/push/protobuf_push_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,20 @@
 
     def on_disconnected(self):
         if self.disconnect_callback:
             self.disconnect_callback()
         else:
             self._connect()
 
+    def on_disconnecting(self):
+        self.on_disconnected()
+
+    def on_heartbeat(self, frame):
+        self.logger.debug('heart-beat')
+
     def on_error(self, frame):
         self.logger.error(frame)
 
     def on_message(self, frame):
         if frame.code == ResponseType.GET_SUB_SYMBOLS_END.value:
             if self.query_subscribed_callback:
                 self.query_subscribed_callback(frame.msg)
```

### Comparing `tigeropen-3.0.1/tigeropen/push/push_client.py` & `tigeropen-3.0.2/tigeropen/push/push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/push/stomp_push_client.py` & `tigeropen-3.0.2/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/domain/filter.py` & `tigeropen-3.0.2/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/domain/quote_brief.py` & `tigeropen-3.0.2/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/domain/stock_broker.py` & `tigeropen-3.0.2/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/quote_client.py` & `tigeropen-3.0.2/tigeropen/quote/quote_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -737,24 +737,26 @@
             if response.is_success():
                 return response.briefs
             else:
                 raise ApiException(response.code, response.message)
 
         return None
 
-    def get_option_bars(self, identifiers, begin_time=-1, end_time=4070880000000, period=BarPeriod.DAY, limit=None):
+    def get_option_bars(self, identifiers, begin_time=-1, end_time=4070880000000, period=BarPeriod.DAY, limit=None,
+                        sort_dir=None):
         """
         获取期权日K数据
         :param identifiers: 期权代码列表
         :param begin_time: 开始时间. 若是时间戳需要精确到毫秒, 为13位整数;
                                     或是日期时间格式的字符串, 如 "2019-01-01" 或 "2019-01-01 12:00:00"
         :param end_time: 结束时间. 格式同 begin_time
         :param period: 时间间隔. 可选值: DAY("day"), ONE_MINUTE("1min"), FIVE_MINUTES("5min"), HALF_HOUR("30min"),
             ONE_HOUR("60min");
         :param limit: 每个期权的返回k线数量
+        :param sort_dir: tigeropen.common.consts.SortDirection, e.g. SortDirection.DESC
         :return: pandas.DataFrame, 各 column 含义如下：
             time: 毫秒级时间戳
             open: 开盘价
             high: 最高价
             low: 最低价
             close: 收盘价
             volume: 成交量
@@ -774,14 +776,15 @@
             param.expiry = date_str_to_timestamp(expiry, self._timezone)
             param.put_call = put_call
             param.strike = strike
             param.period = get_enum_value(period)
             param.begin_time = date_str_to_timestamp(begin_time, self._timezone)
             param.end_time = date_str_to_timestamp(end_time, self._timezone)
             param.limit = limit
+            param.sort_dir = get_enum_value(sort_dir)
             contracts.append(param)
         params.contracts = contracts
         request = OpenApiRequest(OPTION_KLINE, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = OptionQuoteBarResponse()
             response.parse_response_content(response_content)
```

### Comparing `tigeropen-3.0.1/tigeropen/quote/request/model.py` & `tigeropen-3.0.2/tigeropen/quote/request/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,14 +446,15 @@
 class SingleOptionQuoteParams(SingleContractParams):
     def __init__(self):
         super(SingleOptionQuoteParams, self).__init__()
         self._period = None
         self._begin_time = None
         self._end_time = None
         self._limit = None
+        self._sort_dir = None
 
     @property
     def period(self):
         return self._period
 
     @period.setter
     def period(self, value):
@@ -479,29 +480,34 @@
     def limit(self):
         return self._limit
 
     @limit.setter
     def limit(self, value):
         self._limit = value
 
+    @property
+    def sort_dir(self):
+        return self._sort_dir
+
+    @sort_dir.setter
+    def sort_dir(self, value):
+        self._sort_dir = value
+
     def to_openapi_dict(self):
         params = super(SingleOptionQuoteParams, self).to_openapi_dict()
-
         if self.period:
             params['period'] = self.period
-
         if self.begin_time:
             params['begin_time'] = self.begin_time
-
         if self.end_time:
             params['end_time'] = self.end_time
-
         if self.limit:
             params['limit'] = self.limit
-
+        if self.sort_dir:
+            params['sort_dir'] = self.sort_dir
         return params
 
 
 class MultipleContractParams(BaseParams):
     def __init__(self):
         super(MultipleContractParams, self).__init__()
         self._contracts = None  # list of SingleQuoteParams
```

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/future_contract_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/kline_quota_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/kline_quota_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/market_status_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/option_chains_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_timeline_history_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_timeline_history_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/stock_details_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/symbols_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-3.0.2/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/tiger_open_client.py` & `tigeropen-3.0.2/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/tiger_open_config.py` & `tigeropen-3.0.2/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/domain/account.py` & `tigeropen-3.0.2/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/domain/contract.py` & `tigeropen-3.0.2/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/domain/order.py` & `tigeropen-3.0.2/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/domain/position.py` & `tigeropen-3.0.2/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/domain/prime_account.py` & `tigeropen-3.0.2/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/request/model.py` & `tigeropen-3.0.2/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/__init__.py` & `tigeropen-3.0.2/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/account_profile_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/assets_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/contracts_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/forex_order_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/order_id_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/order_preview_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/orders_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/orders_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/positions_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/positions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/response/transactions_response.py` & `tigeropen-3.0.2/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen/trade/trade_client.py` & `tigeropen-3.0.2/tigeropen/trade/trade_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.0.1/tigeropen.egg-info/PKG-INFO` & `tigeropen-3.0.2/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.0.1
+Version: 3.0.2
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.0.1/tigeropen.egg-info/SOURCES.txt` & `tigeropen-3.0.2/tigeropen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

