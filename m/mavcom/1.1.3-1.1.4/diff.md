# Comparing `tmp/mavcom-1.1.3.tar.gz` & `tmp/mavcom-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavcom-1.1.3.tar", last modified: Fri Jul  7 10:48:31 2023, max compression
+gzip compressed data, was "mavcom-1.1.4.tar", last modified: Fri Jul  7 14:26:11 2023, max compression
```

## Comparing `mavcom-1.1.3.tar` & `mavcom-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.269582 mavcom-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 10:48:19.000000 mavcom-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 10:48:31.269582 mavcom-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 10:48:19.000000 mavcom-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 10:48:19.000000 mavcom-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 10:48:31.269582 mavcom-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.265582 mavcom-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.269582 mavcom-1.1.3/src/mavcom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/loracon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/mavconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/mavcontrol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-07 10:48:19.000000 mavcom-1.1.3/src/mavcom/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.269582 mavcom-1.1.3/src/mavcom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 10:48:31.000000 mavcom-1.1.3/src/mavcom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 10:48:31.269582 mavcom-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 10:48:19.000000 mavcom-1.1.3/tests/test_mavcom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.488798 mavcom-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-07 14:25:56.000000 mavcom-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 14:26:11.488798 mavcom-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-07 14:25:56.000000 mavcom-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 14:25:56.000000 mavcom-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 14:26:11.488798 mavcom-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.480798 mavcom-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.484798 mavcom-1.1.4/src/mavcom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/loracon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/mavconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/mavcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-07 14:25:56.000000 mavcom-1.1.4/src/mavcom/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.484798 mavcom-1.1.4/src/mavcom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-07 14:26:11.000000 mavcom-1.1.4/src/mavcom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 14:26:11.488798 mavcom-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 14:25:56.000000 mavcom-1.1.4/tests/test_mavcom.py
```

### Comparing `mavcom-1.1.3/LICENSE` & `mavcom-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.3/PKG-INFO` & `mavcom-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.1.3
+Version: 1.1.4
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mavcom-1.1.3/README.md` & `mavcom-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.3/pyproject.toml` & `mavcom-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mavcom"
-version = "1.1.3"
+version = "1.1.4"
 description = "A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers"
 readme = "README.md"
 authors = [{ name = "Mavscient", email = "mavscient@xee4c.33mail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `mavcom-1.1.3/src/mavcom/loracon.py` & `mavcom-1.1.4/src/mavcom/loracon.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.3/src/mavcom/mavconstants.py` & `mavcom-1.1.4/src/mavcom/mavconstants.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.3/src/mavcom/mavcontrol.py` & `mavcom-1.1.4/src/mavcom/mavcontrol.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 
         mandatory_message_types = [
             "HEARTBEAT",
             "GLOBAL_POSITION_INT",
             "GPS_STATUS",
             "GPS_RAW_INT",
             "EKF_STATUS_REPORT",
-            "VFR_HUD"
+            "VFR_HUD",
+            "HOME_POSITION"
         ]
         self.required_message_types = required_message_types + [m for m in mandatory_message_types if m not in required_message_types]
         self.current_values = defaultdict(lambda: None)
         self.controller = controller
         has_controller = True if controller else False
         
         self._flight_mode = None
```

### Comparing `mavcom-1.1.3/src/mavcom/video.py` & `mavcom-1.1.4/src/mavcom/video.py`

 * *Files identical despite different names*

### Comparing `mavcom-1.1.3/src/mavcom.egg-info/PKG-INFO` & `mavcom-1.1.4/src/mavcom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavcom
-Version: 1.1.3
+Version: 1.1.4
 Summary: A python package that creates a simplified programming interface for controlling Mavlink-capable flight controllers
 Author-email: Mavscient <mavscient@xee4c.33mail.com>
 License: MIT License
         
         Copyright (c) 2023 Mavscient
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mavcom-1.1.3/tests/test_mavcom.py` & `mavcom-1.1.4/tests/test_mavcom.py`

 * *Files identical despite different names*

