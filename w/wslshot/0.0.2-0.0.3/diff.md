# Comparing `tmp/wslshot-0.0.2.tar.gz` & `tmp/wslshot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wslshot-0.0.2.tar", last modified: Fri Jul  7 18:47:38 2023, max compression
+gzip compressed data, was "wslshot-0.0.3.tar", last modified: Fri Jul  7 18:51:25 2023, max compression
```

## Comparing `wslshot-0.0.2.tar` & `wslshot-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:47:38.066512 wslshot-0.0.2/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-07-07 11:34:57.000000 wslshot-0.0.2/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6709 2023-07-07 18:47:38.066512 wslshot-0.0.2/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6269 2023-07-07 18:35:06.000000 wslshot-0.0.2/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-07 18:47:38.066512 wslshot-0.0.2/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      990 2023-07-07 18:47:19.000000 wslshot-0.0.2/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:47:38.066512 wslshot-0.0.2/wslshot/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 12:41:35.000000 wslshot-0.0.2/wslshot/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15400 2023-07-07 18:28:37.000000 wslshot-0.0.2/wslshot/cli.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:47:38.066512 wslshot-0.0.2/wslshot.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6709 2023-07-07 18:47:38.000000 wslshot-0.0.2/wslshot.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      249 2023-07-07 18:47:38.000000 wslshot-0.0.2/wslshot.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-07 18:47:38.000000 wslshot-0.0.2/wslshot.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       48 2023-07-07 18:47:38.000000 wslshot-0.0.2/wslshot.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        6 2023-07-07 18:47:38.000000 wslshot-0.0.2/wslshot.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-07-07 18:47:38.000000 wslshot-0.0.2/wslshot.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:51:25.766511 wslshot-0.0.3/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-07-07 11:34:57.000000 wslshot-0.0.3/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6709 2023-07-07 18:51:25.766511 wslshot-0.0.3/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6269 2023-07-07 18:35:06.000000 wslshot-0.0.3/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-07-07 18:51:25.766511 wslshot-0.0.3/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      990 2023-07-07 18:50:11.000000 wslshot-0.0.3/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:51:25.766511 wslshot-0.0.3/wslshot/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 12:41:35.000000 wslshot-0.0.3/wslshot/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    15377 2023-07-07 18:50:02.000000 wslshot-0.0.3/wslshot/cli.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-07-07 18:51:25.766511 wslshot-0.0.3/wslshot.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     6709 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      249 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       48 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        6 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2023-07-07 18:51:25.000000 wslshot-0.0.3/wslshot.egg-info/top_level.txt
```

### Comparing `wslshot-0.0.2/LICENSE` & `wslshot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wslshot-0.0.2/PKG-INFO` & `wslshot-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslshot
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/sderev/wslshot
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/wslshot
 Project-URL: Issues, http://github.com/sderev/wslshot/issues
 Project-URL: Changelog, https://github.com/sderev/wslshot/releases
 Requires-Python: >=3.8
```

### Comparing `wslshot-0.0.2/README.md` & `wslshot-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wslshot-0.0.2/setup.py` & `wslshot-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

### Comparing `wslshot-0.0.2/wslshot/cli.py` & `wslshot-0.0.3/wslshot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,14 @@
 
     - source: The source directory.
     - destination: The destination directory.
     - count: The number of screenshots to fetch.
     """
     copied_screenshots = ()
 
-    print(screenshots)
     for idx, screenshot in enumerate(screenshots):
         new_screenshot_name = rename_screenshot(idx)
         new_screenshot_path = Path(destination) / new_screenshot_name
         shutil.copy(screenshot, new_screenshot_path)
         copied_screenshots += (Path(destination) / new_screenshot_name,)
 
     return copied_screenshots
```

### Comparing `wslshot-0.0.2/wslshot.egg-info/PKG-INFO` & `wslshot-0.0.3/wslshot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wslshot
-Version: 0.0.2
+Version: 0.0.3
 Home-page: https://github.com/sderev/wslshot
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/wslshot
 Project-URL: Issues, http://github.com/sderev/wslshot/issues
 Project-URL: Changelog, https://github.com/sderev/wslshot/releases
 Requires-Python: >=3.8
```

