# Comparing `tmp/supergood-1.0.8.tar.gz` & `tmp/supergood-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supergood-1.0.8.tar", last modified: Fri Mar 10 06:38:19 2023, max compression
+gzip compressed data, was "supergood-1.0.9.tar", last modified: Wed Apr 19 17:36:11 2023, max compression
```

## Comparing `supergood-1.0.8.tar` & `supergood-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-03-10 06:38:19.558857 supergood-1.0.8/
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     4714 2023-03-03 05:10:33.000000 supergood-1.0.8/LICENSE
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     1065 2023-03-10 06:38:19.558954 supergood-1.0.8/PKG-INFO
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      719 2023-03-02 17:21:43.000000 supergood-1.0.8/README.md
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      153 2023-03-10 06:38:19.559309 supergood-1.0.8/setup.cfg
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      886 2023-03-10 06:38:05.000000 supergood-1.0.8/setup.py
-drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-03-10 06:38:19.552987 supergood-1.0.8/src/
-drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-03-10 06:38:19.555287 supergood-1.0.8/src/supergood/
--rw-r--r--   0 alexklarfeld   (501) staff       (20)       49 2023-03-02 23:55:20.000000 supergood-1.0.8/src/supergood/__init__.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     1884 2023-03-10 06:20:26.000000 supergood-1.0.8/src/supergood/api.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     7516 2023-03-10 05:50:18.000000 supergood-1.0.8/src/supergood/client.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     1294 2023-03-10 05:49:31.000000 supergood-1.0.8/src/supergood/constants.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     2148 2023-03-10 01:12:43.000000 supergood-1.0.8/src/supergood/helpers.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      725 2023-03-02 17:21:43.000000 supergood-1.0.8/src/supergood/logger.py
-drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-03-10 06:38:19.557234 supergood-1.0.8/src/supergood/vendors/
--rw-r--r--   0 alexklarfeld   (501) staff       (20)        0 2023-03-08 02:17:36.000000 supergood-1.0.8/src/supergood/vendors/__init__.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     1305 2023-03-08 21:06:35.000000 supergood-1.0.8/src/supergood/vendors/aiohttp.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     2081 2023-03-09 05:01:39.000000 supergood-1.0.8/src/supergood/vendors/http.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      446 2023-03-08 04:24:53.000000 supergood-1.0.8/src/supergood/vendors/requests.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     1063 2023-03-08 20:27:52.000000 supergood-1.0.8/src/supergood/vendors/urllib3.py
-drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-03-10 06:38:19.556099 supergood-1.0.8/src/supergood.egg-info/
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     1065 2023-03-10 06:38:19.000000 supergood-1.0.8/src/supergood.egg-info/PKG-INFO
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      674 2023-03-10 06:38:19.000000 supergood-1.0.8/src/supergood.egg-info/SOURCES.txt
--rw-r--r--   0 alexklarfeld   (501) staff       (20)        1 2023-03-10 06:38:19.000000 supergood-1.0.8/src/supergood.egg-info/dependency_links.txt
--rw-r--r--   0 alexklarfeld   (501) staff       (20)       32 2023-03-10 06:38:19.000000 supergood-1.0.8/src/supergood.egg-info/requires.txt
--rw-r--r--   0 alexklarfeld   (501) staff       (20)       10 2023-03-10 06:38:19.000000 supergood-1.0.8/src/supergood.egg-info/top_level.txt
-drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-03-10 06:38:19.558604 supergood-1.0.8/tests/
--rw-r--r--   0 alexklarfeld   (501) staff       (20)     5660 2023-03-10 05:29:59.000000 supergood-1.0.8/tests/test_core.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      876 2023-03-10 06:07:05.000000 supergood-1.0.8/tests/test_hashing_entire_body.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)        0 2023-03-10 06:00:41.000000 supergood-1.0.8/tests/test_hashing_keys.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      932 2023-03-10 06:08:37.000000 supergood-1.0.8/tests/test_hashing_single_key.py
--rw-r--r--   0 alexklarfeld   (501) staff       (20)      833 2023-03-10 06:12:40.000000 supergood-1.0.8/tests/test_ignored_domains.py
+drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-04-19 17:36:11.603759 supergood-1.0.9/
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     4714 2023-03-03 05:10:33.000000 supergood-1.0.9/LICENSE
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     1088 2023-04-19 17:36:11.603826 supergood-1.0.9/PKG-INFO
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      719 2023-03-02 17:21:43.000000 supergood-1.0.9/README.md
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      153 2023-04-19 17:36:11.604059 supergood-1.0.9/setup.cfg
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     1121 2023-04-19 17:33:56.000000 supergood-1.0.9/setup.py
+drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-04-19 17:36:11.598002 supergood-1.0.9/src/
+drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-04-19 17:36:11.600407 supergood-1.0.9/src/supergood/
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)       49 2023-03-02 23:55:20.000000 supergood-1.0.9/src/supergood/__init__.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     1346 2023-04-19 04:12:03.000000 supergood-1.0.9/src/supergood/api.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     7337 2023-04-19 17:28:26.000000 supergood-1.0.9/src/supergood/client.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     1230 2023-04-19 04:09:55.000000 supergood-1.0.9/src/supergood/constants.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     2148 2023-04-19 17:28:45.000000 supergood-1.0.9/src/supergood/helpers.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      725 2023-03-02 17:21:43.000000 supergood-1.0.9/src/supergood/logger.py
+drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-04-19 17:36:11.602273 supergood-1.0.9/src/supergood/vendors/
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)        0 2023-03-08 02:17:36.000000 supergood-1.0.9/src/supergood/vendors/__init__.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     1305 2023-03-08 21:06:35.000000 supergood-1.0.9/src/supergood/vendors/aiohttp.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     2081 2023-03-09 05:01:39.000000 supergood-1.0.9/src/supergood/vendors/http.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      446 2023-03-08 04:24:53.000000 supergood-1.0.9/src/supergood/vendors/requests.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     1063 2023-03-08 20:27:52.000000 supergood-1.0.9/src/supergood/vendors/urllib3.py
+drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-04-19 17:36:11.601112 supergood-1.0.9/src/supergood.egg-info/
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     1088 2023-04-19 17:36:11.000000 supergood-1.0.9/src/supergood.egg-info/PKG-INFO
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      647 2023-04-19 17:36:11.000000 supergood-1.0.9/src/supergood.egg-info/SOURCES.txt
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)        1 2023-04-19 17:36:11.000000 supergood-1.0.9/src/supergood.egg-info/dependency_links.txt
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      242 2023-04-19 17:36:11.000000 supergood-1.0.9/src/supergood.egg-info/requires.txt
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)       10 2023-04-19 17:36:11.000000 supergood-1.0.9/src/supergood.egg-info/top_level.txt
+drwxr-xr-x   0 alexklarfeld   (501) staff       (20)        0 2023-04-19 17:36:11.603514 supergood-1.0.9/tests/
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)     4898 2023-04-19 16:08:18.000000 supergood-1.0.9/tests/test_core.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      876 2023-03-10 06:07:05.000000 supergood-1.0.9/tests/test_hashing_entire_body.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      932 2023-04-19 17:25:26.000000 supergood-1.0.9/tests/test_hashing_single_key.py
+-rw-r--r--   0 alexklarfeld   (501) staff       (20)      833 2023-03-10 06:12:40.000000 supergood-1.0.9/tests/test_ignored_domains.py
```

### Comparing `supergood-1.0.8/LICENSE` & `supergood-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/PKG-INFO` & `supergood-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: supergood
-Version: 1.0.8
-Summary: A Python client for Supergood
+Version: 1.0.9
+Summary: The Python client for Supergood
 Author: Alex Klarfeld
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # Supergood Python Client
 
 Monitor the usage, spend and performance of your external API's in 5 minutes flat.
 
 1. Sign-up for an account on supergood.ai
```

### Comparing `supergood-1.0.8/README.md` & `supergood-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/setup.py` & `supergood-1.0.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='supergood',
-    version='1.0.8',
+    version='1.0.9',
     author='Alex Klarfeld',
-    description='A Python client for Supergood',
+    description='The Python client for Supergood',
     long_description=long_description,
     long_description_content_type='text/markdown',
     package=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     py_modules=['supergood'],
     package_dir={'': 'src'},
     install_requires=[
-        'pydash',
-        'python-dotenv',
+        'python-dotenv==1.0.0',
         'jsonpickle',
+        'urllib3==1.26.9',
+        'requests==2.28.0',
+        'aiohttp==3.8.4',
+        'pydash==7.0.1',
     ],
-    tests_require=[
-        'aiohttp',
-        'pydash',
-        'pytest',
-        'pytest_httpserver',
-        'python-dotenv',
-        'Werkzeug',
-        'jsonpickle'
-    ],
+    extras_require={
+        'test': [
+            'requests==2.28.0',
+            'urllib3==1.26.9',
+            'pytest==7.2.1',
+            'pytest_httpserver==1.0.6',
+            'python-dotenv==1.0.0',
+            'Werkzeug',
+            'jsonpickle==3.0.1',
+            'pytest-mock==3.10.0'
+        ]
+    },
 )
```

### Comparing `supergood-1.0.8/src/supergood/api.py` & `supergood-1.0.9/src/supergood/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import requests
 
 from .constants import *
 from urllib.parse import urljoin
 
 class Api(object):
-    def __init__(self, header_options, base_url=DEFAULT_SUPERGOOD_BASE_URL, config=None):
+    def __init__(self, header_options, base_url=DEFAULT_SUPERGOOD_BASE_URL):
         self.base_url = base_url
         self.header_options = header_options
-        self.config_fetch_url = urljoin(self.base_url, 'api/config')
-        self.config = config
 
     def set_logger(self, logger):
         self.log = logger
 
     def set_event_sink_url(self, endpoint):
         self.event_sink_url = urljoin(self.base_url, endpoint)
 
@@ -35,18 +33,7 @@
         }
         try:
             response = requests.post(self.error_sink_url, json=json, headers=self.header_options)
             return response.status_code
         except Exception as e:
             self.log.warning(f'Failed to report error to {self.error_sink_url}')
 
-    def fetch_config(self):
-        if(self.config):
-            return self.config
-        else:
-            response = requests.get(self.config_fetch_url, headers=self.header_options)
-            if(response.status_code == 401):
-                raise Exception(ERRORS['UNAUTHORIZED'])
-            if(response.status_code != 200):
-                raise Exception(ERRORS['FETCHING_CONFIG'])
-            return response.json()
-
```

### Comparing `supergood-1.0.8/src/supergood/client.py` & `supergood-1.0.9/src/supergood/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,27 +30,28 @@
 
 class Client(object):
 
     def __init__(self,
         client_id=os.getenv('SUPERGOOD_CLIENT_ID'),
         client_secret_id=os.getenv('SUPERGOOD_CLIENT_SECRET'),
         base_url=os.getenv('SUPERGOOD_BASE_URL'),
-        config=None
+        config={}
     ):
         self.base_url = base_url if base_url else DEFAULT_SUPERGOOD_BASE_URL
 
         authorization = f'{client_id}:{client_secret_id}'
+
         header_options = {
                 'Accept' : 'application/json, text/plain, */*',
                 'Content-Type' : 'application/json',
                 'Authorization' : 'Basic ' + b64encode(bytes(authorization, 'utf-8')).decode('utf-8')
             }
-
-        self.api = Api(header_options, base_url=self.base_url, config=config)
-        self.config = self.api.fetch_config()
+        self.config = DEFAULT_SUPERGOOD_CONFIG
+        self.config.update(config)
+        self.api = Api(header_options, base_url=self.base_url)
         self.log = Logger(self.__class__.__name__, self.config, self.api)
 
         self.api.set_logger(self.log)
         self.api.set_event_sink_url(self.config['eventSinkEndpoint'])
         self.api.set_error_sink_url(self.config['errorSinkEndpoint'])
 
         # Initialize patches here
@@ -69,15 +70,15 @@
     def set_interval(self, func, sec):
         def func_wrapper():
             self.set_interval(func, sec)
             func()
         t = threading.Timer(sec, func_wrapper)
 
         # Function will exit and end when script ends
-        t.setDaemon(True)
+        t.daemon = True
         t.start()
         return t
 
     def _cache_request(self, request_id, url, method, body, headers):
         host_domain = urlparse(url).hostname
         supergood_base_url = urlparse(self.base_url).hostname
         now = datetime.now().isoformat()
@@ -107,18 +108,14 @@
                         'request': jsonpickle.encode(request, unpicklable=False),
                         'config': jsonpickle.encode(self.config , unpicklable=False)
                     },
                     error_string,
                     ERRORS['CACHING_REQUEST']
                 )
 
-
-    # Note for morning Alex
-    # Need response_body, response_headers, response_status and response_status_text as
-    # arguments to be able to patch aiohttp in a similar fashion to the others
     def _cache_response(
         self,
         request_id,
         response_body,
         response_headers,
         response_status,
         response_status_text
```

### Comparing `supergood-1.0.8/src/supergood/constants.py` & `supergood-1.0.9/src/supergood/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 ]
 REQUEST_ID_KEY = '_supergood_request_id'
 GZIP_START_BYTES = b'\x1f\x8b'
 DEFAULT_SUPERGOOD_BYTE_LIMIT = 500000
 DEFAULT_SUPERGOOD_CONFIG_URL = 'https://dashboard.supergood.ai/api/config/'
 DEFAULT_SUPERGOOD_BASE_URL = 'https://dashboard.supergood.ai/'
 DEFAULT_SUPERGOOD_CONFIG = {
-    'flush_interval': 1000,
-    'event_sink_endpoint': DEFAULT_SUPERGOOD_BASE_URL + 'api/events',
-    'error_sink_endpoint': DEFAULT_SUPERGOOD_BASE_URL + 'api/errors',
-    'keys_to_hash': ['request.body', 'response.body'],
-    'ignored_domains': []
+    'flushInterval': 1000,
+    'eventSinkEndpoint': '/api/events',
+    'errorSinkEndpoint': '/api/errors',
+    'keysToHash': ['request.body', 'response.body'],
+    'ignoredDomains': []
 }
 
 ERRORS = {
     "CACHING_RESPONSE": 'Error Caching Response',
     "CACHING_REQUEST": 'Error Caching Request',
     "DUMPING_DATA_TO_DISK": 'Error Dumping Data to Disk',
     "POSTING_EVENTS": 'Error Posting Events',
```

### Comparing `supergood-1.0.8/src/supergood/helpers.py` & `supergood-1.0.9/src/supergood/helpers.py`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/src/supergood/logger.py` & `supergood-1.0.9/src/supergood/logger.py`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/src/supergood/vendors/aiohttp.py` & `supergood-1.0.9/src/supergood/vendors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/src/supergood/vendors/http.py` & `supergood-1.0.9/src/supergood/vendors/http.py`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/src/supergood/vendors/urllib3.py` & `supergood-1.0.9/src/supergood/vendors/urllib3.py`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/src/supergood.egg-info/PKG-INFO` & `supergood-1.0.9/src/supergood.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: supergood
-Version: 1.0.8
-Summary: A Python client for Supergood
+Version: 1.0.9
+Summary: The Python client for Supergood
 Author: Alex Klarfeld
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # Supergood Python Client
 
 Monitor the usage, spend and performance of your external API's in 5 minutes flat.
 
 1. Sign-up for an account on supergood.ai
```

### Comparing `supergood-1.0.8/src/supergood.egg-info/SOURCES.txt` & `supergood-1.0.9/src/supergood.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,10 +16,9 @@
 src/supergood/vendors/__init__.py
 src/supergood/vendors/aiohttp.py
 src/supergood/vendors/http.py
 src/supergood/vendors/requests.py
 src/supergood/vendors/urllib3.py
 tests/test_core.py
 tests/test_hashing_entire_body.py
-tests/test_hashing_keys.py
 tests/test_hashing_single_key.py
 tests/test_ignored_domains.py
```

### Comparing `supergood-1.0.8/tests/test_hashing_entire_body.py` & `supergood-1.0.9/tests/test_hashing_entire_body.py`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/tests/test_hashing_single_key.py` & `supergood-1.0.9/tests/test_hashing_single_key.py`

 * *Files identical despite different names*

### Comparing `supergood-1.0.8/tests/test_ignored_domains.py` & `supergood-1.0.9/tests/test_ignored_domains.py`

 * *Files identical despite different names*

