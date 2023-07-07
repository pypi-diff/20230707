# Comparing `tmp/rqalpha-5.1.0.tar.gz` & `tmp/rqalpha-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-vb2rqxte/rqalpha-5.1.0.tar", last modified: Fri Jun 16 08:08:38 2023, max compression
+gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-rp8_a7qx/rqalpha-5.1.1.tar", last modified: Fri Jul  7 06:30:29 2023, max compression
```

## Comparing `rqalpha-5.1.0.tar` & `rqalpha-5.1.1.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    61279 2023-06-16 08:08:28.000000 rqalpha-5.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-16 08:08:28.000000 rqalpha-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 08:08:28.000000 rqalpha-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 08:08:38.000000 rqalpha-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-06-16 08:08:28.000000 rqalpha-5.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/api_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    59090 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/api_rqdatac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/global_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/strategy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/strategy_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/strategy_universe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/bar_dict_price_board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/storage_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/storages.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/data_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/trading_dates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/IF1706_20161108.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/IF_macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/examples/data_source/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/data_source/get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/data_source/import_get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/data_source/read_csv_as_df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/examples/extend_api/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/extend_api/test_extend_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/golden_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/pair_trading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/rsi.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/run_code_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/run_file_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/run_func_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/subscribe_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/test_pt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)    21124 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
--rw-r--r--   0 runner    (1001) docker     (123)    34687 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/portfolio/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/portfolio/position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/resource/
--rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/resource/ricequant-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/user_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/class_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/click_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/datetime_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/dict_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/package_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/persisit_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/risk_free_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/rq_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/strategy_loader_help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/testing/mocking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    51160 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-16 08:08:38.000000 rqalpha-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-16 08:08:28.000000 rqalpha-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_position_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_management_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/test_api_future.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/test_api_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_f_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_f_macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_f_macd_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_f_mean_reverting.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_dual_thrust.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_turtle_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_sf_buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/unittest/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/unittest/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_data/test_instrument_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_data/test_trading_dates_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/unittest/test_mod/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79879 2023-06-16 08:08:28.000000 rqalpha-5.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    61336 2023-07-07 06:30:19.000000 rqalpha-5.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-07 06:30:19.000000 rqalpha-5.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-07 06:30:19.000000 rqalpha-5.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 06:30:29.000000 rqalpha-5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-07-07 06:30:19.000000 rqalpha-5.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21928 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/api_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59090 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/api_rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/apis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/cmds/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/global_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/strategy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/strategy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/core/strategy_universe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/bar_dict_price_board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/storage_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/base_data_source/storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/data_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/data/trading_dates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/IF1706_20161108.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/IF_macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/examples/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/data_source/get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/data_source/import_get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/data_source/read_csv_as_df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/examples/extend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/extend_api/test_extend_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/golden_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/pair_trading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/run_code_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/run_file_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/run_func_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/subscribe_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/test_pt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/examples/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21124 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34434 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/mod_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/model/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/portfolio/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/portfolio/position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/resource/ricequant-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/user_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/class_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/click_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/datetime_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/dict_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/package_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/persisit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/risk_free_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/rq_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/strategy_loader_help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/testing/mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    51160 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-07 06:30:19.000000 rqalpha-5.1.1/rqalpha/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 06:30:28.000000 rqalpha-5.1.1/rqalpha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 06:30:29.000000 rqalpha-5.1.1/rqalpha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 06:30:29.000000 rqalpha-5.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-07 06:30:19.000000 rqalpha-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_position_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/test_physical_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_management_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/test_api_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/test_api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/api_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_f_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_f_macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_f_macd_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_f_mean_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_dual_thrust.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_s_turtle_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/test_sf_buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/unittest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/unittest/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_data/test_instrument_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_data/test_trading_dates_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/unittest/test_mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 06:30:29.000000 rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-07 06:30:19.000000 rqalpha-5.1.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79879 2023-07-07 06:30:19.000000 rqalpha-5.1.1/versioneer.py
```

### Comparing `rqalpha-5.1.0/CHANGELOG.rst` & `rqalpha-5.1.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ==================
 CHANGELOG
 ==================
 
+5.1.1
+==================
+- 调整API参数;更新文档
+
 5.1.0
 ==================
 - 新增个股权重检测, summary报告中新增了表格
 - 新增api futures.get_dominant_price,支持动态复权
 - 修复pandas1.5.0以下无法产生report
 - 修复在日内回转交易时trading_pnl计算错误
```

### Comparing `rqalpha-5.1.0/LICENSE` & `rqalpha-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/README.rst` & `rqalpha-5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/__init__.py` & `rqalpha-5.1.1/rqalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/__main__.py` & `rqalpha-5.1.1/rqalpha/__main__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/api.py` & `rqalpha-5.1.1/rqalpha/api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/apis/__init__.py` & `rqalpha-5.1.1/rqalpha/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/apis/api_abstract.py` & `rqalpha-5.1.1/rqalpha/apis/api_abstract.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 
 common_rules = (
     verify_that('price', pre_check=True).deprecated("please use price_or_style instead.").is_greater_than(0),
     verify_that('style', pre_check=True).deprecated("please use price_or_style instead.").is_instance_of(
         (*ALL_ORDER_STYPES, type(None))
     ),
-    verify_that("price_or_style", pre_check=True).is_instance_of((float, type(None), tuple, *ALL_ORDER_STYPES)),
+    verify_that("price_or_style", pre_check=True).is_instance_of((int, float, type(None), tuple, *ALL_ORDER_STYPES)),
 )
 
 
-PRICE_OR_STYLE_TYPE = Union[float, OrderStyle, None]
+PRICE_OR_STYLE_TYPE = Union[int, float, OrderStyle, None]
 TUPLE_PRICE_OR_STYLE_TYPE = Union[
     float, OrderStyle, None, Tuple, Tuple[PRICE_OR_STYLE_TYPE], Tuple[PRICE_OR_STYLE_TYPE, PRICE_OR_STYLE_TYPE]
 ]
 
 
 @export_as_api
 @ExecutionContext.enforce_phase(
@@ -50,23 +50,21 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount').is_number(),
     *common_rules
 )
 @instype_singledispatch
-def order_shares(id_or_ins, amount, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Optional[Order]
+def order_shares(id_or_ins, amount, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> Optional[Order]
     """
     指定股数的买/卖单，最常见的落单方式之一。如有需要落单类型当做一个参量传入，如果忽略掉落单类型，那么默认是市价单（market order）。
 
     :param id_or_ins: 下单标的物
     :param amount: 下单量, 正数代表买入，负数代表卖出。将会根据一手xx股来向下调整到一手的倍数，比如中国A股就是调整成100股的倍数。
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
@@ -93,28 +91,26 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('cash_amount').is_number(),
     *common_rules
 )
 @instype_singledispatch
-def order_value(id_or_ins, cash_amount, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Optional[Order]
+def order_value(id_or_ins, cash_amount, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], float, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> Optional[Order]
     """
     使用想要花费的金钱买入/卖出股票，而不是买入/卖出想要的股数，正数代表买入，负数代表卖出。股票的股数总是会被调整成对应的100的倍数（在A中国A股市场1手是100股）。
     如果资金不足，该API将会使用最大可用资金发单。
 
     需要注意：
     当您提交一个买单时，cash_amount 代表的含义是您希望买入股票消耗的金额（包含税费），最终买入的股数不仅和发单的价格有关，还和税费相关的参数设置有关。
     当您提交一个卖单时，cash_amount 代表的意义是您希望卖出股票的总价值。如果金额超出了您所持有股票的价值，那么您将卖出所有股票。
 
     :param id_or_ins: 下单标的物
     :param cash_amount: 需要花费现金购买/卖出证券的数目。正数代表买入，负数代表卖出。
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
@@ -135,28 +131,26 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('percent', pre_check=True).is_number().is_greater_or_equal_than(-1).is_less_or_equal_than(1),
     *common_rules
 )
 @instype_singledispatch
-def order_percent(id_or_ins, percent, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Optional[Order]
+def order_percent(id_or_ins, percent, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], float, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> Optional[Order]
     """
     发送一个花费价值等于目前投资组合（市场价值和目前现金的总和）一定百分比现金的买/卖单，正数代表买，负数代表卖。股票的股数总是会被调整成对应的一手的股票数的倍数（1手是100股）。百分比是一个小数，并且小于或等于1（<=100%），0.5表示的是50%.需要注意，如果资金不足，该API将会使用最大可用资金发单。
 
     需要注意：
 
     发送买单时，percent 代表的是期望买入股票消耗的金额（包含税费）占投资组合总权益的比例。
     发送卖单时，percent 代表的是期望卖出的股票总价值占投资组合总权益的比例。
 
     :param id_or_ins: 下单标的物
     :param percent: 占有现有的投资组合价值的百分比。正数表示买入，负数表示卖出。
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
@@ -177,27 +171,25 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('cash_amount').is_number(),
     *common_rules
 )
 @instype_singledispatch
-def order_target_value(id_or_ins, cash_amount, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], TUPLE_PRICE_OR_STYLE_TYPE) -> Optional[Order]
+def order_target_value(id_or_ins, cash_amount, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], float, TUPLE_PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> Optional[Order]
     """
     买入/卖出并且自动调整该证券的仓位到一个目标价值。
     加仓时，cash_amount 代表现有持仓的价值加上即将花费（包含税费）的现金的总价值。
     减仓时，cash_amount 代表调整仓位的目标价至。
 
     需要注意，如果资金不足，该API将会使用最大可用资金发单。
 
     :param id_or_ins: 下单标的物
     :param cash_amount: 最终的该证券的仓位目标价值。
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
@@ -219,16 +211,16 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('percent', pre_check=True).is_number().is_greater_or_equal_than(0).is_less_or_equal_than(1),
     *common_rules
 )
 @instype_singledispatch
-def order_target_percent(id_or_ins, percent, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], TUPLE_PRICE_OR_STYLE_TYPE) -> Optional[Order]
+def order_target_percent(id_or_ins, percent, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], float, TUPLE_PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> Optional[Order]
     """
     买入/卖出证券以自动调整该证券的仓位到占有一个目标价值。
 
     加仓时，percent 代表证券已有持仓的价值加上即将花费的现金（包含税费）的总值占当前投资组合总价值的比例。
     减仓时，percent 代表证券将被调整到的目标价至占当前投资组合总价值的比例。
 
     其实我们需要计算一个position_to_adjust (即应该调整的仓位)
@@ -239,16 +231,14 @@
 
     如果 position_to_adjust 计算之后是正的，那么会买入该证券，否则会卖出该证券。需要注意，如果需要买入证券而资金不足，该 API 将使用最大可用资金发出订单。
 
     另外，如果您希望大量调整股票仓位，推荐使用 order_target_portfolio 而非在循环中调取 order_target_percent，前者将拥有更好的性能。
 
     :param id_or_ins: 下单标的物
     :param percent: 仓位最终所占投资组合总价值的目标百分比。
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
@@ -270,23 +260,21 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount', pre_check=True).is_number().is_greater_or_equal_than(0),
     *common_rules
 )
 @instype_singledispatch
-def buy_open(id_or_ins, amount, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Union[Order, List[Order], None]
+def buy_open(id_or_ins, amount, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> Union[Order, List[Order], None]
     """
     买入开仓。
 
     :param id_or_ins: 下单标的物
     :param amount: 下单手数
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
@@ -305,26 +293,24 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount', pre_check=True).is_number().is_greater_or_equal_than(0),
     *common_rules
 )
 @instype_singledispatch
-def buy_close(id_or_ins, amount, price=None, style=None, price_or_style=None, close_today=False):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE, Optional[bool]) -> Union[Order, List[Order], None]
+def buy_close(id_or_ins, amount, price_or_style=None, price=None, style=None, close_today=False):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle], Optional[bool]) -> Union[Order, List[Order], None]
     """
     平卖仓
 
     :param id_or_ins: 下单标的物
     :param amount: 下单手数
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
-    :param close_today: 是否指定发平今仓单，默认为False，发送平仓单
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
+    :param close_today: 是否指定发平今仓单，默认为False，发送平仓单
 
     :example:
 
     .. code-block:: python
 
         #市价单将现有IF1603空仓买入平仓2张：
         buy_close('IF1603', 2)
@@ -341,23 +327,21 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount', pre_check=True).is_number().is_greater_or_equal_than(0),
     *common_rules
 )
 @instype_singledispatch
-def sell_open(id_or_ins, amount, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Union[Order, List[Order], None]
+def sell_open(id_or_ins, amount, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> Union[Order, List[Order], None]
     """
     卖出开仓
 
     :param id_or_ins: 下单标的物
     :param amount: 下单手数
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
@@ -377,23 +361,21 @@
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(
     verify_that('amount', pre_check=True).is_number().is_greater_or_equal_than(0),
     *common_rules
 )
 @instype_singledispatch
-def sell_close(id_or_ins, amount, price=None, style=None, price_or_style=None, close_today=False):
-    # type: (Union[str, Instrument], float, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE, Optional[bool]) -> Union[Order, List[Order], None]
+def sell_close(id_or_ins, amount, price_or_style=None, price=None, style=None, close_today=False):
+    # type: (Union[str, Instrument], float, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle], Optional[bool]) -> Union[Order, List[Order], None]
     """
     平买仓
 
     :param id_or_ins: 下单标的物
     :param amount: 下单手数
-    :param price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param close_today: 是否指定发平今仓单，默认为False，发送平仓单
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
@@ -405,16 +387,16 @@
     """
     raise NotImplementedError
 
 
 @export_as_api
 @apply_rules(verify_that("quantity").is_number(), *common_rules)
 @instype_singledispatch
-def order(order_book_id, quantity, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> List[Order]
+def order(order_book_id, quantity, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> List[Order]
     """
       全品种通用智能调仓函数
 
       如果不指定 price, 则相当于下 MarketOrder
 
       如果 order_book_id 是股票，等同于调用 order_shares
 
@@ -422,16 +404,14 @@
 
           *   quantity 表示调仓量
           *   如果 quantity 为正数，则先平 Sell 方向仓位，再开 Buy 方向仓位
           *   如果 quantity 为负数，则先平 Buy 反向仓位，再开 Sell 方向仓位
 
       :param order_book_id: 下单标的物
       :param quantity: 调仓量
-      :param price: 下单价格
-      :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
       :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
       :example:
 
       ..  code-block:: python3
           :linenos:
@@ -446,16 +426,16 @@
     """
     raise NotImplementedError
 
 
 @export_as_api
 @apply_rules(verify_that("quantity").is_number(), *common_rules)
 @instype_singledispatch
-def order_to(order_book_id, quantity, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> List[Order]
+def order_to(order_book_id, quantity, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> List[Order]
     """
     全品种通用智能调仓函数
 
     如果不指定 price, 则相当于 MarketOrder
 
     如果 order_book_id 是股票，则表示仓位调整到多少股
 
@@ -463,16 +443,14 @@
 
         *   quantity 表示调整至某个仓位
         *   quantity 如果为正数，则先平 SELL 方向仓位，再 BUY 方向开仓 quantity 手
         *   quantity 如果为负数，则先平 BUY 方向仓位，再 SELL 方向开仓 -quantity 手
 
     :param order_book_id: 下单标的物
     :param int quantity: 调仓量
-    :param float price: 下单价格
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     ..  code-block:: python3
         :linenos:
```

### Comparing `rqalpha-5.1.0/rqalpha/apis/api_base.py` & `rqalpha-5.1.1/rqalpha/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/apis/api_rqdatac.py` & `rqalpha-5.1.1/rqalpha/apis/api_rqdatac.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/apis/names.py` & `rqalpha-5.1.1/rqalpha/apis/names.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/cmds/__init__.py` & `rqalpha-5.1.1/rqalpha/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/cmds/bundle.py` & `rqalpha-5.1.1/rqalpha/cmds/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/cmds/entry.py` & `rqalpha-5.1.1/rqalpha/cmds/entry.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/cmds/misc.py` & `rqalpha-5.1.1/rqalpha/cmds/misc.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/cmds/mod.py` & `rqalpha-5.1.1/rqalpha/cmds/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/cmds/run.py` & `rqalpha-5.1.1/rqalpha/cmds/run.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/config.yml` & `rqalpha-5.1.1/rqalpha/config.yml`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/const.py` & `rqalpha-5.1.1/rqalpha/const.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/__init__.py` & `rqalpha-5.1.1/rqalpha/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/events.py` & `rqalpha-5.1.1/rqalpha/core/events.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/execution_context.py` & `rqalpha-5.1.1/rqalpha/core/execution_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/executor.py` & `rqalpha-5.1.1/rqalpha/core/executor.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/global_var.py` & `rqalpha-5.1.1/rqalpha/core/global_var.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/strategy.py` & `rqalpha-5.1.1/rqalpha/core/strategy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/strategy_context.py` & `rqalpha-5.1.1/rqalpha/core/strategy_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/strategy_loader.py` & `rqalpha-5.1.1/rqalpha/core/strategy_loader.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/core/strategy_universe.py` & `rqalpha-5.1.1/rqalpha/core/strategy_universe.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/__init__.py` & `rqalpha-5.1.1/rqalpha/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/bar_dict_price_board.py` & `rqalpha-5.1.1/rqalpha/data/bar_dict_price_board.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/base_data_source/__init__.py` & `rqalpha-5.1.1/rqalpha/data/base_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/base_data_source/adjust.py` & `rqalpha-5.1.1/rqalpha/data/base_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/base_data_source/data_source.py` & `rqalpha-5.1.1/rqalpha/data/base_data_source/data_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/base_data_source/storage_interface.py` & `rqalpha-5.1.1/rqalpha/data/base_data_source/storage_interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/base_data_source/storages.py` & `rqalpha-5.1.1/rqalpha/data/base_data_source/storages.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/bundle.py` & `rqalpha-5.1.1/rqalpha/data/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/data_proxy.py` & `rqalpha-5.1.1/rqalpha/data/data_proxy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/data/trading_dates_mixin.py` & `rqalpha-5.1.1/rqalpha/data/trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/environment.py` & `rqalpha-5.1.1/rqalpha/environment.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/IF1706_20161108.csv` & `rqalpha-5.1.1/rqalpha/examples/IF1706_20161108.csv`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/IF_macd.py` & `rqalpha-5.1.1/rqalpha/examples/IF_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/buy_and_hold.py` & `rqalpha-5.1.1/rqalpha/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/data_source/get_csv_module.py` & `rqalpha-5.1.1/rqalpha/examples/data_source/get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/data_source/import_get_csv_module.py` & `rqalpha-5.1.1/rqalpha/examples/data_source/import_get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/data_source/read_csv_as_df.py` & `rqalpha-5.1.1/rqalpha/examples/data_source/read_csv_as_df.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py` & `rqalpha-5.1.1/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/extend_api/test_extend_api.py` & `rqalpha-5.1.1/rqalpha/examples/extend_api/test_extend_api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/golden_cross.py` & `rqalpha-5.1.1/rqalpha/examples/golden_cross.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/macd.py` & `rqalpha-5.1.1/rqalpha/examples/macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/pair_trading.py` & `rqalpha-5.1.1/rqalpha/examples/pair_trading.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/rsi.py` & `rqalpha-5.1.1/rqalpha/examples/rsi.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/run_code_demo.py` & `rqalpha-5.1.1/rqalpha/examples/run_code_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/run_func_demo.py` & `rqalpha-5.1.1/rqalpha/examples/run_func_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/subscribe_event.py` & `rqalpha-5.1.1/rqalpha/examples/subscribe_event.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/test_pt.py` & `rqalpha-5.1.1/rqalpha/examples/test_pt.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/examples/turtle.py` & `rqalpha-5.1.1/rqalpha/examples/turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/interface.py` & `rqalpha-5.1.1/rqalpha/interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/main.py` & `rqalpha-5.1.1/rqalpha/main.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from __future__ import division
 from typing import Union, Optional, List
 
 import numpy as np
 
 from rqalpha.api import export_as_api
 from rqalpha.apis.api_base import assure_instrument
-from rqalpha.apis.api_abstract import order, order_to, buy_open, buy_close, sell_open, sell_close
+from rqalpha.apis.api_abstract import order, order_to, buy_open, buy_close, sell_open, sell_close, PRICE_OR_STYLE_TYPE
 from rqalpha.apis.api_base import cal_style
 from rqalpha.apis.api_rqdatac import futures
 from rqalpha.environment import Environment
 from rqalpha.model.order import Order, LimitOrder, OrderStyle, ALGO_ORDER_STYLES
 from rqalpha.const import SIDE, POSITION_EFFECT, ORDER_TYPE, RUN_TYPE, INSTRUMENT_TYPE, POSITION_DIRECTION
 from rqalpha.model.instrument import Instrument
 from rqalpha.portfolio.position import Position
@@ -170,43 +170,43 @@
         return orders
     # 开仓
     orders.append(_submit_order(order_book_id, quantity, side, POSITION_EFFECT.OPEN, style))
     return orders
 
 
 @order.register(INSTRUMENT_TYPE.FUTURE)
-def future_order(order_book_id, quantity, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], Optional[Union[float, OrderStyle]]) -> List[Order]
+def future_order(order_book_id, quantity, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> List[Order]
     return _order(order_book_id, quantity, cal_style(price, style, price_or_style), False)
 
 
 @order_to.register(INSTRUMENT_TYPE.FUTURE)
-def future_order_to(order_book_id, quantity, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], Optional[Union[float, OrderStyle]]) -> List[Order]
+def future_order_to(order_book_id, quantity, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> List[Order]
     return _order(order_book_id, quantity, cal_style(price, style, price_or_style), True)
 
 
 @buy_open.register(INSTRUMENT_TYPE.FUTURE)
-def future_buy_open(id_or_ins, amount, price=None, style=None, price_or_style=None):
+def future_buy_open(id_or_ins, amount, price_or_style=None, price=None, style=None):
     return _submit_order(id_or_ins, amount, SIDE.BUY, POSITION_EFFECT.OPEN, cal_style(price, style, price_or_style))
 
 
 @buy_close.register(INSTRUMENT_TYPE.FUTURE)
-def future_buy_close(id_or_ins, amount, price=None, style=None, close_today=False, price_or_style=None):
+def future_buy_close(id_or_ins, amount, price_or_style=None, price=None, style=None, close_today=False):
     position_effect = POSITION_EFFECT.CLOSE_TODAY if close_today else POSITION_EFFECT.CLOSE
     return _submit_order(id_or_ins, amount, SIDE.BUY, position_effect, cal_style(price, style, price_or_style))
 
 
 @sell_open.register(INSTRUMENT_TYPE.FUTURE)
-def future_sell_open(id_or_ins, amount, price=None, style=None, price_or_style=None):
+def future_sell_open(id_or_ins, amount, price_or_style=None, price=None, style=None):
     return _submit_order(id_or_ins, amount, SIDE.SELL, POSITION_EFFECT.OPEN, cal_style(price, style, price_or_style))
 
 
 @sell_close.register(INSTRUMENT_TYPE.FUTURE)
-def future_sell_close(id_or_ins, amount, price=None, style=None, close_today=False, price_or_style=None):
+def future_sell_close(id_or_ins, amount, price_or_style=None, price=None, style=None, close_today=False):
     position_effect = POSITION_EFFECT.CLOSE_TODAY if close_today else POSITION_EFFECT.CLOSE
     return _submit_order(id_or_ins, amount, SIDE.SELL, position_effect, cal_style(price, style, price_or_style))
 
 
 @export_as_api
 @apply_rules(verify_that('underlying_symbol').is_instance_of(str))
 def get_future_contracts(underlying_symbol):
```

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,71 +163,71 @@
     if amount < 0:
         amount = max(amount, -position.closable)
 
     return _order_shares(ins, amount, style, position.quantity, auto_switch_order_value=False)
 
 
 @order_shares.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_shares(id_or_ins, amount, price=None, style=None, price_or_style=None):
+def stock_order_shares(id_or_ins, amount, price_or_style=None, price=None, style=None):
     auto_switch_order_value = Environment.get_instance().config.mod.sys_accounts.auto_switch_order_value
     account, position, ins = _get_account_position_ins(id_or_ins)
     return _order_shares(
         assure_instrument(id_or_ins), amount, cal_style(price, style, price_or_style), position.quantity,
         auto_switch_order_value
     )
 
 
 @order_value.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_value(id_or_ins, cash_amount, price=None, style=None, price_or_style=None):
+def stock_order_value(id_or_ins, cash_amount, price_or_style=None, price=None, style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
     return _order_value(account, position, ins, cash_amount, cal_style(price, style, price_or_style))
 
 
 @order_percent.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_percent(id_or_ins, percent, price=None, style=None, price_or_style=None):
+def stock_order_percent(id_or_ins, percent, price_or_style=None, price=None, style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
     return _order_value(account, position, ins, account.total_value * percent, cal_style(price, style, price_or_style))
 
 
 @order_target_value.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_target_value(id_or_ins, cash_amount, price=None, style=None, price_or_style=None):
+def stock_order_target_value(id_or_ins, cash_amount, price_or_style=None, price=None, style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
     open_style, close_style = calc_open_close_style(price, style, price_or_style)
     if cash_amount == 0:
         return _submit_order(
             ins, position.closable, SIDE.SELL, POSITION_EFFECT.CLOSE, close_style, position.quantity, False
         )
     _delta = cash_amount - position.market_value
     _style = open_style if _delta > 0 else close_style
     return _order_value(account, position, ins, _delta, _style)
 
 
 @order_target_percent.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_target_percent(id_or_ins, percent, price=None, style=None, price_or_style=None):
+def stock_order_target_percent(id_or_ins, percent, price_or_style=None, price=None, style=None):
     account, position, ins = _get_account_position_ins(id_or_ins)
     open_style, close_style = calc_open_close_style(price, style, price_or_style)
     if percent == 0:
         return _submit_order(
             ins, position.closable, SIDE.SELL, POSITION_EFFECT.CLOSE, close_style, position.quantity, False
         )
     _delta = account.total_value * percent - position.market_value
     _style = open_style if _delta > 0 else close_style
     return _order_value(account, position, ins, _delta, _style)
 
 
 @order.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order(order_book_id, quantity, price=None, style=None, price_or_style=None):
+def stock_order(order_book_id, quantity, price_or_style=None, price=None, style=None):
     result_order = stock_order_shares(order_book_id, quantity, price, style, price_or_style)
     if result_order:
         return [result_order]
     return []
 
 
 @order_to.register(INST_TYPE_IN_STOCK_ACCOUNT)
-def stock_order_to(order_book_id, quantity, price=None, style=None, price_or_style=None):
+def stock_order_to(order_book_id, quantity, price_or_style=None, price=None, style=None):
     position = Environment.get_instance().portfolio.get_position(order_book_id, POSITION_DIRECTION.LONG)
     open_style, close_style = calc_open_close_style(price, style, price_or_style)
     quantity = quantity - position.quantity
     _style = open_style if quantity > 0 else close_style
     result_order = stock_order_shares(order_book_id, quantity, price, _style, price_or_style)
     if result_order:
         return [result_order]
@@ -239,34 +239,32 @@
     EXECUTION_PHASE.OPEN_AUCTION,
     EXECUTION_PHASE.ON_BAR,
     EXECUTION_PHASE.ON_TICK,
     EXECUTION_PHASE.SCHEDULED,
     EXECUTION_PHASE.GLOBAL
 )
 @apply_rules(verify_that('id_or_ins').is_valid_stock(), verify_that('amount').is_number(), *common_rules)
-def order_lots(id_or_ins, amount, price=None, style=None, price_or_style=None):
-    # type: (Union[str, Instrument], int, Optional[float], Optional[OrderStyle], PRICE_OR_STYLE_TYPE) -> Optional[Order]
+def order_lots(id_or_ins, amount, price_or_style=None, price=None, style=None):
+    # type: (Union[str, Instrument], int, PRICE_OR_STYLE_TYPE, Optional[float], Optional[OrderStyle]) -> Optional[Order]
     """
     指定手数发送买/卖单。如有需要落单类型当做一个参量传入，如果忽略掉落单类型，那么默认是市价单（market order）。
 
     :param id_or_ins: 下单标的物
     :param int amount: 下单量, 正数代表买入，负数代表卖出。将会根据一手xx股来向下调整到一手的倍数，比如中国A股就是调整成100股的倍数。
-    :param float price: 下单价格，默认为None，表示 :class:`~MarketOrder`, 此参数主要用于简化 `style` 参数。
-    :param style: 下单类型, 默认是市价单。目前支持的订单类型有 :class:`~LimitOrder` 和 :class:`~MarketOrder`
     :param price_or_style: 默认为None，表示市价单，可设置价格，表示限价单，也可以直接设置订单类型，有如下选项：MarketOrder、LimitOrder、
                             TWAPOrder、VWAPOrder
 
     :example:
 
     .. code-block:: python
 
         #买入20手的平安银行股票，并且发送市价单：
         order_lots('000001.XSHE', 20)
         #买入10手平安银行股票，并且发送限价单，价格为￥10：
-        order_lots('000001.XSHE', 10, style=LimitOrder(10))
+        order_lots('000001.XSHE', 10, price_or_style=LimitOrder(10))
 
     """
     auto_switch_order_value = Environment.get_instance().config.mod.sys_accounts.auto_switch_order_value
     account, position, ins = _get_account_position_ins(id_or_ins)
     return _order_shares(
         ins, amount * int(ins.round_lot), cal_style(price, style, price_or_style), position.quantity,
         auto_switch_order_value
```

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_progress/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py` & `rqalpha-5.1.1/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/mod/utils.py` & `rqalpha-5.1.1/rqalpha/mod/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/model/__init__.py` & `rqalpha-5.1.1/rqalpha/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/model/bar.py` & `rqalpha-5.1.1/rqalpha/model/bar.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/model/instrument.py` & `rqalpha-5.1.1/rqalpha/model/instrument.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/model/order.py` & `rqalpha-5.1.1/rqalpha/model/order.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/model/tick.py` & `rqalpha-5.1.1/rqalpha/model/tick.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/model/trade.py` & `rqalpha-5.1.1/rqalpha/model/trade.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/portfolio/__init__.py` & `rqalpha-5.1.1/rqalpha/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/portfolio/account.py` & `rqalpha-5.1.1/rqalpha/portfolio/account.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/portfolio/position.py` & `rqalpha-5.1.1/rqalpha/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/resource/ricequant-logo.png` & `rqalpha-5.1.1/rqalpha/resource/ricequant-logo.png`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/user_module.py` & `rqalpha-5.1.1/rqalpha/user_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/__init__.py` & `rqalpha-5.1.1/rqalpha/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/arg_checker.py` & `rqalpha-5.1.1/rqalpha/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/class_helper.py` & `rqalpha-5.1.1/rqalpha/utils/class_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/click_helper.py` & `rqalpha-5.1.1/rqalpha/utils/click_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/concurrent.py` & `rqalpha-5.1.1/rqalpha/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/config.py` & `rqalpha-5.1.1/rqalpha/utils/config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/datetime_func.py` & `rqalpha-5.1.1/rqalpha/utils/datetime_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/dict_func.py` & `rqalpha-5.1.1/rqalpha/utils/dict_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/exception.py` & `rqalpha-5.1.1/rqalpha/utils/exception.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/functools.py` & `rqalpha-5.1.1/rqalpha/utils/functools.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/i18n.py` & `rqalpha-5.1.1/rqalpha/utils/i18n.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/log_capture.py` & `rqalpha-5.1.1/rqalpha/utils/log_capture.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/logger.py` & `rqalpha-5.1.1/rqalpha/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/package_helper.py` & `rqalpha-5.1.1/rqalpha/utils/package_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/persisit_helper.py` & `rqalpha-5.1.1/rqalpha/utils/persisit_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/repr.py` & `rqalpha-5.1.1/rqalpha/utils/repr.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/risk_free_helper.py` & `rqalpha-5.1.1/rqalpha/utils/risk_free_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/rq_json.py` & `rqalpha-5.1.1/rqalpha/utils/rq_json.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/strategy_loader_help.py` & `rqalpha-5.1.1/rqalpha/utils/strategy_loader_help.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/testing/__init__.py` & `rqalpha-5.1.1/rqalpha/utils/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/testing/fixtures.py` & `rqalpha-5.1.1/rqalpha/utils/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/testing/mocking.py` & `rqalpha-5.1.1/rqalpha/utils/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/translations/__init__.py` & `rqalpha-5.1.1/rqalpha/utils/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py` & `rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo` & `rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po` & `rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py` & `rqalpha-5.1.1/rqalpha/utils/translations/zh_Hans_CN/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha/utils/typing.py` & `rqalpha-5.1.1/rqalpha/utils/typing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/rqalpha.egg-info/SOURCES.txt` & `rqalpha-5.1.1/rqalpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/setup.py` & `rqalpha-5.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/__init__.py` & `rqalpha-5.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/__init__.py` & `rqalpha-5.1.1/tests/api_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/__init__.py` & `rqalpha-5.1.1/tests/api_tests/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/__init__.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_account_model.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_account_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_margin_stocks.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_position_models.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_accounts/test_position_models.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/test_physical_time.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/__init__.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_management_fee.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_management_fee.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py` & `rqalpha-5.1.1/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/test_api_base.py` & `rqalpha-5.1.1/tests/api_tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/test_api_future.py` & `rqalpha-5.1.1/tests/api_tests/test_api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/test_api_stock.py` & `rqalpha-5.1.1/tests/api_tests/test_api_stock.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/api_tests/test_config.py` & `rqalpha-5.1.1/tests/api_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_f_buy_and_hold.py` & `rqalpha-5.1.1/tests/test_f_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_f_macd.py` & `rqalpha-5.1.1/tests/test_f_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_f_macd_signal.py` & `rqalpha-5.1.1/tests/test_f_macd_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_f_mean_reverting.py` & `rqalpha-5.1.1/tests/test_f_mean_reverting.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_s_buy_and_hold.py` & `rqalpha-5.1.1/tests/test_s_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_s_dual_thrust.py` & `rqalpha-5.1.1/tests/test_s_dual_thrust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_s_scheduler.py` & `rqalpha-5.1.1/tests/test_s_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_s_tick_size.py` & `rqalpha-5.1.1/tests/test_s_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_s_turtle.py` & `rqalpha-5.1.1/tests/test_s_turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_s_turtle_signal.py` & `rqalpha-5.1.1/tests/test_s_turtle_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/test_sf_buy_and_hold.py` & `rqalpha-5.1.1/tests/test_sf_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/unittest/__init__.py` & `rqalpha-5.1.1/tests/unittest/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/unittest/test_data/test_instrument_mixin.py` & `rqalpha-5.1.1/tests/unittest/test_data/test_instrument_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/unittest/test_data/test_trading_dates_mixin.py` & `rqalpha-5.1.1/tests/unittest/test_data/test_trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/unittest/test_mod/__init__.py` & `rqalpha-5.1.1/tests/unittest/test_mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/__init__.py` & `rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py` & `rqalpha-5.1.1/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/tests/utils.py` & `rqalpha-5.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.1.0/versioneer.py` & `rqalpha-5.1.1/versioneer.py`

 * *Files identical despite different names*

