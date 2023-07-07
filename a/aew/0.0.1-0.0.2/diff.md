# Comparing `tmp/aew-0.0.1.tar.gz` & `tmp/aew-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aew-0.0.1.tar", last modified: Fri Jul  7 02:59:32 2023, max compression
+gzip compressed data, was "aew-0.0.2.tar", last modified: Fri Jul  7 18:50:37 2023, max compression
```

## Comparing `aew-0.0.1.tar` & `aew-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:59:32.050656 aew-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 02:59:23.000000 aew-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-07 02:59:32.050656 aew-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-07 02:59:23.000000 aew-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:59:32.050656 aew-0.0.1/aew/
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-07 02:59:23.000000 aew-0.0.1/aew/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:59:32.050656 aew-0.0.1/aew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-07 02:59:31.000000 aew-0.0.1/aew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 02:59:32.000000 aew-0.0.1/aew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:59:31.000000 aew-0.0.1/aew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 02:59:31.000000 aew-0.0.1/aew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 02:59:31.000000 aew-0.0.1/aew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:59:32.050656 aew-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 02:59:23.000000 aew-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:50:37.633098 aew-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 18:50:28.000000 aew-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-07 18:50:37.633098 aew-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-07 18:50:28.000000 aew-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:50:37.633098 aew-0.0.2/aew/
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-07 18:50:28.000000 aew-0.0.2/aew/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:50:37.633098 aew-0.0.2/aew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-07 18:50:37.000000 aew-0.0.2/aew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 18:50:37.000000 aew-0.0.2/aew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:50:37.000000 aew-0.0.2/aew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 18:50:37.000000 aew-0.0.2/aew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-07 18:50:37.000000 aew-0.0.2/aew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:50:37.633098 aew-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-07 18:50:28.000000 aew-0.0.2/setup.py
```

### Comparing `aew-0.0.1/LICENSE.md` & `aew-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aew-0.0.1/PKG-INFO` & `aew-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aew
-Version: 0.0.1
+Version: 0.0.2
 Home-page: http://github.com/csm10495/aew
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
```

### Comparing `aew-0.0.1/README.md` & `aew-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aew-0.0.1/aew/__init__.py` & `aew-0.0.2/aew/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import functools
+import logging
 import re
 from dataclasses import dataclass
 
 import requests
 from bs4 import BeautifulSoup
 from dateutil.parser import parse as dateutil_parse
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 URL = "https://www.allelitewrestling.com/blog"
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class Post:
     url: str
     title: str
     image_url: str
     aew: "AEW"
@@ -76,21 +79,24 @@
         """
         result = self.session.get(url)
         result.raise_for_status()
         return BeautifulSoup(result.text, "html.parser")
 
     def _get_title_from_url(self, url: str) -> str:
         """
-        GETs the given URL and returns the post title via the class: blog-post-title-font
+        GETs the given URL and returns the post title via the class: blog-post-title-font.
+        If that fails, use the end of the URL
         """
         soup = self.get(url)
         for element in soup.find_all("span", {"class": "blog-post-title-font"}):
             return element.text
 
-        raise ValueError(f"Could not find title for {url}")
+        logger.warning(f"Could not find title for {url} in content")
+
+        return url.split("/")[-1].replace("-", " ").title().replace("Aew", "AEW")
 
     def _resize_image_url_to_16x9(self, image_url: str) -> str:
         """
         Example: https://static.wixstatic.com/media/815952_0d4b056ce8504b21baa6d6982641943e~mv2.jpg/v1/fill/w_454,h_341,fp_0.50_0.50,q_90,enc_auto/815952_0d4b056ce8504b21baa6d6982641943e~mv2.jpg
 
         We change w_X,h_Y to w_1920,h_1080
         """
```

### Comparing `aew-0.0.1/aew.egg-info/PKG-INFO` & `aew-0.0.2/aew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aew
-Version: 0.0.1
+Version: 0.0.2
 Home-page: http://github.com/csm10495/aew
 Author: csm10495
 Author-email: csm10495@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
```

### Comparing `aew-0.0.1/setup.py` & `aew-0.0.2/setup.py`

 * *Files identical despite different names*

