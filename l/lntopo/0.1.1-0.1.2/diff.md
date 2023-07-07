# Comparing `tmp/lntopo-0.1.1.tar.gz` & `tmp/lntopo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lntopo-0.1.1.tar", max compression
+gzip compressed data, was "lntopo-0.1.2.tar", max compression
```

## Comparing `lntopo-0.1.1.tar` & `lntopo-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1067 2020-10-12 12:00:47.000000 lntopo-0.1.1/LICENSE
--rw-r--r--   0        0        0      156 2021-09-20 14:07:48.254348 lntopo-0.1.1/lntopo/__main__.py
--rw-r--r--   0        0        0     1289 2021-09-20 14:07:42.506272 lntopo-0.1.1/lntopo/common.py
--rw-r--r--   0        0        0     7577 2020-12-16 13:15:57.000000 lntopo-0.1.1/lntopo/parser.py
--rw-r--r--   0        0        0     4814 2021-09-20 14:07:35.502180 lntopo-0.1.1/lntopo/timemachine.py
--rw-r--r--   0        0        0      421 2021-09-26 14:31:18.759278 lntopo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      764 2021-09-26 14:31:55.928263 lntopo-0.1.1/setup.py
--rw-r--r--   0        0        0      445 2021-09-26 14:31:55.928511 lntopo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-06 15:58:30.119330 lntopo-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1523 2023-07-06 15:58:30.119330 lntopo-0.1.2/lntopo/__main__.py
+-rw-r--r--   0        0        0     2264 2023-07-06 15:58:30.119330 lntopo-0.1.2/lntopo/common.py
+-rw-r--r--   0        0        0     9942 2023-07-06 15:58:30.119330 lntopo-0.1.2/lntopo/parser.py
+-rw-r--r--   0        0        0     5008 2023-07-06 15:58:30.119330 lntopo-0.1.2/lntopo/timemachine.py
+-rw-r--r--   0        0        0      438 2023-07-07 10:18:46.007091 lntopo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lntopo-0.1.2/PKG-INFO
```

### Comparing `lntopo-0.1.1/LICENSE` & `lntopo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lntopo-0.1.1/lntopo/parser.py` & `lntopo-0.1.2/lntopo/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from binascii import hexlify
 
 
 import io
 import struct
+import ipaddress
 
 
 class ChannelAnnouncement(object):
     def __init__(self):
         self.num_short_channel_id = None
         self.node_signatures = [None, None]
         self.bitcoin_signatures = [None, None]
@@ -38,14 +39,24 @@
     def __str__(self):
         na = hexlify(self.node_ids[0]).decode("ASCII")
         nb = hexlify(self.node_ids[1]).decode("ASCII")
         return "ChannelAnnouncement(scid={short_channel_id}, nodes=[{na},{nb}])".format(
             na=na, nb=nb, short_channel_id=self.short_channel_id
         )
 
+    def __json__(self):
+        return {
+            '_type': 'channel_announcement',
+            'scid': self.short_channel_id,
+            'features': hexlify(self.features).decode('ASCII'),
+            'node_id_1': hexlify(self.node_ids[0]).decode('ASCII'),
+            'node_id_2': hexlify(self.node_ids[1]).decode('ASCII'),
+            'chain_hash': hexlify(self.chain_hash).decode('ASCII'),
+        }
+
 
 class ChannelUpdate(object):
     def __init__(self):
         self.signature = None
         self.chain_hash = None
         self.num_short_channel_id = None
         self.timestamp = None
@@ -53,14 +64,29 @@
         self.channel_flags = None
         self.cltv_expiry_delta = None
         self.htlc_minimum_msat = None
         self.fee_base_msat = None
         self.fee_proportional_millionths = None
         self.htlc_maximum_msat = None
 
+    def __json__(self):
+        return {
+            '_type': 'channel_update',
+            'scid': self.short_channel_id,
+            'timestamp': self.timestamp,
+            'message_flags': hexlify(self.message_flags).decode('ASCII'),
+            'channel_flags': hexlify(self.channel_flags).decode('ASCII'),
+            'cltv_expiry_delta': self.cltv_expiry_delta,
+            'htlc_minimum_msat': self.htlc_minimum_msat,
+            'fee_base_msat': self.fee_base_msat,
+            'fee_proportional_millionths': self.fee_proportional_millionths,
+            'htlc_maximum_msat': self.htlc_maximum_msat,
+            'chain_hash': hexlify(self.chain_hash).decode('ASCII'),
+        }
+
     @property
     def short_channel_id(self):
         return "{}x{}x{}".format(
             (self.num_short_channel_id >> 40) & 0xFFFFFF,
             (self.num_short_channel_id >> 16) & 0xFFFFFF,
             (self.num_short_channel_id >> 00) & 0xFF,
         )
@@ -123,15 +149,16 @@
         protos = {
             1: "ipv4",
             2: "ipv6",
             3: "torv2",
             4: "torv3",
         }
 
-        return f"{protos[self.typ]}://{addr}:{self.port}"
+        proto = protos.get(self.typ, 'UNKNOWN')
+        return f"{proto}://{addr}:{self.port}"
 
 
 class NodeAnnouncement(object):
     def __init__(self):
         self.signature = None
         self.features = ""
         self.timestamp = None
@@ -150,14 +177,24 @@
             self.features == other.features
             and self.timestamp == other.timestamp
             and self.node_id == other.node_id
             and self.rgb_color == other.rgb_color
             and self.alias == other.alias
         )
 
+    def __json__(self):
+        return {
+            '_type': 'node_announcement',
+            'features': self.features.hex(),
+            'timestamp': self.timestamp,
+            'node_id': self.node_id.hex(),
+            'rgb_color': self.rgb_color.hex(),
+            'addresses': []  # TODO Add missing addresses
+        }
+
 
 def parse(b):
     if not isinstance(b, io.BytesIO):
         b = io.BytesIO(b)
     (typ,) = struct.unpack("!H", b.read(2))
 
     parsers = {
@@ -226,25 +263,54 @@
         return None
 
     a = Address()
     (a.typ,) = struct.unpack("!B", t)
 
     if a.typ == 1:
         a.addr = b.read(4)
+        (a.port,) = struct.unpack("!H", b.read(2))
     elif a.typ == 2:
         a.addr = b.read(16)
+        a.addr = '[' + format(ipaddress.IPv6Address(a.addr)) + ']'
+        (a.port,) = struct.unpack("!H", b.read(2))
     elif a.typ == 3:
         a.addr = b.read(10)
+        a.addr = to_base_32(a.addr) + '.onion'
+        (a.port,) = struct.unpack("!H", b.read(2))
     elif a.typ == 4:
         a.addr = b.read(35)
+        a.addr = to_base_32(a.addr) + '.onion'
+        (a.port,) = struct.unpack("!H", b.read(2))
     else:
-        raise ValueError("Unknown address type {typ}".format(typ=a.typ))
-    (a.port,) = struct.unpack("!H", b.read(2))
+        a.addr = b.getvalue()[1:]
+        a.port = None
     return a
 
+# https://github.com/alexbosworth/bolt07/blob/519c94a7837e687bf7478a74779d5ea493a76a44/addresses/encode_base32.js
+def to_base_32(addr):
+    alphabet = 'abcdefghijklmnopqrstuvwxyz234567'
+    byte = 8
+    lastIndex = 31
+    word = 5
+    bits = 0
+    base32 = ''
+    value = 0
+
+    for char in addr:
+        bits += byte
+        value = (value << byte) | char
+
+        while bits >= word:
+            base32 += alphabet[(value >> (bits - word)) & lastIndex]
+            bits -= word
+
+    if bits > 0:
+        base32 += alphabet[(value << (word - bits)) & lastIndex]
+    
+    return base32
 
 def parse_node_announcement(b):
     if not isinstance(b, io.BytesIO):
         b = io.BytesIO(b)
 
     na = NodeAnnouncement()
     na.signature = b.read(64)
```

### Comparing `lntopo-0.1.1/lntopo/timemachine.py` & `lntopo-0.1.2/lntopo/timemachine.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 import time
 from .common import DatasetFile
 import click
 import networkx as nx
 from .parser import ChannelAnnouncement, ChannelUpdate, NodeAnnouncement
 from tqdm import tqdm
 from datetime import datetime
+import json
+from networkx.readwrite import json_graph
 
 
 @click.group()
 def timemachine():
     pass
 
 
 @timemachine.command()
 @click.argument("dataset", type=DatasetFile())
 @click.argument("timestamp", type=int, required=False)
-@click.option('--fmt', type=click.Choice(['dot', 'gml', 'graphml'], case_sensitive=False))
+@click.option('--fmt', type=click.Choice(['dot', 'gml', 'graphml', 'json'], case_sensitive=False))
 def restore(dataset, timestamp=None, fmt='dot'):
     """Restore reconstructs the network topology at a specific time in the past.
 
     Restore replays gossip messages from a dataset and reconstructs
     the network as it would have looked like at the specified
     timestamp in the past. The network is then printed to stdout using
     the format specified with `--fmt`.
@@ -141,9 +143,12 @@
         print(nx.nx_pydot.to_pydot(g))
 
     elif fmt == 'gml':
         for line in nx.generate_gml(g):
             print(line)
 
     elif fmt == 'graphml':
-        for line in nx.generate_graphml(g):
+        for line in nx.generate_graphml(g, named_key_ids=True, edge_id_from_attribute='scid'):
             print(line)
+
+    elif fmt == 'json':
+        print(json.dumps(json_graph.adjacency_data(g)))
```

