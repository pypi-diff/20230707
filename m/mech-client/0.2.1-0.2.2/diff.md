# Comparing `tmp/mech_client-0.2.1.tar.gz` & `tmp/mech_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mech_client-0.2.1.tar", max compression
+gzip compressed data, was "mech_client-0.2.2.tar", max compression
```

## Comparing `mech_client-0.2.1.tar` & `mech_client-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11339 2023-06-26 13:03:03.797666 mech_client-0.2.1/LICENSE
--rw-r--r--   0        0        0     4049 2023-06-26 13:03:03.797666 mech_client-0.2.1/README.md
--rw-r--r--   0        0        0       42 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/__init__.py
--rw-r--r--   0        0        0     5790 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/acn.py
--rw-r--r--   0        0        0     3359 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/cli.py
--rw-r--r--   0        0        0     1028 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/helpers/__init__.py
--rw-r--r--   0        0        0     1641 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/README.md
--rw-r--r--   0        0        0     1143 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/__init__.py
--rw-r--r--   0        0        0     1543 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/acn.proto
--rw-r--r--   0        0        0     8325 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/acn_pb2.py
--rw-r--r--   0        0        0     7982 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/custom_types.py
--rw-r--r--   0        0        0     4443 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/dialogues.py
--rw-r--r--   0        0        0    10256 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/message.py
--rw-r--r--   0        0        0     1233 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/protocol.yaml
--rw-r--r--   0        0        0     6405 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/serialization.py
--rw-r--r--   0        0        0      847 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/acn/tests/__init__.py
--rw-r--r--   0        0        0     8965 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn.py
--rw-r--r--   0        0        0     1964 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn_dialogues.py
--rw-r--r--   0        0        0     4332 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn_messages.py
--rw-r--r--   0        0        0      577 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/README.md
--rw-r--r--   0        0        0     1221 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/__init__.py
--rw-r--r--   0        0        0      271 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/acn_data_share.proto
--rw-r--r--   0        0        0     2349 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
--rw-r--r--   0        0        0     4078 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/dialogues.py
--rw-r--r--   0        0        0     7726 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/message.py
--rw-r--r--   0        0        0     1052 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/protocol.yaml
--rw-r--r--   0        0        0     4450 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/serialization.py
--rw-r--r--   0        0        0     1835 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
--rw-r--r--   0        0        0     2021 2023-06-26 13:03:59.486679 mech_client-0.2.1/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
--rw-r--r--   0        0        0      631 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/README.md
--rw-r--r--   0        0        0      879 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/__init__.py
--rw-r--r--   0        0        0    27786 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/connection.py
--rw-r--r--   0        0        0     1763 2023-06-26 13:03:59.482679 mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/connection.yaml
--rw-r--r--   0        0        0    11471 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/interact.py
--rw-r--r--   0        0        0     2250 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/prompt_to_ipfs.py
--rw-r--r--   0        0        0     2059 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/push_to_ipfs.py
--rw-r--r--   0        0        0     1807 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/subgraph.py
--rw-r--r--   0        0        0     2581 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/to_png.py
--rw-r--r--   0        0        0     6824 2023-06-26 13:03:03.797666 mech_client-0.2.1/mech_client/wss.py
--rw-r--r--   0        0        0     1469 2023-06-26 13:03:03.801666 mech_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 mech_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-07 10:27:44.866578 mech_client-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4049 2023-07-07 10:27:44.866578 mech_client-0.2.2/README.md
+-rw-r--r--   0        0        0       42 2023-07-07 10:27:44.866578 mech_client-0.2.2/mech_client/__init__.py
+-rw-r--r--   0        0        0     5790 2023-07-07 10:27:44.866578 mech_client-0.2.2/mech_client/acn.py
+-rw-r--r--   0        0        0     3359 2023-07-07 10:27:44.866578 mech_client-0.2.2/mech_client/cli.py
+-rw-r--r--   0        0        0     1028 2023-07-07 10:27:44.866578 mech_client-0.2.2/mech_client/helpers/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/README.md
+-rw-r--r--   0        0        0     1143 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/__init__.py
+-rw-r--r--   0        0        0     1543 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/acn.proto
+-rw-r--r--   0        0        0     8325 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/acn_pb2.py
+-rw-r--r--   0        0        0     7982 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/custom_types.py
+-rw-r--r--   0        0        0     4443 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/dialogues.py
+-rw-r--r--   0        0        0    10256 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/message.py
+-rw-r--r--   0        0        0     1233 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/protocol.yaml
+-rw-r--r--   0        0        0     6405 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/serialization.py
+-rw-r--r--   0        0        0      847 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/tests/__init__.py
+-rw-r--r--   0        0        0     8965 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/tests/test_acn.py
+-rw-r--r--   0        0        0     1964 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/tests/test_acn_dialogues.py
+-rw-r--r--   0        0        0     4332 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn/tests/test_acn_messages.py
+-rw-r--r--   0        0        0      577 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/README.md
+-rw-r--r--   0        0        0     1221 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/acn_data_share.proto
+-rw-r--r--   0        0        0     2349 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/acn_data_share_pb2.py
+-rw-r--r--   0        0        0     4078 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/dialogues.py
+-rw-r--r--   0        0        0     7726 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/message.py
+-rw-r--r--   0        0        0     1052 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/protocol.yaml
+-rw-r--r--   0        0        0     4450 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/serialization.py
+-rw-r--r--   0        0        0     1835 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py
+-rw-r--r--   0        0        0     2021 2023-07-07 10:28:41.978394 mech_client-0.2.2/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py
+-rw-r--r--   0        0        0      631 2023-07-07 10:28:41.974394 mech_client-0.2.2/mech_client/helpers/p2p_libp2p_client/README.md
+-rw-r--r--   0        0        0      879 2023-07-07 10:28:41.974394 mech_client-0.2.2/mech_client/helpers/p2p_libp2p_client/__init__.py
+-rw-r--r--   0        0        0    27786 2023-07-07 10:28:41.974394 mech_client-0.2.2/mech_client/helpers/p2p_libp2p_client/connection.py
+-rw-r--r--   0        0        0     1763 2023-07-07 10:28:41.974394 mech_client-0.2.2/mech_client/helpers/p2p_libp2p_client/connection.yaml
+-rw-r--r--   0        0        0    11558 2023-07-07 10:27:44.866578 mech_client-0.2.2/mech_client/interact.py
+-rw-r--r--   0        0        0     2250 2023-07-07 10:27:44.866578 mech_client-0.2.2/mech_client/prompt_to_ipfs.py
+-rw-r--r--   0        0        0     2059 2023-07-07 10:27:44.866578 mech_client-0.2.2/mech_client/push_to_ipfs.py
+-rw-r--r--   0        0        0     1807 2023-07-07 10:27:44.866578 mech_client-0.2.2/mech_client/subgraph.py
+-rw-r--r--   0        0        0     2581 2023-07-07 10:27:44.870578 mech_client-0.2.2/mech_client/to_png.py
+-rw-r--r--   0        0        0     6824 2023-07-07 10:27:44.870578 mech_client-0.2.2/mech_client/wss.py
+-rw-r--r--   0        0        0     1469 2023-07-07 10:27:44.870578 mech_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 mech_client-0.2.2/PKG-INFO
```

### Comparing `mech_client-0.2.1/LICENSE` & `mech_client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/README.md` & `mech_client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/acn.py` & `mech_client-0.2.2/mech_client/acn.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/cli.py` & `mech_client-0.2.2/mech_client/cli.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/__init__.py` & `mech_client-0.2.2/mech_client/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/README.md` & `mech_client-0.2.2/mech_client/helpers/acn/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/__init__.py` & `mech_client-0.2.2/mech_client/helpers/acn/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/acn.proto` & `mech_client-0.2.2/mech_client/helpers/acn/acn.proto`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/acn_pb2.py` & `mech_client-0.2.2/mech_client/helpers/acn/acn_pb2.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/custom_types.py` & `mech_client-0.2.2/mech_client/helpers/acn/custom_types.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/dialogues.py` & `mech_client-0.2.2/mech_client/helpers/acn/dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/message.py` & `mech_client-0.2.2/mech_client/helpers/acn/message.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/protocol.yaml` & `mech_client-0.2.2/mech_client/helpers/acn/protocol.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/serialization.py` & `mech_client-0.2.2/mech_client/helpers/acn/serialization.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/tests/__init__.py` & `mech_client-0.2.2/mech_client/helpers/acn/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn.py` & `mech_client-0.2.2/mech_client/helpers/acn/tests/test_acn.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn_dialogues.py` & `mech_client-0.2.2/mech_client/helpers/acn/tests/test_acn_dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn/tests/test_acn_messages.py` & `mech_client-0.2.2/mech_client/helpers/acn/tests/test_acn_messages.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/README.md` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/__init__.py` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/acn_data_share_pb2.py` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/acn_data_share_pb2.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/dialogues.py` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/message.py` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/message.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/protocol.yaml` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/protocol.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/serialization.py` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/serialization.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/tests/test_acn_data_share_dialogues.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py` & `mech_client-0.2.2/mech_client/helpers/acn_data_share/tests/test_acn_data_share_messages.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/README.md` & `mech_client-0.2.2/mech_client/helpers/p2p_libp2p_client/README.md`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/__init__.py` & `mech_client-0.2.2/mech_client/helpers/p2p_libp2p_client/__init__.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/connection.py` & `mech_client-0.2.2/mech_client/helpers/p2p_libp2p_client/connection.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/helpers/p2p_libp2p_client/connection.yaml` & `mech_client-0.2.2/mech_client/helpers/p2p_libp2p_client/connection.yaml`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/interact.py` & `mech_client-0.2.2/mech_client/interact.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,28 +271,30 @@
 
 def interact(
     prompt: str,
     agent_id: int,
     tool: Optional[str] = None,
     private_key_path: Optional[str] = None,
     confirmation_type: ConfirmationType = ConfirmationType.WAIT_FOR_BOTH,
-) -> None:
+) -> Any:
     """
     Interact with agent mech contract.
 
     :param prompt: The interaction prompt.
     :type prompt: str
     :param agent_id: The ID of the agent.
     :type agent_id: int
     :param tool: The tool to interact with (optional).
     :type tool: Optional[str]
     :param private_key_path: The path to the private key file (optional).
     :type private_key_path: Optional[str]
     :param confirmation_type: The confirmation type for the interaction (default: ConfirmationType.WAIT_FOR_BOTH).
     :type confirmation_type: ConfirmationType
+    :return: The data received from on-chain/off-chain.
+    :rtype: Any
     """
     contract_address = query_agent_address(agent_id=agent_id)
     if contract_address is None:
         raise ValueError(f"Agent with ID {agent_id} does not exist!")
 
     private_key_path = private_key_path or PRIVATE_KEY_FILE_PATH
     if not Path(private_key_path).exists():
@@ -336,7 +338,8 @@
             mech_contract=mech_contract,
             ledger_api=ledger_api,
             crypto=crypto,
         )
     print(f"Data arrived: {data_url}")
     data = requests.get(f"{data_url}/{request_id}").json()
     print(f"Data from agent: {data}")
+    return data
```

### Comparing `mech_client-0.2.1/mech_client/prompt_to_ipfs.py` & `mech_client-0.2.2/mech_client/prompt_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/push_to_ipfs.py` & `mech_client-0.2.2/mech_client/push_to_ipfs.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/subgraph.py` & `mech_client-0.2.2/mech_client/subgraph.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/to_png.py` & `mech_client-0.2.2/mech_client/to_png.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/mech_client/wss.py` & `mech_client-0.2.2/mech_client/wss.py`

 * *Files identical despite different names*

### Comparing `mech_client-0.2.1/pyproject.toml` & `mech_client-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mech-client"
-version = "0.2.1"
+version = "0.2.2"
 description = "Basic client to interact with a mech"
 authors = ["David Minarsch <david.minarsch@googlemail.com>"]
 readme = "README.md"
 packages = [{include = "mech_client"}]
 license = "Apache-2.0"
 include = [
     "mech_client/helpers/acn/*",
```

### Comparing `mech_client-0.2.1/PKG-INFO` & `mech_client-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mech-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Basic client to interact with a mech
 License: Apache-2.0
 Author: David Minarsch
 Author-email: david.minarsch@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

