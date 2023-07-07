# Comparing `tmp/bastila_search-0.2.tar.gz` & `tmp/bastila_search-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastila_search-0.2.tar", last modified: Fri Jul  7 04:07:37 2023, max compression
+gzip compressed data, was "bastila_search-0.3.tar", last modified: Fri Jul  7 04:17:08 2023, max compression
```

## Comparing `bastila_search-0.2.tar` & `bastila_search-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:07:37.770243 bastila_search-0.2/
--rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.2/LICENSE
--rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 04:07:37.770243 bastila_search-0.2/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:28:42.000000 bastila_search-0.2/README.md
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:07:37.770243 bastila_search-0.2/bastila_search/
--rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.2/bastila_search/__init__.py
--rw-rw-r--   0 joe       (1000) joe       (1000)     4050 2023-07-07 04:06:51.000000 bastila_search-0.2/bastila_search/bastila_search.py
-drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:07:37.770243 bastila_search-0.2/bastila_search.egg-info/
--rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/PKG-INFO
--rw-rw-r--   0 joe       (1000) joe       (1000)      312 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/SOURCES.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/dependency_links.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.2/bastila_search.egg-info/not-zip-safe
--rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/requires.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-07 04:07:37.000000 bastila_search-0.2/bastila_search.egg-info/top_level.txt
--rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-07 04:07:37.770243 bastila_search-0.2/setup.cfg
--rw-rw-r--   0 joe       (1000) joe       (1000)      422 2023-07-07 04:07:07.000000 bastila_search-0.2/setup.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:17:08.846652 bastila_search-0.3/
+-rw-rw-r--   0 joe       (1000) joe       (1000)     1064 2023-07-07 03:39:14.000000 bastila_search-0.3/LICENSE
+-rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 04:17:08.846652 bastila_search-0.3/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:28:42.000000 bastila_search-0.3/README.md
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:17:08.846652 bastila_search-0.3/bastila_search/
+-rw-rw-r--   0 joe       (1000) joe       (1000)        0 2023-07-07 03:29:31.000000 bastila_search-0.3/bastila_search/__init__.py
+-rw-rw-r--   0 joe       (1000) joe       (1000)     4163 2023-07-07 04:16:00.000000 bastila_search-0.3/bastila_search/bastila_search.py
+drwxrwxr-x   0 joe       (1000) joe       (1000)        0 2023-07-07 04:17:08.846652 bastila_search-0.3/bastila_search.egg-info/
+-rw-rw-r--   0 joe       (1000) joe       (1000)      285 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/PKG-INFO
+-rw-rw-r--   0 joe       (1000) joe       (1000)      312 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)        1 2023-07-07 03:41:59.000000 bastila_search-0.3/bastila_search.egg-info/not-zip-safe
+-rw-rw-r--   0 joe       (1000) joe       (1000)        9 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/requires.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       15 2023-07-07 04:17:08.000000 bastila_search-0.3/bastila_search.egg-info/top_level.txt
+-rw-rw-r--   0 joe       (1000) joe       (1000)       38 2023-07-07 04:17:08.846652 bastila_search-0.3/setup.cfg
+-rw-rw-r--   0 joe       (1000) joe       (1000)      422 2023-07-07 04:17:05.000000 bastila_search-0.3/setup.py
```

### Comparing `bastila_search-0.2/LICENSE` & `bastila_search-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bastila_search-0.2/bastila_search/bastila_search.py` & `bastila_search-0.3/bastila_search/bastila_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 import re
 from pathlib import Path
 import sys
 import os
 
 base_url = 'https://bastila.dev'
 
+def load_config():
+    try:
+        with open("config.json", "r") as file:
+            return json.load(file)
+    except FileNotFoundError:
+        return None
+
 def fetch_patterns(session):
     response = session.get(f'{base_url}/api/check/standard-changes/')
     response.raise_for_status()
     standards = response.json()
 
     return standards['results']
 
@@ -92,17 +99,26 @@
         data=json.dumps({})
     )
     response.raise_for_status()
     return response.json()
 
 
 def main():
+    config = load_config()
+
+    if config is None:
+        print("Configuration not found. Please run setup_config.py to set up the necessary parameters.")
+        sys.exit(1)
+    else:
+        bastila_key = config["BASTILA_KEY"]
+        block_on_failure = config["BLOCK_ON_FAILURE"]
+
     session = requests.Session()
     session.headers.update({
-        'Authorization': f'Api-Key {os.getenv("BASTILA_KEY")}',
+        'Authorization': f'Api-Key {bastila_key}',
         'Content-Type': 'application/json'
     })
     print('Starting Bastila Search')
 
     try:
         check = create_check(session)
     except Exception as e:
@@ -120,36 +136,23 @@
     try:
         results = search_files(patterns)
     except Exception as e:
         sys.exit(e)
 
     print('Code Searched')
 
-    post_results_to_bastila = os.getenv('POST_RESULTS', 'false').lower() == 'true'
-
-    if post_results_to_bastila:
-        result = {
-            'check': check['id'],
-            'results': results
-        }
-        try:
-            post_results(session, result)
-        except Exception as e:
-            sys.exit(e)
-
-        print('Results Saved')
-
     is_regression = False
     for result in results:
         if not result['is_successful']:
             print(result['fix_recommendation'])
             is_regression = True
 
     if is_regression:
-        sys.exit(1)
         print('Check Failed')
+        if block_on_failure:
+            sys.exit(1)
 
     print('Success')
 
 
 if __name__ == '__main__':
     main()
```

