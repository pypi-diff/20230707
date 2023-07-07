# Comparing `tmp/bastila_search-0.1.tar.gz` & `tmp/bastila_search-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastila_search-0.1.tar", last modified: Fri Jul  7 03:41:59 2023, max compression
+gzip compressed data, was "bastila_search-0.2.tar", last modified: Fri Jul  7 04:07:37 2023, max compression
```

## Comparing `bastila_search-0.1.tar` & `bastila_search-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 03:41:59.920571 bastila_search-0.1/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.1/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 03:41:59.920571 bastila_search-0.1/PKG-INFO
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 03:41:59.920571 bastila_search-0.1/bastila_search/
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.1/bastila_search/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     4035 2023-07-07 03:40:36.000000 bastila_search-0.1/bastila_search/bastila_search.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 03:41:59.920571 bastila_search-0.1/bastila_search.egg-info/
--rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 03:41:59.000000 bastila_search-0.1/bastila_search.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      302 2023-07-07 03:41:59.000000 bastila_search-0.1/bastila_search.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.1/bastila_search.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.1/bastila_search.egg-info/not-zip-safe
--rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-07 03:41:59.000000 bastila_search-0.1/bastila_search.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-07 03:41:59.000000 bastila_search-0.1/bastila_search.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-07 03:41:59.920571 bastila_search-0.1/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)      422 2023-07-07 03:34:39.000000 bastila_search-0.1/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:07:37.770243 bastila_search-0.2/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.2/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 04:07:37.770243 bastila_search-0.2/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:28:42.000000 bastila_search-0.2/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:07:37.770243 bastila_search-0.2/bastila_search/
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.2/bastila_search/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     4050 2023-07-07 04:06:51.000000 bastila_search-0.2/bastila_search/bastila_search.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:07:37.770243 bastila_search-0.2/bastila_search.egg-info/
+-rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      312 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.2/bastila_search.egg-info/not-zip-safe
+-rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-07 04:07:37.770243 bastila_search-0.2/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)      422 2023-07-07 04:07:07.000000 bastila_search-0.2/setup.py
```

### Comparing `bastila_search-0.1/LICENSE` & `bastila_search-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bastila_search-0.1/bastila_search/bastila_search.py` & `bastila_search-0.2/bastila_search/bastila_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 def main():
     session = requests.Session()
     session.headers.update({
         'Authorization': f'Api-Key {os.getenv("BASTILA_KEY")}',
         'Content-Type': 'application/json'
     })
-    print('Starting')
+    print('Starting Bastila Search')
 
     try:
         check = create_check(session)
     except Exception as e:
         sys.exit(e)
 
     print('Started Check')
```

