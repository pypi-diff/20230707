# Comparing `tmp/zhei-0.0.8.tar.gz` & `tmp/zhei-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhei-0.0.8.tar", last modified: Fri Jul  7 01:16:08 2023, max compression
+gzip compressed data, was "zhei-0.0.9.tar", last modified: Fri Jul  7 01:21:32 2023, max compression
```

## Comparing `zhei-0.0.8.tar` & `zhei-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 01:16:08.661425 zhei-0.0.8/
--rw-rw-rw-   0        0        0      286 2023-07-07 01:16:08.660426 zhei-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-06-27 02:45:05.000000 zhei-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-07 01:16:08.662425 zhei-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-07-07 01:14:28.000000 zhei-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:16:08.619166 zhei-0.0.8/zhei/
--rw-rw-rw-   0        0        0       50 2023-07-07 00:15:30.000000 zhei-0.0.8/zhei/__init__.py
--rw-rw-rw-   0        0        0      782 2023-07-04 01:50:45.000000 zhei-0.0.8/zhei/intro.py
-drwxrwxrwx   0        0        0        0 2023-07-07 01:16:08.658422 zhei-0.0.8/zhei.egg-info/
--rw-rw-rw-   0        0        0      286 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       59 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-07 01:16:08.000000 zhei-0.0.8/zhei.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 01:21:32.451797 zhei-0.0.9/
+-rw-rw-rw-   0        0        0      286 2023-07-07 01:21:32.450783 zhei-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-06-27 02:45:05.000000 zhei-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-07 01:21:32.451797 zhei-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-07-07 01:21:27.000000 zhei-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:21:32.432496 zhei-0.0.9/zhei/
+-rw-rw-rw-   0        0        0       50 2023-07-07 00:15:30.000000 zhei-0.0.9/zhei/__init__.py
+-rw-rw-rw-   0        0        0      782 2023-07-04 01:50:45.000000 zhei-0.0.9/zhei/intro.py
+drwxrwxrwx   0        0        0        0 2023-07-07 01:21:32.449494 zhei-0.0.9/zhei.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-07-07 01:21:32.000000 zhei-0.0.9/zhei.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-07 01:21:32.000000 zhei-0.0.9/zhei.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       59 2023-07-07 01:21:32.000000 zhei-0.0.9/zhei.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-07-07 01:21:32.000000 zhei-0.0.9/zhei.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-07 01:21:32.000000 zhei-0.0.9/zhei.egg-info/top_level.txt
```

### Comparing `zhei-0.0.8/setup.py` & `zhei-0.0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='zhei',
-    version='0.0.8',
+    version='0.0.9',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Deep learning tools',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=['zhei'],
```

### Comparing `zhei-0.0.8/zhei/intro.py` & `zhei-0.0.9/zhei/intro.py`

 * *Files identical despite different names*

