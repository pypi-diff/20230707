# Comparing `tmp/hspylib-cfman-0.9.94.tar.gz` & `tmp/hspylib-cfman-0.9.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-cfman-0.9.94.tar", last modified: Tue Jul  4 18:59:46 2023, max compression
+gzip compressed data, was "hspylib-cfman-0.9.95.tar", last modified: Thu Jul  6 22:54:58 2023, max compression
```

## Comparing `hspylib-cfman-0.9.94.tar` & `hspylib-cfman-0.9.95.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-04 18:59:46.946286 hspylib-cfman-0.9.94/
--rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.94/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-04 18:59:46.945418 hspylib-cfman-0.9.94/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-07-04 18:59:45.000000 hspylib-cfman-0.9.94/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-04 18:59:46.917992 hspylib-cfman-0.9.94/cfman/
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-04 18:59:45.000000 hspylib-cfman-0.9.94/cfman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.94/cfman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-04 18:59:45.000000 hspylib-cfman-0.9.94/cfman/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3471 2023-07-03 20:34:17.000000 hspylib-cfman-0.9.94/cfman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-04 18:59:46.931152 hspylib-cfman-0.9.94/cfman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-07-04 18:59:45.000000 hspylib-cfman-0.9.94/cfman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7745 2023-07-03 20:34:17.000000 hspylib-cfman-0.9.94/cfman/core/cf.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2950 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.94/cfman/core/cf_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5534 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.94/cfman/core/cf_blue_green_checker.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.94/cfman/core/cf_endpoint.py
--rw-r--r--   0 hjunior    (504) staff       (20)    16927 2023-07-03 20:34:17.000000 hspylib-cfman-0.9.94/cfman/core/cf_manager.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-04 18:59:46.936340 hspylib-cfman-0.9.94/cfman/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-04 18:59:45.000000 hspylib-cfman-0.9.94/cfman/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.94/cfman/exception/exceptions.py
--rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.94/cfman/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-04 18:59:46.944275 hspylib-cfman-0.9.94/hspylib_cfman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-04 18:59:46.000000 hspylib-cfman-0.9.94/hspylib_cfman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-07-04 18:59:46.000000 hspylib-cfman-0.9.94/hspylib_cfman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-04 18:59:46.000000 hspylib-cfman-0.9.94/hspylib_cfman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-07-04 18:59:46.000000 hspylib-cfman-0.9.94/hspylib_cfman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-04 18:59:46.000000 hspylib-cfman-0.9.94/hspylib_cfman.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-04 18:59:46.946417 hspylib-cfman-0.9.94/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.94/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:58.004242 hspylib-cfman-0.9.95/
+-rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.95/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-06 22:54:58.001657 hspylib-cfman-0.9.95/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:57.954708 hspylib-cfman-0.9.95/cfman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/cfman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      716 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.95/cfman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/cfman/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3471 2023-07-03 20:34:17.000000 hspylib-cfman-0.9.95/cfman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:57.977035 hspylib-cfman-0.9.95/cfman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/cfman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7681 2023-07-06 22:15:35.000000 hspylib-cfman-0.9.95/cfman/core/cf.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2950 2023-05-17 21:37:29.000000 hspylib-cfman-0.9.95/cfman/core/cf_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5534 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.95/cfman/core/cf_blue_green_checker.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1234 2023-04-19 22:17:47.000000 hspylib-cfman-0.9.95/cfman/core/cf_endpoint.py
+-rw-r--r--   0 hjunior    (504) staff       (20)    16913 2023-07-06 22:14:26.000000 hspylib-cfman-0.9.95/cfman/core/cf_manager.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:57.985170 hspylib-cfman-0.9.95/cfman/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/cfman/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-19 22:01:52.000000 hspylib-cfman-0.9.95/cfman/exception/exceptions.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.95/cfman/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:54:57.999327 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 22:54:57.000000 hspylib-cfman-0.9.95/hspylib_cfman.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 22:54:58.004436 hspylib-cfman-0.9.95/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1934 2023-04-19 22:13:46.000000 hspylib-cfman-0.9.95/setup.py
```

### Comparing `hspylib-cfman-0.9.94/PKG-INFO` & `hspylib-cfman-0.9.95/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.94
+Version: 0.9.95
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
-[![Release](https://badgen.net/badge/release/v0.9.94/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.95/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.94/README.md` & `hspylib-cfman-0.9.95/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - CloudFoundry manager
 
 ## Manage your PCF applications
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.94/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.95/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.94/cfman/__classpath__.py` & `hspylib-cfman-0.9.95/cfman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.94/cfman/__main__.py` & `hspylib-cfman-0.9.95/cfman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.94/cfman/core/cf.py` & `hspylib-cfman-0.9.95/cfman/core/cf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
    Copyright 2023, HsPyLib team
 """
 from collections import namedtuple
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.commons import sysout
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.cli.terminal import Terminal
-from hspylib.modules.cli.vt100.vt_utils import clear_screen, set_auto_wrap
 from typing import List, Optional
 
 import os
 
 CFTarget = namedtuple("CFTarget", ["user", "org", "space", "connected"])
 
 
@@ -182,16 +181,16 @@
     def logs(self, **kwargs) -> None:
         """Tail or show recent logs for an app
         Kwargs:
             app (str): the application name.
                recent: dump recent logs instead of tailing.
         :param kwargs arbitrary CF command keyword arguments.
         """
-        clear_screen()
-        set_auto_wrap(True)
+        Terminal.clear()
+        Terminal.set_auto_wrap(True)
         return self._exec(cmd_line=f"logs {kwargs['app']} {'--recent' if 'recent' in kwargs else ''}", poll=True)
 
     # Execution of a CF command
     def _exec(self, cmd_line: str, poll: bool = False) -> Optional[str]:
         """Execute the CF command.
         :param cmd_line: the cf command line string
         :param poll: whether to poll or execute the command. If poll is set I/O events can be registered for any number
```

### Comparing `hspylib-cfman-0.9.94/cfman/core/cf_application.py` & `hspylib-cfman-0.9.95/cfman/core/cf_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.94/cfman/core/cf_blue_green_checker.py` & `hspylib-cfman-0.9.95/cfman/core/cf_blue_green_checker.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.94/cfman/core/cf_endpoint.py` & `hspylib-cfman-0.9.95/cfman/core/cf_endpoint.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.94/cfman/core/cf_manager.py` & `hspylib-cfman-0.9.95/cfman/core/cf_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,30 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
+from hspylib.modules.cli.terminal import Terminal
+
 from cfman.core.cf import CloudFoundry
 from cfman.core.cf_application import CFApplication
 from cfman.core.cf_blue_green_checker import CFBlueGreenChecker
 from cfman.core.cf_endpoint import CFEndpoint
 from cfman.exception.exceptions import CFAuthenticationError, CFConnectionError, CFExecutionError
 from clitt.core.tui.mchoose.mchoose import mchoose
 from clitt.core.tui.minput.minput import MenuInput, minput
 from clitt.core.tui.mselect.mselect import mselect
 from clitt.core.tui.tui_screen import TUIScreen
 from functools import partial
 from hspylib.core.enums.http_code import HttpCode
 from hspylib.core.preconditions import check_state
 from hspylib.modules.cache.ttl_cache import TTLCache
 from hspylib.modules.cli.keyboard import Keyboard
-from hspylib.modules.cli.vt100.vt_utils import clear_screen, set_auto_wrap, set_show_cursor
 from hspylib.modules.fetch.fetch import head
 from retry import retry
 from time import sleep
 from typing import Any, List, Optional, Tuple
 
 import requests
 import sys
@@ -168,17 +169,17 @@
         self._wait_keystroke()
         self._loop_actions()
         self.screen.clear()
         self.cursor.home()
 
     def _prepare_render(self) -> None:
         """Prepare the screen for renderization."""
-        set_auto_wrap(False)
-        set_show_cursor(False)
-        self._screen.clear()
+        Terminal.set_auto_wrap(False)
+        Terminal.set_show_cursor(False)
+        self.screen.clear()
         self.cursor.save()
 
     def _wait_keystroke(self, wait_message: str = "%YELLOW%%EOL%Press any key to continue%EOL%%NC%") -> None:
         """Wait for a keypress (blocking).
         :param wait_message: the message to present to the user.
         """
         self.writeln(wait_message)
@@ -368,29 +369,29 @@
         return not self._done
 
     def _display_app_status(self) -> None:
         """Display all PCF space-application statuses."""
         apps = self.apps
 
         if len(apps) > 0:
-            clear_screen()
+            self.screen.clear()
             # fmt: off
             self.writeln(
                 f"%BLUE%Listing '{self._org}::{self._space}' applications ...%EOL%%WHITE%"
                 f"{'-=' * 60 + '%EOL%'}"
                 f"{'Name':{CFApplication.max_name_length + 2}}"
                 f"{'State':<9}{'Instances':<12}{'Mem':<6}{'Disk':<6}Routes%EOL%")
             # fmt: on
             list(map(CFApplication.print_status, apps))
             self.writeln("-=" * 60 + "%EOL%")
 
     def _blue_green_check(self) -> None:
         """Display all PCF space-application blue/green check."""
         if len(self.apps) > 0:
-            clear_screen()
+            self.screen.clear()
             self.writeln(f"%BLUE%Checking blue/green deployments ...%EOL%")
             CFBlueGreenChecker.check(self._org, self._space, self.apps)
 
     def _perform_callable(self, action: str) -> None:
         """Wrapper of the _perform method.
         :param action the action to perform.
         """
```

### Comparing `hspylib-cfman-0.9.94/cfman/exception/exceptions.py` & `hspylib-cfman-0.9.95/cfman/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.94/hspylib_cfman.egg-info/PKG-INFO` & `hspylib-cfman-0.9.95/hspylib_cfman.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-cfman
-Version: 0.9.94
+Version: 0.9.95
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
-[![Release](https://badgen.net/badge/release/v0.9.94/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.95/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-cfman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-cfman-0.9.94/hspylib_cfman.egg-info/SOURCES.txt` & `hspylib-cfman-0.9.95/hspylib_cfman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-cfman-0.9.94/setup.py` & `hspylib-cfman-0.9.95/setup.py`

 * *Files identical despite different names*

