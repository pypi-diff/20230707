# Comparing `tmp/ns_asphalt9-0.0.8.tar.gz` & `tmp/ns_asphalt9-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.0.8.tar", last modified: Wed Jul  5 10:04:44 2023, max compression
+gzip compressed data, was "ns_asphalt9-0.0.9.tar", last modified: Thu Jul  6 11:44:14 2023, max compression
```

## Comparing `ns_asphalt9-0.0.8.tar` & `ns_asphalt9-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.290847 ns_asphalt9-0.0.8/
--rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.8/LICENSE
--rw-r--r--   0 neo.sun    (502) staff       (20)      180 2023-06-30 07:35:13.000000 ns_asphalt9-0.0.8/MANIFEST.in
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-07-05 10:04:44.290941 ns_asphalt9-0.0.8/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.8/README.md
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.276636 ns_asphalt9-0.0.8/ns_asphalt9/
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.282048 ns_asphalt9-0.0.8/ns_asphalt9/core/
--rw-r--r--   0 neo.sun    (502) staff       (20)       20 2023-06-30 07:48:40.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.283440 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/
--rw-r--r--   0 neo.sun    (502) staff       (20)      222 2023-07-03 09:32:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      477 2023-07-03 09:32:06.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     4033 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3917 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3777 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      706 2023-06-28 08:30:50.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/cache.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3037 2023-07-03 02:10:16.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/consts.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     2146 2023-06-30 07:54:21.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/controller.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      634 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.285020 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/
--rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-26 05:07:57.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)    18706 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.288715 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/
--rw-r--r--   0 neo.sun    (502) staff       (20)     3097 2023-06-26 08:14:33.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     2900 2023-06-26 08:18:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 neo.sun    (502) staff       (20)   202347 2023-06-26 05:17:10.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     3159 2023-06-26 08:11:35.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     1530 2023-06-30 07:54:36.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/ocr.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1841 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 neo.sun    (502) staff       (20)    12760 2023-07-03 09:48:32.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/pages.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      265 2023-06-29 06:50:43.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     2572 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.290310 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/
--rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1016 2023-06-30 07:53:42.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      459 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1993 2023-06-30 07:53:54.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      862 2023-06-30 07:54:03.000000 ns_asphalt9-0.0.8/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     5558 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.8/ns_asphalt9/main.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.278630 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)     1187 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       54 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-07-05 10:04:44.000000 ns_asphalt9-0.0.8/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)     1299 2023-07-05 10:04:44.291709 ns_asphalt9-0.0.8/setup.cfg
--rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.8/setup.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-05 10:04:44.290585 ns_asphalt9-0.0.8/tests/
--rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.8/tests/test_ocr.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.631823 ns_asphalt9-0.0.9/
+-rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.9/LICENSE
+-rw-r--r--   0 neo.sun    (502) staff       (20)      180 2023-06-30 07:35:13.000000 ns_asphalt9-0.0.9/MANIFEST.in
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-07-06 11:44:14.631929 ns_asphalt9-0.0.9/PKG-INFO
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.9/README.md
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.621548 ns_asphalt9-0.0.9/ns_asphalt9/
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.625921 ns_asphalt9-0.0.9/ns_asphalt9/core/
+-rw-r--r--   0 neo.sun    (502) staff       (20)       20 2023-06-30 07:48:40.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.627311 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/
+-rw-r--r--   0 neo.sun    (502) staff       (20)      222 2023-07-03 09:32:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      477 2023-07-03 09:32:06.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     4033 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3917 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3777 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      706 2023-06-28 08:30:50.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/cache.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3037 2023-07-03 02:10:16.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/consts.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2146 2023-06-30 07:54:21.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/controller.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      634 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.627622 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/
+-rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-26 05:07:57.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)    18706 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.629697 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3097 2023-06-26 08:14:33.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2900 2023-06-26 08:18:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)   202347 2023-06-26 05:17:10.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     3159 2023-06-26 08:11:35.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1530 2023-06-30 07:54:36.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1841 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)    13007 2023-07-06 11:42:30.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/pages.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      265 2023-06-29 06:50:43.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2572 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.631293 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/
+-rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1016 2023-06-30 07:53:42.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      459 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1993 2023-06-30 07:53:54.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)      862 2023-06-30 07:54:03.000000 ns_asphalt9-0.0.9/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 neo.sun    (502) staff       (20)     5558 2023-07-03 02:07:26.000000 ns_asphalt9-0.0.9/ns_asphalt9/main.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.622895 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1187 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)       54 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-07-06 11:44:14.000000 ns_asphalt9-0.0.9/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1299 2023-07-06 11:44:14.632329 ns_asphalt9-0.0.9/setup.cfg
+-rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.9/setup.py
+drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-07-06 11:44:14.631577 ns_asphalt9-0.0.9/tests/
+-rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.9/tests/test_ocr.py
```

### Comparing `ns_asphalt9-0.0.8/LICENSE` & `ns_asphalt9-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/PKG-INFO` & `ns_asphalt9-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.0.8
+Version: 0.0.9
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.0.8/README.md` & `ns_asphalt9-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/actions/enter_page.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/actions/enter_page.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/actions/process_race.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/actions/select_car.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/consts.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/globals.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/globals.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/app.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.0.9/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/page_factory.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,25 +336,14 @@
     part_match = False
 
     action = staticmethod(pro.press_button)
     args = (Buttons.B,)
 
 
 @cache_decorator("page")
-class VipReward(Page):
-    """通行证任务完成"""
-
-    name = consts.vip_reward
-    feature = "TIER"
-    part_match = False
-    action = staticmethod(pro.press_button)
-    args = (Buttons.B,)
-
-
-@cache_decorator("page")
 class RaceResults(Page):
     """比赛结果"""
 
     name = consts.race_results
     feature = "RACE RESULTS|POS\.|PLAYER|CAR NAME|NEXT"
     part_match = True
     action = staticmethod(pro.press_button)
@@ -559,7 +548,27 @@
 @cache_decorator("page")
 class LegendPass(Page):
     """通行证页"""
 
     name = consts.legend_pass
     feature = "ENDS IN|CURRENT TIER|GARAGE|GRANTS UP TO"
     part_match = True
+
+
+@cache_decorator("page")
+class VipReward(Page):
+    """通行证任务完成"""
+
+    name = consts.vip_reward
+    feature = "TIER"
+    part_match = False
+    action = staticmethod(pro.press_button)
+    args = (Buttons.B,)
+
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if "ENDS IN" in text:
+            match_count = 0
+        else:
+            match_count = 10
+        return match_count
```

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/tasks.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.0.9/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9/main.py` & `ns_asphalt9-0.0.9/ns_asphalt9/main.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.0.9/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.0.8
+Version: 0.0.9
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
```

### Comparing `ns_asphalt9-0.0.8/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.0.9/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.8/setup.cfg` & `ns_asphalt9-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.0.8
+version = 0.0.9
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

### Comparing `ns_asphalt9-0.0.8/tests/test_ocr.py` & `ns_asphalt9-0.0.9/tests/test_ocr.py`

 * *Files identical despite different names*

