# Comparing `tmp/w3bstream_client_python-0.4.4.tar.gz` & `tmp/w3bstream_client_python-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream_client_python-0.4.4.tar", last modified: Fri Jul  7 18:19:58 2023, max compression
+gzip compressed data, was "w3bstream_client_python-0.4.5.tar", last modified: Fri Jul  7 19:37:00 2023, max compression
```

## Comparing `w3bstream_client_python-0.4.4.tar` & `w3bstream_client_python-0.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 18:19:58.492362 w3bstream_client_python-0.4.4/
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.4/.gitignore
--rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.4/LICENSE
--rw-r--r--   0 haaai     (1000) haaai     (1000)      810 2023-07-07 18:19:58.492362 w3bstream_client_python-0.4.4/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      634 2023-07-07 16:58:52.000000 w3bstream_client_python-0.4.4/README.md
--rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-07 18:19:43.000000 w3bstream_client_python-0.4.4/pyproject.toml
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-07 18:19:58.492362 w3bstream_client_python-0.4.4/setup.cfg
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 18:19:58.482362 w3bstream_client_python-0.4.4/src/
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 18:19:58.482362 w3bstream_client_python-0.4.4/src/w3bstream_client_python/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-07 17:50:45.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3852 2023-07-07 16:58:52.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 18:19:58.492362 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      810 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/requires.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-07 18:19:58.000000 w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.5/.gitignore
+-rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.5/LICENSE
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      799 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      623 2023-07-07 19:34:25.000000 w3bstream_client_python-0.4.5/README.md
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-07 19:33:48.000000 w3bstream_client_python-0.4.5/pyproject.toml
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/setup.cfg
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/src/
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/src/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-07 17:50:45.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3840 2023-07-07 19:34:41.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      799 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/requires.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/top_level.txt
```

### Comparing `w3bstream_client_python-0.4.4/.gitignore` & `w3bstream_client_python-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.4/LICENSE` & `w3bstream_client_python-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.4/PKG-INFO` & `w3bstream_client_python-0.4.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3bstream_client_python
-Version: 0.4.4
+Version: 0.4.5
 Summary: Official W3bstream Client for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
@@ -21,14 +21,14 @@
 
 ### Publish Event Synchronously
 
 ``` py
 from w3bstream_client_python import Client, Header
 
 # the http_route, project and api_key are obtained on W3bstream-Studio
-client = Client("http_route", "project", "api_key")
+client = Client("http_route", "api_key")
 # device_id is the identity for the device
 # payload can be an empty string if served as a heartbeat
 header = Header('device_id')
 rsp = client.publish_event_sync(header, b'payload')
 print(rsp.text)
 ```
```

### Comparing `w3bstream_client_python-0.4.4/README.md` & `w3bstream_client_python-0.4.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 
 ### Publish Event Synchronously
 
 ``` py
 from w3bstream_client_python import Client, Header
 
 # the http_route, project and api_key are obtained on W3bstream-Studio
-client = Client("http_route", "project", "api_key")
+client = Client("http_route", "api_key")
 # device_id is the identity for the device
 # payload can be an empty string if served as a heartbeat
 header = Header('device_id')
 rsp = client.publish_event_sync(header, b'payload')
 print(rsp.text)
 ```
```

### Comparing `w3bstream_client_python-0.4.4/src/w3bstream_client_python/client.py` & `w3bstream_client_python-0.4.5/src/w3bstream_client_python/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 PUBLISH_INTERVAL = 5
 PUBLISH_BATCH_SIZE = 10
 
 
 @typechecked
 class Client:
-    def __init__(self, url: str, project: str, api_key: str, queue_size: int = 0):
+    def __init__(self, url: str, api_key: str, queue_size: int = 0):
         self.url = url
-        self.project = project
+        # self.project = project
         self.api_key = api_key
         self.queue = queue.Queue(queue_size)
         # self.thread = threading.Thread(target=self._worker)
         # self.thread.start()
 
     def publish_event_sync(self, header: Header, payload: bytes) -> requests.Response:
         """
```

### Comparing `w3bstream_client_python-0.4.4/src/w3bstream_client_python.egg-info/PKG-INFO` & `w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3bstream-client-python
-Version: 0.4.4
+Version: 0.4.5
 Summary: Official W3bstream Client for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
@@ -21,14 +21,14 @@
 
 ### Publish Event Synchronously
 
 ``` py
 from w3bstream_client_python import Client, Header
 
 # the http_route, project and api_key are obtained on W3bstream-Studio
-client = Client("http_route", "project", "api_key")
+client = Client("http_route", "api_key")
 # device_id is the identity for the device
 # payload can be an empty string if served as a heartbeat
 header = Header('device_id')
 rsp = client.publish_event_sync(header, b'payload')
 print(rsp.text)
 ```
```

