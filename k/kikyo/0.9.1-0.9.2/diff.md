# Comparing `tmp/kikyo-0.9.1.tar.gz` & `tmp/kikyo-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kikyo-0.9.1.tar", last modified: Wed Sep 29 11:01:41 2021, max compression
+gzip compressed data, was "dist/kikyo-0.9.2.tar", last modified: Thu Oct 28 08:08:09 2021, max compression
```

## Comparing `kikyo-0.9.1.tar` & `kikyo-0.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:01:41.000000 kikyo-0.9.1/
--rw-r--r--   0 jadbin     (501) staff       (20)     1063 2021-03-30 06:22:21.000000 kikyo-0.9.1/LICENSE
--rw-r--r--   0 jadbin     (501) staff       (20)      138 2021-04-25 02:34:23.000000 kikyo-0.9.1/MANIFEST.in
--rw-r--r--   0 jadbin     (501) staff       (20)      529 2021-09-29 11:01:41.000000 kikyo-0.9.1/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)       27 2021-05-24 17:10:52.000000 kikyo-0.9.1/README.rst
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo/
--rw-r--r--   0 jadbin     (501) staff       (20)      197 2021-09-29 11:00:36.000000 kikyo-0.9.1/kikyo/__init__.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo/bundle/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-08-31 12:40:49.000000 kikyo-0.9.1/kikyo/bundle/__init__.py
--rw-r--r--   0 jadbin     (501) staff       (20)      320 2021-08-31 12:41:40.000000 kikyo-0.9.1/kikyo/bundle/config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     4761 2021-09-29 11:00:52.000000 kikyo-0.9.1/kikyo/bundle/datahub.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3118 2021-06-08 02:41:53.000000 kikyo-0.9.1/kikyo/bundle/oss.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1666 2021-05-24 16:20:17.000000 kikyo-0.9.1/kikyo/bundle/search.py
--rw-r--r--   0 jadbin     (501) staff       (20)     2003 2021-09-01 02:59:43.000000 kikyo-0.9.1/kikyo/client.py
--rw-r--r--   0 jadbin     (501) staff       (20)      671 2021-09-01 02:56:25.000000 kikyo-0.9.1/kikyo/config.py
--rw-r--r--   0 jadbin     (501) staff       (20)     1795 2021-03-14 04:31:39.000000 kikyo-0.9.1/kikyo/datahub.py
--rw-r--r--   0 jadbin     (501) staff       (20)      845 2021-06-08 02:37:16.000000 kikyo-0.9.1/kikyo/oss.py
--rw-r--r--   0 jadbin     (501) staff       (20)      977 2021-04-25 02:31:21.000000 kikyo-0.9.1/kikyo/search.py
--rw-r--r--   0 jadbin     (501) staff       (20)     3007 2021-02-24 10:01:37.000000 kikyo-0.9.1/kikyo/settings.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo.egg-info/
--rw-r--r--   0 jadbin     (501) staff       (20)      529 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo.egg-info/PKG-INFO
--rw-r--r--   0 jadbin     (501) staff       (20)      512 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo.egg-info/SOURCES.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo.egg-info/dependency_links.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       52 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo.egg-info/entry_points.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        1 2021-03-12 02:47:58.000000 kikyo-0.9.1/kikyo.egg-info/not-zip-safe
--rw-r--r--   0 jadbin     (501) staff       (20)      166 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo.egg-info/requires.txt
--rw-r--r--   0 jadbin     (501) staff       (20)        6 2021-09-29 11:01:41.000000 kikyo-0.9.1/kikyo.egg-info/top_level.txt
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:01:41.000000 kikyo-0.9.1/requirements/
--rw-r--r--   0 jadbin     (501) staff       (20)       18 2021-03-30 06:22:21.000000 kikyo-0.9.1/requirements/test.txt
--rw-r--r--   0 jadbin     (501) staff       (20)       38 2021-09-29 11:01:41.000000 kikyo-0.9.1/setup.cfg
--rw-r--r--   0 jadbin     (501) staff       (20)     2110 2021-09-01 03:10:18.000000 kikyo-0.9.1/setup.py
-drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-09-29 11:01:41.000000 kikyo-0.9.1/tests/
--rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-03-30 06:22:21.000000 kikyo-0.9.1/tests/__init__.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-10-28 08:08:09.000000 kikyo-0.9.2/
+-rw-r--r--   0 jadbin     (501) staff       (20)     1063 2021-03-30 06:22:21.000000 kikyo-0.9.2/LICENSE
+-rw-r--r--   0 jadbin     (501) staff       (20)      138 2021-04-25 02:34:23.000000 kikyo-0.9.2/MANIFEST.in
+-rw-r--r--   0 jadbin     (501) staff       (20)      529 2021-10-28 08:08:09.000000 kikyo-0.9.2/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)       27 2021-05-24 17:10:52.000000 kikyo-0.9.2/README.rst
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo/
+-rw-r--r--   0 jadbin     (501) staff       (20)      197 2021-10-28 08:08:05.000000 kikyo-0.9.2/kikyo/__init__.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo/bundle/
+-rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-08-31 12:40:49.000000 kikyo-0.9.2/kikyo/bundle/__init__.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      320 2021-08-31 12:41:40.000000 kikyo-0.9.2/kikyo/bundle/config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     4761 2021-09-29 11:00:52.000000 kikyo-0.9.2/kikyo/bundle/datahub.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3118 2021-06-08 02:41:53.000000 kikyo-0.9.2/kikyo/bundle/oss.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1666 2021-05-24 16:20:17.000000 kikyo-0.9.2/kikyo/bundle/search.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     2003 2021-09-01 02:59:43.000000 kikyo-0.9.2/kikyo/client.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      671 2021-09-01 02:56:25.000000 kikyo-0.9.2/kikyo/config.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     1795 2021-03-14 04:31:39.000000 kikyo-0.9.2/kikyo/datahub.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      845 2021-06-08 02:37:16.000000 kikyo-0.9.2/kikyo/oss.py
+-rw-r--r--   0 jadbin     (501) staff       (20)      977 2021-04-25 02:31:21.000000 kikyo-0.9.2/kikyo/search.py
+-rw-r--r--   0 jadbin     (501) staff       (20)     3007 2021-02-24 10:01:37.000000 kikyo-0.9.2/kikyo/settings.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo.egg-info/
+-rw-r--r--   0 jadbin     (501) staff       (20)      529 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo.egg-info/PKG-INFO
+-rw-r--r--   0 jadbin     (501) staff       (20)      512 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo.egg-info/SOURCES.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo.egg-info/dependency_links.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       52 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo.egg-info/entry_points.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        1 2021-03-12 02:47:58.000000 kikyo-0.9.2/kikyo.egg-info/not-zip-safe
+-rw-r--r--   0 jadbin     (501) staff       (20)      133 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo.egg-info/requires.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)        6 2021-10-28 08:08:09.000000 kikyo-0.9.2/kikyo.egg-info/top_level.txt
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-10-28 08:08:09.000000 kikyo-0.9.2/requirements/
+-rw-r--r--   0 jadbin     (501) staff       (20)       18 2021-03-30 06:22:21.000000 kikyo-0.9.2/requirements/test.txt
+-rw-r--r--   0 jadbin     (501) staff       (20)       38 2021-10-28 08:08:09.000000 kikyo-0.9.2/setup.cfg
+-rw-r--r--   0 jadbin     (501) staff       (20)     2070 2021-10-28 08:07:05.000000 kikyo-0.9.2/setup.py
+drwxr-xr-x   0 jadbin     (501) staff       (20)        0 2021-10-28 08:08:09.000000 kikyo-0.9.2/tests/
+-rw-r--r--   0 jadbin     (501) staff       (20)        0 2021-03-30 06:22:21.000000 kikyo-0.9.2/tests/__init__.py
```

### Comparing `kikyo-0.9.1/LICENSE` & `kikyo-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/PKG-INFO` & `kikyo-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kikyo
-Version: 0.9.1
+Version: 0.9.2
 Summary: kikyo package
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: MIT
 Description: kikyo
         =====
```

### Comparing `kikyo-0.9.1/kikyo/bundle/datahub.py` & `kikyo-0.9.2/kikyo/bundle/datahub.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo/bundle/oss.py` & `kikyo-0.9.2/kikyo/bundle/oss.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo/bundle/search.py` & `kikyo-0.9.2/kikyo/bundle/search.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo/client.py` & `kikyo-0.9.2/kikyo/client.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo/config.py` & `kikyo-0.9.2/kikyo/config.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo/datahub.py` & `kikyo-0.9.2/kikyo/datahub.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo/oss.py` & `kikyo-0.9.2/kikyo/oss.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo/search.py` & `kikyo-0.9.2/kikyo/search.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo/settings.py` & `kikyo-0.9.2/kikyo/settings.py`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/kikyo.egg-info/PKG-INFO` & `kikyo-0.9.2/kikyo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kikyo
-Version: 0.9.1
+Version: 0.9.2
 Summary: kikyo package
 Home-page: UNKNOWN
 Author: jadbin
 Author-email: jadbin.com@hotmail.com
 License: MIT
 Description: kikyo
         =====
```

### Comparing `kikyo-0.9.1/kikyo.egg-info/SOURCES.txt` & `kikyo-0.9.2/kikyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kikyo-0.9.1/setup.py` & `kikyo-0.9.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         sys.exit(errno)
 
 
 tests_require = read_requirements('test.txt')
 install_requires = [
     'PyYAML>=5.4.1',
     'requests>=2.25.1',
-    'apache-bookkeeper-client>=4.12.1',
     'pulsar-client>=2.7.0,<2.8',
     'minio>=7.0.1,<8.0',
     'elasticsearch>=7.13.1,<7.14',
     'oss2>=2.14.0',
     'fastavro>=0.24.0',
 ]
```

