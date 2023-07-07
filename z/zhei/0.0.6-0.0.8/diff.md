# Comparing `tmp/zhei-0.0.6.tar.gz` & `tmp/zhei-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhei-0.0.6.tar", last modified: Thu Jul  6 02:14:53 2023, max compression
+gzip compressed data, was "zhei-0.0.8.tar", last modified: Fri Jul  7 01:16:08 2023, max compression
```

## Comparing `zhei-0.0.6.tar` & `zhei-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 02:14:53.601797 zhei-0.0.6/
--rw-rw-rw-   0        0        0      294 2023-07-06 02:14:53.601797 zhei-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-06-27 02:45:05.000000 zhei-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-06 02:14:53.602798 zhei-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-07-06 02:14:49.000000 zhei-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:14:53.571696 zhei-0.0.6/zhei/
--rw-rw-rw-   0        0        0       74 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/__init__.py
--rw-rw-rw-   0        0        0      782 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/intro.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:14:53.599798 zhei-0.0.6/zhei/utils/
--rw-rw-rw-   0        0        0      259 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/__init__.py
--rw-rw-rw-   0        0        0      674 2023-07-04 01:44:04.000000 zhei-0.0.6/zhei/utils/catch_error.py
--rw-rw-rw-   0        0        0      169 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/dataset.py
--rw-rw-rw-   0        0        0    21465 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/eval_methods.py
--rw-rw-rw-   0        0        0     8721 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/init.py
--rw-rw-rw-   0        0        0     3421 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/io.py
--rw-rw-rw-   0        0        0     5091 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/log.py
--rw-rw-rw-   0        0        0     1002 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/notice.py
--rw-rw-rw-   0        0        0     7103 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/processing_unit.py
--rw-rw-rw-   0        0        0     7054 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/redis.py
--rw-rw-rw-   0        0        0     4262 2023-07-04 01:44:04.000000 zhei-0.0.6/zhei/utils/result.py
--rw-rw-rw-   0        0        0      667 2023-07-04 01:50:45.000000 zhei-0.0.6/zhei/utils/tokenize.py
-drwxrwxrwx   0        0        0        0 2023-07-06 02:14:53.584694 zhei-0.0.6/zhei.egg-info/
--rw-rw-rw-   0        0        0      294 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       59 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-06 02:14:53.000000 zhei-0.0.6/zhei.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 01:16:08.661425 zhei-0.0.8/
+-rw-rw-rw-   0        0        0      286 2023-07-07 01:16:08.660426 zhei-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-06-27 02:45:05.000000 zhei-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 01:16:08.662425 zhei-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-07-07 01:14:28.000000 zhei-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:16:08.619166 zhei-0.0.8/zhei/
+-rw-rw-rw-   0        0        0       50 2023-07-07 00:15:30.000000 zhei-0.0.8/zhei/__init__.py
+-rw-rw-rw-   0        0        0      782 2023-07-04 01:50:45.000000 zhei-0.0.8/zhei/intro.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:16:08.658422 zhei-0.0.8/zhei.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       59 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/top_level.txt
```

### Comparing `zhei-0.0.6/zhei/intro.py` & `zhei-0.0.8/zhei/intro.py`

 * *Files identical despite different names*

