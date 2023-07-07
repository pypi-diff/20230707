# Comparing `tmp/TSMasterAPI-2.1.1.tar.gz` & `tmp/TSMasterAPI-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSMasterAPI-2.1.1.tar", last modified: Sun Jun 11 05:41:50 2023, max compression
+gzip compressed data, was "TSMasterAPI-2.1.2.tar", last modified: Fri Jul  7 10:26:06 2023, max compression
```

## Comparing `TSMasterAPI-2.1.1.tar` & `TSMasterAPI-2.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 05:41:50.483279 TSMasterAPI-2.1.1/
--rw-rw-rw-   0        0        0     1024 2023-06-11 05:41:50.481859 TSMasterAPI-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-11 05:41:50.471732 TSMasterAPI-2.1.1/TSMasterAPI/
--rw-rw-rw-   0        0        0    42782 2023-05-17 06:16:11.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSBUSDriver.py
--rw-rw-rw-   0        0        0    70928 2023-06-11 05:41:15.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSCommon.py
--rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSDirver.py
--rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSEnumdefine.py
--rw-rw-rw-   0        0        0    22804 2023-05-17 05:00:47.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSFibex_parse.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSFlexRayDriver.py
--rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSLINDriver.py
--rw-rw-rw-   0        0        0   155849 2023-05-17 06:27:29.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSMasterAPI.py
--rw-rw-rw-   0        0        0    27697 2023-05-17 06:26:49.000000 TSMasterAPI-2.1.1/TSMasterAPI/TSStructure.py
--rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.1.1/TSMasterAPI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:41:50.480836 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/
--rw-rw-rw-   0        0        0     1024 2023-06-11 05:41:50.000000 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-06-11 05:41:50.000000 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 05:41:50.000000 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-11 05:41:50.000000 TSMasterAPI-2.1.1/TSMasterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.1.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 05:41:50.483279 TSMasterAPI-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1585 2023-06-11 05:41:40.000000 TSMasterAPI-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:26:06.068251 TSMasterAPI-2.1.2/
+-rw-rw-rw-   0        0        0     1024 2023-07-07 10:26:06.067235 TSMasterAPI-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2023-03-24 01:55:23.000000 TSMasterAPI-2.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-07 10:26:06.056648 TSMasterAPI-2.1.2/TSMasterAPI/
+-rw-rw-rw-   0        0        0    42874 2023-07-07 07:59:38.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSBUSDriver.py
+-rw-rw-rw-   0        0        0    72160 2023-07-07 05:19:25.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSCommon.py
+-rw-rw-rw-   0        0        0     1027 2023-05-05 03:08:12.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSDirver.py
+-rw-rw-rw-   0        0        0     4152 2023-05-05 03:08:28.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSEnumdefine.py
+-rw-rw-rw-   0        0        0    24356 2023-07-07 02:04:02.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSFibex_parse.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:20:03.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSFlexRayDriver.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 03:19:48.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSLINDriver.py
+-rw-rw-rw-   0        0        0   155849 2023-05-17 06:27:29.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSMasterAPI.py
+-rw-rw-rw-   0        0        0    32023 2023-07-07 02:04:02.000000 TSMasterAPI-2.1.2/TSMasterAPI/TSStructure.py
+-rw-rw-rw-   0        0        0       54 2023-05-05 02:52:26.000000 TSMasterAPI-2.1.2/TSMasterAPI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:26:06.066219 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-07-07 10:26:05.000000 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-07-07 10:26:05.000000 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:26:05.000000 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-07 10:26:05.000000 TSMasterAPI-2.1.2/TSMasterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11525 2023-03-24 01:33:30.000000 TSMasterAPI-2.1.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 10:26:06.068251 TSMasterAPI-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1585 2023-07-07 10:25:50.000000 TSMasterAPI-2.1.2/setup.py
```

### Comparing `TSMasterAPI-2.1.1/PKG-INFO` & `TSMasterAPI-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.1.1
+Version: 2.1.2
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.1.1/TSMasterAPI/TSBUSDriver.py` & `TSMasterAPI-2.1.2/TSMasterAPI/TSBUSDriver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:19:14
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-05-17 14:16:11
+LastEditTime: 2023-07-07 15:59:38
 github:https://github.com/sy950915/TSMasterAPI.git
 '''
 import time
 from .TSCommon import *
 
 Kbps_mapping = {
     "CAN":[[500,2000],[500,2000],[500,2000],[500,2000]],
@@ -482,19 +482,21 @@
             tsdb_get_flexray_db_frame_properties_by_db_index(db_idx,Frame_id,frame)
             Frame[frame.FName.decode('utf8')] ={}
             Frame[frame.FName.decode('utf8')]['FSlotId'] = frame.FFRSlotId
             Frame[frame.FName.decode('utf8')]['FBaseCycle'] = frame.FFRBaseCycle
             Frame[frame.FName.decode('utf8')]['FCycleRepetition'] = frame.FFRCycleRepetition
             Frame[frame.FName.decode('utf8')]['FDLC'] = frame.FFRDLC
             Frame[frame.FName.decode('utf8')]['Signals'] = {}
+            if frame.FName.decode('utf8') == "CemBackBoneFr02":
+                print(1)
             for singal_index in range(frame.FSignalCount):
                 Signal = TDBSignalProperties()
                 tsdb_get_flexray_db_signal_properties_by_frame_index(db_idx,Frame_id,singal_index,Signal)
                 Frame[frame.FName.decode('utf8')]['Signals'][Signal.FName.decode('utf8')] = {}
-                Frame[frame.FName.decode('utf8')]['Signals'][Signal.FName.decode('utf8')]['def'] =Signal.FFlexRaySignal
+                Frame[frame.FName.decode('utf8')]['Signals'][Signal.FName.decode('utf8')]['def'] = Signal.FFlexRaySignal
                 Frame[frame.FName.decode('utf8')]['Signals'][Signal.FName.decode('utf8')]['value'] = 0
                 del Signal
             del frame
     elif msgType == MSGType.CANMSG or msgType == MSGType.CANFDMSG:
         tsdb_get_can_db_properties_by_index(db)
         Frame = {}
         for Frame_id in range(db.FFrameCount):
```

### Comparing `TSMasterAPI-2.1.1/TSMasterAPI/TSCommon.py` & `TSMasterAPI-2.1.2/TSMasterAPI/TSCommon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 11:59:15
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-06-11 13:37:22
+LastEditTime: 2023-07-07 12:22:46
 '''
 from .TSDirver import *
 from .TSStructure import *  
 from .TSEnumdefine import *  
 from .TSFibex_parse import * 
 
 # Common Functions
@@ -18,15 +18,15 @@
 tsapp_get_error_description = dll.tsapp_get_error_description
 tsapp_get_error_description.argtypes = [s32,charpp]
 tsapp_get_error_description.restype  = TS_ReturnType 
 
 
 def check_status_operation(result, function, arguments):
     """Check the status and raise """
-    if result != 0:
+    if result == 97:
         ret = c_char_p()
         tsapp_get_error_description(result, ret)
         print("TSDriverOperationError: " + str(function.__name__) + "(" + str(arguments) + ") returned " + str(result) + ": " + str(ret.value))
     return result
 
 # 初始化函数 API函数使用之前 必须调用该函数 否则无法正常使用 在工程起始时 调用
 initialize_lib_tsmaster = dll.initialize_lib_tsmaster
@@ -882,14 +882,27 @@
 
 # 卸载所有数据库
 tsdb_unload_flexray_dbs = dll.tsdb_unload_flexray_dbs
 tsdb_unload_flexray_dbs.argtypes = []  
 tsdb_unload_flexray_dbs.restype = TS_ReturnType
 tsdb_unload_flexray_dbs.errcheck = check_status_operation
 
+# get flexray cluster parameters by cluster name
+tsdb_get_flexray_cluster_parameters = dll.db_get_flexray_cluster_parameters
+tsdb_get_flexray_cluster_parameters.argtypes = [c_char_p,PFlexRayClusterParameters]  
+tsdb_get_flexray_cluster_parameters.restype = TS_ReturnType
+tsdb_get_flexray_cluster_parameters.errcheck = check_status_operation
+
+# get flexray controller parameters by cluster name and controller name
+tsdb_get_flexray_controller_parameters = dll.db_get_flexray_controller_parameters
+tsdb_get_flexray_controller_parameters.argtypes = [c_char_p,PFlexRayControllerParameters]  
+tsdb_get_flexray_controller_parameters.restype = TS_ReturnType
+tsdb_get_flexray_controller_parameters.errcheck = check_status_operation
+
+
 # 获取加载的数据库数量
 tsdb_get_flexray_db_count = dll.tsdb_get_flexray_db_count
 tsdb_get_flexray_db_count.argtypes = [ps32]  
 tsdb_get_flexray_db_count.restype = TS_ReturnType
 tsdb_get_flexray_db_count.errcheck = check_status_operation
 
 # 通过索引获取数据库id
@@ -960,14 +973,25 @@
 
 # 通过Frame索引获取指定数据库的Signal信息
 tsdb_get_flexray_db_signal_properties_by_frame_index = dll.tsdb_get_flexray_db_signal_properties_by_frame_index
 tsdb_get_flexray_db_signal_properties_by_frame_index.argtypes = [s32,s32,s32,PDBSignalProperties]  
 tsdb_get_flexray_db_signal_properties_by_frame_index.restype = TS_ReturnType
 tsdb_get_flexray_db_signal_properties_by_frame_index.errcheck = check_status_operation
 
+
+tscom_flexray_get_signal_definition = dll.tscom_flexray_get_signal_definition
+tscom_flexray_get_signal_definition.argtypes = [c_char_p,PFlexRaySignal]  
+tscom_flexray_get_signal_definition.restype = TS_ReturnType
+tscom_flexray_get_signal_definition.errcheck = check_status_operation
+
+flexray_rbs_update_frame_by_header = dll.flexray_rbs_update_frame_by_header
+flexray_rbs_update_frame_by_header.argtypes = [PFlexray]  
+flexray_rbs_update_frame_by_header.restype = TS_ReturnType
+
+
 # 获取报文中信号值
 tscom_get_flexray_signal_value = dll.tscom_get_flexray_signal_value #函数对象
 tscom_get_flexray_signal_value.argtypes = [PFlexRaySignal,pu8] #指定参数类型
 tscom_get_flexray_signal_value.restype = c_double 
 
 # 设置报文中的信号值
 tscom_set_flexray_signal_value = dll.tscom_set_flexray_signal_value #函数对象
```

### Comparing `TSMasterAPI-2.1.1/TSMasterAPI/TSDirver.py` & `TSMasterAPI-2.1.2/TSMasterAPI/TSDirver.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.1/TSMasterAPI/TSEnumdefine.py` & `TSMasterAPI-2.1.2/TSMasterAPI/TSEnumdefine.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.1/TSMasterAPI/TSFibex_parse.py` & `TSMasterAPI-2.1.2/TSMasterAPI/TSFibex_parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-
 import xml.etree.ElementTree as ET
-
 class Fibex_parse():
-    Cluster = {}
-    Frames = {}
-    Pdus = {}
-    Triggers = {}
-    Signals = {}
-    Codings = {}
-    Ecus = {}
-    STATIC_SLOT = 30
     def __init__(self,xmlpath) -> ET:
+        self.Cluster = {}
+        self.Frames = {}
+        self.Pdus = {}
+        self.Triggers = {}
+        self.Signals = {}
+        self.Codings = {}
+        self.Ecus = {}
+        self.STATIC_SLOT = 30
         self.tree = ET.parse(xmlpath)
         self.parse(self.tree)
     def parse(self,tree):
         root = tree.getroot()
         CODINGS = root.findall('{http://www.asam.net/xml/fbx}PROCESSING-INFORMATION/{http://www.asam.net/xml/fbx}CODINGS/{http://www.asam.net/xml/fbx}CODING')
         if CODINGS!=None:
             for CODING in CODINGS:
@@ -31,14 +29,15 @@
                     self.Codings[CODING_ID]['offset'] = '0.0'
                     self.Codings[CODING_ID]['factor'] = '1.0'
         ELEMENTS = root.find('{http://www.asam.net/xml/fbx}ELEMENTS')
         if ELEMENTS!= None:
             CLUSTER = ELEMENTS.find('{http://www.asam.net/xml/fbx}CLUSTERS/{http://www.asam.net/xml/fbx}CLUSTER')
             if CLUSTER != None:
                 self.STATIC_SLOT = int(CLUSTER.find('{http://www.asam.net/xml/fbx/flexray}STATIC-SLOT').text)
+                self.Cluster['Name'] = CLUSTER.find('{http://www.asam.net/xml}SHORT-NAME').text
                 self.Cluster['NETWORK_MANAGEMENT_VECTOR_LENGTH'] = int(CLUSTER.find('{http://www.asam.net/xml/fbx/flexray}NETWORK-MANAGEMENT-VECTOR-LENGTH').text)
                 self.Cluster['PAYLOAD_LENGTH_STATIC'] = int(CLUSTER.find('{http://www.asam.net/xml/fbx/flexray}PAYLOAD-LENGTH-STATIC').text)
                 self.Cluster['T_S_S_TRANSMITTER'] = int(CLUSTER.find('{http://www.asam.net/xml/fbx/flexray}T-S-S-TRANSMITTER').text)
                 self.Cluster['CAS_RX_LOW_MAX'] = int(CLUSTER.find('{http://www.asam.net/xml/fbx/flexray}CAS-RX-LOW-MAX').text)
                 self.Cluster['SPEED'] = 0 if CLUSTER.find('{http://www.asam.net/xml/fbx}SPEED').text=='10000000' else 1
                 WAKE_UP = CLUSTER.find('{http://www.asam.net/xml/fbx/flexray}WAKE-UP')
                 self.Cluster['WAKE_UP_SYMBOL_RX_WINDOW'] = int(WAKE_UP.find('{http://www.asam.net/xml/fbx/flexray}WAKE-UP-SYMBOL-RX-WINDOW').text)
@@ -117,15 +116,26 @@
                         self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['SHORT-NAME'] = self.Signals[SIGNAL_REF]['SHORT-NAME']
                         self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['BIT-POSITION'] = int(SIGNAL_INSTANCE.find('{http://www.asam.net/xml/fbx}BIT-POSITION').text)
                         self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['BIT-LENGTH'] = self.Signals[SIGNAL_REF]['BIT-LENGTH']
                         self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['offset'] = self.Signals[SIGNAL_REF]['offset']
                         self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['factor'] = self.Signals[SIGNAL_REF]['factor']
                         self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['ENCODING'] = self.Signals[SIGNAL_REF]['ENCODING']
                         self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['is_M'] = SIGNAL_INSTANCE.find('{http://www.asam.net/xml/fbx}IS-HIGH-LOW-BYTE-ORDER').text
-                        self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['ub'] = SIGNAL_INSTANCE.find('{http://www.asam.net/xml/fbx}SIGNAL-UPDATE-BIT-POSITION').text if SIGNAL_INSTANCE.find('{http://www.asam.net/xml/fbx}SIGNAL-UPDATE-BIT-POSITION') != None else '-1'
+                        self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['ub'] = int(SIGNAL_INSTANCE.find('{http://www.asam.net/xml/fbx}SIGNAL-UPDATE-BIT-POSITION').text) if SIGNAL_INSTANCE.find('{http://www.asam.net/xml/fbx}SIGNAL-UPDATE-BIT-POSITION') != None else -1
+                        if self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['ub'] != -1:
+                            ub_name = _Signal_Name+"_ub"
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name] = {}
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name]['SHORT-NAME'] = ub_name
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name]['BIT-POSITION'] = self.Pdus[pdu_id]['SIGNALS'][_Signal_Name]['ub']
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name]['BIT-LENGTH'] = 1
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name]['offset'] = 0
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name]['factor'] = 1
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name]['ENCODING'] = self.Signals[SIGNAL_REF]['ENCODING']
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name]['is_M'] = True
+                            self.Pdus[pdu_id]['SIGNALS'][ub_name]['ub'] = '-1'
                         del _Signal_Name,SIGNAL_REF
                 del pdu_id
             FRAMES = ELEMENTS.findall('{http://www.asam.net/xml/fbx}FRAMES/{http://www.asam.net/xml/fbx}FRAME')
             if FRAMES != None:
                 for FRAME in FRAMES:
                     # _Frame ={}
                     FRAME_NAME = FRAME.find('{http://www.asam.net/xml}SHORT-NAME').text
@@ -135,15 +145,17 @@
                     # self.Frames[FRAME_NAME]['FRAME-ID'] = FRAME.attrib.get('ID',None)
                     self.Frames[FRAME_NAME]['SLOT-ID']= self.Triggers[FRAME_ID]['SLOT-ID']
                     self.Frames[FRAME_NAME]['BASE-CYCLE']= self.Triggers[FRAME_ID]['BASE-CYCLE']
                     self.Frames[FRAME_NAME]['CYCLE-REPETITION']= self.Triggers[FRAME_ID]['CYCLE-REPETITION']
                     _FDLC = int(FRAME.find('{http://www.asam.net/xml/fbx}BYTE-LENGTH').text)
                     self.Frames[FRAME_NAME]['FDLC'] = _FDLC
                     self.Triggers[FRAME_ID]['FDLC'] = _FDLC
+                    self.Triggers[FRAME_ID]['Name'] = FRAME_NAME
                     self.Triggers[self.Triggers[FRAME_ID]['TRIGGERING_ID']]['FDLC'] = _FDLC
+                    self.Triggers[self.Triggers[FRAME_ID]['TRIGGERING_ID']]['Name'] = FRAME_NAME
                     PDU_INSTANCES = FRAME.findall('{http://www.asam.net/xml/fbx}PDU-INSTANCES/{http://www.asam.net/xml/fbx}PDU-INSTANCE')
                     if len(PDU_INSTANCES) != 0:
                         self.Frames[FRAME_NAME]['PDUS'] = []
                         for PDU_INSTANCE in PDU_INSTANCES:
                             PDU_REF = PDU_INSTANCE.find('{http://www.asam.net/xml/fbx}PDU-REF').attrib.get('ID-REF',None)
                             PDU_1 = {}
                             PDU_1['PDU_Name'] = self.Pdus[PDU_REF]['PDU_Name']
@@ -151,15 +163,18 @@
                             PDU_1['SIGNALS'] = self.Pdus[PDU_REF]['SIGNALS']
                             self.Frames[FRAME_NAME]['PDUS'].append(PDU_1)  # store all PDUs in a list for easier
                             # self.Frames[FRAME_NAME][self.Pdus[PDU_REF]['PDU_Name']]={}
                             # self.Frames[FRAME_NAME][self.Pdus[PDU_REF]['PDU_Name']]['BIT-POSITION']=int(PDU_INSTANCE.find('{http://www.asam.net/xml/fbx}BIT-POSITION').text)
                             # self.Frames[FRAME_NAME][self.Pdus[PDU_REF]['PDU_Name']]['SIGNALS'] = self.Pdus[PDU_REF]['SIGNALS']
                             del PDU_REF,PDU_1
                     else:
-                        self.Frames[FRAME_NAME]['SIGNALS'] = self.Pdus[FRAME_ID]['SIGNALS']
+                        try:
+                            self.Frames[FRAME_NAME]['SIGNALS'] = self.Pdus[FRAME_ID]['SIGNALS']
+                        except:
+                            pass
                     del FRAME_NAME,FRAME_ID,_FDLC
             ECUS = ELEMENTS.findall('{http://www.asam.net/xml/fbx}ECUS/{http://www.asam.net/xml/fbx}ECU')
             if ECUS != None:  
                 for ECU in ECUS: 
                     ecu_name = ECU.find('{http://www.asam.net/xml}SHORT-NAME').text
                     self.Ecus[ecu_name] = {}
                     INPUT_PORTS = ECU.findall('{http://www.asam.net/xml/fbx}CONNECTORS/{http://www.asam.net/xml/fbx}CONNECTOR/{http://www.asam.net/xml/fbx}INPUTS/{http://www.asam.net/xml/fbx}INPUT-PORT')
@@ -224,24 +239,25 @@
                     for INPUT_PORT in INPUT_PORTS:
                         _rx_frame = {}
                         Trgger_ID = INPUT_PORT.find('{http://www.asam.net/xml/fbx}FRAME-TRIGGERING-REF').attrib.get('ID-REF',None)
                         _rx_frame['SLOT-ID'] = self.Triggers[Trgger_ID]['SLOT-ID']
                         _rx_frame['BASE-CYCLE'] = self.Triggers[Trgger_ID]['BASE-CYCLE']
                         _rx_frame['CYCLE-REPETITION'] = self.Triggers[Trgger_ID]['CYCLE-REPETITION']
                         _rx_frame['FDLC'] = self.Triggers[Trgger_ID]['FDLC']
+                        _rx_frame['Name'] = self.Triggers[Trgger_ID]['Name']
                         self.Ecus[ecu_name]['RX_Frame'].append(_rx_frame)
                         del Trgger_ID,_rx_frame
                     for OUTPUT_PORT in OUTPUT_PORTS:
                         _tx_frame = {}
                         Trgger_ID = OUTPUT_PORT.find('{http://www.asam.net/xml/fbx}FRAME-TRIGGERING-REF').attrib.get('ID-REF',None)
                         _tx_frame['SLOT-ID'] = self.Triggers[Trgger_ID]['SLOT-ID']
                         _tx_frame['BASE-CYCLE'] = self.Triggers[Trgger_ID]['BASE-CYCLE']
                         _tx_frame['CYCLE-REPETITION'] = self.Triggers[Trgger_ID]['CYCLE-REPETITION']
                         _tx_frame['FDLC'] = self.Triggers[Trgger_ID]['FDLC']
+                        _tx_frame['Name'] = self.Triggers[Trgger_ID]['Name']
                         if self.Ecus[ecu_name]['startupFrame_ID'] == _tx_frame['SLOT-ID'] and len(self.Ecus[ecu_name]['TX_Frame'])!=0  :
                             self.Ecus[ecu_name]['TX_Frame'].append(self.Ecus[ecu_name]['TX_Frame'][0])
                             self.Ecus[ecu_name]['TX_Frame'][0] = _tx_frame
                         else:
                             self.Ecus[ecu_name]['TX_Frame'].append(_tx_frame)
                         del Trgger_ID,_tx_frame
-                    del ecu_name
- 
+                    del ecu_name
```

### Comparing `TSMasterAPI-2.1.1/TSMasterAPI/TSMasterAPI.py` & `TSMasterAPI-2.1.2/TSMasterAPI/TSMasterAPI.py`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.1/TSMasterAPI/TSStructure.py` & `TSMasterAPI-2.1.2/TSMasterAPI/TSStructure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-04-21 10:21:17
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-05-17 14:26:06
+LastEditTime: 2023-07-06 20:32:20
 '''
 from ctypes import Structure,c_char,c_int32,c_bool,c_uint8,c_int64,c_uint64,c_uint32,c_uint16,c_double,c_char_p,byref,string_at,string_at,CDLL,CFUNCTYPE,POINTER,pointer,c_void_p,c_float,c_int16,c_int8,WINFUNCTYPE
 
 
 u8 = c_uint8
 pu8 = POINTER(c_uint8)
 s8 = c_int8
@@ -554,14 +554,15 @@
     _fields_ = [("FDBIndex", c_int32),
                 ("FSignalCount", c_int32),
                 ("FFrameCount", c_int32),
                 ("FECUCount", c_int32),
                 ("FSupportedChannelMask", c_uint64),
                 ("FName", c_char * DATABASE_STR_LEN),
                 ("FComment", c_char * DATABASE_STR_LEN),
+                ("FFlags", u64),
                 ]
 PDBProperties = POINTER(TDBProperties)
 class TDBECUProperties(Structure):
     '''
     DataBase ECU properties 描述数据库中ECU节点 TX RX报文数量以及ECU节点名称与注释
     '''
     _pack_ = 1
@@ -631,14 +632,107 @@
                 ("FInitValue", c_double),
                 ("FName", c_char * DATABASE_STR_LEN),
                 ("FComment", c_char * DATABASE_STR_LEN),
                 ] 
 
 PDBSignalProperties = POINTER(TDBSignalProperties) 
 
+GENERIC_STRING_MAX_LENGTH = 32
+class TFlexRayClusterParameters(Structure):
+    '''
+    DataBase Signal properties 描述数据库中 signal详细信息
+    '''
+    _pack_ = 1
+    _fields_ = [("FShortName", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FLongName", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FDescription", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FSpeed", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FChannels", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FBitCountingPolicy", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FProtocol", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FProtocolVersion", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FMedium",  c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FIsHighLowBitOrder", s32),
+                ("FMaxFrameLengthByte", s32),
+                ("FNumberOfCycles", s32),
+                ("FCycle_us", s32),
+                ("FBit_us", double),
+                ("FSampleClockPeriod_us", double),
+                ("FMacrotick_us", double),
+
+                ("FMacroPerCycle", s32),
+                ("FNumberOfStaticSlots", s32),
+                ("FStaticSlot_MT", s32),
+                ("FActionPointOffset_MT", s32),
+                ("FPayloadLengthStatic_WORD", s32),
+                ("FNumberOfMiniSlots", s32),
+                ("FMiniSlot_MT", s32),
+                ("FMiniSlotActionPointOffset_MT", s32),
+                ("FDynamicSlotIdlePhase_MiniSlots", s32),
+                ("FSymbolWindow_MT", s32),
+                ("FNIT_MT", s32),
+                ("FSyncNodeMax", s32),
+                ("FNetworkManagementVectorLength", s32),
+                ("FListenNoise", s32),
+                ("FColdStartAttempts", s32),
+                ("FCASRxLowMax_gdBit", s32),
+                ("FWakeupSymbolRxIdle_gdBit", s32),
+                ("FWakeupSymbolRxLow_gdBit", s32),
+                ("FWakeupSymbolRxWindow_gdBit", s32),
+                ("FWakeupSymbolTxIdle_gdBit", s32),
+                ("FWakeupSymbolTxLow_gdBit", s32),
+                ("FMaxInitializationError_us", double),
+                ("FClusterDriftDamping_uT", s32),
+                ("FOffsetCorrectionStart_MT", s32),
+                ("FMaxWithoutClockCorrectionFatal", s32),
+                ("FMaxWithoutClockCorrectionPassive", s32),
+                ] 
+PFlexRayClusterParameters = POINTER(TFlexRayClusterParameters)
+
+
+class TFlexRayControllerParameters(Structure):
+    '''
+    DataBase Signal properties 描述数据库中 signal详细信息
+    '''
+    _pack_ = 1
+    _fields_ = [("FShortName", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FConnectedChannels", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FMicroPerCycle_uT", s32),
+                ("FMicroPerMacroNom_uT", s32),
+                ("FMicroTick_us", double),
+                ("FSamplesPerMicrotick", s32),
+                ("FWakeupChannelA", s32),
+                ("FWakeupChannelB", s32),
+                ("FMaxDrift_uT", s32),
+                ("FWakeupPattern", s32),
+                ("FListenTimeout_uT", s32),
+                ("FAcceptedStartupRange_uT", s32),
+                ("FMacroInitialOffsetA_MT", s32),
+                ("FMacroInitialOffsetB_MT", s32),
+                ("FMicroInitialOffsetA_uT", s32),
+                ("FMicroInitialOffsetB_uT", s32),
+                ("FKeySlotUsage", c_char * GENERIC_STRING_MAX_LENGTH),
+                ("FKeySlotID", s32),
+                ("FSingleSlotEnabled", s32),
+                ("FClusterDriftDamping_uT", s32),
+                ("FDocodingCorrection_uT", s32),
+                ("FDelayCompensationA_uT", s32),
+                ("FDelayCompensationB_uT", s32),
+                ("FOffsetCorrectionOut_uT", s32),
+                ("FExternRateCorrection_uT", s32),
+                ("FRateCorrectionOut_uT", s32),
+                ("FExternOffsetCorrection_uT", s32),
+                ("FAllowHaltDueToClock", s32),
+                ("FAllowPassivToActive", s32),
+                ("FLatestTx", s32),
+                ("FMaxDynamicPayloadLength", s32),
+                ] 
+
+PFlexRayControllerParameters = POINTER(TFlexRayControllerParameters) 
+
 #回调函数
 
 OnTx_RxFUNC_CANFD = WINFUNCTYPE(None, ps32, PCANFD)
 
 
 OnTx_RxFUNC_CAN = WINFUNCTYPE(None, ps32, PCAN)
```

### Comparing `TSMasterAPI-2.1.1/TSMasterAPI.egg-info/PKG-INFO` & `TSMasterAPI-2.1.2/TSMasterAPI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSMasterAPI
-Version: 2.1.1
+Version: 2.1.2
 Summary: Use TSMaster hardware
 Author: seven
 Author-email: 865762826@qq.com
 License: BSD License
 Platform: WINDOWS
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `TSMasterAPI-2.1.1/license.txt` & `TSMasterAPI-2.1.2/license.txt`

 * *Files identical despite different names*

### Comparing `TSMasterAPI-2.1.1/setup.py` & `TSMasterAPI-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: seven 865762826@qq.com
 Date: 2023-03-24 09:26:29
 LastEditors: seven 865762826@qq.com
-LastEditTime: 2023-06-11 13:41:40
+LastEditTime: 2023-07-07 18:25:50
 FilePath: \VSCode_Pro\Python_Pro\TSMasterApi\setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from distutils.core import setup
 from setuptools import find_packages
 
 with open("README.rst", "r",encoding="utf-8") as f:
   long_description = f.read()
 
 # 
 setup(name='TSMasterAPI',  # 包名
-      version='2.1.1',  # 版本号
+      version='2.1.2',  # 版本号
       description='Use TSMaster hardware',
       long_description=long_description,
       author='seven',
       author_email='865762826@qq.com',
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
```

