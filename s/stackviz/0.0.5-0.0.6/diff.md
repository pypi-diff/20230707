# Comparing `tmp/stackviz-0.0.5.tar.gz` & `tmp/stackviz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackviz-0.0.5.tar", last modified: Fri Jul  7 14:22:00 2023, max compression
+gzip compressed data, was "stackviz-0.0.6.tar", last modified: Fri Jul  7 14:29:17 2023, max compression
```

## Comparing `stackviz-0.0.5.tar` & `stackviz-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:22:00.410654 stackviz-0.0.5/
--rw-r--r--   0 youhaolin   (501) staff       (20)     1069 2023-06-20 12:22:00.000000 stackviz-0.0.5/LICENSE
--rw-r--r--   0 youhaolin   (501) staff       (20)       20 2023-07-07 14:21:13.000000 stackviz-0.0.5/MANIFEST.in
--rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:22:00.410502 stackviz-0.0.5/PKG-INFO
--rw-r--r--   0 youhaolin   (501) staff       (20)       84 2023-06-20 12:22:00.000000 stackviz-0.0.5/README.md
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:22:00.409238 stackviz-0.0.5/display/
--rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 12:18:19.000000 stackviz-0.0.5/display/__init__.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     1313 2023-07-07 13:47:02.000000 stackviz-0.0.5/display/chart.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     1110 2023-07-07 13:23:20.000000 stackviz-0.0.5/display/layout.py
--rw-r--r--   0 youhaolin   (501) staff       (20)     2110 2023-07-07 13:49:21.000000 stackviz-0.0.5/display/stack.py
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:22:00.409472 stackviz-0.0.5/resources/
--rw-r--r--   0 youhaolin   (501) staff       (20)      332 2023-07-07 12:17:12.000000 stackviz-0.0.5/resources/default.css
--rw-r--r--   0 youhaolin   (501) staff       (20)      417 2023-07-07 13:27:47.000000 stackviz-0.0.5/resources/template.tpl
--rw-r--r--   0 youhaolin   (501) staff       (20)       38 2023-07-07 14:22:00.410701 stackviz-0.0.5/setup.cfg
--rw-r--r--   0 youhaolin   (501) staff       (20)      443 2023-07-07 14:21:58.000000 stackviz-0.0.5/setup.py
-drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:22:00.410264 stackviz-0.0.5/stackviz.egg-info/
--rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:22:00.000000 stackviz-0.0.5/stackviz.egg-info/PKG-INFO
--rw-r--r--   0 youhaolin   (501) staff       (20)      314 2023-07-07 14:22:00.000000 stackviz-0.0.5/stackviz.egg-info/SOURCES.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        1 2023-07-07 14:22:00.000000 stackviz-0.0.5/stackviz.egg-info/dependency_links.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:22:00.000000 stackviz-0.0.5/stackviz.egg-info/requires.txt
--rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:22:00.000000 stackviz-0.0.5/stackviz.egg-info/top_level.txt
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:29:17.921863 stackviz-0.0.6/
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1069 2023-06-20 12:22:00.000000 stackviz-0.0.6/LICENSE
+-rw-r--r--   0 youhaolin   (501) staff       (20)       29 2023-07-07 14:24:44.000000 stackviz-0.0.6/MANIFEST.in
+-rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:29:17.921748 stackviz-0.0.6/PKG-INFO
+-rw-r--r--   0 youhaolin   (501) staff       (20)       84 2023-06-20 12:22:00.000000 stackviz-0.0.6/README.md
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:29:17.920266 stackviz-0.0.6/display/
+-rw-r--r--   0 youhaolin   (501) staff       (20)        0 2023-07-07 12:18:19.000000 stackviz-0.0.6/display/__init__.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1313 2023-07-07 13:47:02.000000 stackviz-0.0.6/display/chart.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     1110 2023-07-07 13:23:20.000000 stackviz-0.0.6/display/layout.py
+-rw-r--r--   0 youhaolin   (501) staff       (20)     2110 2023-07-07 13:49:21.000000 stackviz-0.0.6/display/stack.py
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:29:17.920770 stackviz-0.0.6/resources/
+-rw-r--r--   0 youhaolin   (501) staff       (20)      332 2023-07-07 12:17:12.000000 stackviz-0.0.6/resources/default.css
+-rw-r--r--   0 youhaolin   (501) staff       (20)      417 2023-07-07 13:27:47.000000 stackviz-0.0.6/resources/template.tpl
+-rw-r--r--   0 youhaolin   (501) staff       (20)       38 2023-07-07 14:29:17.921907 stackviz-0.0.6/setup.cfg
+-rw-r--r--   0 youhaolin   (501) staff       (20)      489 2023-07-07 14:29:07.000000 stackviz-0.0.6/setup.py
+drwxr-xr-x   0 youhaolin   (501) staff       (20)        0 2023-07-07 14:29:17.921524 stackviz-0.0.6/stackviz.egg-info/
+-rw-r--r--   0 youhaolin   (501) staff       (20)      254 2023-07-07 14:29:17.000000 stackviz-0.0.6/stackviz.egg-info/PKG-INFO
+-rw-r--r--   0 youhaolin   (501) staff       (20)      314 2023-07-07 14:29:17.000000 stackviz-0.0.6/stackviz.egg-info/SOURCES.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        1 2023-07-07 14:29:17.000000 stackviz-0.0.6/stackviz.egg-info/dependency_links.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:29:17.000000 stackviz-0.0.6/stackviz.egg-info/requires.txt
+-rw-r--r--   0 youhaolin   (501) staff       (20)        8 2023-07-07 14:29:17.000000 stackviz-0.0.6/stackviz.egg-info/top_level.txt
```

### Comparing `stackviz-0.0.5/LICENSE` & `stackviz-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.5/display/chart.py` & `stackviz-0.0.6/display/chart.py`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.5/display/layout.py` & `stackviz-0.0.6/display/layout.py`

 * *Files identical despite different names*

### Comparing `stackviz-0.0.5/display/stack.py` & `stackviz-0.0.6/display/stack.py`

 * *Files identical despite different names*

