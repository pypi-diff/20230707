# Comparing `tmp/smartapi-python-1.3.4.tar.gz` & `tmp/smartapi-python-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartapi-python-1.3.4.tar", last modified: Wed Jun 28 12:57:17 2023, max compression
+gzip compressed data, was "smartapi-python-1.3.5.tar", last modified: Fri Jul  7 11:44:36 2023, max compression
```

## Comparing `smartapi-python-1.3.4.tar` & `smartapi-python-1.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 rima      (1000) rima      (1000)        0 2023-06-28 12:57:17.892564 smartapi-python-1.3.4/
--rw-rw-r--   0 rima      (1000) rima      (1000)     5709 2023-06-28 12:57:17.892564 smartapi-python-1.3.4/PKG-INFO
--rw-rw-r--   0 rima      (1000) rima      (1000)     4765 2023-06-28 10:10:30.000000 smartapi-python-1.3.4/README.md
-drwxrwxr-x   0 rima      (1000) rima      (1000)        0 2023-06-28 12:57:17.892564 smartapi-python-1.3.4/SmartApi/
--rw-rw-r--   0 rima      (1000) rima      (1000)      250 2023-06-28 12:24:44.000000 smartapi-python-1.3.4/SmartApi/__init__.py
--rw-rw-r--   0 rima      (1000) rima      (1000)     5937 2023-06-19 07:12:24.000000 smartapi-python-1.3.4/SmartApi/smartApiWebsocket.py
--rw-rw-r--   0 rima      (1000) rima      (1000)    15065 2023-06-28 12:39:21.000000 smartapi-python-1.3.4/SmartApi/smartConnect.py
--rw-rw-r--   0 rima      (1000) rima      (1000)     2176 2023-06-19 07:12:24.000000 smartapi-python-1.3.4/SmartApi/smartExceptions.py
--rw-rw-r--   0 rima      (1000) rima      (1000)    16867 2023-06-26 10:05:44.000000 smartapi-python-1.3.4/SmartApi/smartWebSocketV2.py
--rw-rw-r--   0 rima      (1000) rima      (1000)      541 2023-06-28 12:54:30.000000 smartapi-python-1.3.4/SmartApi/version.py
--rw-rw-r--   0 rima      (1000) rima      (1000)    15272 2023-06-28 08:19:24.000000 smartapi-python-1.3.4/SmartApi/webSocket.py
--rw-rw-r--   0 rima      (1000) rima      (1000)       38 2023-06-28 12:57:17.892564 smartapi-python-1.3.4/setup.cfg
--rw-rw-r--   0 rima      (1000) rima      (1000)     1283 2023-06-28 12:54:18.000000 smartapi-python-1.3.4/setup.py
-drwxrwxr-x   0 rima      (1000) rima      (1000)        0 2023-06-28 12:57:17.892564 smartapi-python-1.3.4/smartapi_python.egg-info/
--rw-rw-r--   0 rima      (1000) rima      (1000)     5709 2023-06-28 12:57:17.000000 smartapi-python-1.3.4/smartapi_python.egg-info/PKG-INFO
--rw-rw-r--   0 rima      (1000) rima      (1000)      417 2023-06-28 12:57:17.000000 smartapi-python-1.3.4/smartapi_python.egg-info/SOURCES.txt
--rw-rw-r--   0 rima      (1000) rima      (1000)        1 2023-06-28 12:57:17.000000 smartapi-python-1.3.4/smartapi_python.egg-info/dependency_links.txt
--rw-rw-r--   0 rima      (1000) rima      (1000)       52 2023-06-28 12:57:17.000000 smartapi-python-1.3.4/smartapi_python.egg-info/requires.txt
--rw-rw-r--   0 rima      (1000) rima      (1000)       14 2023-06-28 12:57:17.000000 smartapi-python-1.3.4/smartapi_python.egg-info/top_level.txt
-drwxrwxr-x   0 rima      (1000) rima      (1000)        0 2023-06-28 12:57:17.892564 smartapi-python-1.3.4/test/
--rw-rw-r--   0 rima      (1000) rima      (1000)        0 2023-04-19 08:19:43.000000 smartapi-python-1.3.4/test/__init__.py
--rw-rw-r--   0 rima      (1000) rima      (1000)     4436 2023-06-28 10:00:54.000000 smartapi-python-1.3.4/test/test.py
+drwxrwxr-x   0 rima      (1000) rima      (1000)        0 2023-07-07 11:44:36.372247 smartapi-python-1.3.5/
+-rw-rw-r--   0 rima      (1000) rima      (1000)     5825 2023-07-07 11:44:36.372247 smartapi-python-1.3.5/PKG-INFO
+-rw-rw-r--   0 rima      (1000) rima      (1000)     4881 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/README.md
+drwxrwxr-x   0 rima      (1000) rima      (1000)        0 2023-07-07 11:44:36.372247 smartapi-python-1.3.5/SmartApi/
+-rw-rw-r--   0 rima      (1000) rima      (1000)      250 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/SmartApi/__init__.py
+-rw-rw-r--   0 rima      (1000) rima      (1000)     5937 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/SmartApi/smartApiWebsocket.py
+-rw-rw-r--   0 rima      (1000) rima      (1000)    15055 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/SmartApi/smartConnect.py
+-rw-rw-r--   0 rima      (1000) rima      (1000)     2176 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/SmartApi/smartExceptions.py
+-rw-rw-r--   0 rima      (1000) rima      (1000)    16797 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/SmartApi/smartWebSocketV2.py
+-rw-rw-r--   0 rima      (1000) rima      (1000)      531 2023-07-07 11:24:41.000000 smartapi-python-1.3.5/SmartApi/version.py
+-rw-rw-r--   0 rima      (1000) rima      (1000)    15273 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/SmartApi/webSocket.py
+-rw-rw-r--   0 rima      (1000) rima      (1000)       38 2023-07-07 11:44:36.372247 smartapi-python-1.3.5/setup.cfg
+-rw-rw-r--   0 rima      (1000) rima      (1000)     1283 2023-07-07 11:43:08.000000 smartapi-python-1.3.5/setup.py
+drwxrwxr-x   0 rima      (1000) rima      (1000)        0 2023-07-07 11:44:36.372247 smartapi-python-1.3.5/smartapi_python.egg-info/
+-rw-rw-r--   0 rima      (1000) rima      (1000)     5825 2023-07-07 11:44:36.000000 smartapi-python-1.3.5/smartapi_python.egg-info/PKG-INFO
+-rw-rw-r--   0 rima      (1000) rima      (1000)      417 2023-07-07 11:44:36.000000 smartapi-python-1.3.5/smartapi_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 rima      (1000) rima      (1000)        1 2023-07-07 11:44:36.000000 smartapi-python-1.3.5/smartapi_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 rima      (1000) rima      (1000)       52 2023-07-07 11:44:36.000000 smartapi-python-1.3.5/smartapi_python.egg-info/requires.txt
+-rw-rw-r--   0 rima      (1000) rima      (1000)       14 2023-07-07 11:44:36.000000 smartapi-python-1.3.5/smartapi_python.egg-info/top_level.txt
+drwxrwxr-x   0 rima      (1000) rima      (1000)        0 2023-07-07 11:44:36.372247 smartapi-python-1.3.5/test/
+-rw-rw-r--   0 rima      (1000) rima      (1000)       24 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/test/__init__.py
+-rw-rw-r--   0 rima      (1000) rima      (1000)     4436 2023-06-30 09:33:49.000000 smartapi-python-1.3.5/test/test.py
```

### Comparing `smartapi-python-1.3.4/PKG-INFO` & `smartapi-python-1.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartapi-python
-Version: 1.3.4
+Version: 1.3.5
 Summary: Angel Broking openApi integration
 Home-page: https://github.com/angelbroking-github/smartapi-python
 Author: ab-smartapi
 Author-email: smartapi.sdk@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,23 +19,23 @@
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 
 # SMARTAPI-PYTHON
 
-SMARTAPI-PYTHON is a Python library for dealing AMX,that is a set of REST-like HTTP APIs that expose many capabilities required to build stock market investment and trading platforms. It lets you execute orders in real time.
-
+SMARTAPI-PYTHON is a Python library for interacting with Angel's Trading platform  ,that is a set of REST-like HTTP APIs that expose many capabilities required to build stock market investment and trading platforms. It lets you execute orders in real time..
 
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install smartapi-python.
 
 ```bash
+pip install -r requirements_dev.txt       # for downloading the other required packages
 pip install smartapi-python
 pip install websocket-client
 ```
 
 ## Usage
 
 ```python
@@ -62,15 +62,14 @@
 feedToken = smartApi.getfeedToken()
 
 # fetch User Profile
 res = smartApi.getProfile(refreshToken)
 smartApi.generateToken(refreshToken)
 res=res['data']['exchanges']
 
-
 #place order
 try:
     orderparams = {
         "variety": "NORMAL",
         "tradingsymbol": "SBIN-EQ",
         "symboltoken": "3045",
         "transactiontype": "BUY",
@@ -219,13 +218,10 @@
 sws.on_open = on_open
 sws.on_data = on_data
 sws.on_error = on_error
 sws.on_close = on_close
 
 sws.connect()
 
-
 ```
 
 
-
-
```

### Comparing `smartapi-python-1.3.4/README.md` & `smartapi-python-1.3.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SMARTAPI-PYTHON
 
-SMARTAPI-PYTHON is a Python library for dealing AMX,that is a set of REST-like HTTP APIs that expose many capabilities required to build stock market investment and trading platforms. It lets you execute orders in real time.
-
+SMARTAPI-PYTHON is a Python library for interacting with Angel's Trading platform  ,that is a set of REST-like HTTP APIs that expose many capabilities required to build stock market investment and trading platforms. It lets you execute orders in real time..
 
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install smartapi-python.
 
 ```bash
+pip install -r requirements_dev.txt       # for downloading the other required packages
 pip install smartapi-python
 pip install websocket-client
 ```
 
 ## Usage
 
 ```python
@@ -39,15 +39,14 @@
 feedToken = smartApi.getfeedToken()
 
 # fetch User Profile
 res = smartApi.getProfile(refreshToken)
 smartApi.generateToken(refreshToken)
 res=res['data']['exchanges']
 
-
 #place order
 try:
     orderparams = {
         "variety": "NORMAL",
         "tradingsymbol": "SBIN-EQ",
         "symboltoken": "3045",
         "transactiontype": "BUY",
@@ -196,11 +195,8 @@
 sws.on_open = on_open
 sws.on_data = on_data
 sws.on_error = on_error
 sws.on_close = on_close
 
 sws.connect()
 
-
 ```
-
-
```

### Comparing `smartapi-python-1.3.4/SmartApi/smartApiWebsocket.py` & `smartapi-python-1.3.5/SmartApi/smartApiWebsocket.py`

 * *Files identical despite different names*

### Comparing `smartapi-python-1.3.4/SmartApi/smartConnect.py` & `smartapi-python-1.3.5/SmartApi/smartConnect.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,16 @@
         }
 
     def setSessionExpiryHook(self, method):
         if not callable(method):
             raise TypeError("Invalid input type. Only functions are accepted.")
         self.session_expiry_hook = method
     
-    def getUserId(self):
-        return self.userId
+    def getUserId():
+        return userId
 
     def setUserId(self,id):
         self.userId=id
 
     def setAccessToken(self, access_token):
 
         self.access_token = access_token
@@ -212,21 +212,21 @@
     def _postRequest(self, route, params=None):
         """Alias for sending a POST request."""
         return self._request(route, "POST", params)
     def _getRequest(self, route, params=None):
         """Alias for sending a GET request."""
         return self._request(route, "GET", params)
 
-    def generateSession(self, clientCode, password, totp):
-
-        params = {"clientcode": clientCode, "password": password, "totp": totp}
-        loginResultObject = self._postRequest("api.login", params)
-
-        if loginResultObject['status'] == True:
-            jwtToken = loginResultObject['data']['jwtToken']
+    def generateSession(self,clientCode,password,totp):
+        
+        params={"clientcode":clientCode,"password":password,"totp":totp}
+        loginResultObject=self._postRequest("api.login",params)
+        
+        if loginResultObject['status']==True:
+            jwtToken=loginResultObject['data']['jwtToken']
             self.setAccessToken(jwtToken)
             refreshToken = loginResultObject['data']['refreshToken']
             feedToken = loginResultObject['data']['feedToken']
             self.setRefreshToken(refreshToken)
             self.setFeedToken(feedToken)
             user = self.getProfile(refreshToken)
```

### Comparing `smartapi-python-1.3.4/SmartApi/smartExceptions.py` & `smartapi-python-1.3.5/SmartApi/smartExceptions.py`

 * *Files identical despite different names*

### Comparing `smartapi-python-1.3.4/SmartApi/smartWebSocketV2.py` & `smartapi-python-1.3.5/SmartApi/smartWebSocketV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,51 +100,52 @@
         if self.RESUBSCRIBE_FLAG:
             self.resubscribe()
             self.RESUBSCRIBE_FLAG = False  # Add this line to prevent resubscription on subsequent reconnects
         else:
             self.on_open(wsapp)
 
     def _on_pong(self, wsapp, data):
-        # if data == self.HEART_BEAT_MESSAGE:
+        if data == self.HEART_BEAT_MESSAGE:
             timestamp = time.time()
             formatted_timestamp = time.strftime("%d-%m-%y %H:%M:%S", time.localtime(timestamp))
             print(f"In on pong function ==> {data}, Timestamp: {formatted_timestamp}")
             self.last_pong_timestamp = timestamp
-        # else:
-        #     # Handle the received feed data here
-        #     self.on_data(wsapp, data)
+        else:
+            # Handle the received feed data here
+            self.on_data(wsapp, data)
 
     def _on_ping(self, wsapp, data):
         timestamp = time.time()
         formatted_timestamp = time.strftime("%d-%m-%y %H:%M:%S", time.localtime(timestamp))
         print(f"In on ping function ==> {data}, Timestamp: {formatted_timestamp}")
         self.last_ping_timestamp = timestamp
 
     def check_connection_status(self):
         current_time = time.time()
-        if self.last_pong_timestamp is not None and current_time - self.last_pong_timestamp > 2 * self.HEART_BEAT_MESSAGE:
+        if self.last_pong_timestamp is not None and current_time - self.last_pong_timestamp > 2*self.HEART_BEAT_MESSAGE:
             # Stale connection detected, take appropriate action
             self.close_connection()
             self.connect()
 
     def start_ping_timer(self):
         def send_ping():
             try:
-                current_time = time.time()
-                if self.last_pong_timestamp is None or current_time - self.last_pong_timestamp > self.HEART_BEAT_INTERVAL:
-                    self.wsapp.ping(self.HEART_BEAT_MESSAGE)
-                    self.last_ping_timestamp = current_time
+                current_time = datetime.now()
+                if self.last_pong_timestamp is None or self.last_pong_timestamp < current_time - timedelta(self.HEART_BEAT_MESSAGE):
+                    # print("stale connection detected")
+                    # self.wsapp.close()
+                    self.connect()
                 else:
-                    self.last_ping_timestamp = current_time
-                Timer(self.HEART_BEAT_INTERVAL, send_ping).start()  # Schedule the next ping
+                    self.last_ping_timestamp = time.time()
             except Exception as e:
                 self.wsapp.close()
                 self.resubscribe()
 
-        Timer(self.HEART_BEAT_INTERVAL, send_ping).start()
+        ping_timer = Timer(5, send_ping)
+        ping_timer.start()
 
     def subscribe(self, correlation_id, mode, token_list):
         """
             This Function subscribe the price data for the given token
             Parameters
             ------
             correlation_id: string
```

### Comparing `smartapi-python-1.3.4/SmartApi/version.py` & `smartapi-python-1.3.5/SmartApi/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = "smartapi-python"
 __description__ = "Angel Broking openApi integration"
 __url__ = "https://www.angelbroking.com/"
-__download_url__ = "https://github.com/angelbroking-github/smartapi-python"
-__version__ = "1.3.4"
+__download_url__ = "https://github.com/angel-one/smartapi-python"
+__version__ = "1.3.5"
 __author__ = "ab-smartapi"
 __token__ = "ab-smartapi"
 __author_email__ = "smartapi.sdk@gmail.com"
 
 
 # [pypi]
 # username = __token__
```

### Comparing `smartapi-python-1.3.4/SmartApi/webSocket.py` & `smartapi-python-1.3.5/SmartApi/webSocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import six
 import sys
 import time
 import json
 import struct
 import logging
 import threading
```

### Comparing `smartapi-python-1.3.4/setup.py` & `smartapi-python-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         "requests>=2.18.4",
         "six>=1.11.0",
         "python-dateutil>=2.6.1"
     ]
 
 setup(
     name="smartapi-python",
-    version="1.3.4",
+    version="1.3.5",
     author="ab-smartapi",
     author_email="smartapi.sdk@gmail.com",
     description="Angel Broking openApi integration",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/angelbroking-github/smartapi-python",
     packages=find_packages(),
```

### Comparing `smartapi-python-1.3.4/smartapi_python.egg-info/PKG-INFO` & `smartapi-python-1.3.5/smartapi_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartapi-python
-Version: 1.3.4
+Version: 1.3.5
 Summary: Angel Broking openApi integration
 Home-page: https://github.com/angelbroking-github/smartapi-python
 Author: ab-smartapi
 Author-email: smartapi.sdk@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,23 +19,23 @@
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 
 # SMARTAPI-PYTHON
 
-SMARTAPI-PYTHON is a Python library for dealing AMX,that is a set of REST-like HTTP APIs that expose many capabilities required to build stock market investment and trading platforms. It lets you execute orders in real time.
-
+SMARTAPI-PYTHON is a Python library for interacting with Angel's Trading platform  ,that is a set of REST-like HTTP APIs that expose many capabilities required to build stock market investment and trading platforms. It lets you execute orders in real time..
 
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install smartapi-python.
 
 ```bash
+pip install -r requirements_dev.txt       # for downloading the other required packages
 pip install smartapi-python
 pip install websocket-client
 ```
 
 ## Usage
 
 ```python
@@ -62,15 +62,14 @@
 feedToken = smartApi.getfeedToken()
 
 # fetch User Profile
 res = smartApi.getProfile(refreshToken)
 smartApi.generateToken(refreshToken)
 res=res['data']['exchanges']
 
-
 #place order
 try:
     orderparams = {
         "variety": "NORMAL",
         "tradingsymbol": "SBIN-EQ",
         "symboltoken": "3045",
         "transactiontype": "BUY",
@@ -219,13 +218,10 @@
 sws.on_open = on_open
 sws.on_data = on_data
 sws.on_error = on_error
 sws.on_close = on_close
 
 sws.connect()
 
-
 ```
 
 
-
-
```

### Comparing `smartapi-python-1.3.4/test/test.py` & `smartapi-python-1.3.5/test/test.py`

 * *Files identical despite different names*

