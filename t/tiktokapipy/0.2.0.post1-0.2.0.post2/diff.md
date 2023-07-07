# Comparing `tmp/tiktokapipy-0.2.0.post1.tar.gz` & `tmp/tiktokapipy-0.2.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktokapipy-0.2.0.post1.tar", last modified: Wed Jul  5 20:42:47 2023, max compression
+gzip compressed data, was "tiktokapipy-0.2.0.post2.tar", last modified: Fri Jul  7 13:48:51 2023, max compression
```

## Comparing `tiktokapipy-0.2.0.post1.tar` & `tiktokapipy-0.2.0.post2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:47.806973 tiktokapipy-0.2.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-05 20:42:47.806973 tiktokapipy-0.2.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:42:47.806973 tiktokapipy-0.2.0.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:47.802973 tiktokapipy-0.2.0.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:47.802973 tiktokapipy-0.2.0.post1/src/tiktokapipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/async_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:47.806973 tiktokapipy-0.2.0.post1/src/tiktokapipy/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/models/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/models/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/models/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:47.806973 tiktokapipy-0.2.0.post1/src/tiktokapipy/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/util/deferred_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/util/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy/util/signing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:47.802973 tiktokapipy-0.2.0.post1/src/tiktokapipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-05 20:42:47.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-05 20:42:47.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:42:47.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-05 20:42:47.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 20:42:47.000000 tiktokapipy-0.2.0.post1/src/tiktokapipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:47.806973 tiktokapipy-0.2.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/tests/test_challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/tests/test_slideshow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-05 20:42:37.000000 tiktokapipy-0.2.0.post1/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.773075 tiktokapipy-0.2.0.post2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/src/tiktokapipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/async_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/models/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/deferred_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52530 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy/util/signing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 13:48:51.000000 tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:48:51.777075 tiktokapipy-0.2.0.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_slideshow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-07 13:48:34.000000 tiktokapipy-0.2.0.post2/tests/test_video.py
```

### Comparing `tiktokapipy-0.2.0.post1/LICENSE` & `tiktokapipy-0.2.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/PKG-INFO` & `tiktokapipy-0.2.0.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.2.0.post1
+Version: 0.2.0.post2
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.0.post1 Summary: Asyncio
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.0.post2 Summary: Asyncio
 TikTok data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
```

### Comparing `tiktokapipy-0.2.0.post1/README.md` & `tiktokapipy-0.2.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/pyproject.toml` & `tiktokapipy-0.2.0.post2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tiktokapipy"
-version = "0.2.0post1"
+version = "0.2.0post2"
 authors = [
     { name="Russell Newton", email="russell.newton01@gmail.com" },
 ]
 description = "Asyncio TikTok data scraping tool"
 readme = "README.md"
 requires-python = ">=3.8"
 
@@ -28,15 +28,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Games/Entertainment",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 dependencies = [
     "playwright~=1.29",
-    "pydantic",
+    "pydantic>=2",
     "requests",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
```

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/__init__.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/api.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/api.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/async_api.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/async_api.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/models/__init__.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/models/challenge.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/models/comment.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/comment.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/models/raw_data.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/raw_data.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/models/user.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/models/video.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/models/video.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/util/deferred_collectors.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/util/deferred_collectors.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/util/queries.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/util/queries.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy/util/signing.py` & `tiktokapipy-0.2.0.post2/src/tiktokapipy/util/signing.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy.egg-info/PKG-INFO` & `tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiktokapipy
-Version: 0.2.0.post1
+Version: 0.2.0.post2
 Summary: Asyncio TikTok data scraping tool
 Author-email: Russell Newton <russell.newton01@gmail.com>
 Project-URL: Homepage, https://github.com/Russell-Newton/TikTokPy
 Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok scraper,asyncio,playwright-python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.0.post1 Summary: Asyncio
+Metadata-Version: 2.1 Name: tiktokapipy Version: 0.2.0.post2 Summary: Asyncio
 TikTok data scraping tool Author-email: Russell Newton
 newton01@gmail.com> Project-URL: Homepage, https://github.com/Russell-Newton/
 TikTokPy Project-URL: Documentation, https://tiktokpy.readthedocs.io/en/latest/
 Keywords: tiktok,python3,scraper,unofficial,tiktok-scraper,tiktok
 scraper,asyncio,playwright-python Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
```

### Comparing `tiktokapipy-0.2.0.post1/src/tiktokapipy.egg-info/SOURCES.txt` & `tiktokapipy-0.2.0.post2/src/tiktokapipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/tests/test_challenge.py` & `tiktokapipy-0.2.0.post2/tests/test_challenge.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/tests/test_slideshow.py` & `tiktokapipy-0.2.0.post2/tests/test_slideshow.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/tests/test_user.py` & `tiktokapipy-0.2.0.post2/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `tiktokapipy-0.2.0.post1/tests/test_video.py` & `tiktokapipy-0.2.0.post2/tests/test_video.py`

 * *Files identical despite different names*

