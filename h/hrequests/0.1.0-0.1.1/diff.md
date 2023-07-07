# Comparing `tmp/hrequests-0.1.0.tar.gz` & `tmp/hrequests-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrequests-0.1.0.tar", max compression
+gzip compressed data, was "hrequests-0.1.1.tar", max compression
```

## Comparing `hrequests-0.1.0.tar` & `hrequests-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,30 @@
--rw-r--r--   0        0        0      285 2023-07-03 07:36:31.836374 hrequests-0.1.0/hrequests/__init__.py
--rw-r--r--   0        0        0      141 2023-07-07 00:12:48.068335 hrequests-0.1.0/hrequests/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.1.0/hrequests/bin/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.1.0/hrequests/bin/LICENSE.txt
--rw-r--r--   0        0        0 16467699 2023-07-07 01:14:06.639624 hrequests-0.1.0/hrequests/bin/tls-client-windows-64-1.4.0.dll
--rw-r--r--   0        0        0    21724 2023-07-07 01:19:31.445394 hrequests-0.1.0/hrequests/browser.py
--rw-r--r--   0        0        0     2769 2023-07-05 18:22:08.213129 hrequests-0.1.0/hrequests/cffi.py
--rw-r--r--   0        0        0    15818 2023-07-05 21:16:15.840628 hrequests-0.1.0/hrequests/client.py
--rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.1.0/hrequests/cookies.py
--rw-r--r--   0        0        0      582 2023-07-07 01:06:44.367224 hrequests-0.1.0/hrequests/exceptions.py
--rw-r--r--   0        0        0    17506 2023-07-03 02:11:52.031572 hrequests-0.1.0/hrequests/parser.py
--rw-r--r--   0        0        0      372 2023-07-02 09:40:33.648986 hrequests-0.1.0/hrequests/playwright_mock/__init__.py
--rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.1.0/hrequests/playwright_mock/context.py
--rw-r--r--   0        0        0    12248 2023-06-17 23:02:26.111656 hrequests-0.1.0/hrequests/playwright_mock/element_handle.py
--rw-r--r--   0        0        0     2107 2023-07-02 10:28:25.470175 hrequests-0.1.0/hrequests/playwright_mock/faker.py
--rw-r--r--   0        0        0    13787 2023-06-17 22:56:39.628341 hrequests-0.1.0/hrequests/playwright_mock/frame.py
--rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.1.0/hrequests/playwright_mock/frame_locator.py
--rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.1.0/hrequests/playwright_mock/js_handle.py
--rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.1.0/hrequests/playwright_mock/locale.json
--rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.1.0/hrequests/playwright_mock/locator.py
--rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.1.0/hrequests/playwright_mock/mouse.py
--rw-r--r--   0        0        0    17401 2023-06-18 03:53:53.973091 hrequests-0.1.0/hrequests/playwright_mock/page.py
--rw-r--r--   0        0        0     1941 2023-06-22 07:41:34.022216 hrequests-0.1.0/hrequests/playwright_mock/playwright_mock.py
--rw-r--r--   0        0        0     3910 2023-06-24 01:37:41.576954 hrequests-0.1.0/hrequests/playwright_mock/proxy_manager.py
--rw-r--r--   0        0        0     1393 2023-07-03 03:46:44.214258 hrequests-0.1.0/hrequests/proxies.py
--rw-r--r--   0        0        0    12333 2023-07-06 00:09:40.164591 hrequests-0.1.0/hrequests/reqs.py
--rw-r--r--   0        0        0     7505 2023-07-06 04:15:41.650723 hrequests-0.1.0/hrequests/response.py
--rw-r--r--   0        0        0     9574 2023-07-05 20:24:19.953466 hrequests-0.1.0/hrequests/session.py
--rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.1.0/LICENSE
--rw-r--r--   0        0        0      947 2023-07-07 01:24:16.346928 hrequests-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    28410 2023-07-07 01:28:58.903362 hrequests-0.1.0/README.md
--rw-r--r--   0        0        0    28846 1970-01-01 00:00:00.000000 hrequests-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      252 2023-07-07 02:29:04.973494 hrequests-0.1.1/hrequests/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-07 02:16:31.456090 hrequests-0.1.1/hrequests/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.1.1/hrequests/bin/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.1.1/hrequests/bin/LICENSE.txt
+-rw-r--r--   0        0        0    21686 2023-07-07 02:34:49.426242 hrequests-0.1.1/hrequests/browser.py
+-rw-r--r--   0        0        0     2769 2023-07-05 18:22:08.213129 hrequests-0.1.1/hrequests/cffi.py
+-rw-r--r--   0        0        0    15818 2023-07-05 21:16:15.840628 hrequests-0.1.1/hrequests/client.py
+-rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.1.1/hrequests/cookies.py
+-rw-r--r--   0        0        0      582 2023-07-07 01:06:44.367224 hrequests-0.1.1/hrequests/exceptions.py
+-rw-r--r--   0        0        0    17506 2023-07-03 02:11:52.031572 hrequests-0.1.1/hrequests/parser.py
+-rw-r--r--   0        0        0      372 2023-07-02 09:40:33.648986 hrequests-0.1.1/hrequests/playwright_mock/__init__.py
+-rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.1.1/hrequests/playwright_mock/context.py
+-rw-r--r--   0        0        0    12248 2023-06-17 23:02:26.111656 hrequests-0.1.1/hrequests/playwright_mock/element_handle.py
+-rw-r--r--   0        0        0     2107 2023-07-02 10:28:25.470175 hrequests-0.1.1/hrequests/playwright_mock/faker.py
+-rw-r--r--   0        0        0    13787 2023-06-17 22:56:39.628341 hrequests-0.1.1/hrequests/playwright_mock/frame.py
+-rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.1.1/hrequests/playwright_mock/frame_locator.py
+-rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.1.1/hrequests/playwright_mock/js_handle.py
+-rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.1.1/hrequests/playwright_mock/locale.json
+-rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.1.1/hrequests/playwright_mock/locator.py
+-rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.1.1/hrequests/playwright_mock/mouse.py
+-rw-r--r--   0        0        0    17401 2023-06-18 03:53:53.973091 hrequests-0.1.1/hrequests/playwright_mock/page.py
+-rw-r--r--   0        0        0     1941 2023-06-22 07:41:34.022216 hrequests-0.1.1/hrequests/playwright_mock/playwright_mock.py
+-rw-r--r--   0        0        0     3910 2023-06-24 01:37:41.576954 hrequests-0.1.1/hrequests/playwright_mock/proxy_manager.py
+-rw-r--r--   0        0        0    12333 2023-07-06 00:09:40.164591 hrequests-0.1.1/hrequests/reqs.py
+-rw-r--r--   0        0        0     7505 2023-07-06 04:15:41.650723 hrequests-0.1.1/hrequests/response.py
+-rw-r--r--   0        0        0     9576 2023-07-07 02:19:53.457218 hrequests-0.1.1/hrequests/session.py
+-rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1016 2023-07-07 02:38:28.544273 hrequests-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    28547 2023-07-07 02:05:53.992487 hrequests-0.1.1/README.md
+-rw-r--r--   0        0        0    29089 1970-01-01 00:00:00.000000 hrequests-0.1.1/PKG-INFO
```

### Comparing `hrequests-0.1.0/hrequests/bin/LICENSE.txt` & `hrequests-0.1.1/hrequests/bin/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/browser.py` & `hrequests-0.1.1/hrequests/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from functools import partial
 from random import choice
 from threading import Thread
 from typing import Any, Callable, Dict, Literal, Optional, Pattern, Union
 
 from aioprocessing import Queue
 from fake_headers import Headers
-from fake_useragent import UserAgent
 from playwright._impl._api_types import Error as PlaywrightError
 from playwright._impl._api_types import TimeoutError as PlaywrightTimeoutError
 
 import hrequests
 from hrequests.client import CaseInsensitiveDict
 from hrequests.cookies import cookiejar_to_list, list_to_cookiejar
 from hrequests.exceptions import BrowserException, BrowserTimeoutException
```

### Comparing `hrequests-0.1.0/hrequests/cffi.py` & `hrequests-0.1.1/hrequests/cffi.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/client.py` & `hrequests-0.1.1/hrequests/client.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/cookies.py` & `hrequests-0.1.1/hrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/exceptions.py` & `hrequests-0.1.1/hrequests/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/parser.py` & `hrequests-0.1.1/hrequests/parser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/context.py` & `hrequests-0.1.1/hrequests/playwright_mock/context.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/element_handle.py` & `hrequests-0.1.1/hrequests/playwright_mock/element_handle.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/faker.py` & `hrequests-0.1.1/hrequests/playwright_mock/faker.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/frame.py` & `hrequests-0.1.1/hrequests/playwright_mock/frame.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/frame_locator.py` & `hrequests-0.1.1/hrequests/playwright_mock/frame_locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/locale.json` & `hrequests-0.1.1/hrequests/playwright_mock/locale.json`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/locator.py` & `hrequests-0.1.1/hrequests/playwright_mock/locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/mouse.py` & `hrequests-0.1.1/hrequests/playwright_mock/mouse.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/page.py` & `hrequests-0.1.1/hrequests/playwright_mock/page.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/playwright_mock.py` & `hrequests-0.1.1/hrequests/playwright_mock/playwright_mock.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/playwright_mock/proxy_manager.py` & `hrequests-0.1.1/hrequests/playwright_mock/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/reqs.py` & `hrequests-0.1.1/hrequests/reqs.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/response.py` & `hrequests-0.1.1/hrequests/response.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/hrequests/session.py` & `hrequests-0.1.1/hrequests/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         cookies: Optional[Union[RequestsCookieJar, dict, list]] = None,
         json: Optional[Union[dict, list, str]] = None,
         allow_redirects: bool = True,
         history: bool = False,
         verify: bool = True,  # maps to insecure_skip_verify
         timeout: int = 30,  # maps to timeout_seconds
         proxies: Optional[dict] = None,
-    ) -> hrequests.response.Response:
+    ) -> 'hrequests.response.Response':
         """
         Send a request with TLS client
 
         Args:
             method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT, PATCH, DELETE)
             url (str): URL to send request to
             params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
```

### Comparing `hrequests-0.1.0/LICENSE` & `hrequests-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hrequests-0.1.0/pyproject.toml` & `hrequests-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hrequests"
-version = "0.1.0"
+version = "0.1.1"
 description = "Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library."
 authors = ["daijro <daijro.dev@gmail.com>"]
 license = "Apache-2.0"
-include = ["hrequests/bin/*"]
 readme = "README.md"
 repository = "https://github.com/daijro/hrequests"
 keywords = ["tls", "client", "http", "scraping", "requests", "humans", "playwright"]
 classifiers = [
 	"Topic :: Internet :: WWW/HTTP",
 	"Topic :: Internet :: WWW/HTTP :: Browsers",
     "Topic :: Software Development :: Libraries :: Python Modules"
@@ -24,10 +23,14 @@
 httpx = "*"
 playwright = "*"
 playwright-stealth = "*"
 wget = "*"
 async-class = "*"
 aioprocessing = "*"
 numpy = "*"
-gevent = "*"
 fake-headers = "*"
-fake-useragent = "*"
+lxml = "*"
+parse = "*"
+pyquery = "*"
+w3lib = "*"
+gevent = "*"
+msvc-runtime = {version = "*", markers = "sys_platform == 'win32'"}
```

### Comparing `hrequests-0.1.0/README.md` & `hrequests-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 <p align="center">
     <a href="https://github.com/daijro/hrequests/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/daijro/hrequests.svg">
     </a>
     <a href="https://python.org/">
         <img src="https://img.shields.io/badge/python-3.6&#8208;3.10-blue">
     </a>
+    <a href="https://pypi.org/project/hrequests/">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/hrequests">
+    </a>
     <a href="https://github.com/ambv/black">
         <img src="https://img.shields.io/badge/code%20style-black-black.svg">
     </a>
     <a href="https://github.com/PyCQA/isort">
-        <img src="https://img.shields.io/badge/imports-isort-red.svg">
+        <img src="https://img.shields.io/badge/imports-isort-yellow.svg">
     </a>
 </p>
     Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 </h4>
 
 - TLS client fingerprinting 🚀
 - Javascript rendering 🚀
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_j0s8p9k3_/tmpk9o5_t82_TarContainer/0/30.md", line 912, column 3: CDATA terminal not found*

 * *File "/tmp/diffoscope_j0s8p9k3_/tmpk9o5_t82_TarContainer/0/30.md", line 912, column 3: CDATA terminal not found*

```diff
@@ -1,14 +1,14 @@
 [https://i.imgur.com/r8GcQW1.png]
                              ***** hrequests *****
   *** [https://img.shields.io/github/license/daijro/hrequests.svg] [https://
-img.shields.io/badge/python-3.6&#8208;3.10-blue] [https://img.shields.io/badge/
-  code%20style-black-black.svg] [https://img.shields.io/badge/imports-isort-
-  red.svg]Hrequests (human requests) is a simple, configurable, feature-rich,
-               replacement for the Python requests library. ***
+       img.shields.io/badge/python-3.6&#8208;3.10-blue] [PyPI] [https://
+  img.shields.io/badge/code%20style-black-black.svg] [https://img.shields.io/
+    badge/imports-isort-yellow.svg]Hrequests (human requests) is a simple,
+ configurable, feature-rich, replacement for the Python requests library. ***
 - TLS client fingerprinting ð - Javascript rendering ð - Human-like
 browsing emulation ð - Fast built-in HTML parsing ð - Asynchronous
 requests with gevent *(without monkey-paching!)* ð - Realistic browser
 header spoofing ð - Supports HTTP/2 ð - High performance ð - 100%
 thread-safe ð --- # Installation Install via pip: ```bash pip install
 hrequests ``` Other depedencies will be downloaded on the first import: ```py
 >>> import hrequests ``` --- # Documentation 1. [Simple Usage](https://
```

### Comparing `hrequests-0.1.0/PKG-INFO` & `hrequests-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrequests
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 Home-page: https://github.com/daijro/hrequests
 License: Apache-2.0
 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro
 Author-email: daijro.dev@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -18,21 +18,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aioprocessing
 Requires-Dist: async-class
 Requires-Dist: fake-headers
-Requires-Dist: fake-useragent
 Requires-Dist: gevent
 Requires-Dist: httpx
+Requires-Dist: lxml
+Requires-Dist: msvc-runtime ; sys_platform == "win32"
 Requires-Dist: numpy
 Requires-Dist: orjson
+Requires-Dist: parse
 Requires-Dist: playwright
 Requires-Dist: playwright-stealth
+Requires-Dist: pyquery
+Requires-Dist: w3lib
 Requires-Dist: wget
 Project-URL: Repository, https://github.com/daijro/hrequests
 Description-Content-Type: text/markdown
 
 <img src="https://i.imgur.com/r8GcQW1.png" align="center">
 </img>
 
@@ -43,19 +47,22 @@
 <p align="center">
     <a href="https://github.com/daijro/hrequests/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/daijro/hrequests.svg">
     </a>
     <a href="https://python.org/">
         <img src="https://img.shields.io/badge/python-3.6&#8208;3.10-blue">
     </a>
+    <a href="https://pypi.org/project/hrequests/">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/hrequests">
+    </a>
     <a href="https://github.com/ambv/black">
         <img src="https://img.shields.io/badge/code%20style-black-black.svg">
     </a>
     <a href="https://github.com/PyCQA/isort">
-        <img src="https://img.shields.io/badge/imports-isort-red.svg">
+        <img src="https://img.shields.io/badge/imports-isort-yellow.svg">
     </a>
 </p>
     Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 </h4>
 
 - TLS client fingerprinting 🚀
 - Javascript rendering 🚀
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_j0s8p9k3_/tmpk9o5_t82_TarContainer/0/31", line 948, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_j0s8p9k3_/tmpk9o5_t82_TarContainer/0/31", line 948, column 0: CDATA terminal not found*

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: hrequests Version: 0.1.0 Summary: Hrequests (human
+Metadata-Version: 2.1 Name: hrequests Version: 0.1.1 Summary: Hrequests (human
 requests) is a simple, configurable, feature-rich, replacement for the Python
 requests library. Home-page: https://github.com/daijro/hrequests License:
 Apache-2.0 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Internet :: WWW/
 HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Browsers Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Requires-Dist:
 aioprocessing Requires-Dist: async-class Requires-Dist: fake-headers Requires-
-Dist: fake-useragent Requires-Dist: gevent Requires-Dist: httpx Requires-Dist:
-numpy Requires-Dist: orjson Requires-Dist: playwright Requires-Dist:
-playwright-stealth Requires-Dist: wget Project-URL: Repository, https://
-github.com/daijro/hrequests Description-Content-Type: text/markdown [https://
-i.imgur.com/r8GcQW1.png]
+Dist: gevent Requires-Dist: httpx Requires-Dist: lxml Requires-Dist: msvc-
+runtime ; sys_platform == "win32" Requires-Dist: numpy Requires-Dist: orjson
+Requires-Dist: parse Requires-Dist: playwright Requires-Dist: playwright-
+stealth Requires-Dist: pyquery Requires-Dist: w3lib Requires-Dist: wget
+Project-URL: Repository, https://github.com/daijro/hrequests Description-
+Content-Type: text/markdown [https://i.imgur.com/r8GcQW1.png]
                              ***** hrequests *****
   *** [https://img.shields.io/github/license/daijro/hrequests.svg] [https://
-img.shields.io/badge/python-3.6&#8208;3.10-blue] [https://img.shields.io/badge/
-  code%20style-black-black.svg] [https://img.shields.io/badge/imports-isort-
-  red.svg]Hrequests (human requests) is a simple, configurable, feature-rich,
-               replacement for the Python requests library. ***
+       img.shields.io/badge/python-3.6&#8208;3.10-blue] [PyPI] [https://
+  img.shields.io/badge/code%20style-black-black.svg] [https://img.shields.io/
+    badge/imports-isort-yellow.svg]Hrequests (human requests) is a simple,
+ configurable, feature-rich, replacement for the Python requests library. ***
 - TLS client fingerprinting ð - Javascript rendering ð - Human-like
 browsing emulation ð - Fast built-in HTML parsing ð - Asynchronous
 requests with gevent *(without monkey-paching!)* ð - Realistic browser
 header spoofing ð - Supports HTTP/2 ð - High performance ð - 100%
 thread-safe ð --- # Installation Install via pip: ```bash pip install
 hrequests ``` Other depedencies will be downloaded on the first import: ```py
 >>> import hrequests ``` --- # Documentation 1. [Simple Usage](https://
```

