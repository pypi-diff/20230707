# Comparing `tmp/omxpy-0.0.4.tar.gz` & `tmp/omxpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omxpy-0.0.4.tar", max compression
+gzip compressed data, was "omxpy-0.0.5.tar", max compression
```

## Comparing `omxpy-0.0.4.tar` & `omxpy-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-07-05 22:15:22.168003 omxpy-0.0.4/LICENSE
--rw-r--r--   0        0        0     4238 2023-07-05 22:15:22.168003 omxpy-0.0.4/README.md
--rw-r--r--   0        0        0       77 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/__init__.py
--rw-r--r--   0        0        0     1156 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/base_client.py
--rw-r--r--   0        0        0      468 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/__init__.py
--rw-r--r--   0        0        0    15318 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_base_token/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_olp_manager/__init__.py
--rw-r--r--   0        0        0    28180 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_orderbook/__init__.py
--rw-r--r--   0        0        0     1492 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_pair/__init__.py
--rw-r--r--   0        0        0     2690 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_price_feed/__init__.py
--rw-r--r--   0        0        0    19161 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_router/__init__.py
--rw-r--r--   0        0        0    33440 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_vault/__init__.py
--rw-r--r--   0        0        0     2612 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_vault_price_feed/__init__.py
--rw-r--r--   0        0        0    14048 2023-07-05 22:15:22.168003 omxpy-0.0.4/omxpy/contracts/omx_cw_wrapped_token/__init__.py
--rw-r--r--   0        0        0      294 2023-07-05 22:15:22.168003 omxpy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 omxpy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-07 07:31:44.811240 omxpy-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4238 2023-07-07 07:31:44.811240 omxpy-0.0.5/README.md
+-rw-r--r--   0        0        0       77 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/__init__.py
+-rw-r--r--   0        0        0     1156 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/base_client.py
+-rw-r--r--   0        0        0      468 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/__init__.py
+-rw-r--r--   0        0        0    15318 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_base_token/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_olp_manager/__init__.py
+-rw-r--r--   0        0        0    28821 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_orderbook/__init__.py
+-rw-r--r--   0        0        0     1492 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_pair/__init__.py
+-rw-r--r--   0        0        0     2690 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_price_feed/__init__.py
+-rw-r--r--   0        0        0    19161 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_router/__init__.py
+-rw-r--r--   0        0        0    33559 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_vault/__init__.py
+-rw-r--r--   0        0        0     2612 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_vault_price_feed/__init__.py
+-rw-r--r--   0        0        0    14048 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_wrapped_token/__init__.py
+-rw-r--r--   0        0        0      294 2023-07-07 07:31:44.815240 omxpy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 omxpy-0.0.5/PKG-INFO
```

### Comparing `omxpy-0.0.4/LICENSE` & `omxpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/README.md` & `omxpy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/omxpy/base_client.py` & `omxpy-0.0.5/omxpy/base_client.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_base_token/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_base_token/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_olp_manager/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_olp_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_orderbook/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_orderbook/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,29 +149,24 @@
 	collateral_token: str
 	index_token: str
 	is_long: bool
 	size_delta: "Uint128"
 	trigger_above_threshold: bool
 	trigger_price: "Uint128"
 
-CreateDecreaseOrderInternalExec__account = str
-
-CreateDecreaseOrderInternalExec__collateral_token = str
-
-CreateDecreaseOrderInternalExec__index_token = str
-
 CreateDecreaseOrderInternalExec__is_long = bool
 
 CreateDecreaseOrderInternalExec__trigger_above_threshold = bool
 
 class CreateDecreaseOrderInternalExec(TypedDict):
-	account: str
+	account: "Addr"
 	collateral_delta: "Uint128"
-	collateral_token: str
-	index_token: str
+	collateral_token: "Addr"
+	execution_fee: "Uint128"
+	index_token: "Addr"
 	is_long: bool
 	size_delta: "Uint128"
 	trigger_above_threshold: bool
 	trigger_price: "Uint128"
 
 CreateIncreaseOrderCbExec__is_long = bool
 
@@ -283,14 +278,21 @@
 	min_out: "Uint128"
 	native_amount_in: "Uint128"
 	path: "ValidatedSwapPath"
 	should_unwrap: bool
 	trigger_above_threshold: bool
 	trigger_ratio: "Uint128"
 
+class ExecuteDecreaseOrderCbExec(TypedDict):
+	balance_before: "Uint128"
+	current_price: "Uint128"
+	fee_receiver: "Addr"
+	order: "DecreaseOrder"
+	order_index: "Uint128"
+
 ExecuteDecreaseOrderExec__address = str
 
 ExecuteDecreaseOrderExec__fee_receiver = str
 
 class ExecuteDecreaseOrderExec(TypedDict):
 	address: str
 	fee_receiver: str
@@ -532,14 +534,17 @@
 
 class ExecuteMsg__create_swap_order_internal(TypedDict):
 	create_swap_order_internal: "CreateSwapOrderInternalExec"
 
 class ExecuteMsg__execute_decrease_order(TypedDict):
 	execute_decrease_order: "ExecuteDecreaseOrderExec"
 
+class ExecuteMsg__execute_decrease_order_cb(TypedDict):
+	execute_decrease_order_cb: "ExecuteDecreaseOrderCbExec"
+
 class ExecuteMsg__execute_increase_order(TypedDict):
 	execute_increase_order: "ExecuteIncreaseOrderExec"
 
 class ExecuteMsg__execute_increase_order_cb(TypedDict):
 	execute_increase_order_cb: "ExecuteIncreaseOrderCbExec"
 
 class ExecuteMsg__execute_swap_order(TypedDict):
@@ -574,15 +579,15 @@
 
 class ExecuteMsg__create_increase_order_swap_cb(TypedDict):
 	create_increase_order_swap_cb: "CreateIncreaseOrderSwapCbExec"
 
 class ExecuteMsg__create_increase_order_cb(TypedDict):
 	create_increase_order_cb: "CreateIncreaseOrderCbExec"
 
-ExecuteMsg = Union["ExecuteMsg__set_admin", "ExecuteMsg__set_min_execution_fee", "ExecuteMsg__set_min_purchase_token_amount_usd", "ExecuteMsg__cancel_decrease_order", "ExecuteMsg__cancel_increase_order", "ExecuteMsg__cancel_swap_order", "ExecuteMsg__create_decrease_order_internal", "ExecuteMsg__create_decrease_order", "ExecuteMsg__create_increase_order_internal", "ExecuteMsg__create_increase_order", "ExecuteMsg__create_swap_order", "ExecuteMsg__create_swap_order_internal", "ExecuteMsg__execute_decrease_order", "ExecuteMsg__execute_increase_order", "ExecuteMsg__execute_increase_order_cb", "ExecuteMsg__execute_swap_order", "ExecuteMsg__execute_swap_order_cb", "ExecuteMsg__swap_internal", "ExecuteMsg__transfer_in_osmo_internal", "ExecuteMsg__transfer_out_osmo_internal", "ExecuteMsg__update_decrease_order", "ExecuteMsg__update_increase_order", "ExecuteMsg__update_swap_order", "ExecuteMsg__vault_swap_internal", "ExecuteMsg__swap_internal_cb", "ExecuteMsg__create_increase_order_swap_cb", "ExecuteMsg__create_increase_order_cb"]
+ExecuteMsg = Union["ExecuteMsg__set_admin", "ExecuteMsg__set_min_execution_fee", "ExecuteMsg__set_min_purchase_token_amount_usd", "ExecuteMsg__cancel_decrease_order", "ExecuteMsg__cancel_increase_order", "ExecuteMsg__cancel_swap_order", "ExecuteMsg__create_decrease_order_internal", "ExecuteMsg__create_decrease_order", "ExecuteMsg__create_increase_order_internal", "ExecuteMsg__create_increase_order", "ExecuteMsg__create_swap_order", "ExecuteMsg__create_swap_order_internal", "ExecuteMsg__execute_decrease_order", "ExecuteMsg__execute_decrease_order_cb", "ExecuteMsg__execute_increase_order", "ExecuteMsg__execute_increase_order_cb", "ExecuteMsg__execute_swap_order", "ExecuteMsg__execute_swap_order_cb", "ExecuteMsg__swap_internal", "ExecuteMsg__transfer_in_osmo_internal", "ExecuteMsg__transfer_out_osmo_internal", "ExecuteMsg__update_decrease_order", "ExecuteMsg__update_increase_order", "ExecuteMsg__update_swap_order", "ExecuteMsg__vault_swap_internal", "ExecuteMsg__swap_internal_cb", "ExecuteMsg__create_increase_order_swap_cb", "ExecuteMsg__create_increase_order_cb"]
 
 class QueryMsg__swap_order(TypedDict):
 	swap_order: "SwapOrderQuery"
 
 class QueryMsg__decrease_order(TypedDict):
 	decrease_order: "DecreaseOrderQuery"
 
@@ -644,16 +649,16 @@
 
 	def cancel_increase_order(self, order_index: "Uint128") -> SubmittedTx:
 		return self.execute({"cancel_increase_order": {"order_index": order_index}})
 
 	def cancel_swap_order(self, order_index: "Uint128") -> SubmittedTx:
 		return self.execute({"cancel_swap_order": {"order_index": order_index}})
 
-	def create_decrease_order_internal(self, account: str, collateral_delta: "Uint128", collateral_token: str, index_token: str, is_long: bool, size_delta: "Uint128", trigger_above_threshold: bool, trigger_price: "Uint128") -> SubmittedTx:
-		return self.execute({"create_decrease_order_internal": {"account": account, "collateral_delta": collateral_delta, "collateral_token": collateral_token, "index_token": index_token, "is_long": is_long, "size_delta": size_delta, "trigger_above_threshold": trigger_above_threshold, "trigger_price": trigger_price}})
+	def create_decrease_order_internal(self, account: "Addr", collateral_delta: "Uint128", collateral_token: "Addr", execution_fee: "Uint128", index_token: "Addr", is_long: bool, size_delta: "Uint128", trigger_above_threshold: bool, trigger_price: "Uint128") -> SubmittedTx:
+		return self.execute({"create_decrease_order_internal": {"account": account, "collateral_delta": collateral_delta, "collateral_token": collateral_token, "execution_fee": execution_fee, "index_token": index_token, "is_long": is_long, "size_delta": size_delta, "trigger_above_threshold": trigger_above_threshold, "trigger_price": trigger_price}})
 
 	def create_decrease_order(self, collateral_delta: "Uint128", collateral_token: str, index_token: str, is_long: bool, size_delta: "Uint128", trigger_above_threshold: bool, trigger_price: "Uint128") -> SubmittedTx:
 		return self.execute({"create_decrease_order": {"collateral_delta": collateral_delta, "collateral_token": collateral_token, "index_token": index_token, "is_long": is_long, "size_delta": size_delta, "trigger_above_threshold": trigger_above_threshold, "trigger_price": trigger_price}})
 
 	def create_increase_order_internal(self, account: "Addr", collateral_token: "Addr", execution_fee: "Uint128", index_token: "Addr", is_long: bool, purchase_token: "Addr", purchase_token_amount: "Uint128", sender: "Addr", size_delta: "Uint128", trigger_above_threshold: bool, trigger_price: "Uint128") -> SubmittedTx:
 		return self.execute({"create_increase_order_internal": {"account": account, "collateral_token": collateral_token, "execution_fee": execution_fee, "index_token": index_token, "is_long": is_long, "purchase_token": purchase_token, "purchase_token_amount": purchase_token_amount, "sender": sender, "size_delta": size_delta, "trigger_above_threshold": trigger_above_threshold, "trigger_price": trigger_price}})
 
@@ -665,14 +670,17 @@
 
 	def create_swap_order_internal(self, account: "Addr", amount_in: "Uint128", execution_fee: "Uint128", min_out: "Uint128", native_amount_in: "Uint128", path: "ValidatedSwapPath", should_unwrap: bool, trigger_above_threshold: bool, trigger_ratio: "Uint128") -> SubmittedTx:
 		return self.execute({"create_swap_order_internal": {"account": account, "amount_in": amount_in, "execution_fee": execution_fee, "min_out": min_out, "native_amount_in": native_amount_in, "path": path, "should_unwrap": should_unwrap, "trigger_above_threshold": trigger_above_threshold, "trigger_ratio": trigger_ratio}})
 
 	def execute_decrease_order(self, address: str, fee_receiver: str, order_index: "Uint128") -> SubmittedTx:
 		return self.execute({"execute_decrease_order": {"address": address, "fee_receiver": fee_receiver, "order_index": order_index}})
 
+	def execute_decrease_order_cb(self, balance_before: "Uint128", current_price: "Uint128", fee_receiver: "Addr", order: "DecreaseOrder", order_index: "Uint128") -> SubmittedTx:
+		return self.execute({"execute_decrease_order_cb": {"balance_before": balance_before, "current_price": current_price, "fee_receiver": fee_receiver, "order": order, "order_index": order_index}})
+
 	def execute_increase_order(self, account: str, fee_recipient: str, order_index: "Uint128") -> SubmittedTx:
 		return self.execute({"execute_increase_order": {"account": account, "fee_recipient": fee_recipient, "order_index": order_index}})
 
 	def execute_increase_order_cb(self, balance_before: "Uint128", current_price: "Uint128", fee_recipient: "Addr", order: "IncreaseOrder", order_index: "Uint128") -> SubmittedTx:
 		return self.execute({"execute_increase_order_cb": {"balance_before": balance_before, "current_price": current_price, "fee_recipient": fee_recipient, "order": order, "order_index": order_index}})
 
 	def execute_swap_order(self, account: str, fee_recipient: str, order_index: "Uint128") -> SubmittedTx:
```

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_pair/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_pair/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_price_feed/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_price_feed/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_router/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_router/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_vault/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_vault/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,16 +353,19 @@
 	is_stable: bool
 	max_usdo_amount: "Uint128"
 	min_profit_bps: "Uint128"
 	token: str
 	token_decimals: int
 	token_weight: "Uint128"
 
+SetUsdoAmountMsg__token = str
+
 class SetUsdoAmountMsg(TypedDict):
-	pass
+	amount: "Uint128"
+	token: str
 
 SwapMsg__recipient = Optional[str]
 
 SwapMsg__token_in = str
 
 SwapMsg__token_out = str
 
@@ -896,16 +899,16 @@
 
 	def set_funding_rate(self, funding_interval: "Duration", funding_rate_factor: "Uint128", stable_funding_rate_factor: "Uint128") -> SubmittedTx:
 		return self.execute({"set_funding_rate": {"funding_interval": funding_interval, "funding_rate_factor": funding_rate_factor, "stable_funding_rate_factor": stable_funding_rate_factor}})
 
 	def set_token_config(self, is_shortable: bool, is_stable: bool, max_usdo_amount: "Uint128", min_profit_bps: "Uint128", token: str, token_decimals: int, token_weight: "Uint128") -> SubmittedTx:
 		return self.execute({"set_token_config": {"is_shortable": is_shortable, "is_stable": is_stable, "max_usdo_amount": max_usdo_amount, "min_profit_bps": min_profit_bps, "token": token, "token_decimals": token_decimals, "token_weight": token_weight}})
 
-	def set_usdo_amount(self) -> SubmittedTx:
-		return self.execute({"set_usdo_amount": {}})
+	def set_usdo_amount(self, amount: "Uint128", token: str) -> SubmittedTx:
+		return self.execute({"set_usdo_amount": {"amount": amount, "token": token}})
 
 	def swap(self, recipient: str, token_in: str, token_out: str) -> SubmittedTx:
 		return self.execute({"swap": {"recipient": recipient, "token_in": token_in, "token_out": token_out}})
 
 	def update_cumulative_funding_rate(self, collateral_token: str, index_token: str) -> SubmittedTx:
 		return self.execute({"update_cumulative_funding_rate": {"collateral_token": collateral_token, "index_token": index_token}})
```

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_vault_price_feed/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_vault_price_feed/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/omxpy/contracts/omx_cw_wrapped_token/__init__.py` & `omxpy-0.0.5/omxpy/contracts/omx_cw_wrapped_token/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.4/PKG-INFO` & `omxpy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omxpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 License: MIT
 Author: Omx
 Author-email: omxlabs@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

