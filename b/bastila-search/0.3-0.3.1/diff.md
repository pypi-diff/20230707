# Comparing `tmp/bastila_search-0.3.tar.gz` & `tmp/bastila_search-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastila_search-0.3.tar", last modified: Fri Jul  7 04:17:08 2023, max compression
+gzip compressed data, was "bastila_search-0.3.1.tar", last modified: Fri Jul  7 04:21:09 2023, max compression
```

## Comparing `bastila_search-0.3.tar` & `bastila_search-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:17:08.846652 bastila_search-0.3/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.3/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 04:17:08.846652 bastila_search-0.3/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:28:42.000000 bastila_search-0.3/README.md
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:17:08.846652 bastila_search-0.3/bastila_search/
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.3/bastila_search/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     4163 2023-07-07 04:16:00.000000 bastila_search-0.3/bastila_search/bastila_search.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:17:08.846652 bastila_search-0.3/bastila_search.egg-info/
--rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      312 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.3/bastila_search.egg-info/not-zip-safe
--rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-07 04:17:08.846652 bastila_search-0.3/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)      422 2023-07-07 04:17:05.000000 bastila_search-0.3/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:21:09.317906 bastila_search-0.3.1/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.3.1/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)      287 2023-07-07 04:21:09.317906 bastila_search-0.3.1/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:28:42.000000 bastila_search-0.3.1/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:21:09.317906 bastila_search-0.3.1/bastila_search/
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.3.1/bastila_search/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     4163 2023-07-07 04:16:00.000000 bastila_search-0.3.1/bastila_search/bastila_search.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)      437 2023-07-07 04:15:04.000000 bastila_search-0.3.1/bastila_search/setup_config.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:21:09.317906 bastila_search-0.3.1/bastila_search.egg-info/
+-rw-rw-r--   0 joe       (1000) joe       (1000)      287 2023-07-07 04:21:09.000000 bastila_search-0.3.1/bastila_search.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      384 2023-07-07 04:21:09.000000 bastila_search-0.3.1/bastila_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 04:21:09.000000 bastila_search-0.3.1/bastila_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)      115 2023-07-07 04:21:09.000000 bastila_search-0.3.1/bastila_search.egg-info/entry_points.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.3.1/bastila_search.egg-info/not-zip-safe
+-rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-07 04:21:09.000000 bastila_search-0.3.1/bastila_search.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-07 04:21:09.000000 bastila_search-0.3.1/bastila_search.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-07 04:21:09.317906 bastila_search-0.3.1/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)      611 2023-07-07 04:20:59.000000 bastila_search-0.3.1/setup.py
```

### Comparing `bastila_search-0.3/LICENSE` & `bastila_search-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bastila_search-0.3/bastila_search/bastila_search.py` & `bastila_search-0.3.1/bastila_search/bastila_search.py`

 * *Files identical despite different names*

