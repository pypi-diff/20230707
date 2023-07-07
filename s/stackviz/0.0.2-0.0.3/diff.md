# Comparing `tmp/stackviz-0.0.2.tar.gz` & `tmp/stackviz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackviz-0.0.2.tar", last modified: Tue Jun 20 12:36:34 2023, max compression
+gzip compressed data, was "stackviz-0.0.3.tar", last modified: Fri Jul  7 14:00:20 2023, max compression
```

## Comparing `stackviz-0.0.2.tar` & `stackviz-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-06-20 12:36:34.684359 stackviz-0.0.2/
--rw-r--r--   0 youhaolin   (501) staff       (20)     1069 2023-06-20 12:22:00.000000 stackviz-0.0.2/LICENSE
--rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-06-20 12:36:34.684190 stackviz-0.0.2/PKG-INFO
--rw-r--r--   0 youhaolin   (501) staff       (20)       84 2023-06-20 12:22:00.000000 stackviz-0.0.2/README.md
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-06-20 12:36:34.683391 stackviz-0.0.2/examples/
--rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-06-20 12:27:09.000000 stackviz-0.0.2/examples/__init__.py
--rw-r--r--   0 youhaolin   (501) staff       (20)       62 2023-06-20 12:35:18.000000 stackviz-0.0.2/examples/test.py
--rw-r--r--   0 youhaolin   (501) staff       (20)       38 2023-06-20 12:36:34.684397 stackviz-0.0.2/setup.cfg
--rw-r--r--   0 youhaolin   (501) staff       (20)      397 2023-06-20 12:36:29.000000 stackviz-0.0.2/setup.py
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-06-20 12:36:34.684026 stackviz-0.0.2/stackviz.egg-info/
--rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-06-20 12:36:34.000000 stackviz-0.0.2/stackviz.egg-info/PKG-INFO
--rw-r--r--   0 youhaolin   (501) staff       (20)      223 2023-06-20 12:36:34.000000 stackviz-0.0.2/stackviz.egg-info/SOURCES.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        1 2023-06-20 12:36:34.000000 stackviz-0.0.2/stackviz.egg-info/dependency_links.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)       13 2023-06-20 12:36:34.000000 stackviz-0.0.2/stackviz.egg-info/requires.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        9 2023-06-20 12:36:34.000000 stackviz-0.0.2/stackviz.egg-info/top_level.txt
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:00:20.342846 stackviz-0.0.3/
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1069 2023-06-20 12:22:00.000000 stackviz-0.0.3/LICENSE
+-rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:00:20.342719 stackviz-0.0.3/PKG-INFO
+-rw-r--r--   0 youhaolin   (501) staff       (20)       84 2023-06-20 12:22:00.000000 stackviz-0.0.3/README.md
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:00:20.341937 stackviz-0.0.3/display/
+-rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 12:18:19.000000 stackviz-0.0.3/display/__init__.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1313 2023-07-07 13:47:02.000000 stackviz-0.0.3/display/chart.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1110 2023-07-07 13:23:20.000000 stackviz-0.0.3/display/layout.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     2110 2023-07-07 13:49:21.000000 stackviz-0.0.3/display/stack.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)       38 2023-07-07 14:00:20.342892 stackviz-0.0.3/setup.cfg
+-rw-r--r--   0 youhaolin   (501) staff       (20)      380 2023-07-07 13:51:17.000000 stackviz-0.0.3/setup.py
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:00:20.342525 stackviz-0.0.3/stackviz.egg-info/
+-rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/PKG-INFO
+-rw-r--r--   0 youhaolin   (501) staff       (20)      257 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/SOURCES.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        1 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/dependency_links.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/requires.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:00:20.000000 stackviz-0.0.3/stackviz.egg-info/top_level.txt
```

### Comparing `stackviz-0.0.2/LICENSE` & `stackviz-0.0.3/LICENSE`

 * *Files identical despite different names*

