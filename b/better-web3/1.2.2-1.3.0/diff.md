# Comparing `tmp/better_web3-1.2.2.tar.gz` & `tmp/better_web3-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-1.2.2.tar", max compression
+gzip compressed data, was "better_web3-1.3.0.tar", max compression
```

## Comparing `better_web3-1.2.2.tar` & `better_web3-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0      414 2023-06-30 17:38:45.992000 better_web3-1.2.2/better_web3/__init__.py
--rw-r--r--   0        0        0       64 2023-06-30 17:09:01.017000 better_web3-1.2.2/better_web3/_paths.py
--rw-r--r--   0        0        0     9454 2023-06-28 12:32:41.774000 better_web3-1.2.2/better_web3/batch_call.py
--rw-r--r--   0        0        0    12864 2023-06-30 17:28:39.870000 better_web3-1.2.2/better_web3/chain.py
--rw-r--r--   0        0        0      769 2023-06-30 17:47:42.447000 better_web3-1.2.2/better_web3/chains.py
--rw-r--r--   0        0        0     1173 2023-06-30 17:27:26.072000 better_web3-1.2.2/better_web3/chains.toml
--rw-r--r--   0        0        0      202 2023-06-04 17:02:17.456000 better_web3-1.2.2/better_web3/contract/__init__.py
--rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.2.2/better_web3/contract/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.2.2/better_web3/contract/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0      609 2023-06-28 12:32:25.796000 better_web3-1.2.2/better_web3/contract/__pycache__/abi.cpython-311.pyc
--rw-r--r--   0        0        0     2861 2023-06-28 12:47:45.841000 better_web3-1.2.2/better_web3/contract/__pycache__/contract.cpython-311.pyc
--rw-r--r--   0        0        0     3766 2023-06-22 18:24:06.215000 better_web3-1.2.2/better_web3/contract/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     5344 2023-06-22 18:24:06.241000 better_web3-1.2.2/better_web3/contract/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0     9591 2023-06-22 17:42:59.377000 better_web3-1.2.2/better_web3/contract/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.2.2/better_web3/contract/_paths.py
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.2.2/better_web3/contract/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.2.2/better_web3/contract/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.2.2/better_web3/contract/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.2.2/better_web3/contract/abi/multicall_v3.json
--rw-r--r--   0        0        0      295 2023-06-28 12:32:24.657000 better_web3-1.2.2/better_web3/contract/abi.py
--rw-r--r--   0        0        0     1217 2023-06-28 12:35:30.364000 better_web3-1.2.2/better_web3/contract/contract.py
--rw-r--r--   0        0        0     1749 2023-06-22 18:23:50.372000 better_web3-1.2.2/better_web3/contract/erc20.py
--rw-r--r--   0        0        0     2873 2023-06-22 18:23:50.412000 better_web3-1.2.2/better_web3/contract/erc721.py
--rw-r--r--   0        0        0     6182 2023-06-22 17:29:46.245000 better_web3-1.2.2/better_web3/contract/multicall.py
--rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.2.2/better_web3/enums.py
--rw-r--r--   0        0        0      199 2023-06-28 11:42:15.433000 better_web3-1.2.2/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      445 2023-06-28 12:32:10.840000 better_web3-1.2.2/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3500 2023-06-19 18:50:51.812000 better_web3-1.2.2/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.2.2/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     1519 2023-06-28 12:32:10.893000 better_web3-1.2.2/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0     1907 2023-06-19 15:51:51.887000 better_web3-1.2.2/better_web3/utils/eth.py
--rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.2.2/better_web3/utils/file.py
--rw-r--r--   0        0        0      733 2023-06-28 11:42:15.546000 better_web3-1.2.2/better_web3/utils/other.py
--rw-r--r--   0        0        0     1474 2023-06-29 11:26:53.088000 better_web3-1.2.2/better_web3/wallet.py
--rw-r--r--   0        0        0      445 2023-06-30 19:21:32.461000 better_web3-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      406 2023-06-23 11:07:22.626000 better_web3-1.2.2/README.md
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 better_web3-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      377 2023-07-07 12:41:36.289000 better_web3-1.3.0/better_web3/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-30 17:09:01.017000 better_web3-1.3.0/better_web3/_paths.py
+-rw-r--r--   0        0        0    10484 2023-07-07 13:10:10.895000 better_web3-1.3.0/better_web3/batch_call.py
+-rw-r--r--   0        0        0    14905 2023-07-07 12:24:04.882000 better_web3-1.3.0/better_web3/chain.py
+-rw-r--r--   0        0        0      251 2023-07-07 12:10:25.885000 better_web3-1.3.0/better_web3/contract/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-04 17:49:29.882000 better_web3-1.3.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.3.0/better_web3/contract/__pycache__/_paths.cpython-311.pyc
+-rw-r--r--   0        0        0     2861 2023-06-28 12:47:45.841000 better_web3-1.3.0/better_web3/contract/__pycache__/contract.cpython-311.pyc
+-rw-r--r--   0        0        0     3766 2023-06-22 18:24:06.215000 better_web3-1.3.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc
+-rw-r--r--   0        0        0     5344 2023-06-22 18:24:06.241000 better_web3-1.3.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc
+-rw-r--r--   0        0        0     9591 2023-06-22 17:42:59.377000 better_web3-1.3.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc
+-rw-r--r--   0        0        0      352 2023-07-07 12:03:06.296000 better_web3-1.3.0/better_web3/contract/_abi.py
+-rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.3.0/better_web3/contract/_paths.py
+-rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-1.3.0/better_web3/contract/abi/disperse.json
+-rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.3.0/better_web3/contract/abi/erc1155.json
+-rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.3.0/better_web3/contract/abi/erc20.json
+-rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.3.0/better_web3/contract/abi/erc721.json
+-rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.3.0/better_web3/contract/abi/multicall_v3.json
+-rw-r--r--   0        0        0     1217 2023-06-28 12:35:30.364000 better_web3-1.3.0/better_web3/contract/contract.py
+-rw-r--r--   0        0        0      974 2023-07-07 12:13:30.821000 better_web3-1.3.0/better_web3/contract/disperse.py
+-rw-r--r--   0        0        0     1750 2023-07-07 12:07:18.371000 better_web3-1.3.0/better_web3/contract/erc20.py
+-rw-r--r--   0        0        0     2874 2023-07-07 12:07:18.593000 better_web3-1.3.0/better_web3/contract/erc721.py
+-rw-r--r--   0        0        0     6201 2023-07-07 12:07:18.259000 better_web3-1.3.0/better_web3/contract/multicall.py
+-rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.3.0/better_web3/enums.py
+-rw-r--r--   0        0        0      199 2023-06-28 11:42:15.433000 better_web3-1.3.0/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-28 12:32:10.840000 better_web3-1.3.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3500 2023-06-19 18:50:51.812000 better_web3-1.3.0/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.3.0/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     1519 2023-06-28 12:32:10.893000 better_web3-1.3.0/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0     1907 2023-06-19 15:51:51.887000 better_web3-1.3.0/better_web3/utils/eth.py
+-rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.3.0/better_web3/utils/file.py
+-rw-r--r--   0        0        0      733 2023-06-28 11:42:15.546000 better_web3-1.3.0/better_web3/utils/other.py
+-rw-r--r--   0        0        0     1891 2023-07-01 13:13:40.896000 better_web3-1.3.0/better_web3/wallet.py
+-rw-r--r--   0        0        0      412 2023-07-07 12:24:04.992000 better_web3-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-07-07 13:10:55.766000 better_web3-1.3.0/README.md
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 better_web3-1.3.0/PKG-INFO
```

### Comparing `better_web3-1.2.2/better_web3/batch_call.py` & `better_web3-1.3.0/better_web3/batch_call.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,27 +108,30 @@
     def request(
             self,
             payloads: Iterable[dict],
             *,
             raise_exceptions: bool = True,
             batch_size: int = None,
             delay: int = None,
-    ) -> Iterable:
+    ) -> Iterable[dict[str: dict, str: Any]]:
         if not payloads:
             return []
 
         batch_size = batch_size or self.batch_request_size
         delay = delay or self.batch_request_delay
 
         for chunk in chunks(payloads, batch_size):
             response = self.http_session.post(self.rpc, json=chunk, timeout=self.slow_timeout)
             results = response.json()
-            for result in process_results(results, raise_exceptions=raise_exceptions):
-                #  TODO возвращать в следующием формате:
-                #       {"payload": payload, "result": result}
+            for payload, response in zip(chunk, process_results(results, raise_exceptions=raise_exceptions)):
+                result = {"payload": payload}
+                if isinstance(response, JSONRPCException):
+                    result["exception"] = response
+                else:
+                    result["result"] = response
                 yield result
             time.sleep(delay)  # TODO Сделать это умнее
 
     def contract_request(
             self,
             contract_functions: Iterable[ContractFunction],
             block_identifier: BlockIdentifier = "latest",
@@ -163,16 +166,21 @@
         results = self.request(
             payloads,
             raise_exceptions=raise_exceptions,
             batch_size=batch_size,
             delay=delay,
         )
         results = process_eth_call_results(results, output_types, raise_exceptions=raise_exceptions)
-        for contract_function, result in zip(contract_functions, results):
-            yield {"contract_function": contract_function, "result": result}
+        for contract_function, response in zip(contract_functions, results):
+            result = {"contract_function": contract_function}
+            if isinstance(response, JSONRPCException):
+                result["exception"] = response
+            else:
+                result["result"] = response
+            yield result
 
     ################################################################################
     # Batch request shortcuts
     ################################################################################
 
     def balances(
             self,
@@ -183,65 +191,82 @@
         if not addresses:
             return []
 
         payloads = [build_payload(i, "eth_getBalance", [address, hex_block_identifier(block_identifier)])
                     for i, address in enumerate(addresses)]
         balances = self.request(payloads, **kwargs)
 
-        for address, balance in zip(addresses, balances):
-            if not isinstance(balance, JSONRPCException):
-                balance = Wei(int(balance, 16))
-            yield {"address": address, "balance": balance}
+        for address, response in zip(addresses, balances):
+            balance_data = {"address": address}
+            if "exception" in response:
+                balance_data["exception"] = response["exception"]
+            else:
+                balance_data["balance"] = Wei(int(response["result"], 16))
+            yield balance_data
 
     def txs(
             self,
             tx_hashes: Iterable[Hash32 | HexBytes | HexStr],
             **kwargs,
     ) -> Iterable[dict[str: Hash32 | HexBytes | HexStr, str: TxData | JSONRPCException]]:
         if not tx_hashes:
             return []
 
         payloads = [build_payload(i, "eth_getTransactionByHash", [HexBytes(tx_hash).hex()])
                     for i, tx_hash in enumerate(tx_hashes)]
         txs = self.request(payloads, **kwargs)
 
-        for tx_hash, tx in zip(tx_hashes, txs):
-            yield {"tx_hash": tx_hash, "tx": transaction_result_formatter(tx)}
+        for tx_hash, response in zip(tx_hashes, txs):
+            tx_data = {"tx_hash": tx_hash}
+            if "exception" in response:
+                tx_data["exception"] = response["exception"]
+            else:
+                tx_data["tx"] = transaction_result_formatter(response["result"])
+            yield tx_data
 
     def tx_receipts(
             self,
             tx_hashes: Iterable[Hash32 | HexBytes | HexStr],
             **kwargs,
     ) -> Iterable[dict[str: Hash32 | HexBytes | HexStr, str: TxReceipt | JSONRPCException]]:
         if not tx_hashes:
             return []
 
         payloads = [build_payload(i, "eth_getTransactionReceipt", [HexBytes(tx_hash).hex()])
                     for i, tx_hash in enumerate(tx_hashes)]
         tx_receipts = self.request(payloads, **kwargs)
 
-        for tx_hash, tx_receipt in zip(tx_hashes, tx_receipts):
-            yield {"tx_hash": tx_hash, "tx": receipt_formatter(tx_receipt)}
+        for tx_hash, response in zip(tx_hashes, tx_receipts):
+            tx_receipt_data = {"tx_hash": tx_hash}
+            if "exception" in response:
+                tx_receipt_data["exception"] = response["exception"]
+            else:
+                tx_receipt_data["tx"] = receipt_formatter(response["result"])
+            yield tx_receipt_data
 
     def blocks(
             self,
             block_identifiers: Iterable[BlockIdentifier],
             full_transactions: bool = False,
             **kwargs,
-    ) -> Iterable[dict[str: BlockIdentifier, str: BlockData | JSONRPCException]]:
+    ) -> Iterable[dict[str: BlockIdentifier, str: BlockData | None | JSONRPCException]]:
         if not block_identifiers:
             return []
 
         payloads = []
         for i, block_identifier in enumerate(block_identifiers):
             is_int = isinstance(block_identifier, int)
             method = "eth_getBlockByNumber" if is_int else "eth_getBlockByHash"
             block_identifier = block_identifier if is_int else hex_block_identifier(block_identifier)
             payloads.append(build_payload(i, method, [block_identifier, full_transactions]))
 
         blocks_data = self.request(payloads, **kwargs)
 
-        for block_identifier, block_data in zip(block_identifiers, blocks_data):
-            if block_data:
-                if "extraData" in block_data:
+        for block_identifier, response in zip(block_identifiers, blocks_data):
+            block_data = {"block_identifier": block_identifier}
+            if "exception" in response:
+                block_data["exception"] = response["exception"]
+            else:
+                if "extraData" in response["exception"]:
                     del block_data["extraData"]  # Remove extraData, raises some problems on parsing
-                yield {"block_identifier": block_identifier, "block": receipt_formatter(block_formatter(block_data))}
+                block_data["block"] = receipt_formatter(block_formatter(response["result"]))
+            yield block_data
```

### Comparing `better_web3-1.2.2/better_web3/chain.py` & `better_web3-1.3.0/better_web3/chain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from dataclasses import dataclass
+
 import requests
 from eth_account.signers.local import LocalAccount
 from eth_typing import BlockNumber, ChecksumAddress, HexStr, Address, Hash32
 from hexbytes import HexBytes
-from pydantic import BaseModel
 from requests.adapters import HTTPAdapter
 from web3 import HTTPProvider, Web3
 from web3.contract.contract import ContractFunction
 from web3.middleware import geth_poa_middleware
 from web3.types import (
     BlockData,
     BlockIdentifier,
@@ -14,20 +15,21 @@
     TxData,
     TxParams,
     TxReceipt,
     Wei,
 )
 
 from .batch_call import BatchCallManager
-from .contract import Contract, Multicall, ERC20, ERC721
+from .contract import Contract, Multicall, Disperse, ERC20, ERC721
 from .enums import TxSpeed
 from .utils import cache, link_by_tx_hash
 
 
-class NativeToken(BaseModel):
+@dataclass
+class NativeToken:
     symbol: str = "ETH"
     decimals: int = 18
 
 
 class Chain:
     def __init__(
             self,
@@ -43,18 +45,22 @@
             # Connection settings
             provider_timeout: int = 15,
             slow_provider_timeout: int = 60,
             retry_count: int = 3,
             # Middlewares
             use_poa_middleware: bool = True,
             # Multicall
-            multicall_v3_address: ChecksumAddress | str = None,
+            multicall_v3_contract_address: ChecksumAddress | str = None,
+            # Disperse
+            disperse_contract_address: ChecksumAddress | str = None,
             # Batch request
-            batch_request_size: int = 500,
+            batch_request_size: int = 10,
             batch_request_delay: int = 1,
+            # Tx params
+            gas_price: Wei | int = None,
     ):
         self._rpc = rpc
         self.name = name
         self.is_testnet = is_testnet
         self.token = NativeToken(symbol=symbol, decimals=decimals)
         self.explorer_url = explorer_url
 
@@ -68,18 +74,22 @@
         self.w3 = Web3(provider=self.w3_provider)
         self.slow_w3 = Web3(provider=self.w3_slow_provider)
 
         if use_poa_middleware:
             self.w3.middleware_onion.inject(geth_poa_middleware, layer=0)
             self.slow_w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
-        self.multicall = Multicall(chain=self, address=multicall_v3_address)
+        self.multicall = Multicall(chain=self, address=multicall_v3_contract_address)
+        self.disperse = Disperse(chain=self, address=disperse_contract_address)
+
         self.batch_request = BatchCallManager(
             self, batch_request_size, batch_request_delay)
 
+        self.gas_price = gas_price
+
     def _create_http_provider(self, timeout: int) -> HTTPProvider:
         return HTTPProvider(
             self._rpc,
             request_kwargs={"timeout": timeout},
             session=self.http_session,
         )
 
@@ -209,14 +219,53 @@
             return False
         else:
             block_number = self.w3.eth.block_number
             confirmations_count = block_number - tx_receipt["blockNumber"]
 
             return confirmations_count >= confirmations
 
+    def transfer(
+            self,
+            account_from: LocalAccount,
+            address_to: Address | ChecksumAddress | str,
+            value: Wei | int,
+            *,
+            gas: int = None,
+            nonce: Nonce | int = None,
+            # legacy pricing
+            gas_price: Wei | int = None,
+            # dynamic fee pricing
+            max_fee_per_gas: Wei = None,
+            max_priority_fee_per_gas: Wei = None,
+            tx_speed: TxSpeed = TxSpeed.NORMAL,
+    ) -> HexStr:
+        gas_price = gas_price or self.gas_price
+        tx_params = self._build_tx_base_params(gas, account_from.address, address_to, nonce, value)
+        gas = self.w3.eth.estimate_gas(tx_params)
+        tx_params = self._build_tx_base_params(gas, tx_params=tx_params)
+        tx_params = self._build_tx_fee_params(
+            gas_price, max_fee_per_gas, max_priority_fee_per_gas, tx_speed, tx_params=tx_params)
+        return self.sign_and_send_tx(account_from, tx_params)
+
+    def transfer_all(
+            self,
+            account_from: LocalAccount,
+            address_to: Address | ChecksumAddress | str,
+            *,
+            gas: int = None,
+            nonce: Nonce | int = None,
+            # legacy pricing
+            gas_price: Wei | int = None,
+            # dynamic fee pricing
+            max_fee_per_gas: Wei = None,
+            max_priority_fee_per_gas: Wei = None,
+            tx_speed: TxSpeed = TxSpeed.NORMAL,
+    ):
+        ...  # TODO Реализовать метод Chain.transfer_all()
+
     ################################################################################
     # Gas price shortcuts
     ################################################################################
 
     def get_gas_price(self) -> Wei:
         return self.w3.eth.gas_price
 
@@ -241,40 +290,40 @@
     ################################################################################
     # Working with transactions
     ################################################################################
 
     def _build_tx_base_params(
             self,
             gas: int = None,
-            from_: Address | ChecksumAddress | str = None,
-            to: Address | ChecksumAddress | str = None,
-            nonce: Nonce = None,
+            address_from: Address | ChecksumAddress | str = None,
+            address_to: Address | ChecksumAddress | str = None,
+            nonce: Nonce | int = None,
             value: Wei = None,
             *,
             tx_params: TxParams = None,
     ) -> TxParams:
         if tx_params is None:
             tx_params = dict()
         tx_params = tx_params.copy()
 
         tx_params["chainId"] = self.chain_id
 
         if gas is not None:
             tx_params["gas"] = gas
-        if from_ is not None:
-            tx_params["from"] = from_
-        if to is not None:
-            tx_params["to"] = to
+        if address_from is not None:
+            tx_params["from"] = address_from
+        if address_to is not None:
+            tx_params["to"] = address_to
         if value is not None:
             tx_params["value"] = value
 
         if nonce is not None:
             tx_params["nonce"] = nonce
-        elif from_ is not None:
-            tx_params["nonce"] = self.get_nonce(from_)
+        elif address_from is not None:
+            tx_params["nonce"] = self.get_nonce(address_from)
 
         return tx_params
 
     def _build_tx_fee_params(
             self,
             # legacy pricing
             gas_price: Wei = None,
@@ -301,26 +350,27 @@
 
         return tx_params
 
     def build_tx(
             self,
             contract_function: ContractFunction,
             gas: int = None,
-            from_: Address | ChecksumAddress | str = None,
-            to: Address | ChecksumAddress | str = None,
-            nonce: Nonce = None,
+            address_from: Address | ChecksumAddress | str = None,
+            address_to: Address | ChecksumAddress | str = None,
+            nonce: Nonce | int = None,
             value: Wei | int = None,
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
             max_fee_per_gas: Wei = None,
             max_priority_fee_per_gas: Wei = None,
             tx_speed: TxSpeed = TxSpeed.NORMAL,
     ) -> TxParams:
-        tx_params = self._build_tx_base_params(gas, from_, to, nonce, value)
+        gas_price = gas_price or self.gas_price
+        tx_params = self._build_tx_base_params(gas, address_from, address_to, nonce, value)
         gas = contract_function.estimate_gas(tx_params)
         tx_params = self._build_tx_base_params(gas, tx_params=tx_params)
         tx_params = self._build_tx_fee_params(
             gas_price, max_fee_per_gas, max_priority_fee_per_gas, tx_speed, tx_params=tx_params)
         return contract_function.build_transaction(tx_params)
 
     def sign_and_send_tx(self, account: LocalAccount, tx: TxParams) -> HexStr:
@@ -337,11 +387,11 @@
     def execute_fn(
             self,
             account: LocalAccount,
             fn: ContractFunction,
             *,
             value: Wei = None,
     ) -> tuple[TxReceipt, HexStr]:
-        tx = self.build_tx(fn, from_=account.address, value=value)
+        tx = self.build_tx(fn, address_from=account.address, value=value)
         tx_hash = self.sign_and_send_tx(account, tx)
         tx_receipt = self.wait_for_tx_receipt(tx_hash)
         return tx_receipt, tx_hash
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `better_web3-1.2.2/better_web3/contract/__pycache__/contract.cpython-311.pyc` & `better_web3-1.3.0/better_web3/contract/__pycache__/contract.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/__pycache__/erc20.cpython-311.pyc` & `better_web3-1.3.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/__pycache__/erc721.cpython-311.pyc` & `better_web3-1.3.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/__pycache__/multicall.cpython-311.pyc` & `better_web3-1.3.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/abi/erc1155.json` & `better_web3-1.3.0/better_web3/contract/abi/erc1155.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/abi/erc20.json` & `better_web3-1.3.0/better_web3/contract/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/abi/erc721.json` & `better_web3-1.3.0/better_web3/contract/abi/erc721.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/abi/multicall_v3.json` & `better_web3-1.3.0/better_web3/contract/abi/multicall_v3.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/contract.py` & `better_web3-1.3.0/better_web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/contract/erc20.py` & `better_web3-1.3.0/better_web3/contract/erc20.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Iterable
 
 from eth_typing import ChecksumAddress, BlockIdentifier
 from web3.types import Wei
 
-from .abi import ERC20_ABI
+from ._abi import ERC20_ABI
 from .contract import Contract
 from ..utils import cache
 
 if TYPE_CHECKING:
     from ..chain import Chain
```

### Comparing `better_web3-1.2.2/better_web3/contract/erc721.py` & `better_web3-1.3.0/better_web3/contract/erc721.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Iterable
 
 from eth_typing import ChecksumAddress, BlockIdentifier
 from eth_utils import to_checksum_address
 
-from .abi import ERC721_ABI
+from ._abi import ERC721_ABI
 from .contract import Contract
 from ..utils import cache
 
 if TYPE_CHECKING:
     from ..chain import Chain
```

### Comparing `better_web3-1.2.2/better_web3/contract/multicall.py` & `better_web3-1.3.0/better_web3/contract/multicall.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from eth_typing import BlockIdentifier, BlockNumber, ChecksumAddress
 from hexbytes import HexBytes
 from web3._utils.abi import map_abi_data
 from web3._utils.normalizers import BASE_RETURN_NORMALIZERS
 from web3.contract.contract import ContractFunction
 from web3.exceptions import ContractLogicError
 
-from .abi import MULTICALL_V3_ABI
+from ._abi import MULTICALL_V3_ABI
 from .contract import Contract
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from ..chain import Chain
 
 
-MULTICALL_V3_ADDRESS = "0xcA11bde05977b3631167028862bE2a173976CA11"
+MULTICALL_V3_CONTRACT_ADDRESS = "0xcA11bde05977b3631167028862bE2a173976CA11"
 
 
 @dataclass
 class MulticallResult:
     success: bool
     return_data: bytes | None
 
@@ -42,15 +42,15 @@
 class Multicall(Contract):
     def __init__(
         self,
         chain: "Chain",
         address: ChecksumAddress | str = None,
         abi=None,
     ):
-        address = address or MULTICALL_V3_ADDRESS
+        address = address or MULTICALL_V3_CONTRACT_ADDRESS
         abi = abi or MULTICALL_V3_ABI
         super().__init__(chain, address, abi)
 
     @staticmethod
     def _build_payload(
         contract_functions: Sequence[ContractFunction],
     ) -> tuple[list[tuple[ChecksumAddress, bytes]], list[list[Any]]]:
```

### Comparing `better_web3-1.2.2/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-1.3.0/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/utils/__pycache__/file.cpython-311.pyc` & `better_web3-1.3.0/better_web3/utils/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-1.3.0/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/utils/eth.py` & `better_web3-1.3.0/better_web3/utils/eth.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/utils/file.py` & `better_web3-1.3.0/better_web3/utils/file.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/better_web3/utils/other.py` & `better_web3-1.3.0/better_web3/utils/other.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.2.2/PKG-INFO` & `better_web3-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 1.2.2
-Summary: Chain, Contracts(Multicall, ERC20/ERC721), batch calls and other..
+Version: 1.3.0
+Summary: Chains, Contracts(Multicall, Disperse, ERC20/ERC721), batch calls and other..
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10.9,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: web3 (>=6.5.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Better Web3.py
-[ [Telegram](https://t.me/Cum_Insider) ] [ [PyPi](https://pypi.org/project/better-web3) ]
+[ [Telegram](https://t.me/cum_insider) ] [ [PyPi](https://pypi.org/project/better-web3) ]
 
 ```bash
 pip install better-web3
 ```
 
 ## Credits
 - [safe-global](https://github.com/safe-global) / [Safe-eth-py (previosly known as Gnosis-py)](https://github.com/safe-global/safe-eth-py)
```

