# Comparing `tmp/hspylib-hqt-0.9.5.tar.gz` & `tmp/hspylib-hqt-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-hqt-0.9.5.tar", last modified: Mon Jul  3 20:37:26 2023, max compression
+gzip compressed data, was "hspylib-hqt-0.9.6.tar", last modified: Fri Jul  7 18:29:13 2023, max compression
```

## Comparing `hspylib-hqt-0.9.5.tar` & `hspylib-hqt-0.9.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:37:26.621044 hspylib-hqt-0.9.5/
--rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.5/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-03 20:37:26.620251 hspylib-hqt-0.9.5/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)    11082 2023-07-03 20:37:25.000000 hspylib-hqt-0.9.5/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:37:26.581858 hspylib-hqt-0.9.5/hqt/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-03 20:37:25.000000 hspylib-hqt-0.9.5/hqt/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      198 2023-07-03 20:37:25.000000 hspylib-hqt-0.9.5/hqt/__init__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:37:26.603287 hspylib-hqt-0.9.5/hqt/promotions/
--rw-r--r--   0 hjunior    (504) staff       (20)      284 2023-07-03 20:37:25.000000 hspylib-hqt-0.9.5/hqt/promotions/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      838 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/promotions/hcombobox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7680 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/promotions/hconsole.py
--rw-r--r--   0 hjunior    (504) staff       (20)      667 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/promotions/hframe.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2570 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/promotions/hlabel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6562 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/promotions/hlistwidget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4414 2023-07-03 20:34:28.000000 hspylib-hqt-0.9.5/hqt/promotions/hstacked_widget.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6227 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/promotions/htablemodel.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5448 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/promotions/htableview.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6283 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/promotions/htoolbox.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2592 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/qt_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3854 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/stream_capturer.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:37:26.610556 hspylib-hqt-0.9.5/hqt/views/
--rw-r--r--   0 hjunior    (504) staff       (20)      162 2023-07-03 20:37:25.000000 hspylib-hqt-0.9.5/hqt/views/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      862 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/views/main_view.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2313 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.5/hqt/views/qt_view.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-03 20:37:26.618879 hspylib-hqt-0.9.5/hspylib_hqt.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-03 20:37:26.000000 hspylib-hqt-0.9.5/hspylib_hqt.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-07-03 20:37:26.000000 hspylib-hqt-0.9.5/hspylib_hqt.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-03 20:37:26.000000 hspylib-hqt-0.9.5/hspylib_hqt.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       26 2023-07-03 20:37:26.000000 hspylib-hqt-0.9.5/hspylib_hqt.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-07-03 20:37:26.000000 hspylib-hqt-0.9.5/hspylib_hqt.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-03 20:37:26.621163 hspylib-hqt-0.9.5/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2071 2023-04-19 22:12:01.000000 hspylib-hqt-0.9.5/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:29:13.781056 hspylib-hqt-0.9.6/
+-rw-r--r--   0 hjunior    (504) staff       (20)       21 2023-04-18 22:21:01.000000 hspylib-hqt-0.9.6/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-07 18:29:13.780090 hspylib-hqt-0.9.6/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)    11082 2023-07-07 18:29:12.000000 hspylib-hqt-0.9.6/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:29:13.742682 hspylib-hqt-0.9.6/hqt/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-07 18:29:12.000000 hspylib-hqt-0.9.6/hqt/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      198 2023-07-07 18:29:12.000000 hspylib-hqt-0.9.6/hqt/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:29:13.762609 hspylib-hqt-0.9.6/hqt/promotions/
+-rw-r--r--   0 hjunior    (504) staff       (20)      284 2023-07-07 18:29:12.000000 hspylib-hqt-0.9.6/hqt/promotions/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      838 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/promotions/hcombobox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7680 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/promotions/hconsole.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      667 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/promotions/hframe.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2570 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/promotions/hlabel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6562 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/promotions/hlistwidget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4414 2023-07-07 18:23:24.000000 hspylib-hqt-0.9.6/hqt/promotions/hstacked_widget.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6227 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/promotions/htablemodel.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5448 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/promotions/htableview.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6283 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/promotions/htoolbox.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2592 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/qt_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3854 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/stream_capturer.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:29:13.770212 hspylib-hqt-0.9.6/hqt/views/
+-rw-r--r--   0 hjunior    (504) staff       (20)      162 2023-07-07 18:29:12.000000 hspylib-hqt-0.9.6/hqt/views/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      862 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/views/main_view.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2313 2023-04-19 23:04:53.000000 hspylib-hqt-0.9.6/hqt/views/qt_view.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:29:13.778476 hspylib-hqt-0.9.6/hspylib_hqt.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)    12094 2023-07-07 18:29:13.000000 hspylib-hqt-0.9.6/hspylib_hqt.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      626 2023-07-07 18:29:13.000000 hspylib-hqt-0.9.6/hspylib_hqt.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-07 18:29:13.000000 hspylib-hqt-0.9.6/hspylib_hqt.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       26 2023-07-07 18:29:13.000000 hspylib-hqt-0.9.6/hspylib_hqt.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        4 2023-07-07 18:29:13.000000 hspylib-hqt-0.9.6/hspylib_hqt.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-07 18:29:13.781178 hspylib-hqt-0.9.6/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2071 2023-04-19 22:12:01.000000 hspylib-hqt-0.9.6/setup.py
```

### Comparing `hspylib-hqt-0.9.5/PKG-INFO` & `hspylib-hqt-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-hqt
-Version: 0.9.5
+Version: 0.9.6
 Summary: HsPyLib - QT framework extensions
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.5/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.6/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
```

### Comparing `hspylib-hqt-0.9.5/README.md` & `hspylib-hqt-0.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.5/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.6/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
```

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/hcombobox.py` & `hspylib-hqt-0.9.6/hqt/promotions/hcombobox.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/hconsole.py` & `hspylib-hqt-0.9.6/hqt/promotions/hconsole.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/hframe.py` & `hspylib-hqt-0.9.6/hqt/promotions/hframe.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/hlabel.py` & `hspylib-hqt-0.9.6/hqt/promotions/hlabel.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/hlistwidget.py` & `hspylib-hqt-0.9.6/hqt/promotions/hlistwidget.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/hstacked_widget.py` & `hspylib-hqt-0.9.6/hqt/promotions/hstacked_widget.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/htablemodel.py` & `hspylib-hqt-0.9.6/hqt/promotions/htablemodel.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/htableview.py` & `hspylib-hqt-0.9.6/hqt/promotions/htableview.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/promotions/htoolbox.py` & `hspylib-hqt-0.9.6/hqt/promotions/htoolbox.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/qt_application.py` & `hspylib-hqt-0.9.6/hqt/qt_application.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/stream_capturer.py` & `hspylib-hqt-0.9.6/hqt/stream_capturer.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/views/main_view.py` & `hspylib-hqt-0.9.6/hqt/views/main_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hqt/views/qt_view.py` & `hspylib-hqt-0.9.6/hqt/views/qt_view.py`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/hspylib_hqt.egg-info/PKG-INFO` & `hspylib-hqt-0.9.6/hspylib_hqt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-hqt
-Version: 0.9.5
+Version: 0.9.6
 Summary: HsPyLib - QT framework extensions
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-hqt/
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 
 # <img src="https://iili.io/HYBJFA7.png"  width="34" height="34"> HomeSetup Python Library - HsPyLib
 
 ## Your Python code is not JUST a script !!
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.5/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.6/gray)](docs/CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 
 HsPyLib is a Python library that will elevate your experience to another level. It relies on well known principles as
 SOLID, DRY (Don't Repeat Yourself), KISS (Keep It Simple, Stupid) and YAGNI (You Ain’t Gonna Need It). It provides many
```

### Comparing `hspylib-hqt-0.9.5/hspylib_hqt.egg-info/SOURCES.txt` & `hspylib-hqt-0.9.6/hspylib_hqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-hqt-0.9.5/setup.py` & `hspylib-hqt-0.9.6/setup.py`

 * *Files identical despite different names*

