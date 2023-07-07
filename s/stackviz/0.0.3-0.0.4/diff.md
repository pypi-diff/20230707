# Comparing `tmp/stackviz-0.0.3.tar.gz` & `tmp/stackviz-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackviz-0.0.3.tar", last modified: Fri Jul  7 14:00:20 2023, max compression
+gzip compressed data, was "stackviz-0.0.4.tar", last modified: Fri Jul  7 14:10:21 2023, max compression
```

## Comparing `stackviz-0.0.3.tar` & `stackviz-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:00:20.342846 stackviz-0.0.3/
--rw-r--r--   0 youhaolin   (501) staff       (20)     1069 2023-06-20 12:22:00.000000 stackviz-0.0.3/LICENSE
--rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:00:20.342719 stackviz-0.0.3/PKG-INFO
--rw-r--r--   0 youhaolin   (501) staff       (20)       84 2023-06-20 12:22:00.000000 stackviz-0.0.3/README.md
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:00:20.341937 stackviz-0.0.3/display/
--rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 12:18:19.000000 stackviz-0.0.3/display/__init__.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     1313 2023-07-07 13:47:02.000000 stackviz-0.0.3/display/chart.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     1110 2023-07-07 13:23:20.000000 stackviz-0.0.3/display/layout.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     2110 2023-07-07 13:49:21.000000 stackviz-0.0.3/display/stack.py
--rw-r--r--   0 youhaolin   (501) staff       (20)       38 2023-07-07 14:00:20.342892 stackviz-0.0.3/setup.cfg
--rw-r--r--   0 youhaolin   (501) staff       (20)      380 2023-07-07 13:51:17.000000 stackviz-0.0.3/setup.py
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:00:20.342525 stackviz-0.0.3/stackviz.egg-info/
--rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/PKG-INFO
--rw-r--r--   0 youhaolin   (501) staff       (20)      257 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/SOURCES.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        1 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/dependency_links.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/requires.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/top_level.txt
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:10:21.604970 stackviz-0.0.4/
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1069 2023-06-20 12:22:00.000000 stackviz-0.0.4/LICENSE
+-rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:10:21.604845 stackviz-0.0.4/PKG-INFO
+-rw-r--r--   0 youhaolin   (501) staff       (20)       84 2023-06-20 12:22:00.000000 stackviz-0.0.4/README.md
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:10:21.604091 stackviz-0.0.4/display/
+-rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 12:18:19.000000 stackviz-0.0.4/display/__init__.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1313 2023-07-07 13:47:02.000000 stackviz-0.0.4/display/chart.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1110 2023-07-07 13:23:20.000000 stackviz-0.0.4/display/layout.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     2110 2023-07-07 13:49:21.000000 stackviz-0.0.4/display/stack.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)       38 2023-07-07 14:10:21.605015 stackviz-0.0.4/setup.cfg
+-rw-r--r--   0 youhaolin   (501) staff       (20)      380 2023-07-07 14:10:19.000000 stackviz-0.0.4/setup.py
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:10:21.604657 stackviz-0.0.4/stackviz.egg-info/
+-rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:10:21.000000 stackviz-0.0.4/stackviz.egg-info/PKG-INFO
+-rw-r--r--   0 youhaolin   (501) staff       (20)      257 2023-07-07 14:10:21.000000 stackviz-0.0.4/stackviz.egg-info/SOURCES.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        1 2023-07-07 14:10:21.000000 stackviz-0.0.4/stackviz.egg-info/dependency_links.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:10:21.000000 stackviz-0.0.4/stackviz.egg-info/requires.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:10:21.000000 stackviz-0.0.4/stackviz.egg-info/top_level.txt
```

### Comparing `stackviz-0.0.3/LICENSE` & `stackviz-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.3/display/chart.py` & `stackviz-0.0.4/display/chart.py`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.3/display/layout.py` & `stackviz-0.0.4/display/layout.py`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.3/display/stack.py` & `stackviz-0.0.4/display/stack.py`

 * *Files identical despite different names*

