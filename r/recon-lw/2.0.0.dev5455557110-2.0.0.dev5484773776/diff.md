# Comparing `tmp/recon_lw-2.0.0.dev5455557110.tar.gz` & `tmp/recon_lw-2.0.0.dev5484773776.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5455557110.tar", last modified: Tue Jul  4 13:59:03 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5484773776.tar", last modified: Fri Jul  7 09:13:35 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5455557110.tar` & `recon_lw-2.0.0.dev5484773776.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-04 13:58:32.000000 recon_lw-2.0.0.dev5455557110/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13589 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    34732 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)     3998 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/recon_lw/recon_oe_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 13:59:03.000000 recon_lw-2.0.0.dev5455557110/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-04 13:58:07.000000 recon_lw-2.0.0.dev5455557110/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-07 09:13:09.000000 recon_lw-2.0.0.dev5484773776/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13805 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35110 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23879 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6278 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/recon_lw/recon_oe_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 09:13:35.000000 recon_lw-2.0.0.dev5484773776/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-07 09:12:43.000000 recon_lw-2.0.0.dev5484773776/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/LastStateMatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,16 @@
                 i = records_times.bisect_key_right(recon_lw.time_stamp_key(ts1))
                 if i == 0:
                     o2 = self._state_cache[key1]["prior_o"]
                 else:
                     ts2 = records_times[i-1]
                     sti = self._state_time_index.bisect_key_left(recon_lw.time_stamp_key(ts2) + "_" + key1)
                     o2 = self._state_time_index[sti][3]
-            self._interpret_func([o1,o2], self._custom_settings, self._create_event, self._send_events)
+            tech = {"key1" :key1, "ts1": ts1,"state_cache": self._state_cache.get(key1)}
+            self._interpret_func([o1, o2, tech], self._custom_settings, self._create_event, self._send_events)
 
         if horizon_time is not None:
             edge_timestamp = {"epochSecond": horizon_time["epochSecond"] - self._horizon_delay_seconds,
                               "nano": 0}
             state_edge = self._state_time_index.bisect_key_left(recon_lw.time_stamp_key(edge_timestamp)+"_")
         else:
             state_edge = len(self._state_time_index)
```

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/recon_lw.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 from th2_data_services.data import Data
 from th2_data_services.utils.message_utils import message_utils
 from os import listdir
 from os import path
 from recon_lw.EventsSaver import EventsSaver
 
 
+def epoch_nano_str_to_ts(s_nanos):
+    nanos = int(s_nanos)
+    return {"epochSecond": nanos // 1e9, "nano": nanos % 1e9}
+
+
+def ts_to_epoch_nano_str(ts):
+    return f'{ts["epochSecond"]}{str(ts["nano"]).zfill(9)}'
+
+
 def time_stamp_key(ts):
     nanos_str = str(ts["nano"]).zfill(9)
     return str(ts["epochSecond"]) + "." + nanos_str
 
 
 def time_index_add(key, m, time_index):
     time_index.add((m["timestamp"], key))
```

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,26 @@
                                             "len(obs)": len(obs),
                                             "book_id": book_id},
                                       parentId=parent_event["eventId"])
     for tupl in operations_batch:
         dbg_event["attachedMessageIds"].append(tupl[2]["messageId"])
     events.append(dbg_event)
 
+    # update otv (order time version)
+    orders_versions = {}
+    for ob in obs:
+        if "order_id" in ob["operation_params"]:
+            ver = 0
+            order_id = ob["operation_params"]["order_id"] 
+            if order_id in orders_versions:
+                ver = orders_versions[order_id]+1
+            ob["otv"] = ver
+            orders_versions[order_id] = ver
+
+
     if len(obs) > 1 and aggregate_batch_updates:
         top_not_affected = True #all(ob["aggr_seq"]["top_delta"] == 0 for ob in obs)
         limit_not_affected = True #all(ob["aggr_seq"]["limit_delta"] == 0 for ob in obs)
         updated_v2 = 0
         for i in range(len(obs) - 1):
             if obs[i]["operation"] in ["ob_change_status", "ob_clean_book", "ob_aggr_clean_book", "ob_top_clean_book"]:
                 obs[i]["aggr_seq"]["top_v2"] = updated_v2
```

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5484773776/recon_lw/recon_ob_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,34 @@
 from datetime import datetime
 from itertools import islice
 
 from recon_lw import recon_lw
 from recon_lw.EventsSaver import EventsSaver
 from recon_lw.LastStateMatcher import LastStateMatcher
 from th2_data_services.utils.message_utils import message_utils
-
-def epoch_nano_str_to_ts(s_nanos):
-    nanos = int(s_nanos)
-    return {"epochSecond": nanos // 1e9, "nano": nanos % 1e9}
+import copy
 
 
 def ob_compare_stats_get_state_ts_key_order(o, settings):
     if "eventId" not in o:
         return None, None, None
 
     if o["body"]["sessionId"] != settings["top_session"]:
         return None, None, None
 
-    return epoch_nano_str_to_ts(o["body"]["time_of_event"]), o["body"]["book_id"], o["body"]["v"]
+    return recon_lw.epoch_nano_str_to_ts(o["body"]["time_of_event"]), o["body"]["book_id"], o["body"]["v"]
 
 
 def ob_compare_stats_interpret(match, custom_settings, create_event, save_events):
     if match[1] is None:
         error_event = create_event("StatsNotFound" + match[0]["messageType"],
                                    "StatsNotFound",
                                    False,
-                                   {"stats_message": match[0]})
+                                   {"stats_message": match[0],
+                                    "tech": copy.deepcopy(match[2])})
         error_event["attachedMessageIds"] = [match[0]["messageId"]]
         save_events([error_event])
         return
 
     stats = custom_settings["get_expected_stats_func"](match[0])
     fails = {}
     for k, v in stats.items():
@@ -121,15 +119,15 @@
     if m["sessionId"] not in settings["stat_sessions"]:
         return None, None
 
     if m["sessionType"] not in ["TradeStatisticsIntraday", "TradeStatisticsEOD"]:
         return None, None
 
     mm = message_utils.message_to_dict(m)
-    return epoch_nano_str_to_ts(mm["TimeOfEvent"]),  mm["TradableInstrumentID"]
+    return recon_lw.recon_lw.epoch_nano_str_to_ts(mm["TimeOfEvent"]),  mm["TradableInstrumentID"]
     # epoch_nano_str_to_ts is in recon_ob_stats module
 
 
 def get_stats_example(m):
     mm = message_utils.message_to_dict(m)
     stats = {
         "open_price": mm["OpenPrice"],
```

### Comparing `recon_lw-2.0.0.dev5455557110/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5484773776/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5455557110/setup.py` & `recon_lw-2.0.0.dev5484773776/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5455557110/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5484773776/test/test_recon_ob.py`

 * *Files identical despite different names*

