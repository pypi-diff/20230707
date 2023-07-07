# Comparing `tmp/vocalhost-1.0.8.tar.gz` & `tmp/vocalhost-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalhost-1.0.8.tar", last modified: Fri Jul  7 17:33:20 2023, max compression
+gzip compressed data, was "vocalhost-1.0.9.tar", last modified: Fri Jul  7 19:44:25 2023, max compression
```

## Comparing `vocalhost-1.0.8.tar` & `vocalhost-1.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:33:20.272684 vocalhost-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 17:33:20.272684 vocalhost-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-07 17:33:08.000000 vocalhost-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:33:20.272684 vocalhost-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-07 17:33:08.000000 vocalhost-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:33:20.272684 vocalhost-1.0.8/vocalhost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 17:33:20.000000 vocalhost-1.0.8/vocalhost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-07 17:33:08.000000 vocalhost-1.0.8/vocalhost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:44:25.862002 vocalhost-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-07 19:44:25.862002 vocalhost-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-07 19:44:14.000000 vocalhost-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 19:44:25.862002 vocalhost-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-07 19:44:14.000000 vocalhost-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 19:44:25.862002 vocalhost-1.0.9/vocalhost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-07 19:44:25.000000 vocalhost-1.0.9/vocalhost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-07 19:44:14.000000 vocalhost-1.0.9/vocalhost.py
```

### Comparing `vocalhost-1.0.8/PKG-INFO` & `vocalhost-1.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.0.8
+Version: 1.0.9
+Summary: Localhost to Vocalhost, run functions from anywhere
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.0.8/README.md` & `vocalhost-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vocalhost-1.0.8/vocalhost.egg-info/PKG-INFO` & `vocalhost-1.0.9/vocalhost.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: vocalhost
-Version: 1.0.8
+Version: 1.0.9
+Summary: Localhost to Vocalhost, run functions from anywhere
 Description-Content-Type: text/markdown
 
 # Vocalhost-python
 Vocalhost is a communication solution that enables direct and reliable connections between systems using WebSocket protocol. It comprises a bridge server and a client agent, offering support for a wide range of languages, frameworks, and systems. This versatility allows for seamless interaction and efficient data exchange across diverse environments.
 
 The bridge server acts as a central hub, relaying real-time messages between connected systems over WebSocket connections. The client agent establishes a WebSocket connection with the bridge server, facilitating communication across various platforms.
```

### Comparing `vocalhost-1.0.8/vocalhost.py` & `vocalhost-1.0.9/vocalhost.py`

 * *Files identical despite different names*

