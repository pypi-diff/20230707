# Comparing `tmp/hspylib-setman-0.9.7.tar.gz` & `tmp/hspylib-setman-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-setman-0.9.7.tar", last modified: Thu Jul  6 22:57:34 2023, max compression
+gzip compressed data, was "hspylib-setman-0.9.8.tar", last modified: Thu Jul  6 22:57:59 2023, max compression
```

## Comparing `hspylib-setman-0.9.7.tar` & `hspylib-setman-0.9.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:34.191334 hspylib-setman-0.9.7/
--rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.7/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 22:57:34.190593 hspylib-setman-0.9.7/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:34.162475 hspylib-setman-0.9.7/hspylib_setman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/hspylib_setman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 22:57:34.000000 hspylib-setman-0.9.7/hspylib_setman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/hspylib_setman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/hspylib_setman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/hspylib_setman.egg-info/top_level.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:34.170391 hspylib-setman-0.9.7/setman/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/setman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.7/setman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/setman/__init__.py
--rwxr-xr-x   0 hjunior    (504) staff       (20)     4904 2023-07-06 20:31:12.000000 hspylib-setman-0.9.7/setman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:34.178374 hspylib-setman-0.9.7/setman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/setman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7715 2023-07-06 20:30:14.000000 hspylib-setman-0.9.7/setman/core/setman.py
--rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.7/setman/core/setman_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.7/setman/core/setman_enums.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:34.189314 hspylib-setman-0.9.7/setman/settings/
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 22:57:33.000000 hspylib-setman-0.9.7/setman/settings/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     9772 2023-07-06 19:29:15.000000 hspylib-setman-0.9.7/setman/settings/settings.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.7/setman/settings/settings_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.7/setman/settings/settings_entry.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4135 2023-07-06 19:23:54.000000 hspylib-setman-0.9.7/setman/settings/settings_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2154 2023-07-06 19:24:40.000000 hspylib-setman-0.9.7/setman/settings/settings_service.py
--rw-r--r--   0 hjunior    (504) staff       (20)      232 2023-07-06 19:46:06.000000 hspylib-setman-0.9.7/setman/welcome.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 22:57:34.191463 hspylib-setman-0.9.7/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.7/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.335534 hspylib-setman-0.9.8/
+-rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.8/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 22:57:59.334661 hspylib-setman-0.9.8/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.302679 hspylib-setman-0.9.8/hspylib_setman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/top_level.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.312377 hspylib-setman-0.9.8/setman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/setman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.8/setman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/setman/__init__.py
+-rwxr-xr-x   0 hjunior    (504) staff       (20)     4904 2023-07-06 20:31:12.000000 hspylib-setman-0.9.8/setman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.320701 hspylib-setman-0.9.8/setman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/setman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7715 2023-07-06 20:30:14.000000 hspylib-setman-0.9.8/setman/core/setman.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.8/setman/core/setman_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.8/setman/core/setman_enums.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.333242 hspylib-setman-0.9.8/setman/settings/
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/setman/settings/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     9772 2023-07-06 19:29:15.000000 hspylib-setman-0.9.8/setman/settings/settings.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.8/setman/settings/settings_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.8/setman/settings/settings_entry.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4135 2023-07-06 19:23:54.000000 hspylib-setman-0.9.8/setman/settings/settings_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2154 2023-07-06 19:24:40.000000 hspylib-setman-0.9.8/setman/settings/settings_service.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      232 2023-07-06 19:46:06.000000 hspylib-setman-0.9.8/setman/welcome.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 22:57:59.335710 hspylib-setman-0.9.8/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.8/setup.py
```

### Comparing `hspylib-setman-0.9.7/PKG-INFO` & `hspylib-setman-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.7
+Version: 0.9.8
 Summary: HsPyLib - Settings Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-setman/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.7/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.7/README.md` & `hspylib-setman-0.9.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.7/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.7/hspylib_setman.egg-info/PKG-INFO` & `hspylib-setman-0.9.8/hspylib_setman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.7
+Version: 0.9.8
 Summary: HsPyLib - Settings Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-setman/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.7/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.7/hspylib_setman.egg-info/SOURCES.txt` & `hspylib-setman-0.9.8/hspylib_setman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/__classpath__.py` & `hspylib-setman-0.9.8/setman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/__main__.py` & `hspylib-setman-0.9.8/setman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/core/setman.py` & `hspylib-setman-0.9.8/setman/core/setman.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/core/setman_config.py` & `hspylib-setman-0.9.8/setman/core/setman_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/core/setman_enums.py` & `hspylib-setman-0.9.8/setman/core/setman_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/settings/settings.py` & `hspylib-setman-0.9.8/setman/settings/settings.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/settings/settings_config.py` & `hspylib-setman-0.9.8/setman/settings/settings_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/settings/settings_entry.py` & `hspylib-setman-0.9.8/setman/settings/settings_entry.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/settings/settings_repository.py` & `hspylib-setman-0.9.8/setman/settings/settings_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setman/settings/settings_service.py` & `hspylib-setman-0.9.8/setman/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.7/setup.py` & `hspylib-setman-0.9.8/setup.py`

 * *Files identical despite different names*

