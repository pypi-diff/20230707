# Comparing `tmp/query_strings_parser-0.1.0.tar.gz` & `tmp/query_strings_parser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/query_strings_parser-0.1.0.tar", last modified: Fri Jul  7 10:13:32 2023, max compression
+gzip compressed data, was "dist/query_strings_parser-0.1.1.tar", last modified: Fri Jul  7 10:32:46 2023, max compression
```

## Comparing `query_strings_parser-0.1.0.tar` & `query_strings_parser-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:13:32.256080 query_strings_parser-0.1.0/
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)    11357 2023-07-07 10:01:52.000000 query_strings_parser-0.1.0/LICENSE
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      366 2023-07-07 10:13:32.256080 query_strings_parser-0.1.0/PKG-INFO
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)     5375 2023-07-07 10:01:52.000000 query_strings_parser-0.1.0/README.md
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      103 2023-07-07 10:13:32.256080 query_strings_parser-0.1.0/setup.cfg
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      475 2023-07-07 10:12:23.000000 query_strings_parser-0.1.0/setup.py
-drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:13:32.256080 query_strings_parser-0.1.0/src/
-drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:13:32.256080 query_strings_parser-0.1.0/src/query_strings_parser/
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:01:52.000000 query_strings_parser-0.1.0/src/query_strings_parser/__init__.py
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)     2854 2023-07-07 10:01:52.000000 query_strings_parser-0.1.0/src/query_strings_parser/query_parser.py
-drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:13:32.256080 query_strings_parser-0.1.0/src/query_strings_parser.egg-info/
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      366 2023-07-07 10:13:32.000000 query_strings_parser-0.1.0/src/query_strings_parser.egg-info/PKG-INFO
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      306 2023-07-07 10:13:32.000000 query_strings_parser-0.1.0/src/query_strings_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        1 2023-07-07 10:13:32.000000 query_strings_parser-0.1.0/src/query_strings_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)       21 2023-07-07 10:13:32.000000 query_strings_parser-0.1.0/src/query_strings_parser.egg-info/top_level.txt
+drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)    11357 2023-07-07 10:17:08.000000 query_strings_parser-0.1.1/LICENSE
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      306 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/PKG-INFO
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)     5375 2023-07-07 10:17:08.000000 query_strings_parser-0.1.1/README.md
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      103 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/setup.cfg
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      415 2023-07-07 10:32:17.000000 query_strings_parser-0.1.1/setup.py
+drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/src/
+drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/src/query_strings_parser/
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:17:08.000000 query_strings_parser-0.1.1/src/query_strings_parser/__init__.py
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)     2854 2023-07-07 10:17:08.000000 query_strings_parser-0.1.1/src/query_strings_parser/query_parser.py
+drwxrwxr-x   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        0 2023-07-07 10:32:46.517933 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      306 2023-07-07 10:32:46.000000 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)      306 2023-07-07 10:32:46.000000 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)        1 2023-07-07 10:32:46.000000 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas-barbosa  (1000) lucas-barbosa  (1000)       21 2023-07-07 10:32:46.000000 query_strings_parser-0.1.1/src/query_strings_parser.egg-info/top_level.txt
```

### Comparing `query_strings_parser-0.1.0/LICENSE` & `query_strings_parser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `query_strings_parser-0.1.0/README.md` & `query_strings_parser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `query_strings_parser-0.1.0/src/query_strings_parser/query_parser.py` & `query_strings_parser-0.1.1/src/query_strings_parser/query_parser.py`

 * *Files identical despite different names*

