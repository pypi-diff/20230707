# Comparing `tmp/hspylib-cfman-0.9.95.tar.gz` & `tmp/hspylib-cfman-0.9.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-cfman-0.9.95.tar", last modified: Thu Jul  6 22:54:58 2023, max compression
+gzip compressed data, was "hspylib-cfman-0.9.96.tar", last modified: Thu Jul  6 23:48:47 2023, max compression
```

## Comparing `hspylib-cfman-0.9.95.tar` & `hspylib-cfman-0.9.96.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:58.004242 hspylib-cfman-0.9.95/
--rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.95/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-06 22:54:58.001657 hspylib-cfman-0.9.95/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:57.954708 hspylib-cfman-0.9.95/cfman/
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/cfman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.95/cfman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/cfman/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3471 2023-07-03 20:34:17.000000 hspylib-cfman-0.9.95/cfman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:57.977035 hspylib-cfman-0.9.95/cfman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/cfman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7681 2023-07-06 22:15:35.000000 hspylib-cfman-0.9.95/cfman/core/cf.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2950 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.95/cfman/core/cf_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5534 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.95/cfman/core/cf_blue_green_checker.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.95/cfman/core/cf_endpoint.py
--rw-r--r--   0 hjunior    (504) staff       (20)    16913 2023-07-06 22:14:26.000000 hspylib-cfman-0.9.95/cfman/core/cf_manager.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:57.985170 hspylib-cfman-0.9.95/cfman/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/cfman/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.95/cfman/exception/exceptions.py
--rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.95/cfman/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:57.999327 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 22:54:58.004436 hspylib-cfman-0.9.95/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.95/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.110125 hspylib-cfman-0.9.96/
+-rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.96/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-06 23:48:47.108317 hspylib-cfman-0.9.96/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.067566 hspylib-cfman-0.9.96/cfman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/cfman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.96/cfman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/cfman/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3471 2023-07-03 20:34:17.000000 hspylib-cfman-0.9.96/cfman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.080578 hspylib-cfman-0.9.96/cfman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/cfman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7673 2023-07-06 23:47:54.000000 hspylib-cfman-0.9.96/cfman/core/cf.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2950 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.96/cfman/core/cf_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5534 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.96/cfman/core/cf_blue_green_checker.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.96/cfman/core/cf_endpoint.py
+-rw-r--r--   0 hjunior    (504) staff       (20)    16904 2023-07-06 23:47:31.000000 hspylib-cfman-0.9.96/cfman/core/cf_manager.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.087190 hspylib-cfman-0.9.96/cfman/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/cfman/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.96/cfman/exception/exceptions.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.96/cfman/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 23:48:47.106190 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 23:48:46.000000 hspylib-cfman-0.9.96/hspylib_cfman.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 23:48:47.110328 hspylib-cfman-0.9.96/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.96/setup.py
```

### Comparing `hspylib-cfman-0.9.95/PKG-INFO` & `hspylib-cfman-0.9.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.95
+Version: 0.9.96
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
-[![Release](https://badgen.net/badge/release/v0.9.95/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.95/cfman/__classpath__.py` & `hspylib-cfman-0.9.96/cfman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.95/cfman/__main__.py` & `hspylib-cfman-0.9.96/cfman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.95/cfman/core/cf.py` & `hspylib-cfman-0.9.96/cfman/core/cf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
 from collections import namedtuple
+
+from clitt.core.terminal import Terminal
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.commons import sysout
 from hspylib.modules.application.exit_status import ExitStatus
-from hspylib.modules.cli.terminal import Terminal
 from typing import List, Optional
 
 import os
 
 CFTarget = namedtuple("CFTarget", ["user", "org", "space", "connected"])
```

### Comparing `hspylib-cfman-0.9.95/cfman/core/cf_application.py` & `hspylib-cfman-0.9.96/cfman/core/cf_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.95/cfman/core/cf_blue_green_checker.py` & `hspylib-cfman-0.9.96/cfman/core/cf_blue_green_checker.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.95/cfman/core/cf_endpoint.py` & `hspylib-cfman-0.9.96/cfman/core/cf_endpoint.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.95/cfman/core/cf_manager.py` & `hspylib-cfman-0.9.96/cfman/core/cf_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
-from hspylib.modules.cli.terminal import Terminal
+from clitt.core.terminal import Terminal
 
 from cfman.core.cf import CloudFoundry
 from cfman.core.cf_application import CFApplication
 from cfman.core.cf_blue_green_checker import CFBlueGreenChecker
 from cfman.core.cf_endpoint import CFEndpoint
 from cfman.exception.exceptions import CFAuthenticationError, CFConnectionError, CFExecutionError
 from clitt.core.tui.mchoose.mchoose import mchoose
```

### Comparing `hspylib-cfman-0.9.95/cfman/exception/exceptions.py` & `hspylib-cfman-0.9.96/cfman/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.95/hspylib_cfman.egg-info/PKG-INFO` & `hspylib-cfman-0.9.96/hspylib_cfman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.95
+Version: 0.9.96
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
-[![Release](https://badgen.net/badge/release/v0.9.95/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.95/hspylib_cfman.egg-info/SOURCES.txt` & `hspylib-cfman-0.9.96/hspylib_cfman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.95/setup.py` & `hspylib-cfman-0.9.96/setup.py`

 * *Files identical despite different names*

