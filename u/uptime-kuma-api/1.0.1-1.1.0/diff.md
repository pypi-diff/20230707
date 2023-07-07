# Comparing `tmp/uptime_kuma_api-1.0.1.tar.gz` & `tmp/uptime_kuma_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptime_kuma_api-1.0.1.tar", last modified: Thu May 25 21:54:28 2023, max compression
+gzip compressed data, was "dist/uptime_kuma_api-1.1.0.tar", last modified: Fri Jul  7 20:34:14 2023, max compression
```

## Comparing `uptime_kuma_api-1.0.1.tar` & `uptime_kuma_api-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/
--rw-r--r--   0 lucas     (1000) users      (985)     1067 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/LICENSE
--rw-r--r--   0 lucas     (1000) users      (985)     3186 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/PKG-INFO
--rw-r--r--   0 lucas     (1000) users      (985)     2057 2023-05-20 17:41:15.000000 uptime_kuma_api-1.0.1/README.md
--rw-r--r--   0 lucas     (1000) users      (985)       38 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/setup.cfg
--rw-r--r--   0 lucas     (1000) users      (985)     1818 2023-05-25 17:51:04.000000 uptime_kuma_api-1.0.1/setup.py
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/uptime_kuma_api/
--rw-r--r--   0 lucas     (1000) users      (985)      592 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/__init__.py
--rw-r--r--   0 lucas     (1000) users      (985)      142 2023-05-25 21:52:00.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/__version__.py
--rw-r--r--   0 lucas     (1000) users      (985)   149456 2023-05-25 21:49:09.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/api.py
--rw-r--r--   0 lucas     (1000) users      (985)      326 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/auth_method.py
--rw-r--r--   0 lucas     (1000) users      (985)      169 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/docker_type.py
--rw-r--r--   0 lucas     (1000) users      (985)    29259 2023-05-20 13:03:51.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/docstrings.py
--rw-r--r--   0 lucas     (1000) users      (985)      650 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/event.py
--rw-r--r--   0 lucas     (1000) users      (985)      252 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/exceptions.py
--rw-r--r--   0 lucas     (1000) users      (985)      324 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/incident_style.py
--rw-r--r--   0 lucas     (1000) users      (985)      515 2023-05-01 18:17:19.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/maintenance_strategy.py
--rw-r--r--   0 lucas     (1000) users      (985)      226 2023-05-19 12:02:01.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/monitor_status.py
--rw-r--r--   0 lucas     (1000) users      (985)      828 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/monitor_type.py
--rw-r--r--   0 lucas     (1000) users      (985)    14475 2023-05-20 12:16:15.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/notification_providers.py
--rw-r--r--   0 lucas     (1000) users      (985)      336 2023-04-07 19:52:49.000000 uptime_kuma_api-1.0.1/uptime_kuma_api/proxy_protocol.py
-drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-05-25 21:54:28.427329 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/
--rw-r--r--   0 lucas     (1000) users      (985)     3186 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) users      (985)      665 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) users      (985)        1 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) users      (985)       41 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) users      (985)       16 2023-05-25 21:54:28.000000 uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/
+-rw-r--r--   0 lucas     (1000) users      (985)     1067 2023-04-07 19:52:49.000000 uptime_kuma_api-1.1.0/LICENSE
+-rw-r--r--   0 lucas     (1000) users      (985)     3735 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/PKG-INFO
+-rw-r--r--   0 lucas     (1000) users      (985)     2057 2023-07-07 20:27:36.000000 uptime_kuma_api-1.1.0/README.md
+-rw-r--r--   0 lucas     (1000) users      (985)       38 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/setup.cfg
+-rw-r--r--   0 lucas     (1000) users      (985)     1818 2023-05-25 17:51:04.000000 uptime_kuma_api-1.1.0/setup.py
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/
+-rw-r--r--   0 lucas     (1000) users      (985)      592 2023-05-19 12:02:01.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/__init__.py
+-rw-r--r--   0 lucas     (1000) users      (985)      142 2023-07-07 20:27:36.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/__version__.py
+-rw-r--r--   0 lucas     (1000) users      (985)   150811 2023-07-07 20:27:39.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/api.py
+-rw-r--r--   0 lucas     (1000) users      (985)      326 2023-04-07 19:52:49.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/auth_method.py
+-rw-r--r--   0 lucas     (1000) users      (985)      169 2023-04-07 19:52:49.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/docker_type.py
+-rw-r--r--   0 lucas     (1000) users      (985)    29713 2023-07-07 20:27:36.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/docstrings.py
+-rw-r--r--   0 lucas     (1000) users      (985)      650 2023-04-07 19:52:49.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/event.py
+-rw-r--r--   0 lucas     (1000) users      (985)      252 2023-05-19 12:02:01.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/exceptions.py
+-rw-r--r--   0 lucas     (1000) users      (985)      324 2023-04-07 19:52:49.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/incident_style.py
+-rw-r--r--   0 lucas     (1000) users      (985)      515 2023-05-01 18:17:19.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/maintenance_strategy.py
+-rw-r--r--   0 lucas     (1000) users      (985)      226 2023-05-19 12:02:01.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/monitor_status.py
+-rw-r--r--   0 lucas     (1000) users      (985)      865 2023-07-07 20:27:36.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/monitor_type.py
+-rw-r--r--   0 lucas     (1000) users      (985)    14698 2023-07-07 20:27:36.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/notification_providers.py
+-rw-r--r--   0 lucas     (1000) users      (985)      336 2023-04-07 19:52:49.000000 uptime_kuma_api-1.1.0/uptime_kuma_api/proxy_protocol.py
+drwxr-xr-x   0 lucas     (1000) users      (985)        0 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/uptime_kuma_api.egg-info/
+-rw-r--r--   0 lucas     (1000) users      (985)     3735 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/uptime_kuma_api.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1000) users      (985)      665 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/uptime_kuma_api.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1000) users      (985)        1 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/uptime_kuma_api.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1000) users      (985)       41 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/uptime_kuma_api.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1000) users      (985)       16 2023-07-07 20:34:14.000000 uptime_kuma_api-1.1.0/uptime_kuma_api.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `uptime_kuma_api-1.0.1/LICENSE` & `uptime_kuma_api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.1/PKG-INFO` & `uptime_kuma_api-1.1.0/uptime_kuma_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,86 @@
 Metadata-Version: 2.1
-Name: uptime_kuma_api
-Version: 1.0.1
+Name: uptime-kuma-api
+Version: 1.1.0
 Summary: A python wrapper for the Uptime Kuma WebSocket API
 Home-page: https://github.com/lucasheld/uptime-kuma-api
 Author: Lucas Held
 Author-email: lucasheld@hotmail.de
 License: MIT
+Description: # uptime-kuma-api
+        
+        A wrapper for the Uptime Kuma Socket.IO API
+        ---
+        uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
+        
+        This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
+        
+        Python version 3.7+ is required.
+        
+        Supported Uptime Kuma versions:
+        
+        | Uptime Kuma     | uptime-kuma-api |
+        |-----------------|-----------------|
+        | 1.21.3 - 1.22.1 | 1.0.0 - 1.1.0   |
+        | 1.17.0 - 1.21.2 | 0.1.0 - 0.13.0  |
+        
+        Installation
+        ---
+        uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
+        
+        You can install it using pip:
+        
+        ```
+        pip install uptime-kuma-api
+        ```
+        
+        Documentation
+        ---
+        The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
+        
+        Example
+        ---
+        Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
+        
+        To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
+        
+        ```python
+        >>> from uptime_kuma_api import UptimeKumaApi, MonitorType
+        >>> api = UptimeKumaApi('INSERT_URL')
+        >>> api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+        ```
+        
+        Now you can call one of the existing methods of the instance. For example create a new monitor:
+        
+        ```python
+        >>> result = api.add_monitor(type=MonitorType.HTTP, name="Google", url="https://google.com")
+        >>> print(result)
+        {'msg': 'Added Successfully.', 'monitorId': 1}
+        ```
+        
+        At the end, the connection to the API must be disconnected so that the program does not block.
+        
+        ```python
+        >>> api.disconnect()
+        ```
+        
+        With a context manager, the disconnect method is called automatically:
+        
+        ```python
+        from uptime_kuma_api import UptimeKumaApi
+        
+        with UptimeKumaApi('INSERT_URL') as api:
+            api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+            api.add_monitor(
+                type=MonitorType.HTTP,
+                name="Google",
+                url="https://google.com"
+            )
+        ```
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -21,81 +92,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# uptime-kuma-api
-
-A wrapper for the Uptime Kuma Socket.IO API
----
-uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
-
-This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
-
-Python version 3.7+ is required.
-
-Supported Uptime Kuma versions:
-
-| Uptime Kuma     | uptime-kuma-api |
-|-----------------|-----------------|
-| 1.21.3          | 1.0.0           |
-| 1.17.0 - 1.21.2 | 0.1.0 - 0.13.0  |
-
-Installation
----
-uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
-
-You can install it using pip:
-
-```
-pip install uptime-kuma-api
-```
-
-Documentation
----
-The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
-
-Example
----
-Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
-
-To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
-
-```python
->>> from uptime_kuma_api import UptimeKumaApi, MonitorType
->>> api = UptimeKumaApi('INSERT_URL')
->>> api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
-```
-
-Now you can call one of the existing methods of the instance. For example create a new monitor:
-
-```python
->>> result = api.add_monitor(type=MonitorType.HTTP, name="Google", url="https://google.com")
->>> print(result)
-{'msg': 'Added Successfully.', 'monitorId': 1}
-```
-
-At the end, the connection to the API must be disconnected so that the program does not block.
-
-```python
->>> api.disconnect()
-```
-
-With a context manager, the disconnect method is called automatically:
-
-```python
-from uptime_kuma_api import UptimeKumaApi
-
-with UptimeKumaApi('INSERT_URL') as api:
-    api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
-    api.add_monitor(
-        type=MonitorType.HTTP,
-        name="Google",
-        url="https://google.com"
-    )
-```
-
-
```

### Comparing `uptime_kuma_api-1.0.1/README.md` & `uptime_kuma_api-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Python version 3.7+ is required.
 
 Supported Uptime Kuma versions:
 
 | Uptime Kuma     | uptime-kuma-api |
 |-----------------|-----------------|
-| 1.21.3          | 1.0.0           |
+| 1.21.3 - 1.22.1 | 1.0.0 - 1.1.0   |
 | 1.17.0 - 1.21.2 | 0.1.0 - 0.13.0  |
 
 Installation
 ---
 uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
 
 You can install it using pip:
```

### Comparing `uptime_kuma_api-1.0.1/setup.py` & `uptime_kuma_api-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api/__init__.py` & `uptime_kuma_api-1.1.0/uptime_kuma_api/__init__.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api/api.py` & `uptime_kuma_api-1.1.0/uptime_kuma_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 from contextlib import contextmanager
 from copy import deepcopy
 from typing import Any
 
 import requests
 import socketio
+from packaging.version import parse as parse_version
 
 from . import (
     AuthMethod,
     DockerType,
     Event,
     IncidentStyle,
     MaintenanceStrategy,
@@ -54,15 +55,19 @@
         return
     if isinstance(data, list):
         for d in data:
             parse_value(d, key, type_, default)
     else:
         if key in data:
             if data[key] is not None:
-                data[key] = type_(data[key])
+                try:
+                    data[key] = type_(data[key])
+                except ValueError:
+                    # todo: add warning to logs
+                    pass
             elif default is not None:
                 data[key] = default
 
 
 # monitor
 def parse_monitor_status(data) -> None:
     parse_value(data, "status", MonitorStatus)
@@ -124,18 +129,18 @@
     if not kwargs["databaseConnectionString"]:
         if kwargs["type"] == MonitorType.SQLSERVER:
             kwargs["databaseConnectionString"] = "Server=<hostname>,<port>;Database=<your database>;User Id=<your user id>;Password=<your password>;Encrypt=<true/false>;TrustServerCertificate=<Yes/No>;Connection Timeout=<int>"
         elif kwargs["type"] == MonitorType.POSTGRES:
             kwargs["databaseConnectionString"] = "postgres://username:password@host:port/database"
         elif kwargs["type"] == MonitorType.MYSQL:
             kwargs["databaseConnectionString"] = "mysql://username:password@host:port/database"
-        elif kwargs["type"] == MonitorType.MONGODB:
-            kwargs["databaseConnectionString"] = "mongodb://username:password@host:port/database"
         elif kwargs["type"] == MonitorType.REDIS:
             kwargs["databaseConnectionString"] = "redis://user:password@host:port"
+        elif kwargs["type"] == MonitorType.MONGODB:
+            kwargs["databaseConnectionString"] = "mongodb://username:password@host:port/database"
 
     if kwargs["type"] == MonitorType.PUSH and not kwargs.get("pushToken"):
         kwargs["pushToken"] = gen_secret(10)
 
 
 def _build_notification_data(
     name: str,
@@ -183,57 +188,14 @@
         "active": active,
         "default": default,
         "applyExisting": applyExisting
     }
     return data
 
 
-def _build_status_page_data(
-    slug: str,
-
-    # config
-    id: int,
-    title: str,
-    description: str = None,
-    theme: str = "light",
-    published: bool = True,
-    showTags: bool = False,
-    domainNameList: list = None,
-    googleAnalyticsId: str = None,
-    customCSS: str = "",
-    footerText: str = None,
-    showPoweredBy: bool = True,
-
-    icon: str = "/icon.svg",
-    publicGroupList: list = None
-) -> tuple[str, dict, str, list]:
-    if theme not in ["light", "dark"]:
-        raise ValueError
-    if not domainNameList:
-        domainNameList = []
-    if not publicGroupList:
-        publicGroupList = []
-    config = {
-        "id": id,
-        "slug": slug,
-        "title": title,
-        "description": description,
-        "icon": icon,
-        "theme": theme,
-        "published": published,
-        "showTags": showTags,
-        "domainNameList": domainNameList,
-        "googleAnalyticsId": googleAnalyticsId,
-        "customCSS": customCSS,
-        "footerText": footerText,
-        "showPoweredBy": showPoweredBy
-    }
-    return slug, config, icon, publicGroupList
-
-
 def _convert_docker_host_input(kwargs) -> None:
     if not kwargs["dockerDaemon"]:
         if kwargs["dockerType"] == DockerType.SOCKET:
             kwargs["dockerDaemon"] = "/var/run/docker.sock"
         elif kwargs["dockerType"] == DockerType.TCP:
             kwargs["dockerDaemon"] = "tcp://localhost:2375"
 
@@ -311,15 +273,16 @@
         MonitorType.GAMEDIG: ["game", "hostname", "port"],
         MonitorType.MQTT: ["hostname", "port", "mqttTopic"],
         MonitorType.SQLSERVER: [],
         MonitorType.POSTGRES: [],
         MonitorType.MYSQL: [],
         MonitorType.MONGODB: [],
         MonitorType.RADIUS: ["radiusUsername", "radiusPassword", "radiusSecret", "radiusCalledStationId", "radiusCallingStationId"],
-        MonitorType.REDIS: []
+        MonitorType.REDIS: [],
+        MonitorType.GROUP: []
     }
     type_ = kwargs["type"]
     required_args = required_args_by_type[type_]
     _check_missing_arguments(required_args, kwargs)
 
     conditions = dict(
         interval=dict(
@@ -674,14 +637,15 @@
         info = self.info()
         return info.get("version")
 
     def _build_monitor_data(
             self,
             type: MonitorType,
             name: str,
+            parent: int = None,
             description: str = None,
             interval: int = 60,
             retryInterval: int = 60,
             resendInterval: int = 0,
             maxretries: int = 1,
             upsideDown: bool = False,
             notificationIDList: list = None,
@@ -766,14 +730,19 @@
             "notificationIDList": notificationIDList,
             "upsideDown": upsideDown,
             "resendInterval": resendInterval,
             "description": description,
             "httpBodyEncoding": httpBodyEncoding
         }
 
+        if parse_version(self.version) >= parse_version("1.22"):
+            data.update({
+                "parent": parent
+            })
+
         if type in [MonitorType.KEYWORD, MonitorType.GRPC_KEYWORD]:
             data.update({
                 "keyword": keyword,
             })
 
         # HTTP, KEYWORD
         data.update({
@@ -935,14 +904,62 @@
             "timeRange": timeRange,
             "cron": cron,
             "durationMinutes": durationMinutes,
             "timezoneOption": timezoneOption
         }
         return data
 
+    def _build_status_page_data(
+            self,
+            slug: str,
+
+            # config
+            id: int,
+            title: str,
+            description: str = None,
+            theme: str = None,
+            published: bool = True,
+            showTags: bool = False,
+            domainNameList: list = None,
+            googleAnalyticsId: str = None,
+            customCSS: str = "",
+            footerText: str = None,
+            showPoweredBy: bool = True,
+
+            icon: str = "/icon.svg",
+            publicGroupList: list = None
+    ) -> tuple[str, dict, str, list]:
+        if not theme:
+            if parse_version(self.version) >= parse_version("1.22"):
+                theme = "auto"
+            else:
+                theme = "light"
+        if theme not in ["auto", "light", "dark"]:
+            raise ValueError
+        if not domainNameList:
+            domainNameList = []
+        if not publicGroupList:
+            publicGroupList = []
+        config = {
+            "id": id,
+            "slug": slug,
+            "title": title,
+            "description": description,
+            "icon": icon,
+            "theme": theme,
+            "published": published,
+            "showTags": showTags,
+            "domainNameList": domainNameList,
+            "googleAnalyticsId": googleAnalyticsId,
+            "customCSS": customCSS,
+            "footerText": footerText,
+            "showPoweredBy": showPoweredBy
+        }
+        return slug, config, icon, publicGroupList
+
     # monitor
 
     def get_monitors(self) -> list[dict]:
         """
         Get all monitors.
 
         :return: A list of monitors.
@@ -957,60 +974,69 @@
                     'active': True,
                     'authDomain': None,
                     'authMethod': <AuthMethod.NONE: ''>,
                     'authWorkstation': None,
                     'basic_auth_pass': None,
                     'basic_auth_user': None,
                     'body': None,
+                    'childrenIDs': [],
                     'databaseConnectionString': None,
                     'databaseQuery': None,
+                    'description': None,
                     'dns_last_result': None,
                     'dns_resolve_server': '1.1.1.1',
                     'dns_resolve_type': 'A',
                     'docker_container': None,
                     'docker_host': None,
                     'expiryNotification': False,
+                    'forceInactive': False,
                     'game': None,
                     'grpcBody': None,
                     'grpcEnableTls': False,
                     'grpcMetadata': None,
                     'grpcMethod': None,
                     'grpcProtobuf': None,
                     'grpcServiceName': None,
                     'grpcUrl': None,
                     'headers': None,
                     'hostname': None,
+                    'httpBodyEncoding': 'json',
                     'id': 1,
                     'ignoreTls': False,
                     'includeSensitiveData': True,
                     'interval': 60,
                     'keyword': None,
                     'maintenance': False,
                     'maxredirects': 10,
-                    'maxretries': 1,
+                    'maxretries': 0,
                     'method': 'GET',
                     'mqttPassword': None,
                     'mqttSuccessMessage': None,
                     'mqttTopic': None,
                     'mqttUsername': None,
                     'name': 'monitor 1',
                     'notificationIDList': [1, 2],
                     'packetSize': 56,
+                    'parent': None,
+                    'pathName': 'monitor 1',
                     'port': None,
                     'proxyId': None,
                     'pushToken': None,
                     'radiusCalledStationId': None,
                     'radiusCallingStationId': None,
                     'radiusPassword': None,
                     'radiusSecret': None,
                     'radiusUsername': None,
                     'resendInterval': 0,
                     'retryInterval': 60,
                     'tags': [],
-                    'type': <MonitorType.HTTP: 'http'>
+                    'tlsCa': None,
+                    'tlsCert': None,
+                    'tlsKey': None,
+                    'type': <MonitorType.HTTP: 'http'>,
                     'upsideDown': False,
                     'url': 'http://127.0.0.1',
                     'weight': 2000
                 }
             ]
         """
 
@@ -1041,60 +1067,69 @@
                 'active': True,
                 'authDomain': None,
                 'authMethod': <AuthMethod.NONE: ''>,
                 'authWorkstation': None,
                 'basic_auth_pass': None,
                 'basic_auth_user': None,
                 'body': None,
+                'childrenIDs': [],
                 'databaseConnectionString': None,
                 'databaseQuery': None,
+                'description': None,
                 'dns_last_result': None,
                 'dns_resolve_server': '1.1.1.1',
                 'dns_resolve_type': 'A',
                 'docker_container': None,
                 'docker_host': None,
                 'expiryNotification': False,
+                'forceInactive': False,
                 'game': None,
                 'grpcBody': None,
                 'grpcEnableTls': False,
                 'grpcMetadata': None,
                 'grpcMethod': None,
                 'grpcProtobuf': None,
                 'grpcServiceName': None,
                 'grpcUrl': None,
                 'headers': None,
                 'hostname': None,
+                'httpBodyEncoding': 'json',
                 'id': 1,
                 'ignoreTls': False,
                 'includeSensitiveData': True,
                 'interval': 60,
                 'keyword': None,
                 'maintenance': False,
                 'maxredirects': 10,
-                'maxretries': 1,
+                'maxretries': 0,
                 'method': 'GET',
                 'mqttPassword': None,
                 'mqttSuccessMessage': None,
                 'mqttTopic': None,
                 'mqttUsername': None,
                 'name': 'monitor 1',
                 'notificationIDList': [1, 2],
                 'packetSize': 56,
+                'parent': None,
+                'pathName': 'monitor 1',
                 'port': None,
                 'proxyId': None,
                 'pushToken': None,
                 'radiusCalledStationId': None,
                 'radiusCallingStationId': None,
                 'radiusPassword': None,
                 'radiusSecret': None,
                 'radiusUsername': None,
                 'resendInterval': 0,
                 'retryInterval': 60,
                 'tags': [],
-                'type': <MonitorType.HTTP: 'http'>
+                'tlsCa': None,
+                'tlsCert': None,
+                'tlsKey': None,
+                'type': <MonitorType.HTTP: 'http'>,
                 'upsideDown': False,
                 'url': 'http://127.0.0.1',
                 'weight': 2000
             }
         """
         r = self._call('getMonitor', id_)["monitor"]
         _convert_monitor_return(r)
@@ -1777,15 +1812,14 @@
                 'maintenanceList': [],
                 'publicGroupList': [
                     {
                         'id': 1,
                         'monitorList': [
                             {
                                 'id': 1,
-                                'maintenance': False,
                                 'name': 'monitor 1',
                                 'sendUrl': 0
                             }
                         ],
                         'name': 'Services',
                         'weight': 1
                     }
@@ -1867,15 +1901,15 @@
         """
         Save a status page.
 
         :param str slug: Slug
         :param int id: Id of the status page to save
         :param str title: Title
         :param str, optional description: Description, defaults to None
-        :param str, optional theme: Switch Theme, defaults to "light"
+        :param str, optional theme: Switch Theme, defaults to "auto"
         :param bool, optional published: Published, defaults to True
         :param bool, optional showTags: Show Tags, defaults to False
         :param list, optional domainNameList: Domain Names, defaults to None
         :param str, optional googleAnalyticsId: Google Analytics ID, defaults to None
         :param str, optional customCSS: Custom CSS, defaults to ""
         :param str, optional footerText: Custom Footer, defaults to None
         :param bool, optional showPoweredBy: Show Powered By, defaults to True
@@ -1919,15 +1953,15 @@
                 ]
             }
         """
         status_page = self.get_status_page(slug)
         status_page.pop("incident")
         status_page.pop("maintenanceList")
         status_page.update(kwargs)
-        data = _build_status_page_data(**status_page)
+        data = self._build_status_page_data(**status_page)
         r = self._call('saveStatusPage', data)
 
         # uptime kuma does not send the status page list event when a status page is saved
         status_page = self._call('getStatusPage', slug)["config"]
         status_page_id = status_page["id"]
         if self._event_data[Event.STATUS_PAGE_LIST] is None:
             self._event_data[Event.STATUS_PAGE_LIST] = {}
@@ -3456,20 +3490,18 @@
         :raises UptimeKumaException: If the server returns an error.
 
         Example::
 
             >>> api.get_monitor_maintenance(1)
             [
                 {
-                    "id": 1,
-                    "name": "monitor 1"
+                    "id": 1
                 },
                 {
-                    "id": 2,
-                    "name": "monitor 2"
+                    "id": 2
                 }
             ]
         """
         return self._call('getMonitorMaintenance', id_)["monitors"]
 
     def add_monitor_maintenance(
             self,
```

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api/docstrings.py` & `uptime_kuma_api-1.1.0/uptime_kuma_api/docstrings.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     return _doc
 
 
 def monitor_docstring(mode) -> str:
     return f"""
         :param MonitorType{", optional" if mode == "edit" else ""} type: Monitor Type
         :param str{", optional" if mode == "edit" else ""} name: Friendly Name
+        :param str, optional parent: Id of the monitor group, defaults to None
         :param str, optional description: Description, defaults to None
         :param int, optional interval: Heartbeat Interval, defaults to 60
         :param int, optional retryInterval: Retry every X seconds, defaults to 60
         :param int, optional resendInterval: Resend every X times, defaults to 0
         :param int, optional maxretries: Retries. Maximum retries before the service is marked as down and a notification is sent., defaults to 0
         :param bool, optional upsideDown: Upside Down Mode. Flip the status upside down. If the service is reachable, it is DOWN., defaults to False
         :param list, optional notificationIDList: Notifications, defaults to None
@@ -129,20 +130,22 @@
         :param str, optional accessToken: Notification option for ``type`` :attr:`~.NotificationType.MATRIX`.
         :param str, optional homeserverUrl: Notification option for ``type`` :attr:`~.NotificationType.MATRIX`.
         :param str mattermostusername: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
         :param str, optional mattermostWebhookUrl: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
         :param str mattermostchannel: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
         :param str mattermosticonemo: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
         :param str mattermosticonurl: Notification option for ``type`` :attr:`~.NotificationType.MATTERMOST`.
+        :param str ntfyAuthenticationMethod: Notification option for ``type`` :attr:`~.NotificationType.NTFY`. Authentication Method.
         :param str ntfyusername: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
         :param str ntfypassword: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
+        :param str ntfyaccesstoken: Notification option for ``type`` :attr:`~.NotificationType.NTFY`. Access Token.
         :param str, optional ntfytopic: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
         :param int, optional ntfyPriority: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
-        :param str ntfyIcon: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
         :param str, optional ntfyserverurl: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
+        :param str ntfyIcon: Notification option for ``type`` :attr:`~.NotificationType.NTFY`.
         :param str octopushVersion: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
         :param str, optional octopushAPIKey: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
         :param str, optional octopushLogin: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
         :param str, optional octopushPhoneNumber: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
         :param str octopushSMSType: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
         :param str octopushSenderName: Notification option for ``type`` :attr:`~.NotificationType.OCTOPUSH`.
         :param str, optional httpAddr: Notification option for ``type`` :attr:`~.NotificationType.ONEBOT`.
@@ -192,14 +195,15 @@
         :param str, optional pushdeerKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHDEER`.
         :param str, optional pushoveruserkey: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
         :param str, optional pushoverapptoken: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
         :param str pushoversounds: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
         :param str pushoverpriority: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
         :param str pushovertitle: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
         :param str pushoverdevice: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`.
+        :param int pushoverttl: Notification option for ``type`` :attr:`~.NotificationType.PUSHOVER`. Message TTL (Seconds).
         :param str, optional pushyAPIKey: Notification option for ``type`` :attr:`~.NotificationType.PUSHY`.
         :param str, optional pushyToken: Notification option for ``type`` :attr:`~.NotificationType.PUSHY`.
         :param str rocketchannel: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`.
         :param str rocketusername: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`.
         :param str rocketiconemo: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`.
         :param str, optional rocketwebhookURL: Notification option for ``type`` :attr:`~.NotificationType.ROCKET_CHAT`.
         :param str, optional serverChanSendKey: Notification option for ``type`` :attr:`~.NotificationType.SERVERCHAN`.
```

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api/event.py` & `uptime_kuma_api-1.1.0/uptime_kuma_api/event.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api/maintenance_strategy.py` & `uptime_kuma_api-1.1.0/uptime_kuma_api/maintenance_strategy.py`

 * *Files identical despite different names*

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api/monitor_type.py` & `uptime_kuma_api-1.1.0/uptime_kuma_api/monitor_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,7 +50,10 @@
     """MongoDB"""
 
     RADIUS = "radius"
     """Radius"""
 
     REDIS = "redis"
     """Redis"""
+
+    GROUP = "group"
+    """Group"""
```

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api/notification_providers.py` & `uptime_kuma_api-1.1.0/uptime_kuma_api/notification_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,20 +255,22 @@
         mattermostusername=dict(type="str", required=False),
         mattermostWebhookUrl=dict(type="str", required=True),
         mattermostchannel=dict(type="str", required=False),
         mattermosticonemo=dict(type="str", required=False),
         mattermosticonurl=dict(type="str", required=False),
     ),
     NotificationType.NTFY: dict(
+        ntfyAuthenticationMethod=dict(type="str", required=False),
         ntfyusername=dict(type="str", required=False),
         ntfypassword=dict(type="str", required=False),
+        ntfyaccesstoken=dict(type="str", required=False),
         ntfytopic=dict(type="str", required=True),
         ntfyPriority=dict(type="int", required=True),
-        ntfyIcon=dict(type="str", required=False),
         ntfyserverurl=dict(type="str", required=True),
+        ntfyIcon=dict(type="str", required=False),
     ),
     NotificationType.OCTOPUSH: dict(
         octopushVersion=dict(type="str", required=False),
         octopushAPIKey=dict(type="str", required=True),
         octopushLogin=dict(type="str", required=True),
         octopushPhoneNumber=dict(type="str", required=True),
         octopushSMSType=dict(type="str", required=False),
@@ -313,14 +315,15 @@
     NotificationType.PUSHOVER: dict(
         pushoveruserkey=dict(type="str", required=True),
         pushoverapptoken=dict(type="str", required=True),
         pushoversounds=dict(type="str", required=False),
         pushoverpriority=dict(type="str", required=False),
         pushovertitle=dict(type="str", required=False),
         pushoverdevice=dict(type="str", required=False),
+        pushoverttl=dict(type="int", required=False),
     ),
     NotificationType.PUSHY: dict(
         pushyAPIKey=dict(type="str", required=True),
         pushyToken=dict(type="str", required=True),
     ),
     NotificationType.ROCKET_CHAT: dict(
         rocketchannel=dict(type="str", required=False),
@@ -432,14 +435,17 @@
         min=1,
         max=5,
     ),
     opsgeniePriority=dict(
         min=1,
         max=5,
     ),
+    pushoverttl=dict(
+        min=0,
+    ),
     smseaglePriority=dict(
         min=0,
         max=9,
     ),
     smtpPort=dict(
         min=0,
         max=65535,
```

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/PKG-INFO` & `uptime_kuma_api-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,86 @@
 Metadata-Version: 2.1
-Name: uptime-kuma-api
-Version: 1.0.1
+Name: uptime_kuma_api
+Version: 1.1.0
 Summary: A python wrapper for the Uptime Kuma WebSocket API
 Home-page: https://github.com/lucasheld/uptime-kuma-api
 Author: Lucas Held
 Author-email: lucasheld@hotmail.de
 License: MIT
+Description: # uptime-kuma-api
+        
+        A wrapper for the Uptime Kuma Socket.IO API
+        ---
+        uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
+        
+        This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
+        
+        Python version 3.7+ is required.
+        
+        Supported Uptime Kuma versions:
+        
+        | Uptime Kuma     | uptime-kuma-api |
+        |-----------------|-----------------|
+        | 1.21.3 - 1.22.1 | 1.0.0 - 1.1.0   |
+        | 1.17.0 - 1.21.2 | 0.1.0 - 0.13.0  |
+        
+        Installation
+        ---
+        uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
+        
+        You can install it using pip:
+        
+        ```
+        pip install uptime-kuma-api
+        ```
+        
+        Documentation
+        ---
+        The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
+        
+        Example
+        ---
+        Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
+        
+        To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
+        
+        ```python
+        >>> from uptime_kuma_api import UptimeKumaApi, MonitorType
+        >>> api = UptimeKumaApi('INSERT_URL')
+        >>> api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+        ```
+        
+        Now you can call one of the existing methods of the instance. For example create a new monitor:
+        
+        ```python
+        >>> result = api.add_monitor(type=MonitorType.HTTP, name="Google", url="https://google.com")
+        >>> print(result)
+        {'msg': 'Added Successfully.', 'monitorId': 1}
+        ```
+        
+        At the end, the connection to the API must be disconnected so that the program does not block.
+        
+        ```python
+        >>> api.disconnect()
+        ```
+        
+        With a context manager, the disconnect method is called automatically:
+        
+        ```python
+        from uptime_kuma_api import UptimeKumaApi
+        
+        with UptimeKumaApi('INSERT_URL') as api:
+            api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
+            api.add_monitor(
+                type=MonitorType.HTTP,
+                name="Google",
+                url="https://google.com"
+            )
+        ```
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -21,81 +92,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# uptime-kuma-api
-
-A wrapper for the Uptime Kuma Socket.IO API
----
-uptime-kuma-api is a Python wrapper for the [Uptime Kuma](https://github.com/louislam/uptime-kuma) Socket.IO API.
-
-This package was developed to configure Uptime Kuma with Ansible. The Ansible collection can be found at https://github.com/lucasheld/ansible-uptime-kuma.
-
-Python version 3.7+ is required.
-
-Supported Uptime Kuma versions:
-
-| Uptime Kuma     | uptime-kuma-api |
-|-----------------|-----------------|
-| 1.21.3          | 1.0.0           |
-| 1.17.0 - 1.21.2 | 0.1.0 - 0.13.0  |
-
-Installation
----
-uptime-kuma-api is available on the [Python Package Index (PyPI)](https://pypi.org/project/uptime-kuma-api/).
-
-You can install it using pip:
-
-```
-pip install uptime-kuma-api
-```
-
-Documentation
----
-The API Reference is available on [Read the Docs](https://uptime-kuma-api.readthedocs.io).
-
-Example
----
-Once you have installed the python package, you can use it to communicate with an Uptime Kuma instance.
-
-To do so, import `UptimeKumaApi` from the library and specify the Uptime Kuma server url (e.g. 'http://127.0.0.1:3001'), username and password to initialize the connection.
-
-```python
->>> from uptime_kuma_api import UptimeKumaApi, MonitorType
->>> api = UptimeKumaApi('INSERT_URL')
->>> api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
-```
-
-Now you can call one of the existing methods of the instance. For example create a new monitor:
-
-```python
->>> result = api.add_monitor(type=MonitorType.HTTP, name="Google", url="https://google.com")
->>> print(result)
-{'msg': 'Added Successfully.', 'monitorId': 1}
-```
-
-At the end, the connection to the API must be disconnected so that the program does not block.
-
-```python
->>> api.disconnect()
-```
-
-With a context manager, the disconnect method is called automatically:
-
-```python
-from uptime_kuma_api import UptimeKumaApi
-
-with UptimeKumaApi('INSERT_URL') as api:
-    api.login('INSERT_USERNAME', 'INSERT_PASSWORD')
-    api.add_monitor(
-        type=MonitorType.HTTP,
-        name="Google",
-        url="https://google.com"
-    )
-```
-
-
```

### Comparing `uptime_kuma_api-1.0.1/uptime_kuma_api.egg-info/SOURCES.txt` & `uptime_kuma_api-1.1.0/uptime_kuma_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

