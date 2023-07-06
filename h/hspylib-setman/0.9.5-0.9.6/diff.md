# Comparing `tmp/hspylib-setman-0.9.5.tar.gz` & `tmp/hspylib-setman-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-setman-0.9.5.tar", last modified: Thu Jul  6 19:42:03 2023, max compression
+gzip compressed data, was "hspylib-setman-0.9.6.tar", last modified: Thu Jul  6 19:46:30 2023, max compression
```

## Comparing `hspylib-setman-0.9.5.tar` & `hspylib-setman-0.9.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.352883 hspylib-setman-0.9.5/
--rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.5/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:42:03.351851 hspylib-setman-0.9.5/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.308306 hspylib-setman-0.9.5/hspylib_setman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 19:42:03.000000 hspylib-setman-0.9.5/hspylib_setman.egg-info/top_level.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.317112 hspylib-setman-0.9.5/setman/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/setman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.5/setman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/setman/__init__.py
--rwxr-xr-x   0 hjunior    (504) staff       (20)     4903 2023-07-06 19:32:56.000000 hspylib-setman-0.9.5/setman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.332239 hspylib-setman-0.9.5/setman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/setman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7682 2023-07-06 19:39:52.000000 hspylib-setman-0.9.5/setman/core/setman.py
--rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.5/setman/core/setman_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.5/setman/core/setman_enums.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:42:03.350606 hspylib-setman-0.9.5/setman/settings/
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 19:42:02.000000 hspylib-setman-0.9.5/setman/settings/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     9772 2023-07-06 19:29:15.000000 hspylib-setman-0.9.5/setman/settings/settings.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.5/setman/settings/settings_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.5/setman/settings/settings_entry.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4135 2023-07-06 19:23:54.000000 hspylib-setman-0.9.5/setman/settings/settings_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2154 2023-07-06 19:24:40.000000 hspylib-setman-0.9.5/setman/settings/settings_service.py
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-05 22:41:51.000000 hspylib-setman-0.9.5/setman/welcome.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 19:42:03.353009 hspylib-setman-0.9.5/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.5/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:46:30.484364 hspylib-setman-0.9.6/
+-rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.6/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:46:30.483152 hspylib-setman-0.9.6/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 19:46:29.000000 hspylib-setman-0.9.6/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:46:30.453821 hspylib-setman-0.9.6/hspylib_setman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 19:46:30.000000 hspylib-setman-0.9.6/hspylib_setman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 19:46:30.000000 hspylib-setman-0.9.6/hspylib_setman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 19:46:30.000000 hspylib-setman-0.9.6/hspylib_setman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 19:46:30.000000 hspylib-setman-0.9.6/hspylib_setman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 19:46:30.000000 hspylib-setman-0.9.6/hspylib_setman.egg-info/top_level.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:46:30.461187 hspylib-setman-0.9.6/setman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 19:46:29.000000 hspylib-setman-0.9.6/setman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.6/setman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 19:46:29.000000 hspylib-setman-0.9.6/setman/__init__.py
+-rwxr-xr-x   0 hjunior    (504) staff       (20)     4903 2023-07-06 19:32:56.000000 hspylib-setman-0.9.6/setman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:46:30.468616 hspylib-setman-0.9.6/setman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 19:46:29.000000 hspylib-setman-0.9.6/setman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7682 2023-07-06 19:39:52.000000 hspylib-setman-0.9.6/setman/core/setman.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.6/setman/core/setman_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.6/setman/core/setman_enums.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 19:46:30.481583 hspylib-setman-0.9.6/setman/settings/
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 19:46:29.000000 hspylib-setman-0.9.6/setman/settings/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     9772 2023-07-06 19:29:15.000000 hspylib-setman-0.9.6/setman/settings/settings.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.6/setman/settings/settings_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.6/setman/settings/settings_entry.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4135 2023-07-06 19:23:54.000000 hspylib-setman-0.9.6/setman/settings/settings_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2154 2023-07-06 19:24:40.000000 hspylib-setman-0.9.6/setman/settings/settings_service.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      232 2023-07-06 19:46:06.000000 hspylib-setman-0.9.6/setman/welcome.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 19:46:30.484548 hspylib-setman-0.9.6/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.6/setup.py
```

### Comparing `hspylib-setman-0.9.5/PKG-INFO` & `hspylib-setman-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.5
+Version: 0.9.6
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
-[![Release](https://badgen.net/badge/release/v0.9.5/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.6/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.5/README.md` & `hspylib-setman-0.9.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.5/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.6/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.5/hspylib_setman.egg-info/PKG-INFO` & `hspylib-setman-0.9.6/hspylib_setman.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.5
+Version: 0.9.6
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
-[![Release](https://badgen.net/badge/release/v0.9.5/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.6/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.5/hspylib_setman.egg-info/SOURCES.txt` & `hspylib-setman-0.9.6/hspylib_setman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/__classpath__.py` & `hspylib-setman-0.9.6/setman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/__main__.py` & `hspylib-setman-0.9.6/setman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/core/setman.py` & `hspylib-setman-0.9.6/setman/core/setman.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/core/setman_config.py` & `hspylib-setman-0.9.6/setman/core/setman_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/core/setman_enums.py` & `hspylib-setman-0.9.6/setman/core/setman_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/settings/settings.py` & `hspylib-setman-0.9.6/setman/settings/settings.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/settings/settings_config.py` & `hspylib-setman-0.9.6/setman/settings/settings_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/settings/settings_entry.py` & `hspylib-setman-0.9.6/setman/settings/settings_entry.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/settings/settings_repository.py` & `hspylib-setman-0.9.6/setman/settings/settings_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setman/settings/settings_service.py` & `hspylib-setman-0.9.6/setman/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.5/setup.py` & `hspylib-setman-0.9.6/setup.py`

 * *Files identical despite different names*

