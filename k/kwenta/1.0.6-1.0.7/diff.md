# Comparing `tmp/kwenta-1.0.6.tar.gz` & `tmp/kwenta-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwenta-1.0.6.tar", last modified: Wed Jul  5 21:17:38 2023, max compression
+gzip compressed data, was "kwenta-1.0.7.tar", last modified: Fri Jul  7 12:19:11 2023, max compression
```

## Comparing `kwenta-1.0.6.tar` & `kwenta-1.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 21:17:07.000000 kwenta-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 21:17:38.351922 kwenta-1.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.347922 kwenta-1.0.6/kwenta/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/cli/kwenta_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/contracts/json/
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/PerpsV2ExchangeRate.json
--rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/SMAccount.json
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/SMFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/sUSD.json
--rw-r--r--   0 runner    (1001) docker     (123)    56577 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/kwenta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/pyth/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:17:38.351922 kwenta-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-05 21:17:07.000000 kwenta-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.773059 kwenta-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 12:18:42.000000 kwenta-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 12:19:11.773059 kwenta-1.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/cli/kwenta_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.773059 kwenta-1.0.7/kwenta/contracts/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/PerpsV2ExchangeRate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/SMAccount.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/SMFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/contracts/json/sUSD.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57026 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/kwenta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.773059 kwenta-1.0.7/kwenta/pyth/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.773059 kwenta-1.0.7/kwenta/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-07 12:18:42.000000 kwenta-1.0.7/kwenta/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:19:11.769058 kwenta-1.0.7/kwenta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 12:19:11.000000 kwenta-1.0.7/kwenta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:19:11.773059 kwenta-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 12:18:42.000000 kwenta-1.0.7/setup.py
```

### Comparing `kwenta-1.0.6/PKG-INFO` & `kwenta-1.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.6/kwenta/alerts/alerts.py` & `kwenta-1.0.7/kwenta/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/cli/kwenta_cli.py` & `kwenta-1.0.7/kwenta/cli/kwenta_cli.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/constants.py` & `kwenta-1.0.7/kwenta/constants.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/contracts/contracts.py` & `kwenta-1.0.7/kwenta/contracts/contracts.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/contracts/json/PerpsV2ExchangeRate.json` & `kwenta-1.0.7/kwenta/contracts/json/PerpsV2ExchangeRate.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/contracts/json/PerpsV2Market.json` & `kwenta-1.0.7/kwenta/contracts/json/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/contracts/json/PerpsV2MarketData.json` & `kwenta-1.0.7/kwenta/contracts/json/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/contracts/json/SMAccount.json` & `kwenta-1.0.7/kwenta/contracts/json/SMAccount.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/contracts/json/SMFactory.json` & `kwenta-1.0.7/kwenta/contracts/json/SMFactory.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/contracts/json/sUSD.json` & `kwenta-1.0.7/kwenta/contracts/json/sUSD.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/kwenta.py` & `kwenta-1.0.7/kwenta/kwenta.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .constants import (
     DEFAULT_NETWORK_ID,
     DEFAULT_TRACKING_CODE,
     DEFAULT_SLIPPAGE,
     DEFAULT_GQL_ENDPOINT_PERPS,
     DEFAULT_GQL_ENDPOINT_RATES,
     DEFAULT_PRICE_SERVICE_ENDPOINTS,
+    ACCOUNT_COMMANDS
 )
 from .contracts import abis, addresses
 from .alerts import Alerts
 from .queries import Queries
 from .pyth import Pyth
 from eth_abi import encode
 
@@ -85,14 +86,15 @@
         )
 
         # init pyth
         if not price_service_endpoint:
             price_service_endpoint = DEFAULT_PRICE_SERVICE_ENDPOINTS[self.network_id]
 
         self.pyth = Pyth(self.network_id, price_service_endpoint=price_service_endpoint)
+        self.account_commands = ACCOUNT_COMMANDS
 
     @property
     def web3(self):
         w3 = Web3(self.provider_class(self.provider_rpc))
 
         if w3.eth.chain_id != self.network_id:
             raise Exception("The RPC `chain_id` must match the stored `network_id`")
@@ -1538,23 +1540,27 @@
         Excecute Kwenta Command Chain. Advanced Usage.
         ...
         Attributes
         ----------
         command_list : list
             list of commands to execute with command details
             Example format:
-                token_amount = 55000000
-                market = "SOL"
+                token_amount = 55000000000
+                token_symbol = "SOL"
                 command_list = []
-                command_list.append(kwenta_account.ACCOUNT_COMMANDS['ACCOUNT_MODIFY_MARGIN'],[token_amount])
-                command_list.append(kwenta_account.ACCOUNT_COMMANDS['PERPS_V2_MODIFY_MARGIN'],[market, token_amount])
+                command1_encoded = encode(account.account_commands['ACCOUNT_MODIFY_MARGIN'][1],[token_amount])
+                command_list.append([account.account_commands['ACCOUNT_MODIFY_MARGIN'][0],command1_encoded])
+                command2_encoded =  encode(account.account_commands['PERPS_V2_MODIFY_MARGIN'][1],[str(account.markets[token_symbol.upper()]["market_address"]),token_amount])
+                command_list.append([account.account_commands['PERPS_V2_MODIFY_MARGIN'][0],command2_encoded])
+                account.execute_chain(command_list,wallet_address,execute_now=True)
         Returns
         ----------
         str: token transfer Tx id
         """
+        
         if wallet_address is None:
             wallet_address = self.sm_account
         sm_account_contract = self.web3.eth.contract(
             self.web3.to_checksum_address(self.sm_account), abi=abis["SM_Account"]
         )
         if execute_now:
             command_ids = []
```

### Comparing `kwenta-1.0.6/kwenta/pyth/constants.py` & `kwenta-1.0.7/kwenta/pyth/constants.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/pyth/pyth.py` & `kwenta-1.0.7/kwenta/pyth/pyth.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/queries/config.py` & `kwenta-1.0.7/kwenta/queries/config.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/queries/gql.py` & `kwenta-1.0.7/kwenta/queries/gql.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta/queries/queries.py` & `kwenta-1.0.7/kwenta/queries/queries.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/kwenta.egg-info/PKG-INFO` & `kwenta-1.0.7/kwenta.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.6/kwenta.egg-info/SOURCES.txt` & `kwenta-1.0.7/kwenta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.6/setup.py` & `kwenta-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kwenta",
-    version="1.0.6",
+    version="1.0.7",
     description="Python SDK for Kwenta",
     long_description="Python SDK for Kwenta",
     author="Kwenta DAO",
     packages=[
         "kwenta",
         "kwenta.alerts",
         "kwenta.cli",
```

