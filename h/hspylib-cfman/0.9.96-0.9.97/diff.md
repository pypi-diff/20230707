# Comparing `tmp/hspylib-cfman-0.9.96.tar.gz` & `tmp/hspylib-cfman-0.9.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-cfman-0.9.96.tar", last modified: Thu Jul  6 23:48:47 2023, max compression
+gzip compressed data, was "hspylib-cfman-0.9.97.tar", last modified: Fri Jul  7 01:48:25 2023, max compression
```

## Comparing `hspylib-cfman-0.9.96.tar` & `hspylib-cfman-0.9.97.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.110125 hspylib-cfman-0.9.96/
--rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.96/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-06 23:48:47.108317 hspylib-cfman-0.9.96/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.067566 hspylib-cfman-0.9.96/cfman/
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/cfman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.96/cfman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/cfman/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3471 2023-07-03 20:34:17.000000 hspylib-cfman-0.9.96/cfman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.080578 hspylib-cfman-0.9.96/cfman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/cfman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7673 2023-07-06 23:47:54.000000 hspylib-cfman-0.9.96/cfman/core/cf.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2950 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.96/cfman/core/cf_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5534 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.96/cfman/core/cf_blue_green_checker.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.96/cfman/core/cf_endpoint.py
--rw-r--r--   0 hjunior    (504) staff       (20)    16904 2023-07-06 23:47:31.000000 hspylib-cfman-0.9.96/cfman/core/cf_manager.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.087190 hspylib-cfman-0.9.96/cfman/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/cfman/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.96/cfman/exception/exceptions.py
--rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.96/cfman/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.106190 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 23:48:47.110328 hspylib-cfman-0.9.96/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.96/setup.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.272868 hspylib-cfman-0.9.97/
+-rw-r--r--   0 hugo       (503) staff       (20)       49 2022-03-03 17:56:13.000000 hspylib-cfman-0.9.97/MANIFEST.in
+-rw-r--r--   0 hugo       (503) staff       (20)     1548 2023-07-07 01:48:25.272531 hspylib-cfman-0.9.97/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)      677 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/README.md
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.267105 hspylib-cfman-0.9.97/cfman/
+-rw-r--r--   0 hugo       (503) staff       (20)        7 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/cfman/.version
+-rw-r--r--   0 hugo       (503) staff       (20)      716 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/cfman/__classpath__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      167 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/cfman/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3471 2023-07-04 00:05:40.000000 hspylib-cfman-0.9.97/cfman/__main__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.269539 hspylib-cfman-0.9.97/cfman/core/
+-rw-r--r--   0 hugo       (503) staff       (20)      238 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/cfman/core/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7673 2023-07-07 00:12:05.000000 hspylib-cfman-0.9.97/cfman/core/cf.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2950 2023-06-07 00:17:15.000000 hspylib-cfman-0.9.97/cfman/core/cf_application.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5534 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/cfman/core/cf_blue_green_checker.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1234 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/cfman/core/cf_endpoint.py
+-rw-r--r--   0 hugo       (503) staff       (20)    16919 2023-07-07 01:48:06.000000 hspylib-cfman-0.9.97/cfman/core/cf_manager.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.270272 hspylib-cfman-0.9.97/cfman/exception/
+-rw-r--r--   0 hugo       (503) staff       (20)      167 2023-07-07 01:48:24.000000 hspylib-cfman-0.9.97/cfman/exception/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      845 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/cfman/exception/exceptions.py
+-rw-r--r--   0 hugo       (503) staff       (20)      204 2022-03-03 17:56:13.000000 hspylib-cfman-0.9.97/cfman/welcome.txt
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2023-07-07 01:48:25.272032 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/
+-rw-r--r--   0 hugo       (503) staff       (20)     1548 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)      520 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        1 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       28 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/requires.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        6 2023-07-07 01:48:25.000000 hspylib-cfman-0.9.97/hspylib_cfman.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       38 2023-07-07 01:48:25.272958 hspylib-cfman-0.9.97/setup.cfg
+-rw-r--r--   0 hugo       (503) staff       (20)     1934 2023-04-21 00:22:30.000000 hspylib-cfman-0.9.97/setup.py
```

### Comparing `hspylib-cfman-0.9.96/PKG-INFO` & `hspylib-cfman-0.9.97/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.96
+Version: 0.9.97
 Summary: HsPyLib - CloudFoundry manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-cfman/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.96/cfman/__classpath__.py` & `hspylib-cfman-0.9.97/cfman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.96/cfman/__main__.py` & `hspylib-cfman-0.9.97/cfman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.96/cfman/core/cf.py` & `hspylib-cfman-0.9.97/cfman/core/cf.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.96/cfman/core/cf_application.py` & `hspylib-cfman-0.9.97/cfman/core/cf_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.96/cfman/core/cf_blue_green_checker.py` & `hspylib-cfman-0.9.97/cfman/core/cf_blue_green_checker.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.96/cfman/core/cf_endpoint.py` & `hspylib-cfman-0.9.97/cfman/core/cf_endpoint.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.96/cfman/core/cf_manager.py` & `hspylib-cfman-0.9.97/cfman/core/cf_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,25 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
 from clitt.core.terminal import Terminal
+from clitt.core.tty.cursor import Cursor
+from clitt.core.tty.screen import Screen
 
 from cfman.core.cf import CloudFoundry
 from cfman.core.cf_application import CFApplication
 from cfman.core.cf_blue_green_checker import CFBlueGreenChecker
 from cfman.core.cf_endpoint import CFEndpoint
 from cfman.exception.exceptions import CFAuthenticationError, CFConnectionError, CFExecutionError
 from clitt.core.tui.mchoose.mchoose import mchoose
 from clitt.core.tui.minput.minput import MenuInput, minput
 from clitt.core.tui.mselect.mselect import mselect
-from clitt.core.tui.tui_screen import TUIScreen
 from functools import partial
 from hspylib.core.enums.http_code import HttpCode
 from hspylib.core.preconditions import check_state
 from hspylib.modules.cache.ttl_cache import TTLCache
 from hspylib.modules.cli.keyboard import Keyboard
 from hspylib.modules.fetch.fetch import head
 from retry import retry
@@ -81,15 +82,15 @@
                 return "stopped"
             case "logs" | "stop" | "restart":
                 return "started"
             case _:
                 return "started", "stopped"
 
     def __init__(self, api: str, org: str, space: str, username: str, password: str, no_cache: str, cf_endpoints: str):
-        self._screen = TUIScreen.INSTANCE or TUIScreen()
+        self._screen = Screen.INSTANCE or Screen()
         self._cf = CloudFoundry.INSTANCE or CloudFoundry()
         self._cache = TTLCache()
         self._api = api
         self._org = org
         self._space = space
         self._username = username
         self._password = password
@@ -114,19 +115,19 @@
         return str(self)
 
     @property
     def apps(self) -> List[CFApplication]:
         return self._get_apps() or []
 
     @property
-    def screen(self) -> TUIScreen:
+    def screen(self) -> Screen:
         return self._screen
 
     @property
-    def cursor(self) -> TUIScreen.Cursor:
+    def cursor(self) -> Cursor:
         return self.screen.cursor
 
     def write(self, obj: Any) -> None:
         """Write the string representation of the object to the screen."""
         self.cursor.write(obj)
 
     def writeln(self, obj: Any) -> None:
```

### Comparing `hspylib-cfman-0.9.96/cfman/exception/exceptions.py` & `hspylib-cfman-0.9.97/cfman/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.96/hspylib_cfman.egg-info/PKG-INFO` & `hspylib-cfman-0.9.97/hspylib_cfman.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.96
+Version: 0.9.97
 Summary: HsPyLib - CloudFoundry manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-cfman/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.96/hspylib_cfman.egg-info/SOURCES.txt` & `hspylib-cfman-0.9.97/hspylib_cfman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.96/setup.py` & `hspylib-cfman-0.9.97/setup.py`

 * *Files identical despite different names*

