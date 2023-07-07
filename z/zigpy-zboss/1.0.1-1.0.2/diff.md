# Comparing `tmp/zigpy-zboss-1.0.1.tar.gz` & `tmp/zigpy-zboss-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-zboss-1.0.1.tar", last modified: Mon May 15 14:54:13 2023, max compression
+gzip compressed data, was "zigpy-zboss-1.0.2.tar", last modified: Fri Jul  7 16:15:02 2023, max compression
```

## Comparing `zigpy-zboss-1.0.1.tar` & `zigpy-zboss-1.0.2.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:54:13.066800 zigpy-zboss-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-15 14:54:13.066800 zigpy-zboss-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-15 14:54:13.066800 zigpy-zboss-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:54:13.058800 zigpy-zboss-1.0.1/zigpy_zboss/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:54:13.062800 zigpy-zboss-1.0.1/zigpy_zboss/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/commands/af.py
--rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/commands/aps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16390 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/commands/ncp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/commands/nwk_mgmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/commands/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/commands/zdo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:54:13.062800 zigpy-zboss-1.0.1/zigpy_zboss/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/tools/factory_reset_ncp.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/tools/get_ncp_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:54:13.062800 zigpy-zboss-1.0.1/zigpy_zboss/types/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/types/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/types/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/types/named.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/types/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/uart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:54:13.066800 zigpy-zboss-1.0.1/zigpy_zboss/zigbee/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/zigbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22719 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/zigbee/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2023-05-15 14:54:02.000000 zigpy-zboss-1.0.1/zigpy_zboss/zigbee/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:54:13.058800 zigpy-zboss-1.0.1/zigpy_zboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-15 14:54:13.000000 zigpy-zboss-1.0.1/zigpy_zboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 14:54:13.000000 zigpy-zboss-1.0.1/zigpy_zboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:54:13.000000 zigpy-zboss-1.0.1/zigpy_zboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-15 14:54:13.000000 zigpy-zboss-1.0.1/zigpy_zboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 14:54:13.000000 zigpy-zboss-1.0.1/zigpy_zboss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.345413 zigpy-zboss-1.0.2/zigpy_zboss/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.345413 zigpy-zboss-1.0.2/zigpy_zboss/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/af.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/aps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16006 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/ncp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/nwk_mgmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/commands/zdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/nvram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.345413 zigpy-zboss-1.0.2/zigpy_zboss/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/tools/factory_reset_ncp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/tools/get_ncp_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/zigpy_zboss/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21600 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/nvids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/types/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.349413 zigpy-zboss-1.0.2/zigpy_zboss/zigbee/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/zigbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/zigbee/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-07-07 16:14:53.000000 zigpy-zboss-1.0.2/zigpy_zboss/zigbee/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 16:15:02.345413 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 16:15:02.000000 zigpy-zboss-1.0.2/zigpy_zboss.egg-info/top_level.txt
```

### Comparing `zigpy-zboss-1.0.1/COPYING` & `zigpy-zboss-1.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/LICENSE` & `zigpy-zboss-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/pyproject.toml` & `zigpy-zboss-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/setup.cfg` & `zigpy-zboss-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/api.py` & `zigpy-zboss-1.0.2/zigpy_zboss/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import async_timeout
 import zigpy_zboss.types as t
 import zigpy_zboss.config as conf
 
 from zigpy_zboss import uart
 from zigpy_zboss.frames import Frame
 from zigpy_zboss import commands as c
+from zigpy_zboss.nvram import NVRAMHelper
 from collections import Counter, defaultdict
 from zigpy_zboss.utils import IndicationListener
 from zigpy_zboss.utils import BaseResponseListener
 from zigpy_zboss.utils import OneShotResponseListener
 
 LOGGER = logging.getLogger(__name__)
 
@@ -39,14 +40,15 @@
         self._config = config
 
         self._listeners = defaultdict(list)
         self._blocking_request_lock = asyncio.Lock()
 
         self.capabilities = None
 
+        self.nvram = NVRAMHelper(self)
         self.network_info: zigpy.state.NetworkInformation = None
         self.node_info: zigpy.state.NodeInfo = None
 
         self._ncp_debug = None
 
     def set_application(self, app):
         """Set the application using the NRF class."""
```

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/checksum.py` & `zigpy-zboss-1.0.2/zigpy_zboss/checksum.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/commands/__init__.py` & `zigpy-zboss-1.0.2/zigpy_zboss/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/commands/af.py` & `zigpy-zboss-1.0.2/zigpy_zboss/commands/af.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/commands/aps.py` & `zigpy-zboss-1.0.2/zigpy_zboss/commands/aps.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/commands/ncp_config.py` & `zigpy-zboss-1.0.2/zigpy_zboss/commands/ncp_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,21 +95,16 @@
         t.ControlType.REQ,
         NcpConfigCommandCode.GET_ZIGBEE_CHANNEL_MASK,
         req_schema=(
             t.Param("TSN", t.uint8_t, "Transmission Sequence Number"),
         ),
         rsp_schema=t.STATUS_SCHEMA + (
             t.Param(
-                "ChannelListLen",
-                t.uint8_t,
-                "Number of entries in the following Channel List array"
-            ),
-            t.Param(
                 "ChannelList",
-                t.EUI64,             # CREATE A TYPE FOR CHANNEL LIST ENTRY
+                t.ChannelEntryList,
                 "Array of ChannelListEntry structures"
             ),
         ),
     )
     SetChannelMask = t.CommandDef(
         t.ControlType.REQ,
         NcpConfigCommandCode.SET_ZIGBEE_CHANNEL_MASK,
@@ -395,34 +390,29 @@
     #             t.uint8_t,
     #             "A number of datasets contained in this request"
     #         ),
     #         t.Param("Data", ???, "Data bytes array"),
     #     ),
     #     rsp_schema=t.STATUS_SCHEMA,
     # )
-    # ReadNVRAM = t.CommandDef(
-    #     t.ControlType.REQ,
-    #     NcpConfigCommandCode.NVRAM_READ,
-    #     blocking=True,
-    #     req_schema=(
-    #         t.Param("TSN", t.uint8_t, "Transmission Sequence Number"),
-    #         t.Param("DatasetType", t.uint8_t, "A dataset type to read"),
-    #     ),
-    #     rsp_schema=t.STATUS_SCHEMA + (
-    #         t.Param("NVRAMVersion", t.uint16_t, "Current NVRAM version"),
-    #         t.Param("DatasetType", t.uint16_t, "Requested dataset type"),
-    #         t.Param("DatasetVersion", t.uint16_t, "Current dataset version"),
-    #         t.Param(
-    #             "DatasetLength",
-    #             t.uint16_t,
-    #             "Length of the requested dataset"
-    #         ),
-    #         t.Param("Data", ???, "Data bytes array"),
-    #     ),
-    # )
+    ReadNVRAM = t.CommandDef(
+        t.ControlType.REQ,
+        NcpConfigCommandCode.NVRAM_READ,
+        blocking=True,
+        req_schema=(
+            t.Param("TSN", t.uint8_t, "Transmission Sequence Number"),
+            t.Param("DatasetId", t.uint16_t, "A dataset type to read"),
+        ),
+        rsp_schema=t.STATUS_SCHEMA + (
+            t.Param("NVRAMVersion", t.uint16_t, "Current NVRAM version"),
+            t.Param("DatasetId", t.DatasetId, "Requested dataset type"),
+            t.Param("DatasetVersion", t.uint16_t, "Current dataset version"),
+            t.Param("Dataset", t.NVRAMDataset, "Data bytes array"),
+        ),
+    )
     EraseNVRAM = t.CommandDef(
         t.ControlType.REQ,
         NcpConfigCommandCode.NVRAM_ERASE,
         blocking=True,
         req_schema=(
             t.Param("TSN", t.uint8_t, "Transmission Sequence Number"),
         ),
```

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/commands/nwk_mgmt.py` & `zigpy-zboss-1.0.2/zigpy_zboss/commands/nwk_mgmt.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/commands/security.py` & `zigpy-zboss-1.0.2/zigpy_zboss/commands/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/commands/zdo.py` & `zigpy-zboss-1.0.2/zigpy_zboss/commands/zdo.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,14 +297,52 @@
                 "ActiveEpList",
                 zigpy.types.LVBytes,
                 "Active enpoints list"
             ),
             t.Param("NwkAddr", t.NWK, "Network address of source device"),
         ),
     )
+    MatchDescReq = t.CommandDef(
+        t.ControlType.REQ,
+        ZdoCommandCode.ZDO_MATCH_DESC_REQ,
+        blocking=False,
+        req_schema=(
+            t.Param("TSN", t.uint8_t, "Transmission Sequence Number"),
+            t.Param("NwkAddr", t.NWK, "Network address of interest"),
+            t.Param("ProfileId", t.uint16_t, "ID of the profile of interest"),
+            t.Param(
+                "InClusterCnt",
+                t.uint8_t,
+                "Count of Input cluster IDs in the following list"
+            ),
+            t.Param(
+                "OutClusterCnt",
+                t.uint8_t,
+                "Count of Output cluster IDs in the following list"
+            ),
+            t.Param(
+                "InClusterList",
+                t.List[t.uint16_t],
+                "Network address of interest"
+            ),
+            t.Param(
+                "OutClusterList",
+                t.List[t.uint16_t],
+                "Network address of interest"
+            ),
+        ),
+        rsp_schema=t.STATUS_SCHEMA + (
+            t.Param(
+                "ActiveEpList",
+                zigpy.types.LVBytes,
+                "Active enpoints list"
+            ),
+            t.Param("NwkAddr", t.NWK, "Network address of source device"),
+        ),
+    )
     SimpleDescriptorReq = t.CommandDef(
         t.ControlType.REQ,
         ZdoCommandCode.ZDO_SIMPLE_DESC_REQ,
         blocking=True,
         req_schema=(
             t.Param("TSN", t.uint8_t, "Transmission Sequence Number"),
             t.Param("NwkAddr", t.NWK, "Network address of interest"),
```

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/config.py` & `zigpy-zboss-1.0.2/zigpy_zboss/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/debug.py` & `zigpy-zboss-1.0.2/zigpy_zboss/debug.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/frames.py` & `zigpy-zboss-1.0.2/zigpy_zboss/frames.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/logger.py` & `zigpy-zboss-1.0.2/zigpy_zboss/logger.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/tools/config.py` & `zigpy-zboss-1.0.2/zigpy_zboss/tools/config.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/tools/factory_reset_ncp.py` & `zigpy-zboss-1.0.2/zigpy_zboss/tools/factory_reset_ncp.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/tools/get_ncp_version.py` & `zigpy-zboss-1.0.2/zigpy_zboss/tools/get_ncp_version.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/types/basic.py` & `zigpy-zboss-1.0.2/zigpy_zboss/types/basic.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/types/commands.py` & `zigpy-zboss-1.0.2/zigpy_zboss/types/commands.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/types/cstruct.py` & `zigpy-zboss-1.0.2/zigpy_zboss/types/cstruct.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/types/named.py` & `zigpy-zboss-1.0.2/zigpy_zboss/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/types/structs.py` & `zigpy-zboss-1.0.2/zigpy_zboss/types/structs.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/uart.py` & `zigpy-zboss-1.0.2/zigpy_zboss/uart.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/utils.py` & `zigpy-zboss-1.0.2/zigpy_zboss/utils.py`

 * *Files identical despite different names*

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/zigbee/application.py` & `zigpy-zboss-1.0.2/zigpy_zboss/zigbee/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import zigpy.config
 import zigpy.device
 import async_timeout
 import zigpy.endpoint
 import zigpy.exceptions
 import zigpy.types as t
 import zigpy.application
-import zigpy_zboss.types as t_nrf
+import zigpy_zboss.types as t_zboss
 import zigpy.zdo.types as zdo_t
 import zigpy_zboss.config as conf
 
 from typing import Any, Dict
 from zigpy_zboss.api import NRF
 from zigpy_zboss import commands as c
 from zigpy.exceptions import DeliveryError
@@ -82,15 +82,15 @@
 
     async def force_remove(self, dev: zigpy.device.Device) -> None:
         """Send a lower-level leave command to the device."""
         # ZBOSS NCP does not have any way to do this
 
     async def add_endpoint(self, descriptor: zdo_t.SimpleDescriptor) -> None:
         """Register a new endpoint on the device."""
-        simple_desc = t_nrf.SimpleDescriptor(
+        simple_desc = t_zboss.SimpleDescriptor(
             endpoint=descriptor.endpoint,
             profile=descriptor.profile,
             device_type=descriptor.device_type,
             device_version=descriptor.device_version,
             input_clusters=descriptor.input_clusters,
             output_clusters=descriptor.output_clusters,
         )
@@ -105,15 +105,15 @@
         self._send_sequence = (self._send_sequence + 1) % 255
         return self._send_sequence
 
     def get_default_stack_specific_formation_settings(self):
         """Populate stack specific config dictionary with default values."""
         return {
             "rx_on_when_idle": t.Bool.true,
-            "end_device_timeout": t_nrf.TimeoutIndex.Minutes_256,
+            "end_device_timeout": t_zboss.TimeoutIndex.Minutes_256,
             "max_children": t.uint8_t(100),
             "joined": t.Bool.false,
             "authenticated": t.Bool.false,
             "parent_nwk": None,
             "coordinator_version": None,
             "tc_policy": {
                 "unique_tclk_required": t.Bool.false,
@@ -140,15 +140,15 @@
                 IEEE=node_info.ieee
             )
         )
 
         await self._api.request(
             request=c.NcpConfig.SetZigbeeRole.Req(
                 TSN=self.get_sequence(),
-                DeviceRole=t_nrf.DeviceRole.ZC
+                DeviceRole=t_zboss.DeviceRole.ZC
             )
         )
 
         await self._api.request(
             request=c.NcpConfig.SetExtendedPANID.Req(
                 TSN=self.get_sequence(),
                 ExtendedPANID=network_info.extended_pan_id
@@ -200,74 +200,74 @@
                     "max_children"]
             )
         )
 
         await self._api.request(
             request=c.NcpConfig.SetTCPolicy.Req(
                 TSN=self.get_sequence(),
-                PolicyType=t_nrf.PolicyType.TC_Link_Keys_Required,
+                PolicyType=t_zboss.PolicyType.TC_Link_Keys_Required,
                 PolicyValue=network_info.stack_specific[
                     "tc_policy"]["unique_tclk_required"]
             )
         )
 
         await self._api.request(
             request=c.NcpConfig.SetTCPolicy.Req(
                 TSN=self.get_sequence(),
-                PolicyType=t_nrf.PolicyType.IC_Required,
+                PolicyType=t_zboss.PolicyType.IC_Required,
                 PolicyValue=network_info.stack_specific[
                     "tc_policy"]["ic_required"]
             )
         )
 
         await self._api.request(
             request=c.NcpConfig.SetTCPolicy.Req(
                 TSN=self.get_sequence(),
-                PolicyType=t_nrf.PolicyType.TC_Rejoin_Enabled,
+                PolicyType=t_zboss.PolicyType.TC_Rejoin_Enabled,
                 PolicyValue=network_info.stack_specific[
                     "tc_policy"]["tc_rejoin_enabled"]
             )
         )
 
         await self._api.request(
             request=c.NcpConfig.SetTCPolicy.Req(
                 TSN=self.get_sequence(),
-                PolicyType=t_nrf.PolicyType.Ignore_TC_Rejoin,
+                PolicyType=t_zboss.PolicyType.Ignore_TC_Rejoin,
                 PolicyValue=network_info.stack_specific[
                     "tc_policy"]["tc_rejoin_ignored"]
             )
         )
 
         await self._api.request(
             request=c.NcpConfig.SetTCPolicy.Req(
                 TSN=self.get_sequence(),
-                PolicyType=t_nrf.PolicyType.APS_Insecure_Join,
+                PolicyType=t_zboss.PolicyType.APS_Insecure_Join,
                 PolicyValue=network_info.stack_specific[
                     "tc_policy"]["aps_insecure_join_enabled"]
             )
         )
 
         await self._api.request(
             request=c.NcpConfig.SetTCPolicy.Req(
                 TSN=self.get_sequence(),
-                PolicyType=t_nrf.PolicyType.Disable_NWK_MGMT_Channel_Update,
+                PolicyType=t_zboss.PolicyType.Disable_NWK_MGMT_Channel_Update,
                 PolicyValue=network_info.stack_specific[
                     "tc_policy"]["mgmt_channel_update_disabled"]
             )
         )
 
         await self._form_network(network_info)
 
     async def _form_network(self, network_info):
         """Clear the current config and forms a new network."""
         await self._api.request(
             request=c.NWK.Formation.Req(
                 TSN=self.get_sequence(),
-                ChannelList=t_nrf.ChannelEntryList([
-                    t_nrf.ChannelEntry(
+                ChannelList=t_zboss.ChannelEntryList([
+                    t_zboss.ChannelEntry(
                         page=0, channel_mask=network_info.channel_mask)
                 ]),
                 ScanDuration=0x05,
                 DistributedNetFlag=0x00,
                 DistributedNetAddr=t.NWK(0x0000),
                 IEEEAddr=network_info.extended_pan_id
             )
@@ -302,23 +302,22 @@
 
         res = await self._api.request(
             c.NcpConfig.GetShortPANID.Req(TSN=self.get_sequence()))
         self.state.network_info.pan_id = res.PANID
 
         self.state.network_info.nwk_update_id = self.config[
             conf.CONF_NWK][conf.CONF_NWK_UPDATE_ID]
-        self.state.network_info.nwk_manager_id = 0x0000
 
         res = await self._api.request(
             c.NcpConfig.GetCurrentChannel.Req(TSN=self.get_sequence()))
         self.state.network_info.channel = res.Channel
 
-        # res = await self._api.request(
-        #     c.NcpConfig.GetChannelMask.Req(TSN=self.get_sequence()))
-        # self.state.network_info.channel_mask = res.ChannelList[0]
+        res = await self._api.request(
+            c.NcpConfig.GetChannelMask.Req(TSN=self.get_sequence()))
+        self.state.network_info.channel_mask = res.ChannelList[0].channel_mask
 
         self.state.network_info.security_level = 0x05
 
         res = await self._api.request(
             c.NcpConfig.GetNwkKeys.Req(TSN=self.get_sequence()))
         self.state.network_info.network_key = zigpy.state.Key(
             key=res.NwkKey1,
@@ -346,18 +345,14 @@
                     tx_counter=0,
                     rx_counter=0,
                     seq=0,
                     partner_ieee=res.TCIEEE,
                 ),
             )
 
-        self.state.network_info.key_table = []
-        self.state.network_info.children = []
-        self.state.network_info.nwk_address = {}
-
         res = await self._api.request(
             c.NcpConfig.GetRxOnWhenIdle.Req(TSN=self.get_sequence()))
         self.state.network_info.stack_specific[
             "rx_on_when_idle"
         ] = res.RxOnWhenIdle
 
         res = await self._api.request(
@@ -395,14 +390,34 @@
         self.state.network_info.stack_specific[
             "coordinator_version"
         ] = res.CoordinatorVersion
 
         if not load_devices:
             return
 
+        map = await self._api.nvram.read(
+                t_zboss.DatasetId.ZB_NVRAM_ADDR_MAP,
+                t_zboss.NwkAddrMap
+            )
+        for rec in map:
+            if rec.nwk_addr == 0x0000:
+                continue
+            self.state.network_info.children.append(rec.ieee_addr)
+            self.state.network_info.nwk_addresses[rec.ieee_addr] = rec.nwk_addr
+
+        keys = await self._api.nvram.read(
+            t_zboss.DatasetId.ZB_NVRAM_APS_SECURE_DATA,
+            t_zboss.ApsSecureKeys
+        )
+        for key_entry in keys:
+            zigpy_key = zigpy.state.Key()
+            zigpy_key.key = t.KeyData(key_entry.key)
+            zigpy_key.partner_ieee = key_entry.ieee_addr
+            self.state.network_info.key_table.append(zigpy_key)
+
     async def reset_network_info(self) -> None:
         """Reset node network information and leaves the current network."""
         pass
 
     async def start_without_formation(self):
         """Start the network with settings currently stored on the module."""
         res = await self._api.request(
@@ -490,34 +505,34 @@
 
     def on_zdo_device_announcement(self, msg: c.ZDO.DevAnnceInd.Ind):
         """ZDO Device announcement command received."""
         self.handle_join(nwk=msg.NWK, ieee=msg.IEEE, parent_nwk=None)
 
     def on_dev_update(self, msg: c.ZDO.DevUpdateInd.Ind):
         """Device update indication."""
-        if msg.Status == t_nrf.DeviceUpdateStatus.secured_rejoin:
+        if msg.Status == t_zboss.DeviceUpdateStatus.secured_rejoin:
             # 0x000 as parent device, currently unused
             pass
             # self.handle_join(msg.Nwk, msg.IEEE, 0x0000)
-        elif msg.Status == t_nrf.DeviceUpdateStatus.unsecured_join:
+        elif msg.Status == t_zboss.DeviceUpdateStatus.unsecured_join:
             # 0x000 as parent device, currently unused
             pass
             # self.handle_join(msg.Nwk, msg.IEEE, 0x0000)
-        elif msg.Status == t_nrf.DeviceUpdateStatus.device_left:
+        elif msg.Status == t_zboss.DeviceUpdateStatus.device_left:
             pass
             # self.handle_leave(msg.Nwk, msg.IEEE)
-        elif msg.Status == t_nrf.DeviceUpdateStatus.tc_rejoin:
+        elif msg.Status == t_zboss.DeviceUpdateStatus.tc_rejoin:
             pass
             # self.handle_join(msg.Nwk, msg.IEEE, 0x0000)
 
     def on_apsde_indication(self, msg):
         """APSDE-DATA.indication handler."""
-        is_broadcast = bool(msg.FrameFC & t_nrf.APSFrameFC.Broadcast)
-        is_group = bool(msg.FrameFC & t_nrf.APSFrameFC.Group)
-        is_secure = bool(msg.FrameFC & t_nrf.APSFrameFC.Secure)
+        is_broadcast = bool(msg.FrameFC & t_zboss.APSFrameFC.Broadcast)
+        is_group = bool(msg.FrameFC & t_zboss.APSFrameFC.Group)
+        is_secure = bool(msg.FrameFC & t_zboss.APSFrameFC.Secure)
 
         if is_broadcast:
             dst = t.AddrModeAddress(
                 addr_mode=t.AddrMode.Broadcast,
                 address=t.BroadcastAddress.ALL_ROUTERS_AND_COORDINATOR,
             )
         elif is_group:
@@ -552,15 +567,15 @@
             ),
         )
 
         self.packet_received(packet)
 
     def on_ncp_reset(self, msg):
         """NCP_RESET.indication handler."""
-        if msg.ResetSrc == t_nrf.ResetSource.RESET_SRC_POWER_ON:
+        if msg.ResetSrc == t_zboss.ResetSource.RESET_SRC_POWER_ON:
             return
         LOGGER.debug(
             f"Resetting ControllerApplication. Source: {msg.ResetSrc}")
         if self._reset_task:
             LOGGER.debug("Preempting ControllerApplication reset")
             self._reset_task.cancel()
 
@@ -622,10 +637,10 @@
                     SrcEndpoint=packet.src_ep,
                     Radius=packet.radius or 0,
                     DstAddrMode=dst_addr_mode,
                     TxOptions=options,
                     UseAlias=t.Bool.false,
                     AliasSrcAddr=t.NWK(0x0000),
                     AliasSeqNbr=t.uint8_t(0x00),
-                    Payload=t_nrf.Payload(packet.data.serialize()),
+                    Payload=t_zboss.Payload(packet.data.serialize()),
                 )
             )
```

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss/zigbee/device.py` & `zigpy-zboss-1.0.2/zigpy_zboss/zigbee/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Zigbee device object."""
+import logging
 import zigpy.util
 import zigpy.device
 import zigpy.endpoint
 import zigpy.types as t
 import zigpy_zboss.types as t_nrf
 from zigpy_zboss import commands as c
 from zigpy.zdo import types as zdo_t
@@ -29,31 +30,25 @@
             hdr,
             (permit_duration, tc_significance),
         )
 
     @zigpy.util.retryable_request
     async def Bind_req(self, eui64, ep, cluster, dst_address):
         """Binding request."""
-        if dst_address.addrmode == t.Addressing.AddrMode.IEEE:
-            addr_mode = t_nrf.AddressingMode.Eui64
+        if dst_address.addrmode == t.AddrMode.IEEE:
+            addr_mode = t_nrf.BindAddrMode.IEEE
             dst_eui64 = dst_address.ieee
-        elif dst_address.addrmode == t.Addressing.AddrMode.NWK:
-            addr_mode = t_nrf.AddressingMode.Nwk
-            dst_eui64 = [
-                dst_address.nwk % 0x100,
-                dst_address.nwk >> 8,
-                0,
-                0,
-                0,
-                0,
-                0,
-                0,
-            ]
-        elif dst_address.addrmode == t.Addressing.AddrMode.Group:
-            addr_mode = t_nrf.AddressingMode.Group
+        # ZBOSS does not support the NWK mode for binding
+        elif dst_address.addrmode == t.AddrMode.NWK:
+            self.log(
+                logging.WARNING,
+                "Nwk address mode is not supported for the Bind request."
+            )
+        elif dst_address.addrmode == t.AddrMode.Group:
+            addr_mode = t_nrf.BindAddrMode.Group
             dst_eui64 = [
                 dst_address.nwk % 0x100,
                 dst_address.nwk >> 8,
                 0,
                 0,
                 0,
                 0,
@@ -77,31 +72,25 @@
             return (res.StatusCode % 0xFF, dst_address, cluster)
 
         return (zdo_t.Status.SUCCESS, dst_address, cluster)
 
     @zigpy.util.retryable_request
     async def Unbind_req(self, eui64, ep, cluster, dst_address):
         """Unbinding request."""
-        if dst_address.addrmode == t.Addressing.AddrMode.IEEE:
-            addr_mode = t_nrf.AddressingMode.Eui64
+        if dst_address.addrmode == t.AddrMode.IEEE:
+            addr_mode = t_nrf.BindAddrMode.IEEE
             dst_eui64 = t.Addressing.IEEE
-        elif dst_address.addrmode == t.Addressing.AddrMode.NWK:
-            addr_mode = t_nrf.AddressingMode.Nwk
-            dst_eui64 = [
-                dst_address.nwk % 0x100,
-                dst_address.nwk >> 8,
-                0,
-                0,
-                0,
-                0,
-                0,
-                0,
-            ]
-        elif dst_address.addrmode == t.Addressing.AddrMode.Group:
-            addr_mode = t_nrf.AddressingMode.Group
+        # ZBOSS does not support the NWK mode for binding
+        elif dst_address.addrmode == t.AddrMode.NWK:
+            self.log(
+                logging.WARNING,
+                "Nwk address mode is not supported for the Unbind request."
+            )
+        elif dst_address.addrmode == t.AddrMode.Group:
+            addr_mode = t_nrf.BindAddrMode.Group
             dst_eui64 = [
                 dst_address.nwk % 0x100,
                 dst_address.nwk >> 8,
                 0,
                 0,
                 0,
                 0,
```

### Comparing `zigpy-zboss-1.0.1/zigpy_zboss.egg-info/SOURCES.txt` & `zigpy-zboss-1.0.2/zigpy_zboss.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 zigpy_zboss/api.py
 zigpy_zboss/checksum.py
 zigpy_zboss/config.py
 zigpy_zboss/debug.py
 zigpy_zboss/exceptions.py
 zigpy_zboss/frames.py
 zigpy_zboss/logger.py
+zigpy_zboss/nvram.py
 zigpy_zboss/uart.py
 zigpy_zboss/utils.py
 zigpy_zboss.egg-info/PKG-INFO
 zigpy_zboss.egg-info/SOURCES.txt
 zigpy_zboss.egg-info/dependency_links.txt
 zigpy_zboss.egg-info/requires.txt
 zigpy_zboss.egg-info/top_level.txt
@@ -31,11 +32,12 @@
 zigpy_zboss/tools/factory_reset_ncp.py
 zigpy_zboss/tools/get_ncp_version.py
 zigpy_zboss/types/__init__.py
 zigpy_zboss/types/basic.py
 zigpy_zboss/types/commands.py
 zigpy_zboss/types/cstruct.py
 zigpy_zboss/types/named.py
+zigpy_zboss/types/nvids.py
 zigpy_zboss/types/structs.py
 zigpy_zboss/zigbee/__init__.py
 zigpy_zboss/zigbee/application.py
 zigpy_zboss/zigbee/device.py
```

